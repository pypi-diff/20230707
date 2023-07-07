# Comparing `tmp/cikuu-2022.8.8.tar.gz` & `tmp/cikuu-2022.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cikuu-2022.8.8.tar", last modified: Sun Jul  2 10:24:49 2023, max compression
+gzip compressed data, was "cikuu-2022.8.9.tar", last modified: Fri Jul  7 10:48:16 2023, max compression
```

## Comparing `cikuu-2022.8.8.tar` & `cikuu-2022.8.9.tar`

### file list

```diff
@@ -1,384 +1,386 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.678426 cikuu-2022.8.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-03-04 12:51:34.000000 cikuu-2022.8.8/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-07-02 10:24:49.678426 cikuu-2022.8.8/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.590426 cikuu-2022.8.8/api/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-03-04 12:49:43.000000 cikuu-2022.8.8/api/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2086 2023-03-04 12:49:43.000000 cikuu-2022.8.8/api/c4.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1236 2023-03-04 12:49:46.000000 cikuu-2022.8.8/api/chunk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1399 2023-03-04 12:49:49.000000 cikuu-2022.8.8/api/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2023-03-04 12:49:43.000000 cikuu-2022.8.8/api/dm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21647 2023-03-04 12:49:44.000000 cikuu-2022.8.8/api/es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-03-04 12:49:46.000000 cikuu-2022.8.8/api/feishu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-03-04 12:49:49.000000 cikuu-2022.8.8/api/mynac.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2023-03-04 12:49:44.000000 cikuu-2022.8.8/api/sntjson-es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-03-04 12:49:44.000000 cikuu-2022.8.8/api/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1333 2023-03-04 12:49:46.000000 cikuu-2022.8.8/api/wget.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.590426 cikuu-2022.8.8/app/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:49:46.000000 cikuu-2022.8.8/app/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.590426 cikuu-2022.8.8/app/dmdsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2097 2023-03-04 12:49:46.000000 cikuu-2022.8.8/app/dmdsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2298 2023-03-04 12:49:46.000000 cikuu-2022.8.8/app/dmdsk/app_navbar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.590426 cikuu-2022.8.8/app/dmdsk/func/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:49:49.000000 cikuu-2022.8.8/app/dmdsk/func/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-03-04 12:49:44.000000 cikuu-2022.8.8/app/dmdsk/func/dim-awl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-03-04 12:49:44.000000 cikuu-2022.8.8/app/dmdsk/func/dims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2023-03-04 12:49:46.000000 cikuu-2022.8.8/app/dmdsk/func/eidv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-03-04 12:49:49.000000 cikuu-2022.8.8/app/dmdsk/func/feedback.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-03-04 12:49:44.000000 cikuu-2022.8.8/app/dmdsk/func/info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-03-04 12:49:44.000000 cikuu-2022.8.8/app/dmdsk/func/lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-03-04 12:49:46.000000 cikuu-2022.8.8/app/dmdsk/func/scores.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      490 2023-03-04 12:49:49.000000 cikuu-2022.8.8/app/dmdsk/func/sent.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-03-04 12:49:44.000000 cikuu-2022.8.8/app/dmdsk/func/trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      708 2023-03-04 12:49:49.000000 cikuu-2022.8.8/app/dmdsk/index.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.590426 cikuu-2022.8.8/cikuu.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-07-02 10:24:49.000000 cikuu-2022.8.8/cikuu.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6426 2023-07-02 10:24:49.000000 cikuu-2022.8.8/cikuu.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 10:24:49.000000 cikuu-2022.8.8/cikuu.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 10:24:49.000000 cikuu-2022.8.8/cikuu.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-07-02 10:24:49.000000 cikuu-2022.8.8/cikuu.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.642426 cikuu-2022.8.8/dic/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6977 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-03-04 12:49:46.000000 cikuu-2022.8.8/dic/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    72703 2023-03-04 12:49:46.000000 cikuu-2022.8.8/dic/adjlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15209 2023-03-04 12:49:48.000000 cikuu-2022.8.8/dic/advlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2036481 2023-05-04 07:44:16.000000 cikuu-2022.8.8/dic/bnc_wordlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   742662 2023-03-04 12:49:49.000000 cikuu-2022.8.8/dic/confu_set.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1423371 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/ecdic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8101 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/errants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   716825 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/essays.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   479692 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/frame.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1966581 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/lemma_lex.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   446749 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/lemma_mf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182701 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/lemma_scale.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1724920 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/lex_lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4088 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/mwe_disconj.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10043 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/mwe_pv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173703 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/n_is_sb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173515 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/nounlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3696547 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/nyt_wc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/oneself.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41916 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/orals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/poslist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2786732 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/propbank.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1350 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/stoplist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/to_redislite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    90499 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/verbform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9125 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/verblist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   147209 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/verbtag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   357010 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/vocab.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43159 2023-05-08 05:59:19.000000 cikuu-2022.8.8/dic/word_awl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   825665 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/word_bits.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   518752 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/word_grade.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46473 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/word_gsl1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42152 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/word_gsl2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2765429 2023-03-04 12:51:15.000000 cikuu-2022.8.8/dic/word_idf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2717304 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/word_oov.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3086978 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/word_pos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182843 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/word_scale.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  4370200 2023-03-04 12:51:15.000000 cikuu-2022.8.8/dic/wordattr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   300932 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/wordcnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   353846 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/wordlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   957421 2023-03-04 12:50:25.000000 cikuu-2022.8.8/dic/wordlist_ed1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   100665 2023-03-04 12:51:15.000000 cikuu-2022.8.8/dic/wordnet_verb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1150605 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/wordpos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    53593 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dic/words.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3636 2023-07-02 10:24:46.000000 cikuu-2022.8.8/dic/yulk.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.646426 cikuu-2022.8.8/dsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7973 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    94356 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5471 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/dm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2874 2023-03-06 07:28:15.000000 cikuu-2022.8.8/dsk/dsk-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-03-06 07:28:15.000000 cikuu-2022.8.8/dsk/dsk-req.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4928 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/dsk-to-dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9144 2023-05-01 01:51:11.000000 cikuu-2022.8.8/dsk/dsk2023.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/dskapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/dskes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5532 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/dskmkf_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2465 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/dsktrain.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/essaydm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/gears-xdsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4284 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/gecv1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7911 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6162 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/innersim.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6946 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/json-to-dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9243 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/kvrdsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8998 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/mkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/mqconsume.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83132 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/pingyu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3416 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/score.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6150 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/sntsdims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      936 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/tok-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3629 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/uvidsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6616 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/wps-gec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13783 2023-04-23 13:45:01.000000 cikuu-2022.8.8/dsk/wps-xgec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11422 2023-05-11 14:49:06.000000 cikuu-2022.8.8/dsk/wps7000.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9689 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/xessay.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10368 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/xgecv1-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-04-23 13:45:57.000000 cikuu-2022.8.8/dsk/xgecv1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4396 2023-03-04 12:51:16.000000 cikuu-2022.8.8/dsk/xmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2902 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/xsnt-gec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2186 2023-03-04 12:50:48.000000 cikuu-2022.8.8/dsk/xsnt-spacy.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/en/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80279 2023-03-20 11:54:15.000000 cikuu-2022.8.8/en/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5503 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6169 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/annotate.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/en/arc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    74716 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/arc/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1257 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/arc/sntjson-innodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15868 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/arc/sntjson-naclite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6901 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/arc/sntjson-naclite0.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23369 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/arc/sntjson-nacp-20230206.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26784 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/arc/sntjson-nacp-20230207.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-cl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3675 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-fts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/c4-gram-upload.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-gram.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      875 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-grams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-np.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/c4-postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      589 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4-trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2039 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4cl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4down.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1884 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/c4gram-mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2812 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4gram-upsert.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1731 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4gram.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5885 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4gramcl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3602 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/c4matcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1401 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4np.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3683 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4skenp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/c4tree.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/c4vp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/clause.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6120 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/dims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16963 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/docfts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8115 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/docjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-03-16 03:10:14.000000 cikuu-2022.8.8/en/en-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8717 2023-03-25 07:35:03.000000 cikuu-2022.8.8/en/es-index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/esbulk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3777 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/esfile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6311 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3506 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/exchunk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1159 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/exphrase.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1387 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/extrp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4656 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/havc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18434 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/kpsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4234 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/lempostag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13757 2023-07-02 09:34:40.000000 cikuu-2022.8.8/en/nacp-kvr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6454 2023-03-16 12:13:36.000000 cikuu-2022.8.8/en/nacp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/nlp-lit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4581 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/nlp-lmdb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1900 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/shav.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/silite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1506 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/snt-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1368 2023-07-02 09:34:39.000000 cikuu-2022.8.8/en/snt-spacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4786 2023-03-16 12:13:36.000000 cikuu-2022.8.8/en/sntjson-fts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-03-16 12:13:36.000000 cikuu-2022.8.8/en/sntjson-kpsnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8237 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/sntjson-mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13520 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/sntjson-nacp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      963 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/sntjson-parse-snt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2031 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/sntjson-si.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/sntjson-spacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2023-03-18 08:29:48.000000 cikuu-2022.8.8/en/sntjson-topk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-30 03:58:22.000000 cikuu-2022.8.8/en/sntjson-tosnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3888 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/sntjson-trpx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/sntjson-vp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2612 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/spacybs-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30937 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/spacybs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2733 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/spider-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6730 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/sqlsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30005 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/terms.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/verbnet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1874 2023-03-04 12:50:48.000000 cikuu-2022.8.8/en/xsnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-03-04 12:51:16.000000 cikuu-2022.8.8/en/zset-load.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/gecdsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9234 2023-05-03 03:14:08.000000 cikuu-2022.8.8/gecdsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      704 2023-05-03 03:19:37.000000 cikuu-2022.8.8/gecdsk/essays.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-05-11 08:23:32.000000 cikuu-2022.8.8/gecdsk/hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      943 2023-05-11 09:20:53.000000 cikuu-2022.8.8/gecdsk/paravs.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/lit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16540 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1467 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/common.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/lit/es/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5386 2023-03-04 12:50:48.000000 cikuu-2022.8.8/lit/es/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:15.000000 cikuu-2022.8.8/lit/es/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:27.000000 cikuu-2022.8.8/lit/essay.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/filling.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1905 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/fillmul.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      778 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/hello-pages.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-03-04 12:51:27.000000 cikuu-2022.8.8/lit/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/mock-scoring.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.658426 cikuu-2022.8.8/lit/penly/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/penly/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/penly/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/penly-resend.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1827 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/redis-dump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-03-04 12:51:27.000000 cikuu-2022.8.8/lit/reorder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/restore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/scoring.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/single.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-03-04 12:51:27.000000 cikuu-2022.8.8/lit/sntspolish.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1091 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/sntupgrade.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1000 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/student-input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1002 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/teacher-admin.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.662426 cikuu-2022.8.8/lit/yulk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      668 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/yulk/YULK.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/yulk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/yulk/common.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.662426 cikuu-2022.8.8/lit/yulk/func/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1063 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/bipos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/cola.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      666 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/corpuslist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      549 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      501 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/eshyb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      581 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/given-expect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/gramx-single.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1912 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/lemvs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/pos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/posvs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1925 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/style-in-mul.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      313 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/style.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      353 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/wcloud.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1547 2023-03-04 12:51:16.000000 cikuu-2022.8.8/lit/yulk/func/wordrank.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-03-04 12:51:27.000000 cikuu-2022.8.8/lit/yulk/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1255 2023-03-04 12:51:18.000000 cikuu-2022.8.8/lit/yulk/lemma.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.662426 cikuu-2022.8.8/pipe/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4906 2023-03-04 12:51:27.000000 cikuu-2022.8.8/pipe/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2622 2023-03-04 12:51:18.000000 cikuu-2022.8.8/pipe/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4039 2023-03-04 12:51:18.000000 cikuu-2022.8.8/pipe/redisgec8180.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6514 2023-03-04 12:51:27.000000 cikuu-2022.8.8/pipe/xgecv1.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.662426 cikuu-2022.8.8/rabbitmq/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3075 2023-04-30 03:58:22.000000 cikuu-2022.8.8/rabbitmq/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.662426 cikuu-2022.8.8/redisr/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      746 2023-04-30 03:58:22.000000 cikuu-2022.8.8/redisr/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8210 2023-05-04 00:09:32.000000 cikuu-2022.8.8/redisr/glove-get.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2023-05-03 09:15:53.000000 cikuu-2022.8.8/redisr/glove.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8249 2023-05-04 11:54:55.000000 cikuu-2022.8.8/redisr/sntvec-get.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.666426 cikuu-2022.8.8/sbert/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-04 10:29:10.000000 cikuu-2022.8.8/sbert/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1316 2023-03-04 12:51:18.000000 cikuu-2022.8.8/sbert/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-03 08:06:44.000000 cikuu-2022.8.8/sbert/hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2023-05-04 13:39:29.000000 cikuu-2022.8.8/sbert/redis-sntvec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2379 2023-05-05 09:11:12.000000 cikuu-2022.8.8/sbert/sntvec-so.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13086 2023-03-04 12:51:18.000000 cikuu-2022.8.8/sbert/sntvec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 10:24:49.678426 cikuu-2022.8.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      791 2023-07-02 10:24:46.000000 cikuu-2022.8.8/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.666426 cikuu-2022.8.8/so/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32507 2023-06-05 12:14:25.000000 cikuu-2022.8.8/so/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2177 2023-05-02 11:43:44.000000 cikuu-2022.8.8/so/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4772 2023-05-18 10:12:50.000000 cikuu-2022.8.8/so/batch-dis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1659 2023-05-19 02:35:35.000000 cikuu-2022.8.8/so/batch-sntspacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      907 2023-05-11 14:51:44.000000 cikuu-2022.8.8/so/dis-bnc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1259 2023-05-11 14:51:44.000000 cikuu-2022.8.8/so/dis-eev.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2040 2023-05-05 09:11:12.000000 cikuu-2022.8.8/so/dis-essays.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-05-05 09:11:12.000000 cikuu-2022.8.8/so/dis-folder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-05-09 13:44:41.000000 cikuu-2022.8.8/so/dis-tosnts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-03 03:14:08.000000 cikuu-2022.8.8/so/dsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1812 2023-05-22 02:37:54.000000 cikuu-2022.8.8/so/dump-pos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1747 2023-05-22 07:12:30.000000 cikuu-2022.8.8/so/dump-trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-05-03 03:14:08.000000 cikuu-2022.8.8/so/folder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1559 2023-03-04 12:51:18.000000 cikuu-2022.8.8/so/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1746 2023-03-04 12:51:18.000000 cikuu-2022.8.8/so/loades.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1222 2023-05-09 12:36:44.000000 cikuu-2022.8.8/so/tok-idf.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.666426 cikuu-2022.8.8/sqlite/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6138 2023-05-01 13:24:28.000000 cikuu-2022.8.8/sqlite/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      500 2023-05-01 14:50:34.000000 cikuu-2022.8.8/sqlite/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.670426 cikuu-2022.8.8/util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6263 2023-05-15 02:53:44.000000 cikuu-2022.8.8/util/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/annotate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3455 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/bcp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2820 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/c4data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/client-blpop.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/client-xwps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3219 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/clientx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9342 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/dsk-util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/fire-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/frame.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4097 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/kvr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/mq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      713 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/nldp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      796 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/pubsub-sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/pubsub2api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/sent-diff.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3123 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/spider.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/sqlitedict-load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4749 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/wps-blpop.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36149 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/wps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/xfile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/xgec-blpop120.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      371 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/xrange.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2034 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/xsnt-spacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-03-04 12:51:34.000000 cikuu-2022.8.8/util/xstream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-03-04 12:51:30.000000 cikuu-2022.8.8/util/xtest-params.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-03-04 12:51:33.000000 cikuu-2022.8.8/util/xtest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.670426 cikuu-2022.8.8/uviapp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-05-01 14:50:34.000000 cikuu-2022.8.8/uviapp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.674426 cikuu-2022.8.8/uvirun/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/Jinja2-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2151 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3034 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6573 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/c4es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2777 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/c4gramsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4734 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/cos_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-04-30 03:58:22.000000 cikuu-2022.8.8/uvirun/demo_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23119 2023-05-11 08:35:49.000000 cikuu-2022.8.8/uvirun/dsk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5335 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/echart_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4778 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/elastic_fastapi.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.674426 cikuu-2022.8.8/uvirun/errant/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7269 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/alignment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/errant/annotator.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.678426 cikuu-2022.8.8/uvirun/errant/commands/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/commands/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16344 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/errant/commands/compare_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-03-04 12:51:30.000000 cikuu-2022.8.8/uvirun/errant/commands/m2_to_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3801 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/commands/parallel_to_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2352 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/errant/edit.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 10:24:49.678426 cikuu-2022.8.8/uvirun/errant/en/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/en/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16879 2023-03-04 12:51:33.000000 cikuu-2022.8.8/uvirun/errant/en/classifier.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12340 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/errant/en/lancaster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5602 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/errant/en/merger.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10943 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/errant_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14040 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/es1_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25631 2023-03-20 01:06:12.000000 cikuu-2022.8.8/uvirun/es_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4806 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/essay_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18163 2023-04-30 03:58:22.000000 cikuu-2022.8.8/uvirun/exchunk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18525 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/feishu_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3892 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/flair_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1809 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1010 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/fusion_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3717 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/gec_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/gec_fastapi_33000.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13116 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/gensim_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6638 2023-04-12 02:56:55.000000 cikuu-2022.8.8/uvirun/gramx_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2562 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/hnswlib_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/kenlm_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6264 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/kpsi_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/kvr_dskdm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/kvr_dskdm1230.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19126 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/nldp_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/nltk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/nsp_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10222 2023-03-16 03:10:15.000000 cikuu-2022.8.8/uvirun/penlykvr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6558 2023-05-04 10:29:10.000000 cikuu-2022.8.8/uvirun/sbert_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/single_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32688 2023-05-08 12:37:28.000000 cikuu-2022.8.8/uvirun/spacy_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4644 2023-05-10 06:34:51.000000 cikuu-2022.8.8/uvirun/textacy_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2089 2023-03-04 12:51:44.000000 cikuu-2022.8.8/uvirun/trans_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4113 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/unmasker_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8742 2023-03-04 12:51:34.000000 cikuu-2022.8.8/uvirun/util_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45795 2023-03-04 12:51:41.000000 cikuu-2022.8.8/uvirun/uviredis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37415 2023-04-13 09:21:47.000000 cikuu-2022.8.8/uvirun/yulk-nac.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:16.484522 cikuu-2022.8.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-03-04 12:51:34.000000 cikuu-2022.8.9/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-07-07 10:48:16.484522 cikuu-2022.8.9/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:12.892508 cikuu-2022.8.9/api/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-03-04 12:49:43.000000 cikuu-2022.8.9/api/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2086 2023-03-04 12:49:43.000000 cikuu-2022.8.9/api/c4.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1236 2023-03-04 12:49:46.000000 cikuu-2022.8.9/api/chunk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1399 2023-03-04 12:49:49.000000 cikuu-2022.8.9/api/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2023-03-04 12:49:43.000000 cikuu-2022.8.9/api/dm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21647 2023-03-04 12:49:44.000000 cikuu-2022.8.9/api/es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-03-04 12:49:46.000000 cikuu-2022.8.9/api/feishu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-03-04 12:49:49.000000 cikuu-2022.8.9/api/mynac.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2023-03-04 12:49:44.000000 cikuu-2022.8.9/api/sntjson-es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-03-04 12:49:44.000000 cikuu-2022.8.9/api/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1333 2023-03-04 12:49:46.000000 cikuu-2022.8.9/api/wget.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:12.892508 cikuu-2022.8.9/app/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:49:46.000000 cikuu-2022.8.9/app/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:12.912508 cikuu-2022.8.9/app/dmdsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2097 2023-03-04 12:49:46.000000 cikuu-2022.8.9/app/dmdsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2298 2023-03-04 12:49:46.000000 cikuu-2022.8.9/app/dmdsk/app_navbar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:12.984508 cikuu-2022.8.9/app/dmdsk/func/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:49:49.000000 cikuu-2022.8.9/app/dmdsk/func/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-03-04 12:49:44.000000 cikuu-2022.8.9/app/dmdsk/func/dim-awl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-03-04 12:49:44.000000 cikuu-2022.8.9/app/dmdsk/func/dims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2023-03-04 12:49:46.000000 cikuu-2022.8.9/app/dmdsk/func/eidv.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-03-04 12:49:49.000000 cikuu-2022.8.9/app/dmdsk/func/feedback.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-03-04 12:49:44.000000 cikuu-2022.8.9/app/dmdsk/func/info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-03-04 12:49:44.000000 cikuu-2022.8.9/app/dmdsk/func/lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-03-04 12:49:46.000000 cikuu-2022.8.9/app/dmdsk/func/scores.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      490 2023-03-04 12:49:49.000000 cikuu-2022.8.9/app/dmdsk/func/sent.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-03-04 12:49:44.000000 cikuu-2022.8.9/app/dmdsk/func/trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      708 2023-03-04 12:49:49.000000 cikuu-2022.8.9/app/dmdsk/index.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:12.984508 cikuu-2022.8.9/cikuu.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-07-07 10:48:11.000000 cikuu-2022.8.9/cikuu.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6462 2023-07-07 10:48:11.000000 cikuu-2022.8.9/cikuu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-07 10:48:11.000000 cikuu-2022.8.9/cikuu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-07 10:48:11.000000 cikuu-2022.8.9/cikuu.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-07-07 10:48:11.000000 cikuu-2022.8.9/cikuu.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.040516 cikuu-2022.8.9/dic/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6977 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-03-04 12:49:46.000000 cikuu-2022.8.9/dic/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    72703 2023-03-04 12:49:46.000000 cikuu-2022.8.9/dic/adjlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15209 2023-03-04 12:49:48.000000 cikuu-2022.8.9/dic/advlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2036481 2023-05-04 07:44:16.000000 cikuu-2022.8.9/dic/bnc_wordlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   742662 2023-03-04 12:49:49.000000 cikuu-2022.8.9/dic/confu_set.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1423371 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/ecdic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8101 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/errants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   716825 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   479692 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/frame.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1966581 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/lemma_lex.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   446749 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/lemma_mf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182701 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/lemma_scale.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1724920 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/lex_lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4088 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/mwe_disconj.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10043 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/mwe_pv.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173703 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/n_is_sb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173515 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/nounlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3696547 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dic/nyt_wc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/oneself.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41916 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/orals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/poslist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2786732 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dic/propbank.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1350 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/stoplist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/to_redislite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    90499 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/verbform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9125 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dic/verblist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   147209 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/verbtag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   357010 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/vocab.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43159 2023-05-08 05:59:19.000000 cikuu-2022.8.9/dic/word_awl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   825665 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dic/word_bits.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   518752 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/word_grade.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46473 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/word_gsl1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42152 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/word_gsl2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2765429 2023-03-04 12:51:15.000000 cikuu-2022.8.9/dic/word_idf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2717304 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dic/word_oov.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3086978 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dic/word_pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182843 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/word_scale.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  4370200 2023-03-04 12:51:15.000000 cikuu-2022.8.9/dic/wordattr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   300932 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dic/wordcnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   353846 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dic/wordlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   957421 2023-03-04 12:50:25.000000 cikuu-2022.8.9/dic/wordlist_ed1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   100665 2023-03-04 12:51:15.000000 cikuu-2022.8.9/dic/wordnet_verb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1150605 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dic/wordpos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    53593 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dic/words.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3812 2023-07-07 10:48:04.000000 cikuu-2022.8.9/dic/yulk.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.244517 cikuu-2022.8.9/dsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7973 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    94356 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5471 2023-03-04 12:51:16.000000 cikuu-2022.8.9/dsk/dm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2874 2023-03-06 07:28:15.000000 cikuu-2022.8.9/dsk/dsk-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-03-06 07:28:15.000000 cikuu-2022.8.9/dsk/dsk-req.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4928 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/dsk-to-dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9144 2023-05-01 01:51:11.000000 cikuu-2022.8.9/dsk/dsk2023.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-03-04 12:51:16.000000 cikuu-2022.8.9/dsk/dskapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/dskes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5532 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/dskmkf_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2465 2023-03-04 12:51:16.000000 cikuu-2022.8.9/dsk/dsktrain.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/essaydm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/gears-xdsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4284 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/gecv1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7911 2023-03-04 12:51:16.000000 cikuu-2022.8.9/dsk/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6162 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/innersim.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6946 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/json-to-dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9243 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/kvrdsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-03-04 12:51:16.000000 cikuu-2022.8.9/dsk/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8998 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/mkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/mqconsume.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83132 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/pingyu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3416 2023-03-04 12:51:16.000000 cikuu-2022.8.9/dsk/score.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6150 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/sntsdims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      936 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-03-04 12:51:16.000000 cikuu-2022.8.9/dsk/tok-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3629 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/uvidsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6616 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/wps-gec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13783 2023-04-23 13:45:01.000000 cikuu-2022.8.9/dsk/wps-xgec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11422 2023-05-11 14:49:06.000000 cikuu-2022.8.9/dsk/wps7000.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9689 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/xessay.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10368 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/xgecv1-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-04-23 13:45:57.000000 cikuu-2022.8.9/dsk/xgecv1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4396 2023-03-04 12:51:16.000000 cikuu-2022.8.9/dsk/xmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2902 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/xsnt-gec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2186 2023-03-04 12:50:48.000000 cikuu-2022.8.9/dsk/xsnt-spacy.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.504518 cikuu-2022.8.9/en/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80711 2023-07-07 10:41:23.000000 cikuu-2022.8.9/en/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5503 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6169 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/annotate.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.512518 cikuu-2022.8.9/en/arc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    74716 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/arc/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1257 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/arc/sntjson-innodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15868 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/arc/sntjson-naclite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6901 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/arc/sntjson-naclite0.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23369 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/arc/sntjson-nacp-20230206.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26784 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/arc/sntjson-nacp-20230207.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4-cl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3675 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4-fts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/c4-gram-upload.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4-gram.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      875 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4-grams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4-np.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/c4-postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      589 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4-trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2039 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4cl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4down.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1884 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/c4gram-mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2812 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4gram-upsert.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1731 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4gram.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5885 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4gramcl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3602 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/c4matcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1401 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4np.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3683 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4skenp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/c4tree.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/c4vp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/clause.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6120 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/dims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16963 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/docfts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8115 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/docjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-03-16 03:10:14.000000 cikuu-2022.8.9/en/en-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8717 2023-03-25 07:35:03.000000 cikuu-2022.8.9/en/es-index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/esbulk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3777 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/esfile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6311 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3506 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/exchunk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1159 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/exphrase.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1387 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/extrp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4656 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/havc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18434 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/kpsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4234 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/lempostag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13757 2023-07-02 09:34:40.000000 cikuu-2022.8.9/en/nacp-kvr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6454 2023-03-16 12:13:36.000000 cikuu-2022.8.9/en/nacp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/nlp-lit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4581 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/nlp-lmdb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1900 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/shav.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/silite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1506 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/snt-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1368 2023-07-02 09:34:39.000000 cikuu-2022.8.9/en/snt-spacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4786 2023-03-16 12:13:36.000000 cikuu-2022.8.9/en/sntjson-fts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-03-16 12:13:36.000000 cikuu-2022.8.9/en/sntjson-kpsnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8237 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/sntjson-mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13520 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/sntjson-nacp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      963 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/sntjson-parse-snt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2031 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/sntjson-si.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/sntjson-spacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2023-03-18 08:29:48.000000 cikuu-2022.8.9/en/sntjson-topk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-30 03:58:22.000000 cikuu-2022.8.9/en/sntjson-tosnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3888 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/sntjson-trpx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/sntjson-vp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13615 2023-07-07 10:41:23.000000 cikuu-2022.8.9/en/sntspacy-si.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2612 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/spacybs-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30937 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/spacybs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2733 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/spider-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6730 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/sqlsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30005 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/terms.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/verbnet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1874 2023-03-04 12:50:48.000000 cikuu-2022.8.9/en/xsnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-03-04 12:51:16.000000 cikuu-2022.8.9/en/zset-load.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.568518 cikuu-2022.8.9/gecdsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9234 2023-05-03 03:14:08.000000 cikuu-2022.8.9/gecdsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      704 2023-05-03 03:19:37.000000 cikuu-2022.8.9/gecdsk/essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-05-11 08:23:32.000000 cikuu-2022.8.9/gecdsk/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      943 2023-05-11 09:20:53.000000 cikuu-2022.8.9/gecdsk/paravs.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.648518 cikuu-2022.8.9/lit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16540 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1467 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/common.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.652518 cikuu-2022.8.9/lit/es/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5386 2023-03-04 12:50:48.000000 cikuu-2022.8.9/lit/es/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:15.000000 cikuu-2022.8.9/lit/es/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:27.000000 cikuu-2022.8.9/lit/essay.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/filling.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1905 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/fillmul.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      778 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/hello-pages.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-03-04 12:51:27.000000 cikuu-2022.8.9/lit/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/mock-scoring.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.652518 cikuu-2022.8.9/lit/penly/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/penly/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/penly/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/penly-resend.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1827 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/redis-dump.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-03-04 12:51:27.000000 cikuu-2022.8.9/lit/reorder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/restore.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/scoring.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/single.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-03-04 12:51:27.000000 cikuu-2022.8.9/lit/sntspolish.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1091 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/sntupgrade.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1000 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/student-input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1002 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/teacher-admin.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.672519 cikuu-2022.8.9/lit/yulk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      668 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/yulk/YULK.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/yulk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/yulk/common.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.688519 cikuu-2022.8.9/lit/yulk/func/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1063 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/bipos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/cola.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      666 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/corpuslist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      549 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      501 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/eshyb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      581 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/given-expect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/gramx-single.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1912 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/lemvs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/posvs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1925 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/style-in-mul.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      313 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/style.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      353 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/wcloud.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1547 2023-03-04 12:51:16.000000 cikuu-2022.8.9/lit/yulk/func/wordrank.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-03-04 12:51:27.000000 cikuu-2022.8.9/lit/yulk/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1255 2023-03-04 12:51:18.000000 cikuu-2022.8.9/lit/yulk/lemma.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.692519 cikuu-2022.8.9/pipe/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4906 2023-03-04 12:51:27.000000 cikuu-2022.8.9/pipe/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2622 2023-03-04 12:51:18.000000 cikuu-2022.8.9/pipe/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4039 2023-03-04 12:51:18.000000 cikuu-2022.8.9/pipe/redisgec8180.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6514 2023-03-04 12:51:27.000000 cikuu-2022.8.9/pipe/xgecv1.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.696519 cikuu-2022.8.9/rabbitmq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3075 2023-04-30 03:58:22.000000 cikuu-2022.8.9/rabbitmq/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.740519 cikuu-2022.8.9/redisr/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      746 2023-04-30 03:58:22.000000 cikuu-2022.8.9/redisr/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8210 2023-05-04 00:09:32.000000 cikuu-2022.8.9/redisr/glove-get.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2023-05-03 09:15:53.000000 cikuu-2022.8.9/redisr/glove.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8249 2023-05-04 11:54:55.000000 cikuu-2022.8.9/redisr/sntvec-get.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:15.772519 cikuu-2022.8.9/sbert/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-04 10:29:10.000000 cikuu-2022.8.9/sbert/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1316 2023-03-04 12:51:18.000000 cikuu-2022.8.9/sbert/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-03 08:06:44.000000 cikuu-2022.8.9/sbert/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2023-05-04 13:39:29.000000 cikuu-2022.8.9/sbert/redis-sntvec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2379 2023-05-05 09:11:12.000000 cikuu-2022.8.9/sbert/sntvec-so.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13086 2023-03-04 12:51:18.000000 cikuu-2022.8.9/sbert/sntvec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-07 10:48:16.484522 cikuu-2022.8.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      791 2023-07-07 10:48:04.000000 cikuu-2022.8.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:16.036520 cikuu-2022.8.9/so/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32569 2023-07-07 08:11:28.000000 cikuu-2022.8.9/so/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2177 2023-05-02 11:43:44.000000 cikuu-2022.8.9/so/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4772 2023-05-18 10:12:50.000000 cikuu-2022.8.9/so/batch-dis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1659 2023-05-19 02:35:35.000000 cikuu-2022.8.9/so/batch-sntspacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      907 2023-05-11 14:51:44.000000 cikuu-2022.8.9/so/dis-bnc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1259 2023-05-11 14:51:44.000000 cikuu-2022.8.9/so/dis-eev.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2040 2023-05-05 09:11:12.000000 cikuu-2022.8.9/so/dis-essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-05-05 09:11:12.000000 cikuu-2022.8.9/so/dis-folder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-05-09 13:44:41.000000 cikuu-2022.8.9/so/dis-tosnts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-03 03:14:08.000000 cikuu-2022.8.9/so/dsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1812 2023-05-22 02:37:54.000000 cikuu-2022.8.9/so/dump-pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1747 2023-05-22 07:12:30.000000 cikuu-2022.8.9/so/dump-trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-05-03 03:14:08.000000 cikuu-2022.8.9/so/folder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1559 2023-03-04 12:51:18.000000 cikuu-2022.8.9/so/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1746 2023-03-04 12:51:18.000000 cikuu-2022.8.9/so/loades.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1507 2023-07-07 03:14:36.000000 cikuu-2022.8.9/so/sntspacy-es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1222 2023-05-09 12:36:44.000000 cikuu-2022.8.9/so/tok-idf.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:16.072520 cikuu-2022.8.9/sqlite/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6138 2023-05-01 13:24:28.000000 cikuu-2022.8.9/sqlite/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      500 2023-05-01 14:50:34.000000 cikuu-2022.8.9/sqlite/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:16.176520 cikuu-2022.8.9/util/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6263 2023-05-15 02:53:44.000000 cikuu-2022.8.9/util/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/annotate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3455 2023-03-04 12:51:34.000000 cikuu-2022.8.9/util/bcp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2820 2023-03-04 12:51:30.000000 cikuu-2022.8.9/util/c4data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/client-blpop.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/client-xwps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3219 2023-03-04 12:51:34.000000 cikuu-2022.8.9/util/clientx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9342 2023-03-04 12:51:30.000000 cikuu-2022.8.9/util/dsk-util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/fire-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-03-04 12:51:34.000000 cikuu-2022.8.9/util/frame.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4097 2023-03-04 12:51:30.000000 cikuu-2022.8.9/util/kvr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/mq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      713 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/nldp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      796 2023-03-04 12:51:34.000000 cikuu-2022.8.9/util/pubsub-sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2023-03-04 12:51:30.000000 cikuu-2022.8.9/util/pubsub2api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/sent-diff.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3123 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/spider.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-03-04 12:51:34.000000 cikuu-2022.8.9/util/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2023-03-04 12:51:30.000000 cikuu-2022.8.9/util/sqlitedict-load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4749 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/wps-blpop.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36149 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/wps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-03-04 12:51:34.000000 cikuu-2022.8.9/util/xfile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-03-04 12:51:30.000000 cikuu-2022.8.9/util/xgec-blpop120.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      371 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/xrange.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2034 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/xsnt-spacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-03-04 12:51:34.000000 cikuu-2022.8.9/util/xstream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-03-04 12:51:30.000000 cikuu-2022.8.9/util/xtest-params.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-03-04 12:51:33.000000 cikuu-2022.8.9/util/xtest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:16.176520 cikuu-2022.8.9/uviapp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-05-01 14:50:34.000000 cikuu-2022.8.9/uviapp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:16.424522 cikuu-2022.8.9/uvirun/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-03-04 12:51:44.000000 cikuu-2022.8.9/uvirun/Jinja2-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2151 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3034 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6573 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/c4es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2777 2023-03-04 12:51:44.000000 cikuu-2022.8.9/uvirun/c4gramsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4734 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/cos_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-04-30 03:58:22.000000 cikuu-2022.8.9/uvirun/demo_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23119 2023-05-11 08:35:49.000000 cikuu-2022.8.9/uvirun/dsk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5335 2023-03-04 12:51:44.000000 cikuu-2022.8.9/uvirun/echart_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4778 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/elastic_fastapi.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:16.456522 cikuu-2022.8.9/uvirun/errant/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-03-04 12:51:33.000000 cikuu-2022.8.9/uvirun/errant/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7269 2023-03-04 12:51:33.000000 cikuu-2022.8.9/uvirun/errant/alignment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/errant/annotator.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:16.480522 cikuu-2022.8.9/uvirun/errant/commands/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.9/uvirun/errant/commands/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16344 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/errant/commands/compare_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-03-04 12:51:30.000000 cikuu-2022.8.9/uvirun/errant/commands/m2_to_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3801 2023-03-04 12:51:33.000000 cikuu-2022.8.9/uvirun/errant/commands/parallel_to_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2352 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/errant/edit.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 10:48:16.484522 cikuu-2022.8.9/uvirun/errant/en/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.9/uvirun/errant/en/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16879 2023-03-04 12:51:33.000000 cikuu-2022.8.9/uvirun/errant/en/classifier.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12340 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/errant/en/lancaster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5602 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/errant/en/merger.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10943 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/errant_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14040 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/es1_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25631 2023-03-20 01:06:12.000000 cikuu-2022.8.9/uvirun/es_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4806 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/essay_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18163 2023-04-30 03:58:22.000000 cikuu-2022.8.9/uvirun/exchunk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18525 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/feishu_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3892 2023-03-04 12:51:44.000000 cikuu-2022.8.9/uvirun/flair_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1809 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1010 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/fusion_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3717 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/gec_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-03-04 12:51:44.000000 cikuu-2022.8.9/uvirun/gec_fastapi_33000.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13116 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/gensim_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6638 2023-04-12 02:56:55.000000 cikuu-2022.8.9/uvirun/gramx_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2562 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/hnswlib_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-03-04 12:51:44.000000 cikuu-2022.8.9/uvirun/kenlm_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6264 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/kpsi_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/kvr_dskdm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/kvr_dskdm1230.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19126 2023-03-04 12:51:44.000000 cikuu-2022.8.9/uvirun/nldp_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/nltk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/nsp_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10222 2023-03-16 03:10:15.000000 cikuu-2022.8.9/uvirun/penlykvr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6558 2023-05-04 10:29:10.000000 cikuu-2022.8.9/uvirun/sbert_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/single_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32688 2023-05-08 12:37:28.000000 cikuu-2022.8.9/uvirun/spacy_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4644 2023-05-10 06:34:51.000000 cikuu-2022.8.9/uvirun/textacy_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2089 2023-03-04 12:51:44.000000 cikuu-2022.8.9/uvirun/trans_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4113 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/unmasker_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8742 2023-03-04 12:51:34.000000 cikuu-2022.8.9/uvirun/util_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45795 2023-03-04 12:51:41.000000 cikuu-2022.8.9/uvirun/uviredis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37415 2023-04-13 09:21:47.000000 cikuu-2022.8.9/uvirun/yulk-nac.py
```

### Comparing `cikuu-2022.8.8/api/c4.py` & `cikuu-2022.8.9/api/c4.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/api/chunk.py` & `cikuu-2022.8.9/api/chunk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/api/common.py` & `cikuu-2022.8.9/api/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/api/dm.py` & `cikuu-2022.8.9/api/dm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/api/es.py` & `cikuu-2022.8.9/api/es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/api/feishu.py` & `cikuu-2022.8.9/api/feishu.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/api/mynac.py` & `cikuu-2022.8.9/api/mynac.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/api/sntjson-es.py` & `cikuu-2022.8.9/api/sntjson-es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/api/wget.py` & `cikuu-2022.8.9/api/wget.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/app/dmdsk/__init__.py` & `cikuu-2022.8.9/app/dmdsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/app/dmdsk/app_navbar.py` & `cikuu-2022.8.9/app/dmdsk/app_navbar.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/app/dmdsk/func/lemma.py` & `cikuu-2022.8.9/app/dmdsk/func/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/app/dmdsk/func/trp.py` & `cikuu-2022.8.9/app/dmdsk/func/trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/app/dmdsk/index.py` & `cikuu-2022.8.9/app/dmdsk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/cikuu.egg-info/SOURCES.txt` & `cikuu-2022.8.9/cikuu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
 en/sntjson-parse-snt.py
 en/sntjson-si.py
 en/sntjson-spacy.py
 en/sntjson-topk.py
 en/sntjson-tosnt.py
 en/sntjson-trpx.py
 en/sntjson-vp.py
+en/sntspacy-si.py
 en/spacybs-esjson.py
 en/spacybs.py
 en/spider-esjson.py
 en/sqlsi.py
 en/terms.py
 en/verbnet.py
 en/xsnt.py
@@ -262,14 +263,15 @@
 so/dis-tosnts.py
 so/dsk.py
 so/dump-pos.py
 so/dump-trp.py
 so/folder.py
 so/load.py
 so/loades.py
+so/sntspacy-es.py
 so/tok-idf.py
 sqlite/__init__.py
 sqlite/__main__.py
 util/__init__.py
 util/__main__.py
 util/annotate.py
 util/bcp.py
```

### Comparing `cikuu-2022.8.8/dic/__init__.py` & `cikuu-2022.8.9/dic/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/adjlist.py` & `cikuu-2022.8.9/dic/adjlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/advlist.py` & `cikuu-2022.8.9/dic/advlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/bnc_wordlist.py` & `cikuu-2022.8.9/dic/bnc_wordlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/confu_set.py` & `cikuu-2022.8.9/dic/confu_set.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/ecdic.py` & `cikuu-2022.8.9/dic/ecdic.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/errants.py` & `cikuu-2022.8.9/dic/errants.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/essays.py` & `cikuu-2022.8.9/dic/essays.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/frame.py` & `cikuu-2022.8.9/dic/frame.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/lemma_lex.py` & `cikuu-2022.8.9/dic/lemma_lex.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/lemma_mf.py` & `cikuu-2022.8.9/dic/lemma_mf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/lemma_scale.py` & `cikuu-2022.8.9/dic/lemma_scale.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/lex_lemma.py` & `cikuu-2022.8.9/dic/lex_lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/mwe_disconj.py` & `cikuu-2022.8.9/dic/mwe_disconj.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/mwe_pv.py` & `cikuu-2022.8.9/dic/mwe_pv.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/n_is_sb.py` & `cikuu-2022.8.9/dic/n_is_sb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/nounlist.py` & `cikuu-2022.8.9/dic/nounlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/nyt_wc.py` & `cikuu-2022.8.9/dic/nyt_wc.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/orals.py` & `cikuu-2022.8.9/dic/orals.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/propbank.py` & `cikuu-2022.8.9/dic/propbank.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/stoplist.py` & `cikuu-2022.8.9/dic/stoplist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/to_redislite.py` & `cikuu-2022.8.9/dic/to_redislite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/verbform.py` & `cikuu-2022.8.9/dic/verbform.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/verblist.py` & `cikuu-2022.8.9/dic/verblist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/verbtag.py` & `cikuu-2022.8.9/dic/verbtag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/vocab.py` & `cikuu-2022.8.9/dic/vocab.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/word_awl.py` & `cikuu-2022.8.9/dic/word_awl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/word_bits.py` & `cikuu-2022.8.9/dic/word_bits.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/word_grade.py` & `cikuu-2022.8.9/dic/word_grade.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/word_gsl1.py` & `cikuu-2022.8.9/dic/word_gsl1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/word_gsl2.py` & `cikuu-2022.8.9/dic/word_gsl2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/word_idf.py` & `cikuu-2022.8.9/dic/word_idf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/word_oov.py` & `cikuu-2022.8.9/dic/word_oov.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/word_pos.py` & `cikuu-2022.8.9/dic/word_pos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/word_scale.py` & `cikuu-2022.8.9/dic/word_scale.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/wordattr.py` & `cikuu-2022.8.9/dic/wordattr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/wordcnt.py` & `cikuu-2022.8.9/dic/wordcnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/wordlist.py` & `cikuu-2022.8.9/dic/wordlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/wordlist_ed1.py` & `cikuu-2022.8.9/dic/wordlist_ed1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/wordnet_verb.py` & `cikuu-2022.8.9/dic/wordnet_verb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/wordpos.py` & `cikuu-2022.8.9/dic/wordpos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/words.py` & `cikuu-2022.8.9/dic/words.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dic/yulk.py` & `cikuu-2022.8.9/dic/yulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,33 @@
 
 snthost = os.getenv('snthost', 'snt.jukuu.com:6206') #  snt => tx98
 if not hasattr(spacy, 'nlp'):
 	spacy.nlp		= spacy.load(os.getenv('spacy_model','en_core_web_sm')) # 3.4.1
 	spacy.from_json = lambda arr: spacy.tokens.Doc(spacy.nlp.vocab).from_json(arr) # added 2022.8.19
 
 def rcon():
-	if not hasattr(redis, 'r'): redis.r = redis.Redis(host=snthost.split(':')[0], port=int(snthost.split(':')[-1]), decode_responses=True)
+	if not hasattr(redis, 'r'): redis.r = redis.Redis(host=snthost.split(':')[0], port=int(snthost.split(':')[-1]), decode_responses=True, health_check_interval=30)
 	return redis.r 
 
+def keys(pattern:str): #f"snt-spacy:{name}:*"
+	r = rcon()
+	for k in r.keys(pattern):
+		yield k 
+
 def docs(name:str='gzjc'):
-	if not hasattr(redis, 'r'): redis.r = redis.Redis(host=snthost.split(':')[0], port=int(snthost.split(':')[-1]), decode_responses=True)
+	if not hasattr(redis, 'r'): redis.r = redis.Redis(host=snthost.split(':')[0], port=int(snthost.split(':')[-1]), decode_responses=True, health_check_interval=30)
 	for k in redis.r.keys(f"snt-spacy:{name}:*"):
 		v = redis.r.get(k)  #redis.r.hget(k, 'spacy')
 		if not v: continue 
 		arr = json.loads(v.strip()) 
 		doc = spacy.from_json(arr) 
 		yield doc 
 
 def txtdocs(name:str='spider'):
-	if not hasattr(redis, 'r'): redis.r = redis.Redis(host=snthost.split(':')[0], port=int(snthost.split(':')[-1]), decode_responses=True)
+	if not hasattr(redis, 'r'): redis.r = redis.Redis(host=snthost.split(':')[0], port=int(snthost.split(':')[-1]), decode_responses=True, health_check_interval=30)
 	for k in redis.r.keys(f"txt-spacy:{name}:*"):
 		v = redis.r.hget(k, 'spacy')
 		if not v: continue 
 		arr = json.loads(v.strip()) 
 		doc = spacy.from_json(arr) 
 		yield doc 
 
@@ -33,15 +38,15 @@
 		redis.r = redis.Redis(host=host, port=port, decode_responses=True)
 		print ( redis.r, flush=True)
 	
 	def hello(self, name:str='gzjc'):
 		for doc in docs(name): print(doc) 
 
 	def sntspacy(self, infile):
-		''' find . -name "*.4.1.gz" -exec python yulk.py sntspacy {} ;  '''
+		''' find . -name "*.4.1.gz" -exec python yulk.py sntspacy {} \;  '''
 		name = infile.split('/')[-1].split('.')[0] # ./sci.jsonlg.3.4.1.gz
 		print ("snt-spacy started:", name ,  ' -> ',  redis.r, flush=True)
 		[ redis.r.delete(k) for k in redis.r.keys(f"snt-spacy:{name}:*")]
 		start = time.time()
 
 		redis.r.hset("snt-spacy", name, 0) 
 		for sid, line in enumerate(fileinput.input(infile,openhook=fileinput.hook_compressed)): #356317 docs of each doc file
```

### Comparing `cikuu-2022.8.8/dsk/__init__.py` & `cikuu-2022.8.9/dsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/__main__.py` & `cikuu-2022.8.9/dsk/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/common.py` & `cikuu-2022.8.9/dsk/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/dm.py` & `cikuu-2022.8.9/dsk/dm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/dsk-hello.py` & `cikuu-2022.8.9/dsk/dsk-hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/dsk-to-dskmkf.py` & `cikuu-2022.8.9/dsk/dsk-to-dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/dsk2023.py` & `cikuu-2022.8.9/dsk/dsk2023.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/dskapi.py` & `cikuu-2022.8.9/dsk/dskapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/dskes.py` & `cikuu-2022.8.9/dsk/dskes.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/dskmkf.py` & `cikuu-2022.8.9/dsk/dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/dskmkf_fastapi.py` & `cikuu-2022.8.9/dsk/dskmkf_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/dsktrain.py` & `cikuu-2022.8.9/dsk/dsktrain.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/essaydm.py` & `cikuu-2022.8.9/dsk/essaydm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/gears-xdsk.py` & `cikuu-2022.8.9/dsk/gears-xdsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/gecv1.py` & `cikuu-2022.8.9/dsk/gecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/index.py` & `cikuu-2022.8.9/dsk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/innersim.py` & `cikuu-2022.8.9/dsk/innersim.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/json-to-dskmkf.py` & `cikuu-2022.8.9/dsk/json-to-dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/kvrdsk.py` & `cikuu-2022.8.9/dsk/kvrdsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/load.py` & `cikuu-2022.8.9/dsk/load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/mkf.py` & `cikuu-2022.8.9/dsk/mkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/mqconsume.py` & `cikuu-2022.8.9/dsk/mqconsume.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/pingyu.py` & `cikuu-2022.8.9/dsk/pingyu.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/score.py` & `cikuu-2022.8.9/dsk/score.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/sntsdims.py` & `cikuu-2022.8.9/dsk/sntsdims.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/test.py` & `cikuu-2022.8.9/dsk/test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/tok-hello.py` & `cikuu-2022.8.9/dsk/tok-hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/uvidsk.py` & `cikuu-2022.8.9/dsk/uvidsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/wps-gec.py` & `cikuu-2022.8.9/dsk/wps-gec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/wps-xgec.py` & `cikuu-2022.8.9/dsk/wps-xgec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/wps7000.py` & `cikuu-2022.8.9/dsk/wps7000.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/xessay.py` & `cikuu-2022.8.9/dsk/xessay.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/xgecv1-test.py` & `cikuu-2022.8.9/dsk/xgecv1-test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/xgecv1.py` & `cikuu-2022.8.9/dsk/xgecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/xmkf.py` & `cikuu-2022.8.9/dsk/xmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/xsnt-gec.py` & `cikuu-2022.8.9/dsk/xsnt-gec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/dsk/xsnt-spacy.py` & `cikuu-2022.8.9/dsk/xsnt-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/__init__.py` & `cikuu-2022.8.9/en/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,4908 +111,4935 @@
 000006e0: 746f 2072 656c 6561 7365 2073 7061 6379  to release spacy
 000006f0: 2773 206d 656d 6f72 7920 2c20 6164 6465  's memory , adde
 00000700: 6420 3230 3233 2e31 2e32 300a 0973 7061  d 2023.1.20..spa
 00000710: 6379 2e6e 6c70 203d 2073 7061 6379 2e6c  cy.nlp = spacy.l
 00000720: 6f61 6428 6f73 2e67 6574 656e 7628 2773  oad(os.getenv('s
 00000730: 7061 6379 5f6d 6f64 656c 272c 2765 6e5f  pacy_model','en_
 00000740: 636f 7265 5f77 6562 5f6c 6727 2929 0a0a  core_web_lg'))..
-00000750: 6465 6620 7068 7261 7365 5f6d 6174 6368  def phrase_match
-00000760: 6572 2820 7275 6c65 7320 3d7b 2770 7027  er( rules ={'pp'
-00000770: 3a5b 5b7b 2750 4f53 273a 2027 4144 5027  :[[{'POS': 'ADP'
-00000780: 7d2c 7b22 504f 5322 3a20 7b22 494e 223a  },{"POS": {"IN":
-00000790: 205b 2244 4554 222c 224e 554d 222c 2241   ["DET","NUM","A
-000007a0: 444a 222c 2750 554e 4354 272c 2743 4f4e  DJ",'PUNCT','CON
-000007b0: 4a27 5d7d 2c20 224f 5022 3a20 222a 227d  J']}, "OP": "*"}
-000007c0: 2c7b 2250 4f53 223a 207b 2249 4e22 3a20  ,{"POS": {"IN": 
-000007d0: 5b22 4e4f 554e 222c 2250 4152 5422 5d7d  ["NOUN","PART"]}
-000007e0: 2c20 224f 5022 3a20 222b 227d 5d5d 207d  , "OP": "+"}]] }
-000007f0: 293a 0a09 2727 2720 666f 7220 6e61 6d65  ):..''' for name
-00000800: 2c20 6962 6567 2c69 656e 6420 696e 206d  , ibeg,iend in m
-00000810: 6174 6368 6572 2864 6f63 2920 3a20 7072  atcher(doc) : pr
-00000820: 696e 7428 7370 6163 792e 6e6c 702e 766f  int(spacy.nlp.vo
-00000830: 6361 625b 6e61 6d65 5d2e 7465 7874 2c20  cab[name].text, 
-00000840: 646f 635b 6962 6567 3a69 656e 645d 2e74  doc[ibeg:iend].t
-00000850: 6578 7429 2027 2727 0a09 6d61 7463 6865  ext) '''..matche
-00000860: 7220 3d20 4d61 7463 6865 7228 7370 6163  r = Matcher(spac
-00000870: 792e 6e6c 702e 766f 6361 6229 0a09 5b6d  y.nlp.vocab)..[m
-00000880: 6174 6368 6572 2e61 6464 286e 616d 652c  atcher.add(name,
-00000890: 2070 6174 732c 2020 6772 6565 6479 203d   pats,  greedy =
-000008a0: 274c 4f4e 4745 5354 2729 2066 6f72 206e  'LONGEST') for n
-000008b0: 616d 652c 2070 6174 7320 696e 2072 756c  ame, pats in rul
-000008c0: 6573 2e69 7465 6d73 2829 5d0a 0972 6574  es.items()]..ret
-000008d0: 7572 6e20 6d61 7463 6865 720a 0a64 6566  urn matcher..def
-000008e0: 2044 6570 4d61 7463 6865 7228 7275 6c65   DepMatcher(rule
-000008f0: 733a 6469 6374 203d 207b 2273 766f 223a  s:dict = {"svo":
-00000900: 5b20 7b22 5249 4748 545f 4944 223a 2022  [ {"RIGHT_ID": "
-00000910: 7622 2c20 2022 5249 4748 545f 4154 5452  v",  "RIGHT_ATTR
-00000920: 5322 3a20 7b22 504f 5322 3a20 2256 4552  S": {"POS": "VER
-00000930: 4222 7d7d 2c20 7b22 4c45 4654 5f49 4422  B"}}, {"LEFT_ID"
-00000940: 3a20 2276 222c 2022 5245 4c5f 4f50 223a  : "v", "REL_OP":
-00000950: 2022 3e22 2c20 2252 4947 4854 5f49 4422   ">", "RIGHT_ID"
-00000960: 3a20 2273 7562 6a65 6374 222c 2022 5249  : "subject", "RI
-00000970: 4748 545f 4154 5452 5322 3a20 7b22 4445  GHT_ATTRS": {"DE
-00000980: 5022 3a20 226e 7375 626a 227d 7d2c 7b22  P": "nsubj"}},{"
-00000990: 4c45 4654 5f49 4422 3a20 2276 222c 2022  LEFT_ID": "v", "
-000009a0: 5245 4c5f 4f50 223a 2022 3e22 2c20 2252  REL_OP": ">", "R
-000009b0: 4947 4854 5f49 4422 3a20 226f 626a 6563  IGHT_ID": "objec
-000009c0: 7422 2c22 5249 4748 545f 4154 5452 5322  t","RIGHT_ATTRS"
-000009d0: 3a20 7b22 4445 5022 3a20 2264 6f62 6a22  : {"DEP": "dobj"
-000009e0: 7d20 207d 5d2c 7d20 293a 0a09 2727 2720  }  }],} ):..''' 
-000009f0: 205b 2873 7061 6379 2e6e 6c70 2e76 6f63   [(spacy.nlp.voc
-00000a00: 6162 5b6e 616d 655d 2e74 6578 742c 2061  ab[name].text, a
-00000a10: 7229 2066 6f72 206e 616d 652c 2061 7220  r) for name, ar 
-00000a20: 696e 206d 6174 6368 6572 2864 6f63 295d  in matcher(doc)]
-00000a30: 2020 235b 2827 7376 6f27 2c20 5b31 2c20    #[('svo', [1, 
-00000a40: 302c 2032 5d29 5d27 2727 0a09 6672 6f6d  0, 2])]'''..from
-00000a50: 2073 7061 6379 2e6d 6174 6368 6572 2069   spacy.matcher i
-00000a60: 6d70 6f72 7420 4465 7065 6e64 656e 6379  mport Dependency
-00000a70: 4d61 7463 6865 720a 096d 6174 6368 6572  Matcher..matcher
-00000a80: 203d 2044 6570 656e 6465 6e63 794d 6174   = DependencyMat
-00000a90: 6368 6572 2873 7061 6379 2e6e 6c70 2e76  cher(spacy.nlp.v
-00000aa0: 6f63 6162 290a 095b 6d61 7463 6865 722e  ocab)..[matcher.
-00000ab0: 6164 6428 6e61 6d65 2c20 5b70 6174 7465  add(name, [patte
-00000ac0: 726e 5d29 2066 6f72 206e 616d 652c 2070  rn]) for name, p
-00000ad0: 6174 7465 726e 2069 6e20 7275 6c65 732e  attern in rules.
-00000ae0: 6974 656d 7328 2920 5d0a 0972 6574 7572  items() ]..retur
-00000af0: 6e20 6d61 7463 6865 7220 0a0a 6465 6620  n matcher ..def 
-00000b00: 736e 7462 7228 6573 7361 792c 2074 7269  sntbr(essay, tri
-00000b10: 6d3a 626f 6f6c 3d46 616c 7365 2c20 7769  m:bool=False, wi
-00000b20: 7468 5f70 6964 3a62 6f6f 6c3d 4661 6c73  th_pid:bool=Fals
-00000b30: 6529 3a20 0a09 2727 2720 6164 6465 6420  e): ..''' added 
-00000b40: 3230 3232 2e35 2e32 3820 2727 270a 0966  2022.5.28 '''..f
-00000b50: 726f 6d20 7370 6163 792e 6c61 6e67 2069  rom spacy.lang i
-00000b60: 6d70 6f72 7420 656e 0a09 6966 206e 6f74  mport en..if not
-00000b70: 2068 6173 6174 7472 2873 6e74 6272 2c20   hasattr(sntbr, 
-00000b80: 2769 6e73 7427 293a 200a 0909 736e 7462  'inst'): ...sntb
-00000b90: 722e 696e 7374 203d 2065 6e2e 456e 676c  r.inst = en.Engl
-00000ba0: 6973 6828 290a 0909 736e 7462 722e 696e  ish()...sntbr.in
-00000bb0: 7374 2e61 6464 5f70 6970 6528 2273 656e  st.add_pipe("sen
-00000bc0: 7465 6e63 697a 6572 2229 0a0a 0964 6f63  tencizer")...doc
-00000bd0: 203d 2073 6e74 6272 2e69 6e73 7428 6573   = sntbr.inst(es
-00000be0: 7361 7929 0a09 6966 206e 6f74 2077 6974  say)..if not wit
-00000bf0: 685f 7069 643a 2072 6574 7572 6e20 5b20  h_pid: return [ 
-00000c00: 736e 742e 7465 7874 2e73 7472 6970 2829  snt.text.strip()
-00000c10: 2069 6620 7472 696d 2065 6c73 6520 736e   if trim else sn
-00000c20: 742e 7465 7874 2066 6f72 2073 6e74 2069  t.text for snt i
-00000c30: 6e20 2064 6f63 2e73 656e 7473 5d0a 0a09  n  doc.sents]...
-00000c40: 7069 6420 3d20 3020 2373 7061 6379 2e73  pid = 0 #spacy.s
-00000c50: 6e74 7069 646f 6666 093d 206c 616d 6264  ntpidoff.= lambd
-00000c60: 6120 6573 7361 793a 2028 7069 643a 3d30  a essay: (pid:=0
-00000c70: 2c20 646f 633a 3d73 7061 6379 2e73 6e74  , doc:=spacy.snt
-00000c80: 6272 2865 7373 6179 292c 205b 2028 2070  br(essay), [ ( p
-00000c90: 6964 203a 3d20 7069 6420 2b20 3120 6966  id := pid + 1 if
-00000ca0: 2022 5c6e 2220 696e 2073 6e74 2e74 6578   "\n" in snt.tex
-00000cb0: 7420 656c 7365 2070 6964 2c20 2028 736e  t else pid,  (sn
-00000cc0: 742e 7465 7874 2c20 7069 642c 2064 6f63  t.text, pid, doc
-00000cd0: 5b73 6e74 2e73 7461 7274 5d2e 6964 7829  [snt.start].idx)
-00000ce0: 295b 2d31 5d20 666f 7220 736e 7420 696e  )[-1] for snt in
-00000cf0: 2020 646f 632e 7365 6e74 735d 2029 5b2d    doc.sents] )[-
-00000d00: 315d 0a09 6172 7220 3d20 5b5d 0a09 666f  1]..arr = []..fo
-00000d10: 7220 736e 7420 696e 2020 646f 632e 7365  r snt in  doc.se
-00000d20: 6e74 733a 0a09 0969 6620 225c 6e22 2069  nts:...if "\n" i
-00000d30: 6e20 736e 742e 7465 7874 3a20 7069 6420  n snt.text: pid 
-00000d40: 3d20 7069 6420 2b20 3120 0a09 0961 7272  = pid + 1 ...arr
-00000d50: 2e61 7070 656e 6428 2028 736e 742e 7465  .append( (snt.te
-00000d60: 7874 2c20 7069 6429 2029 200a 0972 6574  xt, pid) ) ..ret
-00000d70: 7572 6e20 6172 7220 0a0a 6465 6620 636f  urn arr ..def co
-00000d80: 6d6d 6f6e 5f70 6572 6328 736e 743d 2253  mmon_perc(snt="S
-00000d90: 6865 2068 6173 2072 6561 6479 2e22 2c20  he has ready.", 
-00000da0: 7472 616e 733d 2253 6865 2069 7320 7265  trans="She is re
-00000db0: 6164 792e 2229 3a20 0a09 746f 6b73 203d  ady."): ..toks =
-00000dc0: 2073 6574 285b 742e 7465 7874 2066 6f72   set([t.text for
-00000dd0: 2074 2069 6e20 7370 6163 792e 6e6c 702e   t in spacy.nlp.
-00000de0: 746f 6b65 6e69 7a65 7228 736e 7429 5d29  tokenizer(snt)])
-00000df0: 0a09 7265 7475 726e 206c 656e 285b 7420  ..return len([t 
-00000e00: 666f 7220 7420 696e 2073 7061 6379 2e6e  for t in spacy.n
-00000e10: 6c70 2e74 6f6b 656e 697a 6572 2874 7261  lp.tokenizer(tra
-00000e20: 6e73 2920 6966 2074 2e74 6578 7420 696e  ns) if t.text in
-00000e30: 2074 6f6b 735d 2920 2f20 286c 656e 2874   toks]) / (len(t
-00000e40: 6f6b 7329 2b30 2e30 3129 0a0a 6d65 7267  oks)+0.01)..merg
-00000e50: 655f 6e70 7309 093d 2073 7061 6379 2e6e  e_nps..= spacy.n
-00000e60: 6c70 2e63 7265 6174 655f 7069 7065 2822  lp.create_pipe("
-00000e70: 6d65 7267 655f 6e6f 756e 5f63 6875 6e6b  merge_noun_chunk
-00000e80: 7322 2920 236d 6572 6765 5f65 6e74 6974  s") #merge_entit
-00000e90: 6965 730a 6d65 7267 655f 656e 7409 093d  ies.merge_ent..=
-00000ea0: 2073 7061 6379 2e6e 6c70 2e63 7265 6174   spacy.nlp.creat
-00000eb0: 655f 7069 7065 2822 6d65 7267 655f 656e  e_pipe("merge_en
-00000ec0: 7469 7469 6573 2229 200a 6e65 775f 6d61  tities") .new_ma
-00000ed0: 7463 6865 7209 093d 206c 616d 6264 6120  tcher..= lambda 
-00000ee0: 3a20 4d61 7463 6865 7228 7370 6163 792e  : Matcher(spacy.
-00000ef0: 6e6c 702e 766f 6361 6229 2023 2062 7920  nlp.vocab) # by 
-00000f00: 6578 6368 756e 6b0a 746f 6b73 0909 093d  exchunk.toks...=
-00000f10: 206c 616d 6264 6120 646f 633a 2020 5b7b   lambda doc:  [{
-00000f20: 2769 273a 742e 692c 2022 6865 6164 223a  'i':t.i, "head":
-00000f30: 742e 6865 6164 2e69 2c20 276c 6578 273a  t.head.i, 'lex':
-00000f40: 742e 7465 7874 2c20 276c 656d 273a 742e  t.text, 'lem':t.
-00000f50: 6c65 6d6d 615f 2c20 2770 6f73 273a 742e  lemma_, 'pos':t.
-00000f60: 706f 735f 2c20 2774 6167 273a 742e 7461  pos_, 'tag':t.ta
-00000f70: 675f 2c20 2764 6570 273a 742e 6465 705f  g_, 'dep':t.dep_
-00000f80: 2c20 2267 706f 7322 3a74 2e68 6561 642e  , "gpos":t.head.
-00000f90: 706f 735f 2c20 2267 6c65 6d22 3a74 2e68  pos_, "glem":t.h
-00000fa0: 6561 642e 6c65 6d6d 615f 7d20 666f 7220  ead.lemma_} for 
-00000fb0: 7420 696e 2064 6f63 205d 2023 204a 534f  t in doc ] # JSO
-00000fc0: 4e45 6163 6852 6f77 200a 706f 7374 6167  NEachRow .postag
-00000fd0: 0909 093d 206c 616d 6264 6120 646f 633a  ...= lambda doc:
-00000fe0: 2020 225f 5e20 2220 2b20 2220 222e 6a6f    "_^ " + " ".jo
-00000ff0: 696e 285b 2066 227b 742e 7465 7874 7d5f  in([ f"{t.text}_
-00001000: 7b74 2e6c 656d 6d61 5f7d 5f7b 742e 706f  {t.lemma_}_{t.po
-00001010: 735f 7d5f 7b74 2e74 6167 5f7d 2220 666f  s_}_{t.tag_}" fo
-00001020: 7220 7420 696e 2064 6f63 5d29 202b 2022  r t in doc]) + "
-00001030: 205f 2422 0a6e 6f6e 5f72 6f6f 745f 7665   _$".non_root_ve
-00001040: 7262 7309 3d20 6c61 6d62 6461 2064 6f63  rbs.= lambda doc
-00001050: 3a20 205b 7420 666f 7220 7420 696e 2064  :  [t for t in d
-00001060: 6f63 2069 6620 742e 706f 735f 203d 3d20  oc if t.pos_ == 
-00001070: 2756 4552 4227 2061 6e64 2074 2e64 6570  'VERB' and t.dep
-00001080: 5f20 213d 2027 524f 4f54 275d 200a 7369  _ != 'ROOT'] .si
-00001090: 6d70 6c65 5f73 656e 7409 093d 206c 616d  mple_sent..= lam
-000010a0: 6264 6120 646f 633a 2020 6c65 6e28 5b74  bda doc:  len([t
-000010b0: 2066 6f72 2074 2069 6e20 646f 6320 6966   for t in doc if
-000010c0: 2074 2e70 6f73 5f20 3d3d 2027 5645 5242   t.pos_ == 'VERB
-000010d0: 2720 616e 6420 742e 6465 705f 2021 3d20  ' and t.dep_ != 
-000010e0: 2752 4f4f 5427 5d29 203c 3d20 3020 2320  'ROOT']) <= 0 # 
-000010f0: 656c 7365 2069 7320 636f 6d70 6c65 7820  else is complex 
-00001100: 7365 6e74 200a 636f 6d70 6f75 6e64 5f73  sent .compound_s
-00001110: 6e74 093d 206c 616d 6264 6120 646f 633a  nt.= lambda doc:
-00001120: 2020 6c65 6e28 5b74 2066 6f72 2074 2069    len([t for t i
-00001130: 6e20 646f 6320 6966 2074 2e64 6570 5f20  n doc if t.dep_ 
-00001140: 3d3d 2027 636f 6e6a 2720 616e 6420 742e  == 'conj' and t.
-00001150: 6865 6164 2e64 6570 5f20 3d3d 2027 524f  head.dep_ == 'RO
-00001160: 4f54 275d 2920 3e20 300a 736e 745f 736f  OT']) > 0.snt_so
-00001170: 7572 6365 0909 3d20 6c61 6d62 6461 2073  urce..= lambda s
-00001180: 6964 2c20 646f 633a 207b 2774 7970 6527  id, doc: {'type'
-00001190: 3a27 736e 7427 2c20 2773 7263 273a 2073  :'snt', 'src': s
-000011a0: 6964 2c20 2773 6e74 273a 646f 632e 7465  id, 'snt':doc.te
-000011b0: 7874 2c20 2770 7265 645f 6f66 6673 6574  xt, 'pred_offset
-000011c0: 273a 2070 7265 645f 6f66 6673 6574 2864  ': pred_offset(d
-000011d0: 6f63 292c 2009 2770 6f73 7461 6727 3a27  oc), .'postag':'
-000011e0: 5f5e 2027 202b 2027 2027 2e6a 6f69 6e28  _^ ' + ' '.join(
-000011f0: 5b66 227b 742e 7465 7874 7d5f 7b74 2e6c  [f"{t.text}_{t.l
-00001200: 656d 6d61 5f7d 5f7b 742e 706f 735f 7d5f  emma_}_{t.pos_}_
-00001210: 7b74 2e74 6167 5f7d 2220 6966 2074 2e74  {t.tag_}" if t.t
-00001220: 6578 7420 3d3d 2074 2e74 6578 742e 6c6f  ext == t.text.lo
-00001230: 7765 7228 2920 656c 7365 2066 227b 742e  wer() else f"{t.
-00001240: 7465 7874 7d5f 7b74 2e74 6578 742e 6c6f  text}_{t.text.lo
-00001250: 7765 7228 297d 5f7b 742e 6c65 6d6d 615f  wer()}_{t.lemma_
-00001260: 7d5f 7b74 2e70 6f73 5f7d 5f7b 742e 7461  }_{t.pos_}_{t.ta
-00001270: 675f 7d22 2066 6f72 2074 2069 6e20 646f  g_}" for t in do
-00001280: 635d 2920 2b20 2720 5f24 272c 2020 2774  c]) + ' _$',  't
-00001290: 6327 3a20 6c65 6e28 646f 6329 7d0a 7072  c': len(doc)}.pr
-000012a0: 6564 5f6f 6666 7365 7409 093d 206c 616d  ed_offset..= lam
-000012b0: 6264 6120 646f 633a 2028 2061 7220 3a3d  bda doc: ( ar :=
-000012c0: 205b 2074 2e69 2066 6f72 2074 2069 6e20   [ t.i for t in 
-000012d0: 646f 6320 6966 2074 2e64 6570 5f20 3d3d  doc if t.dep_ ==
-000012e0: 2022 524f 4f54 225d 2c20 6f66 6673 6574   "ROOT"], offset
-000012f0: 203a 3d20 6172 5b30 5d20 6966 206c 656e   := ar[0] if len
-00001300: 2861 7229 203e 2030 2065 6c73 6520 302c  (ar) > 0 else 0,
-00001310: 206f 6666 7365 742f 2820 6c65 6e28 646f   offset/( len(do
-00001320: 6329 202b 2030 2e31 2920 295b 2d31 5d0a  c) + 0.1) )[-1].
-00001330: 6861 735f 7a68 0909 093d 206c 616d 6264  has_zh...= lambd
-00001340: 6120 7320 3a20 616e 7928 5b63 2066 6f72  a s : any([c for
-00001350: 2063 2069 6e20 7320 6966 206f 7264 2863   c in s if ord(c
-00001360: 2920 3e20 3235 355d 290a 0a64 6566 2073  ) > 255])..def s
-00001370: 686f 7728 646f 6329 3a0a 0927 2727 2075  how(doc):..''' u
-00001380: 7365 6420 696e 2074 6865 206e 6f74 6562  sed in the noteb
-00001390: 6f6f 6b2c 2066 6f72 2064 6562 7567 2027  ook, for debug '
-000013a0: 2727 0a09 696d 706f 7274 2070 616e 6461  ''..import panda
-000013b0: 7320 6173 2070 640a 0972 6574 7572 6e20  s as pd..return 
-000013c0: 7064 2e44 6174 6146 7261 6d65 287b 2777  pd.DataFrame({'w
-000013d0: 6f72 6427 3a20 5b74 2e74 6578 7420 666f  ord': [t.text fo
-000013e0: 7220 7420 696e 2064 6f63 5d2c 2027 7461  r t in doc], 'ta
-000013f0: 6727 3a20 5b74 2e74 6167 5f20 666f 7220  g': [t.tag_ for 
-00001400: 7420 696e 2064 6f63 5d2c 2770 6f73 273a  t in doc],'pos':
-00001410: 205b 742e 706f 735f 2066 6f72 2074 2069   [t.pos_ for t i
-00001420: 6e20 646f 635d 2c27 6865 6164 273a 205b  n doc],'head': [
-00001430: 742e 6865 6164 2e6f 7274 685f 2066 6f72  t.head.orth_ for
-00001440: 2074 2069 6e20 646f 635d 2c27 6465 7027   t in doc],'dep'
-00001450: 3a20 5b74 2e64 6570 5f20 666f 7220 7420  : [t.dep_ for t 
-00001460: 696e 2064 6f63 5d2c 2027 6c65 6d6d 6127  in doc], 'lemma'
-00001470: 3a20 5b74 2e74 6578 742e 6c6f 7765 7228  : [t.text.lower(
-00001480: 2920 6966 2074 2e6c 656d 6d61 5f20 3d3d  ) if t.lemma_ ==
-00001490: 2027 2d50 524f 4e2d 2720 656c 7365 2074   '-PRON-' else t
-000014a0: 2e6c 656d 6d61 5f20 666f 7220 7420 696e  .lemma_ for t in
-000014b0: 2064 6f63 5d2c 0a09 276e 5f6c 6566 7473   doc],..'n_lefts
-000014c0: 273a 205b 2074 2e6e 5f6c 6566 7473 2066  ': [ t.n_lefts f
-000014d0: 6f72 2074 2069 6e20 646f 635d 2c20 276c  or t in doc], 'l
-000014e0: 6566 745f 6564 6765 273a 205b 2074 2e6c  eft_edge': [ t.l
-000014f0: 6566 745f 6564 6765 2e74 6578 7420 666f  eft_edge.text fo
-00001500: 7220 7420 696e 2064 6f63 5d2c 200a 0927  r t in doc], ..'
-00001510: 6e5f 7269 6768 7473 273a 205b 2074 2e6e  n_rights': [ t.n
-00001520: 5f72 6967 6874 7320 666f 7220 7420 696e  _rights for t in
-00001530: 2064 6f63 5d2c 2027 7269 6768 745f 6564   doc], 'right_ed
-00001540: 6765 273a 205b 2074 2e72 6967 6874 5f65  ge': [ t.right_e
-00001550: 6467 652e 7465 7874 2066 6f72 2074 2069  dge.text for t i
-00001560: 6e20 646f 635d 2c0a 0927 7375 6274 7265  n doc],..'subtre
-00001570: 6527 3a20 5b20 6c69 7374 2874 2e73 7562  e': [ list(t.sub
-00001580: 7472 6565 2920 666f 7220 7420 696e 2064  tree) for t in d
-00001590: 6f63 5d2c 2027 6368 696c 6472 656e 273a  oc], 'children':
-000015a0: 205b 206c 6973 7428 742e 6368 696c 6472   [ list(t.childr
-000015b0: 656e 2920 666f 7220 7420 696e 2064 6f63  en) for t in doc
-000015c0: 5d2c 2009 2327 6d6f 7270 6827 3a20 5b20  ], .#'morph': [ 
-000015d0: 742e 6d6f 7270 6820 666f 7220 7420 696e  t.morph for t in
-000015e0: 2064 6f63 5d2c 0a09 2765 6e74 5f74 7970   doc],..'ent_typ
-000015f0: 6527 3a20 5b20 742e 656e 745f 7479 7065  e': [ t.ent_type
-00001600: 5f20 666f 7220 7420 696e 2064 6f63 5d2c  _ for t in doc],
-00001610: 2027 656e 745f 6964 273a 205b 2074 2e65   'ent_id': [ t.e
-00001620: 6e74 5f69 645f 2066 6f72 2074 2069 6e20  nt_id_ for t in 
-00001630: 646f 635d 2c0a 097d 290a 0a64 6566 2070  doc],..})..def p
-00001640: 6172 7365 2873 6e74 2c20 6d65 7267 655f  arse(snt, merge_
-00001650: 6e70 3d20 4661 6c73 6529 3a0a 0927 2727  np= False):..'''
-00001660: 2075 7365 6420 696e 2074 6865 206e 6f74   used in the not
-00001670: 6562 6f6f 6b2c 2066 6f72 2064 6562 7567  ebook, for debug
-00001680: 2027 2727 0a09 646f 6320 3d20 7370 6163   '''..doc = spac
-00001690: 792e 6e6c 7028 736e 7429 0a09 6966 206d  y.nlp(snt)..if m
-000016a0: 6572 6765 5f6e 7020 3a20 7370 6163 792e  erge_np : spacy.
-000016b0: 6d65 7267 655f 6e70 7328 646f 6329 0a09  merge_nps(doc)..
-000016c0: 7265 7475 726e 2073 686f 7728 646f 6329  return show(doc)
-000016d0: 0a0a 7472 705f 7265 6c09 093d 206c 616d  ..trp_rel..= lam
-000016e0: 6264 6120 743a 2020 6622 7b74 2e64 6570  bda t:  f"{t.dep
-000016f0: 5f7d 5f7b 742e 6865 6164 2e70 6f73 5f7d  _}_{t.head.pos_}
-00001700: 5f7b 742e 706f 735f 7d22 2020 2320 646f  _{t.pos_}"  # do
-00001710: 626a 5f56 4552 425f 4e4f 554e 0a74 7270  bj_VERB_NOUN.trp
-00001720: 5f72 6576 6572 7365 203d 2073 6574 287b  _reverse = set({
-00001730: 2261 6d6f 645f 4e4f 554e 5f41 444a 222c  "amod_NOUN_ADJ",
-00001740: 226e 7375 626a 5f56 4552 425f 4e4f 554e  "nsubj_VERB_NOUN
-00001750: 227d 290a 7472 705f 746f 6b09 093d 206c  "}).trp_tok..= l
-00001760: 616d 6264 6120 646f 632c 2061 7272 3a20  ambda doc, arr: 
-00001770: 205b 2074 2066 6f72 2074 2069 6e20 646f   [ t for t in do
-00001780: 6320 6966 205b 2074 2e64 6570 5f2c 2074  c if [ t.dep_, t
-00001790: 2e68 6561 642e 706f 735f 2c20 742e 706f  .head.pos_, t.po
-000017a0: 735f 2c20 742e 6865 6164 2e6c 656d 6d61  s_, t.head.lemma
-000017b0: 5f2c 2074 2e6c 656d 6d61 5f20 5d20 3d3d  _, t.lemma_ ] ==
-000017c0: 2061 7272 205d 2023 2061 7272 2069 7320   arr ] # arr is 
-000017d0: 6578 6163 746c 7920 3520 6c69 7374 200a  exactly 5 list .
-000017e0: 676f 765f 6465 7009 093d 206c 616d 6264  gov_dep..= lambd
-000017f0: 6120 7265 6c2c 2061 7272 203a 2028 6172  a rel, arr : (ar
-00001800: 725b 305d 2c20 6172 725b 315d 2920 6966  r[0], arr[1]) if
-00001810: 206c 656d 6d61 5f6f 7264 6572 2e67 6574   lemma_order.get
-00001820: 2872 656c 2c20 5472 7565 2920 656c 7365  (rel, True) else
-00001830: 2028 6172 725b 315d 2c20 6172 725b 305d   (arr[1], arr[0]
-00001840: 2920 2023 206f 7065 6e20 646f 6f72 0a68  )  # open door.h
-00001850: 6974 5f74 7270 0909 3d20 6c61 6d62 6461  it_trp..= lambda
-00001860: 2074 2c20 5f72 656c 2c20 5f67 6f76 5f64   t, _rel, _gov_d
-00001870: 6570 3a20 2020 5f72 656c 203d 3d20 7472  ep:   _rel == tr
-00001880: 705f 7265 6c28 7429 2061 6e64 205f 676f  p_rel(t) and _go
-00001890: 765f 6465 7020 3d3d 2028 742e 6865 6164  v_dep == (t.head
-000018a0: 2e6c 656d 6d61 5f2c 2074 2e6c 656d 6d61  .lemma_, t.lemma
-000018b0: 5f29 0a74 7270 5f68 6967 6809 3d20 6c61  _).trp_high.= la
-000018c0: 6d62 6461 2064 6f63 2c20 692c 2069 6865  mbda doc, i, ihe
-000018d0: 6164 203a 2020 2022 222e 6a6f 696e 285b  ad :   "".join([
-000018e0: 2066 223c 623e 7b74 2e74 6578 745f 7769   f"<b>{t.text_wi
-000018f0: 7468 5f77 737d 3c2f 623e 2220 6966 2074  th_ws}</b>" if t
-00001900: 2e69 2069 6e20 2869 2c20 6968 6561 6429  .i in (i, ihead)
-00001910: 2065 6c73 6520 742e 7465 7874 5f77 6974   else t.text_wit
-00001920: 685f 7773 2066 6f72 2074 2069 6e20 646f  h_ws for t in do
-00001930: 6320 5d29 0a6c 656d 5f68 6967 6809 3d20  c ]).lem_high.= 
-00001940: 6c61 6d62 6461 2064 6f63 2c20 6c65 6d20  lambda doc, lem 
-00001950: 3a20 2020 2222 2e6a 6f69 6e28 5b20 6622  :   "".join([ f"
-00001960: 3c62 3e7b 742e 7465 7874 5f77 6974 685f  <b>{t.text_with_
-00001970: 7773 7d3c 2f62 3e22 2069 6620 742e 6c65  ws}</b>" if t.le
-00001980: 6d6d 615f 203d 3d20 6c65 6d20 656c 7365  mma_ == lem else
-00001990: 2074 2e74 6578 745f 7769 7468 5f77 7320   t.text_with_ws 
-000019a0: 666f 7220 7420 696e 2064 6f63 205d 2920  for t in doc ]) 
-000019b0: 2320 6869 6768 6c69 6768 7420 7468 6520  # highlight the 
-000019c0: 6669 7273 7420 6c65 6d6d 6120 0a76 705f  first lemma .vp_
-000019d0: 7370 616e 0909 3d20 6c61 6d62 6461 2064  span..= lambda d
-000019e0: 6f63 2c69 6265 672c 6965 6e64 3a20 646f  oc,ibeg,iend: do
-000019f0: 635b 6962 6567 5d2e 6c65 6d6d 615f 202b  c[ibeg].lemma_ +
-00001a00: 2022 2022 202b 2064 6f63 5b69 6265 672b   " " + doc[ibeg+
-00001a10: 313a 6965 6e64 5d2e 7465 7874 2e6c 6f77  1:iend].text.low
-00001a20: 6572 2829 0a0a 6465 6620 6879 6228 646f  er()..def hyb(do
-00001a30: 632c 2073 7461 7274 2c20 7061 7429 3a20  c, start, pat): 
-00001a40: 236c 3a6c 656d 6d61 2078 3a74 6578 742c  #l:lemma x:text,
-00001a50: 2070 3a70 6f73 2074 3a74 6167 202c 2065   p:pos t:tag , e
-00001a60: 3a65 6e74 5f74 7970 6520 0a09 6172 7220  :ent_type ..arr 
-00001a70: 3d20 5b5d 0a09 666f 7220 692c 6320 696e  = []..for i,c in
-00001a80: 2065 6e75 6d65 7261 7465 2870 6174 293a   enumerate(pat):
-00001a90: 200a 0909 6966 2063 203d 3d20 276c 273a   ...if c == 'l':
-00001aa0: 0961 7272 2e61 7070 656e 6428 646f 635b  .arr.append(doc[
-00001ab0: 7374 6172 7420 2b69 5d2e 6c65 6d6d 615f  start +i].lemma_
-00001ac0: 290a 0909 656c 6966 2063 203d 3d20 2770  )...elif c == 'p
-00001ad0: 273a 0961 7272 2e61 7070 656e 6428 646f  ':.arr.append(do
-00001ae0: 635b 7374 6172 7420 2b69 5d2e 706f 735f  c[start +i].pos_
-00001af0: 290a 0909 656c 6966 2063 203d 3d20 2774  )...elif c == 't
-00001b00: 273a 0961 7272 2e61 7070 656e 6428 646f  ':.arr.append(do
-00001b10: 635b 7374 6172 7420 2b69 5d2e 7461 675f  c[start +i].tag_
-00001b20: 290a 0909 656c 6966 2063 203d 3d20 2765  )...elif c == 'e
-00001b30: 273a 0961 7272 2e61 7070 656e 6428 646f  ':.arr.append(do
-00001b40: 635b 7374 6172 7420 2b69 5d2e 656e 745f  c[start +i].ent_
-00001b50: 7479 7065 5f29 0a09 0965 6c69 6620 6320  type_)...elif c 
-00001b60: 3d3d 2027 7827 3a09 6172 722e 6170 7065  == 'x':.arr.appe
-00001b70: 6e64 2864 6f63 5b73 7461 7274 202b 695d  nd(doc[start +i]
-00001b80: 2e74 6578 742e 6c6f 7765 7228 2929 0a09  .text.lower())..
-00001b90: 0965 6c73 6520 3a09 0909 6172 722e 6170  .else :...arr.ap
-00001ba0: 7065 6e64 2864 6f63 5b73 7461 7274 202b  pend(doc[start +
-00001bb0: 695d 2e74 6578 742e 6c6f 7765 7228 2929  i].text.lower())
-00001bc0: 0a09 7265 7475 726e 2027 2027 2e6a 6f69  ..return ' '.joi
-00001bd0: 6e28 6172 7229 200a 0a64 6566 206b 705f  n(arr) ..def kp_
-00001be0: 7370 616e 2864 6f63 2c20 7374 6172 742c  span(doc, start,
-00001bf0: 2065 6e64 2c20 6e61 6d65 293a 2020 2320   end, name):  # 
-00001c00: 6261 7365 3a56 4552 423a 6265 5f76 626e  base:VERB:be_vbn
-00001c10: 5f70 3a62 6520 6261 7365 6420 6f6e 2020  _p:be based on  
-00001c20: 207c 206c 656d 2c20 706f 732c 2074 7970   | lem, pos, typ
-00001c30: 652c 2063 6875 6e6b 200a 0969 6620 6e61  e, chunk ..if na
-00001c40: 6d65 2e73 7461 7274 7377 6974 6828 2776  me.startswith('v
-00001c50: 2729 3a09 0972 6574 7572 6e20 2864 6f63  '):..return (doc
-00001c60: 5b73 7461 7274 5d2e 6c65 6d6d 615f 2c64  [start].lemma_,d
-00001c70: 6f63 5b73 7461 7274 5d2e 706f 735f 2c20  oc[start].pos_, 
-00001c80: 6e61 6d65 2c76 705f 7370 616e 2864 6f63  name,vp_span(doc
-00001c90: 2c73 7461 7274 2c65 6e64 2920 290a 0965  ,start,end) )..e
-00001ca0: 6c69 6620 6e61 6d65 2e73 7461 7274 7377  lif name.startsw
-00001cb0: 6974 6828 2262 655f 2229 203a 0972 6574  ith("be_") :.ret
-00001cc0: 7572 6e20 2864 6f63 5b73 7461 7274 2b31  urn (doc[start+1
-00001cd0: 5d2e 6c65 6d6d 615f 2c64 6f63 5b73 7461  ].lemma_,doc[sta
-00001ce0: 7274 2b31 5d2e 706f 735f 2c6e 616d 652c  rt+1].pos_,name,
-00001cf0: 7670 5f73 7061 6e28 646f 632c 7374 6172  vp_span(doc,star
-00001d00: 742c 656e 6429 290a 0965 6c69 6620 6e61  t,end))..elif na
-00001d10: 6d65 2069 6e20 2827 6170 272c 2770 7027  me in ('ap','pp'
-00001d20: 2c27 5665 6e64 2729 3a72 6574 7572 6e20  ,'Vend'):return 
-00001d30: 2864 6f63 5b65 6e64 2d31 5d2e 6c65 6d6d  (doc[end-1].lemm
-00001d40: 615f 2c64 6f63 5b65 6e64 2d31 5d2e 706f  a_,doc[end-1].po
-00001d50: 735f 2c6e 616d 652c 646f 635b 7374 6172  s_,name,doc[star
-00001d60: 743a 656e 645d 2e74 6578 742e 6c6f 7765  t:end].text.lowe
-00001d70: 7228 2929 0a09 656c 7365 3a09 0909 0909  r())..else:.....
-00001d80: 0909 7265 7475 726e 2028 646f 635b 7374  ..return (doc[st
-00001d90: 6172 745d 2e6c 656d 6d61 5f2c 646f 635b  art].lemma_,doc[
-00001da0: 7374 6172 745d 2e70 6f73 5f2c 6e61 6d65  start].pos_,name
-00001db0: 2c64 6f63 5b73 7461 7274 3a65 6e64 5d2e  ,doc[start:end].
-00001dc0: 7465 7874 2e6c 6f77 6572 2829 290a 0a6b  text.lower())..k
-00001dd0: 705f 7275 6c65 7320 3d20 7b0a 2256 656e  p_rules = {."Ven
-00001de0: 6422 3a5b 5b7b 2250 4f53 223a 207b 2249  d":[[{"POS": {"I
-00001df0: 4e22 3a20 5b22 4155 5822 2c22 5645 5242  N": ["AUX","VERB
-00001e00: 225d 7d7d 2c7b 2250 4f53 223a 207b 2249  "]}},{"POS": {"I
-00001e10: 4e22 3a20 5b22 4144 5622 5d7d 2c20 224f  N": ["ADV"]}, "O
-00001e20: 5022 3a20 222a 227d 2c20 7b22 504f 5322  P": "*"}, {"POS"
-00001e30: 3a20 7b22 494e 223a 205b 2241 444a 222c  : {"IN": ["ADJ",
-00001e40: 2256 4552 4222 5d7d 2c20 224f 5022 3a20  "VERB"]}, "OP": 
-00001e50: 222a 227d 2c7b 2250 4f53 223a 207b 2249  "*"},{"POS": {"I
-00001e60: 4e22 3a20 5b22 5041 5254 222c 2241 4450  N": ["PART","ADP
-00001e70: 222c 2254 4f22 5d7d 2c20 224f 5022 3a20  ","TO"]}, "OP": 
-00001e80: 222a 227d 2c7b 2250 4f53 223a 2027 5645  "*"},{"POS": 'VE
-00001e90: 5242 277d 5d5d 2c20 2320 636f 756c 6420  RB'}]], # could 
-00001ea0: 6861 7264 6c79 2077 6169 7420 746f 206d  hardly wait to m
-00001eb0: 6565 740a 2276 7022 3a20 205b 5b7b 2750  eet."vp":  [[{'P
-00001ec0: 4f53 273a 2027 5645 5242 277d 2c7b 2250  OS': 'VERB'},{"P
-00001ed0: 4f53 223a 207b 2249 4e22 3a20 5b22 4445  OS": {"IN": ["DE
-00001ee0: 5422 2c22 4144 5022 2c22 4144 4a22 5d7d  T","ADP","ADJ"]}
-00001ef0: 2c20 224f 5022 3a20 222a 227d 2c7b 2250  , "OP": "*"},{"P
-00001f00: 4f53 223a 2027 4e4f 554e 277d 2c20 7b22  OS": 'NOUN'}, {"
-00001f10: 504f 5322 3a20 7b22 494e 223a 205b 2241  POS": {"IN": ["A
-00001f20: 4450 222c 2254 4f22 5d7d 2c20 224f 5022  DP","TO"]}, "OP"
-00001f30: 3a20 222a 227d 5d2c 205b 7b27 504f 5327  : "*"}], [{'POS'
-00001f40: 3a20 2756 4552 4227 7d2c 7b22 504f 5322  : 'VERB'},{"POS"
-00001f50: 3a20 7b22 494e 223a 205b 2244 4554 222c  : {"IN": ["DET",
-00001f60: 2241 4450 222c 2241 444a 222c 2254 4f22  "ADP","ADJ","TO"
-00001f70: 2c22 5041 5254 225d 7d2c 2022 4f50 223a  ,"PART"]}, "OP":
-00001f80: 2022 2a22 7d2c 7b22 504f 5322 3a20 2756   "*"},{"POS": 'V
-00001f90: 4552 4227 7d5d 5d2c 2023 2077 6169 7420  ERB'}]], # wait 
-00001fa0: 746f 206d 6565 740a 2270 7022 3a20 205b  to meet."pp":  [
-00001fb0: 5b7b 2750 4f53 273a 2027 4144 5027 7d2c  [{'POS': 'ADP'},
-00001fc0: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
-00001fd0: 2244 4554 222c 224e 554d 222c 2241 444a  "DET","NUM","ADJ
-00001fe0: 222c 2750 554e 4354 272c 2743 4f4e 4a27  ",'PUNCT','CONJ'
-00001ff0: 5d7d 2c20 224f 5022 3a20 222a 227d 2c7b  ]}, "OP": "*"},{
-00002000: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
-00002010: 4e4f 554e 222c 2250 4152 5422 5d7d 2c20  NOUN","PART"]}, 
-00002020: 224f 5022 3a20 222b 227d 5d5d 2c20 2020  "OP": "+"}]],   
-00002030: 200a 2261 7022 3a20 205b 5b7b 2250 4f53   ."ap":  [[{"POS
-00002040: 223a 207b 2249 4e22 3a20 5b22 4144 5622  ": {"IN": ["ADV"
-00002050: 5d7d 2c20 224f 5022 3a20 222b 227d 2c20  ]}, "OP": "+"}, 
-00002060: 7b22 504f 5322 3a20 2741 444a 277d 5d5d  {"POS": 'ADJ'}]]
-00002070: 2c20 200a 2276 7072 7422 3a09 5b5b 7b22  ,  ."vprt":.[[{"
-00002080: 504f 5322 3a20 2756 4552 4227 2c20 2254  POS": 'VERB', "T
-00002090: 4147 223a 207b 224e 4f54 5f49 4e22 3a20  AG": {"NOT_IN": 
-000020a0: 5b22 5642 4e22 5d7d 7d2c 207b 2250 4f53  ["VBN"]}}, {"POS
-000020b0: 223a 207b 2249 4e22 3a20 5b22 5052 4550  ": {"IN": ["PREP
-000020c0: 222c 2022 4144 5022 2c27 544f 275d 7d2c  ", "ADP",'TO']},
-000020d0: 2022 4f50 223a 2022 2b22 7d5d 5d2c 2020   "OP": "+"}]],  
-000020e0: 2023 206c 6f6f 6b20 7570 202f 6c6f 6f6b   # look up /look
-000020f0: 2075 7020 6672 6f6d 2c20 2063 6f6d 7075   up from,  compu
-00002100: 7465 6420 7477 6963 650a 2276 746f 7622  ted twice."vtov"
-00002110: 3a09 5b5b 7b22 504f 5322 3a20 2756 4552  :.[[{"POS": 'VER
-00002120: 4227 2c20 2254 4147 223a 207b 224e 4f54  B', "TAG": {"NOT
-00002130: 5f49 4e22 3a20 5b22 5642 4e22 5d7d 7d2c  _IN": ["VBN"]}},
-00002140: 207b 2254 4147 223a 2027 544f 277d 2c7b   {"TAG": 'TO'},{
-00002150: 2254 4147 223a 2027 5642 277d 5d5d 2c20  "TAG": 'VB'}]], 
-00002160: 2020 2320 706c 616e 2074 6f20 676f 0a22    # plan to go."
-00002170: 7676 6267 223a 095b 5b7b 2250 4f53 223a  vvbg":.[[{"POS":
-00002180: 2027 5645 5242 272c 2022 5441 4722 3a20   'VERB', "TAG": 
-00002190: 7b22 4e4f 545f 494e 223a 205b 2256 424e  {"NOT_IN": ["VBN
-000021a0: 225d 7d7d 2c20 7b22 5441 4722 3a20 2756  "]}}, {"TAG": 'V
-000021b0: 4247 277d 5d5d 2c20 2020 2320 636f 6e73  BG'}]],   # cons
-000021c0: 6964 6572 2067 6f69 6e67 0a22 7670 6722  ider going."vpg"
-000021d0: 3a09 5b5b 7b22 504f 5322 3a20 2756 4552  :.[[{"POS": 'VER
-000021e0: 4227 2c20 2254 4147 223a 207b 224e 4f54  B', "TAG": {"NOT
-000021f0: 5f49 4e22 3a20 5b22 5642 4e22 5d7d 7d2c  _IN": ["VBN"]}},
-00002200: 207b 2250 4f53 223a 207b 2249 4e22 3a20   {"POS": {"IN": 
-00002210: 5b22 5052 4550 222c 2022 4144 5022 2c27  ["PREP", "ADP",'
-00002220: 5041 5254 275d 7d2c 2022 4f50 223a 2022  PART']}, "OP": "
-00002230: 2b22 7d2c 7b22 5441 4722 3a20 2756 4247  +"},{"TAG": 'VBG
-00002240: 277d 5d5d 2c20 2020 2320 696e 7369 7374  '}]],   # insist
-00002250: 6564 206f 6e20 676f 696e 670a 2262 655f  ed on going."be_
-00002260: 7662 6e5f 7022 3a20 5b5b 7b27 4c45 4d4d  vbn_p": [[{'LEMM
-00002270: 4127 3a20 2762 6527 7d2c 7b22 5441 4722  A': 'be'},{"TAG"
-00002280: 3a20 7b22 494e 223a 205b 2256 424e 225d  : {"IN": ["VBN"]
-00002290: 7d7d 2c20 7b22 504f 5322 3a20 7b22 494e  }}, {"POS": {"IN
-000022a0: 223a 205b 2250 5245 5022 2c20 2241 4450  ": ["PREP", "ADP
-000022b0: 222c 2750 4152 5427 5d7d 7d5d 5d2c 2020  ",'PART']}}]],  
-000022c0: 2023 2062 6173 653a 5645 5242 3a62 655f   # base:VERB:be_
-000022d0: 7662 6e5f 703a 6265 2062 6173 6564 206f  vbn_p:be based o
-000022e0: 6e20 2020 0a22 6265 5f61 646a 5f70 223a  n   ."be_adj_p":
-000022f0: 205b 5b7b 274c 454d 4d41 273a 2027 6265   [[{'LEMMA': 'be
-00002300: 277d 2c7b 2250 4f53 223a 207b 2249 4e22  '},{"POS": {"IN"
-00002310: 3a20 5b22 4144 4a22 5d7d 7d2c 207b 2250  : ["ADJ"]}}, {"P
-00002320: 4f53 223a 207b 2249 4e22 3a20 5b22 5052  OS": {"IN": ["PR
-00002330: 4550 222c 2022 4144 5022 2c27 5041 5254  EP", "ADP",'PART
-00002340: 275d 7d7d 5d5d 2c20 2020 2320 6265 2061  ']}}]],   # be a
-00002350: 6e67 7279 2077 6974 680a 7d20 2366 6f72  ngry with.} #for
-00002360: 206e 616d 652c 2069 6265 672c 6965 6e64   name, ibeg,iend
-00002370: 2069 6e20 6d61 7463 6865 7228 646f 6329   in matcher(doc)
-00002380: 203a 2070 7269 6e74 2873 7061 6379 2e6e   : print(spacy.n
-00002390: 6c70 2e76 6f63 6162 5b6e 616d 655d 2e74  lp.vocab[name].t
-000023a0: 6578 742c 2064 6f63 5b69 6265 673a 6965  ext, doc[ibeg:ie
-000023b0: 6e64 5d2e 7465 7874 290a 0a64 6566 206b  nd].text)..def k
-000023c0: 705f 6d61 7463 6865 7228 646f 6329 3a20  p_matcher(doc): 
-000023d0: 235b 2827 7665 6e64 272c 2027 636f 6e73  #[('vend', 'cons
-000023e0: 6964 6572 2067 6f69 6e67 272c 2031 2c20  ider going', 1, 
-000023f0: 3329 2c20 2827 7670 272c 2027 636f 6e73  3), ('vp', 'cons
-00002400: 6964 6572 2067 6f69 6e67 272c 2031 2c20  ider going', 1, 
-00002410: 3329 2c20 2827 7676 6267 272c 2027 636f  3), ('vvbg', 'co
-00002420: 6e73 6964 6572 2067 6f69 6e67 272c 2031  nsider going', 1
-00002430: 2c20 3329 2c20 2827 7670 7274 272c 2027  , 3), ('vprt', '
-00002440: 676f 696e 6720 746f 272c 2032 2c20 3429  going to', 2, 4)
-00002450: 5d0a 0969 6620 6e6f 7420 6861 7361 7474  ]..if not hasatt
-00002460: 7228 6b70 5f6d 6174 6368 6572 2c20 276d  r(kp_matcher, 'm
-00002470: 6174 6368 6572 2729 3a20 0a09 096b 705f  atcher'): ...kp_
-00002480: 6d61 7463 6865 722e 6d61 7463 6865 7220  matcher.matcher 
-00002490: 3d20 4d61 7463 6865 7228 7370 6163 792e  = Matcher(spacy.
-000024a0: 6e6c 702e 766f 6361 6229 0a09 095b 6b70  nlp.vocab)...[kp
-000024b0: 5f6d 6174 6368 6572 2e6d 6174 6368 6572  _matcher.matcher
-000024c0: 2e61 6464 286e 616d 652c 2070 6174 7465  .add(name, patte
-000024d0: 726e 732c 2020 6772 6565 6479 203d 274c  rns,  greedy ='L
-000024e0: 4f4e 4745 5354 2729 2066 6f72 206e 616d  ONGEST') for nam
-000024f0: 652c 2070 6174 7465 726e 7320 696e 206b  e, patterns in k
-00002500: 705f 7275 6c65 732e 6974 656d 7328 2920  p_rules.items() 
-00002510: 5d0a 0974 7570 7320 3d20 7365 7428 2920  ]..tups = set() 
-00002520: 2023 2072 656d 6f76 6520 7468 6520 6475   # remove the du
-00002530: 706c 6963 6174 6564 2065 6e74 7269 6573  plicated entries
-00002540: 200a 095b 7475 7073 2e61 6464 2820 6b70   ..[tups.add( kp
-00002550: 5f73 7061 6e28 646f 632c 6962 6567 2c69  _span(doc,ibeg,i
-00002560: 656e 642c 2073 7061 6379 2e6e 6c70 2e76  end, spacy.nlp.v
-00002570: 6f63 6162 5b6e 616d 655d 2e74 6578 7429  ocab[name].text)
-00002580: 2029 2066 6f72 206e 616d 652c 2069 6265   ) for name, ibe
-00002590: 672c 6965 6e64 2069 6e20 6b70 5f6d 6174  g,iend in kp_mat
-000025a0: 6368 6572 2e6d 6174 6368 6572 2864 6f63  cher.matcher(doc
-000025b0: 295d 200a 0972 6574 7572 6e20 7475 7073  )] ..return tups
-000025c0: 0a0a 6465 6620 7275 6c65 7228 736e 742c  ..def ruler(snt,
-000025d0: 206e 616d 653a 7374 723d 2773 6d27 293a   name:str='sm'):
-000025e0: 0a09 2727 2720 646f 632e 7370 616e 735b  ..''' doc.spans[
-000025f0: 2772 756c 6572 275d 2032 3032 332e 312e  'ruler'] 2023.1.
-00002600: 3231 2027 2727 0a09 6966 206e 6f74 2068  21 '''..if not h
-00002610: 6173 6174 7472 2872 756c 6572 2c20 6e61  asattr(ruler, na
-00002620: 6d65 293a 2020 0a09 095f 6e6c 7020 3d20  me):  ..._nlp = 
-00002630: 7370 6163 792e 6c6f 6164 2866 2765 6e5f  spacy.load(f'en_
-00002640: 636f 7265 5f77 6562 5f7b 6e61 6d65 7d27  core_web_{name}'
-00002650: 290a 0909 7365 7461 7474 7228 7275 6c65  )...setattr(rule
-00002660: 722c 206e 616d 652c 205f 6e6c 7020 290a  r, name, _nlp ).
-00002670: 0909 5f72 756c 6572 203d 205f 6e6c 702e  .._ruler = _nlp.
-00002680: 6164 645f 7069 7065 2822 7370 616e 5f72  add_pipe("span_r
-00002690: 756c 6572 2229 0a09 0970 6174 7465 726e  uler")...pattern
-000026a0: 7320 3d20 5b7b 226c 6162 656c 223a 2022  s = [{"label": "
-000026b0: 5050 222c 2022 7061 7474 6572 6e22 3a20  PP", "pattern": 
-000026c0: 5b7b 2750 4f53 273a 2027 4144 5027 7d2c  [{'POS': 'ADP'},
-000026d0: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
-000026e0: 2244 4554 222c 224e 554d 222c 2241 444a  "DET","NUM","ADJ
-000026f0: 222c 2750 554e 4354 272c 2743 4f4e 4a27  ",'PUNCT','CONJ'
-00002700: 5d7d 2c20 224f 5022 3a20 222a 227d 2c7b  ]}, "OP": "*"},{
-00002710: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
-00002720: 4e4f 554e 222c 2250 4152 5422 2c22 5052  NOUN","PART","PR
-00002730: 4f50 4e22 5d7d 2c20 224f 5022 3a20 222b  OPN"]}, "OP": "+
-00002740: 227d 5d7d 2c0a 2020 2020 2020 2020 2020  "}]},.          
-00002750: 2020 7b22 6c61 6265 6c22 3a20 2256 5022    {"label": "VP"
-00002760: 2c20 2270 6174 7465 726e 223a 205b 7b27  , "pattern": [{'
-00002770: 504f 5327 3a20 2756 4552 4227 7d2c 7b22  POS': 'VERB'},{"
-00002780: 504f 5322 3a20 7b22 494e 223a 205b 2244  POS": {"IN": ["D
-00002790: 4554 222c 2241 4450 222c 2241 444a 225d  ET","ADP","ADJ"]
-000027a0: 7d2c 2022 4f50 223a 2022 2a22 7d2c 7b22  }, "OP": "*"},{"
-000027b0: 504f 5322 3a20 274e 4f55 4e27 7d2c 207b  POS": 'NOUN'}, {
-000027c0: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
-000027d0: 4144 5022 2c22 544f 225d 7d2c 2022 4f50  ADP","TO"]}, "OP
-000027e0: 223a 2022 2a22 7d5d 7d2c 0a09 0909 7b22  ": "*"}]},....{"
-000027f0: 6c61 6265 6c22 3a20 2256 656e 6422 2c20  label": "Vend", 
-00002800: 2270 6174 7465 726e 223a 205b 7b22 504f  "pattern": [{"PO
-00002810: 5322 3a20 7b22 494e 223a 205b 2241 5558  S": {"IN": ["AUX
-00002820: 222c 2256 4552 4222 5d7d 7d2c 7b22 504f  ","VERB"]}},{"PO
-00002830: 5322 3a20 7b22 494e 223a 205b 2241 4456  S": {"IN": ["ADV
-00002840: 225d 7d2c 2022 4f50 223a 2022 2a22 7d2c  "]}, "OP": "*"},
-00002850: 207b 2250 4f53 223a 207b 2249 4e22 3a20   {"POS": {"IN": 
-00002860: 5b22 4144 4a22 2c22 5645 5242 225d 7d2c  ["ADJ","VERB"]},
-00002870: 2022 4f50 223a 2022 2a22 7d2c 7b22 504f   "OP": "*"},{"PO
-00002880: 5322 3a20 7b22 494e 223a 205b 2250 4152  S": {"IN": ["PAR
-00002890: 5422 2c22 4144 5022 2c22 544f 225d 7d2c  T","ADP","TO"]},
-000028a0: 2022 4f50 223a 2022 2a22 7d2c 7b22 504f   "OP": "*"},{"PO
-000028b0: 5322 3a20 2756 4552 4227 7d5d 7d2c 0a09  S": 'VERB'}]},..
-000028c0: 0909 7b22 6c61 6265 6c22 3a20 2241 5022  ..{"label": "AP"
-000028d0: 2c20 2270 6174 7465 726e 223a 205b 7b22  , "pattern": [{"
-000028e0: 504f 5322 3a20 7b22 494e 223a 205b 2241  POS": {"IN": ["A
-000028f0: 4456 225d 7d2c 2022 4f50 223a 2022 2b22  DV"]}, "OP": "+"
-00002900: 7d2c 207b 2250 4f53 223a 2027 4144 4a27  }, {"POS": 'ADJ'
-00002910: 7d5d 7d2c 0a09 0909 7b22 6c61 6265 6c22  }]},....{"label"
-00002920: 3a20 2276 746f 7622 2c20 2270 6174 7465  : "vtov", "patte
-00002930: 726e 223a 205b 7b22 504f 5322 3a20 2756  rn": [{"POS": 'V
-00002940: 4552 4227 2c20 2254 4147 223a 207b 224e  ERB', "TAG": {"N
-00002950: 4f54 5f49 4e22 3a20 5b22 5642 4e22 5d7d  OT_IN": ["VBN"]}
-00002960: 7d2c 207b 2254 4147 223a 2027 544f 277d  }, {"TAG": 'TO'}
-00002970: 2c7b 2254 4147 223a 2027 5642 277d 5d7d  ,{"TAG": 'VB'}]}
-00002980: 2c0a 0909 097b 226c 6162 656c 223a 2022  ,....{"label": "
-00002990: 7676 6267 222c 2022 7061 7474 6572 6e22  vvbg", "pattern"
-000029a0: 3a20 5b7b 2250 4f53 223a 2027 5645 5242  : [{"POS": 'VERB
-000029b0: 272c 2022 5441 4722 3a20 7b22 4e4f 545f  ', "TAG": {"NOT_
-000029c0: 494e 223a 205b 2256 424e 225d 7d7d 2c20  IN": ["VBN"]}}, 
-000029d0: 7b22 5441 4722 3a20 2756 4247 277d 5d7d  {"TAG": 'VBG'}]}
-000029e0: 2c0a 0909 097b 226c 6162 656c 223a 2022  ,....{"label": "
-000029f0: 7670 7274 222c 2022 7061 7474 6572 6e22  vprt", "pattern"
-00002a00: 3a20 5b7b 2250 4f53 223a 2027 5645 5242  : [{"POS": 'VERB
-00002a10: 272c 2022 5441 4722 3a20 7b22 4e4f 545f  ', "TAG": {"NOT_
-00002a20: 494e 223a 205b 2256 424e 225d 7d7d 2c20  IN": ["VBN"]}}, 
-00002a30: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
-00002a40: 2250 5245 5022 2c20 2241 4450 222c 2754  "PREP", "ADP",'T
-00002a50: 4f27 5d7d 2c20 224f 5022 3a20 222b 227d  O']}, "OP": "+"}
-00002a60: 5d7d 2c0a 0909 097b 226c 6162 656c 223a  ]},....{"label":
-00002a70: 2022 7670 6722 2c20 2270 6174 7465 726e   "vpg", "pattern
-00002a80: 223a 205b 7b22 504f 5322 3a20 2756 4552  ": [{"POS": 'VER
-00002a90: 4227 2c20 2254 4147 223a 207b 224e 4f54  B', "TAG": {"NOT
-00002aa0: 5f49 4e22 3a20 5b22 5642 4e22 5d7d 7d2c  _IN": ["VBN"]}},
-00002ab0: 207b 2250 4f53 223a 207b 2249 4e22 3a20   {"POS": {"IN": 
-00002ac0: 5b22 5052 4550 222c 2022 4144 5022 2c27  ["PREP", "ADP",'
-00002ad0: 5041 5254 275d 7d2c 2022 4f50 223a 2022  PART']}, "OP": "
-00002ae0: 2b22 7d2c 7b22 5441 4722 3a20 2756 4247  +"},{"TAG": 'VBG
-00002af0: 277d 5d7d 2c23 2069 6e73 6973 7465 6420  '}]},# insisted 
-00002b00: 6f6e 2067 6f69 6e67 0a09 0909 7b22 6c61  on going....{"la
-00002b10: 6265 6c22 3a20 2262 655f 7662 6e5f 7022  bel": "be_vbn_p"
-00002b20: 2c20 2270 6174 7465 726e 223a 205b 7b27  , "pattern": [{'
-00002b30: 4c45 4d4d 4127 3a20 2762 6527 7d2c 7b22  LEMMA': 'be'},{"
-00002b40: 5441 4722 3a20 7b22 494e 223a 205b 2256  TAG": {"IN": ["V
-00002b50: 424e 225d 7d7d 2c20 7b22 504f 5322 3a20  BN"]}}, {"POS": 
-00002b60: 7b22 494e 223a 205b 2250 5245 5022 2c20  {"IN": ["PREP", 
-00002b70: 2241 4450 222c 2750 4152 5427 5d7d 7d5d  "ADP",'PART']}}]
-00002b80: 7d2c 2320 6261 7365 3a56 4552 423a 6265  },# base:VERB:be
-00002b90: 5f76 626e 5f70 3a62 6520 6261 7365 6420  _vbn_p:be based 
-00002ba0: 6f6e 2020 200a 0909 097b 226c 6162 656c  on   ....{"label
-00002bb0: 223a 2022 6265 5f61 646a 5f70 222c 2022  ": "be_adj_p", "
-00002bc0: 7061 7474 6572 6e22 3a20 5b7b 274c 454d  pattern": [{'LEM
-00002bd0: 4d41 273a 2027 6265 277d 2c7b 2250 4f53  MA': 'be'},{"POS
-00002be0: 223a 207b 2249 4e22 3a20 5b22 4144 4a22  ": {"IN": ["ADJ"
-00002bf0: 5d7d 7d2c 207b 2250 4f53 223a 207b 2249  ]}}, {"POS": {"I
-00002c00: 4e22 3a20 5b22 5052 4550 222c 2022 4144  N": ["PREP", "AD
-00002c10: 5022 2c27 5041 5254 275d 7d7d 5d7d 2c23  P",'PART']}}]},#
-00002c20: 2062 6520 616e 6772 7920 7769 7468 0a09   be angry with..
-00002c30: 0909 5d0a 0909 5f72 756c 6572 2e61 6464  ..]..._ruler.add
-00002c40: 5f70 6174 7465 726e 7328 7061 7474 6572  _patterns(patter
-00002c50: 6e73 290a 0972 6574 7572 6e20 6765 7461  ns)..return geta
-00002c60: 7474 7228 7275 6c65 722c 206e 616d 6529  ttr(ruler, name)
-00002c70: 2873 6e74 2920 2023 7072 696e 7428 5b28  (snt)  #print([(
-00002c80: 7370 616e 2e74 6578 742c 2073 7061 6e2e  span.text, span.
-00002c90: 6c61 6265 6c5f 2920 666f 7220 7370 616e  label_) for span
-00002ca0: 2069 6e20 2064 6f63 2e73 7061 6e73 5b22   in  doc.spans["
-00002cb0: 7275 6c65 7222 5d20 5d29 0a0a 2320 6164  ruler"] ])..# ad
-00002cc0: 6465 6420 3230 3232 2e37 2e32 350a 706f  ded 2022.7.25.po
-00002cd0: 7374 5f6e 705f 7275 6c65 7320 3d20 7b20  st_np_rules = { 
-00002ce0: 2320 6166 7465 7220 6e70 2069 7320 6d65  # after np is me
-00002cf0: 7267 6564 200a 2276 5f6e 5f76 626e 223a  rged ."v_n_vbn":
-00002d00: 205b 5b7b 2250 4f53 223a 2027 5645 5242   [[{"POS": 'VERB
-00002d10: 272c 2022 5441 4722 3a20 7b22 4e4f 545f  ', "TAG": {"NOT_
-00002d20: 494e 223a 205b 2256 424e 225d 7d7d 2c7b  IN": ["VBN"]}},{
-00002d30: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
-00002d40: 4e4f 554e 225d 7d7d 2c20 7b22 5441 4722  NOUN"]}}, {"TAG"
-00002d50: 3a20 7b22 494e 223a 205b 2256 424e 225d  : {"IN": ["VBN"]
-00002d60: 7d7d 5d5d 2c20 2020 2320 6c65 6176 6520  }}]],   # leave 
-00002d70: 7468 6520 626f 6f6b 206f 7065 6e65 6420  the book opened 
-00002d80: 0a22 765f 6e5f 6164 6a22 3a20 5b5b 7b22  ."v_n_adj": [[{"
-00002d90: 504f 5322 3a20 2756 4552 4227 2c20 2254  POS": 'VERB', "T
-00002da0: 4147 223a 207b 224e 4f54 5f49 4e22 3a20  AG": {"NOT_IN": 
-00002db0: 5b22 5642 4e22 5d7d 7d2c 7b22 504f 5322  ["VBN"]}},{"POS"
-00002dc0: 3a20 7b22 494e 223a 205b 224e 4f55 4e22  : {"IN": ["NOUN"
-00002dd0: 5d7d 7d2c 207b 2250 4f53 223a 207b 2249  ]}}, {"POS": {"I
-00002de0: 4e22 3a20 5b22 4144 4a22 5d7d 7d5d 5d2c  N": ["ADJ"]}}]],
-00002df0: 0a7d 2023 666f 7220 6e61 6d65 2c20 6962  .} #for name, ib
-00002e00: 6567 2c69 656e 6420 696e 206d 6174 6368  eg,iend in match
-00002e10: 6572 2864 6f63 2920 3a20 7072 696e 7428  er(doc) : print(
-00002e20: 7370 6163 792e 6e6c 702e 766f 6361 625b  spacy.nlp.vocab[
-00002e30: 6e61 6d65 5d2e 7465 7874 2c20 646f 635b  name].text, doc[
-00002e40: 6962 6567 3a69 656e 645d 2e74 6578 7429  ibeg:iend].text)
-00002e50: 0a64 6566 2070 6f73 745f 6e70 5f6d 6174  .def post_np_mat
-00002e60: 6368 6572 2864 6f63 293a 200a 0969 6620  cher(doc): ..if 
-00002e70: 6e6f 7420 6861 7361 7474 7228 706f 7374  not hasattr(post
-00002e80: 5f6e 705f 6d61 7463 6865 722c 2027 6d61  _np_matcher, 'ma
-00002e90: 7463 6865 7227 293a 200a 0909 706f 7374  tcher'): ...post
-00002ea0: 5f6e 705f 6d61 7463 6865 722e 6d61 7463  _np_matcher.matc
-00002eb0: 6865 7220 3d20 4d61 7463 6865 7228 7370  her = Matcher(sp
-00002ec0: 6163 792e 6e6c 702e 766f 6361 6229 0a09  acy.nlp.vocab)..
-00002ed0: 095b 706f 7374 5f6e 705f 6d61 7463 6865  .[post_np_matche
-00002ee0: 722e 6d61 7463 6865 722e 6164 6428 6e61  r.matcher.add(na
-00002ef0: 6d65 2c20 7061 7474 6572 6e73 2c20 2067  me, patterns,  g
-00002f00: 7265 6564 7920 3d27 4c4f 4e47 4553 5427  reedy ='LONGEST'
-00002f10: 2920 666f 7220 6e61 6d65 2c20 7061 7474  ) for name, patt
-00002f20: 6572 6e73 2069 6e20 706f 7374 5f6e 705f  erns in post_np_
-00002f30: 7275 6c65 732e 6974 656d 7328 2920 5d0a  rules.items() ].
-00002f40: 0972 6574 7572 6e20 5b28 7370 6163 792e  .return [(spacy.
-00002f50: 6e6c 702e 766f 6361 625b 6e61 6d65 5d2e  nlp.vocab[name].
-00002f60: 7465 7874 2c69 6265 672c 6965 6e64 2920  text,ibeg,iend) 
-00002f70: 666f 7220 6e61 6d65 2c20 6962 6567 2c69  for name, ibeg,i
-00002f80: 656e 6420 696e 2070 6f73 745f 6e70 5f6d  end in post_np_m
-00002f90: 6174 6368 6572 2e6d 6174 6368 6572 2864  atcher.matcher(d
-00002fa0: 6f63 295d 200a 0a64 6566 206e 6577 5f6d  oc)] ..def new_m
-00002fb0: 6174 6368 6572 2870 6174 7465 726e 732c  atcher(patterns,
-00002fc0: 206e 616d 653d 2770 6174 2729 3a0a 096d   name='pat'):..m
-00002fd0: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
-00002fe0: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
-00002ff0: 290a 096d 6174 6368 6572 2e61 6464 286e  )..matcher.add(n
-00003000: 616d 652c 2070 6174 7465 726e 732c 2067  ame, patterns, g
-00003010: 7265 6564 7920 3d27 4c4f 4e47 4553 5427  reedy ='LONGEST'
-00003020: 290a 0972 6574 7572 6e20 6d61 7463 6865  )..return matche
-00003030: 720a 6d61 7463 6865 7273 203d 207b 2020  r.matchers = {  
-00003040: 2320 666f 7220 6e61 6d65 2c73 7461 7274  # for name,start
-00003050: 2c65 6e64 2069 6e20 6d61 7463 6865 7273  ,end in matchers
-00003060: 5b27 6170 275d 2864 6f63 2920 3a0a 2276  ['ap'](doc) :."v
-00003070: 656e 6422 3a6e 6577 5f6d 6174 6368 6572  end":new_matcher
-00003080: 285b 5b7b 2250 4f53 223a 207b 2249 4e22  ([[{"POS": {"IN"
-00003090: 3a20 5b22 4155 5822 2c22 5645 5242 225d  : ["AUX","VERB"]
-000030a0: 7d7d 2c7b 2250 4f53 223a 207b 2249 4e22  }},{"POS": {"IN"
-000030b0: 3a20 5b22 4144 5622 5d7d 2c20 224f 5022  : ["ADV"]}, "OP"
-000030c0: 3a20 222a 227d 2c20 7b22 504f 5322 3a20  : "*"}, {"POS": 
-000030d0: 7b22 494e 223a 205b 2241 444a 222c 2256  {"IN": ["ADJ","V
-000030e0: 4552 4222 5d7d 2c20 224f 5022 3a20 222a  ERB"]}, "OP": "*
-000030f0: 227d 2c7b 2250 4f53 223a 207b 2249 4e22  "},{"POS": {"IN"
-00003100: 3a20 5b22 5041 5254 222c 2241 4450 222c  : ["PART","ADP",
-00003110: 2254 4f22 5d7d 2c20 224f 5022 3a20 222a  "TO"]}, "OP": "*
-00003120: 227d 2c7b 2250 4f53 223a 2027 5645 5242  "},{"POS": 'VERB
-00003130: 277d 5d5d 292c 2023 2063 6f75 6c64 2068  '}]]), # could h
-00003140: 6172 646c 7920 7761 6974 2074 6f20 6d65  ardly wait to me
-00003150: 6574 0a22 7670 223a 2020 6e65 775f 6d61  et."vp":  new_ma
-00003160: 7463 6865 7228 5b5b 7b27 504f 5327 3a20  tcher([[{'POS': 
-00003170: 2756 4552 4227 7d2c 7b22 504f 5322 3a20  'VERB'},{"POS": 
-00003180: 7b22 494e 223a 205b 2244 4554 222c 2241  {"IN": ["DET","A
-00003190: 4450 222c 2241 444a 225d 7d2c 2022 4f50  DP","ADJ"]}, "OP
-000031a0: 223a 2022 2a22 7d2c 7b22 504f 5322 3a20  ": "*"},{"POS": 
-000031b0: 274e 4f55 4e27 7d2c 207b 2250 4f53 223a  'NOUN'}, {"POS":
-000031c0: 207b 2249 4e22 3a20 5b22 4144 5022 2c22   {"IN": ["ADP","
-000031d0: 544f 225d 7d2c 2022 4f50 223a 2022 2a22  TO"]}, "OP": "*"
-000031e0: 7d5d 2c20 2348 6520 7061 6964 2061 2063  }], #He paid a c
-000031f0: 6c6f 7365 2061 7474 656e 7469 6f6e 2074  lose attention t
-00003200: 6f20 7468 6520 626f 6f6b 2e20 7c48 6520  o the book. |He 
-00003210: 6c6f 6f6b 6564 2075 7020 6672 6f6d 2074  looked up from t
-00003220: 6865 2073 6964 652e 207c 206d 616b 6520  he side. | make 
-00003230: 7573 6520 6f66 0a20 2020 2020 2020 2020  use of.         
-00003240: 2020 2020 2020 2020 2020 2020 5b7b 2750              [{'P
-00003250: 4f53 273a 2027 5645 5242 277d 2c7b 2250  OS': 'VERB'},{"P
-00003260: 4f53 223a 207b 2249 4e22 3a20 5b22 4445  OS": {"IN": ["DE
-00003270: 5422 2c22 4144 5022 2c22 4144 4a22 2c22  T","ADP","ADJ","
-00003280: 544f 222c 2250 4152 5422 5d7d 2c20 224f  TO","PART"]}, "O
-00003290: 5022 3a20 222a 227d 2c7b 2250 4f53 223a  P": "*"},{"POS":
-000032a0: 2027 5645 5242 277d 5d5d 292c 2023 2077   'VERB'}]]), # w
-000032b0: 6169 7420 746f 206d 6565 740a 2270 7022  ait to meet."pp"
-000032c0: 3a20 206e 6577 5f6d 6174 6368 6572 285b  :  new_matcher([
-000032d0: 5b7b 2750 4f53 273a 2027 4144 5027 7d2c  [{'POS': 'ADP'},
-000032e0: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
-000032f0: 2244 4554 222c 224e 554d 222c 2241 444a  "DET","NUM","ADJ
-00003300: 222c 2750 554e 4354 272c 2743 4f4e 4a27  ",'PUNCT','CONJ'
-00003310: 5d7d 2c20 224f 5022 3a20 222a 227d 2c7b  ]}, "OP": "*"},{
-00003320: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
-00003330: 4e4f 554e 222c 2250 4152 5422 5d7d 2c20  NOUN","PART"]}, 
-00003340: 224f 5022 3a20 222b 227d 5d5d 292c 2020  "OP": "+"}]]),  
-00003350: 2020 0a22 6170 223a 2020 6e65 775f 6d61    ."ap":  new_ma
-00003360: 7463 6865 7228 5b5b 7b22 504f 5322 3a20  tcher([[{"POS": 
-00003370: 7b22 494e 223a 205b 2241 4456 225d 7d2c  {"IN": ["ADV"]},
-00003380: 2022 4f50 223a 2022 2a22 7d2c 207b 2250   "OP": "*"}, {"P
-00003390: 4f53 223a 2027 4144 4a27 7d5d 5d29 2c20  OS": 'ADJ'}]]), 
-000033a0: 200a 2276 7072 7422 3a20 6e65 775f 6d61   ."vprt": new_ma
-000033b0: 7463 6865 7228 5b5b 7b22 504f 5322 3a20  tcher([[{"POS": 
-000033c0: 2756 4552 4227 2c20 2254 4147 223a 207b  'VERB', "TAG": {
-000033d0: 224e 4f54 5f49 4e22 3a20 5b22 5642 4e22  "NOT_IN": ["VBN"
-000033e0: 5d7d 7d2c 207b 2250 4f53 223a 207b 2249  ]}}, {"POS": {"I
-000033f0: 4e22 3a20 5b22 5052 4550 222c 2022 4144  N": ["PREP", "AD
-00003400: 5022 2c27 544f 275d 7d2c 2022 4f50 223a  P",'TO']}, "OP":
-00003410: 2022 2b22 7d5d 5d29 2c20 2020 2320 6c6f   "+"}]]),   # lo
-00003420: 6f6b 2075 7020 2f6c 6f6f 6b20 7570 2066  ok up /look up f
-00003430: 726f 6d2c 2020 636f 6d70 7574 6564 2074  rom,  computed t
-00003440: 7769 6365 0a22 7674 6f76 223a 206e 6577  wice."vtov": new
-00003450: 5f6d 6174 6368 6572 285b 5b7b 2250 4f53  _matcher([[{"POS
-00003460: 223a 2027 5645 5242 272c 2022 5441 4722  ": 'VERB', "TAG"
-00003470: 3a20 7b22 4e4f 545f 494e 223a 205b 2256  : {"NOT_IN": ["V
-00003480: 424e 225d 7d7d 2c20 7b22 5441 4722 3a20  BN"]}}, {"TAG": 
-00003490: 2754 4f27 7d2c 7b22 5441 4722 3a20 2756  'TO'},{"TAG": 'V
-000034a0: 4227 7d5d 5d29 2c20 2020 2320 706c 616e  B'}]]),   # plan
-000034b0: 2074 6f20 676f 0a22 7676 6267 223a 206e   to go."vvbg": n
-000034c0: 6577 5f6d 6174 6368 6572 285b 5b7b 2250  ew_matcher([[{"P
-000034d0: 4f53 223a 2027 5645 5242 272c 2022 5441  OS": 'VERB', "TA
-000034e0: 4722 3a20 7b22 4e4f 545f 494e 223a 205b  G": {"NOT_IN": [
-000034f0: 2256 424e 225d 7d7d 2c20 7b22 5441 4722  "VBN"]}}, {"TAG"
-00003500: 3a20 2756 4247 277d 5d5d 292c 2020 2023  : 'VBG'}]]),   #
-00003510: 2063 6f6e 7369 6465 7220 676f 696e 670a   consider going.
-00003520: 2276 7067 223a 2020 6e65 775f 6d61 7463  "vpg":  new_matc
-00003530: 6865 7228 5b5b 7b22 504f 5322 3a20 2756  her([[{"POS": 'V
-00003540: 4552 4227 2c20 2254 4147 223a 207b 224e  ERB', "TAG": {"N
-00003550: 4f54 5f49 4e22 3a20 5b22 5642 4e22 5d7d  OT_IN": ["VBN"]}
-00003560: 7d2c 207b 2250 4f53 223a 207b 2249 4e22  }, {"POS": {"IN"
-00003570: 3a20 5b22 5052 4550 222c 2022 4144 5022  : ["PREP", "ADP"
-00003580: 2c27 5041 5254 275d 7d2c 2022 4f50 223a  ,'PART']}, "OP":
-00003590: 2022 2b22 7d2c 7b22 5441 4722 3a20 2756   "+"},{"TAG": 'V
-000035a0: 4247 277d 5d5d 292c 2020 2023 2069 6e73  BG'}]]),   # ins
-000035b0: 6973 7465 6420 6f6e 2067 6f69 6e67 0a22  isted on going."
-000035c0: 7641 7022 3a20 206e 6577 5f6d 6174 6368  vAp":  new_match
-000035d0: 6572 285b 5b7b 274c 454d 4d41 273a 2027  er([[{'LEMMA': '
-000035e0: 6265 277d 2c7b 2254 4147 223a 207b 2249  be'},{"TAG": {"I
-000035f0: 4e22 3a20 5b22 5642 4e22 5d7d 7d2c 207b  N": ["VBN"]}}, {
-00003600: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
-00003610: 5052 4550 222c 2022 4144 5022 2c27 5041  PREP", "ADP",'PA
-00003620: 5254 275d 7d7d 5d5d 292c 2020 2023 2062  RT']}}]]),   # b
-00003630: 6520 6261 7365 6420 6f6e 2020 200a 2276  e based on   ."v
-00003640: 6170 223a 2020 6e65 775f 6d61 7463 6865  ap":  new_matche
-00003650: 7228 5b5b 7b27 4c45 4d4d 4127 3a20 2762  r([[{'LEMMA': 'b
-00003660: 6527 7d2c 7b22 504f 5322 3a20 7b22 494e  e'},{"POS": {"IN
-00003670: 223a 205b 2241 444a 225d 7d7d 2c20 7b22  ": ["ADJ"]}}, {"
-00003680: 504f 5322 3a20 7b22 494e 223a 205b 2250  POS": {"IN": ["P
-00003690: 5245 5022 2c20 2241 4450 222c 2750 4152  REP", "ADP",'PAR
-000036a0: 5427 5d7d 7d5d 5d29 2c20 2020 2320 6265  T']}}]]),   # be
-000036b0: 2061 6e67 7279 2077 6974 680a 7d20 2366   angry with.} #f
-000036c0: 6f72 206e 616d 652c 2069 6265 672c 6965  or name, ibeg,ie
-000036d0: 6e64 2069 6e20 6d61 7463 6865 7228 646f  nd in matcher(do
-000036e0: 6329 203a 2070 7269 6e74 2873 7061 6379  c) : print(spacy
-000036f0: 2e6e 6c70 2e76 6f63 6162 5b6e 616d 655d  .nlp.vocab[name]
-00003700: 2e74 6578 742c 2064 6f63 5b69 6265 673a  .text, doc[ibeg:
-00003710: 6965 6e64 5d2e 7465 7874 290a 0a23 230a  iend].text)..##.
-00003720: 2323 2066 726f 6d20 7665 7262 6e65 742e  ## from verbnet.
-00003730: 7079 0a23 230a 404c 616e 6775 6167 652e  py.##.@Language.
-00003740: 636f 6d70 6f6e 656e 7428 226d 6572 6765  component("merge
-00003750: 5f6e 7022 290a 6465 6620 6d65 7267 655f  _np").def merge_
-00003760: 6e70 2864 6f63 293a 0a09 7769 7468 2064  np(doc):..with d
-00003770: 6f63 2e72 6574 6f6b 656e 697a 6528 2920  oc.retokenize() 
-00003780: 6173 2072 6574 6f6b 656e 697a 6572 3a0a  as retokenizer:.
-00003790: 0909 666f 7220 6e70 2069 6e20 646f 632e  ..for np in doc.
-000037a0: 6e6f 756e 5f63 6875 6e6b 733a 0a09 0909  noun_chunks:....
-000037b0: 6174 7472 7320 3d20 7b22 7461 6722 3a20  attrs = {"tag": 
-000037c0: 6e70 2e72 6f6f 742e 7461 672c 2022 6465  np.root.tag, "de
-000037d0: 7022 3a20 6e70 2e72 6f6f 742e 6465 702c  p": np.root.dep,
-000037e0: 2022 656e 745f 7479 7065 223a 2022 4e50   "ent_type": "NP
-000037f0: 222c 2022 6c65 6d6d 6122 3a64 6f63 5b6e  ", "lemma":doc[n
-00003800: 702e 656e 642d 315d 2e6c 656d 6d61 7d20  p.end-1].lemma} 
-00003810: 2320 2c20 226c 656d 6d61 223a 646f 635b  # , "lemma":doc[
-00003820: 6e70 2e65 6e64 2d31 5d2e 6c65 6d6d 6120  np.end-1].lemma 
-00003830: 7c20 6164 6465 6420 3230 3232 2e37 2e32  | added 2022.7.2
-00003840: 360a 0909 0972 6574 6f6b 656e 697a 6572  6....retokenizer
-00003850: 2e6d 6572 6765 286e 702c 2061 7474 7273  .merge(np, attrs
-00003860: 3d61 7474 7273 2920 0a09 7265 7475 726e  =attrs) ..return
-00003870: 2064 6f63 0a0a 6465 6620 736b 656e 7028   doc..def skenp(
-00003880: 646f 632c 2074 6167 3d22 5f4e 5022 293a  doc, tag="_NP"):
-00003890: 2023 2061 6464 6564 2032 3032 322e 332e   # added 2022.3.
-000038a0: 3232 2c20 666f 7220 736b 6576 6563 0a09  22, for skevec..
-000038b0: 6d65 7267 655f 6e70 2864 6f63 2920 2320  merge_np(doc) # 
-000038c0: 7472 616e 7366 6f72 6d20 646f 6320 2c20  transform doc , 
-000038d0: 6669 6e61 6c6c 7920 746f 2062 6520 6361  finally to be ca
-000038e0: 6c6c 6564 200a 0972 6574 7572 6e20 2220  lled ..return " 
-000038f0: 222e 6a6f 696e 285b 7461 6720 6966 2074  ".join([tag if t
-00003900: 2e65 6e74 5f74 7970 655f 203d 3d20 274e  .ent_type_ == 'N
-00003910: 5027 2065 6c73 6520 742e 7465 7874 2066  P' else t.text f
-00003920: 6f72 2074 2069 6e20 646f 635d 290a 0a64  or t in doc])..d
-00003930: 6566 206d 6572 6765 5f6e 5f6f 665f 6e28  ef merge_n_of_n(
-00003940: 646f 6329 3a0a 0969 6620 6e6f 7420 6861  doc):..if not ha
-00003950: 7361 7474 7228 6d65 7267 655f 6e5f 6f66  sattr(merge_n_of
-00003960: 5f6e 2c20 276d 6174 6368 6572 2729 3a0a  _n, 'matcher'):.
-00003970: 0909 6d65 7267 655f 6e5f 6f66 5f6e 2e6d  ..merge_n_of_n.m
-00003980: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
-00003990: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
-000039a0: 290a 0909 6d65 7267 655f 6e5f 6f66 5f6e  )...merge_n_of_n
-000039b0: 2e6d 6174 6368 6572 2e61 6464 2822 6e2d  .matcher.add("n-
-000039c0: 6f66 2d6e 222c 205b 5b7b 2245 4e54 5f54  of-n", [[{"ENT_T
-000039d0: 5950 4522 3a20 224e 5022 7d2c 207b 224c  YPE": "NP"}, {"L
-000039e0: 454d 4d41 223a 226f 6622 7d2c 7b22 454e  EMMA":"of"},{"EN
-000039f0: 545f 5459 5045 223a 2022 4e50 227d 5d2c  T_TYPE": "NP"}],
-00003a00: 205b 7b22 454e 545f 5459 5045 223a 2022   [{"ENT_TYPE": "
-00003a10: 4e50 227d 2c20 7b22 4c45 4d4d 4122 3a22  NP"}, {"LEMMA":"
-00003a20: 6f66 227d 2c7b 2250 4f53 223a 2022 4e4f  of"},{"POS": "NO
-00003a30: 554e 227d 5d5d 2c20 2067 7265 6564 7920  UN"}]],  greedy 
-00003a40: 3d27 4c4f 4e47 4553 5427 290a 0977 6974  ='LONGEST')..wit
-00003a50: 6820 646f 632e 7265 746f 6b65 6e69 7a65  h doc.retokenize
-00003a60: 2829 2061 7320 7265 746f 6b65 6e69 7a65  () as retokenize
-00003a70: 723a 0a09 0966 6f72 206e 616d 652c 2073  r:...for name, s
-00003a80: 7461 7274 2c20 656e 6420 696e 206d 6572  tart, end in mer
-00003a90: 6765 5f6e 5f6f 665f 6e2e 6d61 7463 6865  ge_n_of_n.matche
-00003aa0: 7228 646f 6329 3a0a 0909 0969 6620 656e  r(doc):....if en
-00003ab0: 6420 2d20 7374 6172 7420 3e20 313a 200a  d - start > 1: .
-00003ac0: 0909 0909 7472 793a 0a09 0909 0909 6920  ....try:......i 
-00003ad0: 3d20 646f 635b 7374 6172 745d 2e68 6561  = doc[start].hea
-00003ae0: 642e 690a 0909 0909 0961 7474 7273 203d  d.i......attrs =
-00003af0: 207b 2270 6f73 223a 2064 6f63 5b69 5d2e   {"pos": doc[i].
-00003b00: 706f 732c 2022 7461 6722 3a20 646f 635b  pos, "tag": doc[
-00003b10: 695d 2e74 6167 2c20 2264 6570 223a 2064  i].tag, "dep": d
-00003b20: 6f63 5b69 5d2e 6465 702c 2022 6c65 6d6d  oc[i].dep, "lemm
-00003b30: 6122 3a64 6f63 5b69 5d2e 6c65 6d6d 612c  a":doc[i].lemma,
-00003b40: 2022 656e 745f 7479 7065 223a 2022 4e50   "ent_type": "NP
-00003b50: 227d 0a09 0909 0909 7265 746f 6b65 6e69  "}......retokeni
-00003b60: 7a65 722e 6d65 7267 6528 646f 635b 7374  zer.merge(doc[st
-00003b70: 6172 7420 3a20 656e 645d 2c20 6174 7472  art : end], attr
-00003b80: 733d 6174 7472 7329 0a09 0909 0965 7863  s=attrs).....exc
-00003b90: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00003ba0: 2065 3a0a 0909 0909 0970 7269 6e74 2028   e:......print (
-00003bb0: 2022 6d65 7267 655f 6e5f 6f66 5f6e 2065   "merge_n_of_n e
-00003bc0: 783a 222c 2065 202c 2073 7461 7274 2c20  x:", e , start, 
-00003bd0: 656e 6429 0a09 7265 7475 726e 2064 6f63  end)..return doc
-00003be0: 0a0a 404c 616e 6775 6167 652e 636f 6d70  ..@Language.comp
-00003bf0: 6f6e 656e 7428 226d 6572 6765 5f76 7022  onent("merge_vp"
-00003c00: 290a 6465 6620 6d65 7267 655f 7670 2864  ).def merge_vp(d
-00003c10: 6f63 293a 0a09 6966 206e 6f74 2068 6173  oc):..if not has
-00003c20: 6174 7472 286d 6572 6765 5f76 702c 2027  attr(merge_vp, '
-00003c30: 6d61 7463 6865 7227 293a 0a09 096d 6572  matcher'):...mer
-00003c40: 6765 5f76 702e 6d61 7463 6865 7220 3d20  ge_vp.matcher = 
-00003c50: 4d61 7463 6865 7228 7370 6163 792e 6e6c  Matcher(spacy.nl
-00003c60: 702e 766f 6361 6229 0a09 096d 6572 6765  p.vocab)...merge
-00003c70: 5f76 702e 6d61 7463 6865 722e 6164 6428  _vp.matcher.add(
-00003c80: 2276 7022 2c20 5b5b 7b22 504f 5322 3a20  "vp", [[{"POS": 
-00003c90: 7b22 494e 223a 5b22 4155 5822 2c22 5041  {"IN":["AUX","PA
-00003ca0: 5254 225d 7d2c 2022 6f70 223a 2022 2a22  RT"]}, "op": "*"
-00003cb0: 7d2c 207b 2250 4f53 223a 2256 4552 4222  }, {"POS":"VERB"
-00003cc0: 7d2c 7b22 504f 5322 3a20 2241 4456 222c  },{"POS": "ADV",
-00003cd0: 2022 6f70 223a 2022 2a22 7d5d 5d2c 2020   "op": "*"}]],  
-00003ce0: 6772 6565 6479 203d 274c 4f4e 4745 5354  greedy ='LONGEST
-00003cf0: 2729 0a09 7769 7468 2064 6f63 2e72 6574  ')..with doc.ret
-00003d00: 6f6b 656e 697a 6528 2920 6173 2072 6574  okenize() as ret
-00003d10: 6f6b 656e 697a 6572 3a0a 0909 666f 7220  okenizer:...for 
-00003d20: 6e61 6d65 2c20 7374 6172 742c 2065 6e64  name, start, end
-00003d30: 2069 6e20 6d65 7267 655f 7670 2e6d 6174   in merge_vp.mat
-00003d40: 6368 6572 2864 6f63 293a 0a09 0909 6966  cher(doc):....if
-00003d50: 2065 6e64 202d 2073 7461 7274 203e 2031   end - start > 1
-00003d60: 3a20 0a09 0909 0974 7279 3a0a 0909 0909  : .....try:.....
-00003d70: 0969 203d 2064 6f63 5b73 7461 7274 5d2e  .i = doc[start].
-00003d80: 6865 6164 2e69 0a09 0909 0909 6174 7472  head.i......attr
-00003d90: 7320 3d20 7b22 706f 7322 3a20 646f 635b  s = {"pos": doc[
-00003da0: 695d 2e70 6f73 2c20 2274 6167 223a 2064  i].pos, "tag": d
-00003db0: 6f63 5b69 5d2e 7461 672c 2022 6465 7022  oc[i].tag, "dep"
-00003dc0: 3a20 646f 635b 695d 2e64 6570 2c20 226c  : doc[i].dep, "l
-00003dd0: 656d 6d61 223a 646f 635b 695d 2e6c 656d  emma":doc[i].lem
-00003de0: 6d61 2c20 2265 6e74 5f74 7970 6522 3a20  ma, "ent_type": 
-00003df0: 2256 5022 7d0a 0909 0909 0972 6574 6f6b  "VP"}......retok
-00003e00: 656e 697a 6572 2e6d 6572 6765 2864 6f63  enizer.merge(doc
-00003e10: 5b73 7461 7274 203a 2065 6e64 5d2c 2061  [start : end], a
-00003e20: 7474 7273 3d61 7474 7273 290a 0909 0909  ttrs=attrs).....
-00003e30: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00003e40: 2061 7320 653a 0a09 0909 0909 7072 696e   as e:......prin
-00003e50: 7420 2820 226d 6572 6765 5f76 7020 6578  t ( "merge_vp ex
-00003e60: 3a22 2c20 6520 2c20 7374 6172 742c 2065  :", e , start, e
-00003e70: 6e64 290a 0972 6574 7572 6e20 646f 630a  nd)..return doc.
-00003e80: 0a64 6566 206d 6572 6765 5f70 7028 646f  .def merge_pp(do
-00003e90: 6329 3a20 0a09 6966 206e 6f74 2068 6173  c): ..if not has
-00003ea0: 6174 7472 286d 6572 6765 5f70 702c 2027  attr(merge_pp, '
-00003eb0: 6d61 7463 6865 7227 293a 0a09 096d 6572  matcher'):...mer
-00003ec0: 6765 5f70 702e 6d61 7463 6865 7220 3d20  ge_pp.matcher = 
-00003ed0: 4d61 7463 6865 7228 7370 6163 792e 6e6c  Matcher(spacy.nl
-00003ee0: 702e 766f 6361 6229 0a09 096d 6572 6765  p.vocab)...merge
-00003ef0: 5f70 702e 6d61 7463 6865 722e 6164 6428  _pp.matcher.add(
-00003f00: 2270 7022 2c20 5b5b 7b22 504f 5322 3a20  "pp", [[{"POS": 
-00003f10: 7b22 494e 223a 5b22 4144 5022 5d7d 2c20  {"IN":["ADP"]}, 
-00003f20: 226f 7022 3a20 222b 227d 2c20 7b22 454e  "op": "+"}, {"EN
-00003f30: 545f 5459 5045 223a 224e 5022 2c20 226f  T_TYPE":"NP", "o
-00003f40: 7022 3a20 222b 227d 5d5d 2c20 2067 7265  p": "+"}]],  gre
-00003f50: 6564 7920 3d27 4c4f 4e47 4553 5427 290a  edy ='LONGEST').
-00003f60: 0977 6974 6820 646f 632e 7265 746f 6b65  .with doc.retoke
-00003f70: 6e69 7a65 2829 2061 7320 7265 746f 6b65  nize() as retoke
-00003f80: 6e69 7a65 723a 0a09 0966 6f72 206e 616d  nizer:...for nam
-00003f90: 652c 2073 7461 7274 2c20 656e 6420 696e  e, start, end in
-00003fa0: 206d 6572 6765 5f70 702e 6d61 7463 6865   merge_pp.matche
-00003fb0: 7228 646f 6329 3a0a 0909 0969 6620 656e  r(doc):....if en
-00003fc0: 6420 2d20 7374 6172 7420 3e20 313a 200a  d - start > 1: .
-00003fd0: 0909 0909 7472 793a 0a09 0909 0909 6920  ....try:......i 
-00003fe0: 3d20 646f 635b 7374 6172 745d 2e68 6561  = doc[start].hea
-00003ff0: 642e 690a 0909 0909 0961 7474 7273 203d  d.i......attrs =
-00004000: 207b 2270 6f73 223a 2064 6f63 5b69 5d2e   {"pos": doc[i].
-00004010: 706f 732c 2022 7461 6722 3a20 646f 635b  pos, "tag": doc[
-00004020: 695d 2e74 6167 2c20 2264 6570 223a 2064  i].tag, "dep": d
-00004030: 6f63 5b69 5d2e 6465 702c 2022 6c65 6d6d  oc[i].dep, "lemm
-00004040: 6122 3a64 6f63 5b69 5d2e 6c65 6d6d 612c  a":doc[i].lemma,
-00004050: 2022 656e 745f 7479 7065 223a 2022 5050   "ent_type": "PP
-00004060: 227d 0a09 0909 0909 7265 746f 6b65 6e69  "}......retokeni
-00004070: 7a65 722e 6d65 7267 6528 646f 635b 7374  zer.merge(doc[st
-00004080: 6172 7420 3a20 656e 645d 2c20 6174 7472  art : end], attr
-00004090: 733d 6174 7472 7329 0a09 0909 0965 7863  s=attrs).....exc
-000040a0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-000040b0: 2065 3a0a 0909 0909 0970 7269 6e74 2028   e:......print (
-000040c0: 2022 6d65 7267 655f 7070 2065 783a 222c   "merge_pp ex:",
-000040d0: 2065 202c 2073 7461 7274 2c20 656e 6429   e , start, end)
-000040e0: 0a09 7265 7475 726e 2064 6f63 0a0a 6465  ..return doc..de
-000040f0: 6620 736b 6570 7028 646f 632c 2074 6167  f skepp(doc, tag
-00004100: 3d22 5f50 5022 293a 2023 2061 6464 6564  ="_PP"): # added
-00004110: 2032 3032 322e 332e 3234 2c20 207c 2046   2022.3.24,  | F
-00004120: 726f 6d20 7468 6520 626f 6f6b 2c20 7468  rom the book, th
-00004130: 6973 2069 7320 616c 736f 2064 6966 6669  is is also diffi
-00004140: 6375 6c74 2074 6f20 2e2e 200a 096d 6572  cult to .. ..mer
-00004150: 6765 5f70 7028 646f 6329 2023 2074 7261  ge_pp(doc) # tra
-00004160: 6e73 666f 726d 2064 6f63 202c 2066 696e  nsform doc , fin
-00004170: 616c 6c79 2074 6f20 6265 2063 616c 6c65  ally to be calle
-00004180: 6420 0a09 7265 7475 726e 2022 2022 2e6a  d ..return " ".j
-00004190: 6f69 6e28 5b74 6167 2069 6620 742e 656e  oin([tag if t.en
-000041a0: 745f 7479 7065 5f20 3d3d 2027 5050 2720  t_type_ == 'PP' 
-000041b0: 656c 7365 2074 2e74 6578 7420 666f 7220  else t.text for 
-000041c0: 7420 696e 2064 6f63 5d29 0a0a 6465 6620  t in doc])..def 
-000041d0: 6d65 7267 655f 636c 6175 7365 2864 6f63  merge_clause(doc
-000041e0: 293a 2023 2073 7562 7472 6565 206f 6620  ): # subtree of 
-000041f0: 6120 7665 7262 2069 7320 7468 6520 636c  a verb is the cl
-00004200: 6175 7365 202c 2068 7474 7073 3a2f 2f73  ause , https://s
-00004210: 7562 7363 7269 7074 696f 6e2e 7061 636b  ubscription.pack
-00004220: 7470 7562 2e63 6f6d 2f62 6f6f 6b2f 6461  tpub.com/book/da
-00004230: 7461 2f39 3738 3138 3338 3938 3733 3132  ta/9781838987312
-00004240: 2f32 2f63 6830 326c 766c 3173 6563 3133  /2/ch02lvl1sec13
-00004250: 2f73 706c 6974 7469 6e67 2d73 656e 7465  /splitting-sente
-00004260: 6e63 6573 2d69 6e74 6f2d 636c 6175 7365  nces-into-clause
-00004270: 730a 0977 6974 6820 646f 632e 7265 746f  s..with doc.reto
-00004280: 6b65 6e69 7a65 2829 2061 7320 7265 746f  kenize() as reto
-00004290: 6b65 6e69 7a65 723a 0a09 0966 6f72 2076  kenizer:...for v
-000042a0: 2069 6e20 5b74 2066 6f72 2074 2069 6e20   in [t for t in 
-000042b0: 646f 6320 6966 2074 2e70 6f73 5f20 3d3d  doc if t.pos_ ==
-000042c0: 2027 5645 5242 2720 616e 6420 742e 6465   'VERB' and t.de
-000042d0: 705f 2021 3d20 2752 4f4f 5427 205d 203a  p_ != 'ROOT' ] :
-000042e0: 2023 206e 6f6e 2d72 6f6f 740a 0909 0974   # non-root....t
-000042f0: 7279 3a0a 0909 0909 6368 696c 6472 656e  ry:.....children
-00004300: 203d 206c 6973 7428 762e 7375 6274 7265   = list(v.subtre
-00004310: 6529 0a09 0909 0973 7461 7274 203d 2063  e).....start = c
-00004320: 6869 6c64 7265 6e5b 305d 2e69 2020 090a  hildren[0].i  ..
-00004330: 0909 0909 656e 6420 3d20 6368 696c 6472  ....end = childr
-00004340: 656e 5b2d 315d 2e69 200a 0909 0909 6174  en[-1].i .....at
-00004350: 7472 7320 3d20 7b22 706f 7322 3a20 762e  trs = {"pos": v.
-00004360: 706f 732c 2022 7461 6722 3a20 762e 7461  pos, "tag": v.ta
-00004370: 672c 2022 6465 7022 3a20 762e 6465 702c  g, "dep": v.dep,
-00004380: 2022 6c65 6d6d 6122 3a76 2e6c 656d 6d61   "lemma":v.lemma
-00004390: 2c20 2265 6e74 5f74 7970 6522 3a20 2253  , "ent_type": "S
-000043a0: 2e22 202b 2076 2e64 6570 5f20 7d20 2320  ." + v.dep_ } # 
-000043b0: 532e 6164 7663 6c20 2c20 2053 2e63 6f6e  S.advcl ,  S.con
-000043c0: 6a20 0a09 0909 0972 6574 6f6b 656e 697a  j .....retokeniz
-000043d0: 6572 2e6d 6572 6765 2864 6f63 5b73 7461  er.merge(doc[sta
-000043e0: 7274 203a 2065 6e64 2b31 5d2c 2061 7474  rt : end+1], att
-000043f0: 7273 3d61 7474 7273 290a 0909 0965 7863  rs=attrs)....exc
-00004400: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00004410: 2065 3a0a 0909 0909 7072 696e 7420 2820   e:.....print ( 
-00004420: 226d 6572 6765 5f63 6c61 7573 6520 6578  "merge_clause ex
-00004430: 3a22 2c20 652c 2076 2029 0a09 7265 7475  :", e, v )..retu
-00004440: 726e 2064 6f63 0a0a 404c 616e 6775 6167  rn doc..@Languag
-00004450: 652e 636f 6d70 6f6e 656e 7428 2273 7061  e.component("spa
-00004460: 6e5f 636c 6175 7365 2229 0a64 6566 2073  n_clause").def s
-00004470: 7061 6e5f 636c 6175 7365 2864 6f63 293a  pan_clause(doc):
-00004480: 2023 207b 2763 6c3a 3427 3a20 5b74 6861   # {'cl:4': [tha
-00004490: 7420 6974 2063 7269 6564 5d2c 2027 636c  t it cried], 'cl
-000044a0: 3a31 3027 3a20 5b74 6861 7420 4920 776f  :10': [that I wo
-000044b0: 756c 6420 6661 696c 5d7d 0a09 666f 7220  uld fail]}..for 
-000044c0: 7620 696e 205b 7420 666f 7220 7420 696e  v in [t for t in
-000044d0: 2064 6f63 2069 6620 742e 706f 735f 203d   doc if t.pos_ =
-000044e0: 3d20 2756 4552 4227 2061 6e64 2074 2e64  = 'VERB' and t.d
-000044f0: 6570 5f20 213d 2027 524f 4f54 2720 5d20  ep_ != 'ROOT' ] 
-00004500: 3a20 2320 6e6f 6e2d 726f 6f74 0a09 0974  : # non-root...t
-00004510: 7279 3a0a 0909 0963 6869 6c64 7265 6e20  ry:....children 
-00004520: 3d20 6c69 7374 2876 2e73 7562 7472 6565  = list(v.subtree
-00004530: 290a 0909 0973 7461 7274 203d 2063 6869  )....start = chi
-00004540: 6c64 7265 6e5b 305d 2e69 2020 090a 0909  ldren[0].i  ....
-00004550: 0965 6e64 203d 2063 6869 6c64 7265 6e5b  .end = children[
-00004560: 2d31 5d2e 6920 0a09 0909 6174 7472 7320  -1].i ....attrs 
-00004570: 3d20 7b22 706f 7322 3a20 762e 706f 735f  = {"pos": v.pos_
-00004580: 2c20 2274 6167 223a 2076 2e74 6167 5f2c  , "tag": v.tag_,
-00004590: 2022 6465 7022 3a20 762e 6465 705f 2c20   "dep": v.dep_, 
-000045a0: 226c 656d 6d61 223a 762e 6c65 6d6d 615f  "lemma":v.lemma_
-000045b0: 2c20 2265 6e74 5f74 7970 6522 3a20 2253  , "ent_type": "S
-000045c0: 2e22 202b 2076 2e64 6570 5f20 7d20 2320  ." + v.dep_ } # 
-000045d0: 532e 6164 7663 6c20 2c20 2053 2e63 6f6e  S.advcl ,  S.con
-000045e0: 6a20 0a09 0909 6e61 6d65 203d 2066 2263  j ....name = f"c
-000045f0: 6c3a 7b73 7461 7274 7d22 200a 0909 0964  l:{start}" ....d
-00004600: 6f63 2e73 7061 6e73 5b6e 616d 655d 203d  oc.spans[name] =
-00004610: 2053 7061 6e47 726f 7570 2864 6f63 2c20   SpanGroup(doc, 
-00004620: 6e61 6d65 3d6e 616d 652c 2073 7061 6e73  name=name, spans
-00004630: 3d5b 2064 6f63 5b73 7461 7274 203a 2065  =[ doc[start : e
-00004640: 6e64 2b31 5d20 5d2c 2061 7474 7273 3d61  nd+1] ], attrs=a
-00004650: 7474 7273 290a 0909 6578 6365 7074 2045  ttrs)...except E
-00004660: 7863 6570 7469 6f6e 2061 7320 653a 0a09  xception as e:..
-00004670: 0909 7072 696e 7420 2820 2273 7061 6e5f  ..print ( "span_
-00004680: 636c 6175 7365 2065 783a 222c 2065 2c20  clause ex:", e, 
-00004690: 7620 290a 0972 6574 7572 6e20 646f 630a  v )..return doc.
-000046a0: 0a4e 505f 7374 6172 7420 3d20 7b22 454e  .NP_start = {"EN
-000046b0: 545f 5459 5045 223a 2022 4e50 222c 2022  T_TYPE": "NP", "
-000046c0: 4953 5f53 454e 545f 5354 4152 5422 3a20  IS_SENT_START": 
-000046d0: 5472 7565 7d0a 5645 5242 0920 3d20 7b22  True}.VERB. = {"
-000046e0: 504f 5322 3a20 7b22 494e 223a 205b 2256  POS": {"IN": ["V
-000046f0: 4552 4222 5d7d 7d0a 4e4f 554e 0920 3d20  ERB"]}}.NOUN. = 
-00004700: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
-00004710: 224e 4f55 4e22 2c22 5052 4f4e 222c 2250  "NOUN","PRON","P
-00004720: 524f 504e 225d 7d7d 0a50 554e 4354 0920  ROPN"]}}.PUNCT. 
-00004730: 3d20 7b22 4953 5f50 554e 4354 223a 2054  = {"IS_PUNCT": T
-00004740: 7275 657d 0a5f 7665 7262 6e65 745f 7275  rue}._verbnet_ru
-00004750: 6c65 7320 3d20 7b20 2023 203a 3120 2c20  les = {  # :1 , 
-00004760: 7665 7262 2773 206f 6666 7365 7420 0a09  verb's offset ..
-00004770: 224e 5020 563a 3122 3a20 5b5b 4e50 5f73  "NP V:1": [[NP_s
-00004780: 7461 7274 2c56 4552 422c 2050 554e 4354  tart,VERB, PUNCT
-00004790: 5d5d 2c20 0a09 224e 5020 6f66 204e 5020  ]], .."NP of NP 
-000047a0: 563a 3322 3a20 5b5b 204e 505f 7374 6172  V:3": [[ NP_star
-000047b0: 742c 7b22 4c45 4d4d 4122 3a20 226f 6622  t,{"LEMMA": "of"
-000047c0: 7d2c 207b 2245 4e54 5f54 5950 4522 3a20  }, {"ENT_TYPE": 
-000047d0: 224e 5022 7d2c 2056 4552 422c 5055 4e43  "NP"}, VERB,PUNC
-000047e0: 545d 5d2c 200a 0922 4e50 2056 204e 503a  T]], .."NP V NP:
-000047f0: 3122 3a20 5b5b 4e4f 554e 2c56 4552 422c  1": [[NOUN,VERB,
-00004800: 204e 4f55 4e2c 7b22 504f 5322 3a20 7b22   NOUN,{"POS": {"
-00004810: 494e 223a 205b 2250 554e 4354 225d 7d7d  IN": ["PUNCT"]}}
-00004820: 5d5d 2c20 0a09 224e 5020 5620 4e50 2041  ]], .."NP V NP A
-00004830: 444a 3a31 223a 205b 5b4e 4f55 4e2c 5645  DJ:1": [[NOUN,VE
-00004840: 5242 2c20 4e4f 554e 2c7b 2250 4f53 223a  RB, NOUN,{"POS":
-00004850: 207b 2249 4e22 3a20 5b22 4144 4a22 5d7d   {"IN": ["ADJ"]}
-00004860: 7d5d 5d2c 200a 0922 4e50 2056 204e 5020  }]], .."NP V NP 
-00004870: 4e50 3a31 223a 205b 5b4e 4f55 4e2c 5645  NP:1": [[NOUN,VE
-00004880: 5242 2c20 4e4f 554e 2c4e 4f55 4e5d 5d2c  RB, NOUN,NOUN]],
-00004890: 200a 0922 4e50 2056 204e 502d 4461 7469   .."NP V NP-Dati
-000048a0: 7665 204e 503a 3122 3a20 5b5b 4e4f 554e  ve NP:1": [[NOUN
-000048b0: 2c56 4552 422c 207b 2244 4550 223a 207b  ,VERB, {"DEP": {
-000048c0: 2249 4e22 3a20 5b22 6461 7469 7665 225d  "IN": ["dative"]
-000048d0: 7d7d 2c4e 4f55 4e5d 5d2c 200a 0922 4e50  }},NOUN]], .."NP
-000048e0: 2056 204e 5020 5050 3a31 223a 205b 5b4e   V NP PP:1": [[N
-000048f0: 4f55 4e2c 5645 5242 2c20 4e4f 554e 2c7b  OUN,VERB, NOUN,{
-00004900: 2244 4550 223a 207b 2249 4e22 3a20 5b22  "DEP": {"IN": ["
-00004910: 7072 6570 225d 7d7d 5d5d 2c20 0a09 224e  prep"]}}]], .."N
-00004920: 5020 5620 4e50 2050 5020 5050 3a31 223a  P V NP PP PP:1":
-00004930: 205b 5b4e 4f55 4e2c 5645 5242 2c20 4e4f   [[NOUN,VERB, NO
-00004940: 554e 2c7b 2244 4550 223a 207b 2249 4e22  UN,{"DEP": {"IN"
-00004950: 3a20 5b22 7072 6570 225d 7d7d 2c20 4e4f  : ["prep"]}}, NO
-00004960: 554e 2c7b 2244 4550 223a 207b 2249 4e22  UN,{"DEP": {"IN"
-00004970: 3a20 5b22 7072 6570 225d 7d7d 2c20 4e4f  : ["prep"]}}, NO
-00004980: 554e 5d5d 2c20 0a09 224e 5020 5620 535f  UN]], .."NP V S_
-00004990: 494e 473a 3122 3a20 5b5b 4e4f 554e 2c56  ING:1": [[NOUN,V
-000049a0: 4552 422c 207b 2254 4147 223a 207b 2249  ERB, {"TAG": {"I
-000049b0: 4e22 3a20 5b22 5642 4722 5d7d 7d5d 5d2c  N": ["VBG"]}}]],
-000049c0: 200a 0922 4e50 2056 2077 6865 7468 6572   .."NP V whether
-000049d0: 2f68 6f77 2053 5f49 4e46 3a31 223a 205b  /how S_INF:1": [
-000049e0: 5b4e 4f55 4e2c 5645 5242 2c20 7b22 4c45  [NOUN,VERB, {"LE
-000049f0: 4d4d 4122 3a20 7b22 494e 223a 205b 2277  MMA": {"IN": ["w
-00004a00: 6865 7468 6572 222c 2268 6f77 225d 7d7d  hether","how"]}}
-00004a10: 2c20 7b22 4c45 4d4d 4122 3a20 7b22 494e  , {"LEMMA": {"IN
-00004a20: 223a 205b 2274 6f22 5d7d 7d2c 2056 4552  ": ["to"]}}, VER
-00004a30: 425d 5d2c 200a 0922 4e50 2056 204e 5020  B]], .."NP V NP 
-00004a40: 746f 2062 6520 4e50 3a31 223a 205b 5b4e  to be NP:1": [[N
-00004a50: 4f55 4e2c 5645 5242 2c20 7b22 4c45 4d4d  OUN,VERB, {"LEMM
-00004a60: 4122 3a20 7b22 494e 223a 205b 2274 6f22  A": {"IN": ["to"
-00004a70: 5d7d 7d2c 207b 224c 454d 4d41 223a 207b  ]}}, {"LEMMA": {
-00004a80: 2249 4e22 3a20 5b22 6265 225d 7d7d 2c20  "IN": ["be"]}}, 
-00004a90: 4e4f 554e 5d5d 2c20 0a09 224e 5020 5620  NOUN]], .."NP V 
-00004aa0: 7468 6174 2f68 6f77 2053 3a31 223a 205b  that/how S:1": [
-00004ab0: 5b4e 4f55 4e2c 5645 5242 2c20 7b22 4c45  [NOUN,VERB, {"LE
-00004ac0: 4d4d 4122 3a20 7b22 494e 223a 205b 2274  MMA": {"IN": ["t
-00004ad0: 6861 7422 2c22 686f 7722 5d7d 2c20 224f  hat","how"]}, "O
-00004ae0: 5022 3a22 2a22 7d2c 204e 4f55 4e2c 207b  P":"*"}, NOUN, {
-00004af0: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
-00004b00: 4155 5822 2c22 5041 5254 225d 7d2c 2022  AUX","PART"]}, "
-00004b10: 4f50 223a 222a 227d 2c7b 2244 4550 223a  OP":"*"},{"DEP":
-00004b20: 207b 2249 4e22 3a20 5b22 6363 6f6d 7022   {"IN": ["ccomp"
-00004b30: 5d7d 7d5d 5d2c 2020 2354 6865 7920 636f  ]}}]],  #They co
-00004b40: 6e73 6964 6572 6564 2074 6861 7420 6865  nsidered that he
-00004b50: 2077 6173 2074 6865 2070 726f 6665 7373   was the profess
-00004b60: 6f72 2e0a 0922 4e50 2056 2077 6865 7468  or..."NP V wheth
-00004b70: 6572 2f69 6620 533a 3122 3a20 5b5b 4e4f  er/if S:1": [[NO
-00004b80: 554e 2c56 4552 422c 207b 224c 454d 4d41  UN,VERB, {"LEMMA
-00004b90: 223a 207b 2249 4e22 3a20 5b22 7768 6574  ": {"IN": ["whet
-00004ba0: 6865 7222 2c22 6966 225d 7d7d 2c20 4e4f  her","if"]}}, NO
-00004bb0: 554e 2c7b 2250 4f53 223a 207b 2249 4e22  UN,{"POS": {"IN"
-00004bc0: 3a20 5b22 4155 5822 2c22 5041 5254 225d  : ["AUX","PART"]
-00004bd0: 7d2c 2022 4f50 223a 222a 227d 2c20 7b22  }, "OP":"*"}, {"
-00004be0: 4445 5022 3a20 7b22 494e 223a 205b 2263  DEP": {"IN": ["c
-00004bf0: 636f 6d70 225d 7d7d 5d5d 2c20 2023 4865  comp"]}}]],  #He
-00004c00: 2063 6f6e 7369 6465 7265 6420 7768 6574   considered whet
-00004c10: 6865 7220 6865 2073 686f 756c 6420 636f  her he should co
-00004c20: 6d65 2e0a 0922 4e50 2056 2077 6861 7420  me..."NP V what 
-00004c30: 533a 3122 3a20 5b5b 4e4f 554e 2c56 4552  S:1": [[NOUN,VER
-00004c40: 422c 207b 224c 454d 4d41 223a 207b 2249  B, {"LEMMA": {"I
-00004c50: 4e22 3a20 5b22 7768 6174 225d 7d7d 2c20  N": ["what"]}}, 
-00004c60: 4e4f 554e 2c7b 2250 4f53 223a 207b 2249  NOUN,{"POS": {"I
-00004c70: 4e22 3a20 5b22 4155 5822 2c22 5041 5254  N": ["AUX","PART
-00004c80: 225d 7d2c 2022 4f50 223a 222a 227d 2c20  "]}, "OP":"*"}, 
-00004c90: 7b22 4445 5022 3a20 7b22 494e 223a 205b  {"DEP": {"IN": [
-00004ca0: 2263 636f 6d70 225d 7d7d 5d5d 2c20 200a  "ccomp"]}}]],  .
-00004cb0: 0922 4e50 2056 2077 6861 7420 535f 494e  ."NP V what S_IN
-00004cc0: 463a 3122 3a20 5b5b 4e4f 554e 2c56 4552  F:1": [[NOUN,VER
-00004cd0: 422c 207b 224c 454d 4d41 223a 207b 2249  B, {"LEMMA": {"I
-00004ce0: 4e22 3a20 5b22 7768 6174 225d 7d7d 2c20  N": ["what"]}}, 
-00004cf0: 7b22 4c45 4d4d 4122 3a20 7b22 494e 223a  {"LEMMA": {"IN":
-00004d00: 205b 2274 6f22 5d7d 7d2c 5645 5242 5d5d   ["to"]}},VERB]]
-00004d10: 2c0a 7d0a 6465 6620 7665 7262 6e65 745f  ,.}.def verbnet_
-00004d20: 6d61 7463 6865 7228 646f 6329 3a20 0a09  matcher(doc): ..
-00004d30: 6966 206e 6f74 2068 6173 6174 7472 2876  if not hasattr(v
-00004d40: 6572 626e 6574 5f6d 6174 6368 6572 2c20  erbnet_matcher, 
-00004d50: 276d 6174 6368 6572 2729 3a20 0a09 0976  'matcher'): ...v
-00004d60: 6572 626e 6574 5f6d 6174 6368 6572 2e6d  erbnet_matcher.m
-00004d70: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
-00004d80: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
-00004d90: 290a 0909 5b20 7665 7262 6e65 745f 6d61  )...[ verbnet_ma
-00004da0: 7463 6865 722e 6d61 7463 6865 722e 6164  tcher.matcher.ad
-00004db0: 6428 6e61 6d65 2c20 7061 7474 6572 6e73  d(name, patterns
-00004dc0: 2c20 6772 6565 6479 203d 274c 4f4e 4745  , greedy ='LONGE
-00004dd0: 5354 2729 2020 666f 7220 6e61 6d65 2c20  ST')  for name, 
-00004de0: 7061 7474 6572 6e73 2069 6e20 5f76 6572  patterns in _ver
-00004df0: 626e 6574 5f72 756c 6573 2e69 7465 6d73  bnet_rules.items
-00004e00: 2829 205d 0a09 6d65 7267 655f 6e70 2864  () ]..merge_np(d
-00004e10: 6f63 290a 096d 6572 6765 5f76 7028 646f  oc)..merge_vp(do
-00004e20: 6329 0a09 7265 7320 3d20 5b5d 0a09 666f  c)..res = []..fo
-00004e30: 7220 6e61 6d65 2c20 6962 6567 2c20 6965  r name, ibeg, ie
-00004e40: 6e64 2069 6e20 7665 7262 6e65 745f 6d61  nd in verbnet_ma
-00004e50: 7463 6865 722e 6d61 7463 6865 7228 646f  tcher.matcher(do
-00004e60: 6329 3a0a 0909 7472 793a 0a09 0909 6172  c):...try:....ar
-00004e70: 7220 3d20 7370 6163 792e 6e6c 702e 766f  r = spacy.nlp.vo
-00004e80: 6361 625b 6e61 6d65 5d2e 7465 7874 2e73  cab[name].text.s
-00004e90: 706c 6974 2827 3a27 2920 0a09 0909 7665  plit(':') ....ve
-00004ea0: 7262 5f69 203d 2069 6265 6720 2b20 696e  rb_i = ibeg + in
-00004eb0: 7428 6172 725b 2d31 5d29 200a 0909 0972  t(arr[-1]) ....r
-00004ec0: 6573 2e61 7070 656e 6428 2028 7665 7262  es.append( (verb
-00004ed0: 5f69 2c20 6962 6567 2c20 6965 6e64 2c20  _i, ibeg, iend, 
-00004ee0: 6172 725b 305d 2e73 7472 6970 2829 2920  arr[0].strip()) 
-00004ef0: 2920 0a09 0965 7863 6570 7420 4578 6365  ) ...except Exce
-00004f00: 7074 696f 6e20 6173 2065 3a0a 0909 0970  ption as e:....p
-00004f10: 7269 6e74 2028 2776 6572 626e 6574 2065  rint ('verbnet e
-00004f20: 783a 272c 2065 2c20 6e61 6d65 2c20 6962  x:', e, name, ib
-00004f30: 6567 2c20 6965 6e64 290a 0972 6574 7572  eg, iend)..retur
-00004f40: 6e20 7265 7320 0a0a 7369 6d70 6c65 5f73  n res ..simple_s
-00004f50: 656e 7409 093d 206c 616d 6264 6120 646f  ent..= lambda do
-00004f60: 633a 206c 656e 285b 7420 666f 7220 7420  c: len([t for t 
-00004f70: 696e 2064 6f63 2069 6620 742e 706f 735f  in doc if t.pos_
-00004f80: 203d 3d20 2756 4552 4227 2061 6e64 2074   == 'VERB' and t
-00004f90: 2e64 6570 5f20 213d 2027 524f 4f54 275d  .dep_ != 'ROOT']
-00004fa0: 2920 3c3d 2030 200a 636f 6d70 6c65 785f  ) <= 0 .complex_
-00004fb0: 7365 6e74 093d 206c 616d 6264 6120 646f  sent.= lambda do
-00004fc0: 633a 206c 656e 285b 7420 666f 7220 7420  c: len([t for t 
-00004fd0: 696e 2064 6f63 2069 6620 742e 706f 735f  in doc if t.pos_
-00004fe0: 203d 3d20 2756 4552 4227 2061 6e64 2074   == 'VERB' and t
-00004ff0: 2e64 6570 5f20 213d 2027 524f 4f54 275d  .dep_ != 'ROOT']
-00005000: 2920 3e20 300a 636f 6d70 6f75 6e64 5f73  ) > 0.compound_s
-00005010: 656e 7409 3d20 6c61 6d62 6461 2064 6f63  ent.= lambda doc
-00005020: 3a20 6c65 6e28 5b74 2066 6f72 2074 2069  : len([t for t i
-00005030: 6e20 646f 6320 6966 2074 2e64 6570 5f20  n doc if t.dep_ 
-00005040: 3d3d 2027 636f 6e6a 2720 616e 6420 742e  == 'conj' and t.
-00005050: 6865 6164 2e64 6570 5f20 3d3d 2027 524f  head.dep_ == 'RO
-00005060: 4f54 275d 2920 3e20 3020 2023 2053 2e63  OT']) > 0  # S.c
-00005070: 6f6e 6a20 0a73 7479 7065 0909 093d 206c  onj .stype...= l
-00005080: 616d 6264 6120 646f 633a 0922 7369 6d70  ambda doc:."simp
-00005090: 6c65 5f73 656e 7422 2069 6620 6c65 6e28  le_sent" if len(
-000050a0: 5b74 2066 6f72 2074 2069 6e20 646f 6320  [t for t in doc 
-000050b0: 6966 2074 2e70 6f73 5f20 3d3d 2027 5645  if t.pos_ == 'VE
-000050c0: 5242 2720 616e 6420 742e 6465 705f 2021  RB' and t.dep_ !
-000050d0: 3d20 2752 4f4f 5427 5d29 203c 3d20 3020  = 'ROOT']) <= 0 
-000050e0: 656c 7365 2022 636f 6d70 6c65 785f 7365  else "complex_se
-000050f0: 6e74 220a 736b 656c 6574 6f6e 0909 3d20  nt".skeleton..= 
-00005100: 6c61 6d62 6461 2064 6f63 3a20 2022 2022  lambda doc:  " "
-00005110: 2e6a 6f69 6e28 5b20 742e 656e 745f 7479  .join([ t.ent_ty
-00005120: 7065 5f20 6966 2074 2e65 6e74 5f74 7970  pe_ if t.ent_typ
-00005130: 655f 2065 6c73 6520 742e 7465 7874 2069  e_ else t.text i
-00005140: 6620 742e 6973 5f70 756e 6374 206f 7220  f t.is_punct or 
-00005150: 742e 6465 705f 203d 3d20 2752 4f4f 5427  t.dep_ == 'ROOT'
-00005160: 2065 6c73 6520 742e 706f 735f 2066 6f72   else t.pos_ for
-00005170: 2074 2069 6e20 646f 6320 5d29 0a0a 6465   t in doc ])..de
-00005180: 6620 636c 6175 7365 2864 6f63 293a 2020  f clause(doc):  
-00005190: 2320 7b27 532e 7072 6570 2d30 273a 207b  # {'S.prep-0': {
-000051a0: 2774 7970 6527 3a20 2753 2e70 7265 7027  'type': 'S.prep'
-000051b0: 2c20 2773 7461 7274 273a 2030 2c20 2765  , 'start': 0, 'e
-000051c0: 6e64 273a 2032 2c20 276c 656d 273a 2027  nd': 2, 'lem': '
-000051d0: 636f 6e73 6964 6572 272c 2027 6368 756e  consider', 'chun
-000051e0: 6b27 3a20 2743 6f6e 7369 6465 7269 6e67  k': 'Considering
-000051f0: 2074 6865 2070 6f73 7369 6269 6c69 7479   the possibility
-00005200: 277d 2c20 2753 2e63 6f6e 6a2d 3927 3a20  '}, 'S.conj-9': 
-00005210: 7b27 7479 7065 273a 2027 532e 636f 6e6a  {'type': 'S.conj
-00005220: 272c 2027 7374 6172 7427 3a20 392c 2027  ', 'start': 9, '
-00005230: 656e 6427 3a20 3132 2c20 276c 656d 273a  end': 12, 'lem':
-00005240: 2027 6265 272c 2027 6368 756e 6b27 3a20   'be', 'chunk': 
-00005250: 2773 6865 2069 7320 6f6b 202e 277d 7d0a  'she is ok .'}}.
-00005260: 0961 7272 203d 205b 5d0a 0966 6f72 2076  .arr = []..for v
-00005270: 2069 6e20 5b74 2066 6f72 2074 2069 6e20   in [t for t in 
-00005280: 646f 6320 6966 2074 2e70 6f73 5f20 3d3d  doc if t.pos_ ==
-00005290: 2027 5645 5242 2720 616e 6420 742e 6465   'VERB' and t.de
-000052a0: 705f 2021 3d20 2752 4f4f 5427 205d 203a  p_ != 'ROOT' ] :
-000052b0: 2023 206e 6f6e 2d72 6f6f 740a 0909 6368   # non-root...ch
-000052c0: 696c 6472 656e 203d 206c 6973 7428 762e  ildren = list(v.
-000052d0: 7375 6274 7265 6529 2023 656e 6420 3d20  subtree) #end = 
-000052e0: 6368 696c 6472 656e 5b2d 315d 2e69 2009  children[-1].i .
-000052f0: 7461 6720 3d20 2253 2e22 202b 2076 2e64  tag = "S." + v.d
-00005300: 6570 5f20 2020 2320 532e 6164 7663 6c20  ep_   # S.advcl 
-00005310: 2c20 2053 2e63 6f6e 6a20 0a09 0973 7461  ,  S.conj ...sta
-00005320: 7274 203d 2063 6869 6c64 7265 6e5b 305d  rt = children[0]
-00005330: 2e69 0a09 0965 6e64 203d 2063 6869 6c64  .i...end = child
-00005340: 7265 6e5b 2d31 5d2e 6920 2b20 3120 2322  ren[-1].i + 1 #"
-00005350: 7479 7065 223a 2263 6c22 2c20 226b 7022  type":"cl", "kp"
-00005360: 3a20 2253 2e22 202b 2076 2e64 6570 5f2c  : "S." + v.dep_,
-00005370: 0a09 0961 7272 2e61 7070 656e 6428 2028  ...arr.append( (
-00005380: 762c 2076 2e64 6570 5f2c 2073 7461 7274  v, v.dep_, start
-00005390: 2c20 656e 642c 2022 2022 2e6a 6f69 6e28  , end, " ".join(
-000053a0: 5b63 2e74 6578 7420 666f 7220 6320 696e  [c.text for c in
-000053b0: 2076 2e73 7562 7472 6565 5d29 2920 2920   v.subtree])) ) 
-000053c0: 236c 6173 7420 6f6e 6520 6973 2027 6368  #last one is 'ch
-000053d0: 756e 6b27 2020 206c 656d 706f 7322 3a76  unk'   lempos":v
-000053e0: 2e6c 656d 6d61 5f20 2b20 225f 2220 2b20  .lemma_ + "_" + 
-000053f0: 762e 706f 735f 2c22 6368 756e 6b22 3a20  v.pos_,"chunk": 
-00005400: 7d20 2322 6c65 6d22 3a76 2e6c 656d 6d61  } #"lem":v.lemma
-00005410: 5f2c 204e 4f54 2063 6f6e 6675 7365 2077  _, NOT confuse w
-00005420: 6974 6820 2774 6f6b 2720 0a09 7265 7475  ith 'tok' ..retu
-00005430: 726e 2061 7272 200a 0a5f 7670 5f72 756c  rn arr .._vp_rul
-00005440: 6573 203d 207b 0a22 7665 6e64 223a 5b5b  es = {."vend":[[
-00005450: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
-00005460: 2241 5558 222c 2256 4552 4222 5d7d 7d2c  "AUX","VERB"]}},
-00005470: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
-00005480: 2241 4456 225d 7d2c 2022 4f50 223a 2022  "ADV"]}, "OP": "
-00005490: 2a22 7d2c 207b 2250 4f53 223a 207b 2249  *"}, {"POS": {"I
-000054a0: 4e22 3a20 5b22 4144 4a22 2c22 5645 5242  N": ["ADJ","VERB
-000054b0: 225d 7d2c 2022 4f50 223a 2022 2a22 7d2c  "]}, "OP": "*"},
-000054c0: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
-000054d0: 2250 4152 5422 2c22 4144 5022 2c22 544f  "PART","ADP","TO
-000054e0: 225d 7d2c 2022 4f50 223a 2022 2a22 7d2c  "]}, "OP": "*"},
-000054f0: 7b22 504f 5322 3a20 2756 4552 4227 7d5d  {"POS": 'VERB'}]
-00005500: 5d2c 2023 2063 6f75 6c64 2068 6172 646c  ], # could hardl
-00005510: 7920 7761 6974 2074 6f20 6d65 6574 0a22  y wait to meet."
-00005520: 7670 223a 2020 5b5b 7b27 504f 5327 3a20  vp":  [[{'POS': 
-00005530: 2756 4552 4227 7d2c 7b22 504f 5322 3a20  'VERB'},{"POS": 
-00005540: 7b22 494e 223a 205b 2244 4554 222c 2241  {"IN": ["DET","A
-00005550: 4450 222c 2241 444a 225d 7d2c 2022 4f50  DP","ADJ"]}, "OP
-00005560: 223a 2022 2a22 7d2c 7b22 504f 5322 3a20  ": "*"},{"POS": 
-00005570: 274e 4f55 4e27 7d2c 207b 2250 4f53 223a  'NOUN'}, {"POS":
-00005580: 207b 2249 4e22 3a20 5b22 4144 5022 2c22   {"IN": ["ADP","
-00005590: 544f 225d 7d2c 2022 4f50 223a 2022 2a22  TO"]}, "OP": "*"
-000055a0: 7d5d 2c20 5b7b 2750 4f53 273a 2027 5645  }], [{'POS': 'VE
-000055b0: 5242 277d 2c7b 2250 4f53 223a 207b 2249  RB'},{"POS": {"I
-000055c0: 4e22 3a20 5b22 4445 5422 2c22 4144 5022  N": ["DET","ADP"
-000055d0: 2c22 4144 4a22 2c22 544f 222c 2250 4152  ,"ADJ","TO","PAR
-000055e0: 5422 5d7d 2c20 224f 5022 3a20 222a 227d  T"]}, "OP": "*"}
-000055f0: 2c7b 2250 4f53 223a 2027 5645 5242 277d  ,{"POS": 'VERB'}
-00005600: 5d5d 2c20 2320 7761 6974 2074 6f20 6d65  ]], # wait to me
-00005610: 6574 0a22 7070 223a 2020 5b5b 7b27 504f  et."pp":  [[{'PO
-00005620: 5327 3a20 2741 4450 277d 2c7b 2250 4f53  S': 'ADP'},{"POS
-00005630: 223a 207b 2249 4e22 3a20 5b22 4445 5422  ": {"IN": ["DET"
-00005640: 2c22 4e55 4d22 2c22 4144 4a22 2c27 5055  ,"NUM","ADJ",'PU
-00005650: 4e43 5427 2c27 434f 4e4a 275d 7d2c 2022  NCT','CONJ']}, "
-00005660: 4f50 223a 2022 2a22 7d2c 7b22 504f 5322  OP": "*"},{"POS"
-00005670: 3a20 7b22 494e 223a 205b 224e 4f55 4e22  : {"IN": ["NOUN"
-00005680: 2c22 5041 5254 225d 7d2c 2022 4f50 223a  ,"PART"]}, "OP":
-00005690: 2022 2b22 7d5d 5d2c 2020 2020 0a22 6170   "+"}]],    ."ap
-000056a0: 223a 2020 5b5b 7b22 504f 5322 3a20 7b22  ":  [[{"POS": {"
-000056b0: 494e 223a 205b 2241 4456 225d 7d2c 2022  IN": ["ADV"]}, "
-000056c0: 4f50 223a 2022 2a22 7d2c 207b 2250 4f53  OP": "*"}, {"POS
-000056d0: 223a 2027 4144 4a27 7d5d 5d2c 2020 0a22  ": 'ADJ'}]],  ."
-000056e0: 7670 7274 223a 5b5b 7b22 504f 5322 3a20  vprt":[[{"POS": 
-000056f0: 2756 4552 4227 7d2c 207b 2250 4f53 223a  'VERB'}, {"POS":
-00005700: 207b 2249 4e22 3a20 5b22 5052 4550 222c   {"IN": ["PREP",
-00005710: 2022 4144 5022 2c27 544f 275d 7d2c 2022   "ADP",'TO']}, "
-00005720: 4f50 223a 2022 2b22 7d5d 5d2c 2020 2023  OP": "+"}]],   #
-00005730: 206c 6f6f 6b20 7570 202f 6c6f 6f6b 2075   look up /look u
-00005740: 7020 6672 6f6d 2c20 2063 6f6d 7075 7465  p from,  compute
-00005750: 6420 7477 6963 650a 2276 746f 7622 3a5b  d twice."vtov":[
-00005760: 5b7b 2250 4f53 223a 2027 5645 5242 277d  [{"POS": 'VERB'}
-00005770: 2c20 7b22 5441 4722 3a20 2754 4f27 7d2c  , {"TAG": 'TO'},
-00005780: 7b22 5441 4722 3a20 2756 4227 7d5d 5d2c  {"TAG": 'VB'}]],
-00005790: 2020 2023 2070 6c61 6e20 746f 2067 6f0a     # plan to go.
-000057a0: 2276 7662 6722 3a5b 5b7b 2250 4f53 223a  "vvbg":[[{"POS":
-000057b0: 2027 5645 5242 277d 2c20 7b22 5441 4722   'VERB'}, {"TAG"
-000057c0: 3a20 2756 4247 277d 5d5d 2c20 2020 2320  : 'VBG'}]],   # 
-000057d0: 636f 6e73 6964 6572 2067 6f69 6e67 0a22  consider going."
-000057e0: 7670 6722 3a20 5b5b 7b22 504f 5322 3a20  vpg": [[{"POS": 
-000057f0: 2756 4552 4227 7d2c 207b 2250 4f53 223a  'VERB'}, {"POS":
-00005800: 207b 2249 4e22 3a20 5b22 5052 4550 222c   {"IN": ["PREP",
-00005810: 2022 4144 5022 2c27 5041 5254 275d 7d2c   "ADP",'PART']},
-00005820: 2022 4f50 223a 2022 2b22 7d2c 7b22 5441   "OP": "+"},{"TA
-00005830: 4722 3a20 2756 4247 277d 5d5d 2c20 2020  G": 'VBG'}]],   
-00005840: 2320 696e 7369 7374 6564 206f 6e20 676f  # insisted on go
-00005850: 696e 670a 2276 4170 223a 205b 5b7b 274c  ing."vAp": [[{'L
-00005860: 454d 4d41 273a 2027 6265 277d 2c7b 2254  EMMA': 'be'},{"T
-00005870: 4147 223a 207b 2249 4e22 3a20 5b22 5642  AG": {"IN": ["VB
-00005880: 4e22 5d7d 7d2c 207b 2250 4f53 223a 207b  N"]}}, {"POS": {
-00005890: 2249 4e22 3a20 5b22 5052 4550 222c 2022  "IN": ["PREP", "
-000058a0: 4144 5022 2c27 5041 5254 275d 7d7d 5d5d  ADP",'PART']}}]]
-000058b0: 2c20 2020 2320 6265 2062 6173 6564 206f  ,   # be based o
-000058c0: 6e20 2020 0a22 7661 7022 3a20 5b5b 7b27  n   ."vap": [[{'
-000058d0: 4c45 4d4d 4127 3a20 2762 6527 7d2c 7b22  LEMMA': 'be'},{"
-000058e0: 504f 5322 3a20 7b22 494e 223a 205b 2241  POS": {"IN": ["A
-000058f0: 444a 225d 7d7d 2c20 7b22 504f 5322 3a20  DJ"]}}, {"POS": 
-00005900: 7b22 494e 223a 205b 2250 5245 5022 2c20  {"IN": ["PREP", 
-00005910: 2241 4450 222c 2750 4152 5427 5d7d 7d5d  "ADP",'PART']}}]
-00005920: 5d2c 2020 2023 2062 6520 616e 6772 7920  ],   # be angry 
-00005930: 7769 7468 0a7d 2023 666f 7220 6e61 6d65  with.} #for name
-00005940: 2c20 6962 6567 2c69 656e 6420 696e 206d  , ibeg,iend in m
-00005950: 6174 6368 6572 2864 6f63 2920 3a20 7072  atcher(doc) : pr
-00005960: 696e 7428 7370 6163 792e 6e6c 702e 766f  int(spacy.nlp.vo
-00005970: 6361 625b 6e61 6d65 5d2e 7465 7874 2c20  cab[name].text, 
-00005980: 646f 635b 6962 6567 3a69 656e 645d 2e74  doc[ibeg:iend].t
-00005990: 6578 7429 0a0a 6465 6620 7670 5f6d 6174  ext)..def vp_mat
-000059a0: 6368 6572 2864 6f63 293a 2023 5b28 2776  cher(doc): #[('v
-000059b0: 656e 6427 2c20 2763 6f6e 7369 6465 7220  end', 'consider 
-000059c0: 676f 696e 6727 2c20 312c 2033 292c 2028  going', 1, 3), (
-000059d0: 2776 7027 2c20 2763 6f6e 7369 6465 7220  'vp', 'consider 
-000059e0: 676f 696e 6727 2c20 312c 2033 292c 2028  going', 1, 3), (
-000059f0: 2776 7662 6727 2c20 2763 6f6e 7369 6465  'vvbg', 'conside
-00005a00: 7220 676f 696e 6727 2c20 312c 2033 292c  r going', 1, 3),
-00005a10: 2028 2776 7072 7427 2c20 2767 6f69 6e67   ('vprt', 'going
-00005a20: 2074 6f27 2c20 322c 2034 295d 0a09 6966   to', 2, 4)]..if
-00005a30: 206e 6f74 2068 6173 6174 7472 2876 705f   not hasattr(vp_
-00005a40: 6d61 7463 6865 722c 2027 6d61 7463 6865  matcher, 'matche
-00005a50: 7227 293a 200a 0909 7670 5f6d 6174 6368  r'): ...vp_match
-00005a60: 6572 2e6d 6174 6368 6572 203d 204d 6174  er.matcher = Mat
-00005a70: 6368 6572 2873 7061 6379 2e6e 6c70 2e76  cher(spacy.nlp.v
-00005a80: 6f63 6162 290a 0909 5b76 705f 6d61 7463  ocab)...[vp_matc
-00005a90: 6865 722e 6d61 7463 6865 722e 6164 6428  her.matcher.add(
-00005aa0: 6e61 6d65 2c20 7061 7474 6572 6e73 2c20  name, patterns, 
-00005ab0: 2067 7265 6564 7920 3d27 4c4f 4e47 4553   greedy ='LONGES
-00005ac0: 5427 2920 666f 7220 6e61 6d65 2c20 7061  T') for name, pa
-00005ad0: 7474 6572 6e73 2069 6e20 5f76 705f 7275  tterns in _vp_ru
-00005ae0: 6c65 732e 6974 656d 7328 2920 5d0a 0923  les.items() ]..#
-00005af0: 7265 7475 726e 205b 2873 7061 6379 2e6e  return [(spacy.n
-00005b00: 6c70 2e76 6f63 6162 5b6e 616d 655d 2e74  lp.vocab[name].t
-00005b10: 6578 742c 2076 705f 7370 616e 2864 6f63  ext, vp_span(doc
-00005b20: 2c69 6265 672c 6965 6e64 292c 2069 6265  ,ibeg,iend), ibe
-00005b30: 672c 2069 656e 6429 2066 6f72 206e 616d  g, iend) for nam
-00005b40: 652c 2069 6265 672c 6965 6e64 2069 6e20  e, ibeg,iend in 
-00005b50: 7670 5f6d 6174 6368 6572 2e6d 6174 6368  vp_matcher.match
-00005b60: 6572 2864 6f63 295d 200a 0974 7570 7320  er(doc)] ..tups 
-00005b70: 3d20 7365 7428 2920 2023 2072 656d 6f76  = set()  # remov
-00005b80: 6520 7468 6520 6475 706c 6963 6174 6564  e the duplicated
-00005b90: 2065 6e74 7269 6573 200a 095b 7475 7073   entries ..[tups
-00005ba0: 2e61 6464 2828 7370 6163 792e 6e6c 702e  .add((spacy.nlp.
-00005bb0: 766f 6361 625b 6e61 6d65 5d2e 7465 7874  vocab[name].text
-00005bc0: 2c20 7670 5f73 7061 6e28 646f 632c 6962  , vp_span(doc,ib
-00005bd0: 6567 2c69 656e 6429 2c20 6962 6567 2c20  eg,iend), ibeg, 
-00005be0: 6965 6e64 2929 2066 6f72 206e 616d 652c  iend)) for name,
-00005bf0: 2069 6265 672c 6965 6e64 2069 6e20 7670   ibeg,iend in vp
-00005c00: 5f6d 6174 6368 6572 2e6d 6174 6368 6572  _matcher.matcher
-00005c10: 2864 6f63 295d 200a 0972 6574 7572 6e20  (doc)] ..return 
-00005c20: 7475 7073 0a0a 5f64 6570 5f72 756c 6573  tups.._dep_rules
-00005c30: 203d 207b 0a22 7376 6f22 3a5b 207b 2252   = {."svo":[ {"R
-00005c40: 4947 4854 5f49 4422 3a20 2276 222c 2020  IGHT_ID": "v",  
-00005c50: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
-00005c60: 2250 4f53 223a 2022 5645 5242 227d 7d2c  "POS": "VERB"}},
-00005c70: 207b 224c 4546 545f 4944 223a 2022 7622   {"LEFT_ID": "v"
-00005c80: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
-00005c90: 2022 5249 4748 545f 4944 223a 2022 7375   "RIGHT_ID": "su
-00005ca0: 626a 6563 7422 2c20 2252 4947 4854 5f41  bject", "RIGHT_A
-00005cb0: 5454 5253 223a 207b 2244 4550 223a 2022  TTRS": {"DEP": "
-00005cc0: 6e73 7562 6a22 7d7d 2c7b 224c 4546 545f  nsubj"}},{"LEFT_
-00005cd0: 4944 223a 2022 7622 2c20 2252 454c 5f4f  ID": "v", "REL_O
-00005ce0: 5022 3a20 223e 222c 2022 5249 4748 545f  P": ">", "RIGHT_
-00005cf0: 4944 223a 2022 6f62 6a65 6374 222c 2252  ID": "object","R
-00005d00: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
-00005d10: 4550 223a 2022 646f 626a 227d 2020 7d5d  EP": "dobj"}  }]
-00005d20: 2c20 2320 5b28 3438 3531 3336 3331 3232  , # [(4851363122
-00005d30: 3936 3236 3734 3137 362c 205b 322c 2030  962674176, [2, 0
-00005d40: 2c20 345d 295d 0a22 7376 6122 3a5b 207b  , 4])]."sva":[ {
-00005d50: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
-00005d60: 2020 2252 4947 4854 5f41 5454 5253 223a    "RIGHT_ATTRS":
-00005d70: 207b 2250 4f53 223a 2022 5645 5242 227d   {"POS": "VERB"}
-00005d80: 7d2c 207b 224c 4546 545f 4944 223a 2022  }, {"LEFT_ID": "
-00005d90: 7622 2c20 2252 454c 5f4f 5022 3a20 223e  v", "REL_OP": ">
-00005da0: 222c 2022 5249 4748 545f 4944 223a 2022  ", "RIGHT_ID": "
-00005db0: 7375 626a 6563 7422 2c20 2252 4947 4854  subject", "RIGHT
-00005dc0: 5f41 5454 5253 223a 207b 2244 4550 223a  _ATTRS": {"DEP":
-00005dd0: 2022 6e73 7562 6a22 7d7d 2c7b 224c 4546   "nsubj"}},{"LEF
-00005de0: 545f 4944 223a 2022 7622 2c20 2252 454c  T_ID": "v", "REL
-00005df0: 5f4f 5022 3a20 223e 222c 2022 5249 4748  _OP": ">", "RIGH
-00005e00: 545f 4944 223a 2022 6f62 6a65 6374 222c  T_ID": "object",
-00005e10: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
-00005e20: 2244 4550 223a 2022 6163 6f6d 7022 7d7d  "DEP": "acomp"}}
-00005e30: 5d2c 200a 2320 706c 616e 2074 6f20 676f  ], .# plan to go
-00005e40: 202c 2065 6e6a 6f79 2073 7769 6d6d 696e   , enjoy swimmin
-00005e50: 6720 0a22 7376 7822 3a5b 207b 2252 4947  g ."svx":[ {"RIG
-00005e60: 4854 5f49 4422 3a20 2276 222c 2022 5249  HT_ID": "v", "RI
-00005e70: 4748 545f 4154 5452 5322 3a20 7b22 504f  GHT_ATTRS": {"PO
-00005e80: 5322 3a20 2256 4552 4222 7d7d 2c20 7b22  S": "VERB"}}, {"
-00005e90: 4c45 4654 5f49 4422 3a20 2276 222c 2022  LEFT_ID": "v", "
-00005ea0: 5245 4c5f 4f50 223a 2022 3e22 2c20 2252  REL_OP": ">", "R
-00005eb0: 4947 4854 5f49 4422 3a20 2273 7562 6a65  IGHT_ID": "subje
-00005ec0: 6374 222c 2022 5249 4748 545f 4154 5452  ct", "RIGHT_ATTR
-00005ed0: 5322 3a20 7b22 4445 5022 3a20 226e 7375  S": {"DEP": "nsu
-00005ee0: 626a 227d 7d2c 207b 224c 4546 545f 4944  bj"}}, {"LEFT_ID
-00005ef0: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
-00005f00: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
-00005f10: 223a 2022 6f62 6a65 6374 222c 2252 4947  ": "object","RIG
-00005f20: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
-00005f30: 223a 2022 7863 6f6d 7022 7d7d 5d2c 200a  ": "xcomp"}}], .
-00005f40: 2320 4920 7468 696e 6b20 6974 2069 7320  # I think it is 
-00005f50: 7269 6768 742e 0a22 7376 6322 3a5b 207b  right.."svc":[ {
-00005f60: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
-00005f70: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
-00005f80: 2250 4f53 223a 2022 5645 5242 227d 7d2c  "POS": "VERB"}},
-00005f90: 207b 224c 4546 545f 4944 223a 2022 7622   {"LEFT_ID": "v"
-00005fa0: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
-00005fb0: 2022 5249 4748 545f 4944 223a 2022 7375   "RIGHT_ID": "su
-00005fc0: 626a 6563 7422 2c20 2252 4947 4854 5f41  bject", "RIGHT_A
-00005fd0: 5454 5253 223a 207b 2244 4550 223a 2022  TTRS": {"DEP": "
-00005fe0: 6e73 7562 6a22 7d7d 2c20 7b22 4c45 4654  nsubj"}}, {"LEFT
-00005ff0: 5f49 4422 3a20 2276 222c 2022 5245 4c5f  _ID": "v", "REL_
-00006000: 4f50 223a 2022 3e22 2c20 2252 4947 4854  OP": ">", "RIGHT
-00006010: 5f49 4422 3a20 226f 626a 6563 7422 2c20  _ID": "object", 
-00006020: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
-00006030: 2244 4550 223a 2022 6363 6f6d 7022 7d7d  "DEP": "ccomp"}}
-00006040: 5d2c 200a 2353 6865 2069 7320 2061 2067  ], .#She is  a g
-00006050: 6972 6c2e 0a22 7361 7474 7222 3a5b 207b  irl.."sattr":[ {
-00006060: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
-00006070: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
-00006080: 7b22 4c45 4d4d 4122 3a20 2262 6522 7d7d  {"LEMMA": "be"}}
-00006090: 2c20 7b22 4c45 4654 5f49 4422 3a20 2276  , {"LEFT_ID": "v
-000060a0: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
-000060b0: 2c20 2252 4947 4854 5f49 4422 3a20 2273  , "RIGHT_ID": "s
-000060c0: 7562 6a65 6374 222c 2252 4947 4854 5f41  ubject","RIGHT_A
-000060d0: 5454 5253 223a 207b 2244 4550 223a 2022  TTRS": {"DEP": "
-000060e0: 6e73 7562 6a22 7d7d 2c7b 224c 4546 545f  nsubj"}},{"LEFT_
-000060f0: 4944 223a 2022 7622 2c22 5245 4c5f 4f50  ID": "v","REL_OP
-00006100: 223a 2022 3e22 2c20 2252 4947 4854 5f49  ": ">", "RIGHT_I
-00006110: 4422 3a20 226f 626a 6563 7422 2c22 5249  D": "object","RI
-00006120: 4748 545f 4154 5452 5322 3a20 7b22 4445  GHT_ATTRS": {"DE
-00006130: 5022 3a20 2261 7474 7222 7d20 207d 5d2c  P": "attr"}  }],
-00006140: 200a 2320 7475 726e 206f 6666 2074 6865   .# turn off the
-00006150: 206c 6967 6874 0a22 7670 6e22 3a5b 207b   light."vpn":[ {
-00006160: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
-00006170: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
-00006180: 7b22 504f 5322 3a20 2256 4552 4222 7d7d  {"POS": "VERB"}}
-00006190: 2c20 7b22 4c45 4654 5f49 4422 3a20 2276  , {"LEFT_ID": "v
-000061a0: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
-000061b0: 2c20 2252 4947 4854 5f49 4422 3a20 2273  , "RIGHT_ID": "s
-000061c0: 7562 6a65 6374 222c 2022 5249 4748 545f  ubject", "RIGHT_
-000061d0: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
-000061e0: 2270 7274 227d 7d2c 207b 224c 4546 545f  "prt"}}, {"LEFT_
-000061f0: 4944 223a 2022 7622 2c20 2252 454c 5f4f  ID": "v", "REL_O
-00006200: 5022 3a20 223e 222c 2252 4947 4854 5f49  P": ">","RIGHT_I
-00006210: 4422 3a20 226f 626a 6563 7422 2c22 5249  D": "object","RI
-00006220: 4748 545f 4154 5452 5322 3a20 7b22 4445  GHT_ATTRS": {"DE
-00006230: 5022 3a20 2264 6f62 6a22 7d20 7d5d 2c20  P": "dobj"} }], 
-00006240: 0a23 2062 6520 6861 7070 7920 7769 7468  .# be happy with
-00006250: 0a22 7661 7022 3a5b 207b 2252 4947 4854  ."vap":[ {"RIGHT
-00006260: 5f49 4422 3a20 2276 222c 2022 5249 4748  _ID": "v", "RIGH
-00006270: 545f 4154 5452 5322 3a20 7b22 504f 5322  T_ATTRS": {"POS"
-00006280: 3a20 2256 4552 4222 7d7d 2c20 7b22 4c45  : "VERB"}}, {"LE
-00006290: 4654 5f49 4422 3a20 2276 222c 2022 5245  FT_ID": "v", "RE
-000062a0: 4c5f 4f50 223a 2022 3e22 2c20 2252 4947  L_OP": ">", "RIG
-000062b0: 4854 5f49 4422 3a20 2261 636f 6d70 222c  HT_ID": "acomp",
-000062c0: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
-000062d0: 2244 4550 223a 2022 6163 6f6d 7022 7d7d  "DEP": "acomp"}}
-000062e0: 2c7b 224c 4546 545f 4944 223a 2022 6163  ,{"LEFT_ID": "ac
-000062f0: 6f6d 7022 2c20 2252 454c 5f4f 5022 3a20  omp", "REL_OP": 
-00006300: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
-00006310: 2022 7072 6570 222c 2022 5249 4748 545f   "prep", "RIGHT_
-00006320: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
-00006330: 2270 7265 7022 7d20 7d5d 2c20 0a23 2062  "prep"} }], .# b
-00006340: 6520 6261 7365 6420 6f6e 0a22 7664 7022  e based on."vdp"
-00006350: 3a5b 207b 2252 4947 4854 5f49 4422 3a20  :[ {"RIGHT_ID": 
-00006360: 2276 222c 2022 5249 4748 545f 4154 5452  "v", "RIGHT_ATTR
-00006370: 5322 3a20 7b22 5441 4722 3a20 2256 424e  S": {"TAG": "VBN
-00006380: 227d 7d2c 207b 224c 4546 545f 4944 223a  "}}, {"LEFT_ID":
-00006390: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
-000063a0: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
-000063b0: 2022 6265 222c 2022 5249 4748 545f 4154   "be", "RIGHT_AT
-000063c0: 5452 5322 3a20 7b22 4c45 4d4d 4122 3a20  TRS": {"LEMMA": 
-000063d0: 2262 6522 7d7d 2c7b 224c 4546 545f 4944  "be"}},{"LEFT_ID
-000063e0: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
-000063f0: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
-00006400: 223a 2022 7072 6570 222c 2022 5249 4748  ": "prep", "RIGH
-00006410: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
-00006420: 3a20 2270 7265 7022 7d7d 5d2c 200a 2320  : "prep"}}], .# 
-00006430: 6c6f 6f6b 2075 7020 6672 6f6d 2070 686f  look up from pho
-00006440: 6e65 0a22 7670 706e 223a 5b20 7b22 5249  ne."vppn":[ {"RI
-00006450: 4748 545f 4944 223a 2022 7622 2c20 2252  GHT_ID": "v", "R
-00006460: 4947 4854 5f41 5454 5253 223a 207b 2250  IGHT_ATTRS": {"P
-00006470: 4f53 223a 2022 5645 5242 227d 7d2c 207b  OS": "VERB"}}, {
-00006480: 2022 4c45 4654 5f49 4422 3a20 2276 222c   "LEFT_ID": "v",
-00006490: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
-000064a0: 5249 4748 545f 4944 223a 2022 7072 7422  RIGHT_ID": "prt"
-000064b0: 2c20 2252 4947 4854 5f41 5454 5253 223a  , "RIGHT_ATTRS":
-000064c0: 207b 2244 4550 223a 2022 7072 7422 7d7d   {"DEP": "prt"}}
-000064d0: 2c7b 224c 4546 545f 4944 223a 2022 7622  ,{"LEFT_ID": "v"
-000064e0: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
-000064f0: 2022 5249 4748 545f 4944 223a 2022 7072   "RIGHT_ID": "pr
-00006500: 6570 222c 2022 5249 4748 545f 4154 5452  ep", "RIGHT_ATTR
-00006510: 5322 3a20 7b22 4445 5022 3a20 2270 7265  S": {"DEP": "pre
-00006520: 7022 7d7d 2c20 7b22 4c45 4654 5f49 4422  p"}}, {"LEFT_ID"
-00006530: 3a20 2270 7265 7022 2c20 2252 454c 5f4f  : "prep", "REL_O
-00006540: 5022 3a20 223e 222c 2022 5249 4748 545f  P": ">", "RIGHT_
-00006550: 4944 223a 2022 6f62 6a65 6374 222c 2022  ID": "object", "
-00006560: 5249 4748 545f 4154 5452 5322 3a20 7b22  RIGHT_ATTRS": {"
-00006570: 4445 5022 3a20 2270 6f62 6a22 7d7d 5d2c  DEP": "pobj"}}],
-00006580: 200a 2320 7661 7279 2066 726f 6d20 4120   .# vary from A 
-00006590: 746f 2042 0a22 7670 6e70 6e22 3a5b 207b  to B."vpnpn":[ {
-000065a0: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
-000065b0: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
-000065c0: 2250 4f53 223a 2022 5645 5242 227d 7d2c  "POS": "VERB"}},
-000065d0: 207b 224c 4546 545f 4944 223a 2022 7622   {"LEFT_ID": "v"
-000065e0: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
-000065f0: 2022 5249 4748 545f 4944 223a 2022 7072   "RIGHT_ID": "pr
-00006600: 6570 3122 2c20 2252 4947 4854 5f41 5454  ep1", "RIGHT_ATT
-00006610: 5253 223a 207b 2244 4550 223a 2022 7072  RS": {"DEP": "pr
-00006620: 6570 227d 7d2c 7b22 4c45 4654 5f49 4422  ep"}},{"LEFT_ID"
-00006630: 3a20 2270 7265 7031 222c 2022 5245 4c5f  : "prep1", "REL_
-00006640: 4f50 223a 2022 3e22 2c20 2252 4947 4854  OP": ">", "RIGHT
-00006650: 5f49 4422 3a20 226f 626a 6563 7431 222c  _ID": "object1",
-00006660: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
-00006670: 7b22 4445 5022 3a20 2270 6f62 6a22 7d7d  {"DEP": "pobj"}}
+00000750: 2320 7573 6167 653a 2020 656e 2e6d 6174  # usage:  en.mat
+00000760: 6368 6572 2820 7275 6c65 7329 2864 6f63  cher( rules)(doc
+00000770: 2920 0a64 6566 206d 6174 6368 6572 2820  ) .def matcher( 
+00000780: 7275 6c65 7320 3d7b 2770 7027 3a5b 5b7b  rules ={'pp':[[{
+00000790: 2750 4f53 273a 2027 4144 5027 7d2c 7b22  'POS': 'ADP'},{"
+000007a0: 504f 5322 3a20 7b22 494e 223a 205b 2244  POS": {"IN": ["D
+000007b0: 4554 222c 224e 554d 222c 2241 444a 222c  ET","NUM","ADJ",
+000007c0: 2750 554e 4354 272c 2743 4f4e 4a27 5d7d  'PUNCT','CONJ']}
+000007d0: 2c20 224f 5022 3a20 222a 227d 2c7b 2250  , "OP": "*"},{"P
+000007e0: 4f53 223a 207b 2249 4e22 3a20 5b22 4e4f  OS": {"IN": ["NO
+000007f0: 554e 222c 2250 4152 5422 5d7d 2c20 224f  UN","PART"]}, "O
+00000800: 5022 3a20 222b 227d 5d5d 207d 293a 0a09  P": "+"}]] }):..
+00000810: 2727 2720 3230 3233 2e37 2e37 2027 2727  ''' 2023.7.7 '''
+00000820: 0a09 6b65 7920 3d20 6a73 6f6e 2e64 756d  ..key = json.dum
+00000830: 7073 2872 756c 6573 290a 0969 6620 6e6f  ps(rules)..if no
+00000840: 7420 6861 7361 7474 7228 6d61 7463 6865  t hasattr(matche
+00000850: 722c 206b 6579 293a 200a 0909 6d20 3d20  r, key): ...m = 
+00000860: 4d61 7463 6865 7228 7370 6163 792e 6e6c  Matcher(spacy.nl
+00000870: 702e 766f 6361 6229 0a09 095b 6d2e 6164  p.vocab)...[m.ad
+00000880: 6428 6e61 6d65 2c20 7061 7473 2c20 2067  d(name, pats,  g
+00000890: 7265 6564 7920 3d27 4c4f 4e47 4553 5427  reedy ='LONGEST'
+000008a0: 2920 666f 7220 6e61 6d65 2c20 7061 7473  ) for name, pats
+000008b0: 2069 6e20 7275 6c65 732e 6974 656d 7328   in rules.items(
+000008c0: 295d 0a09 0973 6574 6174 7472 286d 6174  )]...setattr(mat
+000008d0: 6368 6572 2c20 6b65 792c 206d 290a 0972  cher, key, m)..r
+000008e0: 6574 7572 6e20 6765 7461 7474 7228 6d61  eturn getattr(ma
+000008f0: 7463 6865 722c 206b 6579 2920 0a0a 6465  tcher, key) ..de
+00000900: 6620 4465 704d 6174 6368 6572 2872 756c  f DepMatcher(rul
+00000910: 6573 3a64 6963 7420 3d20 7b22 7376 6f22  es:dict = {"svo"
+00000920: 3a5b 207b 2252 4947 4854 5f49 4422 3a20  :[ {"RIGHT_ID": 
+00000930: 2276 222c 2020 2252 4947 4854 5f41 5454  "v",  "RIGHT_ATT
+00000940: 5253 223a 207b 2250 4f53 223a 2022 5645  RS": {"POS": "VE
+00000950: 5242 227d 7d2c 207b 224c 4546 545f 4944  RB"}}, {"LEFT_ID
+00000960: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
+00000970: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
+00000980: 223a 2022 7375 626a 6563 7422 2c20 2252  ": "subject", "R
+00000990: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
+000009a0: 4550 223a 2022 6e73 7562 6a22 7d7d 2c7b  EP": "nsubj"}},{
+000009b0: 224c 4546 545f 4944 223a 2022 7622 2c20  "LEFT_ID": "v", 
+000009c0: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
+000009d0: 5249 4748 545f 4944 223a 2022 6f62 6a65  RIGHT_ID": "obje
+000009e0: 6374 222c 2252 4947 4854 5f41 5454 5253  ct","RIGHT_ATTRS
+000009f0: 223a 207b 2244 4550 223a 2022 646f 626a  ": {"DEP": "dobj
+00000a00: 227d 2020 7d5d 2c7d 2029 3a0a 0927 2727  "}  }],} ):..'''
+00000a10: 2020 5b28 7370 6163 792e 6e6c 702e 766f    [(spacy.nlp.vo
+00000a20: 6361 625b 6e61 6d65 5d2e 7465 7874 2c20  cab[name].text, 
+00000a30: 6172 2920 666f 7220 6e61 6d65 2c20 6172  ar) for name, ar
+00000a40: 2069 6e20 6d61 7463 6865 7228 646f 6329   in matcher(doc)
+00000a50: 5d20 2023 5b28 2773 766f 272c 205b 312c  ]  #[('svo', [1,
+00000a60: 2030 2c20 325d 295d 2727 270a 0966 726f   0, 2])]'''..fro
+00000a70: 6d20 7370 6163 792e 6d61 7463 6865 7220  m spacy.matcher 
+00000a80: 696d 706f 7274 2044 6570 656e 6465 6e63  import Dependenc
+00000a90: 794d 6174 6368 6572 0a09 6d61 7463 6865  yMatcher..matche
+00000aa0: 7220 3d20 4465 7065 6e64 656e 6379 4d61  r = DependencyMa
+00000ab0: 7463 6865 7228 7370 6163 792e 6e6c 702e  tcher(spacy.nlp.
+00000ac0: 766f 6361 6229 0a09 5b6d 6174 6368 6572  vocab)..[matcher
+00000ad0: 2e61 6464 286e 616d 652c 205b 7061 7474  .add(name, [patt
+00000ae0: 6572 6e5d 2920 666f 7220 6e61 6d65 2c20  ern]) for name, 
+00000af0: 7061 7474 6572 6e20 696e 2072 756c 6573  pattern in rules
+00000b00: 2e69 7465 6d73 2829 205d 0a09 7265 7475  .items() ]..retu
+00000b10: 726e 206d 6174 6368 6572 200a 0a0a 6465  rn matcher ...de
+00000b20: 6620 7068 7261 7365 5f6d 6174 6368 6572  f phrase_matcher
+00000b30: 2820 7275 6c65 7320 3d7b 2770 7027 3a5b  ( rules ={'pp':[
+00000b40: 5b7b 2750 4f53 273a 2027 4144 5027 7d2c  [{'POS': 'ADP'},
+00000b50: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
+00000b60: 2244 4554 222c 224e 554d 222c 2241 444a  "DET","NUM","ADJ
+00000b70: 222c 2750 554e 4354 272c 2743 4f4e 4a27  ",'PUNCT','CONJ'
+00000b80: 5d7d 2c20 224f 5022 3a20 222a 227d 2c7b  ]}, "OP": "*"},{
+00000b90: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
+00000ba0: 4e4f 554e 222c 2250 4152 5422 5d7d 2c20  NOUN","PART"]}, 
+00000bb0: 224f 5022 3a20 222b 227d 5d5d 207d 293a  "OP": "+"}]] }):
+00000bc0: 0a09 2727 2720 666f 7220 6e61 6d65 2c20  ..''' for name, 
+00000bd0: 6962 6567 2c69 656e 6420 696e 206d 6174  ibeg,iend in mat
+00000be0: 6368 6572 2864 6f63 2920 3a20 7072 696e  cher(doc) : prin
+00000bf0: 7428 7370 6163 792e 6e6c 702e 766f 6361  t(spacy.nlp.voca
+00000c00: 625b 6e61 6d65 5d2e 7465 7874 2c20 646f  b[name].text, do
+00000c10: 635b 6962 6567 3a69 656e 645d 2e74 6578  c[ibeg:iend].tex
+00000c20: 7429 2027 2727 0a09 6d61 7463 6865 7220  t) '''..matcher 
+00000c30: 3d20 4d61 7463 6865 7228 7370 6163 792e  = Matcher(spacy.
+00000c40: 6e6c 702e 766f 6361 6229 0a09 5b6d 6174  nlp.vocab)..[mat
+00000c50: 6368 6572 2e61 6464 286e 616d 652c 2070  cher.add(name, p
+00000c60: 6174 732c 2020 6772 6565 6479 203d 274c  ats,  greedy ='L
+00000c70: 4f4e 4745 5354 2729 2066 6f72 206e 616d  ONGEST') for nam
+00000c80: 652c 2070 6174 7320 696e 2072 756c 6573  e, pats in rules
+00000c90: 2e69 7465 6d73 2829 5d0a 0972 6574 7572  .items()]..retur
+00000ca0: 6e20 6d61 7463 6865 720a 0a0a 6465 6620  n matcher...def 
+00000cb0: 736e 7462 7228 6573 7361 792c 2074 7269  sntbr(essay, tri
+00000cc0: 6d3a 626f 6f6c 3d46 616c 7365 2c20 7769  m:bool=False, wi
+00000cd0: 7468 5f70 6964 3a62 6f6f 6c3d 4661 6c73  th_pid:bool=Fals
+00000ce0: 6529 3a20 0a09 2727 2720 6164 6465 6420  e): ..''' added 
+00000cf0: 3230 3232 2e35 2e32 3820 2727 270a 0966  2022.5.28 '''..f
+00000d00: 726f 6d20 7370 6163 792e 6c61 6e67 2069  rom spacy.lang i
+00000d10: 6d70 6f72 7420 656e 0a09 6966 206e 6f74  mport en..if not
+00000d20: 2068 6173 6174 7472 2873 6e74 6272 2c20   hasattr(sntbr, 
+00000d30: 2769 6e73 7427 293a 200a 0909 736e 7462  'inst'): ...sntb
+00000d40: 722e 696e 7374 203d 2065 6e2e 456e 676c  r.inst = en.Engl
+00000d50: 6973 6828 290a 0909 736e 7462 722e 696e  ish()...sntbr.in
+00000d60: 7374 2e61 6464 5f70 6970 6528 2273 656e  st.add_pipe("sen
+00000d70: 7465 6e63 697a 6572 2229 0a0a 0964 6f63  tencizer")...doc
+00000d80: 203d 2073 6e74 6272 2e69 6e73 7428 6573   = sntbr.inst(es
+00000d90: 7361 7929 0a09 6966 206e 6f74 2077 6974  say)..if not wit
+00000da0: 685f 7069 643a 2072 6574 7572 6e20 5b20  h_pid: return [ 
+00000db0: 736e 742e 7465 7874 2e73 7472 6970 2829  snt.text.strip()
+00000dc0: 2069 6620 7472 696d 2065 6c73 6520 736e   if trim else sn
+00000dd0: 742e 7465 7874 2066 6f72 2073 6e74 2069  t.text for snt i
+00000de0: 6e20 2064 6f63 2e73 656e 7473 5d0a 0a09  n  doc.sents]...
+00000df0: 7069 6420 3d20 3020 2373 7061 6379 2e73  pid = 0 #spacy.s
+00000e00: 6e74 7069 646f 6666 093d 206c 616d 6264  ntpidoff.= lambd
+00000e10: 6120 6573 7361 793a 2028 7069 643a 3d30  a essay: (pid:=0
+00000e20: 2c20 646f 633a 3d73 7061 6379 2e73 6e74  , doc:=spacy.snt
+00000e30: 6272 2865 7373 6179 292c 205b 2028 2070  br(essay), [ ( p
+00000e40: 6964 203a 3d20 7069 6420 2b20 3120 6966  id := pid + 1 if
+00000e50: 2022 5c6e 2220 696e 2073 6e74 2e74 6578   "\n" in snt.tex
+00000e60: 7420 656c 7365 2070 6964 2c20 2028 736e  t else pid,  (sn
+00000e70: 742e 7465 7874 2c20 7069 642c 2064 6f63  t.text, pid, doc
+00000e80: 5b73 6e74 2e73 7461 7274 5d2e 6964 7829  [snt.start].idx)
+00000e90: 295b 2d31 5d20 666f 7220 736e 7420 696e  )[-1] for snt in
+00000ea0: 2020 646f 632e 7365 6e74 735d 2029 5b2d    doc.sents] )[-
+00000eb0: 315d 0a09 6172 7220 3d20 5b5d 0a09 666f  1]..arr = []..fo
+00000ec0: 7220 736e 7420 696e 2020 646f 632e 7365  r snt in  doc.se
+00000ed0: 6e74 733a 0a09 0969 6620 225c 6e22 2069  nts:...if "\n" i
+00000ee0: 6e20 736e 742e 7465 7874 3a20 7069 6420  n snt.text: pid 
+00000ef0: 3d20 7069 6420 2b20 3120 0a09 0961 7272  = pid + 1 ...arr
+00000f00: 2e61 7070 656e 6428 2028 736e 742e 7465  .append( (snt.te
+00000f10: 7874 2c20 7069 6429 2029 200a 0972 6574  xt, pid) ) ..ret
+00000f20: 7572 6e20 6172 7220 0a0a 6465 6620 636f  urn arr ..def co
+00000f30: 6d6d 6f6e 5f70 6572 6328 736e 743d 2253  mmon_perc(snt="S
+00000f40: 6865 2068 6173 2072 6561 6479 2e22 2c20  he has ready.", 
+00000f50: 7472 616e 733d 2253 6865 2069 7320 7265  trans="She is re
+00000f60: 6164 792e 2229 3a20 0a09 746f 6b73 203d  ady."): ..toks =
+00000f70: 2073 6574 285b 742e 7465 7874 2066 6f72   set([t.text for
+00000f80: 2074 2069 6e20 7370 6163 792e 6e6c 702e   t in spacy.nlp.
+00000f90: 746f 6b65 6e69 7a65 7228 736e 7429 5d29  tokenizer(snt)])
+00000fa0: 0a09 7265 7475 726e 206c 656e 285b 7420  ..return len([t 
+00000fb0: 666f 7220 7420 696e 2073 7061 6379 2e6e  for t in spacy.n
+00000fc0: 6c70 2e74 6f6b 656e 697a 6572 2874 7261  lp.tokenizer(tra
+00000fd0: 6e73 2920 6966 2074 2e74 6578 7420 696e  ns) if t.text in
+00000fe0: 2074 6f6b 735d 2920 2f20 286c 656e 2874   toks]) / (len(t
+00000ff0: 6f6b 7329 2b30 2e30 3129 0a0a 6d65 7267  oks)+0.01)..merg
+00001000: 655f 6e70 7309 093d 2073 7061 6379 2e6e  e_nps..= spacy.n
+00001010: 6c70 2e63 7265 6174 655f 7069 7065 2822  lp.create_pipe("
+00001020: 6d65 7267 655f 6e6f 756e 5f63 6875 6e6b  merge_noun_chunk
+00001030: 7322 2920 236d 6572 6765 5f65 6e74 6974  s") #merge_entit
+00001040: 6965 730a 6d65 7267 655f 656e 7409 093d  ies.merge_ent..=
+00001050: 2073 7061 6379 2e6e 6c70 2e63 7265 6174   spacy.nlp.creat
+00001060: 655f 7069 7065 2822 6d65 7267 655f 656e  e_pipe("merge_en
+00001070: 7469 7469 6573 2229 200a 6e65 775f 6d61  tities") .new_ma
+00001080: 7463 6865 7209 093d 206c 616d 6264 6120  tcher..= lambda 
+00001090: 3a20 4d61 7463 6865 7228 7370 6163 792e  : Matcher(spacy.
+000010a0: 6e6c 702e 766f 6361 6229 2023 2062 7920  nlp.vocab) # by 
+000010b0: 6578 6368 756e 6b0a 746f 6b73 0909 093d  exchunk.toks...=
+000010c0: 206c 616d 6264 6120 646f 633a 2020 5b7b   lambda doc:  [{
+000010d0: 2769 273a 742e 692c 2022 6865 6164 223a  'i':t.i, "head":
+000010e0: 742e 6865 6164 2e69 2c20 276c 6578 273a  t.head.i, 'lex':
+000010f0: 742e 7465 7874 2c20 276c 656d 273a 742e  t.text, 'lem':t.
+00001100: 6c65 6d6d 615f 2c20 2770 6f73 273a 742e  lemma_, 'pos':t.
+00001110: 706f 735f 2c20 2774 6167 273a 742e 7461  pos_, 'tag':t.ta
+00001120: 675f 2c20 2764 6570 273a 742e 6465 705f  g_, 'dep':t.dep_
+00001130: 2c20 2267 706f 7322 3a74 2e68 6561 642e  , "gpos":t.head.
+00001140: 706f 735f 2c20 2267 6c65 6d22 3a74 2e68  pos_, "glem":t.h
+00001150: 6561 642e 6c65 6d6d 615f 7d20 666f 7220  ead.lemma_} for 
+00001160: 7420 696e 2064 6f63 205d 2023 204a 534f  t in doc ] # JSO
+00001170: 4e45 6163 6852 6f77 200a 706f 7374 6167  NEachRow .postag
+00001180: 0909 093d 206c 616d 6264 6120 646f 633a  ...= lambda doc:
+00001190: 2020 225f 5e20 2220 2b20 2220 222e 6a6f    "_^ " + " ".jo
+000011a0: 696e 285b 2066 227b 742e 7465 7874 7d5f  in([ f"{t.text}_
+000011b0: 7b74 2e6c 656d 6d61 5f7d 5f7b 742e 706f  {t.lemma_}_{t.po
+000011c0: 735f 7d5f 7b74 2e74 6167 5f7d 2220 666f  s_}_{t.tag_}" fo
+000011d0: 7220 7420 696e 2064 6f63 5d29 202b 2022  r t in doc]) + "
+000011e0: 205f 2422 0a6e 6f6e 5f72 6f6f 745f 7665   _$".non_root_ve
+000011f0: 7262 7309 3d20 6c61 6d62 6461 2064 6f63  rbs.= lambda doc
+00001200: 3a20 205b 7420 666f 7220 7420 696e 2064  :  [t for t in d
+00001210: 6f63 2069 6620 742e 706f 735f 203d 3d20  oc if t.pos_ == 
+00001220: 2756 4552 4227 2061 6e64 2074 2e64 6570  'VERB' and t.dep
+00001230: 5f20 213d 2027 524f 4f54 275d 200a 7369  _ != 'ROOT'] .si
+00001240: 6d70 6c65 5f73 656e 7409 093d 206c 616d  mple_sent..= lam
+00001250: 6264 6120 646f 633a 2020 6c65 6e28 5b74  bda doc:  len([t
+00001260: 2066 6f72 2074 2069 6e20 646f 6320 6966   for t in doc if
+00001270: 2074 2e70 6f73 5f20 3d3d 2027 5645 5242   t.pos_ == 'VERB
+00001280: 2720 616e 6420 742e 6465 705f 2021 3d20  ' and t.dep_ != 
+00001290: 2752 4f4f 5427 5d29 203c 3d20 3020 2320  'ROOT']) <= 0 # 
+000012a0: 656c 7365 2069 7320 636f 6d70 6c65 7820  else is complex 
+000012b0: 7365 6e74 200a 636f 6d70 6f75 6e64 5f73  sent .compound_s
+000012c0: 6e74 093d 206c 616d 6264 6120 646f 633a  nt.= lambda doc:
+000012d0: 2020 6c65 6e28 5b74 2066 6f72 2074 2069    len([t for t i
+000012e0: 6e20 646f 6320 6966 2074 2e64 6570 5f20  n doc if t.dep_ 
+000012f0: 3d3d 2027 636f 6e6a 2720 616e 6420 742e  == 'conj' and t.
+00001300: 6865 6164 2e64 6570 5f20 3d3d 2027 524f  head.dep_ == 'RO
+00001310: 4f54 275d 2920 3e20 300a 736e 745f 736f  OT']) > 0.snt_so
+00001320: 7572 6365 0909 3d20 6c61 6d62 6461 2073  urce..= lambda s
+00001330: 6964 2c20 646f 633a 207b 2774 7970 6527  id, doc: {'type'
+00001340: 3a27 736e 7427 2c20 2773 7263 273a 2073  :'snt', 'src': s
+00001350: 6964 2c20 2773 6e74 273a 646f 632e 7465  id, 'snt':doc.te
+00001360: 7874 2c20 2770 7265 645f 6f66 6673 6574  xt, 'pred_offset
+00001370: 273a 2070 7265 645f 6f66 6673 6574 2864  ': pred_offset(d
+00001380: 6f63 292c 2009 2770 6f73 7461 6727 3a27  oc), .'postag':'
+00001390: 5f5e 2027 202b 2027 2027 2e6a 6f69 6e28  _^ ' + ' '.join(
+000013a0: 5b66 227b 742e 7465 7874 7d5f 7b74 2e6c  [f"{t.text}_{t.l
+000013b0: 656d 6d61 5f7d 5f7b 742e 706f 735f 7d5f  emma_}_{t.pos_}_
+000013c0: 7b74 2e74 6167 5f7d 2220 6966 2074 2e74  {t.tag_}" if t.t
+000013d0: 6578 7420 3d3d 2074 2e74 6578 742e 6c6f  ext == t.text.lo
+000013e0: 7765 7228 2920 656c 7365 2066 227b 742e  wer() else f"{t.
+000013f0: 7465 7874 7d5f 7b74 2e74 6578 742e 6c6f  text}_{t.text.lo
+00001400: 7765 7228 297d 5f7b 742e 6c65 6d6d 615f  wer()}_{t.lemma_
+00001410: 7d5f 7b74 2e70 6f73 5f7d 5f7b 742e 7461  }_{t.pos_}_{t.ta
+00001420: 675f 7d22 2066 6f72 2074 2069 6e20 646f  g_}" for t in do
+00001430: 635d 2920 2b20 2720 5f24 272c 2020 2774  c]) + ' _$',  't
+00001440: 6327 3a20 6c65 6e28 646f 6329 7d0a 7072  c': len(doc)}.pr
+00001450: 6564 5f6f 6666 7365 7409 093d 206c 616d  ed_offset..= lam
+00001460: 6264 6120 646f 633a 2028 2061 7220 3a3d  bda doc: ( ar :=
+00001470: 205b 2074 2e69 2066 6f72 2074 2069 6e20   [ t.i for t in 
+00001480: 646f 6320 6966 2074 2e64 6570 5f20 3d3d  doc if t.dep_ ==
+00001490: 2022 524f 4f54 225d 2c20 6f66 6673 6574   "ROOT"], offset
+000014a0: 203a 3d20 6172 5b30 5d20 6966 206c 656e   := ar[0] if len
+000014b0: 2861 7229 203e 2030 2065 6c73 6520 302c  (ar) > 0 else 0,
+000014c0: 206f 6666 7365 742f 2820 6c65 6e28 646f   offset/( len(do
+000014d0: 6329 202b 2030 2e31 2920 295b 2d31 5d0a  c) + 0.1) )[-1].
+000014e0: 6861 735f 7a68 0909 093d 206c 616d 6264  has_zh...= lambd
+000014f0: 6120 7320 3a20 616e 7928 5b63 2066 6f72  a s : any([c for
+00001500: 2063 2069 6e20 7320 6966 206f 7264 2863   c in s if ord(c
+00001510: 2920 3e20 3235 355d 290a 0a64 6566 2073  ) > 255])..def s
+00001520: 686f 7728 646f 6329 3a0a 0927 2727 2075  how(doc):..''' u
+00001530: 7365 6420 696e 2074 6865 206e 6f74 6562  sed in the noteb
+00001540: 6f6f 6b2c 2066 6f72 2064 6562 7567 2027  ook, for debug '
+00001550: 2727 0a09 696d 706f 7274 2070 616e 6461  ''..import panda
+00001560: 7320 6173 2070 640a 0972 6574 7572 6e20  s as pd..return 
+00001570: 7064 2e44 6174 6146 7261 6d65 287b 2777  pd.DataFrame({'w
+00001580: 6f72 6427 3a20 5b74 2e74 6578 7420 666f  ord': [t.text fo
+00001590: 7220 7420 696e 2064 6f63 5d2c 2027 7461  r t in doc], 'ta
+000015a0: 6727 3a20 5b74 2e74 6167 5f20 666f 7220  g': [t.tag_ for 
+000015b0: 7420 696e 2064 6f63 5d2c 2770 6f73 273a  t in doc],'pos':
+000015c0: 205b 742e 706f 735f 2066 6f72 2074 2069   [t.pos_ for t i
+000015d0: 6e20 646f 635d 2c27 6865 6164 273a 205b  n doc],'head': [
+000015e0: 742e 6865 6164 2e6f 7274 685f 2066 6f72  t.head.orth_ for
+000015f0: 2074 2069 6e20 646f 635d 2c27 6465 7027   t in doc],'dep'
+00001600: 3a20 5b74 2e64 6570 5f20 666f 7220 7420  : [t.dep_ for t 
+00001610: 696e 2064 6f63 5d2c 2027 6c65 6d6d 6127  in doc], 'lemma'
+00001620: 3a20 5b74 2e74 6578 742e 6c6f 7765 7228  : [t.text.lower(
+00001630: 2920 6966 2074 2e6c 656d 6d61 5f20 3d3d  ) if t.lemma_ ==
+00001640: 2027 2d50 524f 4e2d 2720 656c 7365 2074   '-PRON-' else t
+00001650: 2e6c 656d 6d61 5f20 666f 7220 7420 696e  .lemma_ for t in
+00001660: 2064 6f63 5d2c 0a09 276e 5f6c 6566 7473   doc],..'n_lefts
+00001670: 273a 205b 2074 2e6e 5f6c 6566 7473 2066  ': [ t.n_lefts f
+00001680: 6f72 2074 2069 6e20 646f 635d 2c20 276c  or t in doc], 'l
+00001690: 6566 745f 6564 6765 273a 205b 2074 2e6c  eft_edge': [ t.l
+000016a0: 6566 745f 6564 6765 2e74 6578 7420 666f  eft_edge.text fo
+000016b0: 7220 7420 696e 2064 6f63 5d2c 200a 0927  r t in doc], ..'
+000016c0: 6e5f 7269 6768 7473 273a 205b 2074 2e6e  n_rights': [ t.n
+000016d0: 5f72 6967 6874 7320 666f 7220 7420 696e  _rights for t in
+000016e0: 2064 6f63 5d2c 2027 7269 6768 745f 6564   doc], 'right_ed
+000016f0: 6765 273a 205b 2074 2e72 6967 6874 5f65  ge': [ t.right_e
+00001700: 6467 652e 7465 7874 2066 6f72 2074 2069  dge.text for t i
+00001710: 6e20 646f 635d 2c0a 0927 7375 6274 7265  n doc],..'subtre
+00001720: 6527 3a20 5b20 6c69 7374 2874 2e73 7562  e': [ list(t.sub
+00001730: 7472 6565 2920 666f 7220 7420 696e 2064  tree) for t in d
+00001740: 6f63 5d2c 2027 6368 696c 6472 656e 273a  oc], 'children':
+00001750: 205b 206c 6973 7428 742e 6368 696c 6472   [ list(t.childr
+00001760: 656e 2920 666f 7220 7420 696e 2064 6f63  en) for t in doc
+00001770: 5d2c 2009 2327 6d6f 7270 6827 3a20 5b20  ], .#'morph': [ 
+00001780: 742e 6d6f 7270 6820 666f 7220 7420 696e  t.morph for t in
+00001790: 2064 6f63 5d2c 0a09 2765 6e74 5f74 7970   doc],..'ent_typ
+000017a0: 6527 3a20 5b20 742e 656e 745f 7479 7065  e': [ t.ent_type
+000017b0: 5f20 666f 7220 7420 696e 2064 6f63 5d2c  _ for t in doc],
+000017c0: 2027 656e 745f 6964 273a 205b 2074 2e65   'ent_id': [ t.e
+000017d0: 6e74 5f69 645f 2066 6f72 2074 2069 6e20  nt_id_ for t in 
+000017e0: 646f 635d 2c0a 097d 290a 0a64 6566 2070  doc],..})..def p
+000017f0: 6172 7365 2873 6e74 2c20 6d65 7267 655f  arse(snt, merge_
+00001800: 6e70 3d20 4661 6c73 6529 3a0a 0927 2727  np= False):..'''
+00001810: 2075 7365 6420 696e 2074 6865 206e 6f74   used in the not
+00001820: 6562 6f6f 6b2c 2066 6f72 2064 6562 7567  ebook, for debug
+00001830: 2027 2727 0a09 646f 6320 3d20 7370 6163   '''..doc = spac
+00001840: 792e 6e6c 7028 736e 7429 0a09 6966 206d  y.nlp(snt)..if m
+00001850: 6572 6765 5f6e 7020 3a20 7370 6163 792e  erge_np : spacy.
+00001860: 6d65 7267 655f 6e70 7328 646f 6329 0a09  merge_nps(doc)..
+00001870: 7265 7475 726e 2073 686f 7728 646f 6329  return show(doc)
+00001880: 0a0a 7472 705f 7265 6c09 093d 206c 616d  ..trp_rel..= lam
+00001890: 6264 6120 743a 2020 6622 7b74 2e64 6570  bda t:  f"{t.dep
+000018a0: 5f7d 5f7b 742e 6865 6164 2e70 6f73 5f7d  _}_{t.head.pos_}
+000018b0: 5f7b 742e 706f 735f 7d22 2020 2320 646f  _{t.pos_}"  # do
+000018c0: 626a 5f56 4552 425f 4e4f 554e 0a74 7270  bj_VERB_NOUN.trp
+000018d0: 5f72 6576 6572 7365 203d 2073 6574 287b  _reverse = set({
+000018e0: 2261 6d6f 645f 4e4f 554e 5f41 444a 222c  "amod_NOUN_ADJ",
+000018f0: 226e 7375 626a 5f56 4552 425f 4e4f 554e  "nsubj_VERB_NOUN
+00001900: 227d 290a 7472 705f 746f 6b09 093d 206c  "}).trp_tok..= l
+00001910: 616d 6264 6120 646f 632c 2061 7272 3a20  ambda doc, arr: 
+00001920: 205b 2074 2066 6f72 2074 2069 6e20 646f   [ t for t in do
+00001930: 6320 6966 205b 2074 2e64 6570 5f2c 2074  c if [ t.dep_, t
+00001940: 2e68 6561 642e 706f 735f 2c20 742e 706f  .head.pos_, t.po
+00001950: 735f 2c20 742e 6865 6164 2e6c 656d 6d61  s_, t.head.lemma
+00001960: 5f2c 2074 2e6c 656d 6d61 5f20 5d20 3d3d  _, t.lemma_ ] ==
+00001970: 2061 7272 205d 2023 2061 7272 2069 7320   arr ] # arr is 
+00001980: 6578 6163 746c 7920 3520 6c69 7374 200a  exactly 5 list .
+00001990: 676f 765f 6465 7009 093d 206c 616d 6264  gov_dep..= lambd
+000019a0: 6120 7265 6c2c 2061 7272 203a 2028 6172  a rel, arr : (ar
+000019b0: 725b 305d 2c20 6172 725b 315d 2920 6966  r[0], arr[1]) if
+000019c0: 206c 656d 6d61 5f6f 7264 6572 2e67 6574   lemma_order.get
+000019d0: 2872 656c 2c20 5472 7565 2920 656c 7365  (rel, True) else
+000019e0: 2028 6172 725b 315d 2c20 6172 725b 305d   (arr[1], arr[0]
+000019f0: 2920 2023 206f 7065 6e20 646f 6f72 0a68  )  # open door.h
+00001a00: 6974 5f74 7270 0909 3d20 6c61 6d62 6461  it_trp..= lambda
+00001a10: 2074 2c20 5f72 656c 2c20 5f67 6f76 5f64   t, _rel, _gov_d
+00001a20: 6570 3a20 2020 5f72 656c 203d 3d20 7472  ep:   _rel == tr
+00001a30: 705f 7265 6c28 7429 2061 6e64 205f 676f  p_rel(t) and _go
+00001a40: 765f 6465 7020 3d3d 2028 742e 6865 6164  v_dep == (t.head
+00001a50: 2e6c 656d 6d61 5f2c 2074 2e6c 656d 6d61  .lemma_, t.lemma
+00001a60: 5f29 0a74 7270 5f68 6967 6809 3d20 6c61  _).trp_high.= la
+00001a70: 6d62 6461 2064 6f63 2c20 692c 2069 6865  mbda doc, i, ihe
+00001a80: 6164 203a 2020 2022 222e 6a6f 696e 285b  ad :   "".join([
+00001a90: 2066 223c 623e 7b74 2e74 6578 745f 7769   f"<b>{t.text_wi
+00001aa0: 7468 5f77 737d 3c2f 623e 2220 6966 2074  th_ws}</b>" if t
+00001ab0: 2e69 2069 6e20 2869 2c20 6968 6561 6429  .i in (i, ihead)
+00001ac0: 2065 6c73 6520 742e 7465 7874 5f77 6974   else t.text_wit
+00001ad0: 685f 7773 2066 6f72 2074 2069 6e20 646f  h_ws for t in do
+00001ae0: 6320 5d29 0a6c 656d 5f68 6967 6809 3d20  c ]).lem_high.= 
+00001af0: 6c61 6d62 6461 2064 6f63 2c20 6c65 6d20  lambda doc, lem 
+00001b00: 3a20 2020 2222 2e6a 6f69 6e28 5b20 6622  :   "".join([ f"
+00001b10: 3c62 3e7b 742e 7465 7874 5f77 6974 685f  <b>{t.text_with_
+00001b20: 7773 7d3c 2f62 3e22 2069 6620 742e 6c65  ws}</b>" if t.le
+00001b30: 6d6d 615f 203d 3d20 6c65 6d20 656c 7365  mma_ == lem else
+00001b40: 2074 2e74 6578 745f 7769 7468 5f77 7320   t.text_with_ws 
+00001b50: 666f 7220 7420 696e 2064 6f63 205d 2920  for t in doc ]) 
+00001b60: 2320 6869 6768 6c69 6768 7420 7468 6520  # highlight the 
+00001b70: 6669 7273 7420 6c65 6d6d 6120 0a76 705f  first lemma .vp_
+00001b80: 7370 616e 0909 3d20 6c61 6d62 6461 2064  span..= lambda d
+00001b90: 6f63 2c69 6265 672c 6965 6e64 3a20 646f  oc,ibeg,iend: do
+00001ba0: 635b 6962 6567 5d2e 6c65 6d6d 615f 202b  c[ibeg].lemma_ +
+00001bb0: 2022 2022 202b 2064 6f63 5b69 6265 672b   " " + doc[ibeg+
+00001bc0: 313a 6965 6e64 5d2e 7465 7874 2e6c 6f77  1:iend].text.low
+00001bd0: 6572 2829 0a0a 6465 6620 6879 6228 646f  er()..def hyb(do
+00001be0: 632c 2073 7461 7274 2c20 7061 7429 3a20  c, start, pat): 
+00001bf0: 236c 3a6c 656d 6d61 2078 3a74 6578 742c  #l:lemma x:text,
+00001c00: 2070 3a70 6f73 2074 3a74 6167 202c 2065   p:pos t:tag , e
+00001c10: 3a65 6e74 5f74 7970 6520 0a09 6172 7220  :ent_type ..arr 
+00001c20: 3d20 5b5d 0a09 666f 7220 692c 6320 696e  = []..for i,c in
+00001c30: 2065 6e75 6d65 7261 7465 2870 6174 293a   enumerate(pat):
+00001c40: 200a 0909 6966 2063 203d 3d20 276c 273a   ...if c == 'l':
+00001c50: 0961 7272 2e61 7070 656e 6428 646f 635b  .arr.append(doc[
+00001c60: 7374 6172 7420 2b69 5d2e 6c65 6d6d 615f  start +i].lemma_
+00001c70: 290a 0909 656c 6966 2063 203d 3d20 2770  )...elif c == 'p
+00001c80: 273a 0961 7272 2e61 7070 656e 6428 646f  ':.arr.append(do
+00001c90: 635b 7374 6172 7420 2b69 5d2e 706f 735f  c[start +i].pos_
+00001ca0: 290a 0909 656c 6966 2063 203d 3d20 2774  )...elif c == 't
+00001cb0: 273a 0961 7272 2e61 7070 656e 6428 646f  ':.arr.append(do
+00001cc0: 635b 7374 6172 7420 2b69 5d2e 7461 675f  c[start +i].tag_
+00001cd0: 290a 0909 656c 6966 2063 203d 3d20 2765  )...elif c == 'e
+00001ce0: 273a 0961 7272 2e61 7070 656e 6428 646f  ':.arr.append(do
+00001cf0: 635b 7374 6172 7420 2b69 5d2e 656e 745f  c[start +i].ent_
+00001d00: 7479 7065 5f29 0a09 0965 6c69 6620 6320  type_)...elif c 
+00001d10: 3d3d 2027 7827 3a09 6172 722e 6170 7065  == 'x':.arr.appe
+00001d20: 6e64 2864 6f63 5b73 7461 7274 202b 695d  nd(doc[start +i]
+00001d30: 2e74 6578 742e 6c6f 7765 7228 2929 0a09  .text.lower())..
+00001d40: 0965 6c73 6520 3a09 0909 6172 722e 6170  .else :...arr.ap
+00001d50: 7065 6e64 2864 6f63 5b73 7461 7274 202b  pend(doc[start +
+00001d60: 695d 2e74 6578 742e 6c6f 7765 7228 2929  i].text.lower())
+00001d70: 0a09 7265 7475 726e 2027 2027 2e6a 6f69  ..return ' '.joi
+00001d80: 6e28 6172 7229 200a 0a64 6566 206b 705f  n(arr) ..def kp_
+00001d90: 7370 616e 2864 6f63 2c20 7374 6172 742c  span(doc, start,
+00001da0: 2065 6e64 2c20 6e61 6d65 293a 2020 2320   end, name):  # 
+00001db0: 6261 7365 3a56 4552 423a 6265 5f76 626e  base:VERB:be_vbn
+00001dc0: 5f70 3a62 6520 6261 7365 6420 6f6e 2020  _p:be based on  
+00001dd0: 207c 206c 656d 2c20 706f 732c 2074 7970   | lem, pos, typ
+00001de0: 652c 2063 6875 6e6b 200a 0969 6620 6e61  e, chunk ..if na
+00001df0: 6d65 2e73 7461 7274 7377 6974 6828 2776  me.startswith('v
+00001e00: 2729 3a09 0972 6574 7572 6e20 2864 6f63  '):..return (doc
+00001e10: 5b73 7461 7274 5d2e 6c65 6d6d 615f 2c64  [start].lemma_,d
+00001e20: 6f63 5b73 7461 7274 5d2e 706f 735f 2c20  oc[start].pos_, 
+00001e30: 6e61 6d65 2c76 705f 7370 616e 2864 6f63  name,vp_span(doc
+00001e40: 2c73 7461 7274 2c65 6e64 2920 290a 0965  ,start,end) )..e
+00001e50: 6c69 6620 6e61 6d65 2e73 7461 7274 7377  lif name.startsw
+00001e60: 6974 6828 2262 655f 2229 203a 0972 6574  ith("be_") :.ret
+00001e70: 7572 6e20 2864 6f63 5b73 7461 7274 2b31  urn (doc[start+1
+00001e80: 5d2e 6c65 6d6d 615f 2c64 6f63 5b73 7461  ].lemma_,doc[sta
+00001e90: 7274 2b31 5d2e 706f 735f 2c6e 616d 652c  rt+1].pos_,name,
+00001ea0: 7670 5f73 7061 6e28 646f 632c 7374 6172  vp_span(doc,star
+00001eb0: 742c 656e 6429 290a 0965 6c69 6620 6e61  t,end))..elif na
+00001ec0: 6d65 2069 6e20 2827 6170 272c 2770 7027  me in ('ap','pp'
+00001ed0: 2c27 5665 6e64 2729 3a72 6574 7572 6e20  ,'Vend'):return 
+00001ee0: 2864 6f63 5b65 6e64 2d31 5d2e 6c65 6d6d  (doc[end-1].lemm
+00001ef0: 615f 2c64 6f63 5b65 6e64 2d31 5d2e 706f  a_,doc[end-1].po
+00001f00: 735f 2c6e 616d 652c 646f 635b 7374 6172  s_,name,doc[star
+00001f10: 743a 656e 645d 2e74 6578 742e 6c6f 7765  t:end].text.lowe
+00001f20: 7228 2929 0a09 656c 7365 3a09 0909 0909  r())..else:.....
+00001f30: 0909 7265 7475 726e 2028 646f 635b 7374  ..return (doc[st
+00001f40: 6172 745d 2e6c 656d 6d61 5f2c 646f 635b  art].lemma_,doc[
+00001f50: 7374 6172 745d 2e70 6f73 5f2c 6e61 6d65  start].pos_,name
+00001f60: 2c64 6f63 5b73 7461 7274 3a65 6e64 5d2e  ,doc[start:end].
+00001f70: 7465 7874 2e6c 6f77 6572 2829 290a 0a6b  text.lower())..k
+00001f80: 705f 7275 6c65 7320 3d20 7b0a 2256 656e  p_rules = {."Ven
+00001f90: 6422 3a5b 5b7b 2250 4f53 223a 207b 2249  d":[[{"POS": {"I
+00001fa0: 4e22 3a20 5b22 4155 5822 2c22 5645 5242  N": ["AUX","VERB
+00001fb0: 225d 7d7d 2c7b 2250 4f53 223a 207b 2249  "]}},{"POS": {"I
+00001fc0: 4e22 3a20 5b22 4144 5622 5d7d 2c20 224f  N": ["ADV"]}, "O
+00001fd0: 5022 3a20 222a 227d 2c20 7b22 504f 5322  P": "*"}, {"POS"
+00001fe0: 3a20 7b22 494e 223a 205b 2241 444a 222c  : {"IN": ["ADJ",
+00001ff0: 2256 4552 4222 5d7d 2c20 224f 5022 3a20  "VERB"]}, "OP": 
+00002000: 222a 227d 2c7b 2250 4f53 223a 207b 2249  "*"},{"POS": {"I
+00002010: 4e22 3a20 5b22 5041 5254 222c 2241 4450  N": ["PART","ADP
+00002020: 222c 2254 4f22 5d7d 2c20 224f 5022 3a20  ","TO"]}, "OP": 
+00002030: 222a 227d 2c7b 2250 4f53 223a 2027 5645  "*"},{"POS": 'VE
+00002040: 5242 277d 5d5d 2c20 2320 636f 756c 6420  RB'}]], # could 
+00002050: 6861 7264 6c79 2077 6169 7420 746f 206d  hardly wait to m
+00002060: 6565 740a 2276 7022 3a20 205b 5b7b 2750  eet."vp":  [[{'P
+00002070: 4f53 273a 2027 5645 5242 277d 2c7b 2250  OS': 'VERB'},{"P
+00002080: 4f53 223a 207b 2249 4e22 3a20 5b22 4445  OS": {"IN": ["DE
+00002090: 5422 2c22 4144 5022 2c22 4144 4a22 5d7d  T","ADP","ADJ"]}
+000020a0: 2c20 224f 5022 3a20 222a 227d 2c7b 2250  , "OP": "*"},{"P
+000020b0: 4f53 223a 2027 4e4f 554e 277d 2c20 7b22  OS": 'NOUN'}, {"
+000020c0: 504f 5322 3a20 7b22 494e 223a 205b 2241  POS": {"IN": ["A
+000020d0: 4450 222c 2254 4f22 5d7d 2c20 224f 5022  DP","TO"]}, "OP"
+000020e0: 3a20 222a 227d 5d2c 205b 7b27 504f 5327  : "*"}], [{'POS'
+000020f0: 3a20 2756 4552 4227 7d2c 7b22 504f 5322  : 'VERB'},{"POS"
+00002100: 3a20 7b22 494e 223a 205b 2244 4554 222c  : {"IN": ["DET",
+00002110: 2241 4450 222c 2241 444a 222c 2254 4f22  "ADP","ADJ","TO"
+00002120: 2c22 5041 5254 225d 7d2c 2022 4f50 223a  ,"PART"]}, "OP":
+00002130: 2022 2a22 7d2c 7b22 504f 5322 3a20 2756   "*"},{"POS": 'V
+00002140: 4552 4227 7d5d 5d2c 2023 2077 6169 7420  ERB'}]], # wait 
+00002150: 746f 206d 6565 740a 2270 7022 3a20 205b  to meet."pp":  [
+00002160: 5b7b 2750 4f53 273a 2027 4144 5027 7d2c  [{'POS': 'ADP'},
+00002170: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
+00002180: 2244 4554 222c 224e 554d 222c 2241 444a  "DET","NUM","ADJ
+00002190: 222c 2750 554e 4354 272c 2743 4f4e 4a27  ",'PUNCT','CONJ'
+000021a0: 5d7d 2c20 224f 5022 3a20 222a 227d 2c7b  ]}, "OP": "*"},{
+000021b0: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
+000021c0: 4e4f 554e 222c 2250 4152 5422 5d7d 2c20  NOUN","PART"]}, 
+000021d0: 224f 5022 3a20 222b 227d 5d5d 2c20 2020  "OP": "+"}]],   
+000021e0: 200a 2261 7022 3a20 205b 5b7b 2250 4f53   ."ap":  [[{"POS
+000021f0: 223a 207b 2249 4e22 3a20 5b22 4144 5622  ": {"IN": ["ADV"
+00002200: 5d7d 2c20 224f 5022 3a20 222b 227d 2c20  ]}, "OP": "+"}, 
+00002210: 7b22 504f 5322 3a20 2741 444a 277d 5d5d  {"POS": 'ADJ'}]]
+00002220: 2c20 200a 2276 7072 7422 3a09 5b5b 7b22  ,  ."vprt":.[[{"
+00002230: 504f 5322 3a20 2756 4552 4227 2c20 2254  POS": 'VERB', "T
+00002240: 4147 223a 207b 224e 4f54 5f49 4e22 3a20  AG": {"NOT_IN": 
+00002250: 5b22 5642 4e22 5d7d 7d2c 207b 2250 4f53  ["VBN"]}}, {"POS
+00002260: 223a 207b 2249 4e22 3a20 5b22 5052 4550  ": {"IN": ["PREP
+00002270: 222c 2022 4144 5022 2c27 544f 275d 7d2c  ", "ADP",'TO']},
+00002280: 2022 4f50 223a 2022 2b22 7d5d 5d2c 2020   "OP": "+"}]],  
+00002290: 2023 206c 6f6f 6b20 7570 202f 6c6f 6f6b   # look up /look
+000022a0: 2075 7020 6672 6f6d 2c20 2063 6f6d 7075   up from,  compu
+000022b0: 7465 6420 7477 6963 650a 2276 746f 7622  ted twice."vtov"
+000022c0: 3a09 5b5b 7b22 504f 5322 3a20 2756 4552  :.[[{"POS": 'VER
+000022d0: 4227 2c20 2254 4147 223a 207b 224e 4f54  B', "TAG": {"NOT
+000022e0: 5f49 4e22 3a20 5b22 5642 4e22 5d7d 7d2c  _IN": ["VBN"]}},
+000022f0: 207b 2254 4147 223a 2027 544f 277d 2c7b   {"TAG": 'TO'},{
+00002300: 2254 4147 223a 2027 5642 277d 5d5d 2c20  "TAG": 'VB'}]], 
+00002310: 2020 2320 706c 616e 2074 6f20 676f 0a22    # plan to go."
+00002320: 7676 6267 223a 095b 5b7b 2250 4f53 223a  vvbg":.[[{"POS":
+00002330: 2027 5645 5242 272c 2022 5441 4722 3a20   'VERB', "TAG": 
+00002340: 7b22 4e4f 545f 494e 223a 205b 2256 424e  {"NOT_IN": ["VBN
+00002350: 225d 7d7d 2c20 7b22 5441 4722 3a20 2756  "]}}, {"TAG": 'V
+00002360: 4247 277d 5d5d 2c20 2020 2320 636f 6e73  BG'}]],   # cons
+00002370: 6964 6572 2067 6f69 6e67 0a22 7670 6722  ider going."vpg"
+00002380: 3a09 5b5b 7b22 504f 5322 3a20 2756 4552  :.[[{"POS": 'VER
+00002390: 4227 2c20 2254 4147 223a 207b 224e 4f54  B', "TAG": {"NOT
+000023a0: 5f49 4e22 3a20 5b22 5642 4e22 5d7d 7d2c  _IN": ["VBN"]}},
+000023b0: 207b 2250 4f53 223a 207b 2249 4e22 3a20   {"POS": {"IN": 
+000023c0: 5b22 5052 4550 222c 2022 4144 5022 2c27  ["PREP", "ADP",'
+000023d0: 5041 5254 275d 7d2c 2022 4f50 223a 2022  PART']}, "OP": "
+000023e0: 2b22 7d2c 7b22 5441 4722 3a20 2756 4247  +"},{"TAG": 'VBG
+000023f0: 277d 5d5d 2c20 2020 2320 696e 7369 7374  '}]],   # insist
+00002400: 6564 206f 6e20 676f 696e 670a 2262 655f  ed on going."be_
+00002410: 7662 6e5f 7022 3a20 5b5b 7b27 4c45 4d4d  vbn_p": [[{'LEMM
+00002420: 4127 3a20 2762 6527 7d2c 7b22 5441 4722  A': 'be'},{"TAG"
+00002430: 3a20 7b22 494e 223a 205b 2256 424e 225d  : {"IN": ["VBN"]
+00002440: 7d7d 2c20 7b22 504f 5322 3a20 7b22 494e  }}, {"POS": {"IN
+00002450: 223a 205b 2250 5245 5022 2c20 2241 4450  ": ["PREP", "ADP
+00002460: 222c 2750 4152 5427 5d7d 7d5d 5d2c 2020  ",'PART']}}]],  
+00002470: 2023 2062 6173 653a 5645 5242 3a62 655f   # base:VERB:be_
+00002480: 7662 6e5f 703a 6265 2062 6173 6564 206f  vbn_p:be based o
+00002490: 6e20 2020 0a22 6265 5f61 646a 5f70 223a  n   ."be_adj_p":
+000024a0: 205b 5b7b 274c 454d 4d41 273a 2027 6265   [[{'LEMMA': 'be
+000024b0: 277d 2c7b 2250 4f53 223a 207b 2249 4e22  '},{"POS": {"IN"
+000024c0: 3a20 5b22 4144 4a22 5d7d 7d2c 207b 2250  : ["ADJ"]}}, {"P
+000024d0: 4f53 223a 207b 2249 4e22 3a20 5b22 5052  OS": {"IN": ["PR
+000024e0: 4550 222c 2022 4144 5022 2c27 5041 5254  EP", "ADP",'PART
+000024f0: 275d 7d7d 5d5d 2c20 2020 2320 6265 2061  ']}}]],   # be a
+00002500: 6e67 7279 2077 6974 680a 7d20 2366 6f72  ngry with.} #for
+00002510: 206e 616d 652c 2069 6265 672c 6965 6e64   name, ibeg,iend
+00002520: 2069 6e20 6d61 7463 6865 7228 646f 6329   in matcher(doc)
+00002530: 203a 2070 7269 6e74 2873 7061 6379 2e6e   : print(spacy.n
+00002540: 6c70 2e76 6f63 6162 5b6e 616d 655d 2e74  lp.vocab[name].t
+00002550: 6578 742c 2064 6f63 5b69 6265 673a 6965  ext, doc[ibeg:ie
+00002560: 6e64 5d2e 7465 7874 290a 0a64 6566 206b  nd].text)..def k
+00002570: 705f 6d61 7463 6865 7228 646f 6329 3a20  p_matcher(doc): 
+00002580: 235b 2827 7665 6e64 272c 2027 636f 6e73  #[('vend', 'cons
+00002590: 6964 6572 2067 6f69 6e67 272c 2031 2c20  ider going', 1, 
+000025a0: 3329 2c20 2827 7670 272c 2027 636f 6e73  3), ('vp', 'cons
+000025b0: 6964 6572 2067 6f69 6e67 272c 2031 2c20  ider going', 1, 
+000025c0: 3329 2c20 2827 7676 6267 272c 2027 636f  3), ('vvbg', 'co
+000025d0: 6e73 6964 6572 2067 6f69 6e67 272c 2031  nsider going', 1
+000025e0: 2c20 3329 2c20 2827 7670 7274 272c 2027  , 3), ('vprt', '
+000025f0: 676f 696e 6720 746f 272c 2032 2c20 3429  going to', 2, 4)
+00002600: 5d0a 0969 6620 6e6f 7420 6861 7361 7474  ]..if not hasatt
+00002610: 7228 6b70 5f6d 6174 6368 6572 2c20 276d  r(kp_matcher, 'm
+00002620: 6174 6368 6572 2729 3a20 0a09 096b 705f  atcher'): ...kp_
+00002630: 6d61 7463 6865 722e 6d61 7463 6865 7220  matcher.matcher 
+00002640: 3d20 4d61 7463 6865 7228 7370 6163 792e  = Matcher(spacy.
+00002650: 6e6c 702e 766f 6361 6229 0a09 095b 6b70  nlp.vocab)...[kp
+00002660: 5f6d 6174 6368 6572 2e6d 6174 6368 6572  _matcher.matcher
+00002670: 2e61 6464 286e 616d 652c 2070 6174 7465  .add(name, patte
+00002680: 726e 732c 2020 6772 6565 6479 203d 274c  rns,  greedy ='L
+00002690: 4f4e 4745 5354 2729 2066 6f72 206e 616d  ONGEST') for nam
+000026a0: 652c 2070 6174 7465 726e 7320 696e 206b  e, patterns in k
+000026b0: 705f 7275 6c65 732e 6974 656d 7328 2920  p_rules.items() 
+000026c0: 5d0a 0974 7570 7320 3d20 7365 7428 2920  ]..tups = set() 
+000026d0: 2023 2072 656d 6f76 6520 7468 6520 6475   # remove the du
+000026e0: 706c 6963 6174 6564 2065 6e74 7269 6573  plicated entries
+000026f0: 200a 095b 7475 7073 2e61 6464 2820 6b70   ..[tups.add( kp
+00002700: 5f73 7061 6e28 646f 632c 6962 6567 2c69  _span(doc,ibeg,i
+00002710: 656e 642c 2073 7061 6379 2e6e 6c70 2e76  end, spacy.nlp.v
+00002720: 6f63 6162 5b6e 616d 655d 2e74 6578 7429  ocab[name].text)
+00002730: 2029 2066 6f72 206e 616d 652c 2069 6265   ) for name, ibe
+00002740: 672c 6965 6e64 2069 6e20 6b70 5f6d 6174  g,iend in kp_mat
+00002750: 6368 6572 2e6d 6174 6368 6572 2864 6f63  cher.matcher(doc
+00002760: 295d 200a 0972 6574 7572 6e20 7475 7073  )] ..return tups
+00002770: 0a0a 6465 6620 7275 6c65 7228 736e 742c  ..def ruler(snt,
+00002780: 206e 616d 653a 7374 723d 2773 6d27 293a   name:str='sm'):
+00002790: 0a09 2727 2720 646f 632e 7370 616e 735b  ..''' doc.spans[
+000027a0: 2772 756c 6572 275d 2032 3032 332e 312e  'ruler'] 2023.1.
+000027b0: 3231 2027 2727 0a09 6966 206e 6f74 2068  21 '''..if not h
+000027c0: 6173 6174 7472 2872 756c 6572 2c20 6e61  asattr(ruler, na
+000027d0: 6d65 293a 2020 0a09 095f 6e6c 7020 3d20  me):  ..._nlp = 
+000027e0: 7370 6163 792e 6c6f 6164 2866 2765 6e5f  spacy.load(f'en_
+000027f0: 636f 7265 5f77 6562 5f7b 6e61 6d65 7d27  core_web_{name}'
+00002800: 290a 0909 7365 7461 7474 7228 7275 6c65  )...setattr(rule
+00002810: 722c 206e 616d 652c 205f 6e6c 7020 290a  r, name, _nlp ).
+00002820: 0909 5f72 756c 6572 203d 205f 6e6c 702e  .._ruler = _nlp.
+00002830: 6164 645f 7069 7065 2822 7370 616e 5f72  add_pipe("span_r
+00002840: 756c 6572 2229 0a09 0970 6174 7465 726e  uler")...pattern
+00002850: 7320 3d20 5b7b 226c 6162 656c 223a 2022  s = [{"label": "
+00002860: 5050 222c 2022 7061 7474 6572 6e22 3a20  PP", "pattern": 
+00002870: 5b7b 2750 4f53 273a 2027 4144 5027 7d2c  [{'POS': 'ADP'},
+00002880: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
+00002890: 2244 4554 222c 224e 554d 222c 2241 444a  "DET","NUM","ADJ
+000028a0: 222c 2750 554e 4354 272c 2743 4f4e 4a27  ",'PUNCT','CONJ'
+000028b0: 5d7d 2c20 224f 5022 3a20 222a 227d 2c7b  ]}, "OP": "*"},{
+000028c0: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
+000028d0: 4e4f 554e 222c 2250 4152 5422 2c22 5052  NOUN","PART","PR
+000028e0: 4f50 4e22 5d7d 2c20 224f 5022 3a20 222b  OPN"]}, "OP": "+
+000028f0: 227d 5d7d 2c0a 2020 2020 2020 2020 2020  "}]},.          
+00002900: 2020 7b22 6c61 6265 6c22 3a20 2256 5022    {"label": "VP"
+00002910: 2c20 2270 6174 7465 726e 223a 205b 7b27  , "pattern": [{'
+00002920: 504f 5327 3a20 2756 4552 4227 7d2c 7b22  POS': 'VERB'},{"
+00002930: 504f 5322 3a20 7b22 494e 223a 205b 2244  POS": {"IN": ["D
+00002940: 4554 222c 2241 4450 222c 2241 444a 225d  ET","ADP","ADJ"]
+00002950: 7d2c 2022 4f50 223a 2022 2a22 7d2c 7b22  }, "OP": "*"},{"
+00002960: 504f 5322 3a20 274e 4f55 4e27 7d2c 207b  POS": 'NOUN'}, {
+00002970: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
+00002980: 4144 5022 2c22 544f 225d 7d2c 2022 4f50  ADP","TO"]}, "OP
+00002990: 223a 2022 2a22 7d5d 7d2c 0a09 0909 7b22  ": "*"}]},....{"
+000029a0: 6c61 6265 6c22 3a20 2256 656e 6422 2c20  label": "Vend", 
+000029b0: 2270 6174 7465 726e 223a 205b 7b22 504f  "pattern": [{"PO
+000029c0: 5322 3a20 7b22 494e 223a 205b 2241 5558  S": {"IN": ["AUX
+000029d0: 222c 2256 4552 4222 5d7d 7d2c 7b22 504f  ","VERB"]}},{"PO
+000029e0: 5322 3a20 7b22 494e 223a 205b 2241 4456  S": {"IN": ["ADV
+000029f0: 225d 7d2c 2022 4f50 223a 2022 2a22 7d2c  "]}, "OP": "*"},
+00002a00: 207b 2250 4f53 223a 207b 2249 4e22 3a20   {"POS": {"IN": 
+00002a10: 5b22 4144 4a22 2c22 5645 5242 225d 7d2c  ["ADJ","VERB"]},
+00002a20: 2022 4f50 223a 2022 2a22 7d2c 7b22 504f   "OP": "*"},{"PO
+00002a30: 5322 3a20 7b22 494e 223a 205b 2250 4152  S": {"IN": ["PAR
+00002a40: 5422 2c22 4144 5022 2c22 544f 225d 7d2c  T","ADP","TO"]},
+00002a50: 2022 4f50 223a 2022 2a22 7d2c 7b22 504f   "OP": "*"},{"PO
+00002a60: 5322 3a20 2756 4552 4227 7d5d 7d2c 0a09  S": 'VERB'}]},..
+00002a70: 0909 7b22 6c61 6265 6c22 3a20 2241 5022  ..{"label": "AP"
+00002a80: 2c20 2270 6174 7465 726e 223a 205b 7b22  , "pattern": [{"
+00002a90: 504f 5322 3a20 7b22 494e 223a 205b 2241  POS": {"IN": ["A
+00002aa0: 4456 225d 7d2c 2022 4f50 223a 2022 2b22  DV"]}, "OP": "+"
+00002ab0: 7d2c 207b 2250 4f53 223a 2027 4144 4a27  }, {"POS": 'ADJ'
+00002ac0: 7d5d 7d2c 0a09 0909 7b22 6c61 6265 6c22  }]},....{"label"
+00002ad0: 3a20 2276 746f 7622 2c20 2270 6174 7465  : "vtov", "patte
+00002ae0: 726e 223a 205b 7b22 504f 5322 3a20 2756  rn": [{"POS": 'V
+00002af0: 4552 4227 2c20 2254 4147 223a 207b 224e  ERB', "TAG": {"N
+00002b00: 4f54 5f49 4e22 3a20 5b22 5642 4e22 5d7d  OT_IN": ["VBN"]}
+00002b10: 7d2c 207b 2254 4147 223a 2027 544f 277d  }, {"TAG": 'TO'}
+00002b20: 2c7b 2254 4147 223a 2027 5642 277d 5d7d  ,{"TAG": 'VB'}]}
+00002b30: 2c0a 0909 097b 226c 6162 656c 223a 2022  ,....{"label": "
+00002b40: 7676 6267 222c 2022 7061 7474 6572 6e22  vvbg", "pattern"
+00002b50: 3a20 5b7b 2250 4f53 223a 2027 5645 5242  : [{"POS": 'VERB
+00002b60: 272c 2022 5441 4722 3a20 7b22 4e4f 545f  ', "TAG": {"NOT_
+00002b70: 494e 223a 205b 2256 424e 225d 7d7d 2c20  IN": ["VBN"]}}, 
+00002b80: 7b22 5441 4722 3a20 2756 4247 277d 5d7d  {"TAG": 'VBG'}]}
+00002b90: 2c0a 0909 097b 226c 6162 656c 223a 2022  ,....{"label": "
+00002ba0: 7670 7274 222c 2022 7061 7474 6572 6e22  vprt", "pattern"
+00002bb0: 3a20 5b7b 2250 4f53 223a 2027 5645 5242  : [{"POS": 'VERB
+00002bc0: 272c 2022 5441 4722 3a20 7b22 4e4f 545f  ', "TAG": {"NOT_
+00002bd0: 494e 223a 205b 2256 424e 225d 7d7d 2c20  IN": ["VBN"]}}, 
+00002be0: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
+00002bf0: 2250 5245 5022 2c20 2241 4450 222c 2754  "PREP", "ADP",'T
+00002c00: 4f27 5d7d 2c20 224f 5022 3a20 222b 227d  O']}, "OP": "+"}
+00002c10: 5d7d 2c0a 0909 097b 226c 6162 656c 223a  ]},....{"label":
+00002c20: 2022 7670 6722 2c20 2270 6174 7465 726e   "vpg", "pattern
+00002c30: 223a 205b 7b22 504f 5322 3a20 2756 4552  ": [{"POS": 'VER
+00002c40: 4227 2c20 2254 4147 223a 207b 224e 4f54  B', "TAG": {"NOT
+00002c50: 5f49 4e22 3a20 5b22 5642 4e22 5d7d 7d2c  _IN": ["VBN"]}},
+00002c60: 207b 2250 4f53 223a 207b 2249 4e22 3a20   {"POS": {"IN": 
+00002c70: 5b22 5052 4550 222c 2022 4144 5022 2c27  ["PREP", "ADP",'
+00002c80: 5041 5254 275d 7d2c 2022 4f50 223a 2022  PART']}, "OP": "
+00002c90: 2b22 7d2c 7b22 5441 4722 3a20 2756 4247  +"},{"TAG": 'VBG
+00002ca0: 277d 5d7d 2c23 2069 6e73 6973 7465 6420  '}]},# insisted 
+00002cb0: 6f6e 2067 6f69 6e67 0a09 0909 7b22 6c61  on going....{"la
+00002cc0: 6265 6c22 3a20 2262 655f 7662 6e5f 7022  bel": "be_vbn_p"
+00002cd0: 2c20 2270 6174 7465 726e 223a 205b 7b27  , "pattern": [{'
+00002ce0: 4c45 4d4d 4127 3a20 2762 6527 7d2c 7b22  LEMMA': 'be'},{"
+00002cf0: 5441 4722 3a20 7b22 494e 223a 205b 2256  TAG": {"IN": ["V
+00002d00: 424e 225d 7d7d 2c20 7b22 504f 5322 3a20  BN"]}}, {"POS": 
+00002d10: 7b22 494e 223a 205b 2250 5245 5022 2c20  {"IN": ["PREP", 
+00002d20: 2241 4450 222c 2750 4152 5427 5d7d 7d5d  "ADP",'PART']}}]
+00002d30: 7d2c 2320 6261 7365 3a56 4552 423a 6265  },# base:VERB:be
+00002d40: 5f76 626e 5f70 3a62 6520 6261 7365 6420  _vbn_p:be based 
+00002d50: 6f6e 2020 200a 0909 097b 226c 6162 656c  on   ....{"label
+00002d60: 223a 2022 6265 5f61 646a 5f70 222c 2022  ": "be_adj_p", "
+00002d70: 7061 7474 6572 6e22 3a20 5b7b 274c 454d  pattern": [{'LEM
+00002d80: 4d41 273a 2027 6265 277d 2c7b 2250 4f53  MA': 'be'},{"POS
+00002d90: 223a 207b 2249 4e22 3a20 5b22 4144 4a22  ": {"IN": ["ADJ"
+00002da0: 5d7d 7d2c 207b 2250 4f53 223a 207b 2249  ]}}, {"POS": {"I
+00002db0: 4e22 3a20 5b22 5052 4550 222c 2022 4144  N": ["PREP", "AD
+00002dc0: 5022 2c27 5041 5254 275d 7d7d 5d7d 2c23  P",'PART']}}]},#
+00002dd0: 2062 6520 616e 6772 7920 7769 7468 0a09   be angry with..
+00002de0: 0909 5d0a 0909 5f72 756c 6572 2e61 6464  ..]..._ruler.add
+00002df0: 5f70 6174 7465 726e 7328 7061 7474 6572  _patterns(patter
+00002e00: 6e73 290a 0972 6574 7572 6e20 6765 7461  ns)..return geta
+00002e10: 7474 7228 7275 6c65 722c 206e 616d 6529  ttr(ruler, name)
+00002e20: 2873 6e74 2920 2023 7072 696e 7428 5b28  (snt)  #print([(
+00002e30: 7370 616e 2e74 6578 742c 2073 7061 6e2e  span.text, span.
+00002e40: 6c61 6265 6c5f 2920 666f 7220 7370 616e  label_) for span
+00002e50: 2069 6e20 2064 6f63 2e73 7061 6e73 5b22   in  doc.spans["
+00002e60: 7275 6c65 7222 5d20 5d29 0a0a 2320 6164  ruler"] ])..# ad
+00002e70: 6465 6420 3230 3232 2e37 2e32 350a 706f  ded 2022.7.25.po
+00002e80: 7374 5f6e 705f 7275 6c65 7320 3d20 7b20  st_np_rules = { 
+00002e90: 2320 6166 7465 7220 6e70 2069 7320 6d65  # after np is me
+00002ea0: 7267 6564 200a 2276 5f6e 5f76 626e 223a  rged ."v_n_vbn":
+00002eb0: 205b 5b7b 2250 4f53 223a 2027 5645 5242   [[{"POS": 'VERB
+00002ec0: 272c 2022 5441 4722 3a20 7b22 4e4f 545f  ', "TAG": {"NOT_
+00002ed0: 494e 223a 205b 2256 424e 225d 7d7d 2c7b  IN": ["VBN"]}},{
+00002ee0: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
+00002ef0: 4e4f 554e 225d 7d7d 2c20 7b22 5441 4722  NOUN"]}}, {"TAG"
+00002f00: 3a20 7b22 494e 223a 205b 2256 424e 225d  : {"IN": ["VBN"]
+00002f10: 7d7d 5d5d 2c20 2020 2320 6c65 6176 6520  }}]],   # leave 
+00002f20: 7468 6520 626f 6f6b 206f 7065 6e65 6420  the book opened 
+00002f30: 0a22 765f 6e5f 6164 6a22 3a20 5b5b 7b22  ."v_n_adj": [[{"
+00002f40: 504f 5322 3a20 2756 4552 4227 2c20 2254  POS": 'VERB', "T
+00002f50: 4147 223a 207b 224e 4f54 5f49 4e22 3a20  AG": {"NOT_IN": 
+00002f60: 5b22 5642 4e22 5d7d 7d2c 7b22 504f 5322  ["VBN"]}},{"POS"
+00002f70: 3a20 7b22 494e 223a 205b 224e 4f55 4e22  : {"IN": ["NOUN"
+00002f80: 5d7d 7d2c 207b 2250 4f53 223a 207b 2249  ]}}, {"POS": {"I
+00002f90: 4e22 3a20 5b22 4144 4a22 5d7d 7d5d 5d2c  N": ["ADJ"]}}]],
+00002fa0: 0a7d 2023 666f 7220 6e61 6d65 2c20 6962  .} #for name, ib
+00002fb0: 6567 2c69 656e 6420 696e 206d 6174 6368  eg,iend in match
+00002fc0: 6572 2864 6f63 2920 3a20 7072 696e 7428  er(doc) : print(
+00002fd0: 7370 6163 792e 6e6c 702e 766f 6361 625b  spacy.nlp.vocab[
+00002fe0: 6e61 6d65 5d2e 7465 7874 2c20 646f 635b  name].text, doc[
+00002ff0: 6962 6567 3a69 656e 645d 2e74 6578 7429  ibeg:iend].text)
+00003000: 0a64 6566 2070 6f73 745f 6e70 5f6d 6174  .def post_np_mat
+00003010: 6368 6572 2864 6f63 293a 200a 0969 6620  cher(doc): ..if 
+00003020: 6e6f 7420 6861 7361 7474 7228 706f 7374  not hasattr(post
+00003030: 5f6e 705f 6d61 7463 6865 722c 2027 6d61  _np_matcher, 'ma
+00003040: 7463 6865 7227 293a 200a 0909 706f 7374  tcher'): ...post
+00003050: 5f6e 705f 6d61 7463 6865 722e 6d61 7463  _np_matcher.matc
+00003060: 6865 7220 3d20 4d61 7463 6865 7228 7370  her = Matcher(sp
+00003070: 6163 792e 6e6c 702e 766f 6361 6229 0a09  acy.nlp.vocab)..
+00003080: 095b 706f 7374 5f6e 705f 6d61 7463 6865  .[post_np_matche
+00003090: 722e 6d61 7463 6865 722e 6164 6428 6e61  r.matcher.add(na
+000030a0: 6d65 2c20 7061 7474 6572 6e73 2c20 2067  me, patterns,  g
+000030b0: 7265 6564 7920 3d27 4c4f 4e47 4553 5427  reedy ='LONGEST'
+000030c0: 2920 666f 7220 6e61 6d65 2c20 7061 7474  ) for name, patt
+000030d0: 6572 6e73 2069 6e20 706f 7374 5f6e 705f  erns in post_np_
+000030e0: 7275 6c65 732e 6974 656d 7328 2920 5d0a  rules.items() ].
+000030f0: 0972 6574 7572 6e20 5b28 7370 6163 792e  .return [(spacy.
+00003100: 6e6c 702e 766f 6361 625b 6e61 6d65 5d2e  nlp.vocab[name].
+00003110: 7465 7874 2c69 6265 672c 6965 6e64 2920  text,ibeg,iend) 
+00003120: 666f 7220 6e61 6d65 2c20 6962 6567 2c69  for name, ibeg,i
+00003130: 656e 6420 696e 2070 6f73 745f 6e70 5f6d  end in post_np_m
+00003140: 6174 6368 6572 2e6d 6174 6368 6572 2864  atcher.matcher(d
+00003150: 6f63 295d 200a 0a64 6566 206e 6577 5f6d  oc)] ..def new_m
+00003160: 6174 6368 6572 2870 6174 7465 726e 732c  atcher(patterns,
+00003170: 206e 616d 653d 2770 6174 2729 3a0a 096d   name='pat'):..m
+00003180: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
+00003190: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
+000031a0: 290a 096d 6174 6368 6572 2e61 6464 286e  )..matcher.add(n
+000031b0: 616d 652c 2070 6174 7465 726e 732c 2067  ame, patterns, g
+000031c0: 7265 6564 7920 3d27 4c4f 4e47 4553 5427  reedy ='LONGEST'
+000031d0: 290a 0972 6574 7572 6e20 6d61 7463 6865  )..return matche
+000031e0: 720a 6d61 7463 6865 7273 203d 207b 2020  r.matchers = {  
+000031f0: 2320 666f 7220 6e61 6d65 2c73 7461 7274  # for name,start
+00003200: 2c65 6e64 2069 6e20 6d61 7463 6865 7273  ,end in matchers
+00003210: 5b27 6170 275d 2864 6f63 2920 3a0a 2276  ['ap'](doc) :."v
+00003220: 656e 6422 3a6e 6577 5f6d 6174 6368 6572  end":new_matcher
+00003230: 285b 5b7b 2250 4f53 223a 207b 2249 4e22  ([[{"POS": {"IN"
+00003240: 3a20 5b22 4155 5822 2c22 5645 5242 225d  : ["AUX","VERB"]
+00003250: 7d7d 2c7b 2250 4f53 223a 207b 2249 4e22  }},{"POS": {"IN"
+00003260: 3a20 5b22 4144 5622 5d7d 2c20 224f 5022  : ["ADV"]}, "OP"
+00003270: 3a20 222a 227d 2c20 7b22 504f 5322 3a20  : "*"}, {"POS": 
+00003280: 7b22 494e 223a 205b 2241 444a 222c 2256  {"IN": ["ADJ","V
+00003290: 4552 4222 5d7d 2c20 224f 5022 3a20 222a  ERB"]}, "OP": "*
+000032a0: 227d 2c7b 2250 4f53 223a 207b 2249 4e22  "},{"POS": {"IN"
+000032b0: 3a20 5b22 5041 5254 222c 2241 4450 222c  : ["PART","ADP",
+000032c0: 2254 4f22 5d7d 2c20 224f 5022 3a20 222a  "TO"]}, "OP": "*
+000032d0: 227d 2c7b 2250 4f53 223a 2027 5645 5242  "},{"POS": 'VERB
+000032e0: 277d 5d5d 292c 2023 2063 6f75 6c64 2068  '}]]), # could h
+000032f0: 6172 646c 7920 7761 6974 2074 6f20 6d65  ardly wait to me
+00003300: 6574 0a22 7670 223a 2020 6e65 775f 6d61  et."vp":  new_ma
+00003310: 7463 6865 7228 5b5b 7b27 504f 5327 3a20  tcher([[{'POS': 
+00003320: 2756 4552 4227 7d2c 7b22 504f 5322 3a20  'VERB'},{"POS": 
+00003330: 7b22 494e 223a 205b 2244 4554 222c 2241  {"IN": ["DET","A
+00003340: 4450 222c 2241 444a 225d 7d2c 2022 4f50  DP","ADJ"]}, "OP
+00003350: 223a 2022 2a22 7d2c 7b22 504f 5322 3a20  ": "*"},{"POS": 
+00003360: 274e 4f55 4e27 7d2c 207b 2250 4f53 223a  'NOUN'}, {"POS":
+00003370: 207b 2249 4e22 3a20 5b22 4144 5022 2c22   {"IN": ["ADP","
+00003380: 544f 225d 7d2c 2022 4f50 223a 2022 2a22  TO"]}, "OP": "*"
+00003390: 7d5d 2c20 2348 6520 7061 6964 2061 2063  }], #He paid a c
+000033a0: 6c6f 7365 2061 7474 656e 7469 6f6e 2074  lose attention t
+000033b0: 6f20 7468 6520 626f 6f6b 2e20 7c48 6520  o the book. |He 
+000033c0: 6c6f 6f6b 6564 2075 7020 6672 6f6d 2074  looked up from t
+000033d0: 6865 2073 6964 652e 207c 206d 616b 6520  he side. | make 
+000033e0: 7573 6520 6f66 0a20 2020 2020 2020 2020  use of.         
+000033f0: 2020 2020 2020 2020 2020 2020 5b7b 2750              [{'P
+00003400: 4f53 273a 2027 5645 5242 277d 2c7b 2250  OS': 'VERB'},{"P
+00003410: 4f53 223a 207b 2249 4e22 3a20 5b22 4445  OS": {"IN": ["DE
+00003420: 5422 2c22 4144 5022 2c22 4144 4a22 2c22  T","ADP","ADJ","
+00003430: 544f 222c 2250 4152 5422 5d7d 2c20 224f  TO","PART"]}, "O
+00003440: 5022 3a20 222a 227d 2c7b 2250 4f53 223a  P": "*"},{"POS":
+00003450: 2027 5645 5242 277d 5d5d 292c 2023 2077   'VERB'}]]), # w
+00003460: 6169 7420 746f 206d 6565 740a 2270 7022  ait to meet."pp"
+00003470: 3a20 206e 6577 5f6d 6174 6368 6572 285b  :  new_matcher([
+00003480: 5b7b 2750 4f53 273a 2027 4144 5027 7d2c  [{'POS': 'ADP'},
+00003490: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
+000034a0: 2244 4554 222c 224e 554d 222c 2241 444a  "DET","NUM","ADJ
+000034b0: 222c 2750 554e 4354 272c 2743 4f4e 4a27  ",'PUNCT','CONJ'
+000034c0: 5d7d 2c20 224f 5022 3a20 222a 227d 2c7b  ]}, "OP": "*"},{
+000034d0: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
+000034e0: 4e4f 554e 222c 2250 4152 5422 5d7d 2c20  NOUN","PART"]}, 
+000034f0: 224f 5022 3a20 222b 227d 5d5d 292c 2020  "OP": "+"}]]),  
+00003500: 2020 0a22 6170 223a 2020 6e65 775f 6d61    ."ap":  new_ma
+00003510: 7463 6865 7228 5b5b 7b22 504f 5322 3a20  tcher([[{"POS": 
+00003520: 7b22 494e 223a 205b 2241 4456 225d 7d2c  {"IN": ["ADV"]},
+00003530: 2022 4f50 223a 2022 2a22 7d2c 207b 2250   "OP": "*"}, {"P
+00003540: 4f53 223a 2027 4144 4a27 7d5d 5d29 2c20  OS": 'ADJ'}]]), 
+00003550: 200a 2276 7072 7422 3a20 6e65 775f 6d61   ."vprt": new_ma
+00003560: 7463 6865 7228 5b5b 7b22 504f 5322 3a20  tcher([[{"POS": 
+00003570: 2756 4552 4227 2c20 2254 4147 223a 207b  'VERB', "TAG": {
+00003580: 224e 4f54 5f49 4e22 3a20 5b22 5642 4e22  "NOT_IN": ["VBN"
+00003590: 5d7d 7d2c 207b 2250 4f53 223a 207b 2249  ]}}, {"POS": {"I
+000035a0: 4e22 3a20 5b22 5052 4550 222c 2022 4144  N": ["PREP", "AD
+000035b0: 5022 2c27 544f 275d 7d2c 2022 4f50 223a  P",'TO']}, "OP":
+000035c0: 2022 2b22 7d5d 5d29 2c20 2020 2320 6c6f   "+"}]]),   # lo
+000035d0: 6f6b 2075 7020 2f6c 6f6f 6b20 7570 2066  ok up /look up f
+000035e0: 726f 6d2c 2020 636f 6d70 7574 6564 2074  rom,  computed t
+000035f0: 7769 6365 0a22 7674 6f76 223a 206e 6577  wice."vtov": new
+00003600: 5f6d 6174 6368 6572 285b 5b7b 2250 4f53  _matcher([[{"POS
+00003610: 223a 2027 5645 5242 272c 2022 5441 4722  ": 'VERB', "TAG"
+00003620: 3a20 7b22 4e4f 545f 494e 223a 205b 2256  : {"NOT_IN": ["V
+00003630: 424e 225d 7d7d 2c20 7b22 5441 4722 3a20  BN"]}}, {"TAG": 
+00003640: 2754 4f27 7d2c 7b22 5441 4722 3a20 2756  'TO'},{"TAG": 'V
+00003650: 4227 7d5d 5d29 2c20 2020 2320 706c 616e  B'}]]),   # plan
+00003660: 2074 6f20 676f 0a22 7676 6267 223a 206e   to go."vvbg": n
+00003670: 6577 5f6d 6174 6368 6572 285b 5b7b 2250  ew_matcher([[{"P
+00003680: 4f53 223a 2027 5645 5242 272c 2022 5441  OS": 'VERB', "TA
+00003690: 4722 3a20 7b22 4e4f 545f 494e 223a 205b  G": {"NOT_IN": [
+000036a0: 2256 424e 225d 7d7d 2c20 7b22 5441 4722  "VBN"]}}, {"TAG"
+000036b0: 3a20 2756 4247 277d 5d5d 292c 2020 2023  : 'VBG'}]]),   #
+000036c0: 2063 6f6e 7369 6465 7220 676f 696e 670a   consider going.
+000036d0: 2276 7067 223a 2020 6e65 775f 6d61 7463  "vpg":  new_matc
+000036e0: 6865 7228 5b5b 7b22 504f 5322 3a20 2756  her([[{"POS": 'V
+000036f0: 4552 4227 2c20 2254 4147 223a 207b 224e  ERB', "TAG": {"N
+00003700: 4f54 5f49 4e22 3a20 5b22 5642 4e22 5d7d  OT_IN": ["VBN"]}
+00003710: 7d2c 207b 2250 4f53 223a 207b 2249 4e22  }, {"POS": {"IN"
+00003720: 3a20 5b22 5052 4550 222c 2022 4144 5022  : ["PREP", "ADP"
+00003730: 2c27 5041 5254 275d 7d2c 2022 4f50 223a  ,'PART']}, "OP":
+00003740: 2022 2b22 7d2c 7b22 5441 4722 3a20 2756   "+"},{"TAG": 'V
+00003750: 4247 277d 5d5d 292c 2020 2023 2069 6e73  BG'}]]),   # ins
+00003760: 6973 7465 6420 6f6e 2067 6f69 6e67 0a22  isted on going."
+00003770: 7641 7022 3a20 206e 6577 5f6d 6174 6368  vAp":  new_match
+00003780: 6572 285b 5b7b 274c 454d 4d41 273a 2027  er([[{'LEMMA': '
+00003790: 6265 277d 2c7b 2254 4147 223a 207b 2249  be'},{"TAG": {"I
+000037a0: 4e22 3a20 5b22 5642 4e22 5d7d 7d2c 207b  N": ["VBN"]}}, {
+000037b0: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
+000037c0: 5052 4550 222c 2022 4144 5022 2c27 5041  PREP", "ADP",'PA
+000037d0: 5254 275d 7d7d 5d5d 292c 2020 2023 2062  RT']}}]]),   # b
+000037e0: 6520 6261 7365 6420 6f6e 2020 200a 2276  e based on   ."v
+000037f0: 6170 223a 2020 6e65 775f 6d61 7463 6865  ap":  new_matche
+00003800: 7228 5b5b 7b27 4c45 4d4d 4127 3a20 2762  r([[{'LEMMA': 'b
+00003810: 6527 7d2c 7b22 504f 5322 3a20 7b22 494e  e'},{"POS": {"IN
+00003820: 223a 205b 2241 444a 225d 7d7d 2c20 7b22  ": ["ADJ"]}}, {"
+00003830: 504f 5322 3a20 7b22 494e 223a 205b 2250  POS": {"IN": ["P
+00003840: 5245 5022 2c20 2241 4450 222c 2750 4152  REP", "ADP",'PAR
+00003850: 5427 5d7d 7d5d 5d29 2c20 2020 2320 6265  T']}}]]),   # be
+00003860: 2061 6e67 7279 2077 6974 680a 7d20 2366   angry with.} #f
+00003870: 6f72 206e 616d 652c 2069 6265 672c 6965  or name, ibeg,ie
+00003880: 6e64 2069 6e20 6d61 7463 6865 7228 646f  nd in matcher(do
+00003890: 6329 203a 2070 7269 6e74 2873 7061 6379  c) : print(spacy
+000038a0: 2e6e 6c70 2e76 6f63 6162 5b6e 616d 655d  .nlp.vocab[name]
+000038b0: 2e74 6578 742c 2064 6f63 5b69 6265 673a  .text, doc[ibeg:
+000038c0: 6965 6e64 5d2e 7465 7874 290a 0a23 230a  iend].text)..##.
+000038d0: 2323 2066 726f 6d20 7665 7262 6e65 742e  ## from verbnet.
+000038e0: 7079 0a23 230a 404c 616e 6775 6167 652e  py.##.@Language.
+000038f0: 636f 6d70 6f6e 656e 7428 226d 6572 6765  component("merge
+00003900: 5f6e 7022 290a 6465 6620 6d65 7267 655f  _np").def merge_
+00003910: 6e70 2864 6f63 293a 0a09 7769 7468 2064  np(doc):..with d
+00003920: 6f63 2e72 6574 6f6b 656e 697a 6528 2920  oc.retokenize() 
+00003930: 6173 2072 6574 6f6b 656e 697a 6572 3a0a  as retokenizer:.
+00003940: 0909 666f 7220 6e70 2069 6e20 646f 632e  ..for np in doc.
+00003950: 6e6f 756e 5f63 6875 6e6b 733a 0a09 0909  noun_chunks:....
+00003960: 6174 7472 7320 3d20 7b22 7461 6722 3a20  attrs = {"tag": 
+00003970: 6e70 2e72 6f6f 742e 7461 672c 2022 6465  np.root.tag, "de
+00003980: 7022 3a20 6e70 2e72 6f6f 742e 6465 702c  p": np.root.dep,
+00003990: 2022 656e 745f 7479 7065 223a 2022 4e50   "ent_type": "NP
+000039a0: 222c 2022 6c65 6d6d 6122 3a64 6f63 5b6e  ", "lemma":doc[n
+000039b0: 702e 656e 642d 315d 2e6c 656d 6d61 7d20  p.end-1].lemma} 
+000039c0: 2320 2c20 226c 656d 6d61 223a 646f 635b  # , "lemma":doc[
+000039d0: 6e70 2e65 6e64 2d31 5d2e 6c65 6d6d 6120  np.end-1].lemma 
+000039e0: 7c20 6164 6465 6420 3230 3232 2e37 2e32  | added 2022.7.2
+000039f0: 360a 0909 0972 6574 6f6b 656e 697a 6572  6....retokenizer
+00003a00: 2e6d 6572 6765 286e 702c 2061 7474 7273  .merge(np, attrs
+00003a10: 3d61 7474 7273 2920 0a09 7265 7475 726e  =attrs) ..return
+00003a20: 2064 6f63 0a0a 6465 6620 736b 656e 7028   doc..def skenp(
+00003a30: 646f 632c 2074 6167 3d22 5f4e 5022 293a  doc, tag="_NP"):
+00003a40: 2023 2061 6464 6564 2032 3032 322e 332e   # added 2022.3.
+00003a50: 3232 2c20 666f 7220 736b 6576 6563 0a09  22, for skevec..
+00003a60: 6d65 7267 655f 6e70 2864 6f63 2920 2320  merge_np(doc) # 
+00003a70: 7472 616e 7366 6f72 6d20 646f 6320 2c20  transform doc , 
+00003a80: 6669 6e61 6c6c 7920 746f 2062 6520 6361  finally to be ca
+00003a90: 6c6c 6564 200a 0972 6574 7572 6e20 2220  lled ..return " 
+00003aa0: 222e 6a6f 696e 285b 7461 6720 6966 2074  ".join([tag if t
+00003ab0: 2e65 6e74 5f74 7970 655f 203d 3d20 274e  .ent_type_ == 'N
+00003ac0: 5027 2065 6c73 6520 742e 7465 7874 2066  P' else t.text f
+00003ad0: 6f72 2074 2069 6e20 646f 635d 290a 0a64  or t in doc])..d
+00003ae0: 6566 206d 6572 6765 5f6e 5f6f 665f 6e28  ef merge_n_of_n(
+00003af0: 646f 6329 3a0a 0969 6620 6e6f 7420 6861  doc):..if not ha
+00003b00: 7361 7474 7228 6d65 7267 655f 6e5f 6f66  sattr(merge_n_of
+00003b10: 5f6e 2c20 276d 6174 6368 6572 2729 3a0a  _n, 'matcher'):.
+00003b20: 0909 6d65 7267 655f 6e5f 6f66 5f6e 2e6d  ..merge_n_of_n.m
+00003b30: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
+00003b40: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
+00003b50: 290a 0909 6d65 7267 655f 6e5f 6f66 5f6e  )...merge_n_of_n
+00003b60: 2e6d 6174 6368 6572 2e61 6464 2822 6e2d  .matcher.add("n-
+00003b70: 6f66 2d6e 222c 205b 5b7b 2245 4e54 5f54  of-n", [[{"ENT_T
+00003b80: 5950 4522 3a20 224e 5022 7d2c 207b 224c  YPE": "NP"}, {"L
+00003b90: 454d 4d41 223a 226f 6622 7d2c 7b22 454e  EMMA":"of"},{"EN
+00003ba0: 545f 5459 5045 223a 2022 4e50 227d 5d2c  T_TYPE": "NP"}],
+00003bb0: 205b 7b22 454e 545f 5459 5045 223a 2022   [{"ENT_TYPE": "
+00003bc0: 4e50 227d 2c20 7b22 4c45 4d4d 4122 3a22  NP"}, {"LEMMA":"
+00003bd0: 6f66 227d 2c7b 2250 4f53 223a 2022 4e4f  of"},{"POS": "NO
+00003be0: 554e 227d 5d5d 2c20 2067 7265 6564 7920  UN"}]],  greedy 
+00003bf0: 3d27 4c4f 4e47 4553 5427 290a 0977 6974  ='LONGEST')..wit
+00003c00: 6820 646f 632e 7265 746f 6b65 6e69 7a65  h doc.retokenize
+00003c10: 2829 2061 7320 7265 746f 6b65 6e69 7a65  () as retokenize
+00003c20: 723a 0a09 0966 6f72 206e 616d 652c 2073  r:...for name, s
+00003c30: 7461 7274 2c20 656e 6420 696e 206d 6572  tart, end in mer
+00003c40: 6765 5f6e 5f6f 665f 6e2e 6d61 7463 6865  ge_n_of_n.matche
+00003c50: 7228 646f 6329 3a0a 0909 0969 6620 656e  r(doc):....if en
+00003c60: 6420 2d20 7374 6172 7420 3e20 313a 200a  d - start > 1: .
+00003c70: 0909 0909 7472 793a 0a09 0909 0909 6920  ....try:......i 
+00003c80: 3d20 646f 635b 7374 6172 745d 2e68 6561  = doc[start].hea
+00003c90: 642e 690a 0909 0909 0961 7474 7273 203d  d.i......attrs =
+00003ca0: 207b 2270 6f73 223a 2064 6f63 5b69 5d2e   {"pos": doc[i].
+00003cb0: 706f 732c 2022 7461 6722 3a20 646f 635b  pos, "tag": doc[
+00003cc0: 695d 2e74 6167 2c20 2264 6570 223a 2064  i].tag, "dep": d
+00003cd0: 6f63 5b69 5d2e 6465 702c 2022 6c65 6d6d  oc[i].dep, "lemm
+00003ce0: 6122 3a64 6f63 5b69 5d2e 6c65 6d6d 612c  a":doc[i].lemma,
+00003cf0: 2022 656e 745f 7479 7065 223a 2022 4e50   "ent_type": "NP
+00003d00: 227d 0a09 0909 0909 7265 746f 6b65 6e69  "}......retokeni
+00003d10: 7a65 722e 6d65 7267 6528 646f 635b 7374  zer.merge(doc[st
+00003d20: 6172 7420 3a20 656e 645d 2c20 6174 7472  art : end], attr
+00003d30: 733d 6174 7472 7329 0a09 0909 0965 7863  s=attrs).....exc
+00003d40: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00003d50: 2065 3a0a 0909 0909 0970 7269 6e74 2028   e:......print (
+00003d60: 2022 6d65 7267 655f 6e5f 6f66 5f6e 2065   "merge_n_of_n e
+00003d70: 783a 222c 2065 202c 2073 7461 7274 2c20  x:", e , start, 
+00003d80: 656e 6429 0a09 7265 7475 726e 2064 6f63  end)..return doc
+00003d90: 0a0a 404c 616e 6775 6167 652e 636f 6d70  ..@Language.comp
+00003da0: 6f6e 656e 7428 226d 6572 6765 5f76 7022  onent("merge_vp"
+00003db0: 290a 6465 6620 6d65 7267 655f 7670 2864  ).def merge_vp(d
+00003dc0: 6f63 293a 0a09 6966 206e 6f74 2068 6173  oc):..if not has
+00003dd0: 6174 7472 286d 6572 6765 5f76 702c 2027  attr(merge_vp, '
+00003de0: 6d61 7463 6865 7227 293a 0a09 096d 6572  matcher'):...mer
+00003df0: 6765 5f76 702e 6d61 7463 6865 7220 3d20  ge_vp.matcher = 
+00003e00: 4d61 7463 6865 7228 7370 6163 792e 6e6c  Matcher(spacy.nl
+00003e10: 702e 766f 6361 6229 0a09 096d 6572 6765  p.vocab)...merge
+00003e20: 5f76 702e 6d61 7463 6865 722e 6164 6428  _vp.matcher.add(
+00003e30: 2276 7022 2c20 5b5b 7b22 504f 5322 3a20  "vp", [[{"POS": 
+00003e40: 7b22 494e 223a 5b22 4155 5822 2c22 5041  {"IN":["AUX","PA
+00003e50: 5254 225d 7d2c 2022 6f70 223a 2022 2a22  RT"]}, "op": "*"
+00003e60: 7d2c 207b 2250 4f53 223a 2256 4552 4222  }, {"POS":"VERB"
+00003e70: 7d2c 7b22 504f 5322 3a20 2241 4456 222c  },{"POS": "ADV",
+00003e80: 2022 6f70 223a 2022 2a22 7d5d 5d2c 2020   "op": "*"}]],  
+00003e90: 6772 6565 6479 203d 274c 4f4e 4745 5354  greedy ='LONGEST
+00003ea0: 2729 0a09 7769 7468 2064 6f63 2e72 6574  ')..with doc.ret
+00003eb0: 6f6b 656e 697a 6528 2920 6173 2072 6574  okenize() as ret
+00003ec0: 6f6b 656e 697a 6572 3a0a 0909 666f 7220  okenizer:...for 
+00003ed0: 6e61 6d65 2c20 7374 6172 742c 2065 6e64  name, start, end
+00003ee0: 2069 6e20 6d65 7267 655f 7670 2e6d 6174   in merge_vp.mat
+00003ef0: 6368 6572 2864 6f63 293a 0a09 0909 6966  cher(doc):....if
+00003f00: 2065 6e64 202d 2073 7461 7274 203e 2031   end - start > 1
+00003f10: 3a20 0a09 0909 0974 7279 3a0a 0909 0909  : .....try:.....
+00003f20: 0969 203d 2064 6f63 5b73 7461 7274 5d2e  .i = doc[start].
+00003f30: 6865 6164 2e69 0a09 0909 0909 6174 7472  head.i......attr
+00003f40: 7320 3d20 7b22 706f 7322 3a20 646f 635b  s = {"pos": doc[
+00003f50: 695d 2e70 6f73 2c20 2274 6167 223a 2064  i].pos, "tag": d
+00003f60: 6f63 5b69 5d2e 7461 672c 2022 6465 7022  oc[i].tag, "dep"
+00003f70: 3a20 646f 635b 695d 2e64 6570 2c20 226c  : doc[i].dep, "l
+00003f80: 656d 6d61 223a 646f 635b 695d 2e6c 656d  emma":doc[i].lem
+00003f90: 6d61 2c20 2265 6e74 5f74 7970 6522 3a20  ma, "ent_type": 
+00003fa0: 2256 5022 7d0a 0909 0909 0972 6574 6f6b  "VP"}......retok
+00003fb0: 656e 697a 6572 2e6d 6572 6765 2864 6f63  enizer.merge(doc
+00003fc0: 5b73 7461 7274 203a 2065 6e64 5d2c 2061  [start : end], a
+00003fd0: 7474 7273 3d61 7474 7273 290a 0909 0909  ttrs=attrs).....
+00003fe0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00003ff0: 2061 7320 653a 0a09 0909 0909 7072 696e   as e:......prin
+00004000: 7420 2820 226d 6572 6765 5f76 7020 6578  t ( "merge_vp ex
+00004010: 3a22 2c20 6520 2c20 7374 6172 742c 2065  :", e , start, e
+00004020: 6e64 290a 0972 6574 7572 6e20 646f 630a  nd)..return doc.
+00004030: 0a64 6566 206d 6572 6765 5f70 7028 646f  .def merge_pp(do
+00004040: 6329 3a20 0a09 6966 206e 6f74 2068 6173  c): ..if not has
+00004050: 6174 7472 286d 6572 6765 5f70 702c 2027  attr(merge_pp, '
+00004060: 6d61 7463 6865 7227 293a 0a09 096d 6572  matcher'):...mer
+00004070: 6765 5f70 702e 6d61 7463 6865 7220 3d20  ge_pp.matcher = 
+00004080: 4d61 7463 6865 7228 7370 6163 792e 6e6c  Matcher(spacy.nl
+00004090: 702e 766f 6361 6229 0a09 096d 6572 6765  p.vocab)...merge
+000040a0: 5f70 702e 6d61 7463 6865 722e 6164 6428  _pp.matcher.add(
+000040b0: 2270 7022 2c20 5b5b 7b22 504f 5322 3a20  "pp", [[{"POS": 
+000040c0: 7b22 494e 223a 5b22 4144 5022 5d7d 2c20  {"IN":["ADP"]}, 
+000040d0: 226f 7022 3a20 222b 227d 2c20 7b22 454e  "op": "+"}, {"EN
+000040e0: 545f 5459 5045 223a 224e 5022 2c20 226f  T_TYPE":"NP", "o
+000040f0: 7022 3a20 222b 227d 5d5d 2c20 2067 7265  p": "+"}]],  gre
+00004100: 6564 7920 3d27 4c4f 4e47 4553 5427 290a  edy ='LONGEST').
+00004110: 0977 6974 6820 646f 632e 7265 746f 6b65  .with doc.retoke
+00004120: 6e69 7a65 2829 2061 7320 7265 746f 6b65  nize() as retoke
+00004130: 6e69 7a65 723a 0a09 0966 6f72 206e 616d  nizer:...for nam
+00004140: 652c 2073 7461 7274 2c20 656e 6420 696e  e, start, end in
+00004150: 206d 6572 6765 5f70 702e 6d61 7463 6865   merge_pp.matche
+00004160: 7228 646f 6329 3a0a 0909 0969 6620 656e  r(doc):....if en
+00004170: 6420 2d20 7374 6172 7420 3e20 313a 200a  d - start > 1: .
+00004180: 0909 0909 7472 793a 0a09 0909 0909 6920  ....try:......i 
+00004190: 3d20 646f 635b 7374 6172 745d 2e68 6561  = doc[start].hea
+000041a0: 642e 690a 0909 0909 0961 7474 7273 203d  d.i......attrs =
+000041b0: 207b 2270 6f73 223a 2064 6f63 5b69 5d2e   {"pos": doc[i].
+000041c0: 706f 732c 2022 7461 6722 3a20 646f 635b  pos, "tag": doc[
+000041d0: 695d 2e74 6167 2c20 2264 6570 223a 2064  i].tag, "dep": d
+000041e0: 6f63 5b69 5d2e 6465 702c 2022 6c65 6d6d  oc[i].dep, "lemm
+000041f0: 6122 3a64 6f63 5b69 5d2e 6c65 6d6d 612c  a":doc[i].lemma,
+00004200: 2022 656e 745f 7479 7065 223a 2022 5050   "ent_type": "PP
+00004210: 227d 0a09 0909 0909 7265 746f 6b65 6e69  "}......retokeni
+00004220: 7a65 722e 6d65 7267 6528 646f 635b 7374  zer.merge(doc[st
+00004230: 6172 7420 3a20 656e 645d 2c20 6174 7472  art : end], attr
+00004240: 733d 6174 7472 7329 0a09 0909 0965 7863  s=attrs).....exc
+00004250: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00004260: 2065 3a0a 0909 0909 0970 7269 6e74 2028   e:......print (
+00004270: 2022 6d65 7267 655f 7070 2065 783a 222c   "merge_pp ex:",
+00004280: 2065 202c 2073 7461 7274 2c20 656e 6429   e , start, end)
+00004290: 0a09 7265 7475 726e 2064 6f63 0a0a 6465  ..return doc..de
+000042a0: 6620 736b 6570 7028 646f 632c 2074 6167  f skepp(doc, tag
+000042b0: 3d22 5f50 5022 293a 2023 2061 6464 6564  ="_PP"): # added
+000042c0: 2032 3032 322e 332e 3234 2c20 207c 2046   2022.3.24,  | F
+000042d0: 726f 6d20 7468 6520 626f 6f6b 2c20 7468  rom the book, th
+000042e0: 6973 2069 7320 616c 736f 2064 6966 6669  is is also diffi
+000042f0: 6375 6c74 2074 6f20 2e2e 200a 096d 6572  cult to .. ..mer
+00004300: 6765 5f70 7028 646f 6329 2023 2074 7261  ge_pp(doc) # tra
+00004310: 6e73 666f 726d 2064 6f63 202c 2066 696e  nsform doc , fin
+00004320: 616c 6c79 2074 6f20 6265 2063 616c 6c65  ally to be calle
+00004330: 6420 0a09 7265 7475 726e 2022 2022 2e6a  d ..return " ".j
+00004340: 6f69 6e28 5b74 6167 2069 6620 742e 656e  oin([tag if t.en
+00004350: 745f 7479 7065 5f20 3d3d 2027 5050 2720  t_type_ == 'PP' 
+00004360: 656c 7365 2074 2e74 6578 7420 666f 7220  else t.text for 
+00004370: 7420 696e 2064 6f63 5d29 0a0a 6465 6620  t in doc])..def 
+00004380: 6d65 7267 655f 636c 6175 7365 2864 6f63  merge_clause(doc
+00004390: 293a 2023 2073 7562 7472 6565 206f 6620  ): # subtree of 
+000043a0: 6120 7665 7262 2069 7320 7468 6520 636c  a verb is the cl
+000043b0: 6175 7365 202c 2068 7474 7073 3a2f 2f73  ause , https://s
+000043c0: 7562 7363 7269 7074 696f 6e2e 7061 636b  ubscription.pack
+000043d0: 7470 7562 2e63 6f6d 2f62 6f6f 6b2f 6461  tpub.com/book/da
+000043e0: 7461 2f39 3738 3138 3338 3938 3733 3132  ta/9781838987312
+000043f0: 2f32 2f63 6830 326c 766c 3173 6563 3133  /2/ch02lvl1sec13
+00004400: 2f73 706c 6974 7469 6e67 2d73 656e 7465  /splitting-sente
+00004410: 6e63 6573 2d69 6e74 6f2d 636c 6175 7365  nces-into-clause
+00004420: 730a 0977 6974 6820 646f 632e 7265 746f  s..with doc.reto
+00004430: 6b65 6e69 7a65 2829 2061 7320 7265 746f  kenize() as reto
+00004440: 6b65 6e69 7a65 723a 0a09 0966 6f72 2076  kenizer:...for v
+00004450: 2069 6e20 5b74 2066 6f72 2074 2069 6e20   in [t for t in 
+00004460: 646f 6320 6966 2074 2e70 6f73 5f20 3d3d  doc if t.pos_ ==
+00004470: 2027 5645 5242 2720 616e 6420 742e 6465   'VERB' and t.de
+00004480: 705f 2021 3d20 2752 4f4f 5427 205d 203a  p_ != 'ROOT' ] :
+00004490: 2023 206e 6f6e 2d72 6f6f 740a 0909 0974   # non-root....t
+000044a0: 7279 3a0a 0909 0909 6368 696c 6472 656e  ry:.....children
+000044b0: 203d 206c 6973 7428 762e 7375 6274 7265   = list(v.subtre
+000044c0: 6529 0a09 0909 0973 7461 7274 203d 2063  e).....start = c
+000044d0: 6869 6c64 7265 6e5b 305d 2e69 2020 090a  hildren[0].i  ..
+000044e0: 0909 0909 656e 6420 3d20 6368 696c 6472  ....end = childr
+000044f0: 656e 5b2d 315d 2e69 200a 0909 0909 6174  en[-1].i .....at
+00004500: 7472 7320 3d20 7b22 706f 7322 3a20 762e  trs = {"pos": v.
+00004510: 706f 732c 2022 7461 6722 3a20 762e 7461  pos, "tag": v.ta
+00004520: 672c 2022 6465 7022 3a20 762e 6465 702c  g, "dep": v.dep,
+00004530: 2022 6c65 6d6d 6122 3a76 2e6c 656d 6d61   "lemma":v.lemma
+00004540: 2c20 2265 6e74 5f74 7970 6522 3a20 2253  , "ent_type": "S
+00004550: 2e22 202b 2076 2e64 6570 5f20 7d20 2320  ." + v.dep_ } # 
+00004560: 532e 6164 7663 6c20 2c20 2053 2e63 6f6e  S.advcl ,  S.con
+00004570: 6a20 0a09 0909 0972 6574 6f6b 656e 697a  j .....retokeniz
+00004580: 6572 2e6d 6572 6765 2864 6f63 5b73 7461  er.merge(doc[sta
+00004590: 7274 203a 2065 6e64 2b31 5d2c 2061 7474  rt : end+1], att
+000045a0: 7273 3d61 7474 7273 290a 0909 0965 7863  rs=attrs)....exc
+000045b0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+000045c0: 2065 3a0a 0909 0909 7072 696e 7420 2820   e:.....print ( 
+000045d0: 226d 6572 6765 5f63 6c61 7573 6520 6578  "merge_clause ex
+000045e0: 3a22 2c20 652c 2076 2029 0a09 7265 7475  :", e, v )..retu
+000045f0: 726e 2064 6f63 0a0a 404c 616e 6775 6167  rn doc..@Languag
+00004600: 652e 636f 6d70 6f6e 656e 7428 2273 7061  e.component("spa
+00004610: 6e5f 636c 6175 7365 2229 0a64 6566 2073  n_clause").def s
+00004620: 7061 6e5f 636c 6175 7365 2864 6f63 293a  pan_clause(doc):
+00004630: 2023 207b 2763 6c3a 3427 3a20 5b74 6861   # {'cl:4': [tha
+00004640: 7420 6974 2063 7269 6564 5d2c 2027 636c  t it cried], 'cl
+00004650: 3a31 3027 3a20 5b74 6861 7420 4920 776f  :10': [that I wo
+00004660: 756c 6420 6661 696c 5d7d 0a09 666f 7220  uld fail]}..for 
+00004670: 7620 696e 205b 7420 666f 7220 7420 696e  v in [t for t in
+00004680: 2064 6f63 2069 6620 742e 706f 735f 203d   doc if t.pos_ =
+00004690: 3d20 2756 4552 4227 2061 6e64 2074 2e64  = 'VERB' and t.d
+000046a0: 6570 5f20 213d 2027 524f 4f54 2720 5d20  ep_ != 'ROOT' ] 
+000046b0: 3a20 2320 6e6f 6e2d 726f 6f74 0a09 0974  : # non-root...t
+000046c0: 7279 3a0a 0909 0963 6869 6c64 7265 6e20  ry:....children 
+000046d0: 3d20 6c69 7374 2876 2e73 7562 7472 6565  = list(v.subtree
+000046e0: 290a 0909 0973 7461 7274 203d 2063 6869  )....start = chi
+000046f0: 6c64 7265 6e5b 305d 2e69 2020 090a 0909  ldren[0].i  ....
+00004700: 0965 6e64 203d 2063 6869 6c64 7265 6e5b  .end = children[
+00004710: 2d31 5d2e 6920 0a09 0909 6174 7472 7320  -1].i ....attrs 
+00004720: 3d20 7b22 706f 7322 3a20 762e 706f 735f  = {"pos": v.pos_
+00004730: 2c20 2274 6167 223a 2076 2e74 6167 5f2c  , "tag": v.tag_,
+00004740: 2022 6465 7022 3a20 762e 6465 705f 2c20   "dep": v.dep_, 
+00004750: 226c 656d 6d61 223a 762e 6c65 6d6d 615f  "lemma":v.lemma_
+00004760: 2c20 2265 6e74 5f74 7970 6522 3a20 2253  , "ent_type": "S
+00004770: 2e22 202b 2076 2e64 6570 5f20 7d20 2320  ." + v.dep_ } # 
+00004780: 532e 6164 7663 6c20 2c20 2053 2e63 6f6e  S.advcl ,  S.con
+00004790: 6a20 0a09 0909 6e61 6d65 203d 2066 2263  j ....name = f"c
+000047a0: 6c3a 7b73 7461 7274 7d22 200a 0909 0964  l:{start}" ....d
+000047b0: 6f63 2e73 7061 6e73 5b6e 616d 655d 203d  oc.spans[name] =
+000047c0: 2053 7061 6e47 726f 7570 2864 6f63 2c20   SpanGroup(doc, 
+000047d0: 6e61 6d65 3d6e 616d 652c 2073 7061 6e73  name=name, spans
+000047e0: 3d5b 2064 6f63 5b73 7461 7274 203a 2065  =[ doc[start : e
+000047f0: 6e64 2b31 5d20 5d2c 2061 7474 7273 3d61  nd+1] ], attrs=a
+00004800: 7474 7273 290a 0909 6578 6365 7074 2045  ttrs)...except E
+00004810: 7863 6570 7469 6f6e 2061 7320 653a 0a09  xception as e:..
+00004820: 0909 7072 696e 7420 2820 2273 7061 6e5f  ..print ( "span_
+00004830: 636c 6175 7365 2065 783a 222c 2065 2c20  clause ex:", e, 
+00004840: 7620 290a 0972 6574 7572 6e20 646f 630a  v )..return doc.
+00004850: 0a4e 505f 7374 6172 7420 3d20 7b22 454e  .NP_start = {"EN
+00004860: 545f 5459 5045 223a 2022 4e50 222c 2022  T_TYPE": "NP", "
+00004870: 4953 5f53 454e 545f 5354 4152 5422 3a20  IS_SENT_START": 
+00004880: 5472 7565 7d0a 5645 5242 0920 3d20 7b22  True}.VERB. = {"
+00004890: 504f 5322 3a20 7b22 494e 223a 205b 2256  POS": {"IN": ["V
+000048a0: 4552 4222 5d7d 7d0a 4e4f 554e 0920 3d20  ERB"]}}.NOUN. = 
+000048b0: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
+000048c0: 224e 4f55 4e22 2c22 5052 4f4e 222c 2250  "NOUN","PRON","P
+000048d0: 524f 504e 225d 7d7d 0a50 554e 4354 0920  ROPN"]}}.PUNCT. 
+000048e0: 3d20 7b22 4953 5f50 554e 4354 223a 2054  = {"IS_PUNCT": T
+000048f0: 7275 657d 0a5f 7665 7262 6e65 745f 7275  rue}._verbnet_ru
+00004900: 6c65 7320 3d20 7b20 2023 203a 3120 2c20  les = {  # :1 , 
+00004910: 7665 7262 2773 206f 6666 7365 7420 0a09  verb's offset ..
+00004920: 224e 5020 563a 3122 3a20 5b5b 4e50 5f73  "NP V:1": [[NP_s
+00004930: 7461 7274 2c56 4552 422c 2050 554e 4354  tart,VERB, PUNCT
+00004940: 5d5d 2c20 0a09 224e 5020 6f66 204e 5020  ]], .."NP of NP 
+00004950: 563a 3322 3a20 5b5b 204e 505f 7374 6172  V:3": [[ NP_star
+00004960: 742c 7b22 4c45 4d4d 4122 3a20 226f 6622  t,{"LEMMA": "of"
+00004970: 7d2c 207b 2245 4e54 5f54 5950 4522 3a20  }, {"ENT_TYPE": 
+00004980: 224e 5022 7d2c 2056 4552 422c 5055 4e43  "NP"}, VERB,PUNC
+00004990: 545d 5d2c 200a 0922 4e50 2056 204e 503a  T]], .."NP V NP:
+000049a0: 3122 3a20 5b5b 4e4f 554e 2c56 4552 422c  1": [[NOUN,VERB,
+000049b0: 204e 4f55 4e2c 7b22 504f 5322 3a20 7b22   NOUN,{"POS": {"
+000049c0: 494e 223a 205b 2250 554e 4354 225d 7d7d  IN": ["PUNCT"]}}
+000049d0: 5d5d 2c20 0a09 224e 5020 5620 4e50 2041  ]], .."NP V NP A
+000049e0: 444a 3a31 223a 205b 5b4e 4f55 4e2c 5645  DJ:1": [[NOUN,VE
+000049f0: 5242 2c20 4e4f 554e 2c7b 2250 4f53 223a  RB, NOUN,{"POS":
+00004a00: 207b 2249 4e22 3a20 5b22 4144 4a22 5d7d   {"IN": ["ADJ"]}
+00004a10: 7d5d 5d2c 200a 0922 4e50 2056 204e 5020  }]], .."NP V NP 
+00004a20: 4e50 3a31 223a 205b 5b4e 4f55 4e2c 5645  NP:1": [[NOUN,VE
+00004a30: 5242 2c20 4e4f 554e 2c4e 4f55 4e5d 5d2c  RB, NOUN,NOUN]],
+00004a40: 200a 0922 4e50 2056 204e 502d 4461 7469   .."NP V NP-Dati
+00004a50: 7665 204e 503a 3122 3a20 5b5b 4e4f 554e  ve NP:1": [[NOUN
+00004a60: 2c56 4552 422c 207b 2244 4550 223a 207b  ,VERB, {"DEP": {
+00004a70: 2249 4e22 3a20 5b22 6461 7469 7665 225d  "IN": ["dative"]
+00004a80: 7d7d 2c4e 4f55 4e5d 5d2c 200a 0922 4e50  }},NOUN]], .."NP
+00004a90: 2056 204e 5020 5050 3a31 223a 205b 5b4e   V NP PP:1": [[N
+00004aa0: 4f55 4e2c 5645 5242 2c20 4e4f 554e 2c7b  OUN,VERB, NOUN,{
+00004ab0: 2244 4550 223a 207b 2249 4e22 3a20 5b22  "DEP": {"IN": ["
+00004ac0: 7072 6570 225d 7d7d 5d5d 2c20 0a09 224e  prep"]}}]], .."N
+00004ad0: 5020 5620 4e50 2050 5020 5050 3a31 223a  P V NP PP PP:1":
+00004ae0: 205b 5b4e 4f55 4e2c 5645 5242 2c20 4e4f   [[NOUN,VERB, NO
+00004af0: 554e 2c7b 2244 4550 223a 207b 2249 4e22  UN,{"DEP": {"IN"
+00004b00: 3a20 5b22 7072 6570 225d 7d7d 2c20 4e4f  : ["prep"]}}, NO
+00004b10: 554e 2c7b 2244 4550 223a 207b 2249 4e22  UN,{"DEP": {"IN"
+00004b20: 3a20 5b22 7072 6570 225d 7d7d 2c20 4e4f  : ["prep"]}}, NO
+00004b30: 554e 5d5d 2c20 0a09 224e 5020 5620 535f  UN]], .."NP V S_
+00004b40: 494e 473a 3122 3a20 5b5b 4e4f 554e 2c56  ING:1": [[NOUN,V
+00004b50: 4552 422c 207b 2254 4147 223a 207b 2249  ERB, {"TAG": {"I
+00004b60: 4e22 3a20 5b22 5642 4722 5d7d 7d5d 5d2c  N": ["VBG"]}}]],
+00004b70: 200a 0922 4e50 2056 2077 6865 7468 6572   .."NP V whether
+00004b80: 2f68 6f77 2053 5f49 4e46 3a31 223a 205b  /how S_INF:1": [
+00004b90: 5b4e 4f55 4e2c 5645 5242 2c20 7b22 4c45  [NOUN,VERB, {"LE
+00004ba0: 4d4d 4122 3a20 7b22 494e 223a 205b 2277  MMA": {"IN": ["w
+00004bb0: 6865 7468 6572 222c 2268 6f77 225d 7d7d  hether","how"]}}
+00004bc0: 2c20 7b22 4c45 4d4d 4122 3a20 7b22 494e  , {"LEMMA": {"IN
+00004bd0: 223a 205b 2274 6f22 5d7d 7d2c 2056 4552  ": ["to"]}}, VER
+00004be0: 425d 5d2c 200a 0922 4e50 2056 204e 5020  B]], .."NP V NP 
+00004bf0: 746f 2062 6520 4e50 3a31 223a 205b 5b4e  to be NP:1": [[N
+00004c00: 4f55 4e2c 5645 5242 2c20 7b22 4c45 4d4d  OUN,VERB, {"LEMM
+00004c10: 4122 3a20 7b22 494e 223a 205b 2274 6f22  A": {"IN": ["to"
+00004c20: 5d7d 7d2c 207b 224c 454d 4d41 223a 207b  ]}}, {"LEMMA": {
+00004c30: 2249 4e22 3a20 5b22 6265 225d 7d7d 2c20  "IN": ["be"]}}, 
+00004c40: 4e4f 554e 5d5d 2c20 0a09 224e 5020 5620  NOUN]], .."NP V 
+00004c50: 7468 6174 2f68 6f77 2053 3a31 223a 205b  that/how S:1": [
+00004c60: 5b4e 4f55 4e2c 5645 5242 2c20 7b22 4c45  [NOUN,VERB, {"LE
+00004c70: 4d4d 4122 3a20 7b22 494e 223a 205b 2274  MMA": {"IN": ["t
+00004c80: 6861 7422 2c22 686f 7722 5d7d 2c20 224f  hat","how"]}, "O
+00004c90: 5022 3a22 2a22 7d2c 204e 4f55 4e2c 207b  P":"*"}, NOUN, {
+00004ca0: 2250 4f53 223a 207b 2249 4e22 3a20 5b22  "POS": {"IN": ["
+00004cb0: 4155 5822 2c22 5041 5254 225d 7d2c 2022  AUX","PART"]}, "
+00004cc0: 4f50 223a 222a 227d 2c7b 2244 4550 223a  OP":"*"},{"DEP":
+00004cd0: 207b 2249 4e22 3a20 5b22 6363 6f6d 7022   {"IN": ["ccomp"
+00004ce0: 5d7d 7d5d 5d2c 2020 2354 6865 7920 636f  ]}}]],  #They co
+00004cf0: 6e73 6964 6572 6564 2074 6861 7420 6865  nsidered that he
+00004d00: 2077 6173 2074 6865 2070 726f 6665 7373   was the profess
+00004d10: 6f72 2e0a 0922 4e50 2056 2077 6865 7468  or..."NP V wheth
+00004d20: 6572 2f69 6620 533a 3122 3a20 5b5b 4e4f  er/if S:1": [[NO
+00004d30: 554e 2c56 4552 422c 207b 224c 454d 4d41  UN,VERB, {"LEMMA
+00004d40: 223a 207b 2249 4e22 3a20 5b22 7768 6574  ": {"IN": ["whet
+00004d50: 6865 7222 2c22 6966 225d 7d7d 2c20 4e4f  her","if"]}}, NO
+00004d60: 554e 2c7b 2250 4f53 223a 207b 2249 4e22  UN,{"POS": {"IN"
+00004d70: 3a20 5b22 4155 5822 2c22 5041 5254 225d  : ["AUX","PART"]
+00004d80: 7d2c 2022 4f50 223a 222a 227d 2c20 7b22  }, "OP":"*"}, {"
+00004d90: 4445 5022 3a20 7b22 494e 223a 205b 2263  DEP": {"IN": ["c
+00004da0: 636f 6d70 225d 7d7d 5d5d 2c20 2023 4865  comp"]}}]],  #He
+00004db0: 2063 6f6e 7369 6465 7265 6420 7768 6574   considered whet
+00004dc0: 6865 7220 6865 2073 686f 756c 6420 636f  her he should co
+00004dd0: 6d65 2e0a 0922 4e50 2056 2077 6861 7420  me..."NP V what 
+00004de0: 533a 3122 3a20 5b5b 4e4f 554e 2c56 4552  S:1": [[NOUN,VER
+00004df0: 422c 207b 224c 454d 4d41 223a 207b 2249  B, {"LEMMA": {"I
+00004e00: 4e22 3a20 5b22 7768 6174 225d 7d7d 2c20  N": ["what"]}}, 
+00004e10: 4e4f 554e 2c7b 2250 4f53 223a 207b 2249  NOUN,{"POS": {"I
+00004e20: 4e22 3a20 5b22 4155 5822 2c22 5041 5254  N": ["AUX","PART
+00004e30: 225d 7d2c 2022 4f50 223a 222a 227d 2c20  "]}, "OP":"*"}, 
+00004e40: 7b22 4445 5022 3a20 7b22 494e 223a 205b  {"DEP": {"IN": [
+00004e50: 2263 636f 6d70 225d 7d7d 5d5d 2c20 200a  "ccomp"]}}]],  .
+00004e60: 0922 4e50 2056 2077 6861 7420 535f 494e  ."NP V what S_IN
+00004e70: 463a 3122 3a20 5b5b 4e4f 554e 2c56 4552  F:1": [[NOUN,VER
+00004e80: 422c 207b 224c 454d 4d41 223a 207b 2249  B, {"LEMMA": {"I
+00004e90: 4e22 3a20 5b22 7768 6174 225d 7d7d 2c20  N": ["what"]}}, 
+00004ea0: 7b22 4c45 4d4d 4122 3a20 7b22 494e 223a  {"LEMMA": {"IN":
+00004eb0: 205b 2274 6f22 5d7d 7d2c 5645 5242 5d5d   ["to"]}},VERB]]
+00004ec0: 2c0a 7d0a 6465 6620 7665 7262 6e65 745f  ,.}.def verbnet_
+00004ed0: 6d61 7463 6865 7228 646f 6329 3a20 0a09  matcher(doc): ..
+00004ee0: 6966 206e 6f74 2068 6173 6174 7472 2876  if not hasattr(v
+00004ef0: 6572 626e 6574 5f6d 6174 6368 6572 2c20  erbnet_matcher, 
+00004f00: 276d 6174 6368 6572 2729 3a20 0a09 0976  'matcher'): ...v
+00004f10: 6572 626e 6574 5f6d 6174 6368 6572 2e6d  erbnet_matcher.m
+00004f20: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
+00004f30: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
+00004f40: 290a 0909 5b20 7665 7262 6e65 745f 6d61  )...[ verbnet_ma
+00004f50: 7463 6865 722e 6d61 7463 6865 722e 6164  tcher.matcher.ad
+00004f60: 6428 6e61 6d65 2c20 7061 7474 6572 6e73  d(name, patterns
+00004f70: 2c20 6772 6565 6479 203d 274c 4f4e 4745  , greedy ='LONGE
+00004f80: 5354 2729 2020 666f 7220 6e61 6d65 2c20  ST')  for name, 
+00004f90: 7061 7474 6572 6e73 2069 6e20 5f76 6572  patterns in _ver
+00004fa0: 626e 6574 5f72 756c 6573 2e69 7465 6d73  bnet_rules.items
+00004fb0: 2829 205d 0a09 6d65 7267 655f 6e70 2864  () ]..merge_np(d
+00004fc0: 6f63 290a 096d 6572 6765 5f76 7028 646f  oc)..merge_vp(do
+00004fd0: 6329 0a09 7265 7320 3d20 5b5d 0a09 666f  c)..res = []..fo
+00004fe0: 7220 6e61 6d65 2c20 6962 6567 2c20 6965  r name, ibeg, ie
+00004ff0: 6e64 2069 6e20 7665 7262 6e65 745f 6d61  nd in verbnet_ma
+00005000: 7463 6865 722e 6d61 7463 6865 7228 646f  tcher.matcher(do
+00005010: 6329 3a0a 0909 7472 793a 0a09 0909 6172  c):...try:....ar
+00005020: 7220 3d20 7370 6163 792e 6e6c 702e 766f  r = spacy.nlp.vo
+00005030: 6361 625b 6e61 6d65 5d2e 7465 7874 2e73  cab[name].text.s
+00005040: 706c 6974 2827 3a27 2920 0a09 0909 7665  plit(':') ....ve
+00005050: 7262 5f69 203d 2069 6265 6720 2b20 696e  rb_i = ibeg + in
+00005060: 7428 6172 725b 2d31 5d29 200a 0909 0972  t(arr[-1]) ....r
+00005070: 6573 2e61 7070 656e 6428 2028 7665 7262  es.append( (verb
+00005080: 5f69 2c20 6962 6567 2c20 6965 6e64 2c20  _i, ibeg, iend, 
+00005090: 6172 725b 305d 2e73 7472 6970 2829 2920  arr[0].strip()) 
+000050a0: 2920 0a09 0965 7863 6570 7420 4578 6365  ) ...except Exce
+000050b0: 7074 696f 6e20 6173 2065 3a0a 0909 0970  ption as e:....p
+000050c0: 7269 6e74 2028 2776 6572 626e 6574 2065  rint ('verbnet e
+000050d0: 783a 272c 2065 2c20 6e61 6d65 2c20 6962  x:', e, name, ib
+000050e0: 6567 2c20 6965 6e64 290a 0972 6574 7572  eg, iend)..retur
+000050f0: 6e20 7265 7320 0a0a 7369 6d70 6c65 5f73  n res ..simple_s
+00005100: 656e 7409 093d 206c 616d 6264 6120 646f  ent..= lambda do
+00005110: 633a 206c 656e 285b 7420 666f 7220 7420  c: len([t for t 
+00005120: 696e 2064 6f63 2069 6620 742e 706f 735f  in doc if t.pos_
+00005130: 203d 3d20 2756 4552 4227 2061 6e64 2074   == 'VERB' and t
+00005140: 2e64 6570 5f20 213d 2027 524f 4f54 275d  .dep_ != 'ROOT']
+00005150: 2920 3c3d 2030 200a 636f 6d70 6c65 785f  ) <= 0 .complex_
+00005160: 7365 6e74 093d 206c 616d 6264 6120 646f  sent.= lambda do
+00005170: 633a 206c 656e 285b 7420 666f 7220 7420  c: len([t for t 
+00005180: 696e 2064 6f63 2069 6620 742e 706f 735f  in doc if t.pos_
+00005190: 203d 3d20 2756 4552 4227 2061 6e64 2074   == 'VERB' and t
+000051a0: 2e64 6570 5f20 213d 2027 524f 4f54 275d  .dep_ != 'ROOT']
+000051b0: 2920 3e20 300a 636f 6d70 6f75 6e64 5f73  ) > 0.compound_s
+000051c0: 656e 7409 3d20 6c61 6d62 6461 2064 6f63  ent.= lambda doc
+000051d0: 3a20 6c65 6e28 5b74 2066 6f72 2074 2069  : len([t for t i
+000051e0: 6e20 646f 6320 6966 2074 2e64 6570 5f20  n doc if t.dep_ 
+000051f0: 3d3d 2027 636f 6e6a 2720 616e 6420 742e  == 'conj' and t.
+00005200: 6865 6164 2e64 6570 5f20 3d3d 2027 524f  head.dep_ == 'RO
+00005210: 4f54 275d 2920 3e20 3020 2023 2053 2e63  OT']) > 0  # S.c
+00005220: 6f6e 6a20 0a73 7479 7065 0909 093d 206c  onj .stype...= l
+00005230: 616d 6264 6120 646f 633a 0922 7369 6d70  ambda doc:."simp
+00005240: 6c65 5f73 656e 7422 2069 6620 6c65 6e28  le_sent" if len(
+00005250: 5b74 2066 6f72 2074 2069 6e20 646f 6320  [t for t in doc 
+00005260: 6966 2074 2e70 6f73 5f20 3d3d 2027 5645  if t.pos_ == 'VE
+00005270: 5242 2720 616e 6420 742e 6465 705f 2021  RB' and t.dep_ !
+00005280: 3d20 2752 4f4f 5427 5d29 203c 3d20 3020  = 'ROOT']) <= 0 
+00005290: 656c 7365 2022 636f 6d70 6c65 785f 7365  else "complex_se
+000052a0: 6e74 220a 736b 656c 6574 6f6e 0909 3d20  nt".skeleton..= 
+000052b0: 6c61 6d62 6461 2064 6f63 3a20 2022 2022  lambda doc:  " "
+000052c0: 2e6a 6f69 6e28 5b20 742e 656e 745f 7479  .join([ t.ent_ty
+000052d0: 7065 5f20 6966 2074 2e65 6e74 5f74 7970  pe_ if t.ent_typ
+000052e0: 655f 2065 6c73 6520 742e 7465 7874 2069  e_ else t.text i
+000052f0: 6620 742e 6973 5f70 756e 6374 206f 7220  f t.is_punct or 
+00005300: 742e 6465 705f 203d 3d20 2752 4f4f 5427  t.dep_ == 'ROOT'
+00005310: 2065 6c73 6520 742e 706f 735f 2066 6f72   else t.pos_ for
+00005320: 2074 2069 6e20 646f 6320 5d29 0a0a 6465   t in doc ])..de
+00005330: 6620 636c 6175 7365 2864 6f63 293a 2020  f clause(doc):  
+00005340: 2320 7b27 532e 7072 6570 2d30 273a 207b  # {'S.prep-0': {
+00005350: 2774 7970 6527 3a20 2753 2e70 7265 7027  'type': 'S.prep'
+00005360: 2c20 2773 7461 7274 273a 2030 2c20 2765  , 'start': 0, 'e
+00005370: 6e64 273a 2032 2c20 276c 656d 273a 2027  nd': 2, 'lem': '
+00005380: 636f 6e73 6964 6572 272c 2027 6368 756e  consider', 'chun
+00005390: 6b27 3a20 2743 6f6e 7369 6465 7269 6e67  k': 'Considering
+000053a0: 2074 6865 2070 6f73 7369 6269 6c69 7479   the possibility
+000053b0: 277d 2c20 2753 2e63 6f6e 6a2d 3927 3a20  '}, 'S.conj-9': 
+000053c0: 7b27 7479 7065 273a 2027 532e 636f 6e6a  {'type': 'S.conj
+000053d0: 272c 2027 7374 6172 7427 3a20 392c 2027  ', 'start': 9, '
+000053e0: 656e 6427 3a20 3132 2c20 276c 656d 273a  end': 12, 'lem':
+000053f0: 2027 6265 272c 2027 6368 756e 6b27 3a20   'be', 'chunk': 
+00005400: 2773 6865 2069 7320 6f6b 202e 277d 7d0a  'she is ok .'}}.
+00005410: 0961 7272 203d 205b 5d0a 0966 6f72 2076  .arr = []..for v
+00005420: 2069 6e20 5b74 2066 6f72 2074 2069 6e20   in [t for t in 
+00005430: 646f 6320 6966 2074 2e70 6f73 5f20 3d3d  doc if t.pos_ ==
+00005440: 2027 5645 5242 2720 616e 6420 742e 6465   'VERB' and t.de
+00005450: 705f 2021 3d20 2752 4f4f 5427 205d 203a  p_ != 'ROOT' ] :
+00005460: 2023 206e 6f6e 2d72 6f6f 740a 0909 6368   # non-root...ch
+00005470: 696c 6472 656e 203d 206c 6973 7428 762e  ildren = list(v.
+00005480: 7375 6274 7265 6529 2023 656e 6420 3d20  subtree) #end = 
+00005490: 6368 696c 6472 656e 5b2d 315d 2e69 2009  children[-1].i .
+000054a0: 7461 6720 3d20 2253 2e22 202b 2076 2e64  tag = "S." + v.d
+000054b0: 6570 5f20 2020 2320 532e 6164 7663 6c20  ep_   # S.advcl 
+000054c0: 2c20 2053 2e63 6f6e 6a20 0a09 0973 7461  ,  S.conj ...sta
+000054d0: 7274 203d 2063 6869 6c64 7265 6e5b 305d  rt = children[0]
+000054e0: 2e69 0a09 0965 6e64 203d 2063 6869 6c64  .i...end = child
+000054f0: 7265 6e5b 2d31 5d2e 6920 2b20 3120 2322  ren[-1].i + 1 #"
+00005500: 7479 7065 223a 2263 6c22 2c20 226b 7022  type":"cl", "kp"
+00005510: 3a20 2253 2e22 202b 2076 2e64 6570 5f2c  : "S." + v.dep_,
+00005520: 0a09 0961 7272 2e61 7070 656e 6428 2028  ...arr.append( (
+00005530: 762c 2076 2e64 6570 5f2c 2073 7461 7274  v, v.dep_, start
+00005540: 2c20 656e 642c 2022 2022 2e6a 6f69 6e28  , end, " ".join(
+00005550: 5b63 2e74 6578 7420 666f 7220 6320 696e  [c.text for c in
+00005560: 2076 2e73 7562 7472 6565 5d29 2920 2920   v.subtree])) ) 
+00005570: 236c 6173 7420 6f6e 6520 6973 2027 6368  #last one is 'ch
+00005580: 756e 6b27 2020 206c 656d 706f 7322 3a76  unk'   lempos":v
+00005590: 2e6c 656d 6d61 5f20 2b20 225f 2220 2b20  .lemma_ + "_" + 
+000055a0: 762e 706f 735f 2c22 6368 756e 6b22 3a20  v.pos_,"chunk": 
+000055b0: 7d20 2322 6c65 6d22 3a76 2e6c 656d 6d61  } #"lem":v.lemma
+000055c0: 5f2c 204e 4f54 2063 6f6e 6675 7365 2077  _, NOT confuse w
+000055d0: 6974 6820 2774 6f6b 2720 0a09 7265 7475  ith 'tok' ..retu
+000055e0: 726e 2061 7272 200a 0a5f 7670 5f72 756c  rn arr .._vp_rul
+000055f0: 6573 203d 207b 0a22 7665 6e64 223a 5b5b  es = {."vend":[[
+00005600: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
+00005610: 2241 5558 222c 2256 4552 4222 5d7d 7d2c  "AUX","VERB"]}},
+00005620: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
+00005630: 2241 4456 225d 7d2c 2022 4f50 223a 2022  "ADV"]}, "OP": "
+00005640: 2a22 7d2c 207b 2250 4f53 223a 207b 2249  *"}, {"POS": {"I
+00005650: 4e22 3a20 5b22 4144 4a22 2c22 5645 5242  N": ["ADJ","VERB
+00005660: 225d 7d2c 2022 4f50 223a 2022 2a22 7d2c  "]}, "OP": "*"},
+00005670: 7b22 504f 5322 3a20 7b22 494e 223a 205b  {"POS": {"IN": [
+00005680: 2250 4152 5422 2c22 4144 5022 2c22 544f  "PART","ADP","TO
+00005690: 225d 7d2c 2022 4f50 223a 2022 2a22 7d2c  "]}, "OP": "*"},
+000056a0: 7b22 504f 5322 3a20 2756 4552 4227 7d5d  {"POS": 'VERB'}]
+000056b0: 5d2c 2023 2063 6f75 6c64 2068 6172 646c  ], # could hardl
+000056c0: 7920 7761 6974 2074 6f20 6d65 6574 0a22  y wait to meet."
+000056d0: 7670 223a 2020 5b5b 7b27 504f 5327 3a20  vp":  [[{'POS': 
+000056e0: 2756 4552 4227 7d2c 7b22 504f 5322 3a20  'VERB'},{"POS": 
+000056f0: 7b22 494e 223a 205b 2244 4554 222c 2241  {"IN": ["DET","A
+00005700: 4450 222c 2241 444a 225d 7d2c 2022 4f50  DP","ADJ"]}, "OP
+00005710: 223a 2022 2a22 7d2c 7b22 504f 5322 3a20  ": "*"},{"POS": 
+00005720: 274e 4f55 4e27 7d2c 207b 2250 4f53 223a  'NOUN'}, {"POS":
+00005730: 207b 2249 4e22 3a20 5b22 4144 5022 2c22   {"IN": ["ADP","
+00005740: 544f 225d 7d2c 2022 4f50 223a 2022 2a22  TO"]}, "OP": "*"
+00005750: 7d5d 2c20 5b7b 2750 4f53 273a 2027 5645  }], [{'POS': 'VE
+00005760: 5242 277d 2c7b 2250 4f53 223a 207b 2249  RB'},{"POS": {"I
+00005770: 4e22 3a20 5b22 4445 5422 2c22 4144 5022  N": ["DET","ADP"
+00005780: 2c22 4144 4a22 2c22 544f 222c 2250 4152  ,"ADJ","TO","PAR
+00005790: 5422 5d7d 2c20 224f 5022 3a20 222a 227d  T"]}, "OP": "*"}
+000057a0: 2c7b 2250 4f53 223a 2027 5645 5242 277d  ,{"POS": 'VERB'}
+000057b0: 5d5d 2c20 2320 7761 6974 2074 6f20 6d65  ]], # wait to me
+000057c0: 6574 0a22 7070 223a 2020 5b5b 7b27 504f  et."pp":  [[{'PO
+000057d0: 5327 3a20 2741 4450 277d 2c7b 2250 4f53  S': 'ADP'},{"POS
+000057e0: 223a 207b 2249 4e22 3a20 5b22 4445 5422  ": {"IN": ["DET"
+000057f0: 2c22 4e55 4d22 2c22 4144 4a22 2c27 5055  ,"NUM","ADJ",'PU
+00005800: 4e43 5427 2c27 434f 4e4a 275d 7d2c 2022  NCT','CONJ']}, "
+00005810: 4f50 223a 2022 2a22 7d2c 7b22 504f 5322  OP": "*"},{"POS"
+00005820: 3a20 7b22 494e 223a 205b 224e 4f55 4e22  : {"IN": ["NOUN"
+00005830: 2c22 5041 5254 225d 7d2c 2022 4f50 223a  ,"PART"]}, "OP":
+00005840: 2022 2b22 7d5d 5d2c 2020 2020 0a22 6170   "+"}]],    ."ap
+00005850: 223a 2020 5b5b 7b22 504f 5322 3a20 7b22  ":  [[{"POS": {"
+00005860: 494e 223a 205b 2241 4456 225d 7d2c 2022  IN": ["ADV"]}, "
+00005870: 4f50 223a 2022 2a22 7d2c 207b 2250 4f53  OP": "*"}, {"POS
+00005880: 223a 2027 4144 4a27 7d5d 5d2c 2020 0a22  ": 'ADJ'}]],  ."
+00005890: 7670 7274 223a 5b5b 7b22 504f 5322 3a20  vprt":[[{"POS": 
+000058a0: 2756 4552 4227 7d2c 207b 2250 4f53 223a  'VERB'}, {"POS":
+000058b0: 207b 2249 4e22 3a20 5b22 5052 4550 222c   {"IN": ["PREP",
+000058c0: 2022 4144 5022 2c27 544f 275d 7d2c 2022   "ADP",'TO']}, "
+000058d0: 4f50 223a 2022 2b22 7d5d 5d2c 2020 2023  OP": "+"}]],   #
+000058e0: 206c 6f6f 6b20 7570 202f 6c6f 6f6b 2075   look up /look u
+000058f0: 7020 6672 6f6d 2c20 2063 6f6d 7075 7465  p from,  compute
+00005900: 6420 7477 6963 650a 2276 746f 7622 3a5b  d twice."vtov":[
+00005910: 5b7b 2250 4f53 223a 2027 5645 5242 277d  [{"POS": 'VERB'}
+00005920: 2c20 7b22 5441 4722 3a20 2754 4f27 7d2c  , {"TAG": 'TO'},
+00005930: 7b22 5441 4722 3a20 2756 4227 7d5d 5d2c  {"TAG": 'VB'}]],
+00005940: 2020 2023 2070 6c61 6e20 746f 2067 6f0a     # plan to go.
+00005950: 2276 7662 6722 3a5b 5b7b 2250 4f53 223a  "vvbg":[[{"POS":
+00005960: 2027 5645 5242 277d 2c20 7b22 5441 4722   'VERB'}, {"TAG"
+00005970: 3a20 2756 4247 277d 5d5d 2c20 2020 2320  : 'VBG'}]],   # 
+00005980: 636f 6e73 6964 6572 2067 6f69 6e67 0a22  consider going."
+00005990: 7670 6722 3a20 5b5b 7b22 504f 5322 3a20  vpg": [[{"POS": 
+000059a0: 2756 4552 4227 7d2c 207b 2250 4f53 223a  'VERB'}, {"POS":
+000059b0: 207b 2249 4e22 3a20 5b22 5052 4550 222c   {"IN": ["PREP",
+000059c0: 2022 4144 5022 2c27 5041 5254 275d 7d2c   "ADP",'PART']},
+000059d0: 2022 4f50 223a 2022 2b22 7d2c 7b22 5441   "OP": "+"},{"TA
+000059e0: 4722 3a20 2756 4247 277d 5d5d 2c20 2020  G": 'VBG'}]],   
+000059f0: 2320 696e 7369 7374 6564 206f 6e20 676f  # insisted on go
+00005a00: 696e 670a 2276 4170 223a 205b 5b7b 274c  ing."vAp": [[{'L
+00005a10: 454d 4d41 273a 2027 6265 277d 2c7b 2254  EMMA': 'be'},{"T
+00005a20: 4147 223a 207b 2249 4e22 3a20 5b22 5642  AG": {"IN": ["VB
+00005a30: 4e22 5d7d 7d2c 207b 2250 4f53 223a 207b  N"]}}, {"POS": {
+00005a40: 2249 4e22 3a20 5b22 5052 4550 222c 2022  "IN": ["PREP", "
+00005a50: 4144 5022 2c27 5041 5254 275d 7d7d 5d5d  ADP",'PART']}}]]
+00005a60: 2c20 2020 2320 6265 2062 6173 6564 206f  ,   # be based o
+00005a70: 6e20 2020 0a22 7661 7022 3a20 5b5b 7b27  n   ."vap": [[{'
+00005a80: 4c45 4d4d 4127 3a20 2762 6527 7d2c 7b22  LEMMA': 'be'},{"
+00005a90: 504f 5322 3a20 7b22 494e 223a 205b 2241  POS": {"IN": ["A
+00005aa0: 444a 225d 7d7d 2c20 7b22 504f 5322 3a20  DJ"]}}, {"POS": 
+00005ab0: 7b22 494e 223a 205b 2250 5245 5022 2c20  {"IN": ["PREP", 
+00005ac0: 2241 4450 222c 2750 4152 5427 5d7d 7d5d  "ADP",'PART']}}]
+00005ad0: 5d2c 2020 2023 2062 6520 616e 6772 7920  ],   # be angry 
+00005ae0: 7769 7468 0a7d 2023 666f 7220 6e61 6d65  with.} #for name
+00005af0: 2c20 6962 6567 2c69 656e 6420 696e 206d  , ibeg,iend in m
+00005b00: 6174 6368 6572 2864 6f63 2920 3a20 7072  atcher(doc) : pr
+00005b10: 696e 7428 7370 6163 792e 6e6c 702e 766f  int(spacy.nlp.vo
+00005b20: 6361 625b 6e61 6d65 5d2e 7465 7874 2c20  cab[name].text, 
+00005b30: 646f 635b 6962 6567 3a69 656e 645d 2e74  doc[ibeg:iend].t
+00005b40: 6578 7429 0a0a 6465 6620 7670 5f6d 6174  ext)..def vp_mat
+00005b50: 6368 6572 2864 6f63 293a 2023 5b28 2776  cher(doc): #[('v
+00005b60: 656e 6427 2c20 2763 6f6e 7369 6465 7220  end', 'consider 
+00005b70: 676f 696e 6727 2c20 312c 2033 292c 2028  going', 1, 3), (
+00005b80: 2776 7027 2c20 2763 6f6e 7369 6465 7220  'vp', 'consider 
+00005b90: 676f 696e 6727 2c20 312c 2033 292c 2028  going', 1, 3), (
+00005ba0: 2776 7662 6727 2c20 2763 6f6e 7369 6465  'vvbg', 'conside
+00005bb0: 7220 676f 696e 6727 2c20 312c 2033 292c  r going', 1, 3),
+00005bc0: 2028 2776 7072 7427 2c20 2767 6f69 6e67   ('vprt', 'going
+00005bd0: 2074 6f27 2c20 322c 2034 295d 0a09 6966   to', 2, 4)]..if
+00005be0: 206e 6f74 2068 6173 6174 7472 2876 705f   not hasattr(vp_
+00005bf0: 6d61 7463 6865 722c 2027 6d61 7463 6865  matcher, 'matche
+00005c00: 7227 293a 200a 0909 7670 5f6d 6174 6368  r'): ...vp_match
+00005c10: 6572 2e6d 6174 6368 6572 203d 204d 6174  er.matcher = Mat
+00005c20: 6368 6572 2873 7061 6379 2e6e 6c70 2e76  cher(spacy.nlp.v
+00005c30: 6f63 6162 290a 0909 5b76 705f 6d61 7463  ocab)...[vp_matc
+00005c40: 6865 722e 6d61 7463 6865 722e 6164 6428  her.matcher.add(
+00005c50: 6e61 6d65 2c20 7061 7474 6572 6e73 2c20  name, patterns, 
+00005c60: 2067 7265 6564 7920 3d27 4c4f 4e47 4553   greedy ='LONGES
+00005c70: 5427 2920 666f 7220 6e61 6d65 2c20 7061  T') for name, pa
+00005c80: 7474 6572 6e73 2069 6e20 5f76 705f 7275  tterns in _vp_ru
+00005c90: 6c65 732e 6974 656d 7328 2920 5d0a 0923  les.items() ]..#
+00005ca0: 7265 7475 726e 205b 2873 7061 6379 2e6e  return [(spacy.n
+00005cb0: 6c70 2e76 6f63 6162 5b6e 616d 655d 2e74  lp.vocab[name].t
+00005cc0: 6578 742c 2076 705f 7370 616e 2864 6f63  ext, vp_span(doc
+00005cd0: 2c69 6265 672c 6965 6e64 292c 2069 6265  ,ibeg,iend), ibe
+00005ce0: 672c 2069 656e 6429 2066 6f72 206e 616d  g, iend) for nam
+00005cf0: 652c 2069 6265 672c 6965 6e64 2069 6e20  e, ibeg,iend in 
+00005d00: 7670 5f6d 6174 6368 6572 2e6d 6174 6368  vp_matcher.match
+00005d10: 6572 2864 6f63 295d 200a 0974 7570 7320  er(doc)] ..tups 
+00005d20: 3d20 7365 7428 2920 2023 2072 656d 6f76  = set()  # remov
+00005d30: 6520 7468 6520 6475 706c 6963 6174 6564  e the duplicated
+00005d40: 2065 6e74 7269 6573 200a 095b 7475 7073   entries ..[tups
+00005d50: 2e61 6464 2828 7370 6163 792e 6e6c 702e  .add((spacy.nlp.
+00005d60: 766f 6361 625b 6e61 6d65 5d2e 7465 7874  vocab[name].text
+00005d70: 2c20 7670 5f73 7061 6e28 646f 632c 6962  , vp_span(doc,ib
+00005d80: 6567 2c69 656e 6429 2c20 6962 6567 2c20  eg,iend), ibeg, 
+00005d90: 6965 6e64 2929 2066 6f72 206e 616d 652c  iend)) for name,
+00005da0: 2069 6265 672c 6965 6e64 2069 6e20 7670   ibeg,iend in vp
+00005db0: 5f6d 6174 6368 6572 2e6d 6174 6368 6572  _matcher.matcher
+00005dc0: 2864 6f63 295d 200a 0972 6574 7572 6e20  (doc)] ..return 
+00005dd0: 7475 7073 0a0a 5f64 6570 5f72 756c 6573  tups.._dep_rules
+00005de0: 203d 207b 0a22 7376 6f22 3a5b 207b 2252   = {."svo":[ {"R
+00005df0: 4947 4854 5f49 4422 3a20 2276 222c 2020  IGHT_ID": "v",  
+00005e00: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
+00005e10: 2250 4f53 223a 2022 5645 5242 227d 7d2c  "POS": "VERB"}},
+00005e20: 207b 224c 4546 545f 4944 223a 2022 7622   {"LEFT_ID": "v"
+00005e30: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
+00005e40: 2022 5249 4748 545f 4944 223a 2022 7375   "RIGHT_ID": "su
+00005e50: 626a 6563 7422 2c20 2252 4947 4854 5f41  bject", "RIGHT_A
+00005e60: 5454 5253 223a 207b 2244 4550 223a 2022  TTRS": {"DEP": "
+00005e70: 6e73 7562 6a22 7d7d 2c7b 224c 4546 545f  nsubj"}},{"LEFT_
+00005e80: 4944 223a 2022 7622 2c20 2252 454c 5f4f  ID": "v", "REL_O
+00005e90: 5022 3a20 223e 222c 2022 5249 4748 545f  P": ">", "RIGHT_
+00005ea0: 4944 223a 2022 6f62 6a65 6374 222c 2252  ID": "object","R
+00005eb0: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
+00005ec0: 4550 223a 2022 646f 626a 227d 2020 7d5d  EP": "dobj"}  }]
+00005ed0: 2c20 2320 5b28 3438 3531 3336 3331 3232  , # [(4851363122
+00005ee0: 3936 3236 3734 3137 362c 205b 322c 2030  962674176, [2, 0
+00005ef0: 2c20 345d 295d 0a22 7376 6122 3a5b 207b  , 4])]."sva":[ {
+00005f00: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
+00005f10: 2020 2252 4947 4854 5f41 5454 5253 223a    "RIGHT_ATTRS":
+00005f20: 207b 2250 4f53 223a 2022 5645 5242 227d   {"POS": "VERB"}
+00005f30: 7d2c 207b 224c 4546 545f 4944 223a 2022  }, {"LEFT_ID": "
+00005f40: 7622 2c20 2252 454c 5f4f 5022 3a20 223e  v", "REL_OP": ">
+00005f50: 222c 2022 5249 4748 545f 4944 223a 2022  ", "RIGHT_ID": "
+00005f60: 7375 626a 6563 7422 2c20 2252 4947 4854  subject", "RIGHT
+00005f70: 5f41 5454 5253 223a 207b 2244 4550 223a  _ATTRS": {"DEP":
+00005f80: 2022 6e73 7562 6a22 7d7d 2c7b 224c 4546   "nsubj"}},{"LEF
+00005f90: 545f 4944 223a 2022 7622 2c20 2252 454c  T_ID": "v", "REL
+00005fa0: 5f4f 5022 3a20 223e 222c 2022 5249 4748  _OP": ">", "RIGH
+00005fb0: 545f 4944 223a 2022 6f62 6a65 6374 222c  T_ID": "object",
+00005fc0: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
+00005fd0: 2244 4550 223a 2022 6163 6f6d 7022 7d7d  "DEP": "acomp"}}
+00005fe0: 5d2c 200a 2320 706c 616e 2074 6f20 676f  ], .# plan to go
+00005ff0: 202c 2065 6e6a 6f79 2073 7769 6d6d 696e   , enjoy swimmin
+00006000: 6720 0a22 7376 7822 3a5b 207b 2252 4947  g ."svx":[ {"RIG
+00006010: 4854 5f49 4422 3a20 2276 222c 2022 5249  HT_ID": "v", "RI
+00006020: 4748 545f 4154 5452 5322 3a20 7b22 504f  GHT_ATTRS": {"PO
+00006030: 5322 3a20 2256 4552 4222 7d7d 2c20 7b22  S": "VERB"}}, {"
+00006040: 4c45 4654 5f49 4422 3a20 2276 222c 2022  LEFT_ID": "v", "
+00006050: 5245 4c5f 4f50 223a 2022 3e22 2c20 2252  REL_OP": ">", "R
+00006060: 4947 4854 5f49 4422 3a20 2273 7562 6a65  IGHT_ID": "subje
+00006070: 6374 222c 2022 5249 4748 545f 4154 5452  ct", "RIGHT_ATTR
+00006080: 5322 3a20 7b22 4445 5022 3a20 226e 7375  S": {"DEP": "nsu
+00006090: 626a 227d 7d2c 207b 224c 4546 545f 4944  bj"}}, {"LEFT_ID
+000060a0: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
+000060b0: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
+000060c0: 223a 2022 6f62 6a65 6374 222c 2252 4947  ": "object","RIG
+000060d0: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
+000060e0: 223a 2022 7863 6f6d 7022 7d7d 5d2c 200a  ": "xcomp"}}], .
+000060f0: 2320 4920 7468 696e 6b20 6974 2069 7320  # I think it is 
+00006100: 7269 6768 742e 0a22 7376 6322 3a5b 207b  right.."svc":[ {
+00006110: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
+00006120: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
+00006130: 2250 4f53 223a 2022 5645 5242 227d 7d2c  "POS": "VERB"}},
+00006140: 207b 224c 4546 545f 4944 223a 2022 7622   {"LEFT_ID": "v"
+00006150: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
+00006160: 2022 5249 4748 545f 4944 223a 2022 7375   "RIGHT_ID": "su
+00006170: 626a 6563 7422 2c20 2252 4947 4854 5f41  bject", "RIGHT_A
+00006180: 5454 5253 223a 207b 2244 4550 223a 2022  TTRS": {"DEP": "
+00006190: 6e73 7562 6a22 7d7d 2c20 7b22 4c45 4654  nsubj"}}, {"LEFT
+000061a0: 5f49 4422 3a20 2276 222c 2022 5245 4c5f  _ID": "v", "REL_
+000061b0: 4f50 223a 2022 3e22 2c20 2252 4947 4854  OP": ">", "RIGHT
+000061c0: 5f49 4422 3a20 226f 626a 6563 7422 2c20  _ID": "object", 
+000061d0: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
+000061e0: 2244 4550 223a 2022 6363 6f6d 7022 7d7d  "DEP": "ccomp"}}
+000061f0: 5d2c 200a 2353 6865 2069 7320 2061 2067  ], .#She is  a g
+00006200: 6972 6c2e 0a22 7361 7474 7222 3a5b 207b  irl.."sattr":[ {
+00006210: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
+00006220: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
+00006230: 7b22 4c45 4d4d 4122 3a20 2262 6522 7d7d  {"LEMMA": "be"}}
+00006240: 2c20 7b22 4c45 4654 5f49 4422 3a20 2276  , {"LEFT_ID": "v
+00006250: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
+00006260: 2c20 2252 4947 4854 5f49 4422 3a20 2273  , "RIGHT_ID": "s
+00006270: 7562 6a65 6374 222c 2252 4947 4854 5f41  ubject","RIGHT_A
+00006280: 5454 5253 223a 207b 2244 4550 223a 2022  TTRS": {"DEP": "
+00006290: 6e73 7562 6a22 7d7d 2c7b 224c 4546 545f  nsubj"}},{"LEFT_
+000062a0: 4944 223a 2022 7622 2c22 5245 4c5f 4f50  ID": "v","REL_OP
+000062b0: 223a 2022 3e22 2c20 2252 4947 4854 5f49  ": ">", "RIGHT_I
+000062c0: 4422 3a20 226f 626a 6563 7422 2c22 5249  D": "object","RI
+000062d0: 4748 545f 4154 5452 5322 3a20 7b22 4445  GHT_ATTRS": {"DE
+000062e0: 5022 3a20 2261 7474 7222 7d20 207d 5d2c  P": "attr"}  }],
+000062f0: 200a 2320 7475 726e 206f 6666 2074 6865   .# turn off the
+00006300: 206c 6967 6874 0a22 7670 6e22 3a5b 207b   light."vpn":[ {
+00006310: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
+00006320: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
+00006330: 7b22 504f 5322 3a20 2256 4552 4222 7d7d  {"POS": "VERB"}}
+00006340: 2c20 7b22 4c45 4654 5f49 4422 3a20 2276  , {"LEFT_ID": "v
+00006350: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
+00006360: 2c20 2252 4947 4854 5f49 4422 3a20 2273  , "RIGHT_ID": "s
+00006370: 7562 6a65 6374 222c 2022 5249 4748 545f  ubject", "RIGHT_
+00006380: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
+00006390: 2270 7274 227d 7d2c 207b 224c 4546 545f  "prt"}}, {"LEFT_
+000063a0: 4944 223a 2022 7622 2c20 2252 454c 5f4f  ID": "v", "REL_O
+000063b0: 5022 3a20 223e 222c 2252 4947 4854 5f49  P": ">","RIGHT_I
+000063c0: 4422 3a20 226f 626a 6563 7422 2c22 5249  D": "object","RI
+000063d0: 4748 545f 4154 5452 5322 3a20 7b22 4445  GHT_ATTRS": {"DE
+000063e0: 5022 3a20 2264 6f62 6a22 7d20 7d5d 2c20  P": "dobj"} }], 
+000063f0: 0a23 2062 6520 6861 7070 7920 7769 7468  .# be happy with
+00006400: 0a22 7661 7022 3a5b 207b 2252 4947 4854  ."vap":[ {"RIGHT
+00006410: 5f49 4422 3a20 2276 222c 2022 5249 4748  _ID": "v", "RIGH
+00006420: 545f 4154 5452 5322 3a20 7b22 504f 5322  T_ATTRS": {"POS"
+00006430: 3a20 2256 4552 4222 7d7d 2c20 7b22 4c45  : "VERB"}}, {"LE
+00006440: 4654 5f49 4422 3a20 2276 222c 2022 5245  FT_ID": "v", "RE
+00006450: 4c5f 4f50 223a 2022 3e22 2c20 2252 4947  L_OP": ">", "RIG
+00006460: 4854 5f49 4422 3a20 2261 636f 6d70 222c  HT_ID": "acomp",
+00006470: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
+00006480: 2244 4550 223a 2022 6163 6f6d 7022 7d7d  "DEP": "acomp"}}
+00006490: 2c7b 224c 4546 545f 4944 223a 2022 6163  ,{"LEFT_ID": "ac
+000064a0: 6f6d 7022 2c20 2252 454c 5f4f 5022 3a20  omp", "REL_OP": 
+000064b0: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
+000064c0: 2022 7072 6570 222c 2022 5249 4748 545f   "prep", "RIGHT_
+000064d0: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
+000064e0: 2270 7265 7022 7d20 7d5d 2c20 0a23 2062  "prep"} }], .# b
+000064f0: 6520 6261 7365 6420 6f6e 0a22 7664 7022  e based on."vdp"
+00006500: 3a5b 207b 2252 4947 4854 5f49 4422 3a20  :[ {"RIGHT_ID": 
+00006510: 2276 222c 2022 5249 4748 545f 4154 5452  "v", "RIGHT_ATTR
+00006520: 5322 3a20 7b22 5441 4722 3a20 2256 424e  S": {"TAG": "VBN
+00006530: 227d 7d2c 207b 224c 4546 545f 4944 223a  "}}, {"LEFT_ID":
+00006540: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
+00006550: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
+00006560: 2022 6265 222c 2022 5249 4748 545f 4154   "be", "RIGHT_AT
+00006570: 5452 5322 3a20 7b22 4c45 4d4d 4122 3a20  TRS": {"LEMMA": 
+00006580: 2262 6522 7d7d 2c7b 224c 4546 545f 4944  "be"}},{"LEFT_ID
+00006590: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
+000065a0: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
+000065b0: 223a 2022 7072 6570 222c 2022 5249 4748  ": "prep", "RIGH
+000065c0: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
+000065d0: 3a20 2270 7265 7022 7d7d 5d2c 200a 2320  : "prep"}}], .# 
+000065e0: 6c6f 6f6b 2075 7020 6672 6f6d 2070 686f  look up from pho
+000065f0: 6e65 0a22 7670 706e 223a 5b20 7b22 5249  ne."vppn":[ {"RI
+00006600: 4748 545f 4944 223a 2022 7622 2c20 2252  GHT_ID": "v", "R
+00006610: 4947 4854 5f41 5454 5253 223a 207b 2250  IGHT_ATTRS": {"P
+00006620: 4f53 223a 2022 5645 5242 227d 7d2c 207b  OS": "VERB"}}, {
+00006630: 2022 4c45 4654 5f49 4422 3a20 2276 222c   "LEFT_ID": "v",
+00006640: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
+00006650: 5249 4748 545f 4944 223a 2022 7072 7422  RIGHT_ID": "prt"
+00006660: 2c20 2252 4947 4854 5f41 5454 5253 223a  , "RIGHT_ATTRS":
+00006670: 207b 2244 4550 223a 2022 7072 7422 7d7d   {"DEP": "prt"}}
 00006680: 2c7b 224c 4546 545f 4944 223a 2022 7622  ,{"LEFT_ID": "v"
 00006690: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
 000066a0: 2022 5249 4748 545f 4944 223a 2022 7072   "RIGHT_ID": "pr
-000066b0: 6570 3222 2c20 2252 4947 4854 5f41 5454  ep2", "RIGHT_ATT
-000066c0: 5253 223a 207b 2244 4550 223a 2022 7072  RS": {"DEP": "pr
-000066d0: 6570 227d 7d2c 7b22 4c45 4654 5f49 4422  ep"}},{"LEFT_ID"
-000066e0: 3a20 2270 7265 7032 222c 2022 5245 4c5f  : "prep2", "REL_
-000066f0: 4f50 223a 2022 3e22 2c20 2252 4947 4854  OP": ">", "RIGHT
-00006700: 5f49 4422 3a20 226f 626a 6563 7432 222c  _ID": "object2",
-00006710: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
-00006720: 7b22 4445 5022 3a20 2270 6f62 6a22 7d7d  {"DEP": "pobj"}}
-00006730: 5d2c 200a 2320 7475 726e 2069 7420 646f  ], .# turn it do
-00006740: 776e 0a22 766e 7022 3a5b 207b 2022 5249  wn."vnp":[ { "RI
-00006750: 4748 545f 4944 223a 2022 7622 2c22 5249  GHT_ID": "v","RI
-00006760: 4748 545f 4154 5452 5322 3a20 7b22 504f  GHT_ATTRS": {"PO
-00006770: 5322 3a20 2256 4552 4222 7d7d 2c7b 224c  S": "VERB"}},{"L
-00006780: 4546 545f 4944 223a 2022 7622 2c22 5245  EFT_ID": "v","RE
-00006790: 4c5f 4f50 223a 2022 3e22 2c22 5249 4748  L_OP": ">","RIGH
-000067a0: 545f 4944 223a 2022 6f62 6a65 6374 222c  T_ID": "object",
-000067b0: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
-000067c0: 7b22 4445 5022 3a20 2264 6f62 6a22 7d7d  {"DEP": "dobj"}}
-000067d0: 2c7b 224c 4546 545f 4944 223a 2022 7622  ,{"LEFT_ID": "v"
-000067e0: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
-000067f0: 2252 4947 4854 5f49 4422 3a20 2273 7562  "RIGHT_ID": "sub
-00006800: 6a65 6374 222c 2022 5249 4748 545f 4154  ject", "RIGHT_AT
-00006810: 5452 5322 3a20 7b22 4445 5022 3a20 2270  TRS": {"DEP": "p
-00006820: 7274 227d 7d5d 2c20 0a23 206d 616b 6520  rt"}}], .# make 
-00006830: 7573 6520 6f66 2062 6f6f 6b73 2c20 7461  use of books, ta
-00006840: 6b65 2073 7468 2069 6e74 6f20 6163 636f  ke sth into acco
-00006850: 756e 740a 2276 6e70 6e22 3a5b 207b 2252  unt."vnpn":[ {"R
-00006860: 4947 4854 5f49 4422 3a20 2276 222c 2022  IGHT_ID": "v", "
-00006870: 5249 4748 545f 4154 5452 5322 3a20 7b22  RIGHT_ATTRS": {"
-00006880: 504f 5322 3a20 2256 4552 4222 7d7d 2c7b  POS": "VERB"}},{
-00006890: 224c 4546 545f 4944 223a 2022 7622 2c20  "LEFT_ID": "v", 
-000068a0: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
-000068b0: 5249 4748 545f 4944 223a 2022 6f62 6a65  RIGHT_ID": "obje
-000068c0: 6374 222c 2252 4947 4854 5f41 5454 5253  ct","RIGHT_ATTRS
-000068d0: 223a 207b 2244 4550 223a 2022 646f 626a  ": {"DEP": "dobj
-000068e0: 227d 7d2c 7b22 4c45 4654 5f49 4422 3a20  "}},{"LEFT_ID": 
-000068f0: 226f 626a 6563 7422 2c22 5245 4c5f 4f50  "object","REL_OP
-00006900: 223a 2022 3e22 2c20 2252 4947 4854 5f49  ": ">", "RIGHT_I
-00006910: 4422 3a20 2270 7265 7022 2c20 2252 4947  D": "prep", "RIG
-00006920: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
-00006930: 223a 2022 7072 6570 227d 7d2c 7b22 4c45  ": "prep"}},{"LE
-00006940: 4654 5f49 4422 3a20 2270 7265 7022 2c20  FT_ID": "prep", 
-00006950: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
-00006960: 5249 4748 545f 4944 223a 2022 706f 626a  RIGHT_ID": "pobj
-00006970: 222c 2022 5249 4748 545f 4154 5452 5322  ", "RIGHT_ATTRS"
-00006980: 3a20 7b22 4445 5022 3a20 2270 6f62 6a22  : {"DEP": "pobj"
-00006990: 7d7d 2020 5d2c 200a 7d20 2320 666f 7220  }}  ], .} # for 
-000069a0: 6e61 6d65 2c20 6172 2069 6e20 6465 706d  name, ar in depm
-000069b0: 6174 6368 6572 735b 2773 7678 275d 2864  atchers['svx'](d
-000069c0: 6f63 2920 3a20 7072 696e 7428 646f 635b  oc) : print(doc[
-000069d0: 6172 5b31 5d5d 2c20 646f 635b 6172 5b30  ar[1]], doc[ar[0
-000069e0: 5d5d 2c20 646f 635b 6172 5b32 5d5d 290a  ]], doc[ar[2]]).
-000069f0: 0a64 6566 2064 6570 5f6d 6174 6368 6572  .def dep_matcher
-00006a00: 2864 6f63 293a 2023 5b28 2773 7678 272c  (doc): #[('svx',
-00006a10: 205b 312c 2030 2c20 325d 295d 0a09 6966   [1, 0, 2])]..if
-00006a20: 206e 6f74 2068 6173 6174 7472 2864 6570   not hasattr(dep
-00006a30: 5f6d 6174 6368 6572 2c20 276d 6174 6368  _matcher, 'match
-00006a40: 6572 2729 3a20 0a09 0964 6570 5f6d 6174  er'): ...dep_mat
-00006a50: 6368 6572 2e6d 6174 6368 6572 203d 2044  cher.matcher = D
-00006a60: 6570 656e 6465 6e63 794d 6174 6368 6572  ependencyMatcher
-00006a70: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
-00006a80: 290a 0909 5b64 6570 5f6d 6174 6368 6572  )...[dep_matcher
-00006a90: 2e6d 6174 6368 6572 2e61 6464 286e 616d  .matcher.add(nam
-00006aa0: 652c 205b 7061 7474 6572 6e5d 2920 666f  e, [pattern]) fo
-00006ab0: 7220 6e61 6d65 2c20 7061 7474 6572 6e20  r name, pattern 
-00006ac0: 696e 205f 6465 705f 7275 6c65 732e 6974  in _dep_rules.it
-00006ad0: 656d 7328 2920 5d0a 0972 6574 7572 6e20  ems() ]..return 
-00006ae0: 5b28 7370 6163 792e 6e6c 702e 766f 6361  [(spacy.nlp.voca
-00006af0: 625b 6e61 6d65 5d2e 7465 7874 2c20 6172  b[name].text, ar
-00006b00: 2920 666f 7220 6e61 6d65 2c20 6172 2069  ) for name, ar i
-00006b10: 6e20 6465 705f 6d61 7463 6865 722e 6d61  n dep_matcher.ma
-00006b20: 7463 6865 7228 646f 6329 5d20 0a09 2366  tcher(doc)] ..#f
-00006b30: 6f72 206e 616d 652c 2061 7220 696e 2064  or name, ar in d
-00006b40: 6570 6d61 7463 6865 7273 5b27 7376 7827  epmatchers['svx'
-00006b50: 5d28 646f 6329 203a 2070 7269 6e74 2864  ](doc) : print(d
-00006b60: 6f63 5b61 725b 315d 5d2c 2064 6f63 5b61  oc[ar[1]], doc[a
-00006b70: 725b 305d 5d2c 2064 6f63 5b61 725b 325d  r[0]], doc[ar[2]
-00006b80: 5d29 0a0a 6573 5f74 6f6b 7320 3d20 6c61  ])..es_toks = la
-00006b90: 6d62 6461 2073 6964 2c20 646f 633a 2020  mbda sid, doc:  
-00006ba0: 5b20 7b27 5f69 6427 3a20 6622 7b73 6964  [ {'_id': f"{sid
-00006bb0: 7d2d 746f 6b2d 7b74 2e69 7d22 2c20 275f  }-tok-{t.i}", '_
-00006bc0: 736f 7572 6365 273a 207b 2274 7970 6522  source': {"type"
-00006bd0: 3a22 746f 6b22 2c20 2273 7263 223a 7369  :"tok", "src":si
-00006be0: 642c 2027 6927 3a74 2e69 2c20 2268 6561  d, 'i':t.i, "hea
-00006bf0: 6422 3a74 2e68 6561 642e 692c 2027 6c65  d":t.head.i, 'le
-00006c00: 7827 3a74 2e74 6578 742c 2027 6c65 6d27  x':t.text, 'lem'
-00006c10: 3a74 2e6c 656d 6d61 5f2c 2027 706f 7327  :t.lemma_, 'pos'
-00006c20: 3a74 2e70 6f73 5f2c 2027 7461 6727 3a74  :t.pos_, 'tag':t
-00006c30: 2e74 6167 5f2c 2027 6465 7027 3a74 2e64  .tag_, 'dep':t.d
-00006c40: 6570 5f2c 2022 6770 6f73 223a 742e 6865  ep_, "gpos":t.he
-00006c50: 6164 2e70 6f73 5f2c 2022 676c 656d 223a  ad.pos_, "glem":
-00006c60: 742e 6865 6164 2e6c 656d 6d61 5f20 7d20  t.head.lemma_ } 
-00006c70: 7d20 666f 7220 7420 696e 2064 6f63 205d  } for t in doc ]
-00006c80: 200a 6465 6620 6573 5f70 6f73 7461 6728   .def es_postag(
-00006c90: 646f 6329 3a20 0a09 6672 6f6d 2064 6963  doc): ..from dic
-00006ca0: 2e6f 6e65 7365 6c66 2069 6d70 6f72 7420  .oneself import 
-00006cb0: 6f6e 6573 656c 6620 0a09 7265 7475 726e  oneself ..return
-00006cc0: 2022 5f5e 2022 202b 2027 2027 2e6a 6f69   "_^ " + ' '.joi
-00006cd0: 6e28 5b20 6622 7b74 2e74 6578 747d 5f7b  n([ f"{t.text}_{
-00006ce0: 742e 706f 735f 7d5f 7b74 2e74 6167 5f7d  t.pos_}_{t.tag_}
-00006cf0: 2220 6966 2074 2e70 6f73 5f20 696e 2028  " if t.pos_ in (
-00006d00: 2750 524f 504e 272c 274e 554d 272c 2758  'PROPN','NUM','X
-00006d10: 272c 2753 5041 4345 272c 2750 554e 4354  ','SPACE','PUNCT
-00006d20: 2729 2065 6c73 6520 6622 7b74 2e74 6578  ') else f"{t.tex
-00006d30: 747d 5f7b 742e 6c65 6d6d 615f 7d5f 7b74  t}_{t.lemma_}_{t
-00006d40: 2e70 6f73 5f7d 5f7b 742e 7461 675f 7d7b  .pos_}_{t.tag_}{
-00006d50: 6f6e 6573 656c 662e 6765 7428 742e 7465  oneself.get(t.te
-00006d60: 7874 2e6c 6f77 6572 2829 2c20 2727 297d  xt.lower(), '')}
-00006d70: 2220 2066 6f72 2074 2069 6e20 646f 635d  "  for t in doc]
-00006d80: 2920 2320 756e 6971 2062 7920 616e 6120  ) # uniq by ana 
-00006d90: 232c 2750 554e 4354 270a 6465 6620 6573  #,'PUNCT'.def es
-00006da0: 5f68 7962 2864 6f63 293a 200a 0966 726f  _hyb(doc): ..fro
-00006db0: 6d20 6469 632e 6f6e 6573 656c 6620 696d  m dic.oneself im
-00006dc0: 706f 7274 206f 6e65 7365 6c66 200a 0961  port oneself ..a
-00006dd0: 7272 203d 205b 2066 227b 742e 7465 7874  rr = [ f"{t.text
-00006de0: 7d5f 7b74 2e70 6f73 5f7d 5f7b 742e 7461  }_{t.pos_}_{t.ta
-00006df0: 675f 7d22 2069 6620 742e 706f 735f 2069  g_}" if t.pos_ i
-00006e00: 6e20 2827 5052 4f50 4e27 2c27 4e55 4d27  n ('PROPN','NUM'
-00006e10: 2c27 5827 2c27 5350 4143 4527 2c27 5055  ,'X','SPACE','PU
-00006e20: 4e43 5427 2920 656c 7365 2066 227b 742e  NCT') else f"{t.
-00006e30: 7465 7874 7d5f 7b74 2e6c 656d 6d61 5f7d  text}_{t.lemma_}
-00006e40: 5f7b 742e 706f 735f 7d5f 7b74 2e74 6167  _{t.pos_}_{t.tag
-00006e50: 5f7d 7b6f 6e65 7365 6c66 2e67 6574 2874  _}{oneself.get(t
-00006e60: 2e74 6578 742e 6c6f 7765 7228 292c 2027  .text.lower(), '
-00006e70: 2729 7d22 2020 666f 7220 7420 696e 2064  ')}"  for t in d
-00006e80: 6f63 5d0a 0972 6574 7572 6e20 225f 5e20  oc]..return "_^ 
-00006e90: 2220 2b20 2720 272e 6a6f 696e 2820 5b73  " + ' '.join( [s
-00006ea0: 2069 6620 275f 5055 4e43 5427 2069 6e20   if '_PUNCT' in 
-00006eb0: 7320 656c 7365 2066 227b 737d 5f2a 2220  s else f"{s}_*" 
-00006ec0: 666f 7220 7320 696e 2061 7272 5d29 2023  for s in arr]) #
-00006ed0: 2073 7570 706f 7274 203a 2020 6120 5f2a   support :  a _*
-00006ee0: 2062 6f6f 6b20 7c20 6120 5f2a 205f 2a20   book | a _* _* 
-00006ef0: 626f 6f6b 0a0a 2320 6164 6465 6420 3230  book..# added 20
-00006f00: 3233 2e31 2e31 362c 206e 6f74 2074 6573  23.1.16, not tes
-00006f10: 7465 6420 7965 740a 636c 5f72 6f6f 7420  ted yet.cl_root 
-00006f20: 3d20 6c61 6d62 6461 2074 3a20 742e 6465  = lambda t: t.de
-00006f30: 705f 2021 3d20 2752 4f4f 5427 2061 6e64  p_ != 'ROOT' and
-00006f40: 2028 2028 742e 706f 735f 203d 3d20 2756   ( (t.pos_ == 'V
-00006f50: 4552 4227 2061 6e64 2074 2e74 6167 5f20  ERB' and t.tag_ 
-00006f60: 213d 2027 5642 4e27 2920 206f 7220 2874  != 'VBN')  or (t
-00006f70: 2e70 6f73 5f20 3d3d 2027 4155 5827 2061  .pos_ == 'AUX' a
-00006f80: 6e64 2074 2e6c 656d 6d61 5f20 3d3d 2027  nd t.lemma_ == '
-00006f90: 6265 2729 2029 0a64 6566 206d 6172 6b5f  be') ).def mark_
-00006fa0: 636c 2864 6f63 293a 0a20 2020 2066 6f72  cl(doc):.    for
-00006fb0: 2074 2069 6e20 646f 633a 200a 2020 2020   t in doc: .    
-00006fc0: 2020 2020 6966 2063 6c5f 726f 6f74 2874      if cl_root(t
-00006fd0: 2920 3a20 742e 656e 745f 6964 5f20 3d20  ) : t.ent_id_ = 
-00006fe0: 2763 6c5f 726f 6f74 270a 6c65 6176 655f  'cl_root'.leave_
-00006ff0: 636c 203d 206c 616d 6264 6120 743a 2063  cl = lambda t: c
-00007000: 6c5f 726f 6f74 2874 2920 616e 6420 6c65  l_root(t) and le
-00007010: 6e28 5b74 7220 666f 7220 7472 2069 6e20  n([tr for tr in 
-00007020: 742e 7375 6274 7265 6520 6966 2074 722e  t.subtree if tr.
-00007030: 656e 745f 6964 5f20 3d3d 2027 636c 5f72  ent_id_ == 'cl_r
-00007040: 6f6f 7427 5d29 203d 3d20 310a 6465 6620  oot']) == 1.def 
-00007050: 6d65 7267 655f 6c65 6176 655f 636c 2864  merge_leave_cl(d
-00007060: 6f63 293a 2023 646f 6320 3d20 7370 6163  oc): #doc = spac
-00007070: 792e 6e6c 7028 2257 6869 6c65 2049 2077  y.nlp("While I w
-00007080: 6173 2074 6872 696c 6c65 6420 7468 6174  as thrilled that
-00007090: 2069 7420 7761 7320 6f6b 2c20 4920 776f   it was ok, I wo
-000070a0: 7272 6965 6420 7468 6174 2049 2077 6f75  rried that I wou
-000070b0: 6c64 2066 6169 6c2e 2229 0a09 6d61 726b  ld fail.")..mark
-000070c0: 5f63 6c28 646f 6329 0a09 7769 7468 2064  _cl(doc)..with d
-000070d0: 6f63 2e72 6574 6f6b 656e 697a 6528 2920  oc.retokenize() 
-000070e0: 6173 2072 6574 6f6b 656e 697a 6572 3a0a  as retokenizer:.
-000070f0: 0909 666f 7220 7620 696e 205b 7420 666f  ..for v in [t fo
-00007100: 7220 7420 696e 2064 6f63 2069 6620 6c65  r t in doc if le
-00007110: 6176 655f 636c 2874 2920 5d20 3a20 2320  ave_cl(t) ] : # 
-00007120: 6e6f 6e2d 726f 6f74 0a09 0909 7472 793a  non-root....try:
-00007130: 0a09 0909 0963 6869 6c64 7265 6e20 3d20  .....children = 
-00007140: 6c69 7374 2876 2e73 7562 7472 6565 290a  list(v.subtree).
-00007150: 0909 0909 7374 6172 7420 3d20 6368 696c  ....start = chil
-00007160: 6472 656e 5b30 5d2e 6920 2009 0a09 0909  dren[0].i  .....
-00007170: 0965 6e64 203d 2063 6869 6c64 7265 6e5b  .end = children[
-00007180: 2d31 5d2e 6920 0a09 0909 0961 7474 7273  -1].i .....attrs
-00007190: 203d 207b 2270 6f73 223a 2076 2e70 6f73   = {"pos": v.pos
-000071a0: 2c20 2274 6167 223a 2076 2e74 6167 2c20  , "tag": v.tag, 
-000071b0: 2264 6570 223a 2076 2e64 6570 2c20 226c  "dep": v.dep, "l
-000071c0: 656d 6d61 223a 762e 6c65 6d6d 612c 2022  emma":v.lemma, "
-000071d0: 656e 745f 7479 7065 223a 2022 532e 2220  ent_type": "S." 
-000071e0: 2b20 762e 6465 705f 207d 2023 2053 2e61  + v.dep_ } # S.a
-000071f0: 6476 636c 202c 2020 532e 636f 6e6a 200a  dvcl ,  S.conj .
-00007200: 0909 0909 6966 2076 2e64 6570 5f20 6e6f  ....if v.dep_ no
-00007210: 7420 696e 2028 2778 636f 6d70 2729 2061  t in ('xcomp') a
-00007220: 6e64 2064 6f63 5b73 7461 7274 5d2e 6c65  nd doc[start].le
-00007230: 6d6d 615f 206e 6f74 2069 6e20 2827 746f  mma_ not in ('to
-00007240: 2729 2061 6e64 2064 6f63 5b73 7461 7274  ') and doc[start
-00007250: 5d2e 7461 675f 206e 6f74 2069 6e20 2827  ].tag_ not in ('
-00007260: 544f 2729 3a20 2320 736b 6970 2074 6f2d  TO'): # skip to-
-00007270: 636c 6175 7365 2020 7c20 4865 206d 6164  clause  | He mad
-00007280: 6520 7468 6520 6368 6f69 6365 2074 6f20  e the choice to 
-00007290: 6769 7665 2061 6c6c 2068 6973 206d 6f6e  give all his mon
-000072a0: 6579 2061 7761 7920 2e0a 0909 0909 0972  ey away .......r
-000072b0: 6574 6f6b 656e 697a 6572 2e6d 6572 6765  etokenizer.merge
-000072c0: 2864 6f63 5b73 7461 7274 203a 2065 6e64  (doc[start : end
-000072d0: 2b31 5d2c 2061 7474 7273 3d61 7474 7273  +1], attrs=attrs
-000072e0: 290a 0909 0965 7863 6570 7420 4578 6365  )....except Exce
-000072f0: 7074 696f 6e20 6173 2065 3a0a 0909 0909  ption as e:.....
-00007300: 7072 696e 7420 2820 226d 6572 6765 5f6c  print ( "merge_l
-00007310: 6561 7665 5f63 6c20 6578 3a22 2c20 652c  eave_cl ex:", e,
-00007320: 2076 2029 0a09 7265 7475 726e 2064 6f63   v )..return doc
-00007330: 200a 0a64 6566 206d 6572 6765 5f63 636f   ..def merge_cco
-00007340: 6d70 2864 6f63 293a 2023 646f 6320 3d20  mp(doc): #doc = 
-00007350: 7370 6163 792e 6e6c 7028 2257 6869 6c65  spacy.nlp("While
-00007360: 2049 2077 6173 2074 6872 696c 6c65 6420   I was thrilled 
-00007370: 7468 6174 2069 7420 7761 7320 6f6b 2c20  that it was ok, 
-00007380: 4920 776f 7272 6965 6420 7468 6174 2049  I worried that I
-00007390: 2077 6f75 6c64 2066 6169 6c2e 2229 0a09   would fail.")..
-000073a0: 7769 7468 2064 6f63 2e72 6574 6f6b 656e  with doc.retoken
-000073b0: 697a 6528 2920 6173 2072 6574 6f6b 656e  ize() as retoken
-000073c0: 697a 6572 3a0a 0909 666f 7220 7620 696e  izer:...for v in
-000073d0: 205b 7420 666f 7220 7420 696e 2064 6f63   [t for t in doc
-000073e0: 2069 6620 742e 706f 735f 203d 3d20 2756   if t.pos_ == 'V
-000073f0: 4552 4227 2061 6e64 2074 2e64 6570 5f20  ERB' and t.dep_ 
-00007400: 3d3d 2027 6363 6f6d 7027 2061 6e64 2074  == 'ccomp' and t
-00007410: 2e74 6167 5f20 6e6f 7420 696e 2028 2756  .tag_ not in ('V
-00007420: 424e 2729 205d 203a 2023 206e 6f6e 2d72  BN') ] : # non-r
-00007430: 6f6f 740a 0909 0974 7279 3a0a 0909 0909  oot....try:.....
-00007440: 6368 696c 6472 656e 203d 206c 6973 7428  children = list(
-00007450: 762e 7375 6274 7265 6529 0a09 0909 0973  v.subtree).....s
-00007460: 7461 7274 203d 2063 6869 6c64 7265 6e5b  tart = children[
-00007470: 305d 2e69 2020 090a 0909 0909 656e 6420  0].i  ......end 
-00007480: 3d20 6368 696c 6472 656e 5b2d 315d 2e69  = children[-1].i
-00007490: 200a 0909 0909 6174 7472 7320 3d20 7b22   .....attrs = {"
-000074a0: 706f 7322 3a20 762e 706f 732c 2022 7461  pos": v.pos, "ta
-000074b0: 6722 3a20 762e 7461 672c 2022 6465 7022  g": v.tag, "dep"
-000074c0: 3a20 762e 6465 702c 2022 6c65 6d6d 6122  : v.dep, "lemma"
-000074d0: 3a76 2e6c 656d 6d61 2c20 2265 6e74 5f74  :v.lemma, "ent_t
-000074e0: 7970 6522 3a20 2253 2e22 202b 2076 2e64  ype": "S." + v.d
-000074f0: 6570 5f20 7d20 2320 532e 6164 7663 6c20  ep_ } # S.advcl 
-00007500: 2c20 2053 2e63 6f6e 6a20 0a09 0909 0972  ,  S.conj .....r
-00007510: 6574 6f6b 656e 697a 6572 2e6d 6572 6765  etokenizer.merge
-00007520: 2864 6f63 5b73 7461 7274 203a 2065 6e64  (doc[start : end
-00007530: 2b31 5d2c 2061 7474 7273 3d61 7474 7273  +1], attrs=attrs
-00007540: 290a 0909 0965 7863 6570 7420 4578 6365  )....except Exce
-00007550: 7074 696f 6e20 6173 2065 3a0a 0909 0909  ption as e:.....
-00007560: 7072 696e 7420 2820 226d 6572 6765 5f63  print ( "merge_c
-00007570: 636f 6d70 2065 783a 222c 2065 2c20 7620  comp ex:", e, v 
-00007580: 290a 0972 6574 7572 6e20 646f 6320 0a0a  )..return doc ..
-00007590: 6465 6620 6174 7461 6368 5f63 6c28 646f  def attach_cl(do
-000075a0: 6329 3a20 2332 3032 332e 312e 3233 0a09  c): #2023.1.23..
-000075b0: 666f 7220 7620 696e 205b 7420 666f 7220  for v in [t for 
-000075c0: 7420 696e 2064 6f63 2069 6620 742e 706f  t in doc if t.po
-000075d0: 735f 203d 3d20 2756 4552 4227 5d20 3a20  s_ == 'VERB'] : 
-000075e0: 2320 6e6f 6e2d 726f 6f74 0a09 0974 7279  # non-root...try
-000075f0: 3a0a 0909 0963 6869 6c64 7265 6e20 3d20  :....children = 
-00007600: 6c69 7374 2876 2e73 7562 7472 6565 290a  list(v.subtree).
-00007610: 0909 0973 7461 7274 203d 2063 6869 6c64  ...start = child
-00007620: 7265 6e5b 305d 2e69 2020 090a 0909 0965  ren[0].i  .....e
-00007630: 6e64 203d 2063 6869 6c64 7265 6e5b 2d31  nd = children[-1
-00007640: 5d2e 6920 0a09 0909 636c 5f6c 656e 203d  ].i ....cl_len =
-00007650: 2065 6e64 202d 2073 7461 7274 202b 2031   end - start + 1
-00007660: 200a 0909 0964 6f63 5b73 7461 7274 5d2e   ....doc[start].
-00007670: 656e 745f 6964 5f20 3d20 6627 5f43 4c7b  ent_id_ = f'_CL{
-00007680: 762e 6465 705f 7d7b 636c 5f6c 656e 7d27  v.dep_}{cl_len}'
-00007690: 2020 2320 6164 6420 636c 5f72 6f6f 7420    # add cl_root 
-000076a0: 3f20 2320 532e 6164 7663 6c20 2c20 2053  ? # S.advcl ,  S
-000076b0: 2e63 6f6e 6a20 0a09 0965 7863 6570 7420  .conj ...except 
-000076c0: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
-000076d0: 0909 0970 7269 6e74 2028 2022 6174 7461  ...print ( "atta
-000076e0: 6368 5f63 6c20 6578 3a22 2c20 652c 2076  ch_cl ex:", e, v
-000076f0: 2029 0a09 7265 7475 726e 2064 6f63 200a   )..return doc .
-00007700: 0a64 6566 2073 6b65 6e70 5f74 6f6b 2874  .def skenp_tok(t
-00007710: 293a 200a 0966 726f 6d20 6469 632e 6f6e  ): ..from dic.on
-00007720: 6573 656c 6620 696d 706f 7274 206f 6e65  eself import one
-00007730: 7365 6c66 200a 0923 7061 6972 203d 2066  self ..#pair = f
-00007740: 225f 7b74 2e6c 656d 6d61 5f7d 5f4e 505f  "_{t.lemma_}_NP_
-00007750: 7b74 2e64 6570 5f7d 2220 6966 2074 2e65  {t.dep_}" if t.e
-00007760: 6e74 5f74 7970 655f 203d 3d20 274e 5027  nt_type_ == 'NP'
-00007770: 2065 6c73 6520 6622 5f7b 742e 706f 735f   else f"_{t.pos_
-00007780: 7d5f 7b74 2e74 6167 5f7d 5f7b 742e 6465  }_{t.tag_}_{t.de
-00007790: 705f 7d22 2069 6620 742e 706f 735f 2069  p_}" if t.pos_ i
-000077a0: 6e20 2827 5052 4f50 4e27 2c27 4e55 4d27  n ('PROPN','NUM'
-000077b0: 2c27 5827 2c27 5350 4143 4527 2c27 5055  ,'X','SPACE','PU
-000077c0: 4e43 5427 2920 656c 7365 2066 227b 742e  NCT') else f"{t.
-000077d0: 7465 7874 2069 6620 742e 7465 7874 2069  text if t.text i
-000077e0: 6e20 2827 4927 2920 656c 7365 2074 2e74  n ('I') else t.t
-000077f0: 6578 742e 6c6f 7765 7228 297d 5f7b 742e  ext.lower()}_{t.
-00007800: 6c65 6d6d 615f 7d5f 7b74 2e70 6f73 5f7d  lemma_}_{t.pos_}
-00007810: 5f7b 742e 7461 675f 7d7b 6f6e 6573 656c  _{t.tag_}{onesel
-00007820: 662e 6765 7428 742e 7465 7874 2e6c 6f77  f.get(t.text.low
-00007830: 6572 2829 2c20 2727 297d 5f7b 742e 6465  er(), '')}_{t.de
-00007840: 705f 7d22 0a09 7061 6972 203d 2066 225f  p_}"..pair = f"_
-00007850: 7b74 2e6c 656d 6d61 5f7d 5f7b 742e 706f  {t.lemma_}_{t.po
-00007860: 735f 7d5f 4e50 5f7b 742e 6465 705f 7d7b  s_}_NP_{t.dep_}{
-00007870: 742e 6865 6164 2e69 7d22 2069 6620 2874  t.head.i}" if (t
-00007880: 2e65 6e74 5f74 7970 655f 203d 3d20 274e  .ent_type_ == 'N
-00007890: 5027 2061 6e64 2074 2e6c 656d 6d61 5f20  P' and t.lemma_ 
-000078a0: 6e6f 7420 696e 2028 2774 6861 7427 2c27  not in ('that','
-000078b0: 7768 6963 6827 2929 2065 6c73 6520 6622  which')) else f"
-000078c0: 5f7b 742e 706f 735f 7d5f 7b74 2e74 6167  _{t.pos_}_{t.tag
-000078d0: 5f7d 5f7b 742e 6465 705f 7d7b 742e 6865  _}_{t.dep_}{t.he
-000078e0: 6164 2e69 7d22 2069 6620 742e 706f 735f  ad.i}" if t.pos_
-000078f0: 2069 6e20 2827 5052 4f50 4e27 2c27 4e55   in ('PROPN','NU
-00007900: 4d27 2c27 5827 2c27 5350 4143 4527 2c27  M','X','SPACE','
-00007910: 5055 4e43 5427 2920 656c 7365 2066 227b  PUNCT') else f"{
-00007920: 742e 7465 7874 2069 6620 742e 7465 7874  t.text if t.text
-00007930: 2069 6e20 2827 4927 2920 656c 7365 2074   in ('I') else t
-00007940: 2e74 6578 742e 6c6f 7765 7228 297d 5f7b  .text.lower()}_{
-00007950: 742e 6c65 6d6d 615f 7d5f 7b74 2e70 6f73  t.lemma_}_{t.pos
-00007960: 5f7d 5f7b 742e 7461 675f 7d7b 6f6e 6573  _}_{t.tag_}{ones
-00007970: 656c 662e 6765 7428 742e 7465 7874 2e6c  elf.get(t.text.l
-00007980: 6f77 6572 2829 2c20 2727 297d 5f7b 742e  ower(), '')}_{t.
-00007990: 6465 705f 7d7b 742e 6865 6164 2e69 7d22  dep_}{t.head.i}"
-000079a0: 0a09 6966 2074 2e65 6e74 5f69 645f 2e73  ..if t.ent_id_.s
-000079b0: 7461 7274 7377 6974 6828 225f 434c 2229  tartswith("_CL")
-000079c0: 2061 6e64 206e 6f74 2027 524f 4f54 2720   and not 'ROOT' 
-000079d0: 696e 2074 2e65 6e74 5f69 645f 3a20 7061  in t.ent_id_: pa
-000079e0: 6972 203d 2070 6169 7220 2b20 742e 656e  ir = pair + t.en
-000079f0: 745f 6964 5f0a 0972 6574 7572 6e20 7061  t_id_..return pa
-00007a00: 6972 200a 0a64 6566 2065 735f 736b 656e  ir ..def es_sken
-00007a10: 7028 646f 6329 3a0a 0923 6d65 7267 655f  p(doc):..#merge_
-00007a20: 6363 6f6d 7028 646f 6329 2023 206d 6572  ccomp(doc) # mer
-00007a30: 6765 5f6c 6561 7665 5f63 6c28 646f 6329  ge_leave_cl(doc)
-00007a40: 200a 096d 6572 6765 5f6e 7028 646f 6329   ..merge_np(doc)
-00007a50: 200a 0961 7474 6163 685f 636c 2864 6f63   ..attach_cl(doc
-00007a60: 290a 0972 6574 7572 6e20 225f 5e20 2220  )..return "_^ " 
-00007a70: 2b20 2720 272e 6a6f 696e 285b 2073 6b65  + ' '.join([ ske
-00007a80: 6e70 5f74 6f6b 2874 2920 666f 7220 7420  np_tok(t) for t 
-00007a90: 696e 2064 6f63 5d29 200a 0a40 4c61 6e67  in doc]) ..@Lang
-00007aa0: 7561 6765 2e63 6f6d 706f 6e65 6e74 2822  uage.component("
-00007ab0: 6d65 7267 655f 7072 7422 290a 6465 6620  merge_prt").def 
-00007ac0: 6d65 7267 655f 7072 7428 646f 6329 3a20  merge_prt(doc): 
-00007ad0: 0a09 2727 2749 2074 7572 6e20 6f66 6620  ..'''I turn off 
-00007ae0: 7468 6520 7261 6469 6f2e 203d 3e20 7475  the radio. => tu
-00007af0: 726e 5f6f 6666 202c 2061 6464 6564 2032  rn_off , added 2
-00007b00: 3032 332e 312e 3133 2727 270a 0969 6620  023.1.13'''..if 
-00007b10: 6e6f 7420 6861 7361 7474 7228 6d65 7267  not hasattr(merg
-00007b20: 655f 7072 742c 2027 6d61 7463 6865 7227  e_prt, 'matcher'
-00007b30: 293a 0a09 096d 6572 6765 5f70 7274 2e6d  ):...merge_prt.m
-00007b40: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
-00007b50: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
-00007b60: 290a 0909 6d65 7267 655f 7072 742e 6d61  )...merge_prt.ma
-00007b70: 7463 6865 722e 6164 6428 2270 7274 222c  tcher.add("prt",
-00007b80: 205b 5b7b 2250 4f53 223a 2256 4552 4222   [[{"POS":"VERB"
-00007b90: 7d2c 207b 2250 4f53 223a 2241 4450 222c  }, {"POS":"ADP",
-00007ba0: 2022 4445 5022 3a22 7072 7422 7d5d 5d2c   "DEP":"prt"}]],
-00007bb0: 2067 7265 6564 7920 3d27 4c4f 4e47 4553   greedy ='LONGES
-00007bc0: 5427 290a 0977 6974 6820 646f 632e 7265  T')..with doc.re
-00007bd0: 746f 6b65 6e69 7a65 2829 2061 7320 7265  tokenize() as re
-00007be0: 746f 6b65 6e69 7a65 723a 0a09 0966 6f72  tokenizer:...for
-00007bf0: 206e 616d 652c 2073 7461 7274 2c20 656e   name, start, en
-00007c00: 6420 696e 206d 6572 6765 5f70 7274 2e6d  d in merge_prt.m
-00007c10: 6174 6368 6572 2864 6f63 293a 0a09 0909  atcher(doc):....
-00007c20: 7472 793a 0a09 0909 0961 7474 7273 203d  try:.....attrs =
-00007c30: 207b 2270 6f73 223a 2064 6f63 5b73 7461   {"pos": doc[sta
-00007c40: 7274 5d2e 706f 732c 2022 7461 6722 3a20  rt].pos, "tag": 
-00007c50: 646f 635b 7374 6172 745d 2e74 6167 2c20  doc[start].tag, 
-00007c60: 2264 6570 223a 2064 6f63 5b73 7461 7274  "dep": doc[start
-00007c70: 5d2e 6465 702c 2022 6c65 6d6d 6122 3a64  ].dep, "lemma":d
-00007c80: 6f63 5b73 7461 7274 5d2e 6c65 6d6d 615f  oc[start].lemma_
-00007c90: 202b 2022 5f22 202b 2064 6f63 5b73 7461   + "_" + doc[sta
-00007ca0: 7274 2b31 5d2e 6c65 6d6d 615f 2c20 2265  rt+1].lemma_, "e
-00007cb0: 6e74 5f74 7970 6522 3a20 2276 7072 7422  nt_type": "vprt"
-00007cc0: 7d0a 0909 0909 7265 746f 6b65 6e69 7a65  }.....retokenize
-00007cd0: 722e 6d65 7267 6528 646f 635b 7374 6172  r.merge(doc[star
-00007ce0: 7420 3a20 656e 645d 2c20 6174 7472 733d  t : end], attrs=
-00007cf0: 6174 7472 7329 0a09 0909 6578 6365 7074  attrs)....except
-00007d00: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00007d10: 0a09 0909 0970 7269 6e74 2028 2022 6d65  .....print ( "me
-00007d20: 7267 655f 7072 7420 6578 3a22 2c20 6520  rge_prt ex:", e 
-00007d30: 2c20 7374 6172 742c 2065 6e64 290a 0972  , start, end)..r
-00007d40: 6574 7572 6e20 646f 630a 0a40 4c61 6e67  eturn doc..@Lang
-00007d50: 7561 6765 2e63 6f6d 706f 6e65 6e74 2822  uage.component("
-00007d60: 6d65 7267 655f 7622 290a 6465 6620 6d65  merge_v").def me
-00007d70: 7267 655f 7628 646f 6329 3a20 2320 3230  rge_v(doc): # 20
-00007d80: 3233 2e31 2e32 320a 0969 6620 6e6f 7420  23.1.22..if not 
-00007d90: 6861 7361 7474 7228 6d65 7267 655f 762c  hasattr(merge_v,
-00007da0: 2027 6d61 7463 6865 7227 293a 0a09 096d   'matcher'):...m
-00007db0: 6572 6765 5f76 2e6d 6174 6368 6572 203d  erge_v.matcher =
-00007dc0: 204d 6174 6368 6572 2873 7061 6379 2e6e   Matcher(spacy.n
-00007dd0: 6c70 2e76 6f63 6162 290a 0909 6d65 7267  lp.vocab)...merg
-00007de0: 655f 762e 6d61 7463 6865 722e 6164 6428  e_v.matcher.add(
-00007df0: 2276 7072 7422 2c20 5b5b 7b22 504f 5322  "vprt", [[{"POS"
-00007e00: 3a22 5645 5242 227d 2c20 7b22 504f 5322  :"VERB"}, {"POS"
-00007e10: 3a22 4144 5022 2c20 2244 4550 223a 2270  :"ADP", "DEP":"p
-00007e20: 7274 227d 5d5d 2c20 6772 6565 6479 203d  rt"}]], greedy =
-00007e30: 274c 4f4e 4745 5354 2729 0a09 0923 6d65  'LONGEST')...#me
-00007e40: 7267 655f 762e 6d61 7463 6865 722e 6164  rge_v.matcher.ad
-00007e50: 6428 2276 746f 7622 2c20 5b5b 7b22 504f  d("vtov", [[{"PO
-00007e60: 5322 3a22 5645 5242 227d 2c7b 224c 454d  S":"VERB"},{"LEM
-00007e70: 4d41 223a 2274 6f22 2c20 2254 4147 223a  MA":"to", "TAG":
-00007e80: 2254 4f22 7d2c 207b 2254 4147 223a 2256  "TO"}, {"TAG":"V
-00007e90: 4222 7d5d 5d2c 2067 7265 6564 7920 3d27  B"}]], greedy ='
-00007ea0: 4c4f 4e47 4553 5427 2920 2020 2020 2023  LONGEST')      #
-00007eb0: 2070 6c61 6e20 746f 2074 7572 6e20 6f66   plan to turn of
-00007ec0: 6620 7468 6520 7261 6469 6f20 0a09 0923  f the radio ...#
-00007ed0: 6d65 7267 655f 762e 6d61 7463 6865 722e  merge_v.matcher.
-00007ee0: 6164 6428 2276 7662 6722 2c20 5b5b 7b22  add("vvbg", [[{"
-00007ef0: 504f 5322 3a22 5645 5242 227d 2c7b 2244  POS":"VERB"},{"D
-00007f00: 4550 223a 2278 636f 6d70 222c 2254 4147  EP":"xcomp","TAG
-00007f10: 223a 2256 4247 227d 5d5d 2c20 6772 6565  ":"VBG"}]], gree
-00007f20: 6479 203d 274c 4f4e 4745 5354 2729 2020  dy ='LONGEST')  
-00007f30: 2020 2020 2020 2020 2020 2020 2020 0a09                ..
-00007f40: 096d 6572 6765 5f76 2e6d 6174 6368 6572  .merge_v.matcher
-00007f50: 2e61 6464 2822 6265 2d70 6e22 2c20 5b5b  .add("be-pn", [[
-00007f60: 7b22 4c45 4d4d 4122 3a22 6265 227d 2c7b  {"LEMMA":"be"},{
-00007f70: 2254 4147 223a 2249 4e22 2c22 504f 5322  "TAG":"IN","POS"
-00007f80: 3a22 4144 5022 7d2c 7b22 5441 4722 3a22  :"ADP"},{"TAG":"
-00007f90: 4e4e 227d 5d5d 2c20 6772 6565 6479 203d  NN"}]], greedy =
-00007fa0: 274c 4f4e 4745 5354 2729 2023 2062 6520  'LONGEST') # be 
-00007fb0: 696e 2063 6f6e 7374 7275 6374 696f 6e0a  in construction.
-00007fc0: 0909 6d65 7267 655f 762e 6d61 7463 6865  ..merge_v.matche
-00007fd0: 722e 6164 6428 2262 652d 6163 6f6d 7022  r.add("be-acomp"
-00007fe0: 2c20 5b5b 7b22 4c45 4d4d 4122 3a22 6265  , [[{"LEMMA":"be
-00007ff0: 227d 2c7b 2244 4550 223a 2261 636f 6d70  "},{"DEP":"acomp
-00008000: 222c 2250 4f53 223a 2241 444a 227d 5d5d  ","POS":"ADJ"}]]
-00008010: 2c20 6772 6565 6479 203d 274c 4f4e 4745  , greedy ='LONGE
-00008020: 5354 2729 2023 2250 4f53 223a 2241 5558  ST') #"POS":"AUX
-00008030: 222c 0a09 096d 6572 6765 5f76 2e6d 6174  ",...merge_v.mat
-00008040: 6368 6572 2e61 6464 2822 6265 2d61 7578  cher.add("be-aux
-00008050: 7061 7373 222c 205b 5b7b 224c 454d 4d41  pass", [[{"LEMMA
-00008060: 223a 2262 6522 2c22 4445 5022 3a22 6175  ":"be","DEP":"au
-00008070: 7870 6173 7322 7d2c 7b22 5441 4722 3a22  xpass"},{"TAG":"
-00008080: 5642 4e22 2c22 504f 5322 3a22 5645 5242  VBN","POS":"VERB
-00008090: 227d 5d5d 2c20 6772 6565 6479 203d 274c  "}]], greedy ='L
-000080a0: 4f4e 4745 5354 2729 0a09 7769 7468 2064  ONGEST')..with d
-000080b0: 6f63 2e72 6574 6f6b 656e 697a 6528 2920  oc.retokenize() 
-000080c0: 6173 2072 6574 6f6b 656e 697a 6572 3a0a  as retokenizer:.
-000080d0: 0909 666f 7220 6e61 6d65 2c20 7374 6172  ..for name, star
-000080e0: 742c 2065 6e64 2069 6e20 6d65 7267 655f  t, end in merge_
-000080f0: 762e 6d61 7463 6865 7228 646f 6329 3a0a  v.matcher(doc):.
-00008100: 0909 0974 7279 3a20 0a09 0909 0961 7474  ...try: .....att
-00008110: 7273 203d 207b 2270 6f73 223a 2022 5645  rs = {"pos": "VE
-00008120: 5242 222c 2022 7461 6722 3a20 646f 635b  RB", "tag": doc[
-00008130: 7374 6172 745d 2e74 6167 2c20 2264 6570  start].tag, "dep
-00008140: 223a 2064 6f63 5b73 7461 7274 5d2e 6465  ": doc[start].de
-00008150: 702c 200a 0909 0909 0922 6c65 6d6d 6122  p, ......"lemma"
-00008160: 3a22 5f22 2e6a 6f69 6e28 5b64 6f63 5b69  :"_".join([doc[i
-00008170: 5d2e 6c65 6d6d 615f 2069 6620 6920 3d3d  ].lemma_ if i ==
-00008180: 2073 7461 7274 2065 6c73 6520 646f 635b   start else doc[
-00008190: 695d 2e74 6578 7420 666f 7220 6920 696e  i].text for i in
-000081a0: 2072 616e 6765 2873 7461 7274 2c65 6e64   range(start,end
-000081b0: 295d 292c 200a 0909 0909 0922 656e 745f  )]), ......"ent_
-000081c0: 7479 7065 223a 2022 6d65 7267 655f 763a  type": "merge_v:
-000081d0: 2220 2b20 7370 6163 792e 6e6c 702e 766f  " + spacy.nlp.vo
-000081e0: 6361 625b 6e61 6d65 5d2e 7465 7874 202b  cab[name].text +
-000081f0: 2066 227c 7b64 6f63 5b73 7461 7274 5d2e   f"|{doc[start].
-00008200: 6c65 6d6d 615f 7d3a 7b64 6f63 5b73 7461  lemma_}:{doc[sta
-00008210: 7274 5d2e 706f 735f 7d3a 7b64 6f63 5b73  rt].pos_}:{doc[s
-00008220: 7461 7274 2b31 5d2e 6465 705f 7d3a 7b64  tart+1].dep_}:{d
-00008230: 6f63 5b73 7461 7274 2b31 5d2e 706f 735f  oc[start+1].pos_
-00008240: 7d3a 7b64 6f63 5b73 7461 7274 2b31 5d2e  }:{doc[start+1].
-00008250: 6c65 6d6d 615f 7d22 207d 0a09 0909 0972  lemma_}" }.....r
-00008260: 6574 6f6b 656e 697a 6572 2e6d 6572 6765  etokenizer.merge
-00008270: 2864 6f63 5b73 7461 7274 203a 2065 6e64  (doc[start : end
-00008280: 5d2c 2061 7474 7273 3d61 7474 7273 290a  ], attrs=attrs).
-00008290: 0909 0965 7863 6570 7420 4578 6365 7074  ...except Except
-000082a0: 696f 6e20 6173 2065 3a0a 0909 0909 7072  ion as e:.....pr
-000082b0: 696e 7420 2820 226d 6572 6765 5f76 2065  int ( "merge_v e
-000082c0: 783a 222c 2065 202c 2073 7461 7274 2c20  x:", e , start, 
-000082d0: 656e 6429 0a09 7265 7475 726e 2064 6f63  end)..return doc
-000082e0: 0a0a 404c 616e 6775 6167 652e 636f 6d70  ..@Language.comp
-000082f0: 6f6e 656e 7428 226d 6572 6765 5f74 7270  onent("merge_trp
-00008300: 2229 0a64 6566 206d 6572 6765 5f74 7270  ").def merge_trp
-00008310: 2864 6f63 293a 2023 2032 3032 332e 312e  (doc): # 2023.1.
-00008320: 3234 2c20 7c74 776f 2077 6f72 6473 2c20  24, |two words, 
-00008330: 7468 6520 7365 636f 6e64 206f 6e65 2069  the second one i
-00008340: 7320 7468 6520 6865 6164 200a 0969 6620  s the head ..if 
-00008350: 6e6f 7420 6861 7361 7474 7228 6d65 7267  not hasattr(merg
-00008360: 655f 7472 702c 2027 6d61 7463 6865 7227  e_trp, 'matcher'
-00008370: 293a 0a09 096d 6572 6765 5f74 7270 2e6d  ):...merge_trp.m
-00008380: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
-00008390: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
-000083a0: 290a 0909 6d65 7267 655f 7472 702e 6d61  )...merge_trp.ma
-000083b0: 7463 6865 722e 6164 6428 2261 6d6f 6422  tcher.add("amod"
-000083c0: 2c20 5b5b 7b22 504f 5322 3a22 4144 4a22  , [[{"POS":"ADJ"
-000083d0: 2c20 2244 4550 223a 2261 6d6f 6422 7d2c  , "DEP":"amod"},
-000083e0: 207b 2250 4f53 223a 224e 4f55 4e22 7d5d   {"POS":"NOUN"}]
-000083f0: 5d29 0a09 096d 6572 6765 5f74 7270 2e6d  ])...merge_trp.m
-00008400: 6174 6368 6572 2e61 6464 2822 6465 7422  atcher.add("det"
-00008410: 2c20 5b5b 7b22 504f 5322 3a22 4445 5422  , [[{"POS":"DET"
-00008420: 2c20 2244 4550 223a 2264 6574 227d 2c20  , "DEP":"det"}, 
-00008430: 7b22 504f 5322 3a22 4e4f 554e 227d 5d5d  {"POS":"NOUN"}]]
-00008440: 290a 0909 6d65 7267 655f 7472 702e 6d61  )...merge_trp.ma
-00008450: 7463 6865 722e 6164 6428 2261 6476 6d6f  tcher.add("advmo
-00008460: 6422 2c20 5b5b 7b22 504f 5322 3a22 4144  d", [[{"POS":"AD
-00008470: 5622 2c20 2244 4550 223a 2261 6476 6d6f  V", "DEP":"advmo
-00008480: 6422 7d2c 207b 2250 4f53 223a 207b 2249  d"}, {"POS": {"I
-00008490: 4e22 3a20 5b22 5645 5242 222c 2022 4144  N": ["VERB", "AD
-000084a0: 4a22 5d7d 7d20 5d5d 290a 0909 0a09 7769  J"]}} ]]).....wi
-000084b0: 7468 2064 6f63 2e72 6574 6f6b 656e 697a  th doc.retokeniz
-000084c0: 6528 2920 6173 2072 6574 6f6b 656e 697a  e() as retokeniz
-000084d0: 6572 3a0a 0909 666f 7220 6e61 6d65 2c20  er:...for name, 
-000084e0: 7374 6172 742c 2065 6e64 2069 6e20 6d65  start, end in me
-000084f0: 7267 655f 7472 702e 6d61 7463 6865 7228  rge_trp.matcher(
-00008500: 646f 6329 3a0a 0909 0974 7279 3a20 0a09  doc):....try: ..
-00008510: 0909 0961 7474 7273 203d 207b 2270 6f73  ...attrs = {"pos
-00008520: 223a 2064 6f63 5b73 7461 7274 2b31 5d2e  ": doc[start+1].
-00008530: 706f 732c 2022 7461 6722 3a20 646f 635b  pos, "tag": doc[
-00008540: 7374 6172 742b 315d 2e74 6167 2c20 2264  start+1].tag, "d
-00008550: 6570 223a 2064 6f63 5b73 7461 7274 2b31  ep": doc[start+1
-00008560: 5d2e 6465 702c 200a 0909 0909 0922 6c65  ].dep, ......"le
-00008570: 6d6d 6122 3a64 6f63 5b73 7461 7274 2b31  mma":doc[start+1
-00008580: 5d2e 6c65 6d6d 612c 200a 0909 0909 0922  ].lemma, ......"
-00008590: 656e 745f 7479 7065 223a 2022 6d65 7267  ent_type": "merg
-000085a0: 655f 7472 703a 2220 2b20 7370 6163 792e  e_trp:" + spacy.
-000085b0: 6e6c 702e 766f 6361 625b 6e61 6d65 5d2e  nlp.vocab[name].
-000085c0: 7465 7874 202b 2066 223a 7b64 6f63 5b73  text + f":{doc[s
-000085d0: 7461 7274 5d2e 7461 675f 7d20 7b64 6f63  tart].tag_} {doc
-000085e0: 5b73 7461 7274 2b31 5d2e 7461 675f 7d22  [start+1].tag_}"
-000085f0: 207d 0a09 0909 0972 6574 6f6b 656e 697a   }.....retokeniz
-00008600: 6572 2e6d 6572 6765 2864 6f63 5b73 7461  er.merge(doc[sta
-00008610: 7274 203a 2065 6e64 5d2c 2061 7474 7273  rt : end], attrs
-00008620: 3d61 7474 7273 290a 0909 0965 7863 6570  =attrs)....excep
-00008630: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00008640: 3a0a 0909 0909 7072 696e 7420 2820 226d  :.....print ( "m
-00008650: 6572 6765 5f74 7270 2065 783a 222c 2065  erge_trp ex:", e
-00008660: 202c 2073 7461 7274 2c20 656e 6429 0a09   , start, end)..
-00008670: 7265 7475 726e 2064 6f63 0a0a 6465 6620  return doc..def 
-00008680: 736b 6528 646f 632c 206e 616d 653a 7374  ske(doc, name:st
-00008690: 723d 2773 6d27 293a 2023 2061 6464 6564  r='sm'): # added
-000086a0: 2032 3032 332e 312e 3235 0a09 6966 206e   2023.1.25..if n
-000086b0: 6f74 2068 6173 6174 7472 2873 6b65 2c20  ot hasattr(ske, 
-000086c0: 276e 6c70 2729 3a0a 0909 736b 652e 6e6c  'nlp'):...ske.nl
-000086d0: 7020 3d20 7370 6163 792e 6c6f 6164 2866  p = spacy.load(f
-000086e0: 2765 6e5f 636f 7265 5f77 6562 5f7b 6e61  'en_core_web_{na
-000086f0: 6d65 7d27 290a 0909 5b20 736b 652e 6e6c  me}')...[ ske.nl
-00008700: 702e 6164 645f 7069 7065 2870 2920 666f  p.add_pipe(p) fo
-00008710: 7220 7020 696e 2028 226d 6572 6765 5f65  r p in ("merge_e
-00008720: 6e74 6974 6965 7322 2c20 226d 6572 6765  ntities", "merge
-00008730: 5f6e 7022 2c20 226d 6572 6765 5f70 7274  _np", "merge_prt
-00008740: 222c 2022 6d65 7267 655f 7472 7022 2c20  ", "merge_trp", 
-00008750: 2273 7061 6e5f 636c 6175 7365 2229 205d  "span_clause") ]
-00008760: 0a09 7265 7475 726e 2073 6b65 2e6e 6c70  ..return ske.nlp
-00008770: 2864 6f63 2920 0a23 7072 696e 7428 2073  (doc) .#print( s
-00008780: 6b65 2822 5468 6520 7175 6963 6b20 666f  ke("The quick fo
-00008790: 7820 6a75 6d70 6564 206f 7665 7220 7468  x jumped over th
-000087a0: 6520 6c61 7a79 2064 6f67 2e22 295b 305d  e lazy dog.")[0]
-000087b0: 2029 0a0a 6465 6620 6d65 7267 655f 7370   )..def merge_sp
-000087c0: 616e 2864 6f63 2c20 7061 743a 6c69 7374  an(doc, pat:list
-000087d0: 3d5b 7b22 504f 5322 3a22 5645 5242 227d  =[{"POS":"VERB"}
-000087e0: 2c7b 224c 454d 4d41 223a 2274 6f22 7d2c  ,{"LEMMA":"to"},
-000087f0: 7b22 5441 4722 3a22 5642 227d 5d29 3a20  {"TAG":"VB"}]): 
-00008800: 0a09 2727 2720 6465 6369 6465 2074 6f20  ..''' decide to 
-00008810: 7361 7665 203d 3e20 6f6e 652c 2032 3032  save => one, 202
-00008820: 332e 312e 3233 2027 2727 200a 0973 7061  3.1.23 ''' ..spa
-00008830: 7420 3d20 6a73 6f6e 2e64 756d 7073 2870  t = json.dumps(p
-00008840: 6174 2920 0a09 6966 206e 6f74 2068 6173  at) ..if not has
-00008850: 6174 7472 286d 6572 6765 5f73 7061 6e2c  attr(merge_span,
-00008860: 2073 7061 7429 3a0a 0909 5f6d 6174 6368   spat):..._match
-00008870: 6572 203d 204d 6174 6368 6572 2873 7061  er = Matcher(spa
-00008880: 6379 2e6e 6c70 2e76 6f63 6162 290a 0909  cy.nlp.vocab)...
-00008890: 5f6d 6174 6368 6572 2e61 6464 2873 7061  _matcher.add(spa
-000088a0: 742c 205b 7061 745d 2c20 6772 6565 6479  t, [pat], greedy
-000088b0: 203d 274c 4f4e 4745 5354 2729 0a09 0973   ='LONGEST')...s
-000088c0: 6574 6174 7472 286d 6572 6765 5f73 7061  etattr(merge_spa
-000088d0: 6e2c 2073 7061 742c 205f 6d61 7463 6865  n, spat, _matche
-000088e0: 7229 200a 0977 6974 6820 646f 632e 7265  r) ..with doc.re
-000088f0: 746f 6b65 6e69 7a65 2829 2061 7320 7265  tokenize() as re
-00008900: 746f 6b65 6e69 7a65 723a 0a09 0966 6f72  tokenizer:...for
-00008910: 206e 616d 652c 2073 7461 7274 2c20 656e   name, start, en
-00008920: 6420 696e 2067 6574 6174 7472 286d 6572  d in getattr(mer
-00008930: 6765 5f73 7061 6e2c 2073 7061 7429 2864  ge_span, spat)(d
-00008940: 6f63 293a 0a09 0909 7472 793a 200a 0909  oc):....try: ...
-00008950: 0909 6174 7472 7320 3d20 7b22 706f 7322  ..attrs = {"pos"
-00008960: 3a20 646f 635b 7374 6172 745d 2e70 6f73  : doc[start].pos
-00008970: 2c20 2274 6167 223a 2064 6f63 5b73 7461  , "tag": doc[sta
-00008980: 7274 5d2e 7461 672c 2022 6465 7022 3a20  rt].tag, "dep": 
-00008990: 646f 635b 7374 6172 745d 2e64 6570 2c20  doc[start].dep, 
-000089a0: 0a09 0909 0909 226c 656d 6d61 223a 225f  ......"lemma":"_
-000089b0: 222e 6a6f 696e 285b 646f 635b 695d 2e6c  ".join([doc[i].l
-000089c0: 656d 6d61 5f20 6966 2069 203d 3d20 7374  emma_ if i == st
-000089d0: 6172 7420 656c 7365 2064 6f63 5b69 5d2e  art else doc[i].
-000089e0: 7465 7874 2066 6f72 2069 2069 6e20 7261  text for i in ra
-000089f0: 6e67 6528 7374 6172 742c 656e 6429 5d29  nge(start,end)])
-00008a00: 2c20 0a09 0909 0909 2265 6e74 5f74 7970  , ......"ent_typ
-00008a10: 6522 3a20 226d 6572 6765 5f73 7061 6e3a  e": "merge_span:
-00008a20: 2220 2b20 7370 6174 207d 0a09 0909 0972  " + spat }.....r
-00008a30: 6574 6f6b 656e 697a 6572 2e6d 6572 6765  etokenizer.merge
-00008a40: 2864 6f63 5b73 7461 7274 203a 2065 6e64  (doc[start : end
-00008a50: 5d2c 2061 7474 7273 3d61 7474 7273 290a  ], attrs=attrs).
-00008a60: 0909 0965 7863 6570 7420 4578 6365 7074  ...except Except
-00008a70: 696f 6e20 6173 2065 3a0a 0909 0909 7072  ion as e:.....pr
-00008a80: 696e 7420 2820 226d 6572 6765 5f76 2065  int ( "merge_v e
-00008a90: 783a 222c 2065 202c 2073 7461 7274 2c20  x:", e , start, 
-00008aa0: 656e 6429 0a09 7265 7475 726e 2064 6f63  end)..return doc
-00008ab0: 0a0a 6465 6620 6465 706d 6174 6368 2829  ..def depmatch()
-00008ac0: 3a20 2366 726f 6d20 7370 6163 792e 6d61  : #from spacy.ma
-00008ad0: 7463 6865 7220 696d 706f 7274 204d 6174  tcher import Mat
-00008ae0: 6368 6572 2c44 6570 656e 6465 6e63 794d  cher,DependencyM
-00008af0: 6174 6368 6572 0a09 2727 2720 3230 3233  atcher..''' 2023
-00008b00: 2e31 2e36 2027 2727 0a09 6966 206e 6f74  .1.6 '''..if not
-00008b10: 2068 6173 6174 7472 2864 6570 6d61 7463   hasattr(depmatc
-00008b20: 682c 276d 6174 6368 6572 2729 3a20 0a09  h,'matcher'): ..
-00008b30: 0964 6570 6d61 7463 682e 6d61 7463 6865  .depmatch.matche
-00008b40: 7220 3d20 4465 7065 6e64 656e 6379 4d61  r = DependencyMa
-00008b50: 7463 6865 7228 7370 6163 792e 6e6c 702e  tcher(spacy.nlp.
-00008b60: 766f 6361 6229 0a09 0970 6174 7465 726e  vocab)...pattern
-00008b70: 203d 207b 0a09 0909 2320 6164 7663 6c2d   = {....# advcl-
-00008b80: 6163 6f6d 7020 776f 7272 7920 6265 2074  acomp worry be t
-00008b90: 6872 696c 6c65 6420 7c20 2257 6869 6c65  hrilled | "While
-00008ba0: 2049 2077 6173 2074 6872 696c 6c65 6420   I was thrilled 
-00008bb0: 7468 6174 2069 7420 7761 7320 6f6b 2c20  that it was ok, 
-00008bc0: 4920 776f 7272 6965 6420 7468 6174 2073  I worried that s
-00008bd0: 6865 2069 7320 6861 7070 792e 220a 0909  he is happy."...
-00008be0: 0922 6164 7663 6c2d 6163 6f6d 7022 3a20  ."advcl-acomp": 
-00008bf0: 5b20 7b22 5249 4748 545f 4944 223a 2022  [ {"RIGHT_ID": "
-00008c00: 7622 2c20 2252 4947 4854 5f41 5454 5253  v", "RIGHT_ATTRS
-00008c10: 223a 207b 2250 4f53 223a 2022 5645 5242  ": {"POS": "VERB
-00008c20: 227d 7d2c 2020 7b20 224c 4546 545f 4944  "}},  { "LEFT_ID
-00008c30: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
-00008c40: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
-00008c50: 223a 2022 6164 7663 6c22 2c20 2252 4947  ": "advcl", "RIG
-00008c60: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
-00008c70: 223a 2022 6164 7663 6c22 7d20 7d2c 207b  ": "advcl"} }, {
-00008c80: 2022 4c45 4654 5f49 4422 3a20 2261 6476   "LEFT_ID": "adv
-00008c90: 636c 222c 2022 5245 4c5f 4f50 223a 2022  cl", "REL_OP": "
-00008ca0: 3e22 2c22 5249 4748 545f 4944 223a 2022  >","RIGHT_ID": "
-00008cb0: 6f62 6a65 6374 222c 2022 5249 4748 545f  object", "RIGHT_
-00008cc0: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
-00008cd0: 2261 636f 6d70 227d 207d 5d20 2c20 0a09  "acomp"} }] , ..
-00008ce0: 0909 2320 5368 6520 6973 2068 6170 7079  ..# She is happy
-00008cf0: 2e20 7c20 6e73 7562 6a2d 6163 6f6d 7020  . | nsubj-acomp 
-00008d00: 6265 2073 6865 2068 6170 7079 0a09 0909  be she happy....
-00008d10: 226e 7375 626a 2d61 636f 6d70 223a 205b  "nsubj-acomp": [
-00008d20: 207b 2022 5249 4748 545f 4944 223a 2022   { "RIGHT_ID": "
-00008d30: 7622 2c20 2020 2252 4947 4854 5f41 5454  v",   "RIGHT_ATT
-00008d40: 5253 223a 207b 224c 454d 4d41 223a 2022  RS": {"LEMMA": "
-00008d50: 6265 227d 7d2c 7b20 224c 4546 545f 4944  be"}},{ "LEFT_ID
-00008d60: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
-00008d70: 3a22 3e22 2c20 2252 4947 4854 5f49 4422  :">", "RIGHT_ID"
-00008d80: 3a20 2273 7562 6a65 6374 222c 2022 5249  : "subject", "RI
-00008d90: 4748 545f 4154 5452 5322 3a20 7b22 4445  GHT_ATTRS": {"DE
-00008da0: 5022 3a20 226e 7375 626a 227d 207d 2c20  P": "nsubj"} }, 
-00008db0: 7b20 2022 4c45 4654 5f49 4422 3a20 2276  {  "LEFT_ID": "v
-00008dc0: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
-00008dd0: 2c20 2022 5249 4748 545f 4944 223a 2022  ,  "RIGHT_ID": "
-00008de0: 6f62 6a65 6374 222c 2020 2020 2252 4947  object",    "RIG
-00008df0: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
-00008e00: 223a 2022 6163 6f6d 7022 7d7d 5d2c 200a  ": "acomp"}}], .
-00008e10: 0909 0923 5368 6520 6973 2020 6120 6769  ...#She is  a gi
-00008e20: 726c 2e20 7c20 6e73 7562 6a2d 6174 7472  rl. | nsubj-attr
-00008e30: 2062 6520 7368 6520 6769 726c 0a09 0909   be she girl....
-00008e40: 226e 7375 626a 2d61 7474 7222 3a20 5b20  "nsubj-attr": [ 
-00008e50: 207b 2252 4947 4854 5f49 4422 3a20 2276   {"RIGHT_ID": "v
-00008e60: 222c 2022 5249 4748 545f 4154 5452 5322  ", "RIGHT_ATTRS"
-00008e70: 3a20 7b22 4c45 4d4d 4122 3a20 2262 6522  : {"LEMMA": "be"
-00008e80: 7d7d 2c20 7b20 224c 4546 545f 4944 223a  }}, { "LEFT_ID":
-00008e90: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
-00008ea0: 223e 222c 2252 4947 4854 5f49 4422 3a20  ">","RIGHT_ID": 
-00008eb0: 2273 7562 6a65 6374 222c 2022 5249 4748  "subject", "RIGH
-00008ec0: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
-00008ed0: 3a20 226e 7375 626a 227d 207d 2c20 7b20  : "nsubj"} }, { 
-00008ee0: 2020 2022 4c45 4654 5f49 4422 3a20 2276     "LEFT_ID": "v
-00008ef0: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
-00008f00: 2c20 2252 4947 4854 5f49 4422 3a20 226f  , "RIGHT_ID": "o
-00008f10: 626a 6563 7422 2c20 2252 4947 4854 5f41  bject", "RIGHT_A
-00008f20: 5454 5253 223a 207b 2244 4550 223a 2022  TTRS": {"DEP": "
-00008f30: 6174 7472 227d 207d 5d2c 0a09 0909 2320  attr"} }],....# 
-00008f40: 2065 6e6a 6f79 2073 7769 6d6d 696e 6720   enjoy swimming 
-00008f50: 7c20 6e73 7562 6a2d 7863 6f6d 7020 656e  | nsubj-xcomp en
-00008f60: 6a6f 7920 4920 7377 696d 6d69 6e67 0a09  joy I swimming..
-00008f70: 0909 226e 7375 626a 2d78 636f 6d70 223a  .."nsubj-xcomp":
-00008f80: 205b 2020 7b22 5249 4748 545f 4944 223a   [  {"RIGHT_ID":
-00008f90: 2022 7622 2c20 2252 4947 4854 5f41 5454   "v", "RIGHT_ATT
-00008fa0: 5253 223a 207b 2250 4f53 223a 2022 5645  RS": {"POS": "VE
-00008fb0: 5242 227d 7d2c 7b22 4c45 4654 5f49 4422  RB"}},{"LEFT_ID"
-00008fc0: 3a20 2276 222c 2022 5245 4c5f 4f50 223a  : "v", "REL_OP":
-00008fd0: 2022 3e22 2c20 2252 4947 4854 5f49 4422   ">", "RIGHT_ID"
-00008fe0: 3a20 2273 7562 6a65 6374 222c 2022 5249  : "subject", "RI
-00008ff0: 4748 545f 4154 5452 5322 3a20 7b22 4445  GHT_ATTRS": {"DE
-00009000: 5022 3a20 226e 7375 626a 227d 207d 2c20  P": "nsubj"} }, 
-00009010: 7b20 224c 4546 545f 4944 223a 2022 7622  { "LEFT_ID": "v"
-00009020: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
-00009030: 2022 5249 4748 545f 4944 223a 2022 6f62   "RIGHT_ID": "ob
-00009040: 6a65 6374 222c 2020 2252 4947 4854 5f41  ject",  "RIGHT_A
-00009050: 5454 5253 223a 207b 2244 4550 223a 2022  TTRS": {"DEP": "
-00009060: 7863 6f6d 7022 7d20 7d5d 2c0a 0909 0923  xcomp"} }],....#
-00009070: 2070 6c61 6e20 746f 2067 6f20 2c20 7c20   plan to go , | 
-00009080: 7863 6f6d 702d 746f 2070 6c61 6e20 676f  xcomp-to plan go
-00009090: 2074 6f0a 0909 0922 7863 6f6d 702d 746f   to...."xcomp-to
-000090a0: 223a 205b 2020 7b22 5249 4748 545f 4944  ": [  {"RIGHT_ID
-000090b0: 223a 2022 7622 2c20 2252 4947 4854 5f41  ": "v", "RIGHT_A
-000090c0: 5454 5253 223a 207b 2250 4f53 223a 2022  TTRS": {"POS": "
-000090d0: 5645 5242 227d 7d2c 207b 2022 4c45 4654  VERB"}}, { "LEFT
-000090e0: 5f49 4422 3a20 2276 222c 2022 5245 4c5f  _ID": "v", "REL_
-000090f0: 4f50 223a 2022 3e22 2c20 2252 4947 4854  OP": ">", "RIGHT
-00009100: 5f49 4422 3a20 226f 626a 6563 7422 2c20  _ID": "object", 
-00009110: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
-00009120: 7b22 4445 5022 3a20 2278 636f 6d70 227d  {"DEP": "xcomp"}
-00009130: 207d 2c20 7b22 4c45 4654 5f49 4422 3a20   }, {"LEFT_ID": 
-00009140: 226f 626a 6563 7422 2c20 2252 454c 5f4f  "object", "REL_O
-00009150: 5022 3a20 223b 222c 2022 5249 4748 545f  P": ";", "RIGHT_
-00009160: 4944 223a 2022 746f 222c 2022 5249 4748  ID": "to", "RIGH
-00009170: 545f 4154 5452 5322 3a20 7b22 4c45 4d4d  T_ATTRS": {"LEMM
-00009180: 4122 3a20 2274 6f22 7d20 7d2c 5d2c 0a09  A": "to"} },],..
-00009190: 0909 2320 7475 726e 206f 6666 2074 6865  ..# turn off the
-000091a0: 206c 6967 6874 207c 2070 7274 2d64 6f62   light | prt-dob
-000091b0: 6a20 7475 726e 206f 6666 206c 6967 6874  j turn off light
-000091c0: 0a09 0909 2264 6f62 6a2d 7072 7422 3a20  ...."dobj-prt": 
-000091d0: 5b20 207b 2252 4947 4854 5f49 4422 3a20  [  {"RIGHT_ID": 
-000091e0: 2276 222c 2252 4947 4854 5f41 5454 5253  "v","RIGHT_ATTRS
-000091f0: 223a 207b 2250 4f53 223a 2022 5645 5242  ": {"POS": "VERB
-00009200: 227d 7d2c 2020 7b20 224c 4546 545f 4944  "}},  { "LEFT_ID
-00009210: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
-00009220: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
-00009230: 223a 2022 7375 626a 6563 7422 2c20 2252  ": "subject", "R
-00009240: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
-00009250: 4550 223a 2022 7072 7422 7d20 7d2c 207b  EP": "prt"} }, {
-00009260: 2022 4c45 4654 5f49 4422 3a20 2276 222c   "LEFT_ID": "v",
-00009270: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
-00009280: 2252 4947 4854 5f49 4422 3a20 226f 626a  "RIGHT_ID": "obj
-00009290: 6563 7422 2c20 2252 4947 4854 5f41 5454  ect", "RIGHT_ATT
-000092a0: 5253 223a 207b 2244 4550 223a 2022 646f  RS": {"DEP": "do
-000092b0: 626a 227d 207d 5d2c 0a09 0909 2320 536f  bj"} }],....# So
-000092c0: 6d65 206f 6620 7468 6520 5265 7075 626c  me of the Republ
-000092d0: 6963 616e 2070 6f6c 6963 6965 7320 6861  ican policies ha
-000092e0: 7665 206c 6566 7420 6665 6d69 6e69 7374  ve left feminist
-000092f0: 7320 6469 736d 6179 6564 2061 6e64 2061  s dismayed and a
-00009300: 6768 6173 742e 207c 2064 6f62 6a2d 6163  ghast. | dobj-ac
-00009310: 6c20 6c65 6176 6520 6665 6d69 6e69 7374  l leave feminist
-00009320: 2064 6973 6d61 7965 640a 0909 0922 646f   dismayed...."do
-00009330: 626a 2d61 636c 223a 5b20 7b22 5249 4748  bj-acl":[ {"RIGH
-00009340: 545f 4944 223a 2022 7622 2c22 5249 4748  T_ID": "v","RIGH
-00009350: 545f 4154 5452 5322 3a20 7b22 504f 5322  T_ATTRS": {"POS"
-00009360: 3a20 2256 4552 4222 7d7d 2c20 7b20 224c  : "VERB"}}, { "L
-00009370: 4546 545f 4944 223a 2022 7622 2c22 5245  EFT_ID": "v","RE
-00009380: 4c5f 4f50 223a 2022 3e22 2c22 5249 4748  L_OP": ">","RIGH
-00009390: 545f 4944 223a 2022 646f 626a 222c 2252  T_ID": "dobj","R
-000093a0: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
-000093b0: 4550 223a 2022 646f 626a 227d 7d2c 7b20  EP": "dobj"}},{ 
-000093c0: 2022 4c45 4654 5f49 4422 3a20 2264 6f62   "LEFT_ID": "dob
-000093d0: 6a22 2c20 2252 454c 5f4f 5022 3a20 223e  j", "REL_OP": ">
-000093e0: 222c 2022 5249 4748 545f 4944 223a 2022  ", "RIGHT_ID": "
-000093f0: 7072 6570 222c 2022 5249 4748 545f 4154  prep", "RIGHT_AT
-00009400: 5452 5322 3a20 7b22 4445 5022 3a20 2261  TRS": {"DEP": "a
-00009410: 636c 227d 7d5d 2c0a 0909 0923 2062 6520  cl"}}],....# be 
-00009420: 6861 7070 7920 7769 7468 207c 206e 7375  happy with | nsu
-00009430: 626a 2d61 636f 6d70 2062 6520 4920 6861  bj-acomp be I ha
-00009440: 7070 790a 0909 0922 6163 6f6d 702d 7072  ppy...."acomp-pr
-00009450: 6570 223a 5b20 7b22 5249 4748 545f 4944  ep":[ {"RIGHT_ID
-00009460: 223a 2022 7622 2c22 5249 4748 545f 4154  ": "v","RIGHT_AT
-00009470: 5452 5322 3a20 7b22 504f 5322 3a20 2256  TRS": {"POS": "V
-00009480: 4552 4222 7d7d 2c20 7b20 224c 4546 545f  ERB"}}, { "LEFT_
-00009490: 4944 223a 2022 7622 2c22 5245 4c5f 4f50  ID": "v","REL_OP
-000094a0: 223a 2022 3e22 2c22 5249 4748 545f 4944  ": ">","RIGHT_ID
-000094b0: 223a 2022 6163 6f6d 7022 2c22 5249 4748  ": "acomp","RIGH
-000094c0: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
-000094d0: 3a20 2261 636f 6d70 227d 7d2c 7b20 2022  : "acomp"}},{  "
-000094e0: 4c45 4654 5f49 4422 3a20 2261 636f 6d70  LEFT_ID": "acomp
-000094f0: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
-00009500: 2c20 2252 4947 4854 5f49 4422 3a20 2270  , "RIGHT_ID": "p
-00009510: 7265 7022 2c20 2252 4947 4854 5f41 5454  rep", "RIGHT_ATT
-00009520: 5253 223a 207b 2244 4550 223a 2022 7072  RS": {"DEP": "pr
-00009530: 6570 227d 7d5d 2c0a 0909 0923 2062 6520  ep"}}],....# be 
-00009540: 6261 7365 6420 6f6e 207c 2062 652d 7662  based on | be-vb
-00009550: 6e2d 7072 6570 2062 6173 6520 6265 206f  n-prep base be o
-00009560: 6e0a 0909 0922 6265 2d76 626e 2d70 7265  n...."be-vbn-pre
-00009570: 7022 3a5b 207b 2252 4947 4854 5f49 4422  p":[ {"RIGHT_ID"
-00009580: 3a20 2276 222c 2022 5249 4748 545f 4154  : "v", "RIGHT_AT
-00009590: 5452 5322 3a20 7b22 5441 4722 3a20 2256  TRS": {"TAG": "V
-000095a0: 424e 227d 7d2c 207b 224c 4546 545f 4944  BN"}}, {"LEFT_ID
-000095b0: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
-000095c0: 3a20 223e 222c 2252 4947 4854 5f49 4422  : ">","RIGHT_ID"
-000095d0: 3a20 2262 6522 2c22 5249 4748 545f 4154  : "be","RIGHT_AT
-000095e0: 5452 5322 3a20 7b22 4c45 4d4d 4122 3a20  TRS": {"LEMMA": 
-000095f0: 2262 6522 7d20 7d2c 207b 2022 4c45 4654  "be"} }, { "LEFT
-00009600: 5f49 4422 3a20 2276 222c 2022 5245 4c5f  _ID": "v", "REL_
-00009610: 4f50 223a 2022 3e22 2c20 2252 4947 4854  OP": ">", "RIGHT
-00009620: 5f49 4422 3a20 2270 7265 7022 2c20 2252  _ID": "prep", "R
-00009630: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
-00009640: 4550 223a 2022 7072 6570 227d 2020 7d5d  EP": "prep"}  }]
-00009650: 2c0a 0909 097d 0a09 0966 6f72 206e 616d  ,....}...for nam
-00009660: 652c 7061 7420 696e 2070 6174 7465 726e  e,pat in pattern
-00009670: 2e69 7465 6d73 2829 3a20 6465 706d 6174  .items(): depmat
-00009680: 6368 2e6d 6174 6368 6572 2e61 6464 286e  ch.matcher.add(n
-00009690: 616d 652c 205b 7061 745d 290a 0972 6574  ame, [pat])..ret
-000096a0: 7572 6e20 6465 706d 6174 6368 2e6d 6174  urn depmatch.mat
-000096b0: 6368 6572 200a 0923 646f 6320 3d20 7370  cher ..#doc = sp
-000096c0: 6163 792e 6e6c 7028 2249 2074 7572 6e20  acy.nlp("I turn 
-000096d0: 6f66 6620 7468 6520 6c69 6768 742c 2061  off the light, a
-000096e0: 6e64 2069 7420 6973 2062 6173 6564 206f  nd it is based o
-000096f0: 6e20 7468 6520 7461 626c 652e 2229 0a09  n the table.")..
-00009700: 2366 6f72 206e 616d 652c 2061 7220 696e  #for name, ar in
-00009710: 206d 6174 6368 6572 2864 6f63 2920 3a20   matcher(doc) : 
-00009720: 7072 696e 7428 7370 6163 792e 6e6c 702e  print(spacy.nlp.
-00009730: 766f 6361 625b 6e61 6d65 5d2e 7465 7874  vocab[name].text
-00009740: 2c20 646f 635b 6172 5b30 5d5d 2e6c 656d  , doc[ar[0]].lem
-00009750: 6d61 5f2c 2064 6f63 5b61 725b 315d 5d2e  ma_, doc[ar[1]].
-00009760: 6c65 6d6d 615f 2c20 646f 635b 6172 5b32  lemma_, doc[ar[2
-00009770: 5d5d 2920 2320 776f 7272 7920 6265 2074  ]]) # worry be t
-00009780: 6872 696c 6c65 640a 0a64 6566 2074 7270  hrilled..def trp
-00009790: 7828 646f 632c 2076 6f63 6162 293a 2023  x(doc, vocab): #
-000097a0: 2073 7061 6379 2e6e 6c70 2e76 6f63 6162   spacy.nlp.vocab
-000097b0: 2c20 3230 3233 2e31 2e32 310a 0966 726f  , 2023.1.21..fro
-000097c0: 6d20 7370 6163 792e 6d61 7463 6865 7220  m spacy.matcher 
-000097d0: 696d 706f 7274 2044 6570 656e 6465 6e63  import Dependenc
-000097e0: 794d 6174 6368 6572 0a09 6966 206e 6f74  yMatcher..if not
-000097f0: 2068 6173 6174 7472 2874 7270 782c 276d   hasattr(trpx,'m
-00009800: 6174 6368 6572 2729 3a20 0a09 0974 7270  atcher'): ...trp
-00009810: 782e 6d61 7463 6865 7220 3d20 4465 7065  x.matcher = Depe
-00009820: 6e64 656e 6379 4d61 7463 6865 7228 766f  ndencyMatcher(vo
-00009830: 6361 6229 0a09 0970 6174 7465 726e 203d  cab)...pattern =
-00009840: 207b 0a09 0909 2320 6164 7663 6c2d 6163   {....# advcl-ac
-00009850: 6f6d 7020 776f 7272 7920 6265 2074 6872  omp worry be thr
-00009860: 696c 6c65 6420 7c20 2257 6869 6c65 2049  illed | "While I
-00009870: 2077 6173 2074 6872 696c 6c65 6420 7468   was thrilled th
-00009880: 6174 2069 7420 7761 7320 6f6b 2c20 4920  at it was ok, I 
-00009890: 776f 7272 6965 6420 7468 6174 2073 6865  worried that she
-000098a0: 2069 7320 6861 7070 792e 220a 0909 0922   is happy."...."
-000098b0: 6164 7663 6c2d 6163 6f6d 7022 3a20 5b20  advcl-acomp": [ 
-000098c0: 7b22 5249 4748 545f 4944 223a 2022 7622  {"RIGHT_ID": "v"
-000098d0: 2c20 2252 4947 4854 5f41 5454 5253 223a  , "RIGHT_ATTRS":
-000098e0: 207b 2250 4f53 223a 2022 5645 5242 227d   {"POS": "VERB"}
-000098f0: 7d2c 2020 7b20 224c 4546 545f 4944 223a  },  { "LEFT_ID":
-00009900: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
-00009910: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
-00009920: 2022 6164 7663 6c22 2c20 2252 4947 4854   "advcl", "RIGHT
-00009930: 5f41 5454 5253 223a 207b 2244 4550 223a  _ATTRS": {"DEP":
-00009940: 2022 6164 7663 6c22 7d20 7d2c 207b 2022   "advcl"} }, { "
-00009950: 4c45 4654 5f49 4422 3a20 2261 6476 636c  LEFT_ID": "advcl
-00009960: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
-00009970: 2c22 5249 4748 545f 4944 223a 2022 6f62  ,"RIGHT_ID": "ob
-00009980: 6a65 6374 222c 2022 5249 4748 545f 4154  ject", "RIGHT_AT
-00009990: 5452 5322 3a20 7b22 4445 5022 3a20 2261  TRS": {"DEP": "a
-000099a0: 636f 6d70 227d 207d 5d20 2c20 0a09 0909  comp"} }] , ....
-000099b0: 2320 5368 6520 6973 2068 6170 7079 2e20  # She is happy. 
-000099c0: 7c20 6e73 7562 6a2d 6163 6f6d 7020 6265  | nsubj-acomp be
-000099d0: 2073 6865 2068 6170 7079 0a09 0909 226e   she happy...."n
-000099e0: 7375 626a 2d61 636f 6d70 223a 205b 207b  subj-acomp": [ {
-000099f0: 2022 5249 4748 545f 4944 223a 2022 7622   "RIGHT_ID": "v"
-00009a00: 2c20 2020 2252 4947 4854 5f41 5454 5253  ,   "RIGHT_ATTRS
-00009a10: 223a 207b 224c 454d 4d41 223a 2022 6265  ": {"LEMMA": "be
-00009a20: 227d 7d2c 7b20 224c 4546 545f 4944 223a  "}},{ "LEFT_ID":
-00009a30: 2022 7622 2c20 2252 454c 5f4f 5022 3a22   "v", "REL_OP":"
-00009a40: 3e22 2c20 2252 4947 4854 5f49 4422 3a20  >", "RIGHT_ID": 
-00009a50: 2273 7562 6a65 6374 222c 2022 5249 4748  "subject", "RIGH
-00009a60: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
-00009a70: 3a20 226e 7375 626a 227d 207d 2c20 7b20  : "nsubj"} }, { 
-00009a80: 2022 4c45 4654 5f49 4422 3a20 2276 222c   "LEFT_ID": "v",
-00009a90: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
-00009aa0: 2022 5249 4748 545f 4944 223a 2022 6f62   "RIGHT_ID": "ob
-00009ab0: 6a65 6374 222c 2020 2020 2252 4947 4854  ject",    "RIGHT
-00009ac0: 5f41 5454 5253 223a 207b 2244 4550 223a  _ATTRS": {"DEP":
-00009ad0: 2022 6163 6f6d 7022 7d7d 5d2c 200a 0909   "acomp"}}], ...
-00009ae0: 0923 5368 6520 6973 2020 6120 6769 726c  .#She is  a girl
-00009af0: 2e20 7c20 6e73 7562 6a2d 6174 7472 2062  . | nsubj-attr b
-00009b00: 6520 7368 6520 6769 726c 0a09 0909 226e  e she girl...."n
-00009b10: 7375 626a 2d61 7474 7222 3a20 5b20 207b  subj-attr": [  {
-00009b20: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
-00009b30: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
-00009b40: 7b22 4c45 4d4d 4122 3a20 2262 6522 7d7d  {"LEMMA": "be"}}
-00009b50: 2c20 7b20 224c 4546 545f 4944 223a 2022  , { "LEFT_ID": "
-00009b60: 7622 2c20 2252 454c 5f4f 5022 3a20 223e  v", "REL_OP": ">
-00009b70: 222c 2252 4947 4854 5f49 4422 3a20 2273  ","RIGHT_ID": "s
-00009b80: 7562 6a65 6374 222c 2022 5249 4748 545f  ubject", "RIGHT_
-00009b90: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
-00009ba0: 226e 7375 626a 227d 207d 2c20 7b20 2020  "nsubj"} }, {   
-00009bb0: 2022 4c45 4654 5f49 4422 3a20 2276 222c   "LEFT_ID": "v",
-00009bc0: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
-00009bd0: 2252 4947 4854 5f49 4422 3a20 226f 626a  "RIGHT_ID": "obj
-00009be0: 6563 7422 2c20 2252 4947 4854 5f41 5454  ect", "RIGHT_ATT
-00009bf0: 5253 223a 207b 2244 4550 223a 2022 6174  RS": {"DEP": "at
-00009c00: 7472 227d 207d 5d2c 0a09 0909 2320 2065  tr"} }],....#  e
-00009c10: 6e6a 6f79 2073 7769 6d6d 696e 6720 7c20  njoy swimming | 
-00009c20: 6e73 7562 6a2d 7863 6f6d 7020 656e 6a6f  nsubj-xcomp enjo
-00009c30: 7920 4920 7377 696d 6d69 6e67 0a09 0909  y I swimming....
-00009c40: 226e 7375 626a 2d78 636f 6d70 223a 205b  "nsubj-xcomp": [
-00009c50: 2020 7b22 5249 4748 545f 4944 223a 2022    {"RIGHT_ID": "
-00009c60: 7622 2c20 2252 4947 4854 5f41 5454 5253  v", "RIGHT_ATTRS
-00009c70: 223a 207b 2250 4f53 223a 2022 5645 5242  ": {"POS": "VERB
-00009c80: 227d 7d2c 7b22 4c45 4654 5f49 4422 3a20  "}},{"LEFT_ID": 
-00009c90: 2276 222c 2022 5245 4c5f 4f50 223a 2022  "v", "REL_OP": "
-00009ca0: 3e22 2c20 2252 4947 4854 5f49 4422 3a20  >", "RIGHT_ID": 
-00009cb0: 2273 7562 6a65 6374 222c 2022 5249 4748  "subject", "RIGH
-00009cc0: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
-00009cd0: 3a20 226e 7375 626a 227d 207d 2c20 7b20  : "nsubj"} }, { 
-00009ce0: 224c 4546 545f 4944 223a 2022 7622 2c20  "LEFT_ID": "v", 
-00009cf0: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
-00009d00: 5249 4748 545f 4944 223a 2022 6f62 6a65  RIGHT_ID": "obje
-00009d10: 6374 222c 2020 2252 4947 4854 5f41 5454  ct",  "RIGHT_ATT
-00009d20: 5253 223a 207b 2244 4550 223a 2022 7863  RS": {"DEP": "xc
-00009d30: 6f6d 7022 7d20 7d5d 2c0a 0909 0923 2070  omp"} }],....# p
-00009d40: 6c61 6e20 746f 2067 6f20 2c20 7c20 7863  lan to go , | xc
-00009d50: 6f6d 702d 746f 2070 6c61 6e20 676f 2074  omp-to plan go t
-00009d60: 6f0a 0909 0922 7863 6f6d 702d 746f 223a  o...."xcomp-to":
-00009d70: 205b 2020 7b22 5249 4748 545f 4944 223a   [  {"RIGHT_ID":
-00009d80: 2022 7622 2c20 2252 4947 4854 5f41 5454   "v", "RIGHT_ATT
-00009d90: 5253 223a 207b 2250 4f53 223a 2022 5645  RS": {"POS": "VE
-00009da0: 5242 227d 7d2c 207b 2022 4c45 4654 5f49  RB"}}, { "LEFT_I
-00009db0: 4422 3a20 2276 222c 2022 5245 4c5f 4f50  D": "v", "REL_OP
-00009dc0: 223a 2022 3e22 2c20 2252 4947 4854 5f49  ": ">", "RIGHT_I
-00009dd0: 4422 3a20 226f 626a 6563 7422 2c20 2022  D": "object",  "
-00009de0: 5249 4748 545f 4154 5452 5322 3a20 7b22  RIGHT_ATTRS": {"
-00009df0: 4445 5022 3a20 2278 636f 6d70 227d 207d  DEP": "xcomp"} }
-00009e00: 2c20 7b22 4c45 4654 5f49 4422 3a20 226f  , {"LEFT_ID": "o
-00009e10: 626a 6563 7422 2c20 2252 454c 5f4f 5022  bject", "REL_OP"
-00009e20: 3a20 223b 222c 2022 5249 4748 545f 4944  : ";", "RIGHT_ID
-00009e30: 223a 2022 746f 222c 2022 5249 4748 545f  ": "to", "RIGHT_
-00009e40: 4154 5452 5322 3a20 7b22 4c45 4d4d 4122  ATTRS": {"LEMMA"
-00009e50: 3a20 2274 6f22 7d20 7d2c 5d2c 0a09 0909  : "to"} },],....
-00009e60: 2320 7475 726e 206f 6666 2074 6865 206c  # turn off the l
-00009e70: 6967 6874 207c 2070 7274 2d64 6f62 6a20  ight | prt-dobj 
-00009e80: 7475 726e 206f 6666 206c 6967 6874 0a09  turn off light..
-00009e90: 0909 2264 6f62 6a2d 7072 7422 3a20 5b20  .."dobj-prt": [ 
-00009ea0: 207b 2252 4947 4854 5f49 4422 3a20 2276   {"RIGHT_ID": "v
-00009eb0: 222c 2252 4947 4854 5f41 5454 5253 223a  ","RIGHT_ATTRS":
-00009ec0: 207b 2250 4f53 223a 2022 5645 5242 227d   {"POS": "VERB"}
-00009ed0: 7d2c 2020 7b20 224c 4546 545f 4944 223a  },  { "LEFT_ID":
-00009ee0: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
-00009ef0: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
-00009f00: 2022 7375 626a 6563 7422 2c20 2252 4947   "subject", "RIG
-00009f10: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
-00009f20: 223a 2022 7072 7422 7d20 7d2c 207b 2022  ": "prt"} }, { "
-00009f30: 4c45 4654 5f49 4422 3a20 2276 222c 2022  LEFT_ID": "v", "
-00009f40: 5245 4c5f 4f50 223a 2022 3e22 2c20 2252  REL_OP": ">", "R
-00009f50: 4947 4854 5f49 4422 3a20 226f 626a 6563  IGHT_ID": "objec
-00009f60: 7422 2c20 2252 4947 4854 5f41 5454 5253  t", "RIGHT_ATTRS
-00009f70: 223a 207b 2244 4550 223a 2022 646f 626a  ": {"DEP": "dobj
-00009f80: 227d 207d 5d2c 0a09 0909 2320 536f 6d65  "} }],....# Some
-00009f90: 206f 6620 7468 6520 5265 7075 626c 6963   of the Republic
-00009fa0: 616e 2070 6f6c 6963 6965 7320 6861 7665  an policies have
-00009fb0: 206c 6566 7420 6665 6d69 6e69 7374 7320   left feminists 
-00009fc0: 6469 736d 6179 6564 2061 6e64 2061 6768  dismayed and agh
-00009fd0: 6173 742e 207c 2064 6f62 6a2d 6163 6c20  ast. | dobj-acl 
-00009fe0: 6c65 6176 6520 6665 6d69 6e69 7374 2064  leave feminist d
-00009ff0: 6973 6d61 7965 640a 0909 0922 646f 626a  ismayed...."dobj
-0000a000: 2d61 636c 223a 5b20 7b22 5249 4748 545f  -acl":[ {"RIGHT_
-0000a010: 4944 223a 2022 7622 2c22 5249 4748 545f  ID": "v","RIGHT_
-0000a020: 4154 5452 5322 3a20 7b22 504f 5322 3a20  ATTRS": {"POS": 
-0000a030: 2256 4552 4222 7d7d 2c20 7b20 224c 4546  "VERB"}}, { "LEF
-0000a040: 545f 4944 223a 2022 7622 2c22 5245 4c5f  T_ID": "v","REL_
-0000a050: 4f50 223a 2022 3e22 2c22 5249 4748 545f  OP": ">","RIGHT_
-0000a060: 4944 223a 2022 646f 626a 222c 2252 4947  ID": "dobj","RIG
-0000a070: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
-0000a080: 223a 2022 646f 626a 227d 7d2c 7b20 2022  ": "dobj"}},{  "
-0000a090: 4c45 4654 5f49 4422 3a20 2264 6f62 6a22  LEFT_ID": "dobj"
-0000a0a0: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
-0000a0b0: 2022 5249 4748 545f 4944 223a 2022 7072   "RIGHT_ID": "pr
-0000a0c0: 6570 222c 2022 5249 4748 545f 4154 5452  ep", "RIGHT_ATTR
-0000a0d0: 5322 3a20 7b22 4445 5022 3a20 2261 636c  S": {"DEP": "acl
-0000a0e0: 227d 7d5d 2c0a 0909 0923 2062 6520 6861  "}}],....# be ha
-0000a0f0: 7070 7920 7769 7468 207c 206e 7375 626a  ppy with | nsubj
-0000a100: 2d61 636f 6d70 2062 6520 4920 6861 7070  -acomp be I happ
-0000a110: 790a 0909 0922 6163 6f6d 702d 7072 6570  y...."acomp-prep
-0000a120: 223a 5b20 7b22 5249 4748 545f 4944 223a  ":[ {"RIGHT_ID":
-0000a130: 2022 7622 2c22 5249 4748 545f 4154 5452   "v","RIGHT_ATTR
-0000a140: 5322 3a20 7b22 504f 5322 3a20 2256 4552  S": {"POS": "VER
-0000a150: 4222 7d7d 2c20 7b20 224c 4546 545f 4944  B"}}, { "LEFT_ID
-0000a160: 223a 2022 7622 2c22 5245 4c5f 4f50 223a  ": "v","REL_OP":
-0000a170: 2022 3e22 2c22 5249 4748 545f 4944 223a   ">","RIGHT_ID":
-0000a180: 2022 6163 6f6d 7022 2c22 5249 4748 545f   "acomp","RIGHT_
-0000a190: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
-0000a1a0: 2261 636f 6d70 227d 7d2c 7b20 2022 4c45  "acomp"}},{  "LE
-0000a1b0: 4654 5f49 4422 3a20 2261 636f 6d70 222c  FT_ID": "acomp",
-0000a1c0: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
-0000a1d0: 2252 4947 4854 5f49 4422 3a20 2270 7265  "RIGHT_ID": "pre
-0000a1e0: 7022 2c20 2252 4947 4854 5f41 5454 5253  p", "RIGHT_ATTRS
-0000a1f0: 223a 207b 2244 4550 223a 2022 7072 6570  ": {"DEP": "prep
-0000a200: 227d 7d5d 2c0a 0909 0923 2062 6520 6261  "}}],....# be ba
-0000a210: 7365 6420 6f6e 207c 2062 652d 7662 6e2d  sed on | be-vbn-
-0000a220: 7072 6570 2062 6173 6520 6265 206f 6e0a  prep base be on.
-0000a230: 0909 0922 6265 2d76 626e 2d70 7265 7022  ..."be-vbn-prep"
-0000a240: 3a5b 207b 2252 4947 4854 5f49 4422 3a20  :[ {"RIGHT_ID": 
-0000a250: 2276 222c 2022 5249 4748 545f 4154 5452  "v", "RIGHT_ATTR
-0000a260: 5322 3a20 7b22 5441 4722 3a20 2256 424e  S": {"TAG": "VBN
-0000a270: 227d 7d2c 207b 224c 4546 545f 4944 223a  "}}, {"LEFT_ID":
-0000a280: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
-0000a290: 223e 222c 2252 4947 4854 5f49 4422 3a20  ">","RIGHT_ID": 
-0000a2a0: 2262 6522 2c22 5249 4748 545f 4154 5452  "be","RIGHT_ATTR
-0000a2b0: 5322 3a20 7b22 4c45 4d4d 4122 3a20 2262  S": {"LEMMA": "b
-0000a2c0: 6522 7d20 7d2c 207b 2022 4c45 4654 5f49  e"} }, { "LEFT_I
-0000a2d0: 4422 3a20 2276 222c 2022 5245 4c5f 4f50  D": "v", "REL_OP
-0000a2e0: 223a 2022 3e22 2c20 2252 4947 4854 5f49  ": ">", "RIGHT_I
-0000a2f0: 4422 3a20 2270 7265 7022 2c20 2252 4947  D": "prep", "RIG
-0000a300: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
-0000a310: 223a 2022 7072 6570 227d 2020 7d5d 2c0a  ": "prep"}  }],.
-0000a320: 0909 097d 0a09 0966 6f72 206e 616d 652c  ...}...for name,
-0000a330: 7061 7420 696e 2070 6174 7465 726e 2e69  pat in pattern.i
-0000a340: 7465 6d73 2829 3a20 7472 7078 2e6d 6174  tems(): trpx.mat
-0000a350: 6368 6572 2e61 6464 2866 2274 7270 783a  cher.add(f"trpx:
-0000a360: 7b6e 616d 657d 222c 205b 7061 745d 290a  {name}", [pat]).
-0000a370: 0966 6f72 206e 616d 652c 2061 7220 696e  .for name, ar in
-0000a380: 2074 7270 782e 6d61 7463 6865 7228 646f   trpx.matcher(do
-0000a390: 6329 203a 0a09 0964 6f63 2e73 7061 6e73  c) :...doc.spans
-0000a3a0: 5b76 6f63 6162 5b6e 616d 655d 2e74 6578  [vocab[name].tex
-0000a3b0: 745d 203d 205b 2064 6f63 5b61 725b 305d  t] = [ doc[ar[0]
-0000a3c0: 3a61 725b 305d 2b31 5d2c 2064 6f63 5b61  :ar[0]+1], doc[a
-0000a3d0: 725b 315d 3a61 725b 315d 2b31 5d2c 2064  r[1]:ar[1]+1], d
-0000a3e0: 6f63 5b61 725b 325d 3a61 725b 325d 2b31  oc[ar[2]:ar[2]+1
-0000a3f0: 5d20 5d0a 0972 6574 7572 6e20 646f 6320  ] ]..return doc 
-0000a400: 0a0a 6465 6620 746f 6b74 7270 2864 6f63  ..def toktrp(doc
-0000a410: 293a 2023 2062 6173 6963 2066 6f72 2073  ): # basic for s
-0000a420: 716c 7369 200a 0961 7272 203d 205b 6622  qlsi ..arr = [f"
-0000a430: 2a3a 736e 746e 756d 225d 0a09 666f 7220  *:sntnum"]..for 
-0000a440: 7420 696e 2064 6f63 3a0a 0909 5b61 7272  t in doc:...[arr
-0000a450: 2e61 7070 656e 6428 7329 2066 6f72 2073  .append(s) for s
-0000a460: 2069 6e20 2028 222a 3a4c 4558 222c 222a   in  ("*:LEX","*
-0000a470: 3a4c 454d 222c 2066 222a 3a7b 742e 706f  :LEM", f"*:{t.po
-0000a480: 735f 7d22 2c20 6622 2a3a 7b74 2e74 6167  s_}", f"*:{t.tag
-0000a490: 5f7d 222c 6622 2a3a 7b74 2e64 6570 5f7d  _}",f"*:{t.dep_}
-0000a4a0: 222c 6622 2a3a 7e7b 742e 6465 705f 7d22  ",f"*:~{t.dep_}"
-0000a4b0: 2920 5d0a 0909 6966 2074 2e70 6f73 5f20  ) ]...if t.pos_ 
-0000a4c0: 696e 2028 2256 4552 4222 2c22 4e4f 554e  in ("VERB","NOUN
-0000a4d0: 222c 2241 444a 222c 2241 4456 2229 203a  ","ADJ","ADV") :
-0000a4e0: 200a 0909 0961 7272 2e61 7070 656e 6428   ....arr.append(
-0000a4f0: 2066 227b 742e 7461 675f 7d3a 7b74 2e74   f"{t.tag_}:{t.t
-0000a500: 6578 742e 6c6f 7765 7228 297d 2229 2020  ext.lower()}")  
-0000a510: 2320 5642 4420 3a20 206d 6164 6520 2c20  # VBD :  made , 
-0000a520: 6164 6465 6420 3230 3232 2e31 322e 3130  added 2022.12.10
-0000a530: 0a0a 0909 6966 206e 6f74 2074 2e70 6f73  ....if not t.pos
-0000a540: 5f20 696e 2028 2750 524f 504e 272c 2758  _ in ('PROPN','X
-0000a550: 272c 2027 5055 4e43 5427 2c22 5350 4143  ', 'PUNCT',"SPAC
-0000a560: 4522 2920 616e 6420 742e 6973 5f61 6c70  E") and t.is_alp
-0000a570: 6861 3a0a 0909 0961 7272 2e65 7874 656e  ha:....arr.exten
-0000a580: 6428 5b66 227b 742e 6c65 6d6d 615f 7d3a  d([f"{t.lemma_}:
-0000a590: 7b74 2e70 6f73 5f7d 222c 6622 7b74 2e6c  {t.pos_}",f"{t.l
-0000a5a0: 656d 6d61 5f7d 3a4c 4558 3a7b 742e 7465  emma_}:LEX:{t.te
-0000a5b0: 7874 2e6c 6f77 6572 2829 7d22 2c66 224c  xt.lower()}",f"L
-0000a5c0: 454d 3a7b 742e 6c65 6d6d 615f 2e6c 6f77  EM:{t.lemma_.low
-0000a5d0: 6572 2829 7d22 2c66 224c 4558 3a7b 742e  er()}",f"LEX:{t.
-0000a5e0: 7465 7874 2e6c 6f77 6572 2829 7d22 2c66  text.lower()}",f
-0000a5f0: 227b 742e 706f 735f 7d3a 7b74 2e6c 656d  "{t.pos_}:{t.lem
-0000a600: 6d61 5f2e 6c6f 7765 7228 297d 222c 6622  ma_.lower()}",f"
-0000a610: 7b74 2e6c 656d 6d61 5f2e 6c6f 7765 7228  {t.lemma_.lower(
-0000a620: 297d 3a7b 742e 706f 735f 7d3a 7b74 2e74  )}:{t.pos_}:{t.t
-0000a630: 6167 5f7d 222c 6622 2a3a 7b74 2e70 6f73  ag_}",f"*:{t.pos
-0000a640: 5f7d 3a7b 742e 7461 675f 7d22 5d29 200a  _}:{t.tag_}"]) .
-0000a650: 0909 6966 2074 2e70 6f73 5f20 6e6f 7420  ..if t.pos_ not 
-0000a660: 696e 2028 2250 524f 504e 222c 2250 554e  in ("PROPN","PUN
-0000a670: 4354 222c 2253 5041 4345 2229 2061 6e64  CT","SPACE") and
-0000a680: 2074 2e69 735f 616c 7068 6120 616e 6420   t.is_alpha and 
-0000a690: 742e 6865 6164 2e69 735f 616c 7068 613a  t.head.is_alpha:
-0000a6a0: 0a09 0909 6172 722e 6578 7465 6e64 285b  ....arr.extend([
-0000a6b0: 6622 7b74 2e68 6561 642e 6c65 6d6d 615f  f"{t.head.lemma_
-0000a6c0: 7d3a 7b74 2e68 6561 642e 706f 735f 7d3a  }:{t.head.pos_}:
-0000a6d0: 7b74 2e64 6570 5f7d 3a7b 742e 706f 735f  {t.dep_}:{t.pos_
-0000a6e0: 7d3a 7b74 2e6c 656d 6d61 5f7d 222c 2066  }:{t.lemma_}", f
-0000a6f0: 227b 742e 6865 6164 2e6c 656d 6d61 5f7d  "{t.head.lemma_}
-0000a700: 3a7b 742e 6865 6164 2e70 6f73 5f7d 3a7b  :{t.head.pos_}:{
-0000a710: 742e 6465 705f 7d3a 7b74 2e70 6f73 5f7d  t.dep_}:{t.pos_}
-0000a720: 222c 6622 7b74 2e68 6561 642e 6c65 6d6d  ",f"{t.head.lemm
-0000a730: 615f 7d3a 7b74 2e68 6561 642e 706f 735f  a_}:{t.head.pos_
-0000a740: 7d3a 7b74 2e64 6570 5f7d 222c 2066 222a  }:{t.dep_}", f"*
-0000a750: 3a7b 742e 6865 6164 2e70 6f73 5f7d 3a7b  :{t.head.pos_}:{
-0000a760: 742e 6465 705f 7d22 2c20 6622 2a3a 7b74  t.dep_}", f"*:{t
-0000a770: 2e68 6561 642e 706f 735f 7d3a 7b74 2e64  .head.pos_}:{t.d
-0000a780: 6570 5f7d 3a7b 742e 706f 735f 7d3a 7b74  ep_}:{t.pos_}:{t
-0000a790: 2e68 6561 642e 6c65 6d6d 615f 7d22 5d29  .head.lemma_}"])
-0000a7a0: 0a09 0909 6966 2074 2e64 6570 5f20 6e6f  ....if t.dep_ no
-0000a7b0: 7420 696e 2028 2752 4f4f 5427 293a 200a  t in ('ROOT'): .
-0000a7c0: 0909 0909 6172 722e 6578 7465 6e64 285b  ....arr.extend([
-0000a7d0: 6622 7b74 2e6c 656d 6d61 5f7d 3a7b 742e  f"{t.lemma_}:{t.
-0000a7e0: 706f 735f 7d3a 7e7b 742e 6465 705f 7d3a  pos_}:~{t.dep_}:
-0000a7f0: 7b74 2e68 6561 642e 706f 735f 7d3a 7b74  {t.head.pos_}:{t
-0000a800: 2e68 6561 642e 6c65 6d6d 615f 7d22 2c20  .head.lemma_}", 
-0000a810: 6622 7b74 2e6c 656d 6d61 5f7d 3a7b 742e  f"{t.lemma_}:{t.
-0000a820: 706f 735f 7d3a 7e7b 742e 6465 705f 7d3a  pos_}:~{t.dep_}:
-0000a830: 7b74 2e68 6561 642e 706f 735f 7d22 2c20  {t.head.pos_}", 
-0000a840: 6622 7b74 2e6c 656d 6d61 5f7d 3a7b 742e  f"{t.lemma_}:{t.
-0000a850: 706f 735f 7d3a 7e7b 742e 6465 705f 7d22  pos_}:~{t.dep_}"
-0000a860: 2c20 6622 2a3a 7b74 2e70 6f73 5f7d 3a7e  , f"*:{t.pos_}:~
-0000a870: 7b74 2e64 6570 5f7d 222c 2066 222a 3a7b  {t.dep_}", f"*:{
-0000a880: 742e 706f 735f 7d3a 7e7b 742e 6465 705f  t.pos_}:~{t.dep_
-0000a890: 7d3a 7b74 2e68 6561 642e 706f 735f 7d3a  }:{t.head.pos_}:
-0000a8a0: 7b74 2e6c 656d 6d61 5f7d 225d 290a 0a09  {t.lemma_}"])...
-0000a8b0: 666f 7220 6e61 6d65 2c20 6172 2069 6e20  for name, ar in 
-0000a8c0: 6465 706d 6174 6368 2829 2864 6f63 293a  depmatch()(doc):
-0000a8d0: 2023 2074 7270 780a 0909 7430 2c74 312c   # trpx...t0,t1,
-0000a8e0: 7432 203d 2064 6f63 5b61 725b 305d 5d2c  t2 = doc[ar[0]],
-0000a8f0: 646f 635b 6172 5b31 5d5d 2c64 6f63 5b61  doc[ar[1]],doc[a
-0000a900: 725b 325d 5d0a 0909 6e61 6d65 203d 2020  r[2]]...name =  
-0000a910: 7370 6163 792e 6e6c 702e 766f 6361 625b  spacy.nlp.vocab[
-0000a920: 6e61 6d65 5d2e 7465 7874 200a 0909 6966  name].text ...if
-0000a930: 206e 616d 6520 696e 2028 2022 6e73 7562   name in ( "nsub
-0000a940: 6a2d 6163 6f6d 7022 2c20 226e 7375 626a  j-acomp", "nsubj
-0000a950: 2d61 7474 7222 293a 2020 0a09 0909 6172  -attr"):  ....ar
-0000a960: 722e 6578 7465 6e64 285b 6622 7b74 312e  r.extend([f"{t1.
-0000a970: 6c65 6d6d 615f 7d3a 7b74 312e 706f 735f  lemma_}:{t1.pos_
-0000a980: 7d3a 7b6e 616d 657d 3a7b 7432 2e70 6f73  }:{name}:{t2.pos
-0000a990: 5f7d 3a7b 7432 2e6c 656d 6d61 5f7d 222c  _}:{t2.lemma_}",
-0000a9a0: 6622 7b74 312e 6c65 6d6d 615f 7d3a 7b74  f"{t1.lemma_}:{t
-0000a9b0: 312e 706f 735f 7d3a 7b6e 616d 657d 3a7b  1.pos_}:{name}:{
-0000a9c0: 7432 2e70 6f73 5f7d 222c 6622 7b74 312e  t2.pos_}",f"{t1.
-0000a9d0: 6c65 6d6d 615f 7d3a 7b74 312e 706f 735f  lemma_}:{t1.pos_
-0000a9e0: 7d3a 7b6e 616d 657d 225d 290a 0909 0961  }:{name}"])....a
-0000a9f0: 7272 2e65 7874 656e 6428 5b66 227b 7432  rr.extend([f"{t2
-0000aa00: 2e6c 656d 6d61 5f7d 3a7b 7432 2e70 6f73  .lemma_}:{t2.pos
-0000aa10: 5f7d 3a7e 7b6e 616d 657d 3a7b 7431 2e70  _}:~{name}:{t1.p
-0000aa20: 6f73 5f7d 3a7b 7431 2e6c 656d 6d61 5f7d  os_}:{t1.lemma_}
-0000aa30: 222c 2066 227b 7432 2e6c 656d 6d61 5f7d  ", f"{t2.lemma_}
-0000aa40: 3a7b 7432 2e70 6f73 5f7d 3a7e 7b6e 616d  :{t2.pos_}:~{nam
-0000aa50: 657d 3a7b 7431 2e70 6f73 5f7d 222c 2066  e}:{t1.pos_}", f
-0000aa60: 227b 7432 2e6c 656d 6d61 5f7d 3a7b 7432  "{t2.lemma_}:{t2
-0000aa70: 2e70 6f73 5f7d 3a7e 7b6e 616d 657d 225d  .pos_}:~{name}"]
-0000aa80: 290a 0909 656c 6966 206e 616d 6520 696e  )...elif name in
-0000aa90: 2028 2261 6476 636c 2d61 636f 6d70 222c   ("advcl-acomp",
-0000aaa0: 2261 636f 6d70 2d70 7265 7022 2920 3a20  "acomp-prep") : 
-0000aab0: 090a 0909 0961 7272 2e65 7874 656e 6428  .....arr.extend(
-0000aac0: 5b66 227b 7430 2e6c 656d 6d61 5f7d 3a7b  [f"{t0.lemma_}:{
-0000aad0: 7430 2e70 6f73 5f7d 3a7b 6e61 6d65 7d3a  t0.pos_}:{name}:
-0000aae0: 7b74 322e 706f 735f 7d3a 7b74 322e 6c65  {t2.pos_}:{t2.le
-0000aaf0: 6d6d 615f 7d22 2c66 227b 7430 2e6c 656d  mma_}",f"{t0.lem
-0000ab00: 6d61 5f7d 3a7b 7430 2e70 6f73 5f7d 3a7b  ma_}:{t0.pos_}:{
-0000ab10: 6e61 6d65 7d3a 7b74 322e 706f 735f 7d22  name}:{t2.pos_}"
-0000ab20: 2c66 227b 7430 2e6c 656d 6d61 5f7d 3a7b  ,f"{t0.lemma_}:{
-0000ab30: 7430 2e70 6f73 5f7d 3a7b 6e61 6d65 7d22  t0.pos_}:{name}"
-0000ab40: 5d29 0a09 0909 6172 722e 6578 7465 6e64  ])....arr.extend
-0000ab50: 285b 6622 7b74 322e 6c65 6d6d 615f 7d3a  ([f"{t2.lemma_}:
-0000ab60: 7b74 322e 706f 735f 7d3a 7e7b 6e61 6d65  {t2.pos_}:~{name
-0000ab70: 7d3a 7b74 302e 706f 735f 7d3a 7b74 302e  }:{t0.pos_}:{t0.
-0000ab80: 6c65 6d6d 615f 7d22 2c66 227b 7432 2e6c  lemma_}",f"{t2.l
-0000ab90: 656d 6d61 5f7d 3a7b 7432 2e70 6f73 5f7d  emma_}:{t2.pos_}
-0000aba0: 3a7e 7b6e 616d 657d 3a7b 7430 2e70 6f73  :~{name}:{t0.pos
-0000abb0: 5f7d 222c 6622 7b74 322e 6c65 6d6d 615f  _}",f"{t2.lemma_
-0000abc0: 7d3a 7b74 322e 706f 735f 7d3a 7e7b 6e61  }:{t2.pos_}:~{na
-0000abd0: 6d65 7d22 5d29 0a09 0965 6c69 6620 6e61  me}"])...elif na
-0000abe0: 6d65 2069 6e20 2822 646f 626a 2d70 7274  me in ("dobj-prt
-0000abf0: 2229 2061 6e64 2074 322e 706f 735f 206e  ") and t2.pos_ n
-0000ac00: 6f74 2069 6e20 2827 5052 4f50 4e27 293a  ot in ('PROPN'):
-0000ac10: 2009 0a09 0909 6172 722e 6170 7065 6e64   .....arr.append
-0000ac20: 2866 227b 7430 2e6c 656d 6d61 5f7d 5f7b  (f"{t0.lemma_}_{
-0000ac30: 7431 2e6c 656d 6d61 5f7d 3a7b 7430 2e70  t1.lemma_}:{t0.p
-0000ac40: 6f73 5f7d 3a64 6f62 6a3a 7b74 322e 706f  os_}:dobj:{t2.po
-0000ac50: 735f 7d3a 7b74 322e 6c65 6d6d 615f 7d22  s_}:{t2.lemma_}"
-0000ac60: 290a 0909 0961 7272 2e61 7070 656e 6428  )....arr.append(
-0000ac70: 6622 7b74 322e 6c65 6d6d 615f 7d3a 7b74  f"{t2.lemma_}:{t
-0000ac80: 322e 706f 735f 7d3a 7e64 6f62 6a3a 7b74  2.pos_}:~dobj:{t
-0000ac90: 302e 706f 735f 7d3a 7b74 302e 6c65 6d6d  0.pos_}:{t0.lemm
-0000aca0: 615f 7d5f 7b74 312e 6c65 6d6d 615f 7d22  a_}_{t1.lemma_}"
-0000acb0: 290a 0909 656c 6966 206e 616d 6520 696e  )...elif name in
-0000acc0: 2028 2262 652d 7662 6e2d 7072 6570 2229   ("be-vbn-prep")
-0000acd0: 203a 2009 2362 6173 653a 5645 5242 3a62   : .#base:VERB:b
-0000ace0: 652d 7662 6e2d 7072 6570 3a62 6520 6261  e-vbn-prep:be ba
-0000acf0: 7365 6420 6f6e 0a09 0909 6172 722e 6578  sed on....arr.ex
-0000ad00: 7465 6e64 285b 6622 7b74 302e 6c65 6d6d  tend([f"{t0.lemm
-0000ad10: 615f 7d3a 7b74 302e 706f 735f 7d3a 7b6e  a_}:{t0.pos_}:{n
-0000ad20: 616d 657d 3a7b 7431 2e6c 656d 6d61 5f7d  ame}:{t1.lemma_}
-0000ad30: 207b 7430 2e74 6578 742e 6c6f 7765 7228   {t0.text.lower(
-0000ad40: 297d 207b 7432 2e74 6578 742e 6c6f 7765  )} {t2.text.lowe
-0000ad50: 7228 297d 222c 6622 7b74 302e 6c65 6d6d  r()}",f"{t0.lemm
-0000ad60: 615f 7d3a 7b74 302e 706f 735f 7d3a 7b6e  a_}:{t0.pos_}:{n
-0000ad70: 616d 657d 225d 290a 0909 090a 0966 6f72  ame}"])......for
-0000ad80: 2073 7020 696e 2064 6f63 2e6e 6f75 6e5f   sp in doc.noun_
-0000ad90: 6368 756e 6b73 3a20 2362 6f6f 6b3a 4e4f  chunks: #book:NO
-0000ada0: 554e 3a6e 703a 6120 626f 6f6b 0a09 0961  UN:np:a book...a
-0000adb0: 7272 2e65 7874 656e 6428 5b66 227b 7370  rr.extend([f"{sp
-0000adc0: 2e72 6f6f 742e 6c65 6d6d 615f 2e6c 6f77  .root.lemma_.low
-0000add0: 6572 2829 7d3a 7b73 702e 726f 6f74 2e70  er()}:{sp.root.p
-0000ade0: 6f73 5f7d 3a6e 703a 7b73 702e 7465 7874  os_}:np:{sp.text
-0000adf0: 2e6c 6f77 6572 2829 7d22 2c20 6622 7b73  .lower()}", f"{s
-0000ae00: 702e 726f 6f74 2e6c 656d 6d61 5f2e 6c6f  p.root.lemma_.lo
-0000ae10: 7765 7228 297d 3a7b 7370 2e72 6f6f 742e  wer()}:{sp.root.
-0000ae20: 706f 735f 7d3a 6e70 222c 2066 222a 3a7b  pos_}:np", f"*:{
-0000ae30: 7370 2e72 6f6f 742e 706f 735f 7d3a 6e70  sp.root.pos_}:np
-0000ae40: 222c 2066 222a 3a6e 7022 5d29 0a09 666f  ", f"*:np"])..fo
-0000ae50: 7220 6c65 6d2c 2070 6f73 2c20 7479 7065  r lem, pos, type
-0000ae60: 2c20 6368 756e 6b20 696e 206b 705f 6d61  , chunk in kp_ma
-0000ae70: 7463 6865 7228 646f 6329 3a20 2362 7269  tcher(doc): #bri
-0000ae80: 6e6b 3a4e 4f55 4e3a 7070 3a6f 6e20 7468  nk:NOUN:pp:on th
-0000ae90: 6520 6272 696e 6b20 2009 2320 5b28 2770  e brink  .# [('p
-0000aea0: 7027 2c20 276f 6e20 7468 6520 6272 696e  p', 'on the brin
-0000aeb0: 6b27 2c20 322c 2035 292c 2028 2761 7027  k', 2, 5), ('ap'
-0000aec0: 2c20 2776 6572 7920 6861 7070 7927 2c20  , 'very happy', 
-0000aed0: 392c 2031 3129 5d0a 0909 6172 722e 6578  9, 11)]...arr.ex
-0000aee0: 7465 6e64 285b 6622 7b6c 656d 7d3a 7b70  tend([f"{lem}:{p
-0000aef0: 6f73 7d3a 7b74 7970 657d 3a7b 6368 756e  os}:{type}:{chun
-0000af00: 6b7d 222c 2066 227b 6c65 6d7d 3a7b 706f  k}", f"{lem}:{po
-0000af10: 737d 3a7b 7479 7065 7d22 2c20 6622 2a3a  s}:{type}", f"*:
-0000af20: 7b70 6f73 7d3a 7b74 7970 657d 222c 2066  {pos}:{type}", f
-0000af30: 222a 3a7b 7479 7065 7d22 5d29 0a09 666f  "*:{type}"])..fo
-0000af40: 7220 7472 7078 2c20 726f 7720 696e 2064  r trpx, row in d
-0000af50: 6570 5f6d 6174 6368 6572 2864 6f63 293a  ep_matcher(doc):
-0000af60: 2023 5b28 2773 7678 272c 205b 312c 2030   #[('svx', [1, 0
-0000af70: 2c20 325d 295d 2023 2320 636f 6e73 6964  , 2])] ## consid
-0000af80: 6572 3a56 4552 423a 766e 706e 3a2a 2a2a  er:VERB:vnpn:***
-0000af90: 2a20 0a09 0976 6572 6269 203d 2072 6f77  * ...verbi = row
-0000afa0: 5b30 5d20 2363 6f6e 7369 6465 723a 5645  [0] #consider:VE
-0000afb0: 5242 3a62 655f 7662 6e5f 703a 6265 2063  RB:be_vbn_p:be c
-0000afc0: 6f6e 7369 6465 7265 6420 6173 0a09 0961  onsidered as...a
-0000afd0: 7272 2e65 7874 656e 6428 5b66 227b 646f  rr.extend([f"{do
-0000afe0: 635b 7665 7262 695d 2e6c 656d 6d61 5f7d  c[verbi].lemma_}
-0000aff0: 3a7b 646f 635b 7665 7262 695d 2e70 6f73  :{doc[verbi].pos
-0000b000: 5f7d 3a7b 7472 7078 7d22 2c20 6622 2a3a  _}:{trpx}", f"*:
-0000b010: 7b64 6f63 5b76 6572 6269 5d2e 706f 735f  {doc[verbi].pos_
-0000b020: 7d3a 7b74 7270 787d 222c 2066 222a 3a7b  }:{trpx}", f"*:{
-0000b030: 7472 7078 7d22 5d29 2023 636f 6e73 6964  trpx}"]) #consid
-0000b040: 6572 3a56 4552 423a 7376 780a 0909 6966  er:VERB:svx...if
-0000b050: 2074 7270 7820 3d3d 2027 7376 6127 2061   trpx == 'sva' a
-0000b060: 6e64 2064 6f63 5b72 6f77 5b30 5d5d 2e6c  nd doc[row[0]].l
-0000b070: 656d 6d61 5f20 3d3d 2027 6265 273a 2023  emma_ == 'be': #
-0000b080: 2066 6174 6520 6973 2073 6561 6c65 642c   fate is sealed,
-0000b090: 2061 6464 6564 2032 3032 322e 372e 3235   added 2022.7.25
-0000b0a0: 0a09 0909 6172 722e 6578 7465 6e64 285b  ....arr.extend([
-0000b0b0: 6622 7b64 6f63 5b72 6f77 5b31 5d5d 2e6c  f"{doc[row[1]].l
-0000b0c0: 656d 6d61 5f7d 3a7b 646f 635b 726f 775b  emma_}:{doc[row[
-0000b0d0: 315d 5d2e 706f 735f 7d3a 7362 6561 3a7b  1]].pos_}:sbea:{
-0000b0e0: 646f 635b 726f 775b 325d 5d2e 706f 735f  doc[row[2]].pos_
-0000b0f0: 7d3a 7b64 6f63 5b72 6f77 5b32 5d5d 2e6c  }:{doc[row[2]].l
-0000b100: 656d 6d61 5f7d 222c 2066 227b 646f 635b  emma_}", f"{doc[
-0000b110: 726f 775b 315d 5d2e 6c65 6d6d 615f 7d3a  row[1]].lemma_}:
-0000b120: 7b64 6f63 5b72 6f77 5b31 5d5d 2e70 6f73  {doc[row[1]].pos
-0000b130: 5f7d 3a73 6265 6122 2c20 6622 2a3a 7b64  _}:sbea", f"*:{d
-0000b140: 6f63 5b72 6f77 5b31 5d5d 2e70 6f73 5f7d  oc[row[1]].pos_}
-0000b150: 3a73 6265 6122 5d29 0a09 0909 6172 722e  :sbea"])....arr.
-0000b160: 6578 7465 6e64 285b 6622 7b64 6f63 5b72  extend([f"{doc[r
-0000b170: 6f77 5b32 5d5d 2e6c 656d 6d61 5f7d 3a7b  ow[2]].lemma_}:{
-0000b180: 646f 635b 726f 775b 325d 5d2e 706f 735f  doc[row[2]].pos_
-0000b190: 7d3a 7e73 6265 613a 7b64 6f63 5b72 6f77  }:~sbea:{doc[row
-0000b1a0: 5b31 5d5d 2e70 6f73 5f7d 3a7b 646f 635b  [1]].pos_}:{doc[
-0000b1b0: 726f 775b 315d 5d2e 6c65 6d6d 615f 7d22  row[1]].lemma_}"
-0000b1c0: 2c20 6622 7b64 6f63 5b72 6f77 5b32 5d5d  , f"{doc[row[2]]
-0000b1d0: 2e6c 656d 6d61 5f7d 3a7b 646f 635b 726f  .lemma_}:{doc[ro
-0000b1e0: 775b 325d 5d2e 706f 735f 7d3a 7e73 6265  w[2]].pos_}:~sbe
-0000b1f0: 6122 2c20 6622 2a3a 7b64 6f63 5b72 6f77  a", f"*:{doc[row
-0000b200: 5b32 5d5d 2e70 6f73 5f7d 3a7e 7362 6561  [2]].pos_}:~sbea
-0000b210: 225d 290a 0966 6f72 2072 6f77 2069 6e20  "])..for row in 
-0000b220: 7665 7262 6e65 745f 6d61 7463 6865 7228  verbnet_matcher(
-0000b230: 646f 6329 3a20 235b 2831 2c20 302c 2033  doc): #[(1, 0, 3
-0000b240: 2c20 274e 5020 5620 535f 494e 4727 295d  , 'NP V S_ING')]
-0000b250: 2023 206c 6173 7420 746f 2062 6520 6361   # last to be ca
-0000b260: 6c6c 6564 2c20 7369 6e63 6520 4e50 2069  lled, since NP i
-0000b270: 7320 6d65 7267 6564 0a09 0969 6620 6c65  s merged...if le
-0000b280: 6e28 726f 7729 203d 3d20 343a 200a 0909  n(row) == 4: ...
-0000b290: 0976 6572 6269 2c20 6962 6567 2c20 6965  .verbi, ibeg, ie
-0000b2a0: 6e64 2c20 6368 756e 6b20 3d20 726f 770a  nd, chunk = row.
-0000b2b0: 0909 0969 6620 646f 635b 7665 7262 695d  ...if doc[verbi]
-0000b2c0: 2e6c 656d 6d61 5f2e 6973 616c 7068 6128  .lemma_.isalpha(
-0000b2d0: 2920 3a20 0a09 0909 0961 7272 2e61 7070  ) : .....arr.app
-0000b2e0: 656e 6428 6622 7b64 6f63 5b76 6572 6269  end(f"{doc[verbi
-0000b2f0: 5d2e 6c65 6d6d 615f 7d3a 7b64 6f63 5b76  ].lemma_}:{doc[v
-0000b300: 6572 6269 5d2e 706f 735f 7d3a 7665 7262  erbi].pos_}:verb
-0000b310: 6e65 743a 7b63 6875 6e6b 7d22 2920 2363  net:{chunk}") #c
-0000b320: 6f6e 7369 6465 723a 5645 5242 3a76 6572  onsider:VERB:ver
-0000b330: 626e 6574 3a4e 5020 5620 535f 494e 470a  bnet:NP V S_ING.
-0000b340: 0966 6f72 206e 616d 652c 6962 6567 2c69  .for name,ibeg,i
-0000b350: 656e 6420 696e 2070 6f73 745f 6e70 5f6d  end in post_np_m
-0000b360: 6174 6368 6572 2864 6f63 293a 2023 6164  atcher(doc): #ad
-0000b370: 6465 6420 3230 3232 2e37 2e32 350a 0909  ded 2022.7.25...
-0000b380: 6966 206e 616d 6520 696e 2028 2776 5f6e  if name in ('v_n
-0000b390: 5f76 626e 272c 2776 5f6e 5f61 646a 2729  _vbn','v_n_adj')
-0000b3a0: 3a20 0a09 0909 6172 722e 6578 7465 6e64  : ....arr.extend
-0000b3b0: 285b 6622 7b64 6f63 5b69 6265 675d 2e6c  ([f"{doc[ibeg].l
-0000b3c0: 656d 6d61 5f7d 3a7b 646f 635b 6962 6567  emma_}:{doc[ibeg
-0000b3d0: 5d2e 706f 735f 7d3a 7b6e 616d 657d 3a7b  ].pos_}:{name}:{
-0000b3e0: 646f 635b 6962 6567 5d2e 6c65 6d6d 615f  doc[ibeg].lemma_
-0000b3f0: 7d20 7b64 6f63 5b69 6265 672b 315d 2e6c  } {doc[ibeg+1].l
-0000b400: 656d 6d61 5f7d 207b 646f 635b 6962 6567  emma_} {doc[ibeg
-0000b410: 2b32 5d2e 7465 7874 7d22 2c20 6622 7b64  +2].text}", f"{d
-0000b420: 6f63 5b69 6265 675d 2e6c 656d 6d61 5f7d  oc[ibeg].lemma_}
-0000b430: 3a7b 646f 635b 6962 6567 5d2e 706f 735f  :{doc[ibeg].pos_
-0000b440: 7d3a 7b6e 616d 657d 222c 2066 222a 3a7b  }:{name}", f"*:{
-0000b450: 646f 635b 6962 6567 5d2e 706f 735f 7d3a  doc[ibeg].pos_}:
-0000b460: 7b6e 616d 657d 225d 290a 0972 6574 7572  {name}"])..retur
-0000b470: 6e20 6172 7220 0a0a 6973 4e50 093d 206c  n arr ..isNP.= l
-0000b480: 616d 6264 6120 743a 2074 2e65 6e74 5f74  ambda t: t.ent_t
-0000b490: 7970 655f 203d 3d20 274e 5027 2061 6e64  ype_ == 'NP' and
-0000b4a0: 2027 2027 2069 6e20 742e 7465 7874 2023   ' ' in t.text #
-0000b4b0: 206c 656e 203e 2031 200a 646f 6374 6f6b   len > 1 .doctok
-0000b4c0: 7320 3d20 6c61 6d62 6461 2064 6f63 3a20  s = lambda doc: 
-0000b4d0: 5b27 3c73 3e27 5d20 2b20 5b20 6622 5f7b  ['<s>'] + [ f"_{
-0000b4e0: 742e 706f 735f 7d22 2069 6620 742e 706f  t.pos_}" if t.po
-0000b4f0: 735f 2069 6e20 2827 5052 4f50 4e27 2c27  s_ in ('PROPN','
-0000b500: 4e55 4d27 2c27 4344 272c 2758 272c 2753  NUM','CD','X','S
-0000b510: 5041 4345 2729 2065 6c73 6520 225f 4e50  PACE') else "_NP
-0000b520: 2220 6966 2069 734e 5028 7429 2065 6c73  " if isNP(t) els
-0000b530: 6520 742e 7465 7874 2e6c 6f77 6572 2829  e t.text.lower()
-0000b540: 2020 666f 7220 7420 696e 2064 6f63 205d    for t in doc ]
-0000b550: 0a64 6566 206e 6772 616d 2874 6f6b 732c  .def ngram(toks,
-0000b560: 206e 3a69 6e74 3d33 293a 200a 0974 7320   n:int=3): ..ts 
-0000b570: 3d20 7365 7428 2920 0a09 746c 656e 203d  = set() ..tlen =
-0000b580: 2020 6c65 6e28 746f 6b73 290a 0966 6f72    len(toks)..for
-0000b590: 2069 2069 6e20 7261 6e67 6528 2074 6c65   i in range( tle
-0000b5a0: 6e20 293a 200a 0909 666f 7220 6a20 696e  n ): ...for j in
-0000b5b0: 2072 616e 6765 286e 293a 200a 0909 0969   range(n): ....i
-0000b5c0: 6620 692b 6a20 3c20 746c 656e 3a20 0a09  f i+j < tlen: ..
-0000b5d0: 0909 0974 732e 6164 6428 2022 2022 2e6a  ...ts.add( " ".j
-0000b5e0: 6f69 6e28 746f 6b73 5b69 3a69 2b6a 5d29  oin(toks[i:i+j])
-0000b5f0: 2029 0a09 7265 7475 726e 205b 7420 666f   )..return [t fo
-0000b600: 7220 7420 696e 2074 7320 6966 2074 2061  r t in ts if t a
-0000b610: 6e64 206e 6f74 2027 2e27 2069 6e20 745d  nd not '.' in t]
-0000b620: 0a0a 6465 6620 6334 6765 7428 6772 616d  ..def c4get(gram
-0000b630: 733a 6c69 7374 3d5b 273c 733e 2069 7327  s:list=['<s> is'
-0000b640: 2c27 6a75 6d70 6564 206f 7665 7220 5f4e  ,'jumped over _N
-0000b650: 5027 5d2c 206e 616d 653d 2763 3467 7261  P'], name='c4gra
-0000b660: 6d27 293a 2020 0a09 6966 206e 6f74 2068  m'):  ..if not h
-0000b670: 6173 6174 7472 2863 3467 6574 2c6e 616d  asattr(c4get,nam
-0000b680: 6529 3a20 7365 7461 7474 7228 2063 3467  e): setattr( c4g
-0000b690: 6574 2c20 6e61 6d65 2c20 7371 6c69 7465  et, name, sqlite
-0000b6a0: 332e 636f 6e6e 6563 7428 6622 2f64 6174  3.connect(f"/dat
-0000b6b0: 612f 6d6f 6465 6c2f 6334 2f7b 6e61 6d65  a/model/c4/{name
-0000b6c0: 7d2e 7369 222c 2063 6865 636b 5f73 616d  }.si", check_sam
-0000b6d0: 655f 7468 7265 6164 3d46 616c 7365 2920  e_thread=False) 
-0000b6e0: 2920 200a 0972 6574 7572 6e20 7b20 726f  )  ..return { ro
-0000b6f0: 775b 305d 203a 2072 6f77 5b31 5d20 666f  w[0] : row[1] fo
-0000b700: 7220 726f 7720 696e 2067 6574 6174 7472  r row in getattr
-0000b710: 2863 3467 6574 2c20 6e61 6d65 292e 6578  (c4get, name).ex
-0000b720: 6563 7574 6528 2273 656c 6563 7420 732c  ecute("select s,
-0000b730: 6920 6672 6f6d 2073 6920 7768 6572 6520  i from si where 
-0000b740: 7320 696e 2028 2722 2b22 272c 2722 2e6a  s in ('"+"','".j
-0000b750: 6f69 6e28 5b6b 2066 6f72 206b 2069 6e20  oin([k for k in 
-0000b760: 6772 616d 7320 6966 206e 6f74 2022 2722  grams if not "'"
-0000b770: 2069 6e20 6b5d 292b 2227 2922 2920 7d20   in k])+"')") } 
-0000b780: 0a0a 6465 6620 6e67 7261 6d5f 6368 6563  ..def ngram_chec
-0000b790: 6b28 7465 7874 3a73 7472 3d22 5468 6520  k(text:str="The 
-0000b7a0: 7175 6963 6b20 666f 7820 6a75 6d70 6564  quick fox jumped
-0000b7b0: 206f 7665 7220 7468 6520 6c61 7a79 2064   over the lazy d
-0000b7c0: 6f67 2e22 2c20 6e3a 696e 743d 3329 3a0a  og.", n:int=3):.
-0000b7d0: 0964 6f63 203d 2073 7061 6379 2e6e 6c70  .doc = spacy.nlp
-0000b7e0: 2874 6578 7429 0a09 6d65 7267 655f 6e70  (text)..merge_np
-0000b7f0: 2864 6f63 2920 0a09 746f 6b73 093d 2064  (doc) ..toks.= d
-0000b800: 6f63 746f 6b73 2864 6f63 290a 0967 7261  octoks(doc)..gra
-0000b810: 6d73 093d 206e 6772 616d 2874 6f6b 732c  ms.= ngram(toks,
-0000b820: 206e 290a 0964 6963 0909 3d20 6334 6765   n)..dic..= c4ge
-0000b830: 7428 6772 616d 7329 200a 0972 6574 7572  t(grams) ..retur
-0000b840: 6e20 5b20 7b22 6772 616d 223a 2077 2c20  n [ {"gram": w, 
-0000b850: 2263 6e74 223a 2064 6963 2e67 6574 2877  "cnt": dic.get(w
-0000b860: 2c30 2920 7d20 666f 7220 7720 696e 2063  ,0) } for w in c
-0000b870: 686b 5d0a 0a64 6566 2067 7261 6d28 646f  hk]..def gram(do
-0000b880: 632c 206e 3a69 6e74 3d37 293a 0a09 7473  c, n:int=7):..ts
-0000b890: 203d 2073 6574 2829 200a 0964 6566 2063   = set() ..def c
-0000b8a0: 6f75 6e74 2874 6f6b 732c 2074 732c 206e  ount(toks, ts, n
-0000b8b0: 293a 2023 2074 733a 2073 6574 200a 0909  ): # ts: set ...
-0000b8c0: 746c 656e 203d 2020 6c65 6e28 746f 6b73  tlen =  len(toks
-0000b8d0: 290a 0909 666f 7220 6920 696e 2072 616e  )...for i in ran
-0000b8e0: 6765 2820 746c 656e 2029 3a20 0a09 0909  ge( tlen ): ....
-0000b8f0: 666f 7220 6a20 696e 2072 616e 6765 286e  for j in range(n
-0000b900: 293a 200a 0909 0909 6966 2069 2b6a 203c  ): .....if i+j <
-0000b910: 2074 6c65 6e3a 200a 0909 0909 0974 732e   tlen: ......ts.
-0000b920: 6164 6428 2022 2022 2e6a 6f69 6e28 746f  add( " ".join(to
-0000b930: 6b73 5b69 3a69 2b6a 5d29 2029 0a0a 0963  ks[i:i+j]) )...c
-0000b940: 6f75 6e74 2820 646f 6374 6f6b 7328 646f  ount( doctoks(do
-0000b950: 6329 2c20 7473 2c20 6e29 200a 096d 6572  c), ts, n) ..mer
-0000b960: 6765 5f6e 7028 646f 6329 200a 0963 6f75  ge_np(doc) ..cou
-0000b970: 6e74 2820 646f 6374 6f6b 7328 646f 6329  nt( doctoks(doc)
-0000b980: 2c20 7473 2c20 6e29 200a 0972 6574 7572  , ts, n) ..retur
-0000b990: 6e20 227c 222e 6a6f 696e 285b 7420 666f  n "|".join([t fo
-0000b9a0: 7220 7420 696e 2074 7320 6966 2074 5d29  r t in ts if t])
-0000b9b0: 0a0a 6465 6620 7371 6c63 6f6e 6e28 6f75  ..def sqlconn(ou
-0000b9c0: 7466 696c 652c 2073 716c 733a 7374 723d  tfile, sqls:str=
-0000b9d0: 5b22 6372 6561 7465 2074 6162 6c65 2069  ["create table i
-0000b9e0: 6620 6e6f 7420 6578 6973 7473 2073 6928  f not exists si(
-0000b9f0: 2073 2076 6172 6368 6172 2836 3429 206e   s varchar(64) n
-0000ba00: 6f74 206e 756c 6c20 7072 696d 6172 7920  ot null primary 
-0000ba10: 6b65 792c 2069 2069 6e74 206e 6f74 206e  key, i int not n
-0000ba20: 756c 6c20 6465 6661 756c 7420 3029 2077  ull default 0) w
-0000ba30: 6974 686f 7574 2072 6f77 6964 222c 2263  ithout rowid","c
-0000ba40: 7265 6174 6520 7461 626c 6520 6966 206e  reate table if n
-0000ba50: 6f74 2065 7869 7374 7320 7374 2820 7320  ot exists st( s 
-0000ba60: 7661 7263 6861 7228 3634 2920 6e6f 7420  varchar(64) not 
-0000ba70: 6e75 6c6c 2070 7269 6d61 7279 206b 6579  null primary key
-0000ba80: 2c20 7420 7465 7874 2c20 636e 7420 696e  , t text, cnt in
-0000ba90: 7420 6e6f 7420 6e75 6c6c 2064 6566 6175  t not null defau
-0000baa0: 6c74 2030 2920 7769 7468 6f75 7420 726f  lt 0) without ro
-0000bab0: 7769 6422 5d29 3a0a 0963 6f6e 6e20 203d  wid"]):..conn  =
-0000bac0: 0973 716c 6974 6533 2e63 6f6e 6e65 6374  .sqlite3.connect
-0000bad0: 286f 7574 6669 6c65 2c20 6368 6563 6b5f  (outfile, check_
-0000bae0: 7361 6d65 5f74 6872 6561 643d 4661 6c73  same_thread=Fals
-0000baf0: 6529 200a 0966 6f72 2073 716c 2069 6e20  e) ..for sql in 
-0000bb00: 7371 6c73 3a20 636f 6e6e 2e65 7865 6375  sqls: conn.execu
-0000bb10: 7465 2873 716c 290a 0963 6f6e 6e2e 6578  te(sql)..conn.ex
-0000bb20: 6563 7574 6528 2750 5241 474d 4120 7379  ecute('PRAGMA sy
-0000bb30: 6e63 6872 6f6e 6f75 733d 4f46 4627 290a  nchronous=OFF').
-0000bb40: 0963 6f6e 6e2e 6578 6563 7574 6528 2750  .conn.execute('P
-0000bb50: 5241 474d 4120 6361 7365 5f73 656e 7369  RAGMA case_sensi
-0000bb60: 7469 7665 5f6c 696b 6520 3d20 3127 2920  tive_like = 1') 
-0000bb70: 2363 6f6e 6e2e 6578 6563 7574 6528 2250  #conn.execute("P
-0000bb80: 5241 474d 4120 6361 6368 655f 7369 7a65  RAGMA cache_size
-0000bb90: 203d 202d 3531 3222 2920 2009 0963 6f6e   = -512")  ..con
-0000bba0: 6e2e 6578 6563 7574 6528 2750 5241 474d  n.execute('PRAGM
-0000bbb0: 4120 6361 6368 655f 7369 7a65 203d 2032  A cache_size = 2
-0000bbc0: 3030 3030 3030 2729 2020 2320 3220 4762  000000')  # 2 Gb
-0000bbd0: 0a09 636f 6e6e 2e63 6f6d 6d69 7428 290a  ..conn.commit().
-0000bbe0: 0972 6574 7572 6e20 636f 6e6e 200a 0a64  .return conn ..d
-0000bbf0: 6566 2073 716c 7369 2869 6e66 696c 652c  ef sqlsi(infile,
-0000bc00: 2066 756e 633a 7374 723d 2774 6f6b 7472   func:str='toktr
-0000bc10: 7027 2c20 6f75 7466 696c 653a 7374 723d  p', outfile:str=
-0000bc20: 4e6f 6e65 2c62 6174 6368 3d31 3030 302c  None,batch=1000,
-0000bc30: 293a 2023 6962 6567 3a69 6e74 3d30 2c20  ): #ibeg:int=0, 
-0000bc40: 6965 6e64 3a69 6e74 3d31 3030 3030 3030  iend:int=1000000
-0000bc50: 2c0a 0927 2727 2064 6174 6120 666f 7220  ,..''' data for 
-0000bc60: 6d79 6e61 632c 2066 756e 6320 6d75 7374  mynac, func must
-0000bc70: 2065 7869 7374 202c 2066 756e 633d 7472   exist , func=tr
-0000bc80: 7078 2027 2727 0a09 6966 206f 7574 6669  px '''..if outfi
-0000bc90: 6c65 2069 7320 4e6f 6e65 206f 7220 6e6f  le is None or no
-0000bca0: 7420 6f75 7466 696c 653a 206f 7574 6669  t outfile: outfi
-0000bcb0: 6c65 203d 2069 6e66 696c 652e 7370 6c69  le = infile.spli
-0000bcc0: 7428 272e 2729 5b30 5d20 2b20 6622 2e73  t('.')[0] + f".s
-0000bcd0: 716c 7369 220a 0970 7269 6e74 2866 2273  qlsi"..print(f"s
-0000bce0: 7461 7274 6564 3a20 5b62 6174 6368 3d7b  tarted: [batch={
-0000bcf0: 6261 7463 687d 5d22 2c20 696e 6669 6c65  batch}]", infile
-0000bd00: 2c20 6f75 7466 696c 6520 2c20 6675 6e63  , outfile , func
-0000bd10: 202c 2066 6c75 7368 3d54 7275 6529 0a09   , flush=True)..
-0000bd20: 6675 6e63 203d 2067 6c6f 6261 6c73 2829  func = globals()
-0000bd30: 5b66 756e 635d 200a 0973 7461 7274 203d  [func] ..start =
-0000bd40: 2074 696d 652e 7469 6d65 2829 0a09 636f   time.time()..co
-0000bd50: 6e6e 203d 2073 716c 636f 6e6e 286f 7574  nn = sqlconn(out
-0000bd60: 6669 6c65 2920 0a09 666f 7220 7369 642c  file) ..for sid,
-0000bd70: 206c 696e 6520 696e 2065 6e75 6d65 7261   line in enumera
-0000bd80: 7465 2866 696c 6569 6e70 7574 2e69 6e70  te(fileinput.inp
-0000bd90: 7574 2869 6e66 696c 652c 6f70 656e 686f  ut(infile,openho
-0000bda0: 6f6b 3d66 696c 6569 6e70 7574 2e68 6f6f  ok=fileinput.hoo
-0000bdb0: 6b5f 636f 6d70 7265 7373 6564 2929 3a20  k_compressed)): 
-0000bdc0: 0a09 0974 7279 3a20 2369 6620 7369 6420  ...try: #if sid 
-0000bdd0: 3c20 6962 6567 203a 2063 6f6e 7469 6e75  < ibeg : continu
-0000bde0: 6520 7c09 6966 2073 6964 203e 3d20 6965  e |.if sid >= ie
-0000bdf0: 6e64 3a20 6272 6561 6b20 0a09 0909 6172  nd: break ....ar
-0000be00: 7220 3d20 6a73 6f6e 2e6c 6f61 6473 286c  r = json.loads(l
-0000be10: 696e 652e 7374 7269 7028 2929 200a 0909  ine.strip()) ...
-0000be20: 0964 6f63 203d 2073 7061 6379 2e66 726f  .doc = spacy.fro
-0000be30: 6d5f 6a73 6f6e 2861 7272 2920 200a 0909  m_json(arr)  ...
-0000be40: 0966 6f72 2074 2069 6e20 646f 633a 2020  .for t in doc:  
-0000be50: 0a09 0909 0969 6620 6e6f 7420 742e 706f  .....if not t.po
-0000be60: 735f 2069 6e20 2827 5052 4f50 4e27 2c27  s_ in ('PROPN','
-0000be70: 5827 2c20 2750 554e 4354 272c 2253 5041  X', 'PUNCT',"SPA
-0000be80: 4345 222c 2752 4f4f 5427 2c27 4e55 4d27  CE",'ROOT','NUM'
-0000be90: 2920 616e 6420 6e6f 7420 742e 6865 6164  ) and not t.head
-0000bea0: 2e70 6f73 5f20 696e 2028 2750 524f 504e  .pos_ in ('PROPN
-0000beb0: 272c 2758 272c 2027 5055 4e43 5427 2c22  ','X', 'PUNCT',"
-0000bec0: 5350 4143 4522 2c27 524f 4f54 272c 274e  SPACE",'ROOT','N
-0000bed0: 554d 2729 2061 6e64 2074 2e69 735f 616c  UM') and t.is_al
-0000bee0: 7068 6120 616e 6420 742e 6865 6164 2e69  pha and t.head.i
-0000bef0: 735f 616c 7068 613a 0a09 0909 0909 7472  s_alpha:......tr
-0000bf00: 7020 3d20 6622 7b74 2e68 6561 642e 6c65  p = f"{t.head.le
-0000bf10: 6d6d 615f 7d3a 7b74 2e68 6561 642e 706f  mma_}:{t.head.po
-0000bf20: 735f 7d3a 7b74 2e64 6570 5f7d 3a7b 742e  s_}:{t.dep_}:{t.
-0000bf30: 706f 735f 7d3a 7b74 2e6c 656d 6d61 5f7d  pos_}:{t.lemma_}
-0000bf40: 220a 0909 0909 0963 6f6e 6e2e 6578 6563  "......conn.exec
-0000bf50: 7574 6528 6622 494e 5345 5254 204f 5220  ute(f"INSERT OR 
-0000bf60: 4947 4e4f 5245 2049 4e54 4f20 7374 2873  IGNORE INTO st(s
-0000bf70: 2c74 2920 5641 4c55 4553 283f 2c3f 2922  ,t) VALUES(?,?)"
-0000bf80: 2c20 2874 7270 2c64 6f63 2e74 6578 7429  , (trp,doc.text)
-0000bf90: 290a 0909 0966 6f72 2073 2069 6e20 6675  )....for s in fu
-0000bfa0: 6e63 2864 6f63 293a 2020 0a09 0909 0963  nc(doc):  .....c
-0000bfb0: 6f6e 6e2e 6578 6563 7574 6528 6622 494e  onn.execute(f"IN
-0000bfc0: 5345 5254 2049 4e54 4f20 7369 2873 2c69  SERT INTO si(s,i
-0000bfd0: 2920 5641 4c55 4553 283f 2c3f 2920 4f4e  ) VALUES(?,?) ON
-0000bfe0: 2043 4f4e 464c 4943 5428 7329 2044 4f20   CONFLICT(s) DO 
-0000bff0: 5550 4441 5445 2053 4554 2069 203d 2069  UPDATE SET i = i
-0000c000: 202b 2031 222c 2028 732c 3129 290a 0909   + 1", (s,1))...
-0000c010: 0969 6620 2873 6964 2920 2520 6261 7463  .if (sid) % batc
-0000c020: 6820 3d3d 2030 203a 200a 0909 0909 7072  h == 0 : .....pr
-0000c030: 696e 7420 2866 2273 6964 203d 207b 7369  int (f"sid = {si
-0000c040: 647d 2c20 5c74 7c20 7573 696e 6728 7329  d}, \t| using(s)
-0000c050: 3a20 222c 2072 6f75 6e64 2874 696d 652e  : ", round(time.
-0000c060: 7469 6d65 2829 202d 2073 7461 7274 2c31  time() - start,1
-0000c070: 292c 2066 6c75 7368 3d54 7275 6529 0a09  ), flush=True)..
-0000c080: 0909 0963 6f6e 6e2e 636f 6d6d 6974 2829  ...conn.commit()
-0000c090: 2023 636f 6e6e 2e63 6c6f 7365 2829 2020   #conn.close()  
-0000c0a0: 2364 656c 2063 6f6e 6e09 0909 2363 6f6e  #del conn...#con
-0000c0b0: 6e20 3d20 7371 6c63 6f6e 6e28 6f75 7466  n = sqlconn(outf
-0000c0c0: 696c 6529 2009 0923 7370 6163 792e 6e6c  ile) ..#spacy.nl
-0000c0d0: 7009 3d20 7370 6163 792e 6c6f 6164 2827  p.= spacy.load('
-0000c0e0: 656e 5f63 6f72 655f 7765 625f 6c67 2729  en_core_web_lg')
-0000c0f0: 0a09 0909 0972 6566 7265 7368 2829 200a  .....refresh() .
-0000c100: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
-0000c110: 6f6e 2061 7320 653a 0a09 0909 7072 696e  on as e:....prin
-0000c120: 7420 2822 6578 3a22 2c20 652c 2073 6964  t ("ex:", e, sid
-0000c130: 2c20 6c69 6e65 2920 0a09 0909 6578 635f  , line) ....exc_
-0000c140: 7479 7065 2c20 6578 635f 7661 6c75 652c  type, exc_value,
-0000c150: 2065 7863 5f6f 626a 203d 2073 7973 2e65   exc_obj = sys.e
-0000c160: 7863 5f69 6e66 6f28 2920 090a 0909 0974  xc_info() .....t
-0000c170: 7261 6365 6261 636b 2e70 7269 6e74 5f74  raceback.print_t
-0000c180: 6228 6578 635f 6f62 6a29 0a09 636f 6e6e  b(exc_obj)..conn
-0000c190: 2e63 6f6d 6d69 7428 290a 0963 6f6e 6e2e  .commit()..conn.
-0000c1a0: 6578 6563 7574 6528 6622 7570 6461 7465  execute(f"update
-0000c1b0: 2073 7420 7365 7420 636e 7420 3d20 2873   st set cnt = (s
-0000c1c0: 656c 6563 7420 6920 6672 6f6d 2073 6920  elect i from si 
-0000c1d0: 7768 6572 6520 7369 2e73 203d 2073 742e  where si.s = st.
-0000c1e0: 7329 2229 0a09 636f 6e6e 2e63 6f6d 6d69  s)")..conn.commi
-0000c1f0: 7428 290a 0970 7269 6e74 2822 7371 6c73  t()..print("sqls
-0000c200: 6920 6669 6e69 7368 6564 3a22 2c20 696e  i finished:", in
-0000c210: 6669 6c65 290a 0a64 6566 2066 6173 7474  file)..def fastt
-0000c220: 6578 7428 696e 6669 6c65 2c20 6f75 7466  ext(infile, outf
-0000c230: 696c 653a 7374 723d 4e6f 6e65 2c62 6174  ile:str=None,bat
-0000c240: 6368 3d31 3030 302c 293a 200a 0927 2727  ch=1000,): ..'''
-0000c250: 2070 7265 7061 7265 2064 6174 6120 666f   prepare data fo
-0000c260: 7220 6661 7374 7465 7874 2069 6e70 7574  r fasttext input
-0000c270: 2c20 7c20 2e2f 6661 7374 7465 7874 2073  , | ./fasttext s
-0000c280: 6b69 7067 7261 6d20 2d69 6e70 7574 2064  kipgram -input d
-0000c290: 6963 2e66 6173 7474 6578 7420 2d6f 7574  ic.fasttext -out
-0000c2a0: 7075 7420 6469 6320 207c 3230 3233 2e31  put dic  |2023.1
-0000c2b0: 2e32 3620 2727 270a 0969 6620 6f75 7466  .26 '''..if outf
-0000c2c0: 696c 6520 6973 204e 6f6e 6520 6f72 206e  ile is None or n
-0000c2d0: 6f74 206f 7574 6669 6c65 3a20 6f75 7466  ot outfile: outf
-0000c2e0: 696c 6520 3d20 696e 6669 6c65 2e73 706c  ile = infile.spl
-0000c2f0: 6974 2827 2e27 295b 305d 202b 2066 222e  it('.')[0] + f".
-0000c300: 6661 7374 7465 7874 220a 0970 7269 6e74  fasttext"..print
-0000c310: 2866 2273 7461 7274 6564 3a20 5b62 6174  (f"started: [bat
-0000c320: 6368 3d7b 6261 7463 687d 5d22 2c20 696e  ch={batch}]", in
-0000c330: 6669 6c65 2c20 6f75 7466 696c 6520 2c20  file, outfile , 
-0000c340: 666c 7573 683d 5472 7565 290a 0a09 6465  flush=True)...de
-0000c350: 6620 6670 6172 7365 2864 6f63 293a 0a09  f fparse(doc):..
-0000c360: 096d 6572 6765 5f65 6e74 2864 6f63 290a  .merge_ent(doc).
-0000c370: 0909 236d 6572 6765 5f6e 7028 646f 6329  ..#merge_np(doc)
-0000c380: 2020 2320 7475 726e 5f6f 6666 2074 6865    # turn_off the
-0000c390: 2072 6164 696f 200a 0909 6d65 7267 655f   radio ...merge_
-0000c3a0: 7628 646f 6329 200a 0909 7265 7475 726e  v(doc) ...return
-0000c3b0: 2022 2022 2e6a 6f69 6e28 5b20 6622 5f7b   " ".join([ f"_{
-0000c3c0: 742e 706f 735f 7d22 2069 6620 742e 706f  t.pos_}" if t.po
-0000c3d0: 735f 2069 6e20 2822 5052 4f50 4e22 2c22  s_ in ("PROPN","
-0000c3e0: 4e55 4d22 2920 656c 7365 2066 227b 742e  NUM") else f"{t.
-0000c3f0: 6c65 6d6d 615f 7d2f 5645 5242 2220 6966  lemma_}/VERB" if
-0000c400: 2074 2e65 6e74 5f74 7970 655f 2e73 7461   t.ent_type_.sta
-0000c410: 7274 7377 6974 6828 226d 6572 6765 5f76  rtswith("merge_v
-0000c420: 3a22 2920 656c 7365 2066 225f 7b74 2e65  :") else f"_{t.e
-0000c430: 6e74 5f74 7970 655f 7d22 2069 6620 742e  nt_type_}" if t.
-0000c440: 656e 745f 7479 7065 5f20 656c 7365 2066  ent_type_ else f
-0000c450: 227b 742e 6c65 6d6d 615f 7d2f 7b74 2e70  "{t.lemma_}/{t.p
-0000c460: 6f73 5f7d 2220 6966 2074 2e70 6f73 5f20  os_}" if t.pos_ 
-0000c470: 696e 2028 2256 4552 4222 2c22 4e4f 554e  in ("VERB","NOUN
-0000c480: 222c 2022 4144 4a22 2c22 4144 5622 2920  ", "ADJ","ADV") 
-0000c490: 656c 7365 2074 2e74 6578 7420 666f 7220  else t.text for 
-0000c4a0: 7420 696e 2064 6f63 5d29 0a0a 0973 7461  t in doc])...sta
-0000c4b0: 7274 203d 2074 696d 652e 7469 6d65 2829  rt = time.time()
-0000c4c0: 0a09 7769 7468 206f 7065 6e28 6f75 7466  ..with open(outf
-0000c4d0: 696c 652c 2027 7727 2920 6173 2066 773a  ile, 'w') as fw:
-0000c4e0: 0a09 0966 6f72 2073 6964 2c20 6c69 6e65  ...for sid, line
-0000c4f0: 2069 6e20 656e 756d 6572 6174 6528 6669   in enumerate(fi
-0000c500: 6c65 696e 7075 742e 696e 7075 7428 696e  leinput.input(in
-0000c510: 6669 6c65 2c6f 7065 6e68 6f6f 6b3d 6669  file,openhook=fi
-0000c520: 6c65 696e 7075 742e 686f 6f6b 5f63 6f6d  leinput.hook_com
-0000c530: 7072 6573 7365 6429 293a 200a 0909 0974  pressed)): ....t
-0000c540: 7279 3a20 0a09 0909 0961 7272 203d 206a  ry: .....arr = j
-0000c550: 736f 6e2e 6c6f 6164 7328 6c69 6e65 2e73  son.loads(line.s
-0000c560: 7472 6970 2829 2920 0a09 0909 0964 6f63  trip()) .....doc
-0000c570: 203d 2073 7061 6379 2e66 726f 6d5f 6a73   = spacy.from_js
-0000c580: 6f6e 2861 7272 2920 200a 0909 0909 6677  on(arr)  .....fw
-0000c590: 2e77 7269 7465 2820 6670 6172 7365 2864  .write( fparse(d
-0000c5a0: 6f63 2920 2b20 225c 6e22 2920 0a09 0909  oc) + "\n") ....
-0000c5b0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0000c5c0: 2061 7320 653a 0a09 0909 0970 7269 6e74   as e:.....print
-0000c5d0: 2028 2265 783a 222c 2065 2c20 7369 642c   ("ex:", e, sid,
-0000c5e0: 206c 696e 6529 200a 0909 0909 6578 635f   line) .....exc_
-0000c5f0: 7479 7065 2c20 6578 635f 7661 6c75 652c  type, exc_value,
-0000c600: 2065 7863 5f6f 626a 203d 2073 7973 2e65   exc_obj = sys.e
-0000c610: 7863 5f69 6e66 6f28 2920 090a 0909 0909  xc_info() ......
-0000c620: 7472 6163 6562 6163 6b2e 7072 696e 745f  traceback.print_
-0000c630: 7462 2865 7863 5f6f 626a 290a 0970 7269  tb(exc_obj)..pri
-0000c640: 6e74 2822 6661 7374 7465 7874 2066 696e  nt("fasttext fin
-0000c650: 6973 6865 643a 222c 2069 6e66 696c 6529  ished:", infile)
-0000c660: 0a0a 6465 6620 7465 7374 2829 3a20 0a09  ..def test(): ..
-0000c670: 646f 6320 3d20 7370 6163 792e 6e6c 7028  doc = spacy.nlp(
-0000c680: 2249 7420 6973 2062 6173 6564 206f 6e20  "It is based on 
-0000c690: 7468 6520 626f 6f6b 2e22 2920 2320 2257  the book.") # "W
-0000c6a0: 6869 6c65 2049 2077 6173 2074 6872 696c  hile I was thril
-0000c6b0: 6c65 6420 7468 6174 2069 7420 7761 7320  led that it was 
-0000c6c0: 6f6b 2c20 4920 776f 7272 6965 6420 7468  ok, I worried th
-0000c6d0: 6174 2073 6865 2069 7320 6861 7070 792e  at she is happy.
-0000c6e0: 220a 0966 6f72 206e 616d 652c 2061 7220  "..for name, ar 
-0000c6f0: 696e 2064 6570 6d61 7463 6828 2928 646f  in depmatch()(do
-0000c700: 6329 203a 200a 0909 7072 696e 7428 7370  c) : ...print(sp
-0000c710: 6163 792e 6e6c 702e 766f 6361 625b 6e61  acy.nlp.vocab[na
-0000c720: 6d65 5d2e 7465 7874 2c20 646f 635b 6172  me].text, doc[ar
-0000c730: 5b30 5d5d 2e6c 656d 6d61 5f2c 2064 6f63  [0]].lemma_, doc
-0000c740: 5b61 725b 315d 5d2e 6c65 6d6d 615f 2c20  [ar[1]].lemma_, 
-0000c750: 646f 635b 6172 5b32 5d5d 290a 0970 7269  doc[ar[2]])..pri
-0000c760: 6e74 2028 2065 735f 736b 656e 7028 646f  nt ( es_skenp(do
-0000c770: 6329 2920 0a0a 6465 6620 6573 5f73 7562  c)) ..def es_sub
-0000c780: 6d69 7428 696e 6669 6c65 2c20 696e 6465  mit(infile, inde
-0000c790: 783a 7374 723d 4e6f 6e65 2c20 6261 7463  x:str=None, batc
-0000c7a0: 683d 3230 3030 3030 2c20 7265 6372 6561  h=200000, recrea
-0000c7b0: 7465 3a62 6f6f 6c3d 5472 7565 2c20 686f  te:bool=True, ho
-0000c7c0: 7374 3d27 3137 322e 3137 2e30 2e31 272c  st='172.17.0.1',
-0000c7d0: 706f 7274 3d39 3230 3029 3a20 0a09 2727  port=9200): ..''
-0000c7e0: 2720 7079 7468 6f6e 3320 2d6d 2061 7069  ' python3 -m api
-0000c7f0: 2e73 6e74 6a73 6f6e 2d65 7320 677a 6a63  .sntjson-es gzjc
-0000c800: 2e6a 736f 6e6c 672e 332e 342e 312e 677a  .jsonlg.3.4.1.gz
-0000c810: 2727 270a 0966 726f 6d20 656c 6173 7469  '''..from elasti
-0000c820: 6373 6561 7263 6820 696d 706f 7274 2045  csearch import E
-0000c830: 6c61 7374 6963 7365 6172 6368 2c68 656c  lasticsearch,hel
-0000c840: 7065 7273 0a09 696d 706f 7274 2073 6f0a  pers..import so.
-0000c850: 0965 7309 203d 2045 6c61 7374 6963 7365  .es. = Elasticse
-0000c860: 6172 6368 285b 2066 2268 7474 703a 2f2f  arch([ f"http://
-0000c870: 7b68 6f73 747d 3a7b 706f 7274 7d22 205d  {host}:{port}" ]
-0000c880: 2920 200a 0969 6620 696e 6465 7820 6973  )  ..if index is
-0000c890: 204e 6f6e 6520 3a20 696e 6465 7820 3d20   None : index = 
-0000c8a0: 696e 6669 6c65 2e73 706c 6974 2827 2e27  infile.split('.'
-0000c8b0: 295b 305d 0a09 7072 696e 7428 6622 3e3e  )[0]..print(f">>
-0000c8c0: 6c6f 6164 2073 7461 7274 6564 3a20 686f  load started: ho
-0000c8d0: 7374 3d7b 686f 7374 7d2c 2069 6e64 6578  st={host}, index
-0000c8e0: 3d7b 696e 6465 787d 2022 202c 2069 6e66  ={index} " , inf
-0000c8f0: 696c 652c 2069 6e64 6578 2c20 666c 7573  ile, index, flus
-0000c900: 683d 5472 7565 2029 0a09 6966 2072 6563  h=True )..if rec
-0000c910: 7265 6174 6520 6f72 206e 6f74 2065 732e  reate or not es.
-0000c920: 696e 6469 6365 732e 6578 6973 7473 2869  indices.exists(i
-0000c930: 6e64 6578 3d69 6e64 6578 293a 200a 0909  ndex=index): ...
-0000c940: 6966 2065 732e 696e 6469 6365 732e 6578  if es.indices.ex
-0000c950: 6973 7473 2869 6e64 6578 3d69 6e64 6578  ists(index=index
-0000c960: 293a 6573 2e69 6e64 6963 6573 2e64 656c  ):es.indices.del
-0000c970: 6574 6528 696e 6465 783d 696e 6465 7829  ete(index=index)
-0000c980: 0a09 0965 732e 696e 6469 6365 732e 6372  ...es.indices.cr
-0000c990: 6561 7465 2869 6e64 6578 3d69 6e64 6578  eate(index=index
-0000c9a0: 2c20 626f 6479 3d73 6f2e 636f 6e66 6967  , body=so.config
-0000c9b0: 2920 0a0a 0961 6374 696f 6e73 3d5b 5d0a  ) ...actions=[].
-0000c9c0: 0964 6566 2061 6464 2873 6f75 7263 6529  .def add(source)
-0000c9d0: 3a20 200a 0909 6163 7469 6f6e 732e 6170  :  ...actions.ap
-0000c9e0: 7065 6e64 2820 7b27 5f6f 705f 7479 7065  pend( {'_op_type
-0000c9f0: 273a 2769 6e64 6578 272c 2027 5f69 6e64  ':'index', '_ind
-0000ca00: 6578 273a 696e 6465 782c 2027 5f69 6427  ex':index, '_id'
-0000ca10: 3a20 736f 7572 6365 5b27 6964 275d 2c20  : source['id'], 
-0000ca20: 275f 736f 7572 6365 273a 2073 6f75 7263  '_source': sourc
-0000ca30: 6520 7d20 290a 0966 6f72 2073 6964 2c20  e } )..for sid, 
-0000ca40: 6c69 6e65 2069 6e20 656e 756d 6572 6174  line in enumerat
-0000ca50: 6528 6669 6c65 696e 7075 742e 696e 7075  e(fileinput.inpu
-0000ca60: 7428 696e 6669 6c65 2c6f 7065 6e68 6f6f  t(infile,openhoo
-0000ca70: 6b3d 6669 6c65 696e 7075 742e 686f 6f6b  k=fileinput.hook
-0000ca80: 5f63 6f6d 7072 6573 7365 6429 293a 200a  _compressed)): .
-0000ca90: 0909 7472 793a 0a09 0909 646f 6320 3d20  ..try:....doc = 
-0000caa0: 446f 6328 7370 6163 792e 6e6c 702e 766f  Doc(spacy.nlp.vo
-0000cab0: 6361 6229 2e66 726f 6d5f 6a73 6f6e 286a  cab).from_json(j
-0000cac0: 736f 6e2e 6c6f 6164 7328 6c69 6e65 2e73  son.loads(line.s
-0000cad0: 7472 6970 2829 2929 2023 2061 6464 2073  trip())) # add s
-0000cae0: 6b65 6e70 200a 0909 0966 6f72 2074 2069  kenp ....for t i
-0000caf0: 6e20 646f 633a 2009 6164 6428 7b22 7479  n doc: .add({"ty
-0000cb00: 7065 223a 2274 6f6b 222c 2022 6964 223a  pe":"tok", "id":
-0000cb10: 2066 227b 7369 647d 2d74 6f6b 2d7b 742e   f"{sid}-tok-{t.
-0000cb20: 697d 222c 2022 7369 6422 3a73 6964 2c20  i}", "sid":sid, 
-0000cb30: 276c 6578 273a 742e 7465 7874 2c20 276c  'lex':t.text, 'l
-0000cb40: 656d 273a 742e 6c65 6d6d 615f 2c20 2770  em':t.lemma_, 'p
-0000cb50: 6f73 273a 742e 706f 735f 2c20 2774 6167  os':t.pos_, 'tag
-0000cb60: 273a 742e 7461 675f 2c20 2764 6570 273a  ':t.tag_, 'dep':
-0000cb70: 742e 6465 705f 2c20 2267 706f 7322 3a74  t.dep_, "gpos":t
-0000cb80: 2e68 6561 642e 706f 735f 2c20 2267 6c65  .head.pos_, "gle
-0000cb90: 6d22 3a74 2e68 6561 642e 6c65 6d6d 615f  m":t.head.lemma_
-0000cba0: 202c 2022 6774 6167 223a 742e 6865 6164   , "gtag":t.head
-0000cbb0: 2e74 6167 5f20 7d29 2023 2769 273a 742e  .tag_ }) #'i':t.
-0000cbc0: 692c 2022 6865 6164 223a 742e 6865 6164  i, "head":t.head
-0000cbd0: 2e69 2c0a 0909 0966 6f72 2073 7020 696e  .i,....for sp in
-0000cbe0: 2064 6f63 2e6e 6f75 6e5f 6368 756e 6b73   doc.noun_chunks
-0000cbf0: 3a20 090a 0909 0909 6966 2073 702e 656e  : ......if sp.en
-0000cc00: 6420 2d20 7370 2e73 7461 7274 203e 2031  d - sp.start > 1
-0000cc10: 3a20 2320 736b 6970 2050 524f 504e 203f  : # skip PROPN ?
-0000cc20: 200a 0909 0909 0961 6464 287b 2274 7970   ......add({"typ
-0000cc30: 6522 3a22 6e70 222c 2022 6964 223a 2066  e":"np", "id": f
-0000cc40: 227b 7369 647d 2d4e 502d 7b73 702e 7374  "{sid}-NP-{sp.st
-0000cc50: 6172 747d 222c 2022 7369 6422 3a73 6964  art}", "sid":sid
-0000cc60: 2c20 2763 6875 6e6b 273a 7370 2e74 6578  , 'chunk':sp.tex
-0000cc70: 742c 2027 6c65 6d27 3a64 6f63 5b73 702e  t, 'lem':doc[sp.
-0000cc80: 656e 642d 315d 2e6c 656d 6d61 5f20 7d29  end-1].lemma_ })
-0000cc90: 0a09 0909 666f 7220 6c65 6d2c 2070 6f73  ....for lem, pos
-0000cca0: 2c20 7479 7065 2c20 6368 756e 6b20 696e  , type, chunk in
-0000ccb0: 206b 705f 6d61 7463 6865 7228 646f 6329   kp_matcher(doc)
-0000ccc0: 3a20 2362 7269 6e6b 3a4e 4f55 4e3a 7070  : #brink:NOUN:pp
-0000ccd0: 3a6f 6e20 7468 6520 6272 696e 6b20 2320  :on the brink # 
-0000cce0: 5b28 2770 7027 2c20 276f 6e20 7468 6520  [('pp', 'on the 
-0000ccf0: 6272 696e 6b27 2c20 322c 2035 292c 2028  brink', 2, 5), (
-0000cd00: 2761 7027 2c20 2776 6572 7920 6861 7070  'ap', 'very happ
-0000cd10: 7927 2c20 392c 2031 3129 5d0a 0909 0909  y', 9, 11)].....
-0000cd20: 6164 6428 7b22 7479 7065 223a 7479 7065  add({"type":type
-0000cd30: 2c20 2269 6422 3a20 6622 7b73 6964 7d2d  , "id": f"{sid}-
-0000cd40: 7b74 7970 657d 2d7b 6368 756e 6b7d 222c  {type}-{chunk}",
-0000cd50: 2022 7369 6422 3a73 6964 2c20 2027 6368   "sid":sid,  'ch
-0000cd60: 756e 6b27 3a63 6875 6e6b 2c20 276c 656d  unk':chunk, 'lem
-0000cd70: 273a 6c65 6d20 2c20 2270 6f73 223a 706f  ':lem , "pos":po
-0000cd80: 737d 2920 2322 7372 6322 3a20 646f 632e  s}) #"src": doc.
-0000cd90: 7465 7874 2c0a 0909 0966 6f72 206e 616d  text,....for nam
-0000cda0: 652c 2061 7220 696e 2064 6570 6d61 7463  e, ar in depmatc
-0000cdb0: 6828 2928 646f 6329 203a 200a 0909 0909  h()(doc) : .....
-0000cdc0: 7479 7065 203d 2073 7061 6379 2e6e 6c70  type = spacy.nlp
-0000cdd0: 2e76 6f63 6162 5b6e 616d 655d 2e74 6578  .vocab[name].tex
-0000cde0: 7420 2320 776f 7272 7920 6265 2074 6872  t # worry be thr
-0000cdf0: 696c 6c65 640a 0909 0909 6c65 6d20 3d20  illed.....lem = 
-0000ce00: 646f 635b 6172 5b30 5d5d 2e6c 656d 6d61  doc[ar[0]].lemma
-0000ce10: 5f0a 0909 0909 6164 6428 7b22 7479 7065  _.....add({"type
-0000ce20: 223a 7479 7065 2c20 2269 6422 3a20 6622  ":type, "id": f"
-0000ce30: 7b73 6964 7d2d 7b74 7970 657d 2d7b 6c65  {sid}-{type}-{le
-0000ce40: 6d7d 222c 2022 7369 6422 3a73 6964 2c20  m}", "sid":sid, 
-0000ce50: 2027 6c65 6d27 3a6c 656d 2c20 2027 7461   'lem':lem,  'ta
-0000ce60: 6727 3a64 6f63 5b61 725b 305d 5d2e 7461  g':doc[ar[0]].ta
-0000ce70: 675f 2c20 276c 656d 3127 3a64 6f63 5b61  g_, 'lem1':doc[a
-0000ce80: 725b 315d 5d2e 6c65 6d6d 615f 2c20 276c  r[1]].lemma_, 'l
-0000ce90: 656d 3227 3a64 6f63 5b61 725b 325d 5d2e  em2':doc[ar[2]].
-0000cea0: 6c65 6d6d 615f 202c 2027 7461 6731 273a  lemma_ , 'tag1':
-0000ceb0: 646f 635b 6172 5b31 5d5d 2e74 6167 5f20  doc[ar[1]].tag_ 
-0000cec0: 2c20 2774 6167 3227 3a64 6f63 5b61 725b  , 'tag2':doc[ar[
-0000ced0: 325d 5d2e 7461 675f 207d 2920 0a09 0909  2]].tag_ }) ....
-0000cee0: 2320 6d65 7267 6564 204e 5020 6d75 7374  # merged NP must
-0000cef0: 2062 6520 6669 6e61 6c6c 7920 6361 6c6c   be finally call
-0000cf00: 6564 200a 0909 0961 6464 2820 7b27 7479  ed ....add( {'ty
-0000cf10: 7065 273a 2773 6e74 272c 2020 2269 6422  pe':'snt',  "id"
-0000cf20: 3a73 6964 2c20 2027 736e 7427 3a64 6f63  :sid,  'snt':doc
-0000cf30: 2e74 6578 742c 2027 706f 7374 6167 273a  .text, 'postag':
-0000cf40: 2065 735f 706f 7374 6167 2864 6f63 292c   es_postag(doc),
-0000cf50: 2027 7463 273a 206c 656e 2864 6f63 292c   'tc': len(doc),
-0000cf60: 2027 736b 656e 7027 3a20 6573 5f73 6b65   'skenp': es_ske
-0000cf70: 6e70 2864 6f63 2920 7d20 2029 2023 2c20  np(doc) }  ) #, 
-0000cf80: 0a09 0909 6966 206c 656e 2861 6374 696f  ....if len(actio
-0000cf90: 6e73 2920 3e3d 2062 6174 6368 3a20 0a09  ns) >= batch: ..
-0000cfa0: 0909 0968 656c 7065 7273 2e62 756c 6b28  ...helpers.bulk(
-0000cfb0: 636c 6965 6e74 3d65 732c 6163 7469 6f6e  client=es,action
-0000cfc0: 733d 6163 7469 6f6e 732c 2072 6169 7365  s=actions, raise
-0000cfd0: 5f6f 6e5f 6572 726f 723d 4661 6c73 6529  _on_error=False)
-0000cfe0: 0a09 0909 0970 7269 6e74 2028 2073 6964  .....print ( sid
-0000cff0: 2c20 6163 7469 6f6e 735b 2d31 5d2c 2066  , actions[-1], f
-0000d000: 6c75 7368 3d54 7275 6529 0a09 0909 0961  lush=True).....a
-0000d010: 6374 696f 6e73 203d 205b 5d0a 0909 0909  ctions = [].....
-0000d020: 2372 6566 7265 7368 2829 2023 2032 3032  #refresh() # 202
-0000d030: 322e 312e 3233 200a 0909 6578 6365 7074  2.1.23 ...except
-0000d040: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-0000d050: 0a09 0909 7072 696e 7428 2265 783a 222c  ....print("ex:",
-0000d060: 2065 2c20 7369 6429 090a 0909 0965 7863   e, sid).....exc
-0000d070: 5f74 7970 652c 2065 7863 5f76 616c 7565  _type, exc_value
-0000d080: 2c20 6578 635f 6f62 6a20 3d20 7379 732e  , exc_obj = sys.
-0000d090: 6578 635f 696e 666f 2829 2009 0a09 0909  exc_info() .....
-0000d0a0: 7472 6163 6562 6163 6b2e 7072 696e 745f  traceback.print_
-0000d0b0: 7462 2865 7863 5f6f 626a 290a 0969 6620  tb(exc_obj)..if 
-0000d0c0: 6163 7469 6f6e 7320 3a20 6865 6c70 6572  actions : helper
-0000d0d0: 732e 6275 6c6b 2863 6c69 656e 743d 6573  s.bulk(client=es
-0000d0e0: 2c61 6374 696f 6e73 3d61 6374 696f 6e73  ,actions=actions
-0000d0f0: 2c20 7261 6973 655f 6f6e 5f65 7272 6f72  , raise_on_error
-0000d100: 3d46 616c 7365 290a 0970 7269 6e74 2822  =False)..print("
-0000d110: 3e3e 6c6f 6164 2066 696e 6973 6865 643a  >>load finished:
-0000d120: 2220 2c20 696e 6669 6c65 2c20 696e 6465  " , infile, inde
-0000d130: 7820 290a 0a23 2076 6e70 3a6d 616b 6520  x )..# vnp:make 
-0000d140: 7573 6520 6f66 0a70 6f73 7461 675f 6675  use of.postag_fu
-0000d150: 6e63 5f6b 7020 3d20 7b20 2023 2064 6f63  nc_kp = {  # doc
-0000d160: 2c73 7461 7274 2c20 656e 642c 2074 6167  ,start, end, tag
-0000d170: 200a 0922 7072 6d6f 6473 223a 206c 616d   .."prmods": lam
-0000d180: 6264 6120 642c 732c 652c 7461 673a 642e  bda d,s,e,tag:d.
-0000d190: 7573 6572 5f64 6174 612e 7570 6461 7465  user_data.update
-0000d1a0: 287b 6622 7b74 6167 7d3a 7b64 5b73 5d2e  ({f"{tag}:{d[s].
-0000d1b0: 6c65 6d6d 615f 7d20 7b64 5b73 2b31 3a65  lemma_} {d[s+1:e
-0000d1c0: 5d2e 7465 7874 2e6c 6f77 6572 2829 7d5b  ].text.lower()}[
-0000d1d0: 7b73 7d2c 7b65 7d29 223a 0a09 097b 226e  {s},{e})":...{"n
-0000d1e0: 6163 223a 205b 645b 652d 315d 2e6c 656d  ac": [d[e-1].lem
-0000d1f0: 6d61 5f20 2b20 6622 3a56 4552 423a 7072  ma_ + f":VERB:pr
-0000d200: 6d6f 6473 7c22 202b 2064 5b73 5d2e 6c65  mods|" + d[s].le
-0000d210: 6d6d 615f 202b 2022 2022 202b 2064 5b73  mma_ + " " + d[s
-0000d220: 2b31 3a65 2d31 5d2e 7465 7874 2e6c 6f77  +1:e-1].text.low
-0000d230: 6572 2829 2c20 645b 652d 315d 2e6c 656d  er(), d[e-1].lem
-0000d240: 6d61 5f20 2b20 6622 3a56 4552 427c 7072  ma_ + f":VERB|pr
-0000d250: 6d6f 6473 225d 2c20 2274 6167 7322 3a20  mods"], "tags": 
-0000d260: 2720 272e 6a6f 696e 285b 742e 7461 675f  ' '.join([t.tag_
-0000d270: 2066 6f72 2074 2069 6e20 645b 733a 655d   for t in d[s:e]
-0000d280: 5d29 207d 7d29 202c 200a 0922 5650 223a  ]) }}) , .."VP":
-0000d290: 206c 616d 6264 6120 642c 732c 652c 7461   lambda d,s,e,ta
-0000d2a0: 673a 2064 2e75 7365 725f 6461 7461 2e75  g: d.user_data.u
-0000d2b0: 7064 6174 6528 7b66 227b 7461 677d 3a7b  pdate({f"{tag}:{
-0000d2c0: 645b 735d 2e6c 656d 6d61 5f7d 207b 645b  d[s].lemma_} {d[
-0000d2d0: 732b 313a 655d 2e74 6578 742e 6c6f 7765  s+1:e].text.lowe
-0000d2e0: 7228 297d 5b7b 737d 2c7b 657d 2922 3a0a  r()}[{s},{e})":.
-0000d2f0: 0909 7b22 6e61 6322 3a20 5b64 5b73 5d2e  ..{"nac": [d[s].
-0000d300: 6c65 6d6d 615f 202b 2066 223a 7b64 5b73  lemma_ + f":{d[s
-0000d310: 5d2e 706f 735f 7d3a 5650 7c22 202b 2064  ].pos_}:VP|" + d
-0000d320: 5b73 5d2e 6c65 6d6d 615f 202b 2022 2022  [s].lemma_ + " "
-0000d330: 202b 2064 5b73 2b31 3a65 5d2e 7465 7874   + d[s+1:e].text
-0000d340: 2e6c 6f77 6572 2829 2c20 645b 735d 2e6c  .lower(), d[s].l
-0000d350: 656d 6d61 5f20 2b20 6622 3a7b 645b 735d  emma_ + f":{d[s]
-0000d360: 2e70 6f73 5f7d 7c56 5022 5d2c 2020 2274  .pos_}|VP"],  "t
-0000d370: 6167 7322 3a20 2720 272e 6a6f 696e 285b  ags": ' '.join([
-0000d380: 742e 7461 675f 2066 6f72 2074 2069 6e20  t.tag_ for t in 
-0000d390: 645b 733a 655d 5d29 7d7d 2920 2c20 0a09  d[s:e]])}}) , ..
-0000d3a0: 2250 5022 3a20 6c61 6d62 6461 2064 2c73  "PP": lambda d,s
-0000d3b0: 2c65 2c74 6167 3a20 642e 7573 6572 5f64  ,e,tag: d.user_d
-0000d3c0: 6174 612e 7570 6461 7465 287b 6622 7b74  ata.update({f"{t
-0000d3d0: 6167 7d3a 7b64 5b73 5d2e 6c65 6d6d 615f  ag}:{d[s].lemma_
-0000d3e0: 7d20 7b64 5b73 2b31 3a65 5d2e 7465 7874  } {d[s+1:e].text
-0000d3f0: 2e6c 6f77 6572 2829 7d5b 7b73 7d2c 7b65  .lower()}[{s},{e
-0000d400: 7d29 223a 0a09 097b 226e 6163 223a 205b  })":...{"nac": [
-0000d410: 645b 652d 315d 2e6c 656d 6d61 5f20 2b20  d[e-1].lemma_ + 
-0000d420: 6622 3a7b 645b 652d 315d 2e70 6f73 5f7d  f":{d[e-1].pos_}
-0000d430: 3a50 507c 2220 2b20 645b 733a 655d 2e74  :PP|" + d[s:e].t
-0000d440: 6578 742e 6c6f 7765 7228 292c 2064 5b65  ext.lower(), d[e
-0000d450: 2d31 5d2e 6c65 6d6d 615f 202b 2066 223a  -1].lemma_ + f":
-0000d460: 7b64 5b65 2d31 5d2e 706f 735f 7d7c 5050  {d[e-1].pos_}|PP
-0000d470: 225d 2c20 2274 6167 7322 3a20 2720 272e  "], "tags": ' '.
-0000d480: 6a6f 696e 285b 742e 7461 675f 2066 6f72  join([t.tag_ for
-0000d490: 2074 2069 6e20 645b 733a 655d 5d29 7d7d   t in d[s:e]])}}
-0000d4a0: 2920 2c0a 0922 4150 223a 206c 616d 6264  ) ,.."AP": lambd
-0000d4b0: 6120 642c 732c 652c 7461 673a 2064 2e75  a d,s,e,tag: d.u
-0000d4c0: 7365 725f 6461 7461 2e75 7064 6174 6528  ser_data.update(
-0000d4d0: 7b66 227b 7461 677d 3a7b 645b 735d 2e6c  {f"{tag}:{d[s].l
-0000d4e0: 656d 6d61 5f7d 207b 645b 732b 313a 655d  emma_} {d[s+1:e]
-0000d4f0: 2e74 6578 742e 6c6f 7765 7228 297d 5b7b  .text.lower()}[{
-0000d500: 737d 2c7b 657d 2922 3a0a 0909 7b22 6e61  s},{e})":...{"na
-0000d510: 6322 3a20 5b64 5b65 2d31 5d2e 6c65 6d6d  c": [d[e-1].lemm
-0000d520: 615f 202b 2066 223a 7b64 5b65 2d31 5d2e  a_ + f":{d[e-1].
-0000d530: 706f 735f 7d3a 4150 7c22 202b 2020 645b  pos_}:AP|" +  d[
-0000d540: 733a 655d 2e74 6578 742c 2064 5b65 2d31  s:e].text, d[e-1
-0000d550: 5d2e 6c65 6d6d 615f 202b 2066 223a 7b64  ].lemma_ + f":{d
-0000d560: 5b65 2d31 5d2e 706f 735f 7d7c 4150 225d  [e-1].pos_}|AP"]
-0000d570: 2c20 2022 7461 6773 223a 2027 2027 2e6a  ,  "tags": ' '.j
-0000d580: 6f69 6e28 5b74 2e74 6167 5f20 666f 7220  oin([t.tag_ for 
-0000d590: 7420 696e 2064 5b73 3a65 5d5d 297d 7d29  t in d[s:e]])}})
-0000d5a0: 202c 0a09 2276 706e 223a 206c 616d 6264   ,.."vpn": lambd
-0000d5b0: 6120 642c 732c 652c 7461 673a 642e 7573  a d,s,e,tag:d.us
-0000d5c0: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
-0000d5d0: 2066 227b 7461 677d 3a7b 645b 735d 2e6c   f"{tag}:{d[s].l
-0000d5e0: 656d 6d61 5f7d 207b 645b 732b 313a 655d  emma_} {d[s+1:e]
-0000d5f0: 2e74 6578 742e 6c6f 7765 7228 297d 5b7b  .text.lower()}[{
-0000d600: 737d 2c7b 657d 2922 3a0a 0909 7b22 6e61  s},{e})":...{"na
-0000d610: 6322 3a20 5b66 227b 645b 735d 2e6c 656d  c": [f"{d[s].lem
-0000d620: 6d61 5f7d 3a56 4552 423a 7670 6e7c 7b64  ma_}:VERB:vpn|{d
-0000d630: 5b73 5d2e 6c65 6d6d 615f 7d20 7b64 5b73  [s].lemma_} {d[s
-0000d640: 2b31 3a65 5d2e 7465 7874 7d22 2c20 6622  +1:e].text}", f"
-0000d650: 7b64 5b73 5d2e 6c65 6d6d 615f 7d3a 5645  {d[s].lemma_}:VE
-0000d660: 5242 7c76 706e 222c 2066 227b 645b 735d  RB|vpn", f"{d[s]
-0000d670: 2e6c 656d 6d61 5f7d 3a56 4552 423a 7670  .lemma_}:VERB:vp
-0000d680: 6e7c 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  n|{d[s].lemma_} 
-0000d690: 7b64 5b73 2b31 5d2e 7465 7874 7d20 5f4e  {d[s+1].text} _N
-0000d6a0: 4f55 4e22 2c0a 0909 0909 6622 7b64 5b65  OUN",.....f"{d[e
-0000d6b0: 2d31 5d2e 6c65 6d6d 615f 7d3a 4e4f 554e  -1].lemma_}:NOUN
-0000d6c0: 3a76 706e 7c7b 645b 735d 2e6c 656d 6d61  :vpn|{d[s].lemma
-0000d6d0: 5f7d 207b 645b 732b 313a 655d 2e74 6578  _} {d[s+1:e].tex
-0000d6e0: 747d 222c 2066 227b 645b 652d 315d 2e6c  t}", f"{d[e-1].l
-0000d6f0: 656d 6d61 5f7d 3a4e 4f55 4e7c 7670 6e22  emma_}:NOUN|vpn"
-0000d700: 2c20 6622 7b64 5b65 2d31 5d2e 6c65 6d6d  , f"{d[e-1].lemm
-0000d710: 615f 7d3a 4e4f 554e 3a76 706e 7c5f 5645  a_}:NOUN:vpn|_VE
-0000d720: 5242 207b 645b 732b 313a 655d 2e74 6578  RB {d[s+1:e].tex
-0000d730: 747d 222c 200a 0909 0909 6622 7b64 5b65  t}", .....f"{d[e
-0000d740: 2d31 5d2e 6c65 6d6d 615f 7d2f 4e4f 554e  -1].lemma_}/NOUN
-0000d750: 7c76 706e 3a5f 7b64 5b73 5d2e 6c65 6d6d  |vpn:_{d[s].lemm
-0000d760: 615f 7d20 7b64 5b73 2b31 3a65 5d2e 7465  a_} {d[s+1:e].te
-0000d770: 7874 7d22 2c20 2023 2066 6f72 6365 2f4e  xt}",  # force/N
-0000d780: 4f55 4e7c 7670 6e3a 636f 6d65 2069 6e74  OUN|vpn:come int
-0000d790: 6f20 666f 7263 650a 0909 0909 5d7d 207d  o force.....]} }
-0000d7a0: 2920 2c20 2320 5f56 4552 4220 7769 7468  ) , # _VERB with
-0000d7b0: 2066 6f72 6365 2c20 6a75 6d70 206f 7665   force, jump ove
-0000d7c0: 7220 7468 6520 646f 673f 200a 0922 6270  r the dog? .."bp
-0000d7d0: 6e22 3a20 6c61 6d62 6461 2064 2c73 2c65  n": lambda d,s,e
-0000d7e0: 2c74 6167 3a64 2e75 7365 725f 6461 7461  ,tag:d.user_data
-0000d7f0: 2e75 7064 6174 6528 7b20 6622 7b74 6167  .update({ f"{tag
-0000d800: 7d3a 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  }:{d[s].lemma_} 
-0000d810: 7b64 5b73 2b31 3a65 5d2e 7465 7874 2e6c  {d[s+1:e].text.l
-0000d820: 6f77 6572 2829 7d5b 7b73 7d2c 7b65 7d29  ower()}[{s},{e})
-0000d830: 223a 0a09 097b 226e 6163 223a 205b 6622  ":...{"nac": [f"
-0000d840: 7b64 5b73 5d2e 6c65 6d6d 615f 7d3a 5645  {d[s].lemma_}:VE
-0000d850: 5242 3a76 706e 7c7b 645b 735d 2e6c 656d  RB:vpn|{d[s].lem
-0000d860: 6d61 5f7d 207b 645b 732b 313a 655d 2e74  ma_} {d[s+1:e].t
-0000d870: 6578 747d 222c 2066 227b 645b 735d 2e6c  ext}", f"{d[s].l
-0000d880: 656d 6d61 5f7d 3a56 4552 427c 7670 6e22  emma_}:VERB|vpn"
-0000d890: 2c20 6622 7b64 5b73 5d2e 6c65 6d6d 615f  , f"{d[s].lemma_
-0000d8a0: 7d3a 5645 5242 3a76 706e 7c7b 645b 735d  }:VERB:vpn|{d[s]
-0000d8b0: 2e6c 656d 6d61 5f7d 207b 645b 732b 315d  .lemma_} {d[s+1]
-0000d8c0: 2e74 6578 747d 205f 4e4f 554e 222c 0a09  .text} _NOUN",..
-0000d8d0: 0909 6622 7b64 5b65 2d31 5d2e 6c65 6d6d  ..f"{d[e-1].lemm
-0000d8e0: 615f 7d3a 4e4f 554e 3a76 706e 7c7b 645b  a_}:NOUN:vpn|{d[
-0000d8f0: 735d 2e6c 656d 6d61 5f7d 207b 645b 732b  s].lemma_} {d[s+
-0000d900: 313a 655d 2e74 6578 747d 222c 2066 227b  1:e].text}", f"{
-0000d910: 645b 652d 315d 2e6c 656d 6d61 5f7d 3a4e  d[e-1].lemma_}:N
-0000d920: 4f55 4e7c 7670 6e22 2c20 6622 7b64 5b65  OUN|vpn", f"{d[e
-0000d930: 2d31 5d2e 6c65 6d6d 615f 7d3a 4e4f 554e  -1].lemma_}:NOUN
-0000d940: 3a76 706e 7c5f 5645 5242 207b 645b 732b  :vpn|_VERB {d[s+
-0000d950: 313a 655d 2e74 6578 747d 222c 0a09 0909  1:e].text}",....
-0000d960: 6622 7b64 5b65 2d31 5d2e 6c65 6d6d 615f  f"{d[e-1].lemma_
-0000d970: 7d2f 4e4f 554e 7c76 706e 3a5f 7b64 5b73  }/NOUN|vpn:_{d[s
-0000d980: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
-0000d990: 3a65 5d2e 7465 7874 7d22 2c20 5d20 7d7d  :e].text}", ] }}
-0000d9a0: 2920 2c20 2320 6265 2077 6974 6820 666f  ) , # be with fo
-0000d9b0: 7263 652c 2062 6520 6973 2061 2056 4552  rce, be is a VER
-0000d9c0: 420a 0922 766e 7022 3a20 6c61 6d62 6461  B.."vnp": lambda
-0000d9d0: 2064 2c73 2c65 2c74 6167 3a64 2e75 7365   d,s,e,tag:d.use
-0000d9e0: 725f 6461 7461 2e75 7064 6174 6528 7b20  r_data.update({ 
-0000d9f0: 6622 7b74 6167 7d3a 7b64 5b73 5d2e 6c65  f"{tag}:{d[s].le
-0000da00: 6d6d 615f 7d20 7b64 5b73 2b31 3a65 5d2e  mma_} {d[s+1:e].
-0000da10: 7465 7874 2e6c 6f77 6572 2829 7d5b 7b73  text.lower()}[{s
-0000da20: 7d2c 7b65 7d29 223a 0a09 097b 226e 6163  },{e})":...{"nac
-0000da30: 223a 205b 6622 7b64 5b73 5d2e 6c65 6d6d  ": [f"{d[s].lemm
-0000da40: 615f 7d3a 5645 5242 3a76 6e70 7c7b 645b  a_}:VERB:vnp|{d[
-0000da50: 735d 2e6c 656d 6d61 5f7d 207b 645b 732b  s].lemma_} {d[s+
-0000da60: 313a 655d 2e74 6578 747d 222c 2066 227b  1:e].text}", f"{
-0000da70: 645b 735d 2e6c 656d 6d61 5f7d 3a56 4552  d[s].lemma_}:VER
-0000da80: 427c 766e 7022 2c20 6622 7b64 5b73 5d2e  B|vnp", f"{d[s].
-0000da90: 6c65 6d6d 615f 7d3a 5645 5242 3a76 6e70  lemma_}:VERB:vnp
-0000daa0: 7c7b 645b 735d 2e6c 656d 6d61 5f7d 205f  |{d[s].lemma_} _
-0000dab0: 4e4f 554e 207b 645b 732b 325d 2e74 6578  NOUN {d[s+2].tex
-0000dac0: 747d 222c 0a09 0909 0966 227b 645b 732b  t}",.....f"{d[s+
-0000dad0: 315d 2e6c 656d 6d61 5f7d 3a4e 4f55 4e3a  1].lemma_}:NOUN:
-0000dae0: 766e 707c 7b64 5b73 5d2e 6c65 6d6d 615f  vnp|{d[s].lemma_
-0000daf0: 7d20 7b64 5b73 2b31 3a65 5d2e 7465 7874  } {d[s+1:e].text
-0000db00: 7d22 2c20 6622 7b64 5b73 2b31 5d2e 6c65  }", f"{d[s+1].le
-0000db10: 6d6d 615f 7d3a 4e4f 554e 7c76 6e70 222c  mma_}:NOUN|vnp",
-0000db20: 2066 227b 645b 732b 315d 2e6c 656d 6d61   f"{d[s+1].lemma
-0000db30: 5f7d 3a4e 4f55 4e3a 766e 707c 5f56 4552  _}:NOUN:vnp|_VER
-0000db40: 4220 7b64 5b73 2b31 3a65 5d2e 7465 7874  B {d[s+1:e].text
-0000db50: 7d22 2c0a 0909 0909 6622 7b64 5b73 5d2e  }",.....f"{d[s].
-0000db60: 6c65 6d6d 615f 7d2f 5645 5242 7c76 6e70  lemma_}/VERB|vnp
-0000db70: 3a5f 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  :_{d[s].lemma_} 
-0000db80: 7b64 5b73 2b31 3a65 5d2e 7465 7874 7d22  {d[s+1:e].text}"
-0000db90: 2c5d 7d7d 2920 2c0a 0922 7670 223a 2020  ,]}}) ,.."vp":  
-0000dba0: 6c61 6d62 6461 2064 2c73 2c65 2c74 6167  lambda d,s,e,tag
-0000dbb0: 3a64 2e75 7365 725f 6461 7461 2e75 7064  :d.user_data.upd
-0000dbc0: 6174 6528 7b20 6622 7b74 6167 7d3a 7b64  ate({ f"{tag}:{d
-0000dbd0: 5b73 5d2e 6c65 6d6d 615f 7d20 7b64 5b73  [s].lemma_} {d[s
-0000dbe0: 2b31 3a65 5d2e 7465 7874 2e6c 6f77 6572  +1:e].text.lower
-0000dbf0: 2829 7d5b 7b73 7d2c 7b65 7d29 223a 0a09  ()}[{s},{e})":..
-0000dc00: 097b 226e 6163 223a 205b 6622 7b64 5b73  .{"nac": [f"{d[s
-0000dc10: 5d2e 6c65 6d6d 615f 7d3a 5645 5242 3a76  ].lemma_}:VERB:v
-0000dc20: 707c 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  p|{d[s].lemma_} 
-0000dc30: 7b64 5b73 2b31 5d2e 7465 7874 7d22 2c20  {d[s+1].text}", 
-0000dc40: 6622 7b64 5b73 5d2e 6c65 6d6d 615f 7d3a  f"{d[s].lemma_}:
-0000dc50: 5645 5242 7c76 7022 2c20 6622 7b64 5b73  VERB|vp", f"{d[s
-0000dc60: 2b31 5d2e 6c65 6d6d 615f 7d3a 7b64 5b73  +1].lemma_}:{d[s
-0000dc70: 2b31 5d2e 706f 735f 7d3a 7670 7c5f 5645  +1].pos_}:vp|_VE
-0000dc80: 5242 207b 645b 732b 315d 2e74 6578 747d  RB {d[s+1].text}
-0000dc90: 222c 0a09 0909 0920 6622 7b64 5b73 5d2e  ",..... f"{d[s].
-0000dca0: 6c65 6d6d 615f 7d2f 5645 5242 7c76 703a  lemma_}/VERB|vp:
-0000dcb0: 5f7b 645b 735d 2e6c 656d 6d61 5f7d 207b  _{d[s].lemma_} {
-0000dcc0: 645b 732b 315d 2e74 6578 742e 6c6f 7765  d[s+1].text.lowe
-0000dcd0: 7228 297d 222c 095d 207d 7d29 202c 0a09  r()}",.] }}) ,..
-0000dce0: 2276 7070 223a 206c 616d 6264 6120 642c  "vpp": lambda d,
-0000dcf0: 732c 652c 7461 673a 642e 7573 6572 5f64  s,e,tag:d.user_d
-0000dd00: 6174 612e 7570 6461 7465 287b 2066 227b  ata.update({ f"{
-0000dd10: 7461 677d 3a7b 645b 735d 2e6c 656d 6d61  tag}:{d[s].lemma
-0000dd20: 5f7d 207b 645b 732b 313a 655d 2e74 6578  _} {d[s+1:e].tex
-0000dd30: 742e 6c6f 7765 7228 297d 5b7b 737d 2c7b  t.lower()}[{s},{
-0000dd40: 657d 2922 3a0a 0909 7b22 6e61 6322 3a20  e})":...{"nac": 
-0000dd50: 5b66 227b 645b 735d 2e6c 656d 6d61 5f7d  [f"{d[s].lemma_}
-0000dd60: 3a56 4552 423a 7670 707c 7b64 5b73 5d2e  :VERB:vpp|{d[s].
-0000dd70: 6c65 6d6d 615f 7d20 7b64 5b73 2b31 3a65  lemma_} {d[s+1:e
-0000dd80: 5d2e 7465 7874 7d22 2c20 6622 7b64 5b73  ].text}", f"{d[s
-0000dd90: 5d2e 6c65 6d6d 615f 7d3a 5645 5242 7c76  ].lemma_}:VERB|v
-0000dda0: 7070 220a 0909 0909 2066 227b 645b 735d  pp"..... f"{d[s]
-0000ddb0: 2e6c 656d 6d61 5f7d 2f56 4552 427c 7670  .lemma_}/VERB|vp
-0000ddc0: 703a 5f7b 645b 735d 2e6c 656d 6d61 5f7d  p:_{d[s].lemma_}
-0000ddd0: 207b 645b 732b 313a 655d 2e74 6578 747d   {d[s+1:e].text}
-0000dde0: 222c 205d 207d 7d29 202c 0a09 2276 7067  ", ] }}) ,.."vpg
-0000ddf0: 223a 206c 616d 6264 6120 642c 732c 652c  ": lambda d,s,e,
-0000de00: 7461 673a 642e 7573 6572 5f64 6174 612e  tag:d.user_data.
-0000de10: 7570 6461 7465 287b 2066 227b 7461 677d  update({ f"{tag}
-0000de20: 3a7b 645b 735d 2e6c 656d 6d61 5f7d 207b  :{d[s].lemma_} {
-0000de30: 645b 732b 313a 655d 2e74 6578 742e 6c6f  d[s+1:e].text.lo
-0000de40: 7765 7228 297d 5b7b 737d 2c7b 657d 2922  wer()}[{s},{e})"
-0000de50: 3a0a 0909 7b22 6e61 6322 3a20 5b66 227b  :...{"nac": [f"{
-0000de60: 645b 735d 2e6c 656d 6d61 5f7d 3a56 4552  d[s].lemma_}:VER
-0000de70: 423a 7670 677c 7b64 5b73 5d2e 6c65 6d6d  B:vpg|{d[s].lemm
-0000de80: 615f 7d20 7b64 5b73 2b31 5d2e 7465 7874  a_} {d[s+1].text
-0000de90: 7d22 2c20 6622 7b64 5b73 5d2e 6c65 6d6d  }", f"{d[s].lemm
-0000dea0: 615f 7d3a 5645 5242 7c76 7067 222c 2066  a_}:VERB|vpg", f
-0000deb0: 227b 645b 735d 2e6c 656d 6d61 5f7d 3a56  "{d[s].lemma_}:V
-0000dec0: 4552 423a 7670 677c 5f7b 645b 735d 2e6c  ERB:vpg|_{d[s].l
-0000ded0: 656d 6d61 5f7d 207b 645b 732b 315d 2e74  emma_} {d[s+1].t
-0000dee0: 6578 747d 205f 5642 4722 2c20 0a09 0909  ext} _VBG", ....
-0000def0: 6622 7b64 5b73 5d2e 6c65 6d6d 615f 7d2f  f"{d[s].lemma_}/
-0000df00: 5645 5242 7c76 7067 3a5f 7b64 5b73 5d2e  VERB|vpg:_{d[s].
-0000df10: 6c65 6d6d 615f 7d20 7b64 5b73 2b31 5d2e  lemma_} {d[s+1].
-0000df20: 7465 7874 7d20 5f56 4247 225d 207d 7d29  text} _VBG"] }})
-0000df30: 202c 0a09 2270 6e22 3a20 206c 616d 6264   ,.."pn":  lambd
-0000df40: 6120 642c 732c 652c 7461 673a 642e 7573  a d,s,e,tag:d.us
-0000df50: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
-0000df60: 2066 227b 7461 677d 3a7b 645b 735d 2e6c   f"{tag}:{d[s].l
-0000df70: 656d 6d61 5f7d 207b 645b 732b 313a 655d  emma_} {d[s+1:e]
-0000df80: 2e74 6578 742e 6c6f 7765 7228 297d 5b7b  .text.lower()}[{
-0000df90: 737d 2c7b 657d 2922 3a0a 0909 7b22 6e61  s},{e})":...{"na
-0000dfa0: 6322 3a20 5b66 227b 645b 732b 315d 2e6c  c": [f"{d[s+1].l
-0000dfb0: 656d 6d61 5f7d 3a4e 4f55 4e3a 706e 7c7b  emma_}:NOUN:pn|{
-0000dfc0: 645b 733a 655d 2e74 6578 742e 6c6f 7765  d[s:e].text.lowe
-0000dfd0: 7228 297d 222c 2066 227b 645b 732b 315d  r()}", f"{d[s+1]
-0000dfe0: 2e6c 656d 6d61 5f7d 3a4e 4f55 4e7c 706e  .lemma_}:NOUN|pn
-0000dff0: 222c 0a09 0909 6622 7b64 5b73 2b31 5d2e  ",....f"{d[s+1].
-0000e000: 6c65 6d6d 615f 7d2f 4e4f 554e 7c70 6e3a  lemma_}/NOUN|pn:
-0000e010: 7b64 5b73 3a65 5d2e 7465 7874 2e6c 6f77  {d[s:e].text.low
-0000e020: 6572 2829 7d22 2c20 5d20 7d7d 2920 2c0a  er()}", ] }}) ,.
-0000e030: 0922 706e 7022 3a20 6c61 6d62 6461 2064  ."pnp": lambda d
-0000e040: 2c73 2c65 2c74 6167 3a64 2e75 7365 725f  ,s,e,tag:d.user_
-0000e050: 6461 7461 2e75 7064 6174 6528 7b20 6622  data.update({ f"
-0000e060: 7b74 6167 7d3a 7b64 5b73 5d2e 6c65 6d6d  {tag}:{d[s].lemm
-0000e070: 615f 7d20 7b64 5b73 2b31 3a65 5d2e 7465  a_} {d[s+1:e].te
-0000e080: 7874 2e6c 6f77 6572 2829 7d5b 7b73 7d2c  xt.lower()}[{s},
-0000e090: 7b65 7d29 223a 0a09 097b 226e 6163 223a  {e})":...{"nac":
-0000e0a0: 205b 6622 7b64 5b73 2b31 5d2e 6c65 6d6d   [f"{d[s+1].lemm
-0000e0b0: 615f 7d3a 4e4f 554e 3a70 6e70 7c7b 645b  a_}:NOUN:pnp|{d[
-0000e0c0: 733a 655d 2e74 6578 742e 6c6f 7765 7228  s:e].text.lower(
-0000e0d0: 297d 222c 2066 227b 645b 732b 315d 2e6c  )}", f"{d[s+1].l
-0000e0e0: 656d 6d61 5f7d 3a4e 4f55 4e3a 706e 7022  emma_}:NOUN:pnp"
-0000e0f0: 2c0a 0909 0966 227b 645b 732b 315d 2e6c  ,....f"{d[s+1].l
-0000e100: 656d 6d61 5f7d 2f4e 4f55 4e7c 706e 703a  emma_}/NOUN|pnp:
-0000e110: 7b64 5b73 3a65 5d2e 7465 7874 2e6c 6f77  {d[s:e].text.low
-0000e120: 6572 2829 7d22 2c5d 207d 7d29 202c 0a09  er()}",] }}) ,..
-0000e130: 2262 6170 7622 3a20 6c61 6d62 6461 2064  "bapv": lambda d
-0000e140: 2c73 2c65 2c74 6167 3a64 2e75 7365 725f  ,s,e,tag:d.user_
-0000e150: 6461 7461 2e75 7064 6174 6528 7b20 6622  data.update({ f"
-0000e160: 7b74 6167 7d3a 7b64 5b73 5d2e 6c65 6d6d  {tag}:{d[s].lemm
-0000e170: 615f 7d20 7b64 5b73 2b31 3a65 5d2e 7465  a_} {d[s+1:e].te
-0000e180: 7874 2e6c 6f77 6572 2829 7d5b 7b73 7d2c  xt.lower()}[{s},
-0000e190: 7b65 7d29 223a 0a09 097b 226e 6163 223a  {e})":...{"nac":
-0000e1a0: 205b 6622 7b64 5b73 2b31 5d2e 6c65 6d6d   [f"{d[s+1].lemm
-0000e1b0: 615f 7d3a 4144 4a3a 6261 7076 7c7b 645b  a_}:ADJ:bapv|{d[
-0000e1c0: 735d 2e6c 656d 6d61 5f7d 207b 645b 732b  s].lemma_} {d[s+
-0000e1d0: 313a 655d 2e74 6578 747d 222c 2066 227b  1:e].text}", f"{
-0000e1e0: 645b 732b 315d 2e6c 656d 6d61 5f7d 3a41  d[s+1].lemma_}:A
-0000e1f0: 444a 7c62 6170 7622 2c20 6622 7b64 5b73  DJ|bapv", f"{d[s
-0000e200: 2b31 5d2e 6c65 6d6d 615f 7d3a 4144 4a3a  +1].lemma_}:ADJ:
-0000e210: 6261 7076 7c5f 7b64 5b73 5d2e 6c65 6d6d  bapv|_{d[s].lemm
-0000e220: 615f 7d20 7b64 5b73 2b31 3a65 2d31 5d2e  a_} {d[s+1:e-1].
-0000e230: 7465 7874 7d20 5f56 4552 4222 5d7d 7d29  text} _VERB"]}})
-0000e240: 202c 2020 0a09 2262 6174 7622 3a20 6c61   ,  .."batv": la
-0000e250: 6d62 6461 2064 2c73 2c65 2c74 6167 3a64  mbda d,s,e,tag:d
-0000e260: 2e75 7365 725f 6461 7461 2e75 7064 6174  .user_data.updat
-0000e270: 6528 7b20 6622 7b74 6167 7d3a 7b64 5b73  e({ f"{tag}:{d[s
-0000e280: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
-0000e290: 3a65 5d2e 7465 7874 2e6c 6f77 6572 2829  :e].text.lower()
-0000e2a0: 7d5b 7b73 7d2c 7b65 7d29 223a 0a09 097b  }[{s},{e})":...{
-0000e2b0: 226e 6163 223a 205b 6622 7b64 5b73 2b31  "nac": [f"{d[s+1
-0000e2c0: 5d2e 6c65 6d6d 615f 7d3a 4144 4a3a 6261  ].lemma_}:ADJ:ba
-0000e2d0: 7476 7c7b 645b 735d 2e6c 656d 6d61 5f7d  tv|{d[s].lemma_}
-0000e2e0: 207b 645b 732b 313a 655d 2e74 6578 747d   {d[s+1:e].text}
-0000e2f0: 222c 2066 227b 645b 732b 315d 2e6c 656d  ", f"{d[s+1].lem
-0000e300: 6d61 5f7d 3a41 444a 7c62 6174 7622 2c20  ma_}:ADJ|batv", 
-0000e310: 6622 7b64 5b73 2b31 5d2e 6c65 6d6d 615f  f"{d[s+1].lemma_
-0000e320: 7d3a 4144 4a3a 6261 7476 7c5f 7b64 5b73  }:ADJ:batv|_{d[s
-0000e330: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
-0000e340: 3a65 2d31 5d2e 7465 7874 7d20 5f56 4552  :e-1].text} _VER
-0000e350: 4222 5d7d 7d29 202c 2020 0a09 2262 6570  B"]}}) ,  .."bep
-0000e360: 7622 3a20 6c61 6d62 6461 2064 2c73 2c65  v": lambda d,s,e
-0000e370: 2c74 6167 3a64 2e75 7365 725f 6461 7461  ,tag:d.user_data
-0000e380: 2e75 7064 6174 6528 7b20 6622 7b74 6167  .update({ f"{tag
-0000e390: 7d3a 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  }:{d[s].lemma_} 
-0000e3a0: 7b64 5b73 2b31 3a65 5d2e 7465 7874 2e6c  {d[s+1:e].text.l
-0000e3b0: 6f77 6572 2829 7d5b 7b73 7d2c 7b65 7d29  ower()}[{s},{e})
-0000e3c0: 223a 0a09 097b 226e 6163 223a 205b 6622  ":...{"nac": [f"
-0000e3d0: 7b64 5b73 2b31 5d2e 6c65 6d6d 615f 7d3a  {d[s+1].lemma_}:
-0000e3e0: 5645 5242 3a62 6570 767c 7b64 5b73 5d2e  VERB:bepv|{d[s].
-0000e3f0: 6c65 6d6d 615f 7d20 7b64 5b73 2b31 3a65  lemma_} {d[s+1:e
-0000e400: 5d2e 7465 7874 7d22 2c66 227b 645b 732b  ].text}",f"{d[s+
-0000e410: 315d 2e6c 656d 6d61 5f7d 3a56 4552 427c  1].lemma_}:VERB|
-0000e420: 6265 7076 222c 2066 227b 645b 732b 315d  bepv", f"{d[s+1]
-0000e430: 2e6c 656d 6d61 5f7d 3a56 4552 423a 6265  .lemma_}:VERB:be
-0000e440: 7076 7c5f 6265 207b 645b 732b 313a 652d  pv|_be {d[s+1:e-
-0000e450: 315d 2e74 6578 747d 205f 5645 5242 222c  1].text} _VERB",
-0000e460: 0a09 0909 6622 7b64 5b73 2b31 5d2e 6c65  ....f"{d[s+1].le
-0000e470: 6d6d 615f 7d2f 5645 5242 7c62 6570 763a  mma_}/VERB|bepv:
-0000e480: 5f7b 645b 735d 2e6c 656d 6d61 5f7d 207b  _{d[s].lemma_} {
-0000e490: 645b 732b 313a 652d 315d 2e74 6578 747d  d[s+1:e-1].text}
-0000e4a0: 205f 7b64 5b65 2d31 5d2e 7461 675f 7d22   _{d[e-1].tag_}"
-0000e4b0: 2c5d 7d7d 2920 2c20 2320 5f62 6520 666f  ,]}}) , # _be fo
-0000e4c0: 7263 6564 2074 6f20 5f56 4552 420a 0922  rced to _VERB.."
-0000e4d0: 6265 7476 223a 206c 616d 6264 6120 642c  betv": lambda d,
-0000e4e0: 732c 652c 7461 673a 642e 7573 6572 5f64  s,e,tag:d.user_d
-0000e4f0: 6174 612e 7570 6461 7465 287b 2066 227b  ata.update({ f"{
-0000e500: 7461 677d 3a7b 645b 735d 2e6c 656d 6d61  tag}:{d[s].lemma
-0000e510: 5f7d 207b 645b 732b 313a 655d 2e74 6578  _} {d[s+1:e].tex
-0000e520: 742e 6c6f 7765 7228 297d 5b7b 737d 2c7b  t.lower()}[{s},{
-0000e530: 657d 2922 3a0a 0909 7b22 6e61 6322 3a20  e})":...{"nac": 
-0000e540: 5b66 227b 645b 732b 315d 2e6c 656d 6d61  [f"{d[s+1].lemma
-0000e550: 5f7d 3a56 4552 423a 6265 7476 7c7b 645b  _}:VERB:betv|{d[
-0000e560: 735d 2e6c 656d 6d61 5f7d 207b 645b 732b  s].lemma_} {d[s+
-0000e570: 313a 655d 2e74 6578 747d 222c 6622 7b64  1:e].text}",f"{d
-0000e580: 5b73 2b31 5d2e 6c65 6d6d 615f 7d3a 5645  [s+1].lemma_}:VE
-0000e590: 5242 7c62 6574 7622 2c20 6622 7b64 5b73  RB|betv", f"{d[s
-0000e5a0: 2b31 5d2e 6c65 6d6d 615f 7d3a 5645 5242  +1].lemma_}:VERB
-0000e5b0: 3a62 6574 767c 5f62 6520 7b64 5b73 2b31  :betv|_be {d[s+1
-0000e5c0: 3a65 2d31 5d2e 7465 7874 7d20 5f56 4552  :e-1].text} _VER
-0000e5d0: 4222 2c0a 0909 2020 2020 2066 227b 645b  B",...     f"{d[
-0000e5e0: 732b 315d 2e6c 656d 6d61 5f7d 2f56 4552  s+1].lemma_}/VER
-0000e5f0: 427c 6265 7476 3a5f 7b64 5b73 5d2e 6c65  B|betv:_{d[s].le
-0000e600: 6d6d 615f 7d20 7b64 5b73 2b31 3a65 2d31  mma_} {d[s+1:e-1
-0000e610: 5d2e 7465 7874 7d20 5f7b 645b 652d 315d  ].text} _{d[e-1]
-0000e620: 2e74 6167 5f7d 222c 5d7d 7d29 202c 2023  .tag_}",]}}) , #
-0000e630: 205f 6265 2066 6f72 6365 6420 746f 205f   _be forced to _
-0000e640: 5645 5242 0a09 2262 6170 223a 206c 616d  VERB.."bap": lam
-0000e650: 6264 6120 642c 732c 652c 7461 673a 642e  bda d,s,e,tag:d.
-0000e660: 7573 6572 5f64 6174 612e 7570 6461 7465  user_data.update
-0000e670: 287b 2066 227b 7461 677d 3a7b 645b 735d  ({ f"{tag}:{d[s]
-0000e680: 2e6c 656d 6d61 5f7d 207b 645b 732b 313a  .lemma_} {d[s+1:
-0000e690: 655d 2e74 6578 742e 6c6f 7765 7228 297d  e].text.lower()}
-0000e6a0: 5b7b 737d 2c7b 657d 2922 3a0a 0909 7b22  [{s},{e})":...{"
-0000e6b0: 6e61 6322 3a20 5b66 227b 645b 732b 315d  nac": [f"{d[s+1]
-0000e6c0: 2e6c 656d 6d61 5f7d 3a41 444a 3a62 6170  .lemma_}:ADJ:bap
-0000e6d0: 7c7b 645b 735d 2e6c 656d 6d61 5f7d 207b  |{d[s].lemma_} {
-0000e6e0: 645b 732b 313a 655d 2e74 6578 747d 222c  d[s+1:e].text}",
-0000e6f0: 2066 227b 645b 732b 315d 2e6c 656d 6d61   f"{d[s+1].lemma
-0000e700: 5f7d 3a41 444a 7c62 6170 222c 0a09 0909  _}:ADJ|bap",....
-0000e710: 0966 227b 645b 732b 315d 2e6c 656d 6d61  .f"{d[s+1].lemma
-0000e720: 5f7d 2f41 444a 7c62 6170 3a5f 7b64 5b73  _}/ADJ|bap:_{d[s
-0000e730: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
-0000e740: 3a65 5d2e 7465 7874 7d22 2c5d 7d7d 2920  :e].text}",]}}) 
-0000e750: 2c0a 0922 6265 7022 3a20 6c61 6d62 6461  ,.."bep": lambda
-0000e760: 2064 2c73 2c65 2c74 6167 3a64 2e75 7365   d,s,e,tag:d.use
-0000e770: 725f 6461 7461 2e75 7064 6174 6528 7b20  r_data.update({ 
-0000e780: 6622 7b74 6167 7d3a 7b64 5b73 5d2e 6c65  f"{tag}:{d[s].le
-0000e790: 6d6d 615f 7d20 7b64 5b73 2b31 3a65 5d2e  mma_} {d[s+1:e].
-0000e7a0: 7465 7874 2e6c 6f77 6572 2829 7d5b 7b73  text.lower()}[{s
-0000e7b0: 7d2c 7b65 7d29 223a 0a09 097b 226e 6163  },{e})":...{"nac
-0000e7c0: 223a 205b 6622 7b64 5b73 2b31 5d2e 6c65  ": [f"{d[s+1].le
-0000e7d0: 6d6d 615f 7d3a 5645 5242 3a62 6570 7c7b  mma_}:VERB:bep|{
-0000e7e0: 645b 735d 2e6c 656d 6d61 5f7d 207b 645b  d[s].lemma_} {d[
-0000e7f0: 732b 313a 655d 2e74 6578 747d 222c 2066  s+1:e].text}", f
-0000e800: 227b 645b 732b 315d 2e6c 656d 6d61 5f7d  "{d[s+1].lemma_}
-0000e810: 3a56 4552 427c 6265 7022 2c0a 0909 0909  :VERB|bep",.....
-0000e820: 6622 7b64 5b73 2b31 5d2e 6c65 6d6d 615f  f"{d[s+1].lemma_
-0000e830: 7d2f 5645 5242 7c62 6570 3a5f 7b64 5b73  }/VERB|bep:_{d[s
-0000e840: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
-0000e850: 3a65 5d2e 7465 7874 7d22 2c5d 7d7d 2920  :e].text}",]}}) 
-0000e860: 2c0a 0922 766f 7022 3a20 6c61 6d62 6461  ,.."vop": lambda
-0000e870: 2064 2c73 2c65 2c74 6167 3a64 2e75 7365   d,s,e,tag:d.use
-0000e880: 725f 6461 7461 2e75 7064 6174 6528 7b20  r_data.update({ 
-0000e890: 6622 7b74 6167 7d3a 7b64 5b73 5d2e 6c65  f"{tag}:{d[s].le
-0000e8a0: 6d6d 615f 7d20 7b64 5b73 2b31 3a65 5d2e  mma_} {d[s+1:e].
-0000e8b0: 7465 7874 2e6c 6f77 6572 2829 7d5b 7b73  text.lower()}[{s
-0000e8c0: 7d2c 7b65 7d29 223a 0a09 097b 226e 6163  },{e})":...{"nac
-0000e8d0: 223a 205b 6622 7b64 5b73 5d2e 6c65 6d6d  ": [f"{d[s].lemm
-0000e8e0: 615f 7d3a 5645 5242 3a76 6f70 7c7b 645b  a_}:VERB:vop|{d[
-0000e8f0: 735d 2e6c 656d 6d61 5f7d 206f 6e65 7365  s].lemma_} onese
-0000e900: 6c66 207b 645b 652d 315d 2e74 6578 747d  lf {d[e-1].text}
-0000e910: 222c 2066 227b 645b 735d 2e6c 656d 6d61  ", f"{d[s].lemma
-0000e920: 5f7d 3a56 4552 427c 766f 7022 2c20 2066  _}:VERB|vop",  f
-0000e930: 227b 645b 735d 2e6c 656d 6d61 5f7d 3a56  "{d[s].lemma_}:V
-0000e940: 4552 423a 766f 707c 5f7b 645b 735d 2e6c  ERB:vop|_{d[s].l
-0000e950: 656d 6d61 5f7d 205f 6f6e 6573 656c 6620  emma_} _oneself 
-0000e960: 7b64 5b65 2d31 5d2e 7465 7874 7d22 2c0a  {d[e-1].text}",.
-0000e970: 0909 0966 227b 645b 735d 2e6c 656d 6d61  ...f"{d[s].lemma
-0000e980: 5f7d 2f56 4552 427c 766f 703a 5f7b 645b  _}/VERB|vop:_{d[
-0000e990: 735d 2e6c 656d 6d61 5f7d 205f 6f6e 6573  s].lemma_} _ones
-0000e9a0: 656c 6620 7b64 5b65 2d31 5d2e 7465 7874  elf {d[e-1].text
-0000e9b0: 2e6c 6f77 6572 2829 7d22 2c5d 7d7d 2920  .lower()}",]}}) 
-0000e9c0: 2c0a 0922 7674 7622 3a20 6c61 6d62 6461  ,.."vtv": lambda
-0000e9d0: 2064 2c73 2c65 2c74 6167 3a64 2e75 7365   d,s,e,tag:d.use
-0000e9e0: 725f 6461 7461 2e75 7064 6174 6528 7b20  r_data.update({ 
-0000e9f0: 6622 7b74 6167 7d3a 7b64 5b73 5d2e 6c65  f"{tag}:{d[s].le
-0000ea00: 6d6d 615f 7d20 7b64 5b73 2b31 3a65 5d2e  mma_} {d[s+1:e].
-0000ea10: 7465 7874 2e6c 6f77 6572 2829 7d5b 7b73  text.lower()}[{s
-0000ea20: 7d2c 7b65 7d29 223a 0a09 097b 226e 6163  },{e})":...{"nac
-0000ea30: 223a 205b 6622 7b64 5b73 5d2e 6c65 6d6d  ": [f"{d[s].lemm
-0000ea40: 615f 7d3a 5645 5242 3a76 7476 7c7b 645b  a_}:VERB:vtv|{d[
-0000ea50: 735d 2e6c 656d 6d61 5f7d 207b 645b 732b  s].lemma_} {d[s+
-0000ea60: 313a 655d 2e74 6578 747d 222c 2066 227b  1:e].text}", f"{
-0000ea70: 645b 735d 2e6c 656d 6d61 5f7d 3a56 4552  d[s].lemma_}:VER
-0000ea80: 423a 7674 767c 5f7b 645b 735d 2e6c 656d  B:vtv|_{d[s].lem
-0000ea90: 6d61 5f7d 207b 645b 732b 313a 652d 315d  ma_} {d[s+1:e-1]
-0000eaa0: 2e74 6578 747d 205f 5645 5242 222c 2066  .text} _VERB", f
-0000eab0: 227b 645b 735d 2e6c 656d 6d61 5f7d 3a56  "{d[s].lemma_}:V
-0000eac0: 4552 427c 7674 7622 2c20 6622 7b64 5b65  ERB|vtv", f"{d[e
-0000ead0: 2d31 5d2e 6c65 6d6d 615f 7d3a 5645 5242  -1].lemma_}:VERB
-0000eae0: 7c7e 7674 7622 2c20 6622 7b64 5b65 2d31  |~vtv", f"{d[e-1
-0000eaf0: 5d2e 6c65 6d6d 615f 7d3a 5645 5242 3a7e  ].lemma_}:VERB:~
-0000eb00: 7674 767c 7b64 5b73 5d2e 6c65 6d6d 615f  vtv|{d[s].lemma_
-0000eb10: 7d22 2c0a 0909 0966 227b 645b 735d 2e6c  }",....f"{d[s].l
-0000eb20: 656d 6d61 5f7d 2f56 4552 427c 7674 763a  emma_}/VERB|vtv:
-0000eb30: 5f7b 645b 735d 2e6c 656d 6d61 5f7d 2074  _{d[s].lemma_} t
-0000eb40: 6f20 5f7b 645b 652d 315d 2e74 6167 5f7d  o _{d[e-1].tag_}
-0000eb50: 222c 5d7d 7d20 2920 2c0a 0922 7667 223a  ",]}} ) ,.."vg":
-0000eb60: 206c 616d 6264 6120 642c 732c 652c 7461   lambda d,s,e,ta
-0000eb70: 673a 2064 2e75 7365 725f 6461 7461 2e75  g: d.user_data.u
-0000eb80: 7064 6174 6528 7b20 6622 7b74 6167 7d3a  pdate({ f"{tag}:
-0000eb90: 7b64 5b73 5d2e 6c65 6d6d 615f 7d20 7b64  {d[s].lemma_} {d
-0000eba0: 5b73 2b31 3a65 5d2e 7465 7874 2e6c 6f77  [s+1:e].text.low
-0000ebb0: 6572 2829 7d5b 7b73 7d2c 7b65 7d29 223a  er()}[{s},{e})":
-0000ebc0: 0a09 097b 226e 6163 223a 205b 6622 7b64  ...{"nac": [f"{d
-0000ebd0: 5b73 5d2e 6c65 6d6d 615f 7d3a 5645 5242  [s].lemma_}:VERB
-0000ebe0: 3a76 677c 7b64 5b73 5d2e 6c65 6d6d 615f  :vg|{d[s].lemma_
-0000ebf0: 7d20 7b64 5b65 2d31 5d2e 7465 7874 7d22  } {d[e-1].text}"
-0000ec00: 2c20 6622 7b64 5b73 5d2e 6c65 6d6d 615f  , f"{d[s].lemma_
-0000ec10: 7d3a 5645 5242 3a76 677c 5f7b 645b 735d  }:VERB:vg|_{d[s]
-0000ec20: 2e6c 656d 6d61 5f7d 205f 5642 4722 2c20  .lemma_} _VBG", 
-0000ec30: 6622 7b64 5b73 5d2e 6c65 6d6d 615f 7d3a  f"{d[s].lemma_}:
-0000ec40: 5645 5242 7c76 6722 2c20 6622 7b64 5b65  VERB|vg", f"{d[e
-0000ec50: 2d31 5d2e 6c65 6d6d 615f 7d3a 5645 5242  -1].lemma_}:VERB
-0000ec60: 7c7e 7667 222c 2066 227b 645b 652d 315d  |~vg", f"{d[e-1]
-0000ec70: 2e6c 656d 6d61 5f7d 3a56 4552 423a 7e76  .lemma_}:VERB:~v
-0000ec80: 677c 7b64 5b73 5d2e 6c65 6d6d 615f 7d22  g|{d[s].lemma_}"
-0000ec90: 2c0a 0909 0909 6622 7b64 5b73 5d2e 6c65  ,.....f"{d[s].le
-0000eca0: 6d6d 615f 7d2f 5645 5242 7c76 673a 5f7b  mma_}/VERB|vg:_{
-0000ecb0: 645b 735d 2e6c 656d 6d61 5f7d 205f 7b64  d[s].lemma_} _{d
-0000ecc0: 5b65 2d31 5d2e 7461 675f 7d22 2c5d 7d7d  [e-1].tag_}",]}}
-0000ecd0: 2920 2c20 0a09 2276 6470 6722 3a20 6c61  ) , .."vdpg": la
-0000ece0: 6d62 6461 2064 2c73 2c65 2c74 6167 3a64  mbda d,s,e,tag:d
-0000ecf0: 2e75 7365 725f 6461 7461 2e75 7064 6174  .user_data.updat
-0000ed00: 6528 7b20 6622 7b74 6167 7d3a 7b64 5b73  e({ f"{tag}:{d[s
-0000ed10: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
-0000ed20: 3a65 5d2e 7465 7874 2e6c 6f77 6572 2829  :e].text.lower()
-0000ed30: 7d5b 7b73 7d2c 7b65 7d29 223a 0a09 097b  }[{s},{e})":...{
-0000ed40: 226e 6163 223a 205b 6622 7b64 5b73 5d2e  "nac": [f"{d[s].
-0000ed50: 6c65 6d6d 615f 7d3a 5645 5242 3a76 6470  lemma_}:VERB:vdp
-0000ed60: 677c 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  g|{d[s].lemma_} 
-0000ed70: 7b64 5b73 2b31 3a65 5d2e 7465 7874 7d22  {d[s+1:e].text}"
-0000ed80: 2c20 6622 7b64 5b73 5d2e 6c65 6d6d 615f  , f"{d[s].lemma_
-0000ed90: 7d3a 5645 5242 7c76 6470 6722 2c20 6622  }:VERB|vdpg", f"
-0000eda0: 5f7b 645b 735d 2e6c 656d 6d61 5f7d 207b  _{d[s].lemma_} {
-0000edb0: 645b 732b 313a 652d 315d 2e74 6578 747d  d[s+1:e-1].text}
-0000edc0: 205f 5642 4722 2c0a 0909 0909 6622 7b64   _VBG",.....f"{d
-0000edd0: 5b73 5d2e 6c65 6d6d 615f 7d2f 5645 5242  [s].lemma_}/VERB
-0000ede0: 7c76 6470 673a 5f7b 645b 735d 2e6c 656d  |vdpg:_{d[s].lem
-0000edf0: 6d61 5f7d 207b 645b 732b 313a 652d 315d  ma_} {d[s+1:e-1]
-0000ee00: 2e74 6578 747d 205f 7b64 5b65 2d31 5d2e  .text} _{d[e-1].
-0000ee10: 7461 675f 7d22 2c5d 207d 7d29 2c0a 097d  tag_}",] }}),..}
-0000ee20: 0a0a 6465 6620 706f 7374 6167 5f6d 6174  ..def postag_mat
-0000ee30: 6368 2864 6f63 2c20 6675 6e63 3d6c 616d  ch(doc, func=lam
-0000ee40: 6264 6120 646f 632c 7374 6172 742c 656e  bda doc,start,en
-0000ee50: 642c 7461 673a 2064 6f63 2e73 7061 6e73  d,tag: doc.spans
-0000ee60: 2e75 7064 6174 6528 7b66 2270 6f73 7461  .update({f"posta
-0000ee70: 675b 7b73 7461 7274 7d2c 7b65 6e64 7d29  g[{start},{end})
-0000ee80: 3a7b 7461 677d 223a 2053 7061 6e47 726f  :{tag}": SpanGro
-0000ee90: 7570 2864 6f63 2c20 6e61 6d65 3d74 6167  up(doc, name=tag
-0000eea0: 2c20 7370 616e 733d 5b20 646f 635b 7374  , spans=[ doc[st
-0000eeb0: 6172 7420 3a20 656e 645d 205d 2c20 6174  art : end] ], at
-0000eec0: 7472 733d 7b7d 2920 7d20 2920 293a 200a  trs={}) } ) ): .
-0000eed0: 0927 2727 2064 6f63 2e73 7061 6e73 5b66  .''' doc.spans[f
-0000eee0: 2273 7061 6e5b 7b73 7461 7274 7d2c 7b65  "span[{start},{e
-0000eef0: 6e64 7d29 3a7b 7461 677d 225d 203d 2053  nd}):{tag}"] = S
-0000ef00: 7061 6e47 726f 7570 2864 6f63 2c20 7c20  panGroup(doc, | 
-0000ef10: 6164 6420 6d61 7463 6865 6420 6e65 7720  add matched new 
-0000ef20: 7370 616e 2062 7920 7068 7261 7365 2072  span by phrase r
-0000ef30: 756c 6573 2c20 3230 3233 2e32 2e36 2027  ules, 2023.2.6 '
-0000ef40: 2727 0a09 6966 206e 6f74 2068 6173 6174  ''..if not hasat
-0000ef50: 7472 2870 6f73 7461 675f 6d61 7463 682c  tr(postag_match,
-0000ef60: 2027 6d61 7463 6865 7227 293a 2020 090a   'matcher'):  ..
-0000ef70: 0909 706f 7374 6167 5f6d 6174 6368 2e6d  ..postag_match.m
-0000ef80: 6174 6368 6572 203d 2070 6872 6173 655f  atcher = phrase_
-0000ef90: 6d61 7463 6865 7228 7b0a 0909 2270 726d  matcher({..."prm
-0000efa0: 6f64 7322 3a5b 5b7b 2250 4f53 223a 207b  ods":[[{"POS": {
-0000efb0: 2249 4e22 3a20 5b22 4155 5822 2c22 5645  "IN": ["AUX","VE
-0000efc0: 5242 225d 7d7d 2c7b 2250 4f53 223a 207b  RB"]}},{"POS": {
-0000efd0: 2249 4e22 3a20 5b22 4144 5622 5d7d 2c20  "IN": ["ADV"]}, 
-0000efe0: 224f 5022 3a20 222a 227d 2c20 7b22 504f  "OP": "*"}, {"PO
-0000eff0: 5322 3a20 7b22 494e 223a 205b 2241 444a  S": {"IN": ["ADJ
-0000f000: 222c 2256 4552 4222 5d7d 2c20 224f 5022  ","VERB"]}, "OP"
-0000f010: 3a20 222a 227d 2c7b 2250 4f53 223a 207b  : "*"},{"POS": {
-0000f020: 2249 4e22 3a20 5b22 5041 5254 222c 2241  "IN": ["PART","A
-0000f030: 4450 222c 2254 4f22 5d7d 2c20 224f 5022  DP","TO"]}, "OP"
-0000f040: 3a20 222a 227d 2c7b 2250 4f53 223a 2027  : "*"},{"POS": '
-0000f050: 5645 5242 277d 5d5d 2c20 2320 636f 756c  VERB'}]], # coul
-0000f060: 6420 6861 7264 6c79 2077 6169 7420 746f  d hardly wait to
-0000f070: 206d 6565 740a 0909 2256 5022 3a20 205b   meet..."VP":  [
-0000f080: 5b7b 2750 4f53 273a 2027 5645 5242 277d  [{'POS': 'VERB'}
-0000f090: 2c7b 2250 4f53 223a 207b 2249 4e22 3a20  ,{"POS": {"IN": 
-0000f0a0: 5b22 4445 5422 2c22 4144 5022 2c22 4144  ["DET","ADP","AD
-0000f0b0: 4a22 5d7d 2c20 224f 5022 3a20 222a 227d  J"]}, "OP": "*"}
-0000f0c0: 2c7b 2250 4f53 223a 2027 4e4f 554e 277d  ,{"POS": 'NOUN'}
-0000f0d0: 2c20 7b22 504f 5322 3a20 7b22 494e 223a  , {"POS": {"IN":
-0000f0e0: 205b 2241 4450 222c 2254 4f22 5d7d 2c20   ["ADP","TO"]}, 
-0000f0f0: 224f 5022 3a20 222a 227d 5d2c 205b 7b27  "OP": "*"}], [{'
-0000f100: 504f 5327 3a20 2756 4552 4227 7d2c 7b22  POS': 'VERB'},{"
-0000f110: 504f 5322 3a20 7b22 494e 223a 205b 2244  POS": {"IN": ["D
-0000f120: 4554 222c 2241 4450 222c 2241 444a 222c  ET","ADP","ADJ",
-0000f130: 2254 4f22 2c22 5041 5254 225d 7d2c 2022  "TO","PART"]}, "
-0000f140: 4f50 223a 2022 2a22 7d2c 7b22 504f 5322  OP": "*"},{"POS"
-0000f150: 3a20 2756 4552 4227 7d5d 5d2c 2023 2077  : 'VERB'}]], # w
-0000f160: 6169 7420 746f 206d 6565 740a 0909 2250  ait to meet..."P
-0000f170: 5022 3a20 205b 5b7b 2750 4f53 273a 2027  P":  [[{'POS': '
-0000f180: 4144 5027 7d2c 7b22 504f 5322 3a20 7b22  ADP'},{"POS": {"
-0000f190: 494e 223a 205b 2244 4554 222c 224e 554d  IN": ["DET","NUM
-0000f1a0: 222c 2241 444a 222c 2750 554e 4354 272c  ","ADJ",'PUNCT',
-0000f1b0: 2743 4f4e 4a27 5d7d 2c20 224f 5022 3a20  'CONJ']}, "OP": 
-0000f1c0: 222a 227d 2c7b 2250 4f53 223a 207b 2249  "*"},{"POS": {"I
-0000f1d0: 4e22 3a20 5b22 4e4f 554e 222c 2250 4152  N": ["NOUN","PAR
-0000f1e0: 5422 5d7d 2c20 224f 5022 3a20 222b 227d  T"]}, "OP": "+"}
-0000f1f0: 5d5d 2c20 2020 200a 0909 2241 5022 3a20  ]],    ..."AP": 
-0000f200: 205b 5b7b 2250 4f53 223a 207b 2249 4e22   [[{"POS": {"IN"
-0000f210: 3a20 5b22 4144 5622 5d7d 2c20 224f 5022  : ["ADV"]}, "OP"
-0000f220: 3a20 222b 227d 2c20 7b22 504f 5322 3a20  : "+"}, {"POS": 
-0000f230: 2741 444a 277d 5d5d 2c20 200a 0909 2276  'ADJ'}]],  ..."v
-0000f240: 706e 223a 205b 5b7b 2250 4f53 223a 2256  pn": [[{"POS":"V
-0000f250: 4552 4222 2c22 5441 4722 3a20 7b22 4e4f  ERB","TAG": {"NO
-0000f260: 545f 494e 223a 205b 2256 424e 225d 7d7d  T_IN": ["VBN"]}}
-0000f270: 2c20 7b22 504f 5322 3a22 4144 5022 7d20  , {"POS":"ADP"} 
-0000f280: 2c20 7b22 5441 4722 3a22 4e4e 222c 2022  , {"TAG":"NN", "
-0000f290: 4953 5f4c 4f57 4552 223a 5472 7565 7d5d  IS_LOWER":True}]
-0000f2a0: 5d2c 2020 2320 636f 6d65 2069 6e74 6f20  ],  # come into 
-0000f2b0: 666f 7263 6520 0a09 0922 6270 6e22 3a20  force ..."bpn": 
-0000f2c0: 5b5b 7b22 4c45 4d4d 4122 3a22 6265 227d  [[{"LEMMA":"be"}
-0000f2d0: 2c20 7b22 504f 5322 3a22 4144 5022 7d20  , {"POS":"ADP"} 
-0000f2e0: 2c20 7b22 5441 4722 3a22 4e4e 227d 5d5d  , {"TAG":"NN"}]]
-0000f2f0: 2c20 2023 2062 6520 696e 2066 6f72 6365  ,  # be in force
-0000f300: 203d 3e20 7670 6e20 0a09 0922 766e 7022   => vpn ..."vnp"
-0000f310: 3a20 5b5b 7b22 504f 5322 3a22 5645 5242  : [[{"POS":"VERB
-0000f320: 222c 2254 4147 223a 207b 224e 4f54 5f49  ","TAG": {"NOT_I
-0000f330: 4e22 3a20 5b22 5642 4e22 5d7d 7d2c 207b  N": ["VBN"]}}, {
-0000f340: 2254 4147 223a 224e 4e22 7d2c 207b 2250  "TAG":"NN"}, {"P
-0000f350: 4f53 223a 2241 4450 227d 205d 5d2c 2020  OS":"ADP"} ]],  
-0000f360: 2320 6d61 6b65 2075 7365 206f 662c 206c  # make use of, l
-0000f370: 6179 2065 6d70 6861 7369 7320 6f6e 0a09  ay emphasis on..
-0000f380: 0922 7670 223a 205b 5b7b 2250 4f53 223a  ."vp": [[{"POS":
-0000f390: 2256 4552 4222 2c22 5441 4722 3a20 7b22  "VERB","TAG": {"
-0000f3a0: 4e4f 545f 494e 223a 205b 2256 424e 225d  NOT_IN": ["VBN"]
-0000f3b0: 7d7d 2c20 7b22 504f 5322 3a22 4144 5022  }}, {"POS":"ADP"
-0000f3c0: 7d20 5d5d 2c20 2023 2061 6269 6465 2062  } ]],  # abide b
-0000f3d0: 7920 7c20 6469 7374 696e 6775 6973 6820  y | distinguish 
-0000f3e0: 6672 6f6d 0a09 0922 7670 7022 3a20 5b5b  from..."vpp": [[
-0000f3f0: 7b22 504f 5322 3a22 5645 5242 222c 2254  {"POS":"VERB","T
-0000f400: 4147 223a 207b 224e 4f54 5f49 4e22 3a20  AG": {"NOT_IN": 
-0000f410: 5b22 5642 4e22 5d7d 7d2c 207b 2250 4f53  ["VBN"]}}, {"POS
-0000f420: 223a 2241 4450 227d 2c20 7b22 504f 5322  ":"ADP"}, {"POS"
-0000f430: 3a22 4144 5022 7d20 5d5d 2c20 2320 6c69  :"ADP"} ]], # li
-0000f440: 7665 2075 7020 746f 0a09 0922 7670 6722  ve up to..."vpg"
-0000f450: 3a20 5b5b 7b22 504f 5322 3a22 5645 5242  : [[{"POS":"VERB
-0000f460: 222c 2254 4147 223a 207b 224e 4f54 5f49  ","TAG": {"NOT_I
-0000f470: 4e22 3a20 5b22 5642 4e22 5d7d 7d2c 207b  N": ["VBN"]}}, {
-0000f480: 2250 4f53 223a 2241 4450 227d 2c20 7b22  "POS":"ADP"}, {"
-0000f490: 5441 4722 3a22 5642 4722 2c22 4445 5022  TAG":"VBG","DEP"
-0000f4a0: 3a22 7063 6f6d 7022 7d20 5d5d 2c20 2320  :"pcomp"} ]], # 
-0000f4b0: 696e 7369 7374 6564 206f 6e20 676f 696e  insisted on goin
-0000f4c0: 670a 0909 2270 6e22 3a20 5b5b 7b22 504f  g..."pn": [[{"PO
-0000f4d0: 5322 3a22 4144 5022 2c20 2244 4550 223a  S":"ADP", "DEP":
-0000f4e0: 2270 7265 7022 7d20 2c20 7b22 5441 4722  "prep"} , {"TAG"
-0000f4f0: 3a22 4e4e 222c 2022 4445 5022 3a22 706f  :"NN", "DEP":"po
-0000f500: 626a 227d 5d5d 2c20 2023 2062 7920 666f  bj"}]],  # by fo
-0000f510: 7263 650a 0909 2270 6e70 223a 205b 5b7b  rce..."pnp": [[{
-0000f520: 2250 4f53 223a 2241 4450 222c 2022 4445  "POS":"ADP", "DE
-0000f530: 5022 3a22 7072 6570 227d 202c 207b 2254  P":"prep"} , {"T
-0000f540: 4147 223a 224e 4e22 2c20 2244 4550 223a  AG":"NN", "DEP":
-0000f550: 2270 6f62 6a22 7d2c 207b 2250 4f53 223a  "pobj"}, {"POS":
-0000f560: 2241 4450 222c 2022 4445 5022 3a22 7072  "ADP", "DEP":"pr
-0000f570: 6570 227d 5d5d 2c20 2023 206f 6e20 6163  ep"}]],  # on ac
-0000f580: 636f 756e 7420 6f66 0a09 0922 6261 7076  count of..."bapv
-0000f590: 223a 205b 5b7b 224c 454d 4d41 223a 2262  ": [[{"LEMMA":"b
-0000f5a0: 6522 7d20 2c20 7b22 5441 4722 3a7b 2249  e"} , {"TAG":{"I
-0000f5b0: 4e22 3a20 5b22 4a4a 225d 7d7d 2c20 7b22  N": ["JJ"]}}, {"
-0000f5c0: 504f 5322 3a22 4144 5022 7d2c 207b 2250  POS":"ADP"}, {"P
-0000f5d0: 4f53 223a 2256 4552 4222 7d5d 5d2c 2020  OS":"VERB"}]],  
-0000f5e0: 2320 0a09 0922 6261 7476 223a 205b 5b7b  # ..."batv": [[{
-0000f5f0: 224c 454d 4d41 223a 2262 6522 7d20 2c20  "LEMMA":"be"} , 
-0000f600: 7b22 5441 4722 3a7b 2249 4e22 3a20 5b22  {"TAG":{"IN": ["
-0000f610: 4a4a 225d 7d7d 2c20 7b22 4c45 4d4d 4122  JJ"]}}, {"LEMMA"
-0000f620: 3a22 746f 227d 2c20 7b22 504f 5322 3a22  :"to"}, {"POS":"
-0000f630: 5645 5242 227d 5d5d 2c20 200a 0909 2262  VERB"}]],  ..."b
-0000f640: 6570 7622 3a20 5b5b 7b22 4c45 4d4d 4122  epv": [[{"LEMMA"
-0000f650: 3a22 6265 227d 202c 207b 2254 4147 223a  :"be"} , {"TAG":
-0000f660: 7b22 494e 223a 205b 2256 424e 225d 7d7d  {"IN": ["VBN"]}}
-0000f670: 2c20 7b22 504f 5322 3a22 4144 5022 7d2c  , {"POS":"ADP"},
-0000f680: 207b 2250 4f53 223a 2256 4552 4222 7d5d   {"POS":"VERB"}]
-0000f690: 5d2c 2020 2320 6265 2066 6f72 6365 6420  ],  # be forced 
-0000f6a0: 6f66 2067 6f69 6e67 202f 203f 2062 6570  of going / ? bep
-0000f6b0: 763f 200a 0909 2262 6574 7622 3a20 5b5b  v? ..."betv": [[
-0000f6c0: 7b22 4c45 4d4d 4122 3a22 6265 227d 202c  {"LEMMA":"be"} ,
-0000f6d0: 207b 2254 4147 223a 7b22 494e 223a 205b   {"TAG":{"IN": [
-0000f6e0: 2256 424e 225d 7d7d 2c20 7b22 4c45 4d4d  "VBN"]}}, {"LEMM
-0000f6f0: 4122 3a22 746f 227d 2c20 7b22 5441 4722  A":"to"}, {"TAG"
-0000f700: 3a22 5642 227d 5d5d 2c20 2023 2062 6520  :"VB"}]],  # be 
-0000f710: 636f 6e73 6964 6572 6564 2074 6f20 6265  considered to be
-0000f720: 2f67 6f0a 0909 2262 6170 223a 205b 5b7b  /go..."bap": [[{
-0000f730: 224c 454d 4d41 223a 2262 6522 7d20 2c20  "LEMMA":"be"} , 
-0000f740: 7b22 5441 4722 3a7b 2249 4e22 3a20 5b22  {"TAG":{"IN": ["
-0000f750: 4a4a 225d 7d7d 2c20 7b22 504f 5322 3a22  JJ"]}}, {"POS":"
-0000f760: 4144 5022 7d5d 5d2c 2023 6265 2069 676e  ADP"}]], #be ign
-0000f770: 6f72 616e 7420 6f66 0a09 0922 6265 7022  orant of..."bep"
-0000f780: 3a20 5b5b 7b22 4c45 4d4d 4122 3a22 6265  : [[{"LEMMA":"be
-0000f790: 227d 202c 207b 2254 4147 223a 7b22 494e  "} , {"TAG":{"IN
-0000f7a0: 223a 205b 2256 424e 225d 7d7d 2c20 7b22  ": ["VBN"]}}, {"
-0000f7b0: 504f 5322 3a22 4144 5022 7d5d 5d2c 2020  POS":"ADP"}]],  
-0000f7c0: 2320 6265 2066 6f72 6365 6420 746f 0a09  # be forced to..
-0000f7d0: 0922 766f 7022 3a20 5b5b 7b22 504f 5322  ."vop": [[{"POS"
-0000f7e0: 3a22 5645 5242 222c 2254 4147 223a 207b  :"VERB","TAG": {
-0000f7f0: 224e 4f54 5f49 4e22 3a20 5b22 5642 4e22  "NOT_IN": ["VBN"
-0000f800: 5d7d 7d20 2c20 7b22 5445 5854 223a 207b  ]}} , {"TEXT": {
-0000f810: 2252 4547 4558 223a 2022 5b61 2d7a 5d2b  "REGEX": "[a-z]+
-0000f820: 7365 6c66 2422 7d7d 2c20 7b22 504f 5322  self$"}}, {"POS"
-0000f830: 3a22 4144 5022 7d5d 5d2c 2023 7468 726f  :"ADP"}]], #thro
-0000f840: 7720 6f6e 6573 656c 6620 696e 746f 0a09  w oneself into..
-0000f850: 0922 7674 7622 3a20 5b5b 7b22 504f 5322  ."vtv": [[{"POS"
-0000f860: 3a22 5645 5242 222c 2254 4147 223a 207b  :"VERB","TAG": {
-0000f870: 224e 4f54 5f49 4e22 3a20 5b22 5642 4e22  "NOT_IN": ["VBN"
-0000f880: 5d7d 7d2c 207b 224c 454d 4d41 223a 2274  ]}}, {"LEMMA":"t
-0000f890: 6f22 7d2c 207b 2250 4f53 223a 2256 4552  o"}, {"POS":"VER
-0000f8a0: 4222 2c20 2244 4550 223a 2278 636f 6d70  B", "DEP":"xcomp
-0000f8b0: 227d 205d 5d2c 200a 0909 2276 6722 3a20  "} ]], ..."vg": 
-0000f8c0: 5b5b 7b22 504f 5322 3a22 5645 5242 222c  [[{"POS":"VERB",
-0000f8d0: 2254 4147 223a 207b 224e 4f54 5f49 4e22  "TAG": {"NOT_IN"
-0000f8e0: 3a20 5b22 5642 4e22 5d7d 7d2c 2020 7b22  : ["VBN"]}},  {"
-0000f8f0: 5441 4722 3a22 5642 4722 2c20 2244 4550  TAG":"VBG", "DEP
-0000f900: 223a 2278 636f 6d70 227d 205d 5d2c 200a  ":"xcomp"} ]], .
-0000f910: 0909 2276 6470 6722 3a20 5b5b 7b22 504f  .."vdpg": [[{"PO
-0000f920: 5322 3a22 5645 5242 227d 2c20 207b 2250  S":"VERB"},  {"P
-0000f930: 4f53 223a 2241 4456 227d 202c 2020 7b22  OS":"ADV"} ,  {"
-0000f940: 504f 5322 3a22 4144 5022 7d20 2c20 207b  POS":"ADP"} ,  {
-0000f950: 2254 4147 223a 2256 4247 227d 205d 5d2c  "TAG":"VBG"} ]],
-0000f960: 2020 2320 6c6f 6f6b 2066 6f72 7761 7264    # look forward
-0000f970: 2074 6f20 7365 6569 6e67 0a09 097d 290a   to seeing...}).
-0000f980: 0966 6f72 206e 616d 652c 2073 7461 7274  .for name, start
-0000f990: 2c20 656e 6420 696e 2070 6f73 7461 675f  , end in postag_
-0000f9a0: 6d61 7463 682e 6d61 7463 6865 7228 646f  match.matcher(do
-0000f9b0: 6329 3a0a 0909 7472 793a 0a09 0909 7461  c):...try:....ta
-0000f9c0: 6720 3d20 7370 6163 792e 6e6c 702e 766f  g = spacy.nlp.vo
-0000f9d0: 6361 625b 6e61 6d65 5d2e 7465 7874 0a09  cab[name].text..
-0000f9e0: 0909 6966 2069 7369 6e73 7461 6e63 6528  ..if isinstance(
-0000f9f0: 6675 6e63 2c20 6469 6374 293a 2023 2074  func, dict): # t
-0000fa00: 6167 202d 3e20 6c61 6d62 6461 200a 0909  ag -> lambda ...
-0000fa10: 0909 6675 6e63 5b74 6167 5d28 646f 632c  ..func[tag](doc,
-0000fa20: 2073 7461 7274 2c20 656e 642c 2074 6167   start, end, tag
-0000fa30: 2920 6966 2074 6167 2069 6e20 6675 6e63  ) if tag in func
-0000fa40: 2065 6c73 6520 7072 696e 7428 2249 6e76   else print("Inv
-0000fa50: 616c 6964 2074 6167 3a22 2c20 7461 672c  alid tag:", tag,
-0000fa60: 2064 6f63 5b73 7461 7274 3a65 6e64 5d2e   doc[start:end].
-0000fa70: 7465 7874 2920 0a09 0909 656c 7365 3a20  text) ....else: 
-0000fa80: 0a09 0909 0966 756e 6328 646f 632c 2073  .....func(doc, s
-0000fa90: 7461 7274 2c20 656e 642c 2074 6167 2920  tart, end, tag) 
-0000faa0: 2023 2069 7320 6120 6675 6e63 746f 722c   # is a functor,
-0000fab0: 2023 646f 632e 7370 616e 735b 6622 706f   #doc.spans[f"po
-0000fac0: 7374 6167 5b7b 7374 6172 747d 2c7b 656e  stag[{start},{en
-0000fad0: 647d 293a 7b74 6167 7d22 5d20 3d20 5370  d}):{tag}"] = Sp
-0000fae0: 616e 4772 6f75 7028 646f 632c 206e 616d  anGroup(doc, nam
-0000faf0: 653d 7461 672c 2073 7061 6e73 3d5b 2064  e=tag, spans=[ d
-0000fb00: 6f63 5b73 7461 7274 203a 2065 6e64 5d20  oc[start : end] 
-0000fb10: 5d2c 2061 7474 7273 3d7b 7d29 2023 6174  ], attrs={}) #at
-0000fb20: 7472 7320 3d20 7b22 706f 7322 3a20 762e  trs = {"pos": v.
-0000fb30: 706f 735f 2c20 2274 6167 223a 2076 2e74  pos_, "tag": v.t
-0000fb40: 6167 5f2c 2022 6465 7022 3a20 762e 6465  ag_, "dep": v.de
-0000fb50: 705f 2c20 226c 656d 6d61 223a 762e 6c65  p_, "lemma":v.le
-0000fb60: 6d6d 615f 2c20 2265 6e74 5f74 7970 6522  mma_, "ent_type"
-0000fb70: 3a20 2253 2e22 202b 2076 2e64 6570 5f20  : "S." + v.dep_ 
-0000fb80: 7d20 0a09 0965 7863 6570 7420 4578 6365  } ...except Exce
-0000fb90: 7074 696f 6e20 6173 2065 3a0a 0909 0970  ption as e:....p
-0000fba0: 7269 6e74 2028 2270 6f73 7461 675f 6d61  rint ("postag_ma
-0000fbb0: 7463 6820 6578 3a22 2c20 652c 206e 616d  tch ex:", e, nam
-0000fbc0: 652c 2073 7461 7274 2c20 656e 6429 200a  e, start, end) .
-0000fbd0: 0a64 6566 2073 6b65 6e70 5f6d 6174 6368  .def skenp_match
-0000fbe0: 2864 6f63 2c20 6675 6e63 3d6c 616d 6264  (doc, func=lambd
-0000fbf0: 6120 646f 632c 7374 6172 742c 656e 642c  a doc,start,end,
-0000fc00: 7461 673a 2064 6f63 2e73 7061 6e73 2e75  tag: doc.spans.u
-0000fc10: 7064 6174 6528 7b66 2273 6b65 6e70 5b7b  pdate({f"skenp[{
-0000fc20: 7374 6172 747d 2c7b 656e 647d 293a 7b74  start},{end}):{t
-0000fc30: 6167 7d22 3a20 5370 616e 4772 6f75 7028  ag}": SpanGroup(
-0000fc40: 646f 632c 206e 616d 653d 7461 672c 2073  doc, name=tag, s
-0000fc50: 7061 6e73 3d5b 2064 6f63 5b73 7461 7274  pans=[ doc[start
-0000fc60: 203a 2065 6e64 5d20 5d2c 2061 7474 7273   : end] ], attrs
-0000fc70: 3d7b 7d29 207d 2029 293a 200a 0969 6620  ={}) } )): ..if 
-0000fc80: 6e6f 7420 6861 7361 7474 7228 736b 656e  not hasattr(sken
-0000fc90: 705f 6d61 7463 682c 2027 6d61 7463 6865  p_match, 'matche
-0000fca0: 7227 293a 2073 6b65 6e70 5f6d 6174 6368  r'): skenp_match
-0000fcb0: 2e6d 6174 6368 6572 203d 2070 6872 6173  .matcher = phras
-0000fcc0: 655f 6d61 7463 6865 7228 7b0a 0922 766e  e_matcher({.."vn
-0000fcd0: 704e 223a 205b 5b7b 2250 4f53 223a 2256  pN": [[{"POS":"V
-0000fce0: 4552 4222 2c22 5441 4722 3a20 7b22 4e4f  ERB","TAG": {"NO
-0000fcf0: 545f 494e 223a 205b 2256 424e 225d 7d7d  T_IN": ["VBN"]}}
-0000fd00: 2c20 7b22 454e 545f 5459 5045 223a 224e  , {"ENT_TYPE":"N
-0000fd10: 5022 7d2c 207b 2250 4f53 223a 7b22 494e  P"}, {"POS":{"IN
-0000fd20: 223a 205b 2241 4450 225d 7d7d 2c20 7b22  ": ["ADP"]}}, {"
-0000fd30: 454e 545f 5459 5045 223a 224e 5022 7d5d  ENT_TYPE":"NP"}]
-0000fd40: 5d2c 2020 2320 7265 6d69 6e64 205f 4e50  ],  # remind _NP
-0000fd50: 206f 6620 5f4e 5020 2c20 6272 696e 6720   of _NP , bring 
-0000fd60: 5f4e 5020 746f 206c 6966 650a 0922 766e  _NP to life.."vn
-0000fd70: 706e 223a 205b 5b7b 2250 4f53 223a 2256  pn": [[{"POS":"V
-0000fd80: 4552 4222 2c22 5441 4722 3a20 7b22 4e4f  ERB","TAG": {"NO
-0000fd90: 545f 494e 223a 205b 2256 424e 225d 7d7d  T_IN": ["VBN"]}}
-0000fda0: 2c20 7b22 454e 545f 5459 5045 223a 224e  , {"ENT_TYPE":"N
-0000fdb0: 5022 7d2c 207b 2250 4f53 223a 7b22 494e  P"}, {"POS":{"IN
-0000fdc0: 223a 205b 2241 4450 225d 7d7d 2c20 7b22  ": ["ADP"]}}, {"
-0000fdd0: 5441 4722 3a22 4e4e 227d 5d5d 2c20 2023  TAG":"NN"}]],  #
-0000fde0: 2074 616b 6520 5f4e 5020 696e 746f 2061   take _NP into a
-0000fdf0: 6363 6f75 6e74 0a09 2276 706e 706e 223a  ccount.."vpnpn":
-0000fe00: 205b 5b7b 2250 4f53 223a 2256 4552 4222   [[{"POS":"VERB"
-0000fe10: 2c22 5441 4722 3a20 7b22 4e4f 545f 494e  ,"TAG": {"NOT_IN
-0000fe20: 223a 205b 2256 424e 225d 7d7d 2c20 7b22  ": ["VBN"]}}, {"
-0000fe30: 504f 5322 3a7b 2249 4e22 3a20 5b22 4144  POS":{"IN": ["AD
-0000fe40: 5022 5d7d 7d2c 207b 2245 4e54 5f54 5950  P"]}}, {"ENT_TYP
-0000fe50: 4522 3a22 4e50 227d 2c20 7b22 504f 5322  E":"NP"}, {"POS"
-0000fe60: 3a7b 2249 4e22 3a20 5b22 4144 5022 5d7d  :{"IN": ["ADP"]}
-0000fe70: 7d2c 207b 2245 4e54 5f54 5950 4522 3a22  }, {"ENT_TYPE":"
-0000fe80: 4e50 227d 5d5d 2c20 2023 2076 6172 7920  NP"}]],  # vary 
-0000fe90: 6672 6f6d 205f 4e50 2074 6f20 5f4e 5020  from _NP to _NP 
-0000fea0: 0a09 2276 6e70 6522 3a20 5b5b 7b22 504f  .."vnpe": [[{"PO
-0000feb0: 5322 3a22 5645 5242 222c 2254 4147 223a  S":"VERB","TAG":
-0000fec0: 207b 224e 4f54 5f49 4e22 3a20 5b22 5642   {"NOT_IN": ["VB
-0000fed0: 4e22 5d7d 7d2c 207b 2245 4e54 5f54 5950  N"]}}, {"ENT_TYP
-0000fee0: 4522 3a22 4e50 227d 2c20 7b22 5441 4722  E":"NP"}, {"TAG"
-0000fef0: 3a22 494e 227d 2c20 7b22 5441 4722 3a22  :"IN"}, {"TAG":"
-0000ff00: 5642 4e22 7d5d 5d2c 2020 2320 7461 6b65  VBN"}]],  # take
-0000ff10: 205f 4e50 2066 6f72 2f61 7320 6772 616e   _NP for/as gran
-0000ff20: 7465 640a 0922 7670 706e 223a 205b 5b7b  ted.."vppn": [[{
-0000ff30: 2250 4f53 223a 2256 4552 4222 7d2c 207b  "POS":"VERB"}, {
-0000ff40: 2250 4f53 223a 2241 4450 227d 2c20 7b22  "POS":"ADP"}, {"
-0000ff50: 504f 5322 3a22 4144 5022 7d2c 207b 2245  POS":"ADP"}, {"E
-0000ff60: 4e54 5f54 5950 4522 3a22 4e50 227d 205d  NT_TYPE":"NP"} ]
-0000ff70: 5d2c 2020 2320 6c69 7665 2075 7020 746f  ],  # live up to
-0000ff80: 205f 4e50 0a09 2276 6470 6e22 3a20 5b5b   _NP.."vdpn": [[
-0000ff90: 7b22 504f 5322 3a22 5645 5242 227d 2c20  {"POS":"VERB"}, 
-0000ffa0: 7b22 504f 5322 3a22 4144 5622 7d2c 207b  {"POS":"ADV"}, {
-0000ffb0: 2250 4f53 223a 2241 4450 227d 2c20 7b22  "POS":"ADP"}, {"
-0000ffc0: 454e 545f 5459 5045 223a 224e 5022 7d20  ENT_TYPE":"NP"} 
-0000ffd0: 5d5d 2c20 2023 206c 6f6f 6b20 6261 636b  ]],  # look back
-0000ffe0: 206f 6e20 5f4e 5020 0a09 2276 706e 6e22   on _NP .."vpnn"
-0000fff0: 3a20 5b5b 7b22 504f 5322 3a22 5645 5242  : [[{"POS":"VERB
-00010000: 227d 2c20 7b22 504f 5322 3a22 4144 5022  "}, {"POS":"ADP"
-00010010: 7d2c 207b 2254 4147 223a 224e 4f55 4e22  }, {"TAG":"NOUN"
+000066b0: 6570 222c 2022 5249 4748 545f 4154 5452  ep", "RIGHT_ATTR
+000066c0: 5322 3a20 7b22 4445 5022 3a20 2270 7265  S": {"DEP": "pre
+000066d0: 7022 7d7d 2c20 7b22 4c45 4654 5f49 4422  p"}}, {"LEFT_ID"
+000066e0: 3a20 2270 7265 7022 2c20 2252 454c 5f4f  : "prep", "REL_O
+000066f0: 5022 3a20 223e 222c 2022 5249 4748 545f  P": ">", "RIGHT_
+00006700: 4944 223a 2022 6f62 6a65 6374 222c 2022  ID": "object", "
+00006710: 5249 4748 545f 4154 5452 5322 3a20 7b22  RIGHT_ATTRS": {"
+00006720: 4445 5022 3a20 2270 6f62 6a22 7d7d 5d2c  DEP": "pobj"}}],
+00006730: 200a 2320 7661 7279 2066 726f 6d20 4120   .# vary from A 
+00006740: 746f 2042 0a22 7670 6e70 6e22 3a5b 207b  to B."vpnpn":[ {
+00006750: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
+00006760: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
+00006770: 2250 4f53 223a 2022 5645 5242 227d 7d2c  "POS": "VERB"}},
+00006780: 207b 224c 4546 545f 4944 223a 2022 7622   {"LEFT_ID": "v"
+00006790: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
+000067a0: 2022 5249 4748 545f 4944 223a 2022 7072   "RIGHT_ID": "pr
+000067b0: 6570 3122 2c20 2252 4947 4854 5f41 5454  ep1", "RIGHT_ATT
+000067c0: 5253 223a 207b 2244 4550 223a 2022 7072  RS": {"DEP": "pr
+000067d0: 6570 227d 7d2c 7b22 4c45 4654 5f49 4422  ep"}},{"LEFT_ID"
+000067e0: 3a20 2270 7265 7031 222c 2022 5245 4c5f  : "prep1", "REL_
+000067f0: 4f50 223a 2022 3e22 2c20 2252 4947 4854  OP": ">", "RIGHT
+00006800: 5f49 4422 3a20 226f 626a 6563 7431 222c  _ID": "object1",
+00006810: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
+00006820: 7b22 4445 5022 3a20 2270 6f62 6a22 7d7d  {"DEP": "pobj"}}
+00006830: 2c7b 224c 4546 545f 4944 223a 2022 7622  ,{"LEFT_ID": "v"
+00006840: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
+00006850: 2022 5249 4748 545f 4944 223a 2022 7072   "RIGHT_ID": "pr
+00006860: 6570 3222 2c20 2252 4947 4854 5f41 5454  ep2", "RIGHT_ATT
+00006870: 5253 223a 207b 2244 4550 223a 2022 7072  RS": {"DEP": "pr
+00006880: 6570 227d 7d2c 7b22 4c45 4654 5f49 4422  ep"}},{"LEFT_ID"
+00006890: 3a20 2270 7265 7032 222c 2022 5245 4c5f  : "prep2", "REL_
+000068a0: 4f50 223a 2022 3e22 2c20 2252 4947 4854  OP": ">", "RIGHT
+000068b0: 5f49 4422 3a20 226f 626a 6563 7432 222c  _ID": "object2",
+000068c0: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
+000068d0: 7b22 4445 5022 3a20 2270 6f62 6a22 7d7d  {"DEP": "pobj"}}
+000068e0: 5d2c 200a 2320 7475 726e 2069 7420 646f  ], .# turn it do
+000068f0: 776e 0a22 766e 7022 3a5b 207b 2022 5249  wn."vnp":[ { "RI
+00006900: 4748 545f 4944 223a 2022 7622 2c22 5249  GHT_ID": "v","RI
+00006910: 4748 545f 4154 5452 5322 3a20 7b22 504f  GHT_ATTRS": {"PO
+00006920: 5322 3a20 2256 4552 4222 7d7d 2c7b 224c  S": "VERB"}},{"L
+00006930: 4546 545f 4944 223a 2022 7622 2c22 5245  EFT_ID": "v","RE
+00006940: 4c5f 4f50 223a 2022 3e22 2c22 5249 4748  L_OP": ">","RIGH
+00006950: 545f 4944 223a 2022 6f62 6a65 6374 222c  T_ID": "object",
+00006960: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
+00006970: 7b22 4445 5022 3a20 2264 6f62 6a22 7d7d  {"DEP": "dobj"}}
+00006980: 2c7b 224c 4546 545f 4944 223a 2022 7622  ,{"LEFT_ID": "v"
+00006990: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
+000069a0: 2252 4947 4854 5f49 4422 3a20 2273 7562  "RIGHT_ID": "sub
+000069b0: 6a65 6374 222c 2022 5249 4748 545f 4154  ject", "RIGHT_AT
+000069c0: 5452 5322 3a20 7b22 4445 5022 3a20 2270  TRS": {"DEP": "p
+000069d0: 7274 227d 7d5d 2c20 0a23 206d 616b 6520  rt"}}], .# make 
+000069e0: 7573 6520 6f66 2062 6f6f 6b73 2c20 7461  use of books, ta
+000069f0: 6b65 2073 7468 2069 6e74 6f20 6163 636f  ke sth into acco
+00006a00: 756e 740a 2276 6e70 6e22 3a5b 207b 2252  unt."vnpn":[ {"R
+00006a10: 4947 4854 5f49 4422 3a20 2276 222c 2022  IGHT_ID": "v", "
+00006a20: 5249 4748 545f 4154 5452 5322 3a20 7b22  RIGHT_ATTRS": {"
+00006a30: 504f 5322 3a20 2256 4552 4222 7d7d 2c7b  POS": "VERB"}},{
+00006a40: 224c 4546 545f 4944 223a 2022 7622 2c20  "LEFT_ID": "v", 
+00006a50: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
+00006a60: 5249 4748 545f 4944 223a 2022 6f62 6a65  RIGHT_ID": "obje
+00006a70: 6374 222c 2252 4947 4854 5f41 5454 5253  ct","RIGHT_ATTRS
+00006a80: 223a 207b 2244 4550 223a 2022 646f 626a  ": {"DEP": "dobj
+00006a90: 227d 7d2c 7b22 4c45 4654 5f49 4422 3a20  "}},{"LEFT_ID": 
+00006aa0: 226f 626a 6563 7422 2c22 5245 4c5f 4f50  "object","REL_OP
+00006ab0: 223a 2022 3e22 2c20 2252 4947 4854 5f49  ": ">", "RIGHT_I
+00006ac0: 4422 3a20 2270 7265 7022 2c20 2252 4947  D": "prep", "RIG
+00006ad0: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
+00006ae0: 223a 2022 7072 6570 227d 7d2c 7b22 4c45  ": "prep"}},{"LE
+00006af0: 4654 5f49 4422 3a20 2270 7265 7022 2c20  FT_ID": "prep", 
+00006b00: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
+00006b10: 5249 4748 545f 4944 223a 2022 706f 626a  RIGHT_ID": "pobj
+00006b20: 222c 2022 5249 4748 545f 4154 5452 5322  ", "RIGHT_ATTRS"
+00006b30: 3a20 7b22 4445 5022 3a20 2270 6f62 6a22  : {"DEP": "pobj"
+00006b40: 7d7d 2020 5d2c 200a 7d20 2320 666f 7220  }}  ], .} # for 
+00006b50: 6e61 6d65 2c20 6172 2069 6e20 6465 706d  name, ar in depm
+00006b60: 6174 6368 6572 735b 2773 7678 275d 2864  atchers['svx'](d
+00006b70: 6f63 2920 3a20 7072 696e 7428 646f 635b  oc) : print(doc[
+00006b80: 6172 5b31 5d5d 2c20 646f 635b 6172 5b30  ar[1]], doc[ar[0
+00006b90: 5d5d 2c20 646f 635b 6172 5b32 5d5d 290a  ]], doc[ar[2]]).
+00006ba0: 0a64 6566 2064 6570 5f6d 6174 6368 6572  .def dep_matcher
+00006bb0: 2864 6f63 293a 2023 5b28 2773 7678 272c  (doc): #[('svx',
+00006bc0: 205b 312c 2030 2c20 325d 295d 0a09 6966   [1, 0, 2])]..if
+00006bd0: 206e 6f74 2068 6173 6174 7472 2864 6570   not hasattr(dep
+00006be0: 5f6d 6174 6368 6572 2c20 276d 6174 6368  _matcher, 'match
+00006bf0: 6572 2729 3a20 0a09 0964 6570 5f6d 6174  er'): ...dep_mat
+00006c00: 6368 6572 2e6d 6174 6368 6572 203d 2044  cher.matcher = D
+00006c10: 6570 656e 6465 6e63 794d 6174 6368 6572  ependencyMatcher
+00006c20: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
+00006c30: 290a 0909 5b64 6570 5f6d 6174 6368 6572  )...[dep_matcher
+00006c40: 2e6d 6174 6368 6572 2e61 6464 286e 616d  .matcher.add(nam
+00006c50: 652c 205b 7061 7474 6572 6e5d 2920 666f  e, [pattern]) fo
+00006c60: 7220 6e61 6d65 2c20 7061 7474 6572 6e20  r name, pattern 
+00006c70: 696e 205f 6465 705f 7275 6c65 732e 6974  in _dep_rules.it
+00006c80: 656d 7328 2920 5d0a 0972 6574 7572 6e20  ems() ]..return 
+00006c90: 5b28 7370 6163 792e 6e6c 702e 766f 6361  [(spacy.nlp.voca
+00006ca0: 625b 6e61 6d65 5d2e 7465 7874 2c20 6172  b[name].text, ar
+00006cb0: 2920 666f 7220 6e61 6d65 2c20 6172 2069  ) for name, ar i
+00006cc0: 6e20 6465 705f 6d61 7463 6865 722e 6d61  n dep_matcher.ma
+00006cd0: 7463 6865 7228 646f 6329 5d20 0a09 2366  tcher(doc)] ..#f
+00006ce0: 6f72 206e 616d 652c 2061 7220 696e 2064  or name, ar in d
+00006cf0: 6570 6d61 7463 6865 7273 5b27 7376 7827  epmatchers['svx'
+00006d00: 5d28 646f 6329 203a 2070 7269 6e74 2864  ](doc) : print(d
+00006d10: 6f63 5b61 725b 315d 5d2c 2064 6f63 5b61  oc[ar[1]], doc[a
+00006d20: 725b 305d 5d2c 2064 6f63 5b61 725b 325d  r[0]], doc[ar[2]
+00006d30: 5d29 0a0a 6573 5f74 6f6b 7320 3d20 6c61  ])..es_toks = la
+00006d40: 6d62 6461 2073 6964 2c20 646f 633a 2020  mbda sid, doc:  
+00006d50: 5b20 7b27 5f69 6427 3a20 6622 7b73 6964  [ {'_id': f"{sid
+00006d60: 7d2d 746f 6b2d 7b74 2e69 7d22 2c20 275f  }-tok-{t.i}", '_
+00006d70: 736f 7572 6365 273a 207b 2274 7970 6522  source': {"type"
+00006d80: 3a22 746f 6b22 2c20 2273 7263 223a 7369  :"tok", "src":si
+00006d90: 642c 2027 6927 3a74 2e69 2c20 2268 6561  d, 'i':t.i, "hea
+00006da0: 6422 3a74 2e68 6561 642e 692c 2027 6c65  d":t.head.i, 'le
+00006db0: 7827 3a74 2e74 6578 742c 2027 6c65 6d27  x':t.text, 'lem'
+00006dc0: 3a74 2e6c 656d 6d61 5f2c 2027 706f 7327  :t.lemma_, 'pos'
+00006dd0: 3a74 2e70 6f73 5f2c 2027 7461 6727 3a74  :t.pos_, 'tag':t
+00006de0: 2e74 6167 5f2c 2027 6465 7027 3a74 2e64  .tag_, 'dep':t.d
+00006df0: 6570 5f2c 2022 6770 6f73 223a 742e 6865  ep_, "gpos":t.he
+00006e00: 6164 2e70 6f73 5f2c 2022 676c 656d 223a  ad.pos_, "glem":
+00006e10: 742e 6865 6164 2e6c 656d 6d61 5f20 7d20  t.head.lemma_ } 
+00006e20: 7d20 666f 7220 7420 696e 2064 6f63 205d  } for t in doc ]
+00006e30: 200a 6465 6620 6573 5f70 6f73 7461 6728   .def es_postag(
+00006e40: 646f 6329 3a20 0a09 6672 6f6d 2064 6963  doc): ..from dic
+00006e50: 2e6f 6e65 7365 6c66 2069 6d70 6f72 7420  .oneself import 
+00006e60: 6f6e 6573 656c 6620 0a09 7265 7475 726e  oneself ..return
+00006e70: 2022 5f5e 2022 202b 2027 2027 2e6a 6f69   "_^ " + ' '.joi
+00006e80: 6e28 5b20 6622 7b74 2e74 6578 747d 5f7b  n([ f"{t.text}_{
+00006e90: 742e 706f 735f 7d5f 7b74 2e74 6167 5f7d  t.pos_}_{t.tag_}
+00006ea0: 2220 6966 2074 2e70 6f73 5f20 696e 2028  " if t.pos_ in (
+00006eb0: 2750 524f 504e 272c 274e 554d 272c 2758  'PROPN','NUM','X
+00006ec0: 272c 2753 5041 4345 272c 2750 554e 4354  ','SPACE','PUNCT
+00006ed0: 2729 2065 6c73 6520 6622 7b74 2e74 6578  ') else f"{t.tex
+00006ee0: 747d 5f7b 742e 6c65 6d6d 615f 7d5f 7b74  t}_{t.lemma_}_{t
+00006ef0: 2e70 6f73 5f7d 5f7b 742e 7461 675f 7d7b  .pos_}_{t.tag_}{
+00006f00: 6f6e 6573 656c 662e 6765 7428 742e 7465  oneself.get(t.te
+00006f10: 7874 2e6c 6f77 6572 2829 2c20 2727 297d  xt.lower(), '')}
+00006f20: 2220 2066 6f72 2074 2069 6e20 646f 635d  "  for t in doc]
+00006f30: 2920 2320 756e 6971 2062 7920 616e 6120  ) # uniq by ana 
+00006f40: 232c 2750 554e 4354 270a 6465 6620 6573  #,'PUNCT'.def es
+00006f50: 5f68 7962 2864 6f63 293a 200a 0966 726f  _hyb(doc): ..fro
+00006f60: 6d20 6469 632e 6f6e 6573 656c 6620 696d  m dic.oneself im
+00006f70: 706f 7274 206f 6e65 7365 6c66 200a 0961  port oneself ..a
+00006f80: 7272 203d 205b 2066 227b 742e 7465 7874  rr = [ f"{t.text
+00006f90: 7d5f 7b74 2e70 6f73 5f7d 5f7b 742e 7461  }_{t.pos_}_{t.ta
+00006fa0: 675f 7d22 2069 6620 742e 706f 735f 2069  g_}" if t.pos_ i
+00006fb0: 6e20 2827 5052 4f50 4e27 2c27 4e55 4d27  n ('PROPN','NUM'
+00006fc0: 2c27 5827 2c27 5350 4143 4527 2c27 5055  ,'X','SPACE','PU
+00006fd0: 4e43 5427 2920 656c 7365 2066 227b 742e  NCT') else f"{t.
+00006fe0: 7465 7874 7d5f 7b74 2e6c 656d 6d61 5f7d  text}_{t.lemma_}
+00006ff0: 5f7b 742e 706f 735f 7d5f 7b74 2e74 6167  _{t.pos_}_{t.tag
+00007000: 5f7d 7b6f 6e65 7365 6c66 2e67 6574 2874  _}{oneself.get(t
+00007010: 2e74 6578 742e 6c6f 7765 7228 292c 2027  .text.lower(), '
+00007020: 2729 7d22 2020 666f 7220 7420 696e 2064  ')}"  for t in d
+00007030: 6f63 5d0a 0972 6574 7572 6e20 225f 5e20  oc]..return "_^ 
+00007040: 2220 2b20 2720 272e 6a6f 696e 2820 5b73  " + ' '.join( [s
+00007050: 2069 6620 275f 5055 4e43 5427 2069 6e20   if '_PUNCT' in 
+00007060: 7320 656c 7365 2066 227b 737d 5f2a 2220  s else f"{s}_*" 
+00007070: 666f 7220 7320 696e 2061 7272 5d29 2023  for s in arr]) #
+00007080: 2073 7570 706f 7274 203a 2020 6120 5f2a   support :  a _*
+00007090: 2062 6f6f 6b20 7c20 6120 5f2a 205f 2a20   book | a _* _* 
+000070a0: 626f 6f6b 0a0a 2320 6164 6465 6420 3230  book..# added 20
+000070b0: 3233 2e31 2e31 362c 206e 6f74 2074 6573  23.1.16, not tes
+000070c0: 7465 6420 7965 740a 636c 5f72 6f6f 7420  ted yet.cl_root 
+000070d0: 3d20 6c61 6d62 6461 2074 3a20 742e 6465  = lambda t: t.de
+000070e0: 705f 2021 3d20 2752 4f4f 5427 2061 6e64  p_ != 'ROOT' and
+000070f0: 2028 2028 742e 706f 735f 203d 3d20 2756   ( (t.pos_ == 'V
+00007100: 4552 4227 2061 6e64 2074 2e74 6167 5f20  ERB' and t.tag_ 
+00007110: 213d 2027 5642 4e27 2920 206f 7220 2874  != 'VBN')  or (t
+00007120: 2e70 6f73 5f20 3d3d 2027 4155 5827 2061  .pos_ == 'AUX' a
+00007130: 6e64 2074 2e6c 656d 6d61 5f20 3d3d 2027  nd t.lemma_ == '
+00007140: 6265 2729 2029 0a64 6566 206d 6172 6b5f  be') ).def mark_
+00007150: 636c 2864 6f63 293a 0a20 2020 2066 6f72  cl(doc):.    for
+00007160: 2074 2069 6e20 646f 633a 200a 2020 2020   t in doc: .    
+00007170: 2020 2020 6966 2063 6c5f 726f 6f74 2874      if cl_root(t
+00007180: 2920 3a20 742e 656e 745f 6964 5f20 3d20  ) : t.ent_id_ = 
+00007190: 2763 6c5f 726f 6f74 270a 6c65 6176 655f  'cl_root'.leave_
+000071a0: 636c 203d 206c 616d 6264 6120 743a 2063  cl = lambda t: c
+000071b0: 6c5f 726f 6f74 2874 2920 616e 6420 6c65  l_root(t) and le
+000071c0: 6e28 5b74 7220 666f 7220 7472 2069 6e20  n([tr for tr in 
+000071d0: 742e 7375 6274 7265 6520 6966 2074 722e  t.subtree if tr.
+000071e0: 656e 745f 6964 5f20 3d3d 2027 636c 5f72  ent_id_ == 'cl_r
+000071f0: 6f6f 7427 5d29 203d 3d20 310a 6465 6620  oot']) == 1.def 
+00007200: 6d65 7267 655f 6c65 6176 655f 636c 2864  merge_leave_cl(d
+00007210: 6f63 293a 2023 646f 6320 3d20 7370 6163  oc): #doc = spac
+00007220: 792e 6e6c 7028 2257 6869 6c65 2049 2077  y.nlp("While I w
+00007230: 6173 2074 6872 696c 6c65 6420 7468 6174  as thrilled that
+00007240: 2069 7420 7761 7320 6f6b 2c20 4920 776f   it was ok, I wo
+00007250: 7272 6965 6420 7468 6174 2049 2077 6f75  rried that I wou
+00007260: 6c64 2066 6169 6c2e 2229 0a09 6d61 726b  ld fail.")..mark
+00007270: 5f63 6c28 646f 6329 0a09 7769 7468 2064  _cl(doc)..with d
+00007280: 6f63 2e72 6574 6f6b 656e 697a 6528 2920  oc.retokenize() 
+00007290: 6173 2072 6574 6f6b 656e 697a 6572 3a0a  as retokenizer:.
+000072a0: 0909 666f 7220 7620 696e 205b 7420 666f  ..for v in [t fo
+000072b0: 7220 7420 696e 2064 6f63 2069 6620 6c65  r t in doc if le
+000072c0: 6176 655f 636c 2874 2920 5d20 3a20 2320  ave_cl(t) ] : # 
+000072d0: 6e6f 6e2d 726f 6f74 0a09 0909 7472 793a  non-root....try:
+000072e0: 0a09 0909 0963 6869 6c64 7265 6e20 3d20  .....children = 
+000072f0: 6c69 7374 2876 2e73 7562 7472 6565 290a  list(v.subtree).
+00007300: 0909 0909 7374 6172 7420 3d20 6368 696c  ....start = chil
+00007310: 6472 656e 5b30 5d2e 6920 2009 0a09 0909  dren[0].i  .....
+00007320: 0965 6e64 203d 2063 6869 6c64 7265 6e5b  .end = children[
+00007330: 2d31 5d2e 6920 0a09 0909 0961 7474 7273  -1].i .....attrs
+00007340: 203d 207b 2270 6f73 223a 2076 2e70 6f73   = {"pos": v.pos
+00007350: 2c20 2274 6167 223a 2076 2e74 6167 2c20  , "tag": v.tag, 
+00007360: 2264 6570 223a 2076 2e64 6570 2c20 226c  "dep": v.dep, "l
+00007370: 656d 6d61 223a 762e 6c65 6d6d 612c 2022  emma":v.lemma, "
+00007380: 656e 745f 7479 7065 223a 2022 532e 2220  ent_type": "S." 
+00007390: 2b20 762e 6465 705f 207d 2023 2053 2e61  + v.dep_ } # S.a
+000073a0: 6476 636c 202c 2020 532e 636f 6e6a 200a  dvcl ,  S.conj .
+000073b0: 0909 0909 6966 2076 2e64 6570 5f20 6e6f  ....if v.dep_ no
+000073c0: 7420 696e 2028 2778 636f 6d70 2729 2061  t in ('xcomp') a
+000073d0: 6e64 2064 6f63 5b73 7461 7274 5d2e 6c65  nd doc[start].le
+000073e0: 6d6d 615f 206e 6f74 2069 6e20 2827 746f  mma_ not in ('to
+000073f0: 2729 2061 6e64 2064 6f63 5b73 7461 7274  ') and doc[start
+00007400: 5d2e 7461 675f 206e 6f74 2069 6e20 2827  ].tag_ not in ('
+00007410: 544f 2729 3a20 2320 736b 6970 2074 6f2d  TO'): # skip to-
+00007420: 636c 6175 7365 2020 7c20 4865 206d 6164  clause  | He mad
+00007430: 6520 7468 6520 6368 6f69 6365 2074 6f20  e the choice to 
+00007440: 6769 7665 2061 6c6c 2068 6973 206d 6f6e  give all his mon
+00007450: 6579 2061 7761 7920 2e0a 0909 0909 0972  ey away .......r
+00007460: 6574 6f6b 656e 697a 6572 2e6d 6572 6765  etokenizer.merge
+00007470: 2864 6f63 5b73 7461 7274 203a 2065 6e64  (doc[start : end
+00007480: 2b31 5d2c 2061 7474 7273 3d61 7474 7273  +1], attrs=attrs
+00007490: 290a 0909 0965 7863 6570 7420 4578 6365  )....except Exce
+000074a0: 7074 696f 6e20 6173 2065 3a0a 0909 0909  ption as e:.....
+000074b0: 7072 696e 7420 2820 226d 6572 6765 5f6c  print ( "merge_l
+000074c0: 6561 7665 5f63 6c20 6578 3a22 2c20 652c  eave_cl ex:", e,
+000074d0: 2076 2029 0a09 7265 7475 726e 2064 6f63   v )..return doc
+000074e0: 200a 0a64 6566 206d 6572 6765 5f63 636f   ..def merge_cco
+000074f0: 6d70 2864 6f63 293a 2023 646f 6320 3d20  mp(doc): #doc = 
+00007500: 7370 6163 792e 6e6c 7028 2257 6869 6c65  spacy.nlp("While
+00007510: 2049 2077 6173 2074 6872 696c 6c65 6420   I was thrilled 
+00007520: 7468 6174 2069 7420 7761 7320 6f6b 2c20  that it was ok, 
+00007530: 4920 776f 7272 6965 6420 7468 6174 2049  I worried that I
+00007540: 2077 6f75 6c64 2066 6169 6c2e 2229 0a09   would fail.")..
+00007550: 7769 7468 2064 6f63 2e72 6574 6f6b 656e  with doc.retoken
+00007560: 697a 6528 2920 6173 2072 6574 6f6b 656e  ize() as retoken
+00007570: 697a 6572 3a0a 0909 666f 7220 7620 696e  izer:...for v in
+00007580: 205b 7420 666f 7220 7420 696e 2064 6f63   [t for t in doc
+00007590: 2069 6620 742e 706f 735f 203d 3d20 2756   if t.pos_ == 'V
+000075a0: 4552 4227 2061 6e64 2074 2e64 6570 5f20  ERB' and t.dep_ 
+000075b0: 3d3d 2027 6363 6f6d 7027 2061 6e64 2074  == 'ccomp' and t
+000075c0: 2e74 6167 5f20 6e6f 7420 696e 2028 2756  .tag_ not in ('V
+000075d0: 424e 2729 205d 203a 2023 206e 6f6e 2d72  BN') ] : # non-r
+000075e0: 6f6f 740a 0909 0974 7279 3a0a 0909 0909  oot....try:.....
+000075f0: 6368 696c 6472 656e 203d 206c 6973 7428  children = list(
+00007600: 762e 7375 6274 7265 6529 0a09 0909 0973  v.subtree).....s
+00007610: 7461 7274 203d 2063 6869 6c64 7265 6e5b  tart = children[
+00007620: 305d 2e69 2020 090a 0909 0909 656e 6420  0].i  ......end 
+00007630: 3d20 6368 696c 6472 656e 5b2d 315d 2e69  = children[-1].i
+00007640: 200a 0909 0909 6174 7472 7320 3d20 7b22   .....attrs = {"
+00007650: 706f 7322 3a20 762e 706f 732c 2022 7461  pos": v.pos, "ta
+00007660: 6722 3a20 762e 7461 672c 2022 6465 7022  g": v.tag, "dep"
+00007670: 3a20 762e 6465 702c 2022 6c65 6d6d 6122  : v.dep, "lemma"
+00007680: 3a76 2e6c 656d 6d61 2c20 2265 6e74 5f74  :v.lemma, "ent_t
+00007690: 7970 6522 3a20 2253 2e22 202b 2076 2e64  ype": "S." + v.d
+000076a0: 6570 5f20 7d20 2320 532e 6164 7663 6c20  ep_ } # S.advcl 
+000076b0: 2c20 2053 2e63 6f6e 6a20 0a09 0909 0972  ,  S.conj .....r
+000076c0: 6574 6f6b 656e 697a 6572 2e6d 6572 6765  etokenizer.merge
+000076d0: 2864 6f63 5b73 7461 7274 203a 2065 6e64  (doc[start : end
+000076e0: 2b31 5d2c 2061 7474 7273 3d61 7474 7273  +1], attrs=attrs
+000076f0: 290a 0909 0965 7863 6570 7420 4578 6365  )....except Exce
+00007700: 7074 696f 6e20 6173 2065 3a0a 0909 0909  ption as e:.....
+00007710: 7072 696e 7420 2820 226d 6572 6765 5f63  print ( "merge_c
+00007720: 636f 6d70 2065 783a 222c 2065 2c20 7620  comp ex:", e, v 
+00007730: 290a 0972 6574 7572 6e20 646f 6320 0a0a  )..return doc ..
+00007740: 6465 6620 6174 7461 6368 5f63 6c28 646f  def attach_cl(do
+00007750: 6329 3a20 2332 3032 332e 312e 3233 0a09  c): #2023.1.23..
+00007760: 666f 7220 7620 696e 205b 7420 666f 7220  for v in [t for 
+00007770: 7420 696e 2064 6f63 2069 6620 742e 706f  t in doc if t.po
+00007780: 735f 203d 3d20 2756 4552 4227 5d20 3a20  s_ == 'VERB'] : 
+00007790: 2320 6e6f 6e2d 726f 6f74 0a09 0974 7279  # non-root...try
+000077a0: 3a0a 0909 0963 6869 6c64 7265 6e20 3d20  :....children = 
+000077b0: 6c69 7374 2876 2e73 7562 7472 6565 290a  list(v.subtree).
+000077c0: 0909 0973 7461 7274 203d 2063 6869 6c64  ...start = child
+000077d0: 7265 6e5b 305d 2e69 2020 090a 0909 0965  ren[0].i  .....e
+000077e0: 6e64 203d 2063 6869 6c64 7265 6e5b 2d31  nd = children[-1
+000077f0: 5d2e 6920 0a09 0909 636c 5f6c 656e 203d  ].i ....cl_len =
+00007800: 2065 6e64 202d 2073 7461 7274 202b 2031   end - start + 1
+00007810: 200a 0909 0964 6f63 5b73 7461 7274 5d2e   ....doc[start].
+00007820: 656e 745f 6964 5f20 3d20 6627 5f43 4c7b  ent_id_ = f'_CL{
+00007830: 762e 6465 705f 7d7b 636c 5f6c 656e 7d27  v.dep_}{cl_len}'
+00007840: 2020 2320 6164 6420 636c 5f72 6f6f 7420    # add cl_root 
+00007850: 3f20 2320 532e 6164 7663 6c20 2c20 2053  ? # S.advcl ,  S
+00007860: 2e63 6f6e 6a20 0a09 0965 7863 6570 7420  .conj ...except 
+00007870: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
+00007880: 0909 0970 7269 6e74 2028 2022 6174 7461  ...print ( "atta
+00007890: 6368 5f63 6c20 6578 3a22 2c20 652c 2076  ch_cl ex:", e, v
+000078a0: 2029 0a09 7265 7475 726e 2064 6f63 200a   )..return doc .
+000078b0: 0a64 6566 2073 6b65 6e70 5f74 6f6b 2874  .def skenp_tok(t
+000078c0: 293a 200a 0966 726f 6d20 6469 632e 6f6e  ): ..from dic.on
+000078d0: 6573 656c 6620 696d 706f 7274 206f 6e65  eself import one
+000078e0: 7365 6c66 200a 0923 7061 6972 203d 2066  self ..#pair = f
+000078f0: 225f 7b74 2e6c 656d 6d61 5f7d 5f4e 505f  "_{t.lemma_}_NP_
+00007900: 7b74 2e64 6570 5f7d 2220 6966 2074 2e65  {t.dep_}" if t.e
+00007910: 6e74 5f74 7970 655f 203d 3d20 274e 5027  nt_type_ == 'NP'
+00007920: 2065 6c73 6520 6622 5f7b 742e 706f 735f   else f"_{t.pos_
+00007930: 7d5f 7b74 2e74 6167 5f7d 5f7b 742e 6465  }_{t.tag_}_{t.de
+00007940: 705f 7d22 2069 6620 742e 706f 735f 2069  p_}" if t.pos_ i
+00007950: 6e20 2827 5052 4f50 4e27 2c27 4e55 4d27  n ('PROPN','NUM'
+00007960: 2c27 5827 2c27 5350 4143 4527 2c27 5055  ,'X','SPACE','PU
+00007970: 4e43 5427 2920 656c 7365 2066 227b 742e  NCT') else f"{t.
+00007980: 7465 7874 2069 6620 742e 7465 7874 2069  text if t.text i
+00007990: 6e20 2827 4927 2920 656c 7365 2074 2e74  n ('I') else t.t
+000079a0: 6578 742e 6c6f 7765 7228 297d 5f7b 742e  ext.lower()}_{t.
+000079b0: 6c65 6d6d 615f 7d5f 7b74 2e70 6f73 5f7d  lemma_}_{t.pos_}
+000079c0: 5f7b 742e 7461 675f 7d7b 6f6e 6573 656c  _{t.tag_}{onesel
+000079d0: 662e 6765 7428 742e 7465 7874 2e6c 6f77  f.get(t.text.low
+000079e0: 6572 2829 2c20 2727 297d 5f7b 742e 6465  er(), '')}_{t.de
+000079f0: 705f 7d22 0a09 7061 6972 203d 2066 225f  p_}"..pair = f"_
+00007a00: 7b74 2e6c 656d 6d61 5f7d 5f7b 742e 706f  {t.lemma_}_{t.po
+00007a10: 735f 7d5f 4e50 5f7b 742e 6465 705f 7d7b  s_}_NP_{t.dep_}{
+00007a20: 742e 6865 6164 2e69 7d22 2069 6620 2874  t.head.i}" if (t
+00007a30: 2e65 6e74 5f74 7970 655f 203d 3d20 274e  .ent_type_ == 'N
+00007a40: 5027 2061 6e64 2074 2e6c 656d 6d61 5f20  P' and t.lemma_ 
+00007a50: 6e6f 7420 696e 2028 2774 6861 7427 2c27  not in ('that','
+00007a60: 7768 6963 6827 2929 2065 6c73 6520 6622  which')) else f"
+00007a70: 5f7b 742e 706f 735f 7d5f 7b74 2e74 6167  _{t.pos_}_{t.tag
+00007a80: 5f7d 5f7b 742e 6465 705f 7d7b 742e 6865  _}_{t.dep_}{t.he
+00007a90: 6164 2e69 7d22 2069 6620 742e 706f 735f  ad.i}" if t.pos_
+00007aa0: 2069 6e20 2827 5052 4f50 4e27 2c27 4e55   in ('PROPN','NU
+00007ab0: 4d27 2c27 5827 2c27 5350 4143 4527 2c27  M','X','SPACE','
+00007ac0: 5055 4e43 5427 2920 656c 7365 2066 227b  PUNCT') else f"{
+00007ad0: 742e 7465 7874 2069 6620 742e 7465 7874  t.text if t.text
+00007ae0: 2069 6e20 2827 4927 2920 656c 7365 2074   in ('I') else t
+00007af0: 2e74 6578 742e 6c6f 7765 7228 297d 5f7b  .text.lower()}_{
+00007b00: 742e 6c65 6d6d 615f 7d5f 7b74 2e70 6f73  t.lemma_}_{t.pos
+00007b10: 5f7d 5f7b 742e 7461 675f 7d7b 6f6e 6573  _}_{t.tag_}{ones
+00007b20: 656c 662e 6765 7428 742e 7465 7874 2e6c  elf.get(t.text.l
+00007b30: 6f77 6572 2829 2c20 2727 297d 5f7b 742e  ower(), '')}_{t.
+00007b40: 6465 705f 7d7b 742e 6865 6164 2e69 7d22  dep_}{t.head.i}"
+00007b50: 0a09 6966 2074 2e65 6e74 5f69 645f 2e73  ..if t.ent_id_.s
+00007b60: 7461 7274 7377 6974 6828 225f 434c 2229  tartswith("_CL")
+00007b70: 2061 6e64 206e 6f74 2027 524f 4f54 2720   and not 'ROOT' 
+00007b80: 696e 2074 2e65 6e74 5f69 645f 3a20 7061  in t.ent_id_: pa
+00007b90: 6972 203d 2070 6169 7220 2b20 742e 656e  ir = pair + t.en
+00007ba0: 745f 6964 5f0a 0972 6574 7572 6e20 7061  t_id_..return pa
+00007bb0: 6972 200a 0a64 6566 2065 735f 736b 656e  ir ..def es_sken
+00007bc0: 7028 646f 6329 3a0a 0923 6d65 7267 655f  p(doc):..#merge_
+00007bd0: 6363 6f6d 7028 646f 6329 2023 206d 6572  ccomp(doc) # mer
+00007be0: 6765 5f6c 6561 7665 5f63 6c28 646f 6329  ge_leave_cl(doc)
+00007bf0: 200a 096d 6572 6765 5f6e 7028 646f 6329   ..merge_np(doc)
+00007c00: 200a 0961 7474 6163 685f 636c 2864 6f63   ..attach_cl(doc
+00007c10: 290a 0972 6574 7572 6e20 225f 5e20 2220  )..return "_^ " 
+00007c20: 2b20 2720 272e 6a6f 696e 285b 2073 6b65  + ' '.join([ ske
+00007c30: 6e70 5f74 6f6b 2874 2920 666f 7220 7420  np_tok(t) for t 
+00007c40: 696e 2064 6f63 5d29 200a 0a40 4c61 6e67  in doc]) ..@Lang
+00007c50: 7561 6765 2e63 6f6d 706f 6e65 6e74 2822  uage.component("
+00007c60: 6d65 7267 655f 7072 7422 290a 6465 6620  merge_prt").def 
+00007c70: 6d65 7267 655f 7072 7428 646f 6329 3a20  merge_prt(doc): 
+00007c80: 0a09 2727 2749 2074 7572 6e20 6f66 6620  ..'''I turn off 
+00007c90: 7468 6520 7261 6469 6f2e 203d 3e20 7475  the radio. => tu
+00007ca0: 726e 5f6f 6666 202c 2061 6464 6564 2032  rn_off , added 2
+00007cb0: 3032 332e 312e 3133 2727 270a 0969 6620  023.1.13'''..if 
+00007cc0: 6e6f 7420 6861 7361 7474 7228 6d65 7267  not hasattr(merg
+00007cd0: 655f 7072 742c 2027 6d61 7463 6865 7227  e_prt, 'matcher'
+00007ce0: 293a 0a09 096d 6572 6765 5f70 7274 2e6d  ):...merge_prt.m
+00007cf0: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
+00007d00: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
+00007d10: 290a 0909 6d65 7267 655f 7072 742e 6d61  )...merge_prt.ma
+00007d20: 7463 6865 722e 6164 6428 2270 7274 222c  tcher.add("prt",
+00007d30: 205b 5b7b 2250 4f53 223a 2256 4552 4222   [[{"POS":"VERB"
+00007d40: 7d2c 207b 2250 4f53 223a 2241 4450 222c  }, {"POS":"ADP",
+00007d50: 2022 4445 5022 3a22 7072 7422 7d5d 5d2c   "DEP":"prt"}]],
+00007d60: 2067 7265 6564 7920 3d27 4c4f 4e47 4553   greedy ='LONGES
+00007d70: 5427 290a 0977 6974 6820 646f 632e 7265  T')..with doc.re
+00007d80: 746f 6b65 6e69 7a65 2829 2061 7320 7265  tokenize() as re
+00007d90: 746f 6b65 6e69 7a65 723a 0a09 0966 6f72  tokenizer:...for
+00007da0: 206e 616d 652c 2073 7461 7274 2c20 656e   name, start, en
+00007db0: 6420 696e 206d 6572 6765 5f70 7274 2e6d  d in merge_prt.m
+00007dc0: 6174 6368 6572 2864 6f63 293a 0a09 0909  atcher(doc):....
+00007dd0: 7472 793a 0a09 0909 0961 7474 7273 203d  try:.....attrs =
+00007de0: 207b 2270 6f73 223a 2064 6f63 5b73 7461   {"pos": doc[sta
+00007df0: 7274 5d2e 706f 732c 2022 7461 6722 3a20  rt].pos, "tag": 
+00007e00: 646f 635b 7374 6172 745d 2e74 6167 2c20  doc[start].tag, 
+00007e10: 2264 6570 223a 2064 6f63 5b73 7461 7274  "dep": doc[start
+00007e20: 5d2e 6465 702c 2022 6c65 6d6d 6122 3a64  ].dep, "lemma":d
+00007e30: 6f63 5b73 7461 7274 5d2e 6c65 6d6d 615f  oc[start].lemma_
+00007e40: 202b 2022 5f22 202b 2064 6f63 5b73 7461   + "_" + doc[sta
+00007e50: 7274 2b31 5d2e 6c65 6d6d 615f 2c20 2265  rt+1].lemma_, "e
+00007e60: 6e74 5f74 7970 6522 3a20 2276 7072 7422  nt_type": "vprt"
+00007e70: 7d0a 0909 0909 7265 746f 6b65 6e69 7a65  }.....retokenize
+00007e80: 722e 6d65 7267 6528 646f 635b 7374 6172  r.merge(doc[star
+00007e90: 7420 3a20 656e 645d 2c20 6174 7472 733d  t : end], attrs=
+00007ea0: 6174 7472 7329 0a09 0909 6578 6365 7074  attrs)....except
+00007eb0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00007ec0: 0a09 0909 0970 7269 6e74 2028 2022 6d65  .....print ( "me
+00007ed0: 7267 655f 7072 7420 6578 3a22 2c20 6520  rge_prt ex:", e 
+00007ee0: 2c20 7374 6172 742c 2065 6e64 290a 0972  , start, end)..r
+00007ef0: 6574 7572 6e20 646f 630a 0a40 4c61 6e67  eturn doc..@Lang
+00007f00: 7561 6765 2e63 6f6d 706f 6e65 6e74 2822  uage.component("
+00007f10: 6d65 7267 655f 7622 290a 6465 6620 6d65  merge_v").def me
+00007f20: 7267 655f 7628 646f 6329 3a20 2320 3230  rge_v(doc): # 20
+00007f30: 3233 2e31 2e32 320a 0969 6620 6e6f 7420  23.1.22..if not 
+00007f40: 6861 7361 7474 7228 6d65 7267 655f 762c  hasattr(merge_v,
+00007f50: 2027 6d61 7463 6865 7227 293a 0a09 096d   'matcher'):...m
+00007f60: 6572 6765 5f76 2e6d 6174 6368 6572 203d  erge_v.matcher =
+00007f70: 204d 6174 6368 6572 2873 7061 6379 2e6e   Matcher(spacy.n
+00007f80: 6c70 2e76 6f63 6162 290a 0909 6d65 7267  lp.vocab)...merg
+00007f90: 655f 762e 6d61 7463 6865 722e 6164 6428  e_v.matcher.add(
+00007fa0: 2276 7072 7422 2c20 5b5b 7b22 504f 5322  "vprt", [[{"POS"
+00007fb0: 3a22 5645 5242 227d 2c20 7b22 504f 5322  :"VERB"}, {"POS"
+00007fc0: 3a22 4144 5022 2c20 2244 4550 223a 2270  :"ADP", "DEP":"p
+00007fd0: 7274 227d 5d5d 2c20 6772 6565 6479 203d  rt"}]], greedy =
+00007fe0: 274c 4f4e 4745 5354 2729 0a09 0923 6d65  'LONGEST')...#me
+00007ff0: 7267 655f 762e 6d61 7463 6865 722e 6164  rge_v.matcher.ad
+00008000: 6428 2276 746f 7622 2c20 5b5b 7b22 504f  d("vtov", [[{"PO
+00008010: 5322 3a22 5645 5242 227d 2c7b 224c 454d  S":"VERB"},{"LEM
+00008020: 4d41 223a 2274 6f22 2c20 2254 4147 223a  MA":"to", "TAG":
+00008030: 2254 4f22 7d2c 207b 2254 4147 223a 2256  "TO"}, {"TAG":"V
+00008040: 4222 7d5d 5d2c 2067 7265 6564 7920 3d27  B"}]], greedy ='
+00008050: 4c4f 4e47 4553 5427 2920 2020 2020 2023  LONGEST')      #
+00008060: 2070 6c61 6e20 746f 2074 7572 6e20 6f66   plan to turn of
+00008070: 6620 7468 6520 7261 6469 6f20 0a09 0923  f the radio ...#
+00008080: 6d65 7267 655f 762e 6d61 7463 6865 722e  merge_v.matcher.
+00008090: 6164 6428 2276 7662 6722 2c20 5b5b 7b22  add("vvbg", [[{"
+000080a0: 504f 5322 3a22 5645 5242 227d 2c7b 2244  POS":"VERB"},{"D
+000080b0: 4550 223a 2278 636f 6d70 222c 2254 4147  EP":"xcomp","TAG
+000080c0: 223a 2256 4247 227d 5d5d 2c20 6772 6565  ":"VBG"}]], gree
+000080d0: 6479 203d 274c 4f4e 4745 5354 2729 2020  dy ='LONGEST')  
+000080e0: 2020 2020 2020 2020 2020 2020 2020 0a09                ..
+000080f0: 096d 6572 6765 5f76 2e6d 6174 6368 6572  .merge_v.matcher
+00008100: 2e61 6464 2822 6265 2d70 6e22 2c20 5b5b  .add("be-pn", [[
+00008110: 7b22 4c45 4d4d 4122 3a22 6265 227d 2c7b  {"LEMMA":"be"},{
+00008120: 2254 4147 223a 2249 4e22 2c22 504f 5322  "TAG":"IN","POS"
+00008130: 3a22 4144 5022 7d2c 7b22 5441 4722 3a22  :"ADP"},{"TAG":"
+00008140: 4e4e 227d 5d5d 2c20 6772 6565 6479 203d  NN"}]], greedy =
+00008150: 274c 4f4e 4745 5354 2729 2023 2062 6520  'LONGEST') # be 
+00008160: 696e 2063 6f6e 7374 7275 6374 696f 6e0a  in construction.
+00008170: 0909 6d65 7267 655f 762e 6d61 7463 6865  ..merge_v.matche
+00008180: 722e 6164 6428 2262 652d 6163 6f6d 7022  r.add("be-acomp"
+00008190: 2c20 5b5b 7b22 4c45 4d4d 4122 3a22 6265  , [[{"LEMMA":"be
+000081a0: 227d 2c7b 2244 4550 223a 2261 636f 6d70  "},{"DEP":"acomp
+000081b0: 222c 2250 4f53 223a 2241 444a 227d 5d5d  ","POS":"ADJ"}]]
+000081c0: 2c20 6772 6565 6479 203d 274c 4f4e 4745  , greedy ='LONGE
+000081d0: 5354 2729 2023 2250 4f53 223a 2241 5558  ST') #"POS":"AUX
+000081e0: 222c 0a09 096d 6572 6765 5f76 2e6d 6174  ",...merge_v.mat
+000081f0: 6368 6572 2e61 6464 2822 6265 2d61 7578  cher.add("be-aux
+00008200: 7061 7373 222c 205b 5b7b 224c 454d 4d41  pass", [[{"LEMMA
+00008210: 223a 2262 6522 2c22 4445 5022 3a22 6175  ":"be","DEP":"au
+00008220: 7870 6173 7322 7d2c 7b22 5441 4722 3a22  xpass"},{"TAG":"
+00008230: 5642 4e22 2c22 504f 5322 3a22 5645 5242  VBN","POS":"VERB
+00008240: 227d 5d5d 2c20 6772 6565 6479 203d 274c  "}]], greedy ='L
+00008250: 4f4e 4745 5354 2729 0a09 7769 7468 2064  ONGEST')..with d
+00008260: 6f63 2e72 6574 6f6b 656e 697a 6528 2920  oc.retokenize() 
+00008270: 6173 2072 6574 6f6b 656e 697a 6572 3a0a  as retokenizer:.
+00008280: 0909 666f 7220 6e61 6d65 2c20 7374 6172  ..for name, star
+00008290: 742c 2065 6e64 2069 6e20 6d65 7267 655f  t, end in merge_
+000082a0: 762e 6d61 7463 6865 7228 646f 6329 3a0a  v.matcher(doc):.
+000082b0: 0909 0974 7279 3a20 0a09 0909 0961 7474  ...try: .....att
+000082c0: 7273 203d 207b 2270 6f73 223a 2022 5645  rs = {"pos": "VE
+000082d0: 5242 222c 2022 7461 6722 3a20 646f 635b  RB", "tag": doc[
+000082e0: 7374 6172 745d 2e74 6167 2c20 2264 6570  start].tag, "dep
+000082f0: 223a 2064 6f63 5b73 7461 7274 5d2e 6465  ": doc[start].de
+00008300: 702c 200a 0909 0909 0922 6c65 6d6d 6122  p, ......"lemma"
+00008310: 3a22 5f22 2e6a 6f69 6e28 5b64 6f63 5b69  :"_".join([doc[i
+00008320: 5d2e 6c65 6d6d 615f 2069 6620 6920 3d3d  ].lemma_ if i ==
+00008330: 2073 7461 7274 2065 6c73 6520 646f 635b   start else doc[
+00008340: 695d 2e74 6578 7420 666f 7220 6920 696e  i].text for i in
+00008350: 2072 616e 6765 2873 7461 7274 2c65 6e64   range(start,end
+00008360: 295d 292c 200a 0909 0909 0922 656e 745f  )]), ......"ent_
+00008370: 7479 7065 223a 2022 6d65 7267 655f 763a  type": "merge_v:
+00008380: 2220 2b20 7370 6163 792e 6e6c 702e 766f  " + spacy.nlp.vo
+00008390: 6361 625b 6e61 6d65 5d2e 7465 7874 202b  cab[name].text +
+000083a0: 2066 227c 7b64 6f63 5b73 7461 7274 5d2e   f"|{doc[start].
+000083b0: 6c65 6d6d 615f 7d3a 7b64 6f63 5b73 7461  lemma_}:{doc[sta
+000083c0: 7274 5d2e 706f 735f 7d3a 7b64 6f63 5b73  rt].pos_}:{doc[s
+000083d0: 7461 7274 2b31 5d2e 6465 705f 7d3a 7b64  tart+1].dep_}:{d
+000083e0: 6f63 5b73 7461 7274 2b31 5d2e 706f 735f  oc[start+1].pos_
+000083f0: 7d3a 7b64 6f63 5b73 7461 7274 2b31 5d2e  }:{doc[start+1].
+00008400: 6c65 6d6d 615f 7d22 207d 0a09 0909 0972  lemma_}" }.....r
+00008410: 6574 6f6b 656e 697a 6572 2e6d 6572 6765  etokenizer.merge
+00008420: 2864 6f63 5b73 7461 7274 203a 2065 6e64  (doc[start : end
+00008430: 5d2c 2061 7474 7273 3d61 7474 7273 290a  ], attrs=attrs).
+00008440: 0909 0965 7863 6570 7420 4578 6365 7074  ...except Except
+00008450: 696f 6e20 6173 2065 3a0a 0909 0909 7072  ion as e:.....pr
+00008460: 696e 7420 2820 226d 6572 6765 5f76 2065  int ( "merge_v e
+00008470: 783a 222c 2065 202c 2073 7461 7274 2c20  x:", e , start, 
+00008480: 656e 6429 0a09 7265 7475 726e 2064 6f63  end)..return doc
+00008490: 0a0a 404c 616e 6775 6167 652e 636f 6d70  ..@Language.comp
+000084a0: 6f6e 656e 7428 226d 6572 6765 5f74 7270  onent("merge_trp
+000084b0: 2229 0a64 6566 206d 6572 6765 5f74 7270  ").def merge_trp
+000084c0: 2864 6f63 293a 2023 2032 3032 332e 312e  (doc): # 2023.1.
+000084d0: 3234 2c20 7c74 776f 2077 6f72 6473 2c20  24, |two words, 
+000084e0: 7468 6520 7365 636f 6e64 206f 6e65 2069  the second one i
+000084f0: 7320 7468 6520 6865 6164 200a 0969 6620  s the head ..if 
+00008500: 6e6f 7420 6861 7361 7474 7228 6d65 7267  not hasattr(merg
+00008510: 655f 7472 702c 2027 6d61 7463 6865 7227  e_trp, 'matcher'
+00008520: 293a 0a09 096d 6572 6765 5f74 7270 2e6d  ):...merge_trp.m
+00008530: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
+00008540: 2873 7061 6379 2e6e 6c70 2e76 6f63 6162  (spacy.nlp.vocab
+00008550: 290a 0909 6d65 7267 655f 7472 702e 6d61  )...merge_trp.ma
+00008560: 7463 6865 722e 6164 6428 2261 6d6f 6422  tcher.add("amod"
+00008570: 2c20 5b5b 7b22 504f 5322 3a22 4144 4a22  , [[{"POS":"ADJ"
+00008580: 2c20 2244 4550 223a 2261 6d6f 6422 7d2c  , "DEP":"amod"},
+00008590: 207b 2250 4f53 223a 224e 4f55 4e22 7d5d   {"POS":"NOUN"}]
+000085a0: 5d29 0a09 096d 6572 6765 5f74 7270 2e6d  ])...merge_trp.m
+000085b0: 6174 6368 6572 2e61 6464 2822 6465 7422  atcher.add("det"
+000085c0: 2c20 5b5b 7b22 504f 5322 3a22 4445 5422  , [[{"POS":"DET"
+000085d0: 2c20 2244 4550 223a 2264 6574 227d 2c20  , "DEP":"det"}, 
+000085e0: 7b22 504f 5322 3a22 4e4f 554e 227d 5d5d  {"POS":"NOUN"}]]
+000085f0: 290a 0909 6d65 7267 655f 7472 702e 6d61  )...merge_trp.ma
+00008600: 7463 6865 722e 6164 6428 2261 6476 6d6f  tcher.add("advmo
+00008610: 6422 2c20 5b5b 7b22 504f 5322 3a22 4144  d", [[{"POS":"AD
+00008620: 5622 2c20 2244 4550 223a 2261 6476 6d6f  V", "DEP":"advmo
+00008630: 6422 7d2c 207b 2250 4f53 223a 207b 2249  d"}, {"POS": {"I
+00008640: 4e22 3a20 5b22 5645 5242 222c 2022 4144  N": ["VERB", "AD
+00008650: 4a22 5d7d 7d20 5d5d 290a 0909 0a09 7769  J"]}} ]]).....wi
+00008660: 7468 2064 6f63 2e72 6574 6f6b 656e 697a  th doc.retokeniz
+00008670: 6528 2920 6173 2072 6574 6f6b 656e 697a  e() as retokeniz
+00008680: 6572 3a0a 0909 666f 7220 6e61 6d65 2c20  er:...for name, 
+00008690: 7374 6172 742c 2065 6e64 2069 6e20 6d65  start, end in me
+000086a0: 7267 655f 7472 702e 6d61 7463 6865 7228  rge_trp.matcher(
+000086b0: 646f 6329 3a0a 0909 0974 7279 3a20 0a09  doc):....try: ..
+000086c0: 0909 0961 7474 7273 203d 207b 2270 6f73  ...attrs = {"pos
+000086d0: 223a 2064 6f63 5b73 7461 7274 2b31 5d2e  ": doc[start+1].
+000086e0: 706f 732c 2022 7461 6722 3a20 646f 635b  pos, "tag": doc[
+000086f0: 7374 6172 742b 315d 2e74 6167 2c20 2264  start+1].tag, "d
+00008700: 6570 223a 2064 6f63 5b73 7461 7274 2b31  ep": doc[start+1
+00008710: 5d2e 6465 702c 200a 0909 0909 0922 6c65  ].dep, ......"le
+00008720: 6d6d 6122 3a64 6f63 5b73 7461 7274 2b31  mma":doc[start+1
+00008730: 5d2e 6c65 6d6d 612c 200a 0909 0909 0922  ].lemma, ......"
+00008740: 656e 745f 7479 7065 223a 2022 6d65 7267  ent_type": "merg
+00008750: 655f 7472 703a 2220 2b20 7370 6163 792e  e_trp:" + spacy.
+00008760: 6e6c 702e 766f 6361 625b 6e61 6d65 5d2e  nlp.vocab[name].
+00008770: 7465 7874 202b 2066 223a 7b64 6f63 5b73  text + f":{doc[s
+00008780: 7461 7274 5d2e 7461 675f 7d20 7b64 6f63  tart].tag_} {doc
+00008790: 5b73 7461 7274 2b31 5d2e 7461 675f 7d22  [start+1].tag_}"
+000087a0: 207d 0a09 0909 0972 6574 6f6b 656e 697a   }.....retokeniz
+000087b0: 6572 2e6d 6572 6765 2864 6f63 5b73 7461  er.merge(doc[sta
+000087c0: 7274 203a 2065 6e64 5d2c 2061 7474 7273  rt : end], attrs
+000087d0: 3d61 7474 7273 290a 0909 0965 7863 6570  =attrs)....excep
+000087e0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+000087f0: 3a0a 0909 0909 7072 696e 7420 2820 226d  :.....print ( "m
+00008800: 6572 6765 5f74 7270 2065 783a 222c 2065  erge_trp ex:", e
+00008810: 202c 2073 7461 7274 2c20 656e 6429 0a09   , start, end)..
+00008820: 7265 7475 726e 2064 6f63 0a0a 6465 6620  return doc..def 
+00008830: 736b 6528 646f 632c 206e 616d 653a 7374  ske(doc, name:st
+00008840: 723d 2773 6d27 293a 2023 2061 6464 6564  r='sm'): # added
+00008850: 2032 3032 332e 312e 3235 0a09 6966 206e   2023.1.25..if n
+00008860: 6f74 2068 6173 6174 7472 2873 6b65 2c20  ot hasattr(ske, 
+00008870: 276e 6c70 2729 3a0a 0909 736b 652e 6e6c  'nlp'):...ske.nl
+00008880: 7020 3d20 7370 6163 792e 6c6f 6164 2866  p = spacy.load(f
+00008890: 2765 6e5f 636f 7265 5f77 6562 5f7b 6e61  'en_core_web_{na
+000088a0: 6d65 7d27 290a 0909 5b20 736b 652e 6e6c  me}')...[ ske.nl
+000088b0: 702e 6164 645f 7069 7065 2870 2920 666f  p.add_pipe(p) fo
+000088c0: 7220 7020 696e 2028 226d 6572 6765 5f65  r p in ("merge_e
+000088d0: 6e74 6974 6965 7322 2c20 226d 6572 6765  ntities", "merge
+000088e0: 5f6e 7022 2c20 226d 6572 6765 5f70 7274  _np", "merge_prt
+000088f0: 222c 2022 6d65 7267 655f 7472 7022 2c20  ", "merge_trp", 
+00008900: 2273 7061 6e5f 636c 6175 7365 2229 205d  "span_clause") ]
+00008910: 0a09 7265 7475 726e 2073 6b65 2e6e 6c70  ..return ske.nlp
+00008920: 2864 6f63 2920 0a23 7072 696e 7428 2073  (doc) .#print( s
+00008930: 6b65 2822 5468 6520 7175 6963 6b20 666f  ke("The quick fo
+00008940: 7820 6a75 6d70 6564 206f 7665 7220 7468  x jumped over th
+00008950: 6520 6c61 7a79 2064 6f67 2e22 295b 305d  e lazy dog.")[0]
+00008960: 2029 0a0a 6465 6620 6d65 7267 655f 7370   )..def merge_sp
+00008970: 616e 2864 6f63 2c20 7061 743a 6c69 7374  an(doc, pat:list
+00008980: 3d5b 7b22 504f 5322 3a22 5645 5242 227d  =[{"POS":"VERB"}
+00008990: 2c7b 224c 454d 4d41 223a 2274 6f22 7d2c  ,{"LEMMA":"to"},
+000089a0: 7b22 5441 4722 3a22 5642 227d 5d29 3a20  {"TAG":"VB"}]): 
+000089b0: 0a09 2727 2720 6465 6369 6465 2074 6f20  ..''' decide to 
+000089c0: 7361 7665 203d 3e20 6f6e 652c 2032 3032  save => one, 202
+000089d0: 332e 312e 3233 2027 2727 200a 0973 7061  3.1.23 ''' ..spa
+000089e0: 7420 3d20 6a73 6f6e 2e64 756d 7073 2870  t = json.dumps(p
+000089f0: 6174 2920 0a09 6966 206e 6f74 2068 6173  at) ..if not has
+00008a00: 6174 7472 286d 6572 6765 5f73 7061 6e2c  attr(merge_span,
+00008a10: 2073 7061 7429 3a0a 0909 5f6d 6174 6368   spat):..._match
+00008a20: 6572 203d 204d 6174 6368 6572 2873 7061  er = Matcher(spa
+00008a30: 6379 2e6e 6c70 2e76 6f63 6162 290a 0909  cy.nlp.vocab)...
+00008a40: 5f6d 6174 6368 6572 2e61 6464 2873 7061  _matcher.add(spa
+00008a50: 742c 205b 7061 745d 2c20 6772 6565 6479  t, [pat], greedy
+00008a60: 203d 274c 4f4e 4745 5354 2729 0a09 0973   ='LONGEST')...s
+00008a70: 6574 6174 7472 286d 6572 6765 5f73 7061  etattr(merge_spa
+00008a80: 6e2c 2073 7061 742c 205f 6d61 7463 6865  n, spat, _matche
+00008a90: 7229 200a 0977 6974 6820 646f 632e 7265  r) ..with doc.re
+00008aa0: 746f 6b65 6e69 7a65 2829 2061 7320 7265  tokenize() as re
+00008ab0: 746f 6b65 6e69 7a65 723a 0a09 0966 6f72  tokenizer:...for
+00008ac0: 206e 616d 652c 2073 7461 7274 2c20 656e   name, start, en
+00008ad0: 6420 696e 2067 6574 6174 7472 286d 6572  d in getattr(mer
+00008ae0: 6765 5f73 7061 6e2c 2073 7061 7429 2864  ge_span, spat)(d
+00008af0: 6f63 293a 0a09 0909 7472 793a 200a 0909  oc):....try: ...
+00008b00: 0909 6174 7472 7320 3d20 7b22 706f 7322  ..attrs = {"pos"
+00008b10: 3a20 646f 635b 7374 6172 745d 2e70 6f73  : doc[start].pos
+00008b20: 2c20 2274 6167 223a 2064 6f63 5b73 7461  , "tag": doc[sta
+00008b30: 7274 5d2e 7461 672c 2022 6465 7022 3a20  rt].tag, "dep": 
+00008b40: 646f 635b 7374 6172 745d 2e64 6570 2c20  doc[start].dep, 
+00008b50: 0a09 0909 0909 226c 656d 6d61 223a 225f  ......"lemma":"_
+00008b60: 222e 6a6f 696e 285b 646f 635b 695d 2e6c  ".join([doc[i].l
+00008b70: 656d 6d61 5f20 6966 2069 203d 3d20 7374  emma_ if i == st
+00008b80: 6172 7420 656c 7365 2064 6f63 5b69 5d2e  art else doc[i].
+00008b90: 7465 7874 2066 6f72 2069 2069 6e20 7261  text for i in ra
+00008ba0: 6e67 6528 7374 6172 742c 656e 6429 5d29  nge(start,end)])
+00008bb0: 2c20 0a09 0909 0909 2265 6e74 5f74 7970  , ......"ent_typ
+00008bc0: 6522 3a20 226d 6572 6765 5f73 7061 6e3a  e": "merge_span:
+00008bd0: 2220 2b20 7370 6174 207d 0a09 0909 0972  " + spat }.....r
+00008be0: 6574 6f6b 656e 697a 6572 2e6d 6572 6765  etokenizer.merge
+00008bf0: 2864 6f63 5b73 7461 7274 203a 2065 6e64  (doc[start : end
+00008c00: 5d2c 2061 7474 7273 3d61 7474 7273 290a  ], attrs=attrs).
+00008c10: 0909 0965 7863 6570 7420 4578 6365 7074  ...except Except
+00008c20: 696f 6e20 6173 2065 3a0a 0909 0909 7072  ion as e:.....pr
+00008c30: 696e 7420 2820 226d 6572 6765 5f76 2065  int ( "merge_v e
+00008c40: 783a 222c 2065 202c 2073 7461 7274 2c20  x:", e , start, 
+00008c50: 656e 6429 0a09 7265 7475 726e 2064 6f63  end)..return doc
+00008c60: 0a0a 6465 6620 6465 706d 6174 6368 2829  ..def depmatch()
+00008c70: 3a20 2366 726f 6d20 7370 6163 792e 6d61  : #from spacy.ma
+00008c80: 7463 6865 7220 696d 706f 7274 204d 6174  tcher import Mat
+00008c90: 6368 6572 2c44 6570 656e 6465 6e63 794d  cher,DependencyM
+00008ca0: 6174 6368 6572 0a09 2727 2720 3230 3233  atcher..''' 2023
+00008cb0: 2e31 2e36 2027 2727 0a09 6966 206e 6f74  .1.6 '''..if not
+00008cc0: 2068 6173 6174 7472 2864 6570 6d61 7463   hasattr(depmatc
+00008cd0: 682c 276d 6174 6368 6572 2729 3a20 0a09  h,'matcher'): ..
+00008ce0: 0964 6570 6d61 7463 682e 6d61 7463 6865  .depmatch.matche
+00008cf0: 7220 3d20 4465 7065 6e64 656e 6379 4d61  r = DependencyMa
+00008d00: 7463 6865 7228 7370 6163 792e 6e6c 702e  tcher(spacy.nlp.
+00008d10: 766f 6361 6229 0a09 0970 6174 7465 726e  vocab)...pattern
+00008d20: 203d 207b 0a09 0909 2320 6164 7663 6c2d   = {....# advcl-
+00008d30: 6163 6f6d 7020 776f 7272 7920 6265 2074  acomp worry be t
+00008d40: 6872 696c 6c65 6420 7c20 2257 6869 6c65  hrilled | "While
+00008d50: 2049 2077 6173 2074 6872 696c 6c65 6420   I was thrilled 
+00008d60: 7468 6174 2069 7420 7761 7320 6f6b 2c20  that it was ok, 
+00008d70: 4920 776f 7272 6965 6420 7468 6174 2073  I worried that s
+00008d80: 6865 2069 7320 6861 7070 792e 220a 0909  he is happy."...
+00008d90: 0922 6164 7663 6c2d 6163 6f6d 7022 3a20  ."advcl-acomp": 
+00008da0: 5b20 7b22 5249 4748 545f 4944 223a 2022  [ {"RIGHT_ID": "
+00008db0: 7622 2c20 2252 4947 4854 5f41 5454 5253  v", "RIGHT_ATTRS
+00008dc0: 223a 207b 2250 4f53 223a 2022 5645 5242  ": {"POS": "VERB
+00008dd0: 227d 7d2c 2020 7b20 224c 4546 545f 4944  "}},  { "LEFT_ID
+00008de0: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
+00008df0: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
+00008e00: 223a 2022 6164 7663 6c22 2c20 2252 4947  ": "advcl", "RIG
+00008e10: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
+00008e20: 223a 2022 6164 7663 6c22 7d20 7d2c 207b  ": "advcl"} }, {
+00008e30: 2022 4c45 4654 5f49 4422 3a20 2261 6476   "LEFT_ID": "adv
+00008e40: 636c 222c 2022 5245 4c5f 4f50 223a 2022  cl", "REL_OP": "
+00008e50: 3e22 2c22 5249 4748 545f 4944 223a 2022  >","RIGHT_ID": "
+00008e60: 6f62 6a65 6374 222c 2022 5249 4748 545f  object", "RIGHT_
+00008e70: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
+00008e80: 2261 636f 6d70 227d 207d 5d20 2c20 0a09  "acomp"} }] , ..
+00008e90: 0909 2320 5368 6520 6973 2068 6170 7079  ..# She is happy
+00008ea0: 2e20 7c20 6e73 7562 6a2d 6163 6f6d 7020  . | nsubj-acomp 
+00008eb0: 6265 2073 6865 2068 6170 7079 0a09 0909  be she happy....
+00008ec0: 226e 7375 626a 2d61 636f 6d70 223a 205b  "nsubj-acomp": [
+00008ed0: 207b 2022 5249 4748 545f 4944 223a 2022   { "RIGHT_ID": "
+00008ee0: 7622 2c20 2020 2252 4947 4854 5f41 5454  v",   "RIGHT_ATT
+00008ef0: 5253 223a 207b 224c 454d 4d41 223a 2022  RS": {"LEMMA": "
+00008f00: 6265 227d 7d2c 7b20 224c 4546 545f 4944  be"}},{ "LEFT_ID
+00008f10: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
+00008f20: 3a22 3e22 2c20 2252 4947 4854 5f49 4422  :">", "RIGHT_ID"
+00008f30: 3a20 2273 7562 6a65 6374 222c 2022 5249  : "subject", "RI
+00008f40: 4748 545f 4154 5452 5322 3a20 7b22 4445  GHT_ATTRS": {"DE
+00008f50: 5022 3a20 226e 7375 626a 227d 207d 2c20  P": "nsubj"} }, 
+00008f60: 7b20 2022 4c45 4654 5f49 4422 3a20 2276  {  "LEFT_ID": "v
+00008f70: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
+00008f80: 2c20 2022 5249 4748 545f 4944 223a 2022  ,  "RIGHT_ID": "
+00008f90: 6f62 6a65 6374 222c 2020 2020 2252 4947  object",    "RIG
+00008fa0: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
+00008fb0: 223a 2022 6163 6f6d 7022 7d7d 5d2c 200a  ": "acomp"}}], .
+00008fc0: 0909 0923 5368 6520 6973 2020 6120 6769  ...#She is  a gi
+00008fd0: 726c 2e20 7c20 6e73 7562 6a2d 6174 7472  rl. | nsubj-attr
+00008fe0: 2062 6520 7368 6520 6769 726c 0a09 0909   be she girl....
+00008ff0: 226e 7375 626a 2d61 7474 7222 3a20 5b20  "nsubj-attr": [ 
+00009000: 207b 2252 4947 4854 5f49 4422 3a20 2276   {"RIGHT_ID": "v
+00009010: 222c 2022 5249 4748 545f 4154 5452 5322  ", "RIGHT_ATTRS"
+00009020: 3a20 7b22 4c45 4d4d 4122 3a20 2262 6522  : {"LEMMA": "be"
+00009030: 7d7d 2c20 7b20 224c 4546 545f 4944 223a  }}, { "LEFT_ID":
+00009040: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
+00009050: 223e 222c 2252 4947 4854 5f49 4422 3a20  ">","RIGHT_ID": 
+00009060: 2273 7562 6a65 6374 222c 2022 5249 4748  "subject", "RIGH
+00009070: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
+00009080: 3a20 226e 7375 626a 227d 207d 2c20 7b20  : "nsubj"} }, { 
+00009090: 2020 2022 4c45 4654 5f49 4422 3a20 2276     "LEFT_ID": "v
+000090a0: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
+000090b0: 2c20 2252 4947 4854 5f49 4422 3a20 226f  , "RIGHT_ID": "o
+000090c0: 626a 6563 7422 2c20 2252 4947 4854 5f41  bject", "RIGHT_A
+000090d0: 5454 5253 223a 207b 2244 4550 223a 2022  TTRS": {"DEP": "
+000090e0: 6174 7472 227d 207d 5d2c 0a09 0909 2320  attr"} }],....# 
+000090f0: 2065 6e6a 6f79 2073 7769 6d6d 696e 6720   enjoy swimming 
+00009100: 7c20 6e73 7562 6a2d 7863 6f6d 7020 656e  | nsubj-xcomp en
+00009110: 6a6f 7920 4920 7377 696d 6d69 6e67 0a09  joy I swimming..
+00009120: 0909 226e 7375 626a 2d78 636f 6d70 223a  .."nsubj-xcomp":
+00009130: 205b 2020 7b22 5249 4748 545f 4944 223a   [  {"RIGHT_ID":
+00009140: 2022 7622 2c20 2252 4947 4854 5f41 5454   "v", "RIGHT_ATT
+00009150: 5253 223a 207b 2250 4f53 223a 2022 5645  RS": {"POS": "VE
+00009160: 5242 227d 7d2c 7b22 4c45 4654 5f49 4422  RB"}},{"LEFT_ID"
+00009170: 3a20 2276 222c 2022 5245 4c5f 4f50 223a  : "v", "REL_OP":
+00009180: 2022 3e22 2c20 2252 4947 4854 5f49 4422   ">", "RIGHT_ID"
+00009190: 3a20 2273 7562 6a65 6374 222c 2022 5249  : "subject", "RI
+000091a0: 4748 545f 4154 5452 5322 3a20 7b22 4445  GHT_ATTRS": {"DE
+000091b0: 5022 3a20 226e 7375 626a 227d 207d 2c20  P": "nsubj"} }, 
+000091c0: 7b20 224c 4546 545f 4944 223a 2022 7622  { "LEFT_ID": "v"
+000091d0: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
+000091e0: 2022 5249 4748 545f 4944 223a 2022 6f62   "RIGHT_ID": "ob
+000091f0: 6a65 6374 222c 2020 2252 4947 4854 5f41  ject",  "RIGHT_A
+00009200: 5454 5253 223a 207b 2244 4550 223a 2022  TTRS": {"DEP": "
+00009210: 7863 6f6d 7022 7d20 7d5d 2c0a 0909 0923  xcomp"} }],....#
+00009220: 2070 6c61 6e20 746f 2067 6f20 2c20 7c20   plan to go , | 
+00009230: 7863 6f6d 702d 746f 2070 6c61 6e20 676f  xcomp-to plan go
+00009240: 2074 6f0a 0909 0922 7863 6f6d 702d 746f   to...."xcomp-to
+00009250: 223a 205b 2020 7b22 5249 4748 545f 4944  ": [  {"RIGHT_ID
+00009260: 223a 2022 7622 2c20 2252 4947 4854 5f41  ": "v", "RIGHT_A
+00009270: 5454 5253 223a 207b 2250 4f53 223a 2022  TTRS": {"POS": "
+00009280: 5645 5242 227d 7d2c 207b 2022 4c45 4654  VERB"}}, { "LEFT
+00009290: 5f49 4422 3a20 2276 222c 2022 5245 4c5f  _ID": "v", "REL_
+000092a0: 4f50 223a 2022 3e22 2c20 2252 4947 4854  OP": ">", "RIGHT
+000092b0: 5f49 4422 3a20 226f 626a 6563 7422 2c20  _ID": "object", 
+000092c0: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
+000092d0: 7b22 4445 5022 3a20 2278 636f 6d70 227d  {"DEP": "xcomp"}
+000092e0: 207d 2c20 7b22 4c45 4654 5f49 4422 3a20   }, {"LEFT_ID": 
+000092f0: 226f 626a 6563 7422 2c20 2252 454c 5f4f  "object", "REL_O
+00009300: 5022 3a20 223b 222c 2022 5249 4748 545f  P": ";", "RIGHT_
+00009310: 4944 223a 2022 746f 222c 2022 5249 4748  ID": "to", "RIGH
+00009320: 545f 4154 5452 5322 3a20 7b22 4c45 4d4d  T_ATTRS": {"LEMM
+00009330: 4122 3a20 2274 6f22 7d20 7d2c 5d2c 0a09  A": "to"} },],..
+00009340: 0909 2320 7475 726e 206f 6666 2074 6865  ..# turn off the
+00009350: 206c 6967 6874 207c 2070 7274 2d64 6f62   light | prt-dob
+00009360: 6a20 7475 726e 206f 6666 206c 6967 6874  j turn off light
+00009370: 0a09 0909 2264 6f62 6a2d 7072 7422 3a20  ...."dobj-prt": 
+00009380: 5b20 207b 2252 4947 4854 5f49 4422 3a20  [  {"RIGHT_ID": 
+00009390: 2276 222c 2252 4947 4854 5f41 5454 5253  "v","RIGHT_ATTRS
+000093a0: 223a 207b 2250 4f53 223a 2022 5645 5242  ": {"POS": "VERB
+000093b0: 227d 7d2c 2020 7b20 224c 4546 545f 4944  "}},  { "LEFT_ID
+000093c0: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
+000093d0: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
+000093e0: 223a 2022 7375 626a 6563 7422 2c20 2252  ": "subject", "R
+000093f0: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
+00009400: 4550 223a 2022 7072 7422 7d20 7d2c 207b  EP": "prt"} }, {
+00009410: 2022 4c45 4654 5f49 4422 3a20 2276 222c   "LEFT_ID": "v",
+00009420: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
+00009430: 2252 4947 4854 5f49 4422 3a20 226f 626a  "RIGHT_ID": "obj
+00009440: 6563 7422 2c20 2252 4947 4854 5f41 5454  ect", "RIGHT_ATT
+00009450: 5253 223a 207b 2244 4550 223a 2022 646f  RS": {"DEP": "do
+00009460: 626a 227d 207d 5d2c 0a09 0909 2320 536f  bj"} }],....# So
+00009470: 6d65 206f 6620 7468 6520 5265 7075 626c  me of the Republ
+00009480: 6963 616e 2070 6f6c 6963 6965 7320 6861  ican policies ha
+00009490: 7665 206c 6566 7420 6665 6d69 6e69 7374  ve left feminist
+000094a0: 7320 6469 736d 6179 6564 2061 6e64 2061  s dismayed and a
+000094b0: 6768 6173 742e 207c 2064 6f62 6a2d 6163  ghast. | dobj-ac
+000094c0: 6c20 6c65 6176 6520 6665 6d69 6e69 7374  l leave feminist
+000094d0: 2064 6973 6d61 7965 640a 0909 0922 646f   dismayed...."do
+000094e0: 626a 2d61 636c 223a 5b20 7b22 5249 4748  bj-acl":[ {"RIGH
+000094f0: 545f 4944 223a 2022 7622 2c22 5249 4748  T_ID": "v","RIGH
+00009500: 545f 4154 5452 5322 3a20 7b22 504f 5322  T_ATTRS": {"POS"
+00009510: 3a20 2256 4552 4222 7d7d 2c20 7b20 224c  : "VERB"}}, { "L
+00009520: 4546 545f 4944 223a 2022 7622 2c22 5245  EFT_ID": "v","RE
+00009530: 4c5f 4f50 223a 2022 3e22 2c22 5249 4748  L_OP": ">","RIGH
+00009540: 545f 4944 223a 2022 646f 626a 222c 2252  T_ID": "dobj","R
+00009550: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
+00009560: 4550 223a 2022 646f 626a 227d 7d2c 7b20  EP": "dobj"}},{ 
+00009570: 2022 4c45 4654 5f49 4422 3a20 2264 6f62   "LEFT_ID": "dob
+00009580: 6a22 2c20 2252 454c 5f4f 5022 3a20 223e  j", "REL_OP": ">
+00009590: 222c 2022 5249 4748 545f 4944 223a 2022  ", "RIGHT_ID": "
+000095a0: 7072 6570 222c 2022 5249 4748 545f 4154  prep", "RIGHT_AT
+000095b0: 5452 5322 3a20 7b22 4445 5022 3a20 2261  TRS": {"DEP": "a
+000095c0: 636c 227d 7d5d 2c0a 0909 0923 2062 6520  cl"}}],....# be 
+000095d0: 6861 7070 7920 7769 7468 207c 206e 7375  happy with | nsu
+000095e0: 626a 2d61 636f 6d70 2062 6520 4920 6861  bj-acomp be I ha
+000095f0: 7070 790a 0909 0922 6163 6f6d 702d 7072  ppy...."acomp-pr
+00009600: 6570 223a 5b20 7b22 5249 4748 545f 4944  ep":[ {"RIGHT_ID
+00009610: 223a 2022 7622 2c22 5249 4748 545f 4154  ": "v","RIGHT_AT
+00009620: 5452 5322 3a20 7b22 504f 5322 3a20 2256  TRS": {"POS": "V
+00009630: 4552 4222 7d7d 2c20 7b20 224c 4546 545f  ERB"}}, { "LEFT_
+00009640: 4944 223a 2022 7622 2c22 5245 4c5f 4f50  ID": "v","REL_OP
+00009650: 223a 2022 3e22 2c22 5249 4748 545f 4944  ": ">","RIGHT_ID
+00009660: 223a 2022 6163 6f6d 7022 2c22 5249 4748  ": "acomp","RIGH
+00009670: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
+00009680: 3a20 2261 636f 6d70 227d 7d2c 7b20 2022  : "acomp"}},{  "
+00009690: 4c45 4654 5f49 4422 3a20 2261 636f 6d70  LEFT_ID": "acomp
+000096a0: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
+000096b0: 2c20 2252 4947 4854 5f49 4422 3a20 2270  , "RIGHT_ID": "p
+000096c0: 7265 7022 2c20 2252 4947 4854 5f41 5454  rep", "RIGHT_ATT
+000096d0: 5253 223a 207b 2244 4550 223a 2022 7072  RS": {"DEP": "pr
+000096e0: 6570 227d 7d5d 2c0a 0909 0923 2062 6520  ep"}}],....# be 
+000096f0: 6261 7365 6420 6f6e 207c 2062 652d 7662  based on | be-vb
+00009700: 6e2d 7072 6570 2062 6173 6520 6265 206f  n-prep base be o
+00009710: 6e0a 0909 0922 6265 2d76 626e 2d70 7265  n...."be-vbn-pre
+00009720: 7022 3a5b 207b 2252 4947 4854 5f49 4422  p":[ {"RIGHT_ID"
+00009730: 3a20 2276 222c 2022 5249 4748 545f 4154  : "v", "RIGHT_AT
+00009740: 5452 5322 3a20 7b22 5441 4722 3a20 2256  TRS": {"TAG": "V
+00009750: 424e 227d 7d2c 207b 224c 4546 545f 4944  BN"}}, {"LEFT_ID
+00009760: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
+00009770: 3a20 223e 222c 2252 4947 4854 5f49 4422  : ">","RIGHT_ID"
+00009780: 3a20 2262 6522 2c22 5249 4748 545f 4154  : "be","RIGHT_AT
+00009790: 5452 5322 3a20 7b22 4c45 4d4d 4122 3a20  TRS": {"LEMMA": 
+000097a0: 2262 6522 7d20 7d2c 207b 2022 4c45 4654  "be"} }, { "LEFT
+000097b0: 5f49 4422 3a20 2276 222c 2022 5245 4c5f  _ID": "v", "REL_
+000097c0: 4f50 223a 2022 3e22 2c20 2252 4947 4854  OP": ">", "RIGHT
+000097d0: 5f49 4422 3a20 2270 7265 7022 2c20 2252  _ID": "prep", "R
+000097e0: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
+000097f0: 4550 223a 2022 7072 6570 227d 2020 7d5d  EP": "prep"}  }]
+00009800: 2c0a 0909 097d 0a09 0966 6f72 206e 616d  ,....}...for nam
+00009810: 652c 7061 7420 696e 2070 6174 7465 726e  e,pat in pattern
+00009820: 2e69 7465 6d73 2829 3a20 6465 706d 6174  .items(): depmat
+00009830: 6368 2e6d 6174 6368 6572 2e61 6464 286e  ch.matcher.add(n
+00009840: 616d 652c 205b 7061 745d 290a 0972 6574  ame, [pat])..ret
+00009850: 7572 6e20 6465 706d 6174 6368 2e6d 6174  urn depmatch.mat
+00009860: 6368 6572 200a 0923 646f 6320 3d20 7370  cher ..#doc = sp
+00009870: 6163 792e 6e6c 7028 2249 2074 7572 6e20  acy.nlp("I turn 
+00009880: 6f66 6620 7468 6520 6c69 6768 742c 2061  off the light, a
+00009890: 6e64 2069 7420 6973 2062 6173 6564 206f  nd it is based o
+000098a0: 6e20 7468 6520 7461 626c 652e 2229 0a09  n the table.")..
+000098b0: 2366 6f72 206e 616d 652c 2061 7220 696e  #for name, ar in
+000098c0: 206d 6174 6368 6572 2864 6f63 2920 3a20   matcher(doc) : 
+000098d0: 7072 696e 7428 7370 6163 792e 6e6c 702e  print(spacy.nlp.
+000098e0: 766f 6361 625b 6e61 6d65 5d2e 7465 7874  vocab[name].text
+000098f0: 2c20 646f 635b 6172 5b30 5d5d 2e6c 656d  , doc[ar[0]].lem
+00009900: 6d61 5f2c 2064 6f63 5b61 725b 315d 5d2e  ma_, doc[ar[1]].
+00009910: 6c65 6d6d 615f 2c20 646f 635b 6172 5b32  lemma_, doc[ar[2
+00009920: 5d5d 2920 2320 776f 7272 7920 6265 2074  ]]) # worry be t
+00009930: 6872 696c 6c65 640a 0a64 6566 2074 7270  hrilled..def trp
+00009940: 7828 646f 632c 2076 6f63 6162 293a 2023  x(doc, vocab): #
+00009950: 2073 7061 6379 2e6e 6c70 2e76 6f63 6162   spacy.nlp.vocab
+00009960: 2c20 3230 3233 2e31 2e32 310a 0966 726f  , 2023.1.21..fro
+00009970: 6d20 7370 6163 792e 6d61 7463 6865 7220  m spacy.matcher 
+00009980: 696d 706f 7274 2044 6570 656e 6465 6e63  import Dependenc
+00009990: 794d 6174 6368 6572 0a09 6966 206e 6f74  yMatcher..if not
+000099a0: 2068 6173 6174 7472 2874 7270 782c 276d   hasattr(trpx,'m
+000099b0: 6174 6368 6572 2729 3a20 0a09 0974 7270  atcher'): ...trp
+000099c0: 782e 6d61 7463 6865 7220 3d20 4465 7065  x.matcher = Depe
+000099d0: 6e64 656e 6379 4d61 7463 6865 7228 766f  ndencyMatcher(vo
+000099e0: 6361 6229 0a09 0970 6174 7465 726e 203d  cab)...pattern =
+000099f0: 207b 0a09 0909 2320 6164 7663 6c2d 6163   {....# advcl-ac
+00009a00: 6f6d 7020 776f 7272 7920 6265 2074 6872  omp worry be thr
+00009a10: 696c 6c65 6420 7c20 2257 6869 6c65 2049  illed | "While I
+00009a20: 2077 6173 2074 6872 696c 6c65 6420 7468   was thrilled th
+00009a30: 6174 2069 7420 7761 7320 6f6b 2c20 4920  at it was ok, I 
+00009a40: 776f 7272 6965 6420 7468 6174 2073 6865  worried that she
+00009a50: 2069 7320 6861 7070 792e 220a 0909 0922   is happy."...."
+00009a60: 6164 7663 6c2d 6163 6f6d 7022 3a20 5b20  advcl-acomp": [ 
+00009a70: 7b22 5249 4748 545f 4944 223a 2022 7622  {"RIGHT_ID": "v"
+00009a80: 2c20 2252 4947 4854 5f41 5454 5253 223a  , "RIGHT_ATTRS":
+00009a90: 207b 2250 4f53 223a 2022 5645 5242 227d   {"POS": "VERB"}
+00009aa0: 7d2c 2020 7b20 224c 4546 545f 4944 223a  },  { "LEFT_ID":
+00009ab0: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
+00009ac0: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
+00009ad0: 2022 6164 7663 6c22 2c20 2252 4947 4854   "advcl", "RIGHT
+00009ae0: 5f41 5454 5253 223a 207b 2244 4550 223a  _ATTRS": {"DEP":
+00009af0: 2022 6164 7663 6c22 7d20 7d2c 207b 2022   "advcl"} }, { "
+00009b00: 4c45 4654 5f49 4422 3a20 2261 6476 636c  LEFT_ID": "advcl
+00009b10: 222c 2022 5245 4c5f 4f50 223a 2022 3e22  ", "REL_OP": ">"
+00009b20: 2c22 5249 4748 545f 4944 223a 2022 6f62  ,"RIGHT_ID": "ob
+00009b30: 6a65 6374 222c 2022 5249 4748 545f 4154  ject", "RIGHT_AT
+00009b40: 5452 5322 3a20 7b22 4445 5022 3a20 2261  TRS": {"DEP": "a
+00009b50: 636f 6d70 227d 207d 5d20 2c20 0a09 0909  comp"} }] , ....
+00009b60: 2320 5368 6520 6973 2068 6170 7079 2e20  # She is happy. 
+00009b70: 7c20 6e73 7562 6a2d 6163 6f6d 7020 6265  | nsubj-acomp be
+00009b80: 2073 6865 2068 6170 7079 0a09 0909 226e   she happy...."n
+00009b90: 7375 626a 2d61 636f 6d70 223a 205b 207b  subj-acomp": [ {
+00009ba0: 2022 5249 4748 545f 4944 223a 2022 7622   "RIGHT_ID": "v"
+00009bb0: 2c20 2020 2252 4947 4854 5f41 5454 5253  ,   "RIGHT_ATTRS
+00009bc0: 223a 207b 224c 454d 4d41 223a 2022 6265  ": {"LEMMA": "be
+00009bd0: 227d 7d2c 7b20 224c 4546 545f 4944 223a  "}},{ "LEFT_ID":
+00009be0: 2022 7622 2c20 2252 454c 5f4f 5022 3a22   "v", "REL_OP":"
+00009bf0: 3e22 2c20 2252 4947 4854 5f49 4422 3a20  >", "RIGHT_ID": 
+00009c00: 2273 7562 6a65 6374 222c 2022 5249 4748  "subject", "RIGH
+00009c10: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
+00009c20: 3a20 226e 7375 626a 227d 207d 2c20 7b20  : "nsubj"} }, { 
+00009c30: 2022 4c45 4654 5f49 4422 3a20 2276 222c   "LEFT_ID": "v",
+00009c40: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
+00009c50: 2022 5249 4748 545f 4944 223a 2022 6f62   "RIGHT_ID": "ob
+00009c60: 6a65 6374 222c 2020 2020 2252 4947 4854  ject",    "RIGHT
+00009c70: 5f41 5454 5253 223a 207b 2244 4550 223a  _ATTRS": {"DEP":
+00009c80: 2022 6163 6f6d 7022 7d7d 5d2c 200a 0909   "acomp"}}], ...
+00009c90: 0923 5368 6520 6973 2020 6120 6769 726c  .#She is  a girl
+00009ca0: 2e20 7c20 6e73 7562 6a2d 6174 7472 2062  . | nsubj-attr b
+00009cb0: 6520 7368 6520 6769 726c 0a09 0909 226e  e she girl...."n
+00009cc0: 7375 626a 2d61 7474 7222 3a20 5b20 207b  subj-attr": [  {
+00009cd0: 2252 4947 4854 5f49 4422 3a20 2276 222c  "RIGHT_ID": "v",
+00009ce0: 2022 5249 4748 545f 4154 5452 5322 3a20   "RIGHT_ATTRS": 
+00009cf0: 7b22 4c45 4d4d 4122 3a20 2262 6522 7d7d  {"LEMMA": "be"}}
+00009d00: 2c20 7b20 224c 4546 545f 4944 223a 2022  , { "LEFT_ID": "
+00009d10: 7622 2c20 2252 454c 5f4f 5022 3a20 223e  v", "REL_OP": ">
+00009d20: 222c 2252 4947 4854 5f49 4422 3a20 2273  ","RIGHT_ID": "s
+00009d30: 7562 6a65 6374 222c 2022 5249 4748 545f  ubject", "RIGHT_
+00009d40: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
+00009d50: 226e 7375 626a 227d 207d 2c20 7b20 2020  "nsubj"} }, {   
+00009d60: 2022 4c45 4654 5f49 4422 3a20 2276 222c   "LEFT_ID": "v",
+00009d70: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
+00009d80: 2252 4947 4854 5f49 4422 3a20 226f 626a  "RIGHT_ID": "obj
+00009d90: 6563 7422 2c20 2252 4947 4854 5f41 5454  ect", "RIGHT_ATT
+00009da0: 5253 223a 207b 2244 4550 223a 2022 6174  RS": {"DEP": "at
+00009db0: 7472 227d 207d 5d2c 0a09 0909 2320 2065  tr"} }],....#  e
+00009dc0: 6e6a 6f79 2073 7769 6d6d 696e 6720 7c20  njoy swimming | 
+00009dd0: 6e73 7562 6a2d 7863 6f6d 7020 656e 6a6f  nsubj-xcomp enjo
+00009de0: 7920 4920 7377 696d 6d69 6e67 0a09 0909  y I swimming....
+00009df0: 226e 7375 626a 2d78 636f 6d70 223a 205b  "nsubj-xcomp": [
+00009e00: 2020 7b22 5249 4748 545f 4944 223a 2022    {"RIGHT_ID": "
+00009e10: 7622 2c20 2252 4947 4854 5f41 5454 5253  v", "RIGHT_ATTRS
+00009e20: 223a 207b 2250 4f53 223a 2022 5645 5242  ": {"POS": "VERB
+00009e30: 227d 7d2c 7b22 4c45 4654 5f49 4422 3a20  "}},{"LEFT_ID": 
+00009e40: 2276 222c 2022 5245 4c5f 4f50 223a 2022  "v", "REL_OP": "
+00009e50: 3e22 2c20 2252 4947 4854 5f49 4422 3a20  >", "RIGHT_ID": 
+00009e60: 2273 7562 6a65 6374 222c 2022 5249 4748  "subject", "RIGH
+00009e70: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
+00009e80: 3a20 226e 7375 626a 227d 207d 2c20 7b20  : "nsubj"} }, { 
+00009e90: 224c 4546 545f 4944 223a 2022 7622 2c20  "LEFT_ID": "v", 
+00009ea0: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
+00009eb0: 5249 4748 545f 4944 223a 2022 6f62 6a65  RIGHT_ID": "obje
+00009ec0: 6374 222c 2020 2252 4947 4854 5f41 5454  ct",  "RIGHT_ATT
+00009ed0: 5253 223a 207b 2244 4550 223a 2022 7863  RS": {"DEP": "xc
+00009ee0: 6f6d 7022 7d20 7d5d 2c0a 0909 0923 2070  omp"} }],....# p
+00009ef0: 6c61 6e20 746f 2067 6f20 2c20 7c20 7863  lan to go , | xc
+00009f00: 6f6d 702d 746f 2070 6c61 6e20 676f 2074  omp-to plan go t
+00009f10: 6f0a 0909 0922 7863 6f6d 702d 746f 223a  o...."xcomp-to":
+00009f20: 205b 2020 7b22 5249 4748 545f 4944 223a   [  {"RIGHT_ID":
+00009f30: 2022 7622 2c20 2252 4947 4854 5f41 5454   "v", "RIGHT_ATT
+00009f40: 5253 223a 207b 2250 4f53 223a 2022 5645  RS": {"POS": "VE
+00009f50: 5242 227d 7d2c 207b 2022 4c45 4654 5f49  RB"}}, { "LEFT_I
+00009f60: 4422 3a20 2276 222c 2022 5245 4c5f 4f50  D": "v", "REL_OP
+00009f70: 223a 2022 3e22 2c20 2252 4947 4854 5f49  ": ">", "RIGHT_I
+00009f80: 4422 3a20 226f 626a 6563 7422 2c20 2022  D": "object",  "
+00009f90: 5249 4748 545f 4154 5452 5322 3a20 7b22  RIGHT_ATTRS": {"
+00009fa0: 4445 5022 3a20 2278 636f 6d70 227d 207d  DEP": "xcomp"} }
+00009fb0: 2c20 7b22 4c45 4654 5f49 4422 3a20 226f  , {"LEFT_ID": "o
+00009fc0: 626a 6563 7422 2c20 2252 454c 5f4f 5022  bject", "REL_OP"
+00009fd0: 3a20 223b 222c 2022 5249 4748 545f 4944  : ";", "RIGHT_ID
+00009fe0: 223a 2022 746f 222c 2022 5249 4748 545f  ": "to", "RIGHT_
+00009ff0: 4154 5452 5322 3a20 7b22 4c45 4d4d 4122  ATTRS": {"LEMMA"
+0000a000: 3a20 2274 6f22 7d20 7d2c 5d2c 0a09 0909  : "to"} },],....
+0000a010: 2320 7475 726e 206f 6666 2074 6865 206c  # turn off the l
+0000a020: 6967 6874 207c 2070 7274 2d64 6f62 6a20  ight | prt-dobj 
+0000a030: 7475 726e 206f 6666 206c 6967 6874 0a09  turn off light..
+0000a040: 0909 2264 6f62 6a2d 7072 7422 3a20 5b20  .."dobj-prt": [ 
+0000a050: 207b 2252 4947 4854 5f49 4422 3a20 2276   {"RIGHT_ID": "v
+0000a060: 222c 2252 4947 4854 5f41 5454 5253 223a  ","RIGHT_ATTRS":
+0000a070: 207b 2250 4f53 223a 2022 5645 5242 227d   {"POS": "VERB"}
+0000a080: 7d2c 2020 7b20 224c 4546 545f 4944 223a  },  { "LEFT_ID":
+0000a090: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
+0000a0a0: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
+0000a0b0: 2022 7375 626a 6563 7422 2c20 2252 4947   "subject", "RIG
+0000a0c0: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
+0000a0d0: 223a 2022 7072 7422 7d20 7d2c 207b 2022  ": "prt"} }, { "
+0000a0e0: 4c45 4654 5f49 4422 3a20 2276 222c 2022  LEFT_ID": "v", "
+0000a0f0: 5245 4c5f 4f50 223a 2022 3e22 2c20 2252  REL_OP": ">", "R
+0000a100: 4947 4854 5f49 4422 3a20 226f 626a 6563  IGHT_ID": "objec
+0000a110: 7422 2c20 2252 4947 4854 5f41 5454 5253  t", "RIGHT_ATTRS
+0000a120: 223a 207b 2244 4550 223a 2022 646f 626a  ": {"DEP": "dobj
+0000a130: 227d 207d 5d2c 0a09 0909 2320 536f 6d65  "} }],....# Some
+0000a140: 206f 6620 7468 6520 5265 7075 626c 6963   of the Republic
+0000a150: 616e 2070 6f6c 6963 6965 7320 6861 7665  an policies have
+0000a160: 206c 6566 7420 6665 6d69 6e69 7374 7320   left feminists 
+0000a170: 6469 736d 6179 6564 2061 6e64 2061 6768  dismayed and agh
+0000a180: 6173 742e 207c 2064 6f62 6a2d 6163 6c20  ast. | dobj-acl 
+0000a190: 6c65 6176 6520 6665 6d69 6e69 7374 2064  leave feminist d
+0000a1a0: 6973 6d61 7965 640a 0909 0922 646f 626a  ismayed...."dobj
+0000a1b0: 2d61 636c 223a 5b20 7b22 5249 4748 545f  -acl":[ {"RIGHT_
+0000a1c0: 4944 223a 2022 7622 2c22 5249 4748 545f  ID": "v","RIGHT_
+0000a1d0: 4154 5452 5322 3a20 7b22 504f 5322 3a20  ATTRS": {"POS": 
+0000a1e0: 2256 4552 4222 7d7d 2c20 7b20 224c 4546  "VERB"}}, { "LEF
+0000a1f0: 545f 4944 223a 2022 7622 2c22 5245 4c5f  T_ID": "v","REL_
+0000a200: 4f50 223a 2022 3e22 2c22 5249 4748 545f  OP": ">","RIGHT_
+0000a210: 4944 223a 2022 646f 626a 222c 2252 4947  ID": "dobj","RIG
+0000a220: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
+0000a230: 223a 2022 646f 626a 227d 7d2c 7b20 2022  ": "dobj"}},{  "
+0000a240: 4c45 4654 5f49 4422 3a20 2264 6f62 6a22  LEFT_ID": "dobj"
+0000a250: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
+0000a260: 2022 5249 4748 545f 4944 223a 2022 7072   "RIGHT_ID": "pr
+0000a270: 6570 222c 2022 5249 4748 545f 4154 5452  ep", "RIGHT_ATTR
+0000a280: 5322 3a20 7b22 4445 5022 3a20 2261 636c  S": {"DEP": "acl
+0000a290: 227d 7d5d 2c0a 0909 0923 2062 6520 6861  "}}],....# be ha
+0000a2a0: 7070 7920 7769 7468 207c 206e 7375 626a  ppy with | nsubj
+0000a2b0: 2d61 636f 6d70 2062 6520 4920 6861 7070  -acomp be I happ
+0000a2c0: 790a 0909 0922 6163 6f6d 702d 7072 6570  y...."acomp-prep
+0000a2d0: 223a 5b20 7b22 5249 4748 545f 4944 223a  ":[ {"RIGHT_ID":
+0000a2e0: 2022 7622 2c22 5249 4748 545f 4154 5452   "v","RIGHT_ATTR
+0000a2f0: 5322 3a20 7b22 504f 5322 3a20 2256 4552  S": {"POS": "VER
+0000a300: 4222 7d7d 2c20 7b20 224c 4546 545f 4944  B"}}, { "LEFT_ID
+0000a310: 223a 2022 7622 2c22 5245 4c5f 4f50 223a  ": "v","REL_OP":
+0000a320: 2022 3e22 2c22 5249 4748 545f 4944 223a   ">","RIGHT_ID":
+0000a330: 2022 6163 6f6d 7022 2c22 5249 4748 545f   "acomp","RIGHT_
+0000a340: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
+0000a350: 2261 636f 6d70 227d 7d2c 7b20 2022 4c45  "acomp"}},{  "LE
+0000a360: 4654 5f49 4422 3a20 2261 636f 6d70 222c  FT_ID": "acomp",
+0000a370: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
+0000a380: 2252 4947 4854 5f49 4422 3a20 2270 7265  "RIGHT_ID": "pre
+0000a390: 7022 2c20 2252 4947 4854 5f41 5454 5253  p", "RIGHT_ATTRS
+0000a3a0: 223a 207b 2244 4550 223a 2022 7072 6570  ": {"DEP": "prep
+0000a3b0: 227d 7d5d 2c0a 0909 0923 2062 6520 6261  "}}],....# be ba
+0000a3c0: 7365 6420 6f6e 207c 2062 652d 7662 6e2d  sed on | be-vbn-
+0000a3d0: 7072 6570 2062 6173 6520 6265 206f 6e0a  prep base be on.
+0000a3e0: 0909 0922 6265 2d76 626e 2d70 7265 7022  ..."be-vbn-prep"
+0000a3f0: 3a5b 207b 2252 4947 4854 5f49 4422 3a20  :[ {"RIGHT_ID": 
+0000a400: 2276 222c 2022 5249 4748 545f 4154 5452  "v", "RIGHT_ATTR
+0000a410: 5322 3a20 7b22 5441 4722 3a20 2256 424e  S": {"TAG": "VBN
+0000a420: 227d 7d2c 207b 224c 4546 545f 4944 223a  "}}, {"LEFT_ID":
+0000a430: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
+0000a440: 223e 222c 2252 4947 4854 5f49 4422 3a20  ">","RIGHT_ID": 
+0000a450: 2262 6522 2c22 5249 4748 545f 4154 5452  "be","RIGHT_ATTR
+0000a460: 5322 3a20 7b22 4c45 4d4d 4122 3a20 2262  S": {"LEMMA": "b
+0000a470: 6522 7d20 7d2c 207b 2022 4c45 4654 5f49  e"} }, { "LEFT_I
+0000a480: 4422 3a20 2276 222c 2022 5245 4c5f 4f50  D": "v", "REL_OP
+0000a490: 223a 2022 3e22 2c20 2252 4947 4854 5f49  ": ">", "RIGHT_I
+0000a4a0: 4422 3a20 2270 7265 7022 2c20 2252 4947  D": "prep", "RIG
+0000a4b0: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
+0000a4c0: 223a 2022 7072 6570 227d 2020 7d5d 2c0a  ": "prep"}  }],.
+0000a4d0: 0909 097d 0a09 0966 6f72 206e 616d 652c  ...}...for name,
+0000a4e0: 7061 7420 696e 2070 6174 7465 726e 2e69  pat in pattern.i
+0000a4f0: 7465 6d73 2829 3a20 7472 7078 2e6d 6174  tems(): trpx.mat
+0000a500: 6368 6572 2e61 6464 2866 2274 7270 783a  cher.add(f"trpx:
+0000a510: 7b6e 616d 657d 222c 205b 7061 745d 290a  {name}", [pat]).
+0000a520: 0966 6f72 206e 616d 652c 2061 7220 696e  .for name, ar in
+0000a530: 2074 7270 782e 6d61 7463 6865 7228 646f   trpx.matcher(do
+0000a540: 6329 203a 0a09 0964 6f63 2e73 7061 6e73  c) :...doc.spans
+0000a550: 5b76 6f63 6162 5b6e 616d 655d 2e74 6578  [vocab[name].tex
+0000a560: 745d 203d 205b 2064 6f63 5b61 725b 305d  t] = [ doc[ar[0]
+0000a570: 3a61 725b 305d 2b31 5d2c 2064 6f63 5b61  :ar[0]+1], doc[a
+0000a580: 725b 315d 3a61 725b 315d 2b31 5d2c 2064  r[1]:ar[1]+1], d
+0000a590: 6f63 5b61 725b 325d 3a61 725b 325d 2b31  oc[ar[2]:ar[2]+1
+0000a5a0: 5d20 5d0a 0972 6574 7572 6e20 646f 6320  ] ]..return doc 
+0000a5b0: 0a0a 6465 6620 746f 6b74 7270 2864 6f63  ..def toktrp(doc
+0000a5c0: 293a 2023 2062 6173 6963 2066 6f72 2073  ): # basic for s
+0000a5d0: 716c 7369 200a 0961 7272 203d 205b 6622  qlsi ..arr = [f"
+0000a5e0: 2a3a 736e 746e 756d 225d 0a09 666f 7220  *:sntnum"]..for 
+0000a5f0: 7420 696e 2064 6f63 3a0a 0909 5b61 7272  t in doc:...[arr
+0000a600: 2e61 7070 656e 6428 7329 2066 6f72 2073  .append(s) for s
+0000a610: 2069 6e20 2028 222a 3a4c 4558 222c 222a   in  ("*:LEX","*
+0000a620: 3a4c 454d 222c 2066 222a 3a7b 742e 706f  :LEM", f"*:{t.po
+0000a630: 735f 7d22 2c20 6622 2a3a 7b74 2e74 6167  s_}", f"*:{t.tag
+0000a640: 5f7d 222c 6622 2a3a 7b74 2e64 6570 5f7d  _}",f"*:{t.dep_}
+0000a650: 222c 6622 2a3a 7e7b 742e 6465 705f 7d22  ",f"*:~{t.dep_}"
+0000a660: 2920 5d0a 0909 6966 2074 2e70 6f73 5f20  ) ]...if t.pos_ 
+0000a670: 696e 2028 2256 4552 4222 2c22 4e4f 554e  in ("VERB","NOUN
+0000a680: 222c 2241 444a 222c 2241 4456 2229 203a  ","ADJ","ADV") :
+0000a690: 200a 0909 0961 7272 2e61 7070 656e 6428   ....arr.append(
+0000a6a0: 2066 227b 742e 7461 675f 7d3a 7b74 2e74   f"{t.tag_}:{t.t
+0000a6b0: 6578 742e 6c6f 7765 7228 297d 2229 2020  ext.lower()}")  
+0000a6c0: 2320 5642 4420 3a20 206d 6164 6520 2c20  # VBD :  made , 
+0000a6d0: 6164 6465 6420 3230 3232 2e31 322e 3130  added 2022.12.10
+0000a6e0: 0a0a 0909 6966 206e 6f74 2074 2e70 6f73  ....if not t.pos
+0000a6f0: 5f20 696e 2028 2750 524f 504e 272c 2758  _ in ('PROPN','X
+0000a700: 272c 2027 5055 4e43 5427 2c22 5350 4143  ', 'PUNCT',"SPAC
+0000a710: 4522 2920 616e 6420 742e 6973 5f61 6c70  E") and t.is_alp
+0000a720: 6861 3a0a 0909 0961 7272 2e65 7874 656e  ha:....arr.exten
+0000a730: 6428 5b66 227b 742e 6c65 6d6d 615f 7d3a  d([f"{t.lemma_}:
+0000a740: 7b74 2e70 6f73 5f7d 222c 6622 7b74 2e6c  {t.pos_}",f"{t.l
+0000a750: 656d 6d61 5f7d 3a4c 4558 3a7b 742e 7465  emma_}:LEX:{t.te
+0000a760: 7874 2e6c 6f77 6572 2829 7d22 2c66 224c  xt.lower()}",f"L
+0000a770: 454d 3a7b 742e 6c65 6d6d 615f 2e6c 6f77  EM:{t.lemma_.low
+0000a780: 6572 2829 7d22 2c66 224c 4558 3a7b 742e  er()}",f"LEX:{t.
+0000a790: 7465 7874 2e6c 6f77 6572 2829 7d22 2c66  text.lower()}",f
+0000a7a0: 227b 742e 706f 735f 7d3a 7b74 2e6c 656d  "{t.pos_}:{t.lem
+0000a7b0: 6d61 5f2e 6c6f 7765 7228 297d 222c 6622  ma_.lower()}",f"
+0000a7c0: 7b74 2e6c 656d 6d61 5f2e 6c6f 7765 7228  {t.lemma_.lower(
+0000a7d0: 297d 3a7b 742e 706f 735f 7d3a 7b74 2e74  )}:{t.pos_}:{t.t
+0000a7e0: 6167 5f7d 222c 6622 2a3a 7b74 2e70 6f73  ag_}",f"*:{t.pos
+0000a7f0: 5f7d 3a7b 742e 7461 675f 7d22 5d29 200a  _}:{t.tag_}"]) .
+0000a800: 0909 6966 2074 2e70 6f73 5f20 6e6f 7420  ..if t.pos_ not 
+0000a810: 696e 2028 2250 524f 504e 222c 2250 554e  in ("PROPN","PUN
+0000a820: 4354 222c 2253 5041 4345 2229 2061 6e64  CT","SPACE") and
+0000a830: 2074 2e69 735f 616c 7068 6120 616e 6420   t.is_alpha and 
+0000a840: 742e 6865 6164 2e69 735f 616c 7068 613a  t.head.is_alpha:
+0000a850: 0a09 0909 6172 722e 6578 7465 6e64 285b  ....arr.extend([
+0000a860: 6622 7b74 2e68 6561 642e 6c65 6d6d 615f  f"{t.head.lemma_
+0000a870: 7d3a 7b74 2e68 6561 642e 706f 735f 7d3a  }:{t.head.pos_}:
+0000a880: 7b74 2e64 6570 5f7d 3a7b 742e 706f 735f  {t.dep_}:{t.pos_
+0000a890: 7d3a 7b74 2e6c 656d 6d61 5f7d 222c 2066  }:{t.lemma_}", f
+0000a8a0: 227b 742e 6865 6164 2e6c 656d 6d61 5f7d  "{t.head.lemma_}
+0000a8b0: 3a7b 742e 6865 6164 2e70 6f73 5f7d 3a7b  :{t.head.pos_}:{
+0000a8c0: 742e 6465 705f 7d3a 7b74 2e70 6f73 5f7d  t.dep_}:{t.pos_}
+0000a8d0: 222c 6622 7b74 2e68 6561 642e 6c65 6d6d  ",f"{t.head.lemm
+0000a8e0: 615f 7d3a 7b74 2e68 6561 642e 706f 735f  a_}:{t.head.pos_
+0000a8f0: 7d3a 7b74 2e64 6570 5f7d 222c 2066 222a  }:{t.dep_}", f"*
+0000a900: 3a7b 742e 6865 6164 2e70 6f73 5f7d 3a7b  :{t.head.pos_}:{
+0000a910: 742e 6465 705f 7d22 2c20 6622 2a3a 7b74  t.dep_}", f"*:{t
+0000a920: 2e68 6561 642e 706f 735f 7d3a 7b74 2e64  .head.pos_}:{t.d
+0000a930: 6570 5f7d 3a7b 742e 706f 735f 7d3a 7b74  ep_}:{t.pos_}:{t
+0000a940: 2e68 6561 642e 6c65 6d6d 615f 7d22 5d29  .head.lemma_}"])
+0000a950: 0a09 0909 6966 2074 2e64 6570 5f20 6e6f  ....if t.dep_ no
+0000a960: 7420 696e 2028 2752 4f4f 5427 293a 200a  t in ('ROOT'): .
+0000a970: 0909 0909 6172 722e 6578 7465 6e64 285b  ....arr.extend([
+0000a980: 6622 7b74 2e6c 656d 6d61 5f7d 3a7b 742e  f"{t.lemma_}:{t.
+0000a990: 706f 735f 7d3a 7e7b 742e 6465 705f 7d3a  pos_}:~{t.dep_}:
+0000a9a0: 7b74 2e68 6561 642e 706f 735f 7d3a 7b74  {t.head.pos_}:{t
+0000a9b0: 2e68 6561 642e 6c65 6d6d 615f 7d22 2c20  .head.lemma_}", 
+0000a9c0: 6622 7b74 2e6c 656d 6d61 5f7d 3a7b 742e  f"{t.lemma_}:{t.
+0000a9d0: 706f 735f 7d3a 7e7b 742e 6465 705f 7d3a  pos_}:~{t.dep_}:
+0000a9e0: 7b74 2e68 6561 642e 706f 735f 7d22 2c20  {t.head.pos_}", 
+0000a9f0: 6622 7b74 2e6c 656d 6d61 5f7d 3a7b 742e  f"{t.lemma_}:{t.
+0000aa00: 706f 735f 7d3a 7e7b 742e 6465 705f 7d22  pos_}:~{t.dep_}"
+0000aa10: 2c20 6622 2a3a 7b74 2e70 6f73 5f7d 3a7e  , f"*:{t.pos_}:~
+0000aa20: 7b74 2e64 6570 5f7d 222c 2066 222a 3a7b  {t.dep_}", f"*:{
+0000aa30: 742e 706f 735f 7d3a 7e7b 742e 6465 705f  t.pos_}:~{t.dep_
+0000aa40: 7d3a 7b74 2e68 6561 642e 706f 735f 7d3a  }:{t.head.pos_}:
+0000aa50: 7b74 2e6c 656d 6d61 5f7d 225d 290a 0a09  {t.lemma_}"])...
+0000aa60: 666f 7220 6e61 6d65 2c20 6172 2069 6e20  for name, ar in 
+0000aa70: 6465 706d 6174 6368 2829 2864 6f63 293a  depmatch()(doc):
+0000aa80: 2023 2074 7270 780a 0909 7430 2c74 312c   # trpx...t0,t1,
+0000aa90: 7432 203d 2064 6f63 5b61 725b 305d 5d2c  t2 = doc[ar[0]],
+0000aaa0: 646f 635b 6172 5b31 5d5d 2c64 6f63 5b61  doc[ar[1]],doc[a
+0000aab0: 725b 325d 5d0a 0909 6e61 6d65 203d 2020  r[2]]...name =  
+0000aac0: 7370 6163 792e 6e6c 702e 766f 6361 625b  spacy.nlp.vocab[
+0000aad0: 6e61 6d65 5d2e 7465 7874 200a 0909 6966  name].text ...if
+0000aae0: 206e 616d 6520 696e 2028 2022 6e73 7562   name in ( "nsub
+0000aaf0: 6a2d 6163 6f6d 7022 2c20 226e 7375 626a  j-acomp", "nsubj
+0000ab00: 2d61 7474 7222 293a 2020 0a09 0909 6172  -attr"):  ....ar
+0000ab10: 722e 6578 7465 6e64 285b 6622 7b74 312e  r.extend([f"{t1.
+0000ab20: 6c65 6d6d 615f 7d3a 7b74 312e 706f 735f  lemma_}:{t1.pos_
+0000ab30: 7d3a 7b6e 616d 657d 3a7b 7432 2e70 6f73  }:{name}:{t2.pos
+0000ab40: 5f7d 3a7b 7432 2e6c 656d 6d61 5f7d 222c  _}:{t2.lemma_}",
+0000ab50: 6622 7b74 312e 6c65 6d6d 615f 7d3a 7b74  f"{t1.lemma_}:{t
+0000ab60: 312e 706f 735f 7d3a 7b6e 616d 657d 3a7b  1.pos_}:{name}:{
+0000ab70: 7432 2e70 6f73 5f7d 222c 6622 7b74 312e  t2.pos_}",f"{t1.
+0000ab80: 6c65 6d6d 615f 7d3a 7b74 312e 706f 735f  lemma_}:{t1.pos_
+0000ab90: 7d3a 7b6e 616d 657d 225d 290a 0909 0961  }:{name}"])....a
+0000aba0: 7272 2e65 7874 656e 6428 5b66 227b 7432  rr.extend([f"{t2
+0000abb0: 2e6c 656d 6d61 5f7d 3a7b 7432 2e70 6f73  .lemma_}:{t2.pos
+0000abc0: 5f7d 3a7e 7b6e 616d 657d 3a7b 7431 2e70  _}:~{name}:{t1.p
+0000abd0: 6f73 5f7d 3a7b 7431 2e6c 656d 6d61 5f7d  os_}:{t1.lemma_}
+0000abe0: 222c 2066 227b 7432 2e6c 656d 6d61 5f7d  ", f"{t2.lemma_}
+0000abf0: 3a7b 7432 2e70 6f73 5f7d 3a7e 7b6e 616d  :{t2.pos_}:~{nam
+0000ac00: 657d 3a7b 7431 2e70 6f73 5f7d 222c 2066  e}:{t1.pos_}", f
+0000ac10: 227b 7432 2e6c 656d 6d61 5f7d 3a7b 7432  "{t2.lemma_}:{t2
+0000ac20: 2e70 6f73 5f7d 3a7e 7b6e 616d 657d 225d  .pos_}:~{name}"]
+0000ac30: 290a 0909 656c 6966 206e 616d 6520 696e  )...elif name in
+0000ac40: 2028 2261 6476 636c 2d61 636f 6d70 222c   ("advcl-acomp",
+0000ac50: 2261 636f 6d70 2d70 7265 7022 2920 3a20  "acomp-prep") : 
+0000ac60: 090a 0909 0961 7272 2e65 7874 656e 6428  .....arr.extend(
+0000ac70: 5b66 227b 7430 2e6c 656d 6d61 5f7d 3a7b  [f"{t0.lemma_}:{
+0000ac80: 7430 2e70 6f73 5f7d 3a7b 6e61 6d65 7d3a  t0.pos_}:{name}:
+0000ac90: 7b74 322e 706f 735f 7d3a 7b74 322e 6c65  {t2.pos_}:{t2.le
+0000aca0: 6d6d 615f 7d22 2c66 227b 7430 2e6c 656d  mma_}",f"{t0.lem
+0000acb0: 6d61 5f7d 3a7b 7430 2e70 6f73 5f7d 3a7b  ma_}:{t0.pos_}:{
+0000acc0: 6e61 6d65 7d3a 7b74 322e 706f 735f 7d22  name}:{t2.pos_}"
+0000acd0: 2c66 227b 7430 2e6c 656d 6d61 5f7d 3a7b  ,f"{t0.lemma_}:{
+0000ace0: 7430 2e70 6f73 5f7d 3a7b 6e61 6d65 7d22  t0.pos_}:{name}"
+0000acf0: 5d29 0a09 0909 6172 722e 6578 7465 6e64  ])....arr.extend
+0000ad00: 285b 6622 7b74 322e 6c65 6d6d 615f 7d3a  ([f"{t2.lemma_}:
+0000ad10: 7b74 322e 706f 735f 7d3a 7e7b 6e61 6d65  {t2.pos_}:~{name
+0000ad20: 7d3a 7b74 302e 706f 735f 7d3a 7b74 302e  }:{t0.pos_}:{t0.
+0000ad30: 6c65 6d6d 615f 7d22 2c66 227b 7432 2e6c  lemma_}",f"{t2.l
+0000ad40: 656d 6d61 5f7d 3a7b 7432 2e70 6f73 5f7d  emma_}:{t2.pos_}
+0000ad50: 3a7e 7b6e 616d 657d 3a7b 7430 2e70 6f73  :~{name}:{t0.pos
+0000ad60: 5f7d 222c 6622 7b74 322e 6c65 6d6d 615f  _}",f"{t2.lemma_
+0000ad70: 7d3a 7b74 322e 706f 735f 7d3a 7e7b 6e61  }:{t2.pos_}:~{na
+0000ad80: 6d65 7d22 5d29 0a09 0965 6c69 6620 6e61  me}"])...elif na
+0000ad90: 6d65 2069 6e20 2822 646f 626a 2d70 7274  me in ("dobj-prt
+0000ada0: 2229 2061 6e64 2074 322e 706f 735f 206e  ") and t2.pos_ n
+0000adb0: 6f74 2069 6e20 2827 5052 4f50 4e27 293a  ot in ('PROPN'):
+0000adc0: 2009 0a09 0909 6172 722e 6170 7065 6e64   .....arr.append
+0000add0: 2866 227b 7430 2e6c 656d 6d61 5f7d 5f7b  (f"{t0.lemma_}_{
+0000ade0: 7431 2e6c 656d 6d61 5f7d 3a7b 7430 2e70  t1.lemma_}:{t0.p
+0000adf0: 6f73 5f7d 3a64 6f62 6a3a 7b74 322e 706f  os_}:dobj:{t2.po
+0000ae00: 735f 7d3a 7b74 322e 6c65 6d6d 615f 7d22  s_}:{t2.lemma_}"
+0000ae10: 290a 0909 0961 7272 2e61 7070 656e 6428  )....arr.append(
+0000ae20: 6622 7b74 322e 6c65 6d6d 615f 7d3a 7b74  f"{t2.lemma_}:{t
+0000ae30: 322e 706f 735f 7d3a 7e64 6f62 6a3a 7b74  2.pos_}:~dobj:{t
+0000ae40: 302e 706f 735f 7d3a 7b74 302e 6c65 6d6d  0.pos_}:{t0.lemm
+0000ae50: 615f 7d5f 7b74 312e 6c65 6d6d 615f 7d22  a_}_{t1.lemma_}"
+0000ae60: 290a 0909 656c 6966 206e 616d 6520 696e  )...elif name in
+0000ae70: 2028 2262 652d 7662 6e2d 7072 6570 2229   ("be-vbn-prep")
+0000ae80: 203a 2009 2362 6173 653a 5645 5242 3a62   : .#base:VERB:b
+0000ae90: 652d 7662 6e2d 7072 6570 3a62 6520 6261  e-vbn-prep:be ba
+0000aea0: 7365 6420 6f6e 0a09 0909 6172 722e 6578  sed on....arr.ex
+0000aeb0: 7465 6e64 285b 6622 7b74 302e 6c65 6d6d  tend([f"{t0.lemm
+0000aec0: 615f 7d3a 7b74 302e 706f 735f 7d3a 7b6e  a_}:{t0.pos_}:{n
+0000aed0: 616d 657d 3a7b 7431 2e6c 656d 6d61 5f7d  ame}:{t1.lemma_}
+0000aee0: 207b 7430 2e74 6578 742e 6c6f 7765 7228   {t0.text.lower(
+0000aef0: 297d 207b 7432 2e74 6578 742e 6c6f 7765  )} {t2.text.lowe
+0000af00: 7228 297d 222c 6622 7b74 302e 6c65 6d6d  r()}",f"{t0.lemm
+0000af10: 615f 7d3a 7b74 302e 706f 735f 7d3a 7b6e  a_}:{t0.pos_}:{n
+0000af20: 616d 657d 225d 290a 0909 090a 0966 6f72  ame}"])......for
+0000af30: 2073 7020 696e 2064 6f63 2e6e 6f75 6e5f   sp in doc.noun_
+0000af40: 6368 756e 6b73 3a20 2362 6f6f 6b3a 4e4f  chunks: #book:NO
+0000af50: 554e 3a6e 703a 6120 626f 6f6b 0a09 0961  UN:np:a book...a
+0000af60: 7272 2e65 7874 656e 6428 5b66 227b 7370  rr.extend([f"{sp
+0000af70: 2e72 6f6f 742e 6c65 6d6d 615f 2e6c 6f77  .root.lemma_.low
+0000af80: 6572 2829 7d3a 7b73 702e 726f 6f74 2e70  er()}:{sp.root.p
+0000af90: 6f73 5f7d 3a6e 703a 7b73 702e 7465 7874  os_}:np:{sp.text
+0000afa0: 2e6c 6f77 6572 2829 7d22 2c20 6622 7b73  .lower()}", f"{s
+0000afb0: 702e 726f 6f74 2e6c 656d 6d61 5f2e 6c6f  p.root.lemma_.lo
+0000afc0: 7765 7228 297d 3a7b 7370 2e72 6f6f 742e  wer()}:{sp.root.
+0000afd0: 706f 735f 7d3a 6e70 222c 2066 222a 3a7b  pos_}:np", f"*:{
+0000afe0: 7370 2e72 6f6f 742e 706f 735f 7d3a 6e70  sp.root.pos_}:np
+0000aff0: 222c 2066 222a 3a6e 7022 5d29 0a09 666f  ", f"*:np"])..fo
+0000b000: 7220 6c65 6d2c 2070 6f73 2c20 7479 7065  r lem, pos, type
+0000b010: 2c20 6368 756e 6b20 696e 206b 705f 6d61  , chunk in kp_ma
+0000b020: 7463 6865 7228 646f 6329 3a20 2362 7269  tcher(doc): #bri
+0000b030: 6e6b 3a4e 4f55 4e3a 7070 3a6f 6e20 7468  nk:NOUN:pp:on th
+0000b040: 6520 6272 696e 6b20 2009 2320 5b28 2770  e brink  .# [('p
+0000b050: 7027 2c20 276f 6e20 7468 6520 6272 696e  p', 'on the brin
+0000b060: 6b27 2c20 322c 2035 292c 2028 2761 7027  k', 2, 5), ('ap'
+0000b070: 2c20 2776 6572 7920 6861 7070 7927 2c20  , 'very happy', 
+0000b080: 392c 2031 3129 5d0a 0909 6172 722e 6578  9, 11)]...arr.ex
+0000b090: 7465 6e64 285b 6622 7b6c 656d 7d3a 7b70  tend([f"{lem}:{p
+0000b0a0: 6f73 7d3a 7b74 7970 657d 3a7b 6368 756e  os}:{type}:{chun
+0000b0b0: 6b7d 222c 2066 227b 6c65 6d7d 3a7b 706f  k}", f"{lem}:{po
+0000b0c0: 737d 3a7b 7479 7065 7d22 2c20 6622 2a3a  s}:{type}", f"*:
+0000b0d0: 7b70 6f73 7d3a 7b74 7970 657d 222c 2066  {pos}:{type}", f
+0000b0e0: 222a 3a7b 7479 7065 7d22 5d29 0a09 666f  "*:{type}"])..fo
+0000b0f0: 7220 7472 7078 2c20 726f 7720 696e 2064  r trpx, row in d
+0000b100: 6570 5f6d 6174 6368 6572 2864 6f63 293a  ep_matcher(doc):
+0000b110: 2023 5b28 2773 7678 272c 205b 312c 2030   #[('svx', [1, 0
+0000b120: 2c20 325d 295d 2023 2320 636f 6e73 6964  , 2])] ## consid
+0000b130: 6572 3a56 4552 423a 766e 706e 3a2a 2a2a  er:VERB:vnpn:***
+0000b140: 2a20 0a09 0976 6572 6269 203d 2072 6f77  * ...verbi = row
+0000b150: 5b30 5d20 2363 6f6e 7369 6465 723a 5645  [0] #consider:VE
+0000b160: 5242 3a62 655f 7662 6e5f 703a 6265 2063  RB:be_vbn_p:be c
+0000b170: 6f6e 7369 6465 7265 6420 6173 0a09 0961  onsidered as...a
+0000b180: 7272 2e65 7874 656e 6428 5b66 227b 646f  rr.extend([f"{do
+0000b190: 635b 7665 7262 695d 2e6c 656d 6d61 5f7d  c[verbi].lemma_}
+0000b1a0: 3a7b 646f 635b 7665 7262 695d 2e70 6f73  :{doc[verbi].pos
+0000b1b0: 5f7d 3a7b 7472 7078 7d22 2c20 6622 2a3a  _}:{trpx}", f"*:
+0000b1c0: 7b64 6f63 5b76 6572 6269 5d2e 706f 735f  {doc[verbi].pos_
+0000b1d0: 7d3a 7b74 7270 787d 222c 2066 222a 3a7b  }:{trpx}", f"*:{
+0000b1e0: 7472 7078 7d22 5d29 2023 636f 6e73 6964  trpx}"]) #consid
+0000b1f0: 6572 3a56 4552 423a 7376 780a 0909 6966  er:VERB:svx...if
+0000b200: 2074 7270 7820 3d3d 2027 7376 6127 2061   trpx == 'sva' a
+0000b210: 6e64 2064 6f63 5b72 6f77 5b30 5d5d 2e6c  nd doc[row[0]].l
+0000b220: 656d 6d61 5f20 3d3d 2027 6265 273a 2023  emma_ == 'be': #
+0000b230: 2066 6174 6520 6973 2073 6561 6c65 642c   fate is sealed,
+0000b240: 2061 6464 6564 2032 3032 322e 372e 3235   added 2022.7.25
+0000b250: 0a09 0909 6172 722e 6578 7465 6e64 285b  ....arr.extend([
+0000b260: 6622 7b64 6f63 5b72 6f77 5b31 5d5d 2e6c  f"{doc[row[1]].l
+0000b270: 656d 6d61 5f7d 3a7b 646f 635b 726f 775b  emma_}:{doc[row[
+0000b280: 315d 5d2e 706f 735f 7d3a 7362 6561 3a7b  1]].pos_}:sbea:{
+0000b290: 646f 635b 726f 775b 325d 5d2e 706f 735f  doc[row[2]].pos_
+0000b2a0: 7d3a 7b64 6f63 5b72 6f77 5b32 5d5d 2e6c  }:{doc[row[2]].l
+0000b2b0: 656d 6d61 5f7d 222c 2066 227b 646f 635b  emma_}", f"{doc[
+0000b2c0: 726f 775b 315d 5d2e 6c65 6d6d 615f 7d3a  row[1]].lemma_}:
+0000b2d0: 7b64 6f63 5b72 6f77 5b31 5d5d 2e70 6f73  {doc[row[1]].pos
+0000b2e0: 5f7d 3a73 6265 6122 2c20 6622 2a3a 7b64  _}:sbea", f"*:{d
+0000b2f0: 6f63 5b72 6f77 5b31 5d5d 2e70 6f73 5f7d  oc[row[1]].pos_}
+0000b300: 3a73 6265 6122 5d29 0a09 0909 6172 722e  :sbea"])....arr.
+0000b310: 6578 7465 6e64 285b 6622 7b64 6f63 5b72  extend([f"{doc[r
+0000b320: 6f77 5b32 5d5d 2e6c 656d 6d61 5f7d 3a7b  ow[2]].lemma_}:{
+0000b330: 646f 635b 726f 775b 325d 5d2e 706f 735f  doc[row[2]].pos_
+0000b340: 7d3a 7e73 6265 613a 7b64 6f63 5b72 6f77  }:~sbea:{doc[row
+0000b350: 5b31 5d5d 2e70 6f73 5f7d 3a7b 646f 635b  [1]].pos_}:{doc[
+0000b360: 726f 775b 315d 5d2e 6c65 6d6d 615f 7d22  row[1]].lemma_}"
+0000b370: 2c20 6622 7b64 6f63 5b72 6f77 5b32 5d5d  , f"{doc[row[2]]
+0000b380: 2e6c 656d 6d61 5f7d 3a7b 646f 635b 726f  .lemma_}:{doc[ro
+0000b390: 775b 325d 5d2e 706f 735f 7d3a 7e73 6265  w[2]].pos_}:~sbe
+0000b3a0: 6122 2c20 6622 2a3a 7b64 6f63 5b72 6f77  a", f"*:{doc[row
+0000b3b0: 5b32 5d5d 2e70 6f73 5f7d 3a7e 7362 6561  [2]].pos_}:~sbea
+0000b3c0: 225d 290a 0966 6f72 2072 6f77 2069 6e20  "])..for row in 
+0000b3d0: 7665 7262 6e65 745f 6d61 7463 6865 7228  verbnet_matcher(
+0000b3e0: 646f 6329 3a20 235b 2831 2c20 302c 2033  doc): #[(1, 0, 3
+0000b3f0: 2c20 274e 5020 5620 535f 494e 4727 295d  , 'NP V S_ING')]
+0000b400: 2023 206c 6173 7420 746f 2062 6520 6361   # last to be ca
+0000b410: 6c6c 6564 2c20 7369 6e63 6520 4e50 2069  lled, since NP i
+0000b420: 7320 6d65 7267 6564 0a09 0969 6620 6c65  s merged...if le
+0000b430: 6e28 726f 7729 203d 3d20 343a 200a 0909  n(row) == 4: ...
+0000b440: 0976 6572 6269 2c20 6962 6567 2c20 6965  .verbi, ibeg, ie
+0000b450: 6e64 2c20 6368 756e 6b20 3d20 726f 770a  nd, chunk = row.
+0000b460: 0909 0969 6620 646f 635b 7665 7262 695d  ...if doc[verbi]
+0000b470: 2e6c 656d 6d61 5f2e 6973 616c 7068 6128  .lemma_.isalpha(
+0000b480: 2920 3a20 0a09 0909 0961 7272 2e61 7070  ) : .....arr.app
+0000b490: 656e 6428 6622 7b64 6f63 5b76 6572 6269  end(f"{doc[verbi
+0000b4a0: 5d2e 6c65 6d6d 615f 7d3a 7b64 6f63 5b76  ].lemma_}:{doc[v
+0000b4b0: 6572 6269 5d2e 706f 735f 7d3a 7665 7262  erbi].pos_}:verb
+0000b4c0: 6e65 743a 7b63 6875 6e6b 7d22 2920 2363  net:{chunk}") #c
+0000b4d0: 6f6e 7369 6465 723a 5645 5242 3a76 6572  onsider:VERB:ver
+0000b4e0: 626e 6574 3a4e 5020 5620 535f 494e 470a  bnet:NP V S_ING.
+0000b4f0: 0966 6f72 206e 616d 652c 6962 6567 2c69  .for name,ibeg,i
+0000b500: 656e 6420 696e 2070 6f73 745f 6e70 5f6d  end in post_np_m
+0000b510: 6174 6368 6572 2864 6f63 293a 2023 6164  atcher(doc): #ad
+0000b520: 6465 6420 3230 3232 2e37 2e32 350a 0909  ded 2022.7.25...
+0000b530: 6966 206e 616d 6520 696e 2028 2776 5f6e  if name in ('v_n
+0000b540: 5f76 626e 272c 2776 5f6e 5f61 646a 2729  _vbn','v_n_adj')
+0000b550: 3a20 0a09 0909 6172 722e 6578 7465 6e64  : ....arr.extend
+0000b560: 285b 6622 7b64 6f63 5b69 6265 675d 2e6c  ([f"{doc[ibeg].l
+0000b570: 656d 6d61 5f7d 3a7b 646f 635b 6962 6567  emma_}:{doc[ibeg
+0000b580: 5d2e 706f 735f 7d3a 7b6e 616d 657d 3a7b  ].pos_}:{name}:{
+0000b590: 646f 635b 6962 6567 5d2e 6c65 6d6d 615f  doc[ibeg].lemma_
+0000b5a0: 7d20 7b64 6f63 5b69 6265 672b 315d 2e6c  } {doc[ibeg+1].l
+0000b5b0: 656d 6d61 5f7d 207b 646f 635b 6962 6567  emma_} {doc[ibeg
+0000b5c0: 2b32 5d2e 7465 7874 7d22 2c20 6622 7b64  +2].text}", f"{d
+0000b5d0: 6f63 5b69 6265 675d 2e6c 656d 6d61 5f7d  oc[ibeg].lemma_}
+0000b5e0: 3a7b 646f 635b 6962 6567 5d2e 706f 735f  :{doc[ibeg].pos_
+0000b5f0: 7d3a 7b6e 616d 657d 222c 2066 222a 3a7b  }:{name}", f"*:{
+0000b600: 646f 635b 6962 6567 5d2e 706f 735f 7d3a  doc[ibeg].pos_}:
+0000b610: 7b6e 616d 657d 225d 290a 0972 6574 7572  {name}"])..retur
+0000b620: 6e20 6172 7220 0a0a 6973 4e50 093d 206c  n arr ..isNP.= l
+0000b630: 616d 6264 6120 743a 2074 2e65 6e74 5f74  ambda t: t.ent_t
+0000b640: 7970 655f 203d 3d20 274e 5027 2061 6e64  ype_ == 'NP' and
+0000b650: 2027 2027 2069 6e20 742e 7465 7874 2023   ' ' in t.text #
+0000b660: 206c 656e 203e 2031 200a 646f 6374 6f6b   len > 1 .doctok
+0000b670: 7320 3d20 6c61 6d62 6461 2064 6f63 3a20  s = lambda doc: 
+0000b680: 5b27 3c73 3e27 5d20 2b20 5b20 6622 5f7b  ['<s>'] + [ f"_{
+0000b690: 742e 706f 735f 7d22 2069 6620 742e 706f  t.pos_}" if t.po
+0000b6a0: 735f 2069 6e20 2827 5052 4f50 4e27 2c27  s_ in ('PROPN','
+0000b6b0: 4e55 4d27 2c27 4344 272c 2758 272c 2753  NUM','CD','X','S
+0000b6c0: 5041 4345 2729 2065 6c73 6520 225f 4e50  PACE') else "_NP
+0000b6d0: 2220 6966 2069 734e 5028 7429 2065 6c73  " if isNP(t) els
+0000b6e0: 6520 742e 7465 7874 2e6c 6f77 6572 2829  e t.text.lower()
+0000b6f0: 2020 666f 7220 7420 696e 2064 6f63 205d    for t in doc ]
+0000b700: 0a64 6566 206e 6772 616d 2874 6f6b 732c  .def ngram(toks,
+0000b710: 206e 3a69 6e74 3d33 293a 200a 0974 7320   n:int=3): ..ts 
+0000b720: 3d20 7365 7428 2920 0a09 746c 656e 203d  = set() ..tlen =
+0000b730: 2020 6c65 6e28 746f 6b73 290a 0966 6f72    len(toks)..for
+0000b740: 2069 2069 6e20 7261 6e67 6528 2074 6c65   i in range( tle
+0000b750: 6e20 293a 200a 0909 666f 7220 6a20 696e  n ): ...for j in
+0000b760: 2072 616e 6765 286e 293a 200a 0909 0969   range(n): ....i
+0000b770: 6620 692b 6a20 3c20 746c 656e 3a20 0a09  f i+j < tlen: ..
+0000b780: 0909 0974 732e 6164 6428 2022 2022 2e6a  ...ts.add( " ".j
+0000b790: 6f69 6e28 746f 6b73 5b69 3a69 2b6a 5d29  oin(toks[i:i+j])
+0000b7a0: 2029 0a09 7265 7475 726e 205b 7420 666f   )..return [t fo
+0000b7b0: 7220 7420 696e 2074 7320 6966 2074 2061  r t in ts if t a
+0000b7c0: 6e64 206e 6f74 2027 2e27 2069 6e20 745d  nd not '.' in t]
+0000b7d0: 0a0a 6465 6620 6334 6765 7428 6772 616d  ..def c4get(gram
+0000b7e0: 733a 6c69 7374 3d5b 273c 733e 2069 7327  s:list=['<s> is'
+0000b7f0: 2c27 6a75 6d70 6564 206f 7665 7220 5f4e  ,'jumped over _N
+0000b800: 5027 5d2c 206e 616d 653d 2763 3467 7261  P'], name='c4gra
+0000b810: 6d27 293a 2020 0a09 6966 206e 6f74 2068  m'):  ..if not h
+0000b820: 6173 6174 7472 2863 3467 6574 2c6e 616d  asattr(c4get,nam
+0000b830: 6529 3a20 7365 7461 7474 7228 2063 3467  e): setattr( c4g
+0000b840: 6574 2c20 6e61 6d65 2c20 7371 6c69 7465  et, name, sqlite
+0000b850: 332e 636f 6e6e 6563 7428 6622 2f64 6174  3.connect(f"/dat
+0000b860: 612f 6d6f 6465 6c2f 6334 2f7b 6e61 6d65  a/model/c4/{name
+0000b870: 7d2e 7369 222c 2063 6865 636b 5f73 616d  }.si", check_sam
+0000b880: 655f 7468 7265 6164 3d46 616c 7365 2920  e_thread=False) 
+0000b890: 2920 200a 0972 6574 7572 6e20 7b20 726f  )  ..return { ro
+0000b8a0: 775b 305d 203a 2072 6f77 5b31 5d20 666f  w[0] : row[1] fo
+0000b8b0: 7220 726f 7720 696e 2067 6574 6174 7472  r row in getattr
+0000b8c0: 2863 3467 6574 2c20 6e61 6d65 292e 6578  (c4get, name).ex
+0000b8d0: 6563 7574 6528 2273 656c 6563 7420 732c  ecute("select s,
+0000b8e0: 6920 6672 6f6d 2073 6920 7768 6572 6520  i from si where 
+0000b8f0: 7320 696e 2028 2722 2b22 272c 2722 2e6a  s in ('"+"','".j
+0000b900: 6f69 6e28 5b6b 2066 6f72 206b 2069 6e20  oin([k for k in 
+0000b910: 6772 616d 7320 6966 206e 6f74 2022 2722  grams if not "'"
+0000b920: 2069 6e20 6b5d 292b 2227 2922 2920 7d20   in k])+"')") } 
+0000b930: 0a0a 6465 6620 6e67 7261 6d5f 6368 6563  ..def ngram_chec
+0000b940: 6b28 7465 7874 3a73 7472 3d22 5468 6520  k(text:str="The 
+0000b950: 7175 6963 6b20 666f 7820 6a75 6d70 6564  quick fox jumped
+0000b960: 206f 7665 7220 7468 6520 6c61 7a79 2064   over the lazy d
+0000b970: 6f67 2e22 2c20 6e3a 696e 743d 3329 3a0a  og.", n:int=3):.
+0000b980: 0964 6f63 203d 2073 7061 6379 2e6e 6c70  .doc = spacy.nlp
+0000b990: 2874 6578 7429 0a09 6d65 7267 655f 6e70  (text)..merge_np
+0000b9a0: 2864 6f63 2920 0a09 746f 6b73 093d 2064  (doc) ..toks.= d
+0000b9b0: 6f63 746f 6b73 2864 6f63 290a 0967 7261  octoks(doc)..gra
+0000b9c0: 6d73 093d 206e 6772 616d 2874 6f6b 732c  ms.= ngram(toks,
+0000b9d0: 206e 290a 0964 6963 0909 3d20 6334 6765   n)..dic..= c4ge
+0000b9e0: 7428 6772 616d 7329 200a 0972 6574 7572  t(grams) ..retur
+0000b9f0: 6e20 5b20 7b22 6772 616d 223a 2077 2c20  n [ {"gram": w, 
+0000ba00: 2263 6e74 223a 2064 6963 2e67 6574 2877  "cnt": dic.get(w
+0000ba10: 2c30 2920 7d20 666f 7220 7720 696e 2063  ,0) } for w in c
+0000ba20: 686b 5d0a 0a64 6566 2067 7261 6d28 646f  hk]..def gram(do
+0000ba30: 632c 206e 3a69 6e74 3d37 293a 0a09 7473  c, n:int=7):..ts
+0000ba40: 203d 2073 6574 2829 200a 0964 6566 2063   = set() ..def c
+0000ba50: 6f75 6e74 2874 6f6b 732c 2074 732c 206e  ount(toks, ts, n
+0000ba60: 293a 2023 2074 733a 2073 6574 200a 0909  ): # ts: set ...
+0000ba70: 746c 656e 203d 2020 6c65 6e28 746f 6b73  tlen =  len(toks
+0000ba80: 290a 0909 666f 7220 6920 696e 2072 616e  )...for i in ran
+0000ba90: 6765 2820 746c 656e 2029 3a20 0a09 0909  ge( tlen ): ....
+0000baa0: 666f 7220 6a20 696e 2072 616e 6765 286e  for j in range(n
+0000bab0: 293a 200a 0909 0909 6966 2069 2b6a 203c  ): .....if i+j <
+0000bac0: 2074 6c65 6e3a 200a 0909 0909 0974 732e   tlen: ......ts.
+0000bad0: 6164 6428 2022 2022 2e6a 6f69 6e28 746f  add( " ".join(to
+0000bae0: 6b73 5b69 3a69 2b6a 5d29 2029 0a0a 0963  ks[i:i+j]) )...c
+0000baf0: 6f75 6e74 2820 646f 6374 6f6b 7328 646f  ount( doctoks(do
+0000bb00: 6329 2c20 7473 2c20 6e29 200a 096d 6572  c), ts, n) ..mer
+0000bb10: 6765 5f6e 7028 646f 6329 200a 0963 6f75  ge_np(doc) ..cou
+0000bb20: 6e74 2820 646f 6374 6f6b 7328 646f 6329  nt( doctoks(doc)
+0000bb30: 2c20 7473 2c20 6e29 200a 0972 6574 7572  , ts, n) ..retur
+0000bb40: 6e20 227c 222e 6a6f 696e 285b 7420 666f  n "|".join([t fo
+0000bb50: 7220 7420 696e 2074 7320 6966 2074 5d29  r t in ts if t])
+0000bb60: 0a0a 6465 6620 7371 6c63 6f6e 6e28 6f75  ..def sqlconn(ou
+0000bb70: 7466 696c 652c 2073 716c 733a 7374 723d  tfile, sqls:str=
+0000bb80: 5b22 6372 6561 7465 2074 6162 6c65 2069  ["create table i
+0000bb90: 6620 6e6f 7420 6578 6973 7473 2073 6928  f not exists si(
+0000bba0: 2073 2076 6172 6368 6172 2836 3429 206e   s varchar(64) n
+0000bbb0: 6f74 206e 756c 6c20 7072 696d 6172 7920  ot null primary 
+0000bbc0: 6b65 792c 2069 2069 6e74 206e 6f74 206e  key, i int not n
+0000bbd0: 756c 6c20 6465 6661 756c 7420 3029 2077  ull default 0) w
+0000bbe0: 6974 686f 7574 2072 6f77 6964 222c 2263  ithout rowid","c
+0000bbf0: 7265 6174 6520 7461 626c 6520 6966 206e  reate table if n
+0000bc00: 6f74 2065 7869 7374 7320 7374 2820 7320  ot exists st( s 
+0000bc10: 7661 7263 6861 7228 3634 2920 6e6f 7420  varchar(64) not 
+0000bc20: 6e75 6c6c 2070 7269 6d61 7279 206b 6579  null primary key
+0000bc30: 2c20 7420 7465 7874 2c20 636e 7420 696e  , t text, cnt in
+0000bc40: 7420 6e6f 7420 6e75 6c6c 2064 6566 6175  t not null defau
+0000bc50: 6c74 2030 2920 7769 7468 6f75 7420 726f  lt 0) without ro
+0000bc60: 7769 6422 5d29 3a0a 0963 6f6e 6e20 203d  wid"]):..conn  =
+0000bc70: 0973 716c 6974 6533 2e63 6f6e 6e65 6374  .sqlite3.connect
+0000bc80: 286f 7574 6669 6c65 2c20 6368 6563 6b5f  (outfile, check_
+0000bc90: 7361 6d65 5f74 6872 6561 643d 4661 6c73  same_thread=Fals
+0000bca0: 6529 200a 0966 6f72 2073 716c 2069 6e20  e) ..for sql in 
+0000bcb0: 7371 6c73 3a20 636f 6e6e 2e65 7865 6375  sqls: conn.execu
+0000bcc0: 7465 2873 716c 290a 0963 6f6e 6e2e 6578  te(sql)..conn.ex
+0000bcd0: 6563 7574 6528 2750 5241 474d 4120 7379  ecute('PRAGMA sy
+0000bce0: 6e63 6872 6f6e 6f75 733d 4f46 4627 290a  nchronous=OFF').
+0000bcf0: 0963 6f6e 6e2e 6578 6563 7574 6528 2750  .conn.execute('P
+0000bd00: 5241 474d 4120 6361 7365 5f73 656e 7369  RAGMA case_sensi
+0000bd10: 7469 7665 5f6c 696b 6520 3d20 3127 2920  tive_like = 1') 
+0000bd20: 2363 6f6e 6e2e 6578 6563 7574 6528 2250  #conn.execute("P
+0000bd30: 5241 474d 4120 6361 6368 655f 7369 7a65  RAGMA cache_size
+0000bd40: 203d 202d 3531 3222 2920 2009 0963 6f6e   = -512")  ..con
+0000bd50: 6e2e 6578 6563 7574 6528 2750 5241 474d  n.execute('PRAGM
+0000bd60: 4120 6361 6368 655f 7369 7a65 203d 2032  A cache_size = 2
+0000bd70: 3030 3030 3030 2729 2020 2320 3220 4762  000000')  # 2 Gb
+0000bd80: 0a09 636f 6e6e 2e63 6f6d 6d69 7428 290a  ..conn.commit().
+0000bd90: 0972 6574 7572 6e20 636f 6e6e 200a 0a64  .return conn ..d
+0000bda0: 6566 2073 716c 7369 2869 6e66 696c 652c  ef sqlsi(infile,
+0000bdb0: 2066 756e 633a 7374 723d 2774 6f6b 7472   func:str='toktr
+0000bdc0: 7027 2c20 6f75 7466 696c 653a 7374 723d  p', outfile:str=
+0000bdd0: 4e6f 6e65 2c62 6174 6368 3d31 3030 302c  None,batch=1000,
+0000bde0: 293a 2023 6962 6567 3a69 6e74 3d30 2c20  ): #ibeg:int=0, 
+0000bdf0: 6965 6e64 3a69 6e74 3d31 3030 3030 3030  iend:int=1000000
+0000be00: 2c0a 0927 2727 2064 6174 6120 666f 7220  ,..''' data for 
+0000be10: 6d79 6e61 632c 2066 756e 6320 6d75 7374  mynac, func must
+0000be20: 2065 7869 7374 202c 2066 756e 633d 7472   exist , func=tr
+0000be30: 7078 2027 2727 0a09 6966 206f 7574 6669  px '''..if outfi
+0000be40: 6c65 2069 7320 4e6f 6e65 206f 7220 6e6f  le is None or no
+0000be50: 7420 6f75 7466 696c 653a 206f 7574 6669  t outfile: outfi
+0000be60: 6c65 203d 2069 6e66 696c 652e 7370 6c69  le = infile.spli
+0000be70: 7428 272e 2729 5b30 5d20 2b20 6622 2e73  t('.')[0] + f".s
+0000be80: 716c 7369 220a 0970 7269 6e74 2866 2273  qlsi"..print(f"s
+0000be90: 7461 7274 6564 3a20 5b62 6174 6368 3d7b  tarted: [batch={
+0000bea0: 6261 7463 687d 5d22 2c20 696e 6669 6c65  batch}]", infile
+0000beb0: 2c20 6f75 7466 696c 6520 2c20 6675 6e63  , outfile , func
+0000bec0: 202c 2066 6c75 7368 3d54 7275 6529 0a09   , flush=True)..
+0000bed0: 6675 6e63 203d 2067 6c6f 6261 6c73 2829  func = globals()
+0000bee0: 5b66 756e 635d 200a 0973 7461 7274 203d  [func] ..start =
+0000bef0: 2074 696d 652e 7469 6d65 2829 0a09 636f   time.time()..co
+0000bf00: 6e6e 203d 2073 716c 636f 6e6e 286f 7574  nn = sqlconn(out
+0000bf10: 6669 6c65 2920 0a09 666f 7220 7369 642c  file) ..for sid,
+0000bf20: 206c 696e 6520 696e 2065 6e75 6d65 7261   line in enumera
+0000bf30: 7465 2866 696c 6569 6e70 7574 2e69 6e70  te(fileinput.inp
+0000bf40: 7574 2869 6e66 696c 652c 6f70 656e 686f  ut(infile,openho
+0000bf50: 6f6b 3d66 696c 6569 6e70 7574 2e68 6f6f  ok=fileinput.hoo
+0000bf60: 6b5f 636f 6d70 7265 7373 6564 2929 3a20  k_compressed)): 
+0000bf70: 0a09 0974 7279 3a20 2369 6620 7369 6420  ...try: #if sid 
+0000bf80: 3c20 6962 6567 203a 2063 6f6e 7469 6e75  < ibeg : continu
+0000bf90: 6520 7c09 6966 2073 6964 203e 3d20 6965  e |.if sid >= ie
+0000bfa0: 6e64 3a20 6272 6561 6b20 0a09 0909 6172  nd: break ....ar
+0000bfb0: 7220 3d20 6a73 6f6e 2e6c 6f61 6473 286c  r = json.loads(l
+0000bfc0: 696e 652e 7374 7269 7028 2929 200a 0909  ine.strip()) ...
+0000bfd0: 0964 6f63 203d 2073 7061 6379 2e66 726f  .doc = spacy.fro
+0000bfe0: 6d5f 6a73 6f6e 2861 7272 2920 200a 0909  m_json(arr)  ...
+0000bff0: 0966 6f72 2074 2069 6e20 646f 633a 2020  .for t in doc:  
+0000c000: 0a09 0909 0969 6620 6e6f 7420 742e 706f  .....if not t.po
+0000c010: 735f 2069 6e20 2827 5052 4f50 4e27 2c27  s_ in ('PROPN','
+0000c020: 5827 2c20 2750 554e 4354 272c 2253 5041  X', 'PUNCT',"SPA
+0000c030: 4345 222c 2752 4f4f 5427 2c27 4e55 4d27  CE",'ROOT','NUM'
+0000c040: 2920 616e 6420 6e6f 7420 742e 6865 6164  ) and not t.head
+0000c050: 2e70 6f73 5f20 696e 2028 2750 524f 504e  .pos_ in ('PROPN
+0000c060: 272c 2758 272c 2027 5055 4e43 5427 2c22  ','X', 'PUNCT',"
+0000c070: 5350 4143 4522 2c27 524f 4f54 272c 274e  SPACE",'ROOT','N
+0000c080: 554d 2729 2061 6e64 2074 2e69 735f 616c  UM') and t.is_al
+0000c090: 7068 6120 616e 6420 742e 6865 6164 2e69  pha and t.head.i
+0000c0a0: 735f 616c 7068 613a 0a09 0909 0909 7472  s_alpha:......tr
+0000c0b0: 7020 3d20 6622 7b74 2e68 6561 642e 6c65  p = f"{t.head.le
+0000c0c0: 6d6d 615f 7d3a 7b74 2e68 6561 642e 706f  mma_}:{t.head.po
+0000c0d0: 735f 7d3a 7b74 2e64 6570 5f7d 3a7b 742e  s_}:{t.dep_}:{t.
+0000c0e0: 706f 735f 7d3a 7b74 2e6c 656d 6d61 5f7d  pos_}:{t.lemma_}
+0000c0f0: 220a 0909 0909 0963 6f6e 6e2e 6578 6563  "......conn.exec
+0000c100: 7574 6528 6622 494e 5345 5254 204f 5220  ute(f"INSERT OR 
+0000c110: 4947 4e4f 5245 2049 4e54 4f20 7374 2873  IGNORE INTO st(s
+0000c120: 2c74 2920 5641 4c55 4553 283f 2c3f 2922  ,t) VALUES(?,?)"
+0000c130: 2c20 2874 7270 2c64 6f63 2e74 6578 7429  , (trp,doc.text)
+0000c140: 290a 0909 0966 6f72 2073 2069 6e20 6675  )....for s in fu
+0000c150: 6e63 2864 6f63 293a 2020 0a09 0909 0963  nc(doc):  .....c
+0000c160: 6f6e 6e2e 6578 6563 7574 6528 6622 494e  onn.execute(f"IN
+0000c170: 5345 5254 2049 4e54 4f20 7369 2873 2c69  SERT INTO si(s,i
+0000c180: 2920 5641 4c55 4553 283f 2c3f 2920 4f4e  ) VALUES(?,?) ON
+0000c190: 2043 4f4e 464c 4943 5428 7329 2044 4f20   CONFLICT(s) DO 
+0000c1a0: 5550 4441 5445 2053 4554 2069 203d 2069  UPDATE SET i = i
+0000c1b0: 202b 2031 222c 2028 732c 3129 290a 0909   + 1", (s,1))...
+0000c1c0: 0969 6620 2873 6964 2920 2520 6261 7463  .if (sid) % batc
+0000c1d0: 6820 3d3d 2030 203a 200a 0909 0909 7072  h == 0 : .....pr
+0000c1e0: 696e 7420 2866 2273 6964 203d 207b 7369  int (f"sid = {si
+0000c1f0: 647d 2c20 5c74 7c20 7573 696e 6728 7329  d}, \t| using(s)
+0000c200: 3a20 222c 2072 6f75 6e64 2874 696d 652e  : ", round(time.
+0000c210: 7469 6d65 2829 202d 2073 7461 7274 2c31  time() - start,1
+0000c220: 292c 2066 6c75 7368 3d54 7275 6529 0a09  ), flush=True)..
+0000c230: 0909 0963 6f6e 6e2e 636f 6d6d 6974 2829  ...conn.commit()
+0000c240: 2023 636f 6e6e 2e63 6c6f 7365 2829 2020   #conn.close()  
+0000c250: 2364 656c 2063 6f6e 6e09 0909 2363 6f6e  #del conn...#con
+0000c260: 6e20 3d20 7371 6c63 6f6e 6e28 6f75 7466  n = sqlconn(outf
+0000c270: 696c 6529 2009 0923 7370 6163 792e 6e6c  ile) ..#spacy.nl
+0000c280: 7009 3d20 7370 6163 792e 6c6f 6164 2827  p.= spacy.load('
+0000c290: 656e 5f63 6f72 655f 7765 625f 6c67 2729  en_core_web_lg')
+0000c2a0: 0a09 0909 0972 6566 7265 7368 2829 200a  .....refresh() .
+0000c2b0: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
+0000c2c0: 6f6e 2061 7320 653a 0a09 0909 7072 696e  on as e:....prin
+0000c2d0: 7420 2822 6578 3a22 2c20 652c 2073 6964  t ("ex:", e, sid
+0000c2e0: 2c20 6c69 6e65 2920 0a09 0909 6578 635f  , line) ....exc_
+0000c2f0: 7479 7065 2c20 6578 635f 7661 6c75 652c  type, exc_value,
+0000c300: 2065 7863 5f6f 626a 203d 2073 7973 2e65   exc_obj = sys.e
+0000c310: 7863 5f69 6e66 6f28 2920 090a 0909 0974  xc_info() .....t
+0000c320: 7261 6365 6261 636b 2e70 7269 6e74 5f74  raceback.print_t
+0000c330: 6228 6578 635f 6f62 6a29 0a09 636f 6e6e  b(exc_obj)..conn
+0000c340: 2e63 6f6d 6d69 7428 290a 0963 6f6e 6e2e  .commit()..conn.
+0000c350: 6578 6563 7574 6528 6622 7570 6461 7465  execute(f"update
+0000c360: 2073 7420 7365 7420 636e 7420 3d20 2873   st set cnt = (s
+0000c370: 656c 6563 7420 6920 6672 6f6d 2073 6920  elect i from si 
+0000c380: 7768 6572 6520 7369 2e73 203d 2073 742e  where si.s = st.
+0000c390: 7329 2229 0a09 636f 6e6e 2e63 6f6d 6d69  s)")..conn.commi
+0000c3a0: 7428 290a 0970 7269 6e74 2822 7371 6c73  t()..print("sqls
+0000c3b0: 6920 6669 6e69 7368 6564 3a22 2c20 696e  i finished:", in
+0000c3c0: 6669 6c65 290a 0a64 6566 2066 6173 7474  file)..def fastt
+0000c3d0: 6578 7428 696e 6669 6c65 2c20 6f75 7466  ext(infile, outf
+0000c3e0: 696c 653a 7374 723d 4e6f 6e65 2c62 6174  ile:str=None,bat
+0000c3f0: 6368 3d31 3030 302c 293a 200a 0927 2727  ch=1000,): ..'''
+0000c400: 2070 7265 7061 7265 2064 6174 6120 666f   prepare data fo
+0000c410: 7220 6661 7374 7465 7874 2069 6e70 7574  r fasttext input
+0000c420: 2c20 7c20 2e2f 6661 7374 7465 7874 2073  , | ./fasttext s
+0000c430: 6b69 7067 7261 6d20 2d69 6e70 7574 2064  kipgram -input d
+0000c440: 6963 2e66 6173 7474 6578 7420 2d6f 7574  ic.fasttext -out
+0000c450: 7075 7420 6469 6320 207c 3230 3233 2e31  put dic  |2023.1
+0000c460: 2e32 3620 2727 270a 0969 6620 6f75 7466  .26 '''..if outf
+0000c470: 696c 6520 6973 204e 6f6e 6520 6f72 206e  ile is None or n
+0000c480: 6f74 206f 7574 6669 6c65 3a20 6f75 7466  ot outfile: outf
+0000c490: 696c 6520 3d20 696e 6669 6c65 2e73 706c  ile = infile.spl
+0000c4a0: 6974 2827 2e27 295b 305d 202b 2066 222e  it('.')[0] + f".
+0000c4b0: 6661 7374 7465 7874 220a 0970 7269 6e74  fasttext"..print
+0000c4c0: 2866 2273 7461 7274 6564 3a20 5b62 6174  (f"started: [bat
+0000c4d0: 6368 3d7b 6261 7463 687d 5d22 2c20 696e  ch={batch}]", in
+0000c4e0: 6669 6c65 2c20 6f75 7466 696c 6520 2c20  file, outfile , 
+0000c4f0: 666c 7573 683d 5472 7565 290a 0a09 6465  flush=True)...de
+0000c500: 6620 6670 6172 7365 2864 6f63 293a 0a09  f fparse(doc):..
+0000c510: 096d 6572 6765 5f65 6e74 2864 6f63 290a  .merge_ent(doc).
+0000c520: 0909 236d 6572 6765 5f6e 7028 646f 6329  ..#merge_np(doc)
+0000c530: 2020 2320 7475 726e 5f6f 6666 2074 6865    # turn_off the
+0000c540: 2072 6164 696f 200a 0909 6d65 7267 655f   radio ...merge_
+0000c550: 7628 646f 6329 200a 0909 7265 7475 726e  v(doc) ...return
+0000c560: 2022 2022 2e6a 6f69 6e28 5b20 6622 5f7b   " ".join([ f"_{
+0000c570: 742e 706f 735f 7d22 2069 6620 742e 706f  t.pos_}" if t.po
+0000c580: 735f 2069 6e20 2822 5052 4f50 4e22 2c22  s_ in ("PROPN","
+0000c590: 4e55 4d22 2920 656c 7365 2066 227b 742e  NUM") else f"{t.
+0000c5a0: 6c65 6d6d 615f 7d2f 5645 5242 2220 6966  lemma_}/VERB" if
+0000c5b0: 2074 2e65 6e74 5f74 7970 655f 2e73 7461   t.ent_type_.sta
+0000c5c0: 7274 7377 6974 6828 226d 6572 6765 5f76  rtswith("merge_v
+0000c5d0: 3a22 2920 656c 7365 2066 225f 7b74 2e65  :") else f"_{t.e
+0000c5e0: 6e74 5f74 7970 655f 7d22 2069 6620 742e  nt_type_}" if t.
+0000c5f0: 656e 745f 7479 7065 5f20 656c 7365 2066  ent_type_ else f
+0000c600: 227b 742e 6c65 6d6d 615f 7d2f 7b74 2e70  "{t.lemma_}/{t.p
+0000c610: 6f73 5f7d 2220 6966 2074 2e70 6f73 5f20  os_}" if t.pos_ 
+0000c620: 696e 2028 2256 4552 4222 2c22 4e4f 554e  in ("VERB","NOUN
+0000c630: 222c 2022 4144 4a22 2c22 4144 5622 2920  ", "ADJ","ADV") 
+0000c640: 656c 7365 2074 2e74 6578 7420 666f 7220  else t.text for 
+0000c650: 7420 696e 2064 6f63 5d29 0a0a 0973 7461  t in doc])...sta
+0000c660: 7274 203d 2074 696d 652e 7469 6d65 2829  rt = time.time()
+0000c670: 0a09 7769 7468 206f 7065 6e28 6f75 7466  ..with open(outf
+0000c680: 696c 652c 2027 7727 2920 6173 2066 773a  ile, 'w') as fw:
+0000c690: 0a09 0966 6f72 2073 6964 2c20 6c69 6e65  ...for sid, line
+0000c6a0: 2069 6e20 656e 756d 6572 6174 6528 6669   in enumerate(fi
+0000c6b0: 6c65 696e 7075 742e 696e 7075 7428 696e  leinput.input(in
+0000c6c0: 6669 6c65 2c6f 7065 6e68 6f6f 6b3d 6669  file,openhook=fi
+0000c6d0: 6c65 696e 7075 742e 686f 6f6b 5f63 6f6d  leinput.hook_com
+0000c6e0: 7072 6573 7365 6429 293a 200a 0909 0974  pressed)): ....t
+0000c6f0: 7279 3a20 0a09 0909 0961 7272 203d 206a  ry: .....arr = j
+0000c700: 736f 6e2e 6c6f 6164 7328 6c69 6e65 2e73  son.loads(line.s
+0000c710: 7472 6970 2829 2920 0a09 0909 0964 6f63  trip()) .....doc
+0000c720: 203d 2073 7061 6379 2e66 726f 6d5f 6a73   = spacy.from_js
+0000c730: 6f6e 2861 7272 2920 200a 0909 0909 6677  on(arr)  .....fw
+0000c740: 2e77 7269 7465 2820 6670 6172 7365 2864  .write( fparse(d
+0000c750: 6f63 2920 2b20 225c 6e22 2920 0a09 0909  oc) + "\n") ....
+0000c760: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+0000c770: 2061 7320 653a 0a09 0909 0970 7269 6e74   as e:.....print
+0000c780: 2028 2265 783a 222c 2065 2c20 7369 642c   ("ex:", e, sid,
+0000c790: 206c 696e 6529 200a 0909 0909 6578 635f   line) .....exc_
+0000c7a0: 7479 7065 2c20 6578 635f 7661 6c75 652c  type, exc_value,
+0000c7b0: 2065 7863 5f6f 626a 203d 2073 7973 2e65   exc_obj = sys.e
+0000c7c0: 7863 5f69 6e66 6f28 2920 090a 0909 0909  xc_info() ......
+0000c7d0: 7472 6163 6562 6163 6b2e 7072 696e 745f  traceback.print_
+0000c7e0: 7462 2865 7863 5f6f 626a 290a 0970 7269  tb(exc_obj)..pri
+0000c7f0: 6e74 2822 6661 7374 7465 7874 2066 696e  nt("fasttext fin
+0000c800: 6973 6865 643a 222c 2069 6e66 696c 6529  ished:", infile)
+0000c810: 0a0a 6465 6620 7465 7374 2829 3a20 0a09  ..def test(): ..
+0000c820: 646f 6320 3d20 7370 6163 792e 6e6c 7028  doc = spacy.nlp(
+0000c830: 2249 7420 6973 2062 6173 6564 206f 6e20  "It is based on 
+0000c840: 7468 6520 626f 6f6b 2e22 2920 2320 2257  the book.") # "W
+0000c850: 6869 6c65 2049 2077 6173 2074 6872 696c  hile I was thril
+0000c860: 6c65 6420 7468 6174 2069 7420 7761 7320  led that it was 
+0000c870: 6f6b 2c20 4920 776f 7272 6965 6420 7468  ok, I worried th
+0000c880: 6174 2073 6865 2069 7320 6861 7070 792e  at she is happy.
+0000c890: 220a 0966 6f72 206e 616d 652c 2061 7220  "..for name, ar 
+0000c8a0: 696e 2064 6570 6d61 7463 6828 2928 646f  in depmatch()(do
+0000c8b0: 6329 203a 200a 0909 7072 696e 7428 7370  c) : ...print(sp
+0000c8c0: 6163 792e 6e6c 702e 766f 6361 625b 6e61  acy.nlp.vocab[na
+0000c8d0: 6d65 5d2e 7465 7874 2c20 646f 635b 6172  me].text, doc[ar
+0000c8e0: 5b30 5d5d 2e6c 656d 6d61 5f2c 2064 6f63  [0]].lemma_, doc
+0000c8f0: 5b61 725b 315d 5d2e 6c65 6d6d 615f 2c20  [ar[1]].lemma_, 
+0000c900: 646f 635b 6172 5b32 5d5d 290a 0970 7269  doc[ar[2]])..pri
+0000c910: 6e74 2028 2065 735f 736b 656e 7028 646f  nt ( es_skenp(do
+0000c920: 6329 2920 0a0a 6465 6620 6573 5f73 7562  c)) ..def es_sub
+0000c930: 6d69 7428 696e 6669 6c65 2c20 696e 6465  mit(infile, inde
+0000c940: 783a 7374 723d 4e6f 6e65 2c20 6261 7463  x:str=None, batc
+0000c950: 683d 3230 3030 3030 2c20 7265 6372 6561  h=200000, recrea
+0000c960: 7465 3a62 6f6f 6c3d 5472 7565 2c20 686f  te:bool=True, ho
+0000c970: 7374 3d27 3137 322e 3137 2e30 2e31 272c  st='172.17.0.1',
+0000c980: 706f 7274 3d39 3230 3029 3a20 0a09 2727  port=9200): ..''
+0000c990: 2720 7079 7468 6f6e 3320 2d6d 2061 7069  ' python3 -m api
+0000c9a0: 2e73 6e74 6a73 6f6e 2d65 7320 677a 6a63  .sntjson-es gzjc
+0000c9b0: 2e6a 736f 6e6c 672e 332e 342e 312e 677a  .jsonlg.3.4.1.gz
+0000c9c0: 2727 270a 0966 726f 6d20 656c 6173 7469  '''..from elasti
+0000c9d0: 6373 6561 7263 6820 696d 706f 7274 2045  csearch import E
+0000c9e0: 6c61 7374 6963 7365 6172 6368 2c68 656c  lasticsearch,hel
+0000c9f0: 7065 7273 0a09 696d 706f 7274 2073 6f0a  pers..import so.
+0000ca00: 0965 7309 203d 2045 6c61 7374 6963 7365  .es. = Elasticse
+0000ca10: 6172 6368 285b 2066 2268 7474 703a 2f2f  arch([ f"http://
+0000ca20: 7b68 6f73 747d 3a7b 706f 7274 7d22 205d  {host}:{port}" ]
+0000ca30: 2920 200a 0969 6620 696e 6465 7820 6973  )  ..if index is
+0000ca40: 204e 6f6e 6520 3a20 696e 6465 7820 3d20   None : index = 
+0000ca50: 696e 6669 6c65 2e73 706c 6974 2827 2e27  infile.split('.'
+0000ca60: 295b 305d 0a09 7072 696e 7428 6622 3e3e  )[0]..print(f">>
+0000ca70: 6c6f 6164 2073 7461 7274 6564 3a20 686f  load started: ho
+0000ca80: 7374 3d7b 686f 7374 7d2c 2069 6e64 6578  st={host}, index
+0000ca90: 3d7b 696e 6465 787d 2022 202c 2069 6e66  ={index} " , inf
+0000caa0: 696c 652c 2069 6e64 6578 2c20 666c 7573  ile, index, flus
+0000cab0: 683d 5472 7565 2029 0a09 6966 2072 6563  h=True )..if rec
+0000cac0: 7265 6174 6520 6f72 206e 6f74 2065 732e  reate or not es.
+0000cad0: 696e 6469 6365 732e 6578 6973 7473 2869  indices.exists(i
+0000cae0: 6e64 6578 3d69 6e64 6578 293a 200a 0909  ndex=index): ...
+0000caf0: 6966 2065 732e 696e 6469 6365 732e 6578  if es.indices.ex
+0000cb00: 6973 7473 2869 6e64 6578 3d69 6e64 6578  ists(index=index
+0000cb10: 293a 6573 2e69 6e64 6963 6573 2e64 656c  ):es.indices.del
+0000cb20: 6574 6528 696e 6465 783d 696e 6465 7829  ete(index=index)
+0000cb30: 0a09 0965 732e 696e 6469 6365 732e 6372  ...es.indices.cr
+0000cb40: 6561 7465 2869 6e64 6578 3d69 6e64 6578  eate(index=index
+0000cb50: 2c20 626f 6479 3d73 6f2e 636f 6e66 6967  , body=so.config
+0000cb60: 2920 0a0a 0961 6374 696f 6e73 3d5b 5d0a  ) ...actions=[].
+0000cb70: 0964 6566 2061 6464 2873 6f75 7263 6529  .def add(source)
+0000cb80: 3a20 200a 0909 6163 7469 6f6e 732e 6170  :  ...actions.ap
+0000cb90: 7065 6e64 2820 7b27 5f6f 705f 7479 7065  pend( {'_op_type
+0000cba0: 273a 2769 6e64 6578 272c 2027 5f69 6e64  ':'index', '_ind
+0000cbb0: 6578 273a 696e 6465 782c 2027 5f69 6427  ex':index, '_id'
+0000cbc0: 3a20 736f 7572 6365 5b27 6964 275d 2c20  : source['id'], 
+0000cbd0: 275f 736f 7572 6365 273a 2073 6f75 7263  '_source': sourc
+0000cbe0: 6520 7d20 290a 0966 6f72 2073 6964 2c20  e } )..for sid, 
+0000cbf0: 6c69 6e65 2069 6e20 656e 756d 6572 6174  line in enumerat
+0000cc00: 6528 6669 6c65 696e 7075 742e 696e 7075  e(fileinput.inpu
+0000cc10: 7428 696e 6669 6c65 2c6f 7065 6e68 6f6f  t(infile,openhoo
+0000cc20: 6b3d 6669 6c65 696e 7075 742e 686f 6f6b  k=fileinput.hook
+0000cc30: 5f63 6f6d 7072 6573 7365 6429 293a 200a  _compressed)): .
+0000cc40: 0909 7472 793a 0a09 0909 646f 6320 3d20  ..try:....doc = 
+0000cc50: 446f 6328 7370 6163 792e 6e6c 702e 766f  Doc(spacy.nlp.vo
+0000cc60: 6361 6229 2e66 726f 6d5f 6a73 6f6e 286a  cab).from_json(j
+0000cc70: 736f 6e2e 6c6f 6164 7328 6c69 6e65 2e73  son.loads(line.s
+0000cc80: 7472 6970 2829 2929 2023 2061 6464 2073  trip())) # add s
+0000cc90: 6b65 6e70 200a 0909 0966 6f72 2074 2069  kenp ....for t i
+0000cca0: 6e20 646f 633a 2009 6164 6428 7b22 7479  n doc: .add({"ty
+0000ccb0: 7065 223a 2274 6f6b 222c 2022 6964 223a  pe":"tok", "id":
+0000ccc0: 2066 227b 7369 647d 2d74 6f6b 2d7b 742e   f"{sid}-tok-{t.
+0000ccd0: 697d 222c 2022 7369 6422 3a73 6964 2c20  i}", "sid":sid, 
+0000cce0: 276c 6578 273a 742e 7465 7874 2c20 276c  'lex':t.text, 'l
+0000ccf0: 656d 273a 742e 6c65 6d6d 615f 2c20 2770  em':t.lemma_, 'p
+0000cd00: 6f73 273a 742e 706f 735f 2c20 2774 6167  os':t.pos_, 'tag
+0000cd10: 273a 742e 7461 675f 2c20 2764 6570 273a  ':t.tag_, 'dep':
+0000cd20: 742e 6465 705f 2c20 2267 706f 7322 3a74  t.dep_, "gpos":t
+0000cd30: 2e68 6561 642e 706f 735f 2c20 2267 6c65  .head.pos_, "gle
+0000cd40: 6d22 3a74 2e68 6561 642e 6c65 6d6d 615f  m":t.head.lemma_
+0000cd50: 202c 2022 6774 6167 223a 742e 6865 6164   , "gtag":t.head
+0000cd60: 2e74 6167 5f20 7d29 2023 2769 273a 742e  .tag_ }) #'i':t.
+0000cd70: 692c 2022 6865 6164 223a 742e 6865 6164  i, "head":t.head
+0000cd80: 2e69 2c0a 0909 0966 6f72 2073 7020 696e  .i,....for sp in
+0000cd90: 2064 6f63 2e6e 6f75 6e5f 6368 756e 6b73   doc.noun_chunks
+0000cda0: 3a20 090a 0909 0909 6966 2073 702e 656e  : ......if sp.en
+0000cdb0: 6420 2d20 7370 2e73 7461 7274 203e 2031  d - sp.start > 1
+0000cdc0: 3a20 2320 736b 6970 2050 524f 504e 203f  : # skip PROPN ?
+0000cdd0: 200a 0909 0909 0961 6464 287b 2274 7970   ......add({"typ
+0000cde0: 6522 3a22 6e70 222c 2022 6964 223a 2066  e":"np", "id": f
+0000cdf0: 227b 7369 647d 2d4e 502d 7b73 702e 7374  "{sid}-NP-{sp.st
+0000ce00: 6172 747d 222c 2022 7369 6422 3a73 6964  art}", "sid":sid
+0000ce10: 2c20 2763 6875 6e6b 273a 7370 2e74 6578  , 'chunk':sp.tex
+0000ce20: 742c 2027 6c65 6d27 3a64 6f63 5b73 702e  t, 'lem':doc[sp.
+0000ce30: 656e 642d 315d 2e6c 656d 6d61 5f20 7d29  end-1].lemma_ })
+0000ce40: 0a09 0909 666f 7220 6c65 6d2c 2070 6f73  ....for lem, pos
+0000ce50: 2c20 7479 7065 2c20 6368 756e 6b20 696e  , type, chunk in
+0000ce60: 206b 705f 6d61 7463 6865 7228 646f 6329   kp_matcher(doc)
+0000ce70: 3a20 2362 7269 6e6b 3a4e 4f55 4e3a 7070  : #brink:NOUN:pp
+0000ce80: 3a6f 6e20 7468 6520 6272 696e 6b20 2320  :on the brink # 
+0000ce90: 5b28 2770 7027 2c20 276f 6e20 7468 6520  [('pp', 'on the 
+0000cea0: 6272 696e 6b27 2c20 322c 2035 292c 2028  brink', 2, 5), (
+0000ceb0: 2761 7027 2c20 2776 6572 7920 6861 7070  'ap', 'very happ
+0000cec0: 7927 2c20 392c 2031 3129 5d0a 0909 0909  y', 9, 11)].....
+0000ced0: 6164 6428 7b22 7479 7065 223a 7479 7065  add({"type":type
+0000cee0: 2c20 2269 6422 3a20 6622 7b73 6964 7d2d  , "id": f"{sid}-
+0000cef0: 7b74 7970 657d 2d7b 6368 756e 6b7d 222c  {type}-{chunk}",
+0000cf00: 2022 7369 6422 3a73 6964 2c20 2027 6368   "sid":sid,  'ch
+0000cf10: 756e 6b27 3a63 6875 6e6b 2c20 276c 656d  unk':chunk, 'lem
+0000cf20: 273a 6c65 6d20 2c20 2270 6f73 223a 706f  ':lem , "pos":po
+0000cf30: 737d 2920 2322 7372 6322 3a20 646f 632e  s}) #"src": doc.
+0000cf40: 7465 7874 2c0a 0909 0966 6f72 206e 616d  text,....for nam
+0000cf50: 652c 2061 7220 696e 2064 6570 6d61 7463  e, ar in depmatc
+0000cf60: 6828 2928 646f 6329 203a 200a 0909 0909  h()(doc) : .....
+0000cf70: 7479 7065 203d 2073 7061 6379 2e6e 6c70  type = spacy.nlp
+0000cf80: 2e76 6f63 6162 5b6e 616d 655d 2e74 6578  .vocab[name].tex
+0000cf90: 7420 2320 776f 7272 7920 6265 2074 6872  t # worry be thr
+0000cfa0: 696c 6c65 640a 0909 0909 6c65 6d20 3d20  illed.....lem = 
+0000cfb0: 646f 635b 6172 5b30 5d5d 2e6c 656d 6d61  doc[ar[0]].lemma
+0000cfc0: 5f0a 0909 0909 6164 6428 7b22 7479 7065  _.....add({"type
+0000cfd0: 223a 7479 7065 2c20 2269 6422 3a20 6622  ":type, "id": f"
+0000cfe0: 7b73 6964 7d2d 7b74 7970 657d 2d7b 6c65  {sid}-{type}-{le
+0000cff0: 6d7d 222c 2022 7369 6422 3a73 6964 2c20  m}", "sid":sid, 
+0000d000: 2027 6c65 6d27 3a6c 656d 2c20 2027 7461   'lem':lem,  'ta
+0000d010: 6727 3a64 6f63 5b61 725b 305d 5d2e 7461  g':doc[ar[0]].ta
+0000d020: 675f 2c20 276c 656d 3127 3a64 6f63 5b61  g_, 'lem1':doc[a
+0000d030: 725b 315d 5d2e 6c65 6d6d 615f 2c20 276c  r[1]].lemma_, 'l
+0000d040: 656d 3227 3a64 6f63 5b61 725b 325d 5d2e  em2':doc[ar[2]].
+0000d050: 6c65 6d6d 615f 202c 2027 7461 6731 273a  lemma_ , 'tag1':
+0000d060: 646f 635b 6172 5b31 5d5d 2e74 6167 5f20  doc[ar[1]].tag_ 
+0000d070: 2c20 2774 6167 3227 3a64 6f63 5b61 725b  , 'tag2':doc[ar[
+0000d080: 325d 5d2e 7461 675f 207d 2920 0a09 0909  2]].tag_ }) ....
+0000d090: 2320 6d65 7267 6564 204e 5020 6d75 7374  # merged NP must
+0000d0a0: 2062 6520 6669 6e61 6c6c 7920 6361 6c6c   be finally call
+0000d0b0: 6564 200a 0909 0961 6464 2820 7b27 7479  ed ....add( {'ty
+0000d0c0: 7065 273a 2773 6e74 272c 2020 2269 6422  pe':'snt',  "id"
+0000d0d0: 3a73 6964 2c20 2027 736e 7427 3a64 6f63  :sid,  'snt':doc
+0000d0e0: 2e74 6578 742c 2027 706f 7374 6167 273a  .text, 'postag':
+0000d0f0: 2065 735f 706f 7374 6167 2864 6f63 292c   es_postag(doc),
+0000d100: 2027 7463 273a 206c 656e 2864 6f63 292c   'tc': len(doc),
+0000d110: 2027 736b 656e 7027 3a20 6573 5f73 6b65   'skenp': es_ske
+0000d120: 6e70 2864 6f63 2920 7d20 2029 2023 2c20  np(doc) }  ) #, 
+0000d130: 0a09 0909 6966 206c 656e 2861 6374 696f  ....if len(actio
+0000d140: 6e73 2920 3e3d 2062 6174 6368 3a20 0a09  ns) >= batch: ..
+0000d150: 0909 0968 656c 7065 7273 2e62 756c 6b28  ...helpers.bulk(
+0000d160: 636c 6965 6e74 3d65 732c 6163 7469 6f6e  client=es,action
+0000d170: 733d 6163 7469 6f6e 732c 2072 6169 7365  s=actions, raise
+0000d180: 5f6f 6e5f 6572 726f 723d 4661 6c73 6529  _on_error=False)
+0000d190: 0a09 0909 0970 7269 6e74 2028 2073 6964  .....print ( sid
+0000d1a0: 2c20 6163 7469 6f6e 735b 2d31 5d2c 2066  , actions[-1], f
+0000d1b0: 6c75 7368 3d54 7275 6529 0a09 0909 0961  lush=True).....a
+0000d1c0: 6374 696f 6e73 203d 205b 5d0a 0909 0909  ctions = [].....
+0000d1d0: 2372 6566 7265 7368 2829 2023 2032 3032  #refresh() # 202
+0000d1e0: 322e 312e 3233 200a 0909 6578 6365 7074  2.1.23 ...except
+0000d1f0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+0000d200: 0a09 0909 7072 696e 7428 2265 783a 222c  ....print("ex:",
+0000d210: 2065 2c20 7369 6429 090a 0909 0965 7863   e, sid).....exc
+0000d220: 5f74 7970 652c 2065 7863 5f76 616c 7565  _type, exc_value
+0000d230: 2c20 6578 635f 6f62 6a20 3d20 7379 732e  , exc_obj = sys.
+0000d240: 6578 635f 696e 666f 2829 2009 0a09 0909  exc_info() .....
+0000d250: 7472 6163 6562 6163 6b2e 7072 696e 745f  traceback.print_
+0000d260: 7462 2865 7863 5f6f 626a 290a 0969 6620  tb(exc_obj)..if 
+0000d270: 6163 7469 6f6e 7320 3a20 6865 6c70 6572  actions : helper
+0000d280: 732e 6275 6c6b 2863 6c69 656e 743d 6573  s.bulk(client=es
+0000d290: 2c61 6374 696f 6e73 3d61 6374 696f 6e73  ,actions=actions
+0000d2a0: 2c20 7261 6973 655f 6f6e 5f65 7272 6f72  , raise_on_error
+0000d2b0: 3d46 616c 7365 290a 0970 7269 6e74 2822  =False)..print("
+0000d2c0: 3e3e 6c6f 6164 2066 696e 6973 6865 643a  >>load finished:
+0000d2d0: 2220 2c20 696e 6669 6c65 2c20 696e 6465  " , infile, inde
+0000d2e0: 7820 290a 0a23 2076 6e70 3a6d 616b 6520  x )..# vnp:make 
+0000d2f0: 7573 6520 6f66 0a70 6f73 7461 675f 6675  use of.postag_fu
+0000d300: 6e63 5f6b 7020 3d20 7b20 2023 2064 6f63  nc_kp = {  # doc
+0000d310: 2c73 7461 7274 2c20 656e 642c 2074 6167  ,start, end, tag
+0000d320: 200a 0922 7072 6d6f 6473 223a 206c 616d   .."prmods": lam
+0000d330: 6264 6120 642c 732c 652c 7461 673a 642e  bda d,s,e,tag:d.
+0000d340: 7573 6572 5f64 6174 612e 7570 6461 7465  user_data.update
+0000d350: 287b 6622 7b74 6167 7d3a 7b64 5b73 5d2e  ({f"{tag}:{d[s].
+0000d360: 6c65 6d6d 615f 7d20 7b64 5b73 2b31 3a65  lemma_} {d[s+1:e
+0000d370: 5d2e 7465 7874 2e6c 6f77 6572 2829 7d5b  ].text.lower()}[
+0000d380: 7b73 7d2c 7b65 7d29 223a 0a09 097b 226e  {s},{e})":...{"n
+0000d390: 6163 223a 205b 645b 652d 315d 2e6c 656d  ac": [d[e-1].lem
+0000d3a0: 6d61 5f20 2b20 6622 3a56 4552 423a 7072  ma_ + f":VERB:pr
+0000d3b0: 6d6f 6473 7c22 202b 2064 5b73 5d2e 6c65  mods|" + d[s].le
+0000d3c0: 6d6d 615f 202b 2022 2022 202b 2064 5b73  mma_ + " " + d[s
+0000d3d0: 2b31 3a65 2d31 5d2e 7465 7874 2e6c 6f77  +1:e-1].text.low
+0000d3e0: 6572 2829 2c20 645b 652d 315d 2e6c 656d  er(), d[e-1].lem
+0000d3f0: 6d61 5f20 2b20 6622 3a56 4552 427c 7072  ma_ + f":VERB|pr
+0000d400: 6d6f 6473 225d 2c20 2274 6167 7322 3a20  mods"], "tags": 
+0000d410: 2720 272e 6a6f 696e 285b 742e 7461 675f  ' '.join([t.tag_
+0000d420: 2066 6f72 2074 2069 6e20 645b 733a 655d   for t in d[s:e]
+0000d430: 5d29 207d 7d29 202c 200a 0922 5650 223a  ]) }}) , .."VP":
+0000d440: 206c 616d 6264 6120 642c 732c 652c 7461   lambda d,s,e,ta
+0000d450: 673a 2064 2e75 7365 725f 6461 7461 2e75  g: d.user_data.u
+0000d460: 7064 6174 6528 7b66 227b 7461 677d 3a7b  pdate({f"{tag}:{
+0000d470: 645b 735d 2e6c 656d 6d61 5f7d 207b 645b  d[s].lemma_} {d[
+0000d480: 732b 313a 655d 2e74 6578 742e 6c6f 7765  s+1:e].text.lowe
+0000d490: 7228 297d 5b7b 737d 2c7b 657d 2922 3a0a  r()}[{s},{e})":.
+0000d4a0: 0909 7b22 6e61 6322 3a20 5b64 5b73 5d2e  ..{"nac": [d[s].
+0000d4b0: 6c65 6d6d 615f 202b 2066 223a 7b64 5b73  lemma_ + f":{d[s
+0000d4c0: 5d2e 706f 735f 7d3a 5650 7c22 202b 2064  ].pos_}:VP|" + d
+0000d4d0: 5b73 5d2e 6c65 6d6d 615f 202b 2022 2022  [s].lemma_ + " "
+0000d4e0: 202b 2064 5b73 2b31 3a65 5d2e 7465 7874   + d[s+1:e].text
+0000d4f0: 2e6c 6f77 6572 2829 2c20 645b 735d 2e6c  .lower(), d[s].l
+0000d500: 656d 6d61 5f20 2b20 6622 3a7b 645b 735d  emma_ + f":{d[s]
+0000d510: 2e70 6f73 5f7d 7c56 5022 5d2c 2020 2274  .pos_}|VP"],  "t
+0000d520: 6167 7322 3a20 2720 272e 6a6f 696e 285b  ags": ' '.join([
+0000d530: 742e 7461 675f 2066 6f72 2074 2069 6e20  t.tag_ for t in 
+0000d540: 645b 733a 655d 5d29 7d7d 2920 2c20 0a09  d[s:e]])}}) , ..
+0000d550: 2250 5022 3a20 6c61 6d62 6461 2064 2c73  "PP": lambda d,s
+0000d560: 2c65 2c74 6167 3a20 642e 7573 6572 5f64  ,e,tag: d.user_d
+0000d570: 6174 612e 7570 6461 7465 287b 6622 7b74  ata.update({f"{t
+0000d580: 6167 7d3a 7b64 5b73 5d2e 6c65 6d6d 615f  ag}:{d[s].lemma_
+0000d590: 7d20 7b64 5b73 2b31 3a65 5d2e 7465 7874  } {d[s+1:e].text
+0000d5a0: 2e6c 6f77 6572 2829 7d5b 7b73 7d2c 7b65  .lower()}[{s},{e
+0000d5b0: 7d29 223a 0a09 097b 226e 6163 223a 205b  })":...{"nac": [
+0000d5c0: 645b 652d 315d 2e6c 656d 6d61 5f20 2b20  d[e-1].lemma_ + 
+0000d5d0: 6622 3a7b 645b 652d 315d 2e70 6f73 5f7d  f":{d[e-1].pos_}
+0000d5e0: 3a50 507c 2220 2b20 645b 733a 655d 2e74  :PP|" + d[s:e].t
+0000d5f0: 6578 742e 6c6f 7765 7228 292c 2064 5b65  ext.lower(), d[e
+0000d600: 2d31 5d2e 6c65 6d6d 615f 202b 2066 223a  -1].lemma_ + f":
+0000d610: 7b64 5b65 2d31 5d2e 706f 735f 7d7c 5050  {d[e-1].pos_}|PP
+0000d620: 225d 2c20 2274 6167 7322 3a20 2720 272e  "], "tags": ' '.
+0000d630: 6a6f 696e 285b 742e 7461 675f 2066 6f72  join([t.tag_ for
+0000d640: 2074 2069 6e20 645b 733a 655d 5d29 7d7d   t in d[s:e]])}}
+0000d650: 2920 2c0a 0922 4150 223a 206c 616d 6264  ) ,.."AP": lambd
+0000d660: 6120 642c 732c 652c 7461 673a 2064 2e75  a d,s,e,tag: d.u
+0000d670: 7365 725f 6461 7461 2e75 7064 6174 6528  ser_data.update(
+0000d680: 7b66 227b 7461 677d 3a7b 645b 735d 2e6c  {f"{tag}:{d[s].l
+0000d690: 656d 6d61 5f7d 207b 645b 732b 313a 655d  emma_} {d[s+1:e]
+0000d6a0: 2e74 6578 742e 6c6f 7765 7228 297d 5b7b  .text.lower()}[{
+0000d6b0: 737d 2c7b 657d 2922 3a0a 0909 7b22 6e61  s},{e})":...{"na
+0000d6c0: 6322 3a20 5b64 5b65 2d31 5d2e 6c65 6d6d  c": [d[e-1].lemm
+0000d6d0: 615f 202b 2066 223a 7b64 5b65 2d31 5d2e  a_ + f":{d[e-1].
+0000d6e0: 706f 735f 7d3a 4150 7c22 202b 2020 645b  pos_}:AP|" +  d[
+0000d6f0: 733a 655d 2e74 6578 742c 2064 5b65 2d31  s:e].text, d[e-1
+0000d700: 5d2e 6c65 6d6d 615f 202b 2066 223a 7b64  ].lemma_ + f":{d
+0000d710: 5b65 2d31 5d2e 706f 735f 7d7c 4150 225d  [e-1].pos_}|AP"]
+0000d720: 2c20 2022 7461 6773 223a 2027 2027 2e6a  ,  "tags": ' '.j
+0000d730: 6f69 6e28 5b74 2e74 6167 5f20 666f 7220  oin([t.tag_ for 
+0000d740: 7420 696e 2064 5b73 3a65 5d5d 297d 7d29  t in d[s:e]])}})
+0000d750: 202c 0a09 2276 706e 223a 206c 616d 6264   ,.."vpn": lambd
+0000d760: 6120 642c 732c 652c 7461 673a 642e 7573  a d,s,e,tag:d.us
+0000d770: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
+0000d780: 2066 227b 7461 677d 3a7b 645b 735d 2e6c   f"{tag}:{d[s].l
+0000d790: 656d 6d61 5f7d 207b 645b 732b 313a 655d  emma_} {d[s+1:e]
+0000d7a0: 2e74 6578 742e 6c6f 7765 7228 297d 5b7b  .text.lower()}[{
+0000d7b0: 737d 2c7b 657d 2922 3a0a 0909 7b22 6e61  s},{e})":...{"na
+0000d7c0: 6322 3a20 5b66 227b 645b 735d 2e6c 656d  c": [f"{d[s].lem
+0000d7d0: 6d61 5f7d 3a56 4552 423a 7670 6e7c 7b64  ma_}:VERB:vpn|{d
+0000d7e0: 5b73 5d2e 6c65 6d6d 615f 7d20 7b64 5b73  [s].lemma_} {d[s
+0000d7f0: 2b31 3a65 5d2e 7465 7874 7d22 2c20 6622  +1:e].text}", f"
+0000d800: 7b64 5b73 5d2e 6c65 6d6d 615f 7d3a 5645  {d[s].lemma_}:VE
+0000d810: 5242 7c76 706e 222c 2066 227b 645b 735d  RB|vpn", f"{d[s]
+0000d820: 2e6c 656d 6d61 5f7d 3a56 4552 423a 7670  .lemma_}:VERB:vp
+0000d830: 6e7c 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  n|{d[s].lemma_} 
+0000d840: 7b64 5b73 2b31 5d2e 7465 7874 7d20 5f4e  {d[s+1].text} _N
+0000d850: 4f55 4e22 2c0a 0909 0909 6622 7b64 5b65  OUN",.....f"{d[e
+0000d860: 2d31 5d2e 6c65 6d6d 615f 7d3a 4e4f 554e  -1].lemma_}:NOUN
+0000d870: 3a76 706e 7c7b 645b 735d 2e6c 656d 6d61  :vpn|{d[s].lemma
+0000d880: 5f7d 207b 645b 732b 313a 655d 2e74 6578  _} {d[s+1:e].tex
+0000d890: 747d 222c 2066 227b 645b 652d 315d 2e6c  t}", f"{d[e-1].l
+0000d8a0: 656d 6d61 5f7d 3a4e 4f55 4e7c 7670 6e22  emma_}:NOUN|vpn"
+0000d8b0: 2c20 6622 7b64 5b65 2d31 5d2e 6c65 6d6d  , f"{d[e-1].lemm
+0000d8c0: 615f 7d3a 4e4f 554e 3a76 706e 7c5f 5645  a_}:NOUN:vpn|_VE
+0000d8d0: 5242 207b 645b 732b 313a 655d 2e74 6578  RB {d[s+1:e].tex
+0000d8e0: 747d 222c 200a 0909 0909 6622 7b64 5b65  t}", .....f"{d[e
+0000d8f0: 2d31 5d2e 6c65 6d6d 615f 7d2f 4e4f 554e  -1].lemma_}/NOUN
+0000d900: 7c76 706e 3a5f 7b64 5b73 5d2e 6c65 6d6d  |vpn:_{d[s].lemm
+0000d910: 615f 7d20 7b64 5b73 2b31 3a65 5d2e 7465  a_} {d[s+1:e].te
+0000d920: 7874 7d22 2c20 2023 2066 6f72 6365 2f4e  xt}",  # force/N
+0000d930: 4f55 4e7c 7670 6e3a 636f 6d65 2069 6e74  OUN|vpn:come int
+0000d940: 6f20 666f 7263 650a 0909 0909 5d7d 207d  o force.....]} }
+0000d950: 2920 2c20 2320 5f56 4552 4220 7769 7468  ) , # _VERB with
+0000d960: 2066 6f72 6365 2c20 6a75 6d70 206f 7665   force, jump ove
+0000d970: 7220 7468 6520 646f 673f 200a 0922 6270  r the dog? .."bp
+0000d980: 6e22 3a20 6c61 6d62 6461 2064 2c73 2c65  n": lambda d,s,e
+0000d990: 2c74 6167 3a64 2e75 7365 725f 6461 7461  ,tag:d.user_data
+0000d9a0: 2e75 7064 6174 6528 7b20 6622 7b74 6167  .update({ f"{tag
+0000d9b0: 7d3a 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  }:{d[s].lemma_} 
+0000d9c0: 7b64 5b73 2b31 3a65 5d2e 7465 7874 2e6c  {d[s+1:e].text.l
+0000d9d0: 6f77 6572 2829 7d5b 7b73 7d2c 7b65 7d29  ower()}[{s},{e})
+0000d9e0: 223a 0a09 097b 226e 6163 223a 205b 6622  ":...{"nac": [f"
+0000d9f0: 7b64 5b73 5d2e 6c65 6d6d 615f 7d3a 5645  {d[s].lemma_}:VE
+0000da00: 5242 3a76 706e 7c7b 645b 735d 2e6c 656d  RB:vpn|{d[s].lem
+0000da10: 6d61 5f7d 207b 645b 732b 313a 655d 2e74  ma_} {d[s+1:e].t
+0000da20: 6578 747d 222c 2066 227b 645b 735d 2e6c  ext}", f"{d[s].l
+0000da30: 656d 6d61 5f7d 3a56 4552 427c 7670 6e22  emma_}:VERB|vpn"
+0000da40: 2c20 6622 7b64 5b73 5d2e 6c65 6d6d 615f  , f"{d[s].lemma_
+0000da50: 7d3a 5645 5242 3a76 706e 7c7b 645b 735d  }:VERB:vpn|{d[s]
+0000da60: 2e6c 656d 6d61 5f7d 207b 645b 732b 315d  .lemma_} {d[s+1]
+0000da70: 2e74 6578 747d 205f 4e4f 554e 222c 0a09  .text} _NOUN",..
+0000da80: 0909 6622 7b64 5b65 2d31 5d2e 6c65 6d6d  ..f"{d[e-1].lemm
+0000da90: 615f 7d3a 4e4f 554e 3a76 706e 7c7b 645b  a_}:NOUN:vpn|{d[
+0000daa0: 735d 2e6c 656d 6d61 5f7d 207b 645b 732b  s].lemma_} {d[s+
+0000dab0: 313a 655d 2e74 6578 747d 222c 2066 227b  1:e].text}", f"{
+0000dac0: 645b 652d 315d 2e6c 656d 6d61 5f7d 3a4e  d[e-1].lemma_}:N
+0000dad0: 4f55 4e7c 7670 6e22 2c20 6622 7b64 5b65  OUN|vpn", f"{d[e
+0000dae0: 2d31 5d2e 6c65 6d6d 615f 7d3a 4e4f 554e  -1].lemma_}:NOUN
+0000daf0: 3a76 706e 7c5f 5645 5242 207b 645b 732b  :vpn|_VERB {d[s+
+0000db00: 313a 655d 2e74 6578 747d 222c 0a09 0909  1:e].text}",....
+0000db10: 6622 7b64 5b65 2d31 5d2e 6c65 6d6d 615f  f"{d[e-1].lemma_
+0000db20: 7d2f 4e4f 554e 7c76 706e 3a5f 7b64 5b73  }/NOUN|vpn:_{d[s
+0000db30: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
+0000db40: 3a65 5d2e 7465 7874 7d22 2c20 5d20 7d7d  :e].text}", ] }}
+0000db50: 2920 2c20 2320 6265 2077 6974 6820 666f  ) , # be with fo
+0000db60: 7263 652c 2062 6520 6973 2061 2056 4552  rce, be is a VER
+0000db70: 420a 0922 766e 7022 3a20 6c61 6d62 6461  B.."vnp": lambda
+0000db80: 2064 2c73 2c65 2c74 6167 3a64 2e75 7365   d,s,e,tag:d.use
+0000db90: 725f 6461 7461 2e75 7064 6174 6528 7b20  r_data.update({ 
+0000dba0: 6622 7b74 6167 7d3a 7b64 5b73 5d2e 6c65  f"{tag}:{d[s].le
+0000dbb0: 6d6d 615f 7d20 7b64 5b73 2b31 3a65 5d2e  mma_} {d[s+1:e].
+0000dbc0: 7465 7874 2e6c 6f77 6572 2829 7d5b 7b73  text.lower()}[{s
+0000dbd0: 7d2c 7b65 7d29 223a 0a09 097b 226e 6163  },{e})":...{"nac
+0000dbe0: 223a 205b 6622 7b64 5b73 5d2e 6c65 6d6d  ": [f"{d[s].lemm
+0000dbf0: 615f 7d3a 5645 5242 3a76 6e70 7c7b 645b  a_}:VERB:vnp|{d[
+0000dc00: 735d 2e6c 656d 6d61 5f7d 207b 645b 732b  s].lemma_} {d[s+
+0000dc10: 313a 655d 2e74 6578 747d 222c 2066 227b  1:e].text}", f"{
+0000dc20: 645b 735d 2e6c 656d 6d61 5f7d 3a56 4552  d[s].lemma_}:VER
+0000dc30: 427c 766e 7022 2c20 6622 7b64 5b73 5d2e  B|vnp", f"{d[s].
+0000dc40: 6c65 6d6d 615f 7d3a 5645 5242 3a76 6e70  lemma_}:VERB:vnp
+0000dc50: 7c7b 645b 735d 2e6c 656d 6d61 5f7d 205f  |{d[s].lemma_} _
+0000dc60: 4e4f 554e 207b 645b 732b 325d 2e74 6578  NOUN {d[s+2].tex
+0000dc70: 747d 222c 0a09 0909 0966 227b 645b 732b  t}",.....f"{d[s+
+0000dc80: 315d 2e6c 656d 6d61 5f7d 3a4e 4f55 4e3a  1].lemma_}:NOUN:
+0000dc90: 766e 707c 7b64 5b73 5d2e 6c65 6d6d 615f  vnp|{d[s].lemma_
+0000dca0: 7d20 7b64 5b73 2b31 3a65 5d2e 7465 7874  } {d[s+1:e].text
+0000dcb0: 7d22 2c20 6622 7b64 5b73 2b31 5d2e 6c65  }", f"{d[s+1].le
+0000dcc0: 6d6d 615f 7d3a 4e4f 554e 7c76 6e70 222c  mma_}:NOUN|vnp",
+0000dcd0: 2066 227b 645b 732b 315d 2e6c 656d 6d61   f"{d[s+1].lemma
+0000dce0: 5f7d 3a4e 4f55 4e3a 766e 707c 5f56 4552  _}:NOUN:vnp|_VER
+0000dcf0: 4220 7b64 5b73 2b31 3a65 5d2e 7465 7874  B {d[s+1:e].text
+0000dd00: 7d22 2c0a 0909 0909 6622 7b64 5b73 5d2e  }",.....f"{d[s].
+0000dd10: 6c65 6d6d 615f 7d2f 5645 5242 7c76 6e70  lemma_}/VERB|vnp
+0000dd20: 3a5f 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  :_{d[s].lemma_} 
+0000dd30: 7b64 5b73 2b31 3a65 5d2e 7465 7874 7d22  {d[s+1:e].text}"
+0000dd40: 2c5d 7d7d 2920 2c0a 0922 7670 223a 2020  ,]}}) ,.."vp":  
+0000dd50: 6c61 6d62 6461 2064 2c73 2c65 2c74 6167  lambda d,s,e,tag
+0000dd60: 3a64 2e75 7365 725f 6461 7461 2e75 7064  :d.user_data.upd
+0000dd70: 6174 6528 7b20 6622 7b74 6167 7d3a 7b64  ate({ f"{tag}:{d
+0000dd80: 5b73 5d2e 6c65 6d6d 615f 7d20 7b64 5b73  [s].lemma_} {d[s
+0000dd90: 2b31 3a65 5d2e 7465 7874 2e6c 6f77 6572  +1:e].text.lower
+0000dda0: 2829 7d5b 7b73 7d2c 7b65 7d29 223a 0a09  ()}[{s},{e})":..
+0000ddb0: 097b 226e 6163 223a 205b 6622 7b64 5b73  .{"nac": [f"{d[s
+0000ddc0: 5d2e 6c65 6d6d 615f 7d3a 5645 5242 3a76  ].lemma_}:VERB:v
+0000ddd0: 707c 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  p|{d[s].lemma_} 
+0000dde0: 7b64 5b73 2b31 5d2e 7465 7874 7d22 2c20  {d[s+1].text}", 
+0000ddf0: 6622 7b64 5b73 5d2e 6c65 6d6d 615f 7d3a  f"{d[s].lemma_}:
+0000de00: 5645 5242 7c76 7022 2c20 6622 7b64 5b73  VERB|vp", f"{d[s
+0000de10: 2b31 5d2e 6c65 6d6d 615f 7d3a 7b64 5b73  +1].lemma_}:{d[s
+0000de20: 2b31 5d2e 706f 735f 7d3a 7670 7c5f 5645  +1].pos_}:vp|_VE
+0000de30: 5242 207b 645b 732b 315d 2e74 6578 747d  RB {d[s+1].text}
+0000de40: 222c 0a09 0909 0920 6622 7b64 5b73 5d2e  ",..... f"{d[s].
+0000de50: 6c65 6d6d 615f 7d2f 5645 5242 7c76 703a  lemma_}/VERB|vp:
+0000de60: 5f7b 645b 735d 2e6c 656d 6d61 5f7d 207b  _{d[s].lemma_} {
+0000de70: 645b 732b 315d 2e74 6578 742e 6c6f 7765  d[s+1].text.lowe
+0000de80: 7228 297d 222c 095d 207d 7d29 202c 0a09  r()}",.] }}) ,..
+0000de90: 2276 7070 223a 206c 616d 6264 6120 642c  "vpp": lambda d,
+0000dea0: 732c 652c 7461 673a 642e 7573 6572 5f64  s,e,tag:d.user_d
+0000deb0: 6174 612e 7570 6461 7465 287b 2066 227b  ata.update({ f"{
+0000dec0: 7461 677d 3a7b 645b 735d 2e6c 656d 6d61  tag}:{d[s].lemma
+0000ded0: 5f7d 207b 645b 732b 313a 655d 2e74 6578  _} {d[s+1:e].tex
+0000dee0: 742e 6c6f 7765 7228 297d 5b7b 737d 2c7b  t.lower()}[{s},{
+0000def0: 657d 2922 3a0a 0909 7b22 6e61 6322 3a20  e})":...{"nac": 
+0000df00: 5b66 227b 645b 735d 2e6c 656d 6d61 5f7d  [f"{d[s].lemma_}
+0000df10: 3a56 4552 423a 7670 707c 7b64 5b73 5d2e  :VERB:vpp|{d[s].
+0000df20: 6c65 6d6d 615f 7d20 7b64 5b73 2b31 3a65  lemma_} {d[s+1:e
+0000df30: 5d2e 7465 7874 7d22 2c20 6622 7b64 5b73  ].text}", f"{d[s
+0000df40: 5d2e 6c65 6d6d 615f 7d3a 5645 5242 7c76  ].lemma_}:VERB|v
+0000df50: 7070 220a 0909 0909 2066 227b 645b 735d  pp"..... f"{d[s]
+0000df60: 2e6c 656d 6d61 5f7d 2f56 4552 427c 7670  .lemma_}/VERB|vp
+0000df70: 703a 5f7b 645b 735d 2e6c 656d 6d61 5f7d  p:_{d[s].lemma_}
+0000df80: 207b 645b 732b 313a 655d 2e74 6578 747d   {d[s+1:e].text}
+0000df90: 222c 205d 207d 7d29 202c 0a09 2276 7067  ", ] }}) ,.."vpg
+0000dfa0: 223a 206c 616d 6264 6120 642c 732c 652c  ": lambda d,s,e,
+0000dfb0: 7461 673a 642e 7573 6572 5f64 6174 612e  tag:d.user_data.
+0000dfc0: 7570 6461 7465 287b 2066 227b 7461 677d  update({ f"{tag}
+0000dfd0: 3a7b 645b 735d 2e6c 656d 6d61 5f7d 207b  :{d[s].lemma_} {
+0000dfe0: 645b 732b 313a 655d 2e74 6578 742e 6c6f  d[s+1:e].text.lo
+0000dff0: 7765 7228 297d 5b7b 737d 2c7b 657d 2922  wer()}[{s},{e})"
+0000e000: 3a0a 0909 7b22 6e61 6322 3a20 5b66 227b  :...{"nac": [f"{
+0000e010: 645b 735d 2e6c 656d 6d61 5f7d 3a56 4552  d[s].lemma_}:VER
+0000e020: 423a 7670 677c 7b64 5b73 5d2e 6c65 6d6d  B:vpg|{d[s].lemm
+0000e030: 615f 7d20 7b64 5b73 2b31 5d2e 7465 7874  a_} {d[s+1].text
+0000e040: 7d22 2c20 6622 7b64 5b73 5d2e 6c65 6d6d  }", f"{d[s].lemm
+0000e050: 615f 7d3a 5645 5242 7c76 7067 222c 2066  a_}:VERB|vpg", f
+0000e060: 227b 645b 735d 2e6c 656d 6d61 5f7d 3a56  "{d[s].lemma_}:V
+0000e070: 4552 423a 7670 677c 5f7b 645b 735d 2e6c  ERB:vpg|_{d[s].l
+0000e080: 656d 6d61 5f7d 207b 645b 732b 315d 2e74  emma_} {d[s+1].t
+0000e090: 6578 747d 205f 5642 4722 2c20 0a09 0909  ext} _VBG", ....
+0000e0a0: 6622 7b64 5b73 5d2e 6c65 6d6d 615f 7d2f  f"{d[s].lemma_}/
+0000e0b0: 5645 5242 7c76 7067 3a5f 7b64 5b73 5d2e  VERB|vpg:_{d[s].
+0000e0c0: 6c65 6d6d 615f 7d20 7b64 5b73 2b31 5d2e  lemma_} {d[s+1].
+0000e0d0: 7465 7874 7d20 5f56 4247 225d 207d 7d29  text} _VBG"] }})
+0000e0e0: 202c 0a09 2270 6e22 3a20 206c 616d 6264   ,.."pn":  lambd
+0000e0f0: 6120 642c 732c 652c 7461 673a 642e 7573  a d,s,e,tag:d.us
+0000e100: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
+0000e110: 2066 227b 7461 677d 3a7b 645b 735d 2e6c   f"{tag}:{d[s].l
+0000e120: 656d 6d61 5f7d 207b 645b 732b 313a 655d  emma_} {d[s+1:e]
+0000e130: 2e74 6578 742e 6c6f 7765 7228 297d 5b7b  .text.lower()}[{
+0000e140: 737d 2c7b 657d 2922 3a0a 0909 7b22 6e61  s},{e})":...{"na
+0000e150: 6322 3a20 5b66 227b 645b 732b 315d 2e6c  c": [f"{d[s+1].l
+0000e160: 656d 6d61 5f7d 3a4e 4f55 4e3a 706e 7c7b  emma_}:NOUN:pn|{
+0000e170: 645b 733a 655d 2e74 6578 742e 6c6f 7765  d[s:e].text.lowe
+0000e180: 7228 297d 222c 2066 227b 645b 732b 315d  r()}", f"{d[s+1]
+0000e190: 2e6c 656d 6d61 5f7d 3a4e 4f55 4e7c 706e  .lemma_}:NOUN|pn
+0000e1a0: 222c 0a09 0909 6622 7b64 5b73 2b31 5d2e  ",....f"{d[s+1].
+0000e1b0: 6c65 6d6d 615f 7d2f 4e4f 554e 7c70 6e3a  lemma_}/NOUN|pn:
+0000e1c0: 7b64 5b73 3a65 5d2e 7465 7874 2e6c 6f77  {d[s:e].text.low
+0000e1d0: 6572 2829 7d22 2c20 5d20 7d7d 2920 2c0a  er()}", ] }}) ,.
+0000e1e0: 0922 706e 7022 3a20 6c61 6d62 6461 2064  ."pnp": lambda d
+0000e1f0: 2c73 2c65 2c74 6167 3a64 2e75 7365 725f  ,s,e,tag:d.user_
+0000e200: 6461 7461 2e75 7064 6174 6528 7b20 6622  data.update({ f"
+0000e210: 7b74 6167 7d3a 7b64 5b73 5d2e 6c65 6d6d  {tag}:{d[s].lemm
+0000e220: 615f 7d20 7b64 5b73 2b31 3a65 5d2e 7465  a_} {d[s+1:e].te
+0000e230: 7874 2e6c 6f77 6572 2829 7d5b 7b73 7d2c  xt.lower()}[{s},
+0000e240: 7b65 7d29 223a 0a09 097b 226e 6163 223a  {e})":...{"nac":
+0000e250: 205b 6622 7b64 5b73 2b31 5d2e 6c65 6d6d   [f"{d[s+1].lemm
+0000e260: 615f 7d3a 4e4f 554e 3a70 6e70 7c7b 645b  a_}:NOUN:pnp|{d[
+0000e270: 733a 655d 2e74 6578 742e 6c6f 7765 7228  s:e].text.lower(
+0000e280: 297d 222c 2066 227b 645b 732b 315d 2e6c  )}", f"{d[s+1].l
+0000e290: 656d 6d61 5f7d 3a4e 4f55 4e3a 706e 7022  emma_}:NOUN:pnp"
+0000e2a0: 2c0a 0909 0966 227b 645b 732b 315d 2e6c  ,....f"{d[s+1].l
+0000e2b0: 656d 6d61 5f7d 2f4e 4f55 4e7c 706e 703a  emma_}/NOUN|pnp:
+0000e2c0: 7b64 5b73 3a65 5d2e 7465 7874 2e6c 6f77  {d[s:e].text.low
+0000e2d0: 6572 2829 7d22 2c5d 207d 7d29 202c 0a09  er()}",] }}) ,..
+0000e2e0: 2262 6170 7622 3a20 6c61 6d62 6461 2064  "bapv": lambda d
+0000e2f0: 2c73 2c65 2c74 6167 3a64 2e75 7365 725f  ,s,e,tag:d.user_
+0000e300: 6461 7461 2e75 7064 6174 6528 7b20 6622  data.update({ f"
+0000e310: 7b74 6167 7d3a 7b64 5b73 5d2e 6c65 6d6d  {tag}:{d[s].lemm
+0000e320: 615f 7d20 7b64 5b73 2b31 3a65 5d2e 7465  a_} {d[s+1:e].te
+0000e330: 7874 2e6c 6f77 6572 2829 7d5b 7b73 7d2c  xt.lower()}[{s},
+0000e340: 7b65 7d29 223a 0a09 097b 226e 6163 223a  {e})":...{"nac":
+0000e350: 205b 6622 7b64 5b73 2b31 5d2e 6c65 6d6d   [f"{d[s+1].lemm
+0000e360: 615f 7d3a 4144 4a3a 6261 7076 7c7b 645b  a_}:ADJ:bapv|{d[
+0000e370: 735d 2e6c 656d 6d61 5f7d 207b 645b 732b  s].lemma_} {d[s+
+0000e380: 313a 655d 2e74 6578 747d 222c 2066 227b  1:e].text}", f"{
+0000e390: 645b 732b 315d 2e6c 656d 6d61 5f7d 3a41  d[s+1].lemma_}:A
+0000e3a0: 444a 7c62 6170 7622 2c20 6622 7b64 5b73  DJ|bapv", f"{d[s
+0000e3b0: 2b31 5d2e 6c65 6d6d 615f 7d3a 4144 4a3a  +1].lemma_}:ADJ:
+0000e3c0: 6261 7076 7c5f 7b64 5b73 5d2e 6c65 6d6d  bapv|_{d[s].lemm
+0000e3d0: 615f 7d20 7b64 5b73 2b31 3a65 2d31 5d2e  a_} {d[s+1:e-1].
+0000e3e0: 7465 7874 7d20 5f56 4552 4222 5d7d 7d29  text} _VERB"]}})
+0000e3f0: 202c 2020 0a09 2262 6174 7622 3a20 6c61   ,  .."batv": la
+0000e400: 6d62 6461 2064 2c73 2c65 2c74 6167 3a64  mbda d,s,e,tag:d
+0000e410: 2e75 7365 725f 6461 7461 2e75 7064 6174  .user_data.updat
+0000e420: 6528 7b20 6622 7b74 6167 7d3a 7b64 5b73  e({ f"{tag}:{d[s
+0000e430: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
+0000e440: 3a65 5d2e 7465 7874 2e6c 6f77 6572 2829  :e].text.lower()
+0000e450: 7d5b 7b73 7d2c 7b65 7d29 223a 0a09 097b  }[{s},{e})":...{
+0000e460: 226e 6163 223a 205b 6622 7b64 5b73 2b31  "nac": [f"{d[s+1
+0000e470: 5d2e 6c65 6d6d 615f 7d3a 4144 4a3a 6261  ].lemma_}:ADJ:ba
+0000e480: 7476 7c7b 645b 735d 2e6c 656d 6d61 5f7d  tv|{d[s].lemma_}
+0000e490: 207b 645b 732b 313a 655d 2e74 6578 747d   {d[s+1:e].text}
+0000e4a0: 222c 2066 227b 645b 732b 315d 2e6c 656d  ", f"{d[s+1].lem
+0000e4b0: 6d61 5f7d 3a41 444a 7c62 6174 7622 2c20  ma_}:ADJ|batv", 
+0000e4c0: 6622 7b64 5b73 2b31 5d2e 6c65 6d6d 615f  f"{d[s+1].lemma_
+0000e4d0: 7d3a 4144 4a3a 6261 7476 7c5f 7b64 5b73  }:ADJ:batv|_{d[s
+0000e4e0: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
+0000e4f0: 3a65 2d31 5d2e 7465 7874 7d20 5f56 4552  :e-1].text} _VER
+0000e500: 4222 5d7d 7d29 202c 2020 0a09 2262 6570  B"]}}) ,  .."bep
+0000e510: 7622 3a20 6c61 6d62 6461 2064 2c73 2c65  v": lambda d,s,e
+0000e520: 2c74 6167 3a64 2e75 7365 725f 6461 7461  ,tag:d.user_data
+0000e530: 2e75 7064 6174 6528 7b20 6622 7b74 6167  .update({ f"{tag
+0000e540: 7d3a 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  }:{d[s].lemma_} 
+0000e550: 7b64 5b73 2b31 3a65 5d2e 7465 7874 2e6c  {d[s+1:e].text.l
+0000e560: 6f77 6572 2829 7d5b 7b73 7d2c 7b65 7d29  ower()}[{s},{e})
+0000e570: 223a 0a09 097b 226e 6163 223a 205b 6622  ":...{"nac": [f"
+0000e580: 7b64 5b73 2b31 5d2e 6c65 6d6d 615f 7d3a  {d[s+1].lemma_}:
+0000e590: 5645 5242 3a62 6570 767c 7b64 5b73 5d2e  VERB:bepv|{d[s].
+0000e5a0: 6c65 6d6d 615f 7d20 7b64 5b73 2b31 3a65  lemma_} {d[s+1:e
+0000e5b0: 5d2e 7465 7874 7d22 2c66 227b 645b 732b  ].text}",f"{d[s+
+0000e5c0: 315d 2e6c 656d 6d61 5f7d 3a56 4552 427c  1].lemma_}:VERB|
+0000e5d0: 6265 7076 222c 2066 227b 645b 732b 315d  bepv", f"{d[s+1]
+0000e5e0: 2e6c 656d 6d61 5f7d 3a56 4552 423a 6265  .lemma_}:VERB:be
+0000e5f0: 7076 7c5f 6265 207b 645b 732b 313a 652d  pv|_be {d[s+1:e-
+0000e600: 315d 2e74 6578 747d 205f 5645 5242 222c  1].text} _VERB",
+0000e610: 0a09 0909 6622 7b64 5b73 2b31 5d2e 6c65  ....f"{d[s+1].le
+0000e620: 6d6d 615f 7d2f 5645 5242 7c62 6570 763a  mma_}/VERB|bepv:
+0000e630: 5f7b 645b 735d 2e6c 656d 6d61 5f7d 207b  _{d[s].lemma_} {
+0000e640: 645b 732b 313a 652d 315d 2e74 6578 747d  d[s+1:e-1].text}
+0000e650: 205f 7b64 5b65 2d31 5d2e 7461 675f 7d22   _{d[e-1].tag_}"
+0000e660: 2c5d 7d7d 2920 2c20 2320 5f62 6520 666f  ,]}}) , # _be fo
+0000e670: 7263 6564 2074 6f20 5f56 4552 420a 0922  rced to _VERB.."
+0000e680: 6265 7476 223a 206c 616d 6264 6120 642c  betv": lambda d,
+0000e690: 732c 652c 7461 673a 642e 7573 6572 5f64  s,e,tag:d.user_d
+0000e6a0: 6174 612e 7570 6461 7465 287b 2066 227b  ata.update({ f"{
+0000e6b0: 7461 677d 3a7b 645b 735d 2e6c 656d 6d61  tag}:{d[s].lemma
+0000e6c0: 5f7d 207b 645b 732b 313a 655d 2e74 6578  _} {d[s+1:e].tex
+0000e6d0: 742e 6c6f 7765 7228 297d 5b7b 737d 2c7b  t.lower()}[{s},{
+0000e6e0: 657d 2922 3a0a 0909 7b22 6e61 6322 3a20  e})":...{"nac": 
+0000e6f0: 5b66 227b 645b 732b 315d 2e6c 656d 6d61  [f"{d[s+1].lemma
+0000e700: 5f7d 3a56 4552 423a 6265 7476 7c7b 645b  _}:VERB:betv|{d[
+0000e710: 735d 2e6c 656d 6d61 5f7d 207b 645b 732b  s].lemma_} {d[s+
+0000e720: 313a 655d 2e74 6578 747d 222c 6622 7b64  1:e].text}",f"{d
+0000e730: 5b73 2b31 5d2e 6c65 6d6d 615f 7d3a 5645  [s+1].lemma_}:VE
+0000e740: 5242 7c62 6574 7622 2c20 6622 7b64 5b73  RB|betv", f"{d[s
+0000e750: 2b31 5d2e 6c65 6d6d 615f 7d3a 5645 5242  +1].lemma_}:VERB
+0000e760: 3a62 6574 767c 5f62 6520 7b64 5b73 2b31  :betv|_be {d[s+1
+0000e770: 3a65 2d31 5d2e 7465 7874 7d20 5f56 4552  :e-1].text} _VER
+0000e780: 4222 2c0a 0909 2020 2020 2066 227b 645b  B",...     f"{d[
+0000e790: 732b 315d 2e6c 656d 6d61 5f7d 2f56 4552  s+1].lemma_}/VER
+0000e7a0: 427c 6265 7476 3a5f 7b64 5b73 5d2e 6c65  B|betv:_{d[s].le
+0000e7b0: 6d6d 615f 7d20 7b64 5b73 2b31 3a65 2d31  mma_} {d[s+1:e-1
+0000e7c0: 5d2e 7465 7874 7d20 5f7b 645b 652d 315d  ].text} _{d[e-1]
+0000e7d0: 2e74 6167 5f7d 222c 5d7d 7d29 202c 2023  .tag_}",]}}) , #
+0000e7e0: 205f 6265 2066 6f72 6365 6420 746f 205f   _be forced to _
+0000e7f0: 5645 5242 0a09 2262 6170 223a 206c 616d  VERB.."bap": lam
+0000e800: 6264 6120 642c 732c 652c 7461 673a 642e  bda d,s,e,tag:d.
+0000e810: 7573 6572 5f64 6174 612e 7570 6461 7465  user_data.update
+0000e820: 287b 2066 227b 7461 677d 3a7b 645b 735d  ({ f"{tag}:{d[s]
+0000e830: 2e6c 656d 6d61 5f7d 207b 645b 732b 313a  .lemma_} {d[s+1:
+0000e840: 655d 2e74 6578 742e 6c6f 7765 7228 297d  e].text.lower()}
+0000e850: 5b7b 737d 2c7b 657d 2922 3a0a 0909 7b22  [{s},{e})":...{"
+0000e860: 6e61 6322 3a20 5b66 227b 645b 732b 315d  nac": [f"{d[s+1]
+0000e870: 2e6c 656d 6d61 5f7d 3a41 444a 3a62 6170  .lemma_}:ADJ:bap
+0000e880: 7c7b 645b 735d 2e6c 656d 6d61 5f7d 207b  |{d[s].lemma_} {
+0000e890: 645b 732b 313a 655d 2e74 6578 747d 222c  d[s+1:e].text}",
+0000e8a0: 2066 227b 645b 732b 315d 2e6c 656d 6d61   f"{d[s+1].lemma
+0000e8b0: 5f7d 3a41 444a 7c62 6170 222c 0a09 0909  _}:ADJ|bap",....
+0000e8c0: 0966 227b 645b 732b 315d 2e6c 656d 6d61  .f"{d[s+1].lemma
+0000e8d0: 5f7d 2f41 444a 7c62 6170 3a5f 7b64 5b73  _}/ADJ|bap:_{d[s
+0000e8e0: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
+0000e8f0: 3a65 5d2e 7465 7874 7d22 2c5d 7d7d 2920  :e].text}",]}}) 
+0000e900: 2c0a 0922 6265 7022 3a20 6c61 6d62 6461  ,.."bep": lambda
+0000e910: 2064 2c73 2c65 2c74 6167 3a64 2e75 7365   d,s,e,tag:d.use
+0000e920: 725f 6461 7461 2e75 7064 6174 6528 7b20  r_data.update({ 
+0000e930: 6622 7b74 6167 7d3a 7b64 5b73 5d2e 6c65  f"{tag}:{d[s].le
+0000e940: 6d6d 615f 7d20 7b64 5b73 2b31 3a65 5d2e  mma_} {d[s+1:e].
+0000e950: 7465 7874 2e6c 6f77 6572 2829 7d5b 7b73  text.lower()}[{s
+0000e960: 7d2c 7b65 7d29 223a 0a09 097b 226e 6163  },{e})":...{"nac
+0000e970: 223a 205b 6622 7b64 5b73 2b31 5d2e 6c65  ": [f"{d[s+1].le
+0000e980: 6d6d 615f 7d3a 5645 5242 3a62 6570 7c7b  mma_}:VERB:bep|{
+0000e990: 645b 735d 2e6c 656d 6d61 5f7d 207b 645b  d[s].lemma_} {d[
+0000e9a0: 732b 313a 655d 2e74 6578 747d 222c 2066  s+1:e].text}", f
+0000e9b0: 227b 645b 732b 315d 2e6c 656d 6d61 5f7d  "{d[s+1].lemma_}
+0000e9c0: 3a56 4552 427c 6265 7022 2c0a 0909 0909  :VERB|bep",.....
+0000e9d0: 6622 7b64 5b73 2b31 5d2e 6c65 6d6d 615f  f"{d[s+1].lemma_
+0000e9e0: 7d2f 5645 5242 7c62 6570 3a5f 7b64 5b73  }/VERB|bep:_{d[s
+0000e9f0: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
+0000ea00: 3a65 5d2e 7465 7874 7d22 2c5d 7d7d 2920  :e].text}",]}}) 
+0000ea10: 2c0a 0922 766f 7022 3a20 6c61 6d62 6461  ,.."vop": lambda
+0000ea20: 2064 2c73 2c65 2c74 6167 3a64 2e75 7365   d,s,e,tag:d.use
+0000ea30: 725f 6461 7461 2e75 7064 6174 6528 7b20  r_data.update({ 
+0000ea40: 6622 7b74 6167 7d3a 7b64 5b73 5d2e 6c65  f"{tag}:{d[s].le
+0000ea50: 6d6d 615f 7d20 7b64 5b73 2b31 3a65 5d2e  mma_} {d[s+1:e].
+0000ea60: 7465 7874 2e6c 6f77 6572 2829 7d5b 7b73  text.lower()}[{s
+0000ea70: 7d2c 7b65 7d29 223a 0a09 097b 226e 6163  },{e})":...{"nac
+0000ea80: 223a 205b 6622 7b64 5b73 5d2e 6c65 6d6d  ": [f"{d[s].lemm
+0000ea90: 615f 7d3a 5645 5242 3a76 6f70 7c7b 645b  a_}:VERB:vop|{d[
+0000eaa0: 735d 2e6c 656d 6d61 5f7d 206f 6e65 7365  s].lemma_} onese
+0000eab0: 6c66 207b 645b 652d 315d 2e74 6578 747d  lf {d[e-1].text}
+0000eac0: 222c 2066 227b 645b 735d 2e6c 656d 6d61  ", f"{d[s].lemma
+0000ead0: 5f7d 3a56 4552 427c 766f 7022 2c20 2066  _}:VERB|vop",  f
+0000eae0: 227b 645b 735d 2e6c 656d 6d61 5f7d 3a56  "{d[s].lemma_}:V
+0000eaf0: 4552 423a 766f 707c 5f7b 645b 735d 2e6c  ERB:vop|_{d[s].l
+0000eb00: 656d 6d61 5f7d 205f 6f6e 6573 656c 6620  emma_} _oneself 
+0000eb10: 7b64 5b65 2d31 5d2e 7465 7874 7d22 2c0a  {d[e-1].text}",.
+0000eb20: 0909 0966 227b 645b 735d 2e6c 656d 6d61  ...f"{d[s].lemma
+0000eb30: 5f7d 2f56 4552 427c 766f 703a 5f7b 645b  _}/VERB|vop:_{d[
+0000eb40: 735d 2e6c 656d 6d61 5f7d 205f 6f6e 6573  s].lemma_} _ones
+0000eb50: 656c 6620 7b64 5b65 2d31 5d2e 7465 7874  elf {d[e-1].text
+0000eb60: 2e6c 6f77 6572 2829 7d22 2c5d 7d7d 2920  .lower()}",]}}) 
+0000eb70: 2c0a 0922 7674 7622 3a20 6c61 6d62 6461  ,.."vtv": lambda
+0000eb80: 2064 2c73 2c65 2c74 6167 3a64 2e75 7365   d,s,e,tag:d.use
+0000eb90: 725f 6461 7461 2e75 7064 6174 6528 7b20  r_data.update({ 
+0000eba0: 6622 7b74 6167 7d3a 7b64 5b73 5d2e 6c65  f"{tag}:{d[s].le
+0000ebb0: 6d6d 615f 7d20 7b64 5b73 2b31 3a65 5d2e  mma_} {d[s+1:e].
+0000ebc0: 7465 7874 2e6c 6f77 6572 2829 7d5b 7b73  text.lower()}[{s
+0000ebd0: 7d2c 7b65 7d29 223a 0a09 097b 226e 6163  },{e})":...{"nac
+0000ebe0: 223a 205b 6622 7b64 5b73 5d2e 6c65 6d6d  ": [f"{d[s].lemm
+0000ebf0: 615f 7d3a 5645 5242 3a76 7476 7c7b 645b  a_}:VERB:vtv|{d[
+0000ec00: 735d 2e6c 656d 6d61 5f7d 207b 645b 732b  s].lemma_} {d[s+
+0000ec10: 313a 655d 2e74 6578 747d 222c 2066 227b  1:e].text}", f"{
+0000ec20: 645b 735d 2e6c 656d 6d61 5f7d 3a56 4552  d[s].lemma_}:VER
+0000ec30: 423a 7674 767c 5f7b 645b 735d 2e6c 656d  B:vtv|_{d[s].lem
+0000ec40: 6d61 5f7d 207b 645b 732b 313a 652d 315d  ma_} {d[s+1:e-1]
+0000ec50: 2e74 6578 747d 205f 5645 5242 222c 2066  .text} _VERB", f
+0000ec60: 227b 645b 735d 2e6c 656d 6d61 5f7d 3a56  "{d[s].lemma_}:V
+0000ec70: 4552 427c 7674 7622 2c20 6622 7b64 5b65  ERB|vtv", f"{d[e
+0000ec80: 2d31 5d2e 6c65 6d6d 615f 7d3a 5645 5242  -1].lemma_}:VERB
+0000ec90: 7c7e 7674 7622 2c20 6622 7b64 5b65 2d31  |~vtv", f"{d[e-1
+0000eca0: 5d2e 6c65 6d6d 615f 7d3a 5645 5242 3a7e  ].lemma_}:VERB:~
+0000ecb0: 7674 767c 7b64 5b73 5d2e 6c65 6d6d 615f  vtv|{d[s].lemma_
+0000ecc0: 7d22 2c0a 0909 0966 227b 645b 735d 2e6c  }",....f"{d[s].l
+0000ecd0: 656d 6d61 5f7d 2f56 4552 427c 7674 763a  emma_}/VERB|vtv:
+0000ece0: 5f7b 645b 735d 2e6c 656d 6d61 5f7d 2074  _{d[s].lemma_} t
+0000ecf0: 6f20 5f7b 645b 652d 315d 2e74 6167 5f7d  o _{d[e-1].tag_}
+0000ed00: 222c 5d7d 7d20 2920 2c0a 0922 7667 223a  ",]}} ) ,.."vg":
+0000ed10: 206c 616d 6264 6120 642c 732c 652c 7461   lambda d,s,e,ta
+0000ed20: 673a 2064 2e75 7365 725f 6461 7461 2e75  g: d.user_data.u
+0000ed30: 7064 6174 6528 7b20 6622 7b74 6167 7d3a  pdate({ f"{tag}:
+0000ed40: 7b64 5b73 5d2e 6c65 6d6d 615f 7d20 7b64  {d[s].lemma_} {d
+0000ed50: 5b73 2b31 3a65 5d2e 7465 7874 2e6c 6f77  [s+1:e].text.low
+0000ed60: 6572 2829 7d5b 7b73 7d2c 7b65 7d29 223a  er()}[{s},{e})":
+0000ed70: 0a09 097b 226e 6163 223a 205b 6622 7b64  ...{"nac": [f"{d
+0000ed80: 5b73 5d2e 6c65 6d6d 615f 7d3a 5645 5242  [s].lemma_}:VERB
+0000ed90: 3a76 677c 7b64 5b73 5d2e 6c65 6d6d 615f  :vg|{d[s].lemma_
+0000eda0: 7d20 7b64 5b65 2d31 5d2e 7465 7874 7d22  } {d[e-1].text}"
+0000edb0: 2c20 6622 7b64 5b73 5d2e 6c65 6d6d 615f  , f"{d[s].lemma_
+0000edc0: 7d3a 5645 5242 3a76 677c 5f7b 645b 735d  }:VERB:vg|_{d[s]
+0000edd0: 2e6c 656d 6d61 5f7d 205f 5642 4722 2c20  .lemma_} _VBG", 
+0000ede0: 6622 7b64 5b73 5d2e 6c65 6d6d 615f 7d3a  f"{d[s].lemma_}:
+0000edf0: 5645 5242 7c76 6722 2c20 6622 7b64 5b65  VERB|vg", f"{d[e
+0000ee00: 2d31 5d2e 6c65 6d6d 615f 7d3a 5645 5242  -1].lemma_}:VERB
+0000ee10: 7c7e 7667 222c 2066 227b 645b 652d 315d  |~vg", f"{d[e-1]
+0000ee20: 2e6c 656d 6d61 5f7d 3a56 4552 423a 7e76  .lemma_}:VERB:~v
+0000ee30: 677c 7b64 5b73 5d2e 6c65 6d6d 615f 7d22  g|{d[s].lemma_}"
+0000ee40: 2c0a 0909 0909 6622 7b64 5b73 5d2e 6c65  ,.....f"{d[s].le
+0000ee50: 6d6d 615f 7d2f 5645 5242 7c76 673a 5f7b  mma_}/VERB|vg:_{
+0000ee60: 645b 735d 2e6c 656d 6d61 5f7d 205f 7b64  d[s].lemma_} _{d
+0000ee70: 5b65 2d31 5d2e 7461 675f 7d22 2c5d 7d7d  [e-1].tag_}",]}}
+0000ee80: 2920 2c20 0a09 2276 6470 6722 3a20 6c61  ) , .."vdpg": la
+0000ee90: 6d62 6461 2064 2c73 2c65 2c74 6167 3a64  mbda d,s,e,tag:d
+0000eea0: 2e75 7365 725f 6461 7461 2e75 7064 6174  .user_data.updat
+0000eeb0: 6528 7b20 6622 7b74 6167 7d3a 7b64 5b73  e({ f"{tag}:{d[s
+0000eec0: 5d2e 6c65 6d6d 615f 7d20 7b64 5b73 2b31  ].lemma_} {d[s+1
+0000eed0: 3a65 5d2e 7465 7874 2e6c 6f77 6572 2829  :e].text.lower()
+0000eee0: 7d5b 7b73 7d2c 7b65 7d29 223a 0a09 097b  }[{s},{e})":...{
+0000eef0: 226e 6163 223a 205b 6622 7b64 5b73 5d2e  "nac": [f"{d[s].
+0000ef00: 6c65 6d6d 615f 7d3a 5645 5242 3a76 6470  lemma_}:VERB:vdp
+0000ef10: 677c 7b64 5b73 5d2e 6c65 6d6d 615f 7d20  g|{d[s].lemma_} 
+0000ef20: 7b64 5b73 2b31 3a65 5d2e 7465 7874 7d22  {d[s+1:e].text}"
+0000ef30: 2c20 6622 7b64 5b73 5d2e 6c65 6d6d 615f  , f"{d[s].lemma_
+0000ef40: 7d3a 5645 5242 7c76 6470 6722 2c20 6622  }:VERB|vdpg", f"
+0000ef50: 5f7b 645b 735d 2e6c 656d 6d61 5f7d 207b  _{d[s].lemma_} {
+0000ef60: 645b 732b 313a 652d 315d 2e74 6578 747d  d[s+1:e-1].text}
+0000ef70: 205f 5642 4722 2c0a 0909 0909 6622 7b64   _VBG",.....f"{d
+0000ef80: 5b73 5d2e 6c65 6d6d 615f 7d2f 5645 5242  [s].lemma_}/VERB
+0000ef90: 7c76 6470 673a 5f7b 645b 735d 2e6c 656d  |vdpg:_{d[s].lem
+0000efa0: 6d61 5f7d 207b 645b 732b 313a 652d 315d  ma_} {d[s+1:e-1]
+0000efb0: 2e74 6578 747d 205f 7b64 5b65 2d31 5d2e  .text} _{d[e-1].
+0000efc0: 7461 675f 7d22 2c5d 207d 7d29 2c0a 097d  tag_}",] }}),..}
+0000efd0: 0a0a 6465 6620 706f 7374 6167 5f6d 6174  ..def postag_mat
+0000efe0: 6368 2864 6f63 2c20 6675 6e63 3d6c 616d  ch(doc, func=lam
+0000eff0: 6264 6120 646f 632c 7374 6172 742c 656e  bda doc,start,en
+0000f000: 642c 7461 673a 2064 6f63 2e73 7061 6e73  d,tag: doc.spans
+0000f010: 2e75 7064 6174 6528 7b66 2270 6f73 7461  .update({f"posta
+0000f020: 675b 7b73 7461 7274 7d2c 7b65 6e64 7d29  g[{start},{end})
+0000f030: 3a7b 7461 677d 223a 2053 7061 6e47 726f  :{tag}": SpanGro
+0000f040: 7570 2864 6f63 2c20 6e61 6d65 3d74 6167  up(doc, name=tag
+0000f050: 2c20 7370 616e 733d 5b20 646f 635b 7374  , spans=[ doc[st
+0000f060: 6172 7420 3a20 656e 645d 205d 2c20 6174  art : end] ], at
+0000f070: 7472 733d 7b7d 2920 7d20 2920 293a 200a  trs={}) } ) ): .
+0000f080: 0927 2727 2064 6f63 2e73 7061 6e73 5b66  .''' doc.spans[f
+0000f090: 2273 7061 6e5b 7b73 7461 7274 7d2c 7b65  "span[{start},{e
+0000f0a0: 6e64 7d29 3a7b 7461 677d 225d 203d 2053  nd}):{tag}"] = S
+0000f0b0: 7061 6e47 726f 7570 2864 6f63 2c20 7c20  panGroup(doc, | 
+0000f0c0: 6164 6420 6d61 7463 6865 6420 6e65 7720  add matched new 
+0000f0d0: 7370 616e 2062 7920 7068 7261 7365 2072  span by phrase r
+0000f0e0: 756c 6573 2c20 3230 3233 2e32 2e36 2027  ules, 2023.2.6 '
+0000f0f0: 2727 0a09 6966 206e 6f74 2068 6173 6174  ''..if not hasat
+0000f100: 7472 2870 6f73 7461 675f 6d61 7463 682c  tr(postag_match,
+0000f110: 2027 6d61 7463 6865 7227 293a 2020 090a   'matcher'):  ..
+0000f120: 0909 706f 7374 6167 5f6d 6174 6368 2e6d  ..postag_match.m
+0000f130: 6174 6368 6572 203d 2070 6872 6173 655f  atcher = phrase_
+0000f140: 6d61 7463 6865 7228 7b0a 0909 2270 726d  matcher({..."prm
+0000f150: 6f64 7322 3a5b 5b7b 2250 4f53 223a 207b  ods":[[{"POS": {
+0000f160: 2249 4e22 3a20 5b22 4155 5822 2c22 5645  "IN": ["AUX","VE
+0000f170: 5242 225d 7d7d 2c7b 2250 4f53 223a 207b  RB"]}},{"POS": {
+0000f180: 2249 4e22 3a20 5b22 4144 5622 5d7d 2c20  "IN": ["ADV"]}, 
+0000f190: 224f 5022 3a20 222a 227d 2c20 7b22 504f  "OP": "*"}, {"PO
+0000f1a0: 5322 3a20 7b22 494e 223a 205b 2241 444a  S": {"IN": ["ADJ
+0000f1b0: 222c 2256 4552 4222 5d7d 2c20 224f 5022  ","VERB"]}, "OP"
+0000f1c0: 3a20 222a 227d 2c7b 2250 4f53 223a 207b  : "*"},{"POS": {
+0000f1d0: 2249 4e22 3a20 5b22 5041 5254 222c 2241  "IN": ["PART","A
+0000f1e0: 4450 222c 2254 4f22 5d7d 2c20 224f 5022  DP","TO"]}, "OP"
+0000f1f0: 3a20 222a 227d 2c7b 2250 4f53 223a 2027  : "*"},{"POS": '
+0000f200: 5645 5242 277d 5d5d 2c20 2320 636f 756c  VERB'}]], # coul
+0000f210: 6420 6861 7264 6c79 2077 6169 7420 746f  d hardly wait to
+0000f220: 206d 6565 740a 0909 2256 5022 3a20 205b   meet..."VP":  [
+0000f230: 5b7b 2750 4f53 273a 2027 5645 5242 277d  [{'POS': 'VERB'}
+0000f240: 2c7b 2250 4f53 223a 207b 2249 4e22 3a20  ,{"POS": {"IN": 
+0000f250: 5b22 4445 5422 2c22 4144 5022 2c22 4144  ["DET","ADP","AD
+0000f260: 4a22 5d7d 2c20 224f 5022 3a20 222a 227d  J"]}, "OP": "*"}
+0000f270: 2c7b 2250 4f53 223a 2027 4e4f 554e 277d  ,{"POS": 'NOUN'}
+0000f280: 2c20 7b22 504f 5322 3a20 7b22 494e 223a  , {"POS": {"IN":
+0000f290: 205b 2241 4450 222c 2254 4f22 5d7d 2c20   ["ADP","TO"]}, 
+0000f2a0: 224f 5022 3a20 222a 227d 5d2c 205b 7b27  "OP": "*"}], [{'
+0000f2b0: 504f 5327 3a20 2756 4552 4227 7d2c 7b22  POS': 'VERB'},{"
+0000f2c0: 504f 5322 3a20 7b22 494e 223a 205b 2244  POS": {"IN": ["D
+0000f2d0: 4554 222c 2241 4450 222c 2241 444a 222c  ET","ADP","ADJ",
+0000f2e0: 2254 4f22 2c22 5041 5254 225d 7d2c 2022  "TO","PART"]}, "
+0000f2f0: 4f50 223a 2022 2a22 7d2c 7b22 504f 5322  OP": "*"},{"POS"
+0000f300: 3a20 2756 4552 4227 7d5d 5d2c 2023 2077  : 'VERB'}]], # w
+0000f310: 6169 7420 746f 206d 6565 740a 0909 2250  ait to meet..."P
+0000f320: 5022 3a20 205b 5b7b 2750 4f53 273a 2027  P":  [[{'POS': '
+0000f330: 4144 5027 7d2c 7b22 504f 5322 3a20 7b22  ADP'},{"POS": {"
+0000f340: 494e 223a 205b 2244 4554 222c 224e 554d  IN": ["DET","NUM
+0000f350: 222c 2241 444a 222c 2750 554e 4354 272c  ","ADJ",'PUNCT',
+0000f360: 2743 4f4e 4a27 5d7d 2c20 224f 5022 3a20  'CONJ']}, "OP": 
+0000f370: 222a 227d 2c7b 2250 4f53 223a 207b 2249  "*"},{"POS": {"I
+0000f380: 4e22 3a20 5b22 4e4f 554e 222c 2250 4152  N": ["NOUN","PAR
+0000f390: 5422 5d7d 2c20 224f 5022 3a20 222b 227d  T"]}, "OP": "+"}
+0000f3a0: 5d5d 2c20 2020 200a 0909 2241 5022 3a20  ]],    ..."AP": 
+0000f3b0: 205b 5b7b 2250 4f53 223a 207b 2249 4e22   [[{"POS": {"IN"
+0000f3c0: 3a20 5b22 4144 5622 5d7d 2c20 224f 5022  : ["ADV"]}, "OP"
+0000f3d0: 3a20 222b 227d 2c20 7b22 504f 5322 3a20  : "+"}, {"POS": 
+0000f3e0: 2741 444a 277d 5d5d 2c20 200a 0909 2276  'ADJ'}]],  ..."v
+0000f3f0: 706e 223a 205b 5b7b 2250 4f53 223a 2256  pn": [[{"POS":"V
+0000f400: 4552 4222 2c22 5441 4722 3a20 7b22 4e4f  ERB","TAG": {"NO
+0000f410: 545f 494e 223a 205b 2256 424e 225d 7d7d  T_IN": ["VBN"]}}
+0000f420: 2c20 7b22 504f 5322 3a22 4144 5022 7d20  , {"POS":"ADP"} 
+0000f430: 2c20 7b22 5441 4722 3a22 4e4e 222c 2022  , {"TAG":"NN", "
+0000f440: 4953 5f4c 4f57 4552 223a 5472 7565 7d5d  IS_LOWER":True}]
+0000f450: 5d2c 2020 2320 636f 6d65 2069 6e74 6f20  ],  # come into 
+0000f460: 666f 7263 6520 0a09 0922 6270 6e22 3a20  force ..."bpn": 
+0000f470: 5b5b 7b22 4c45 4d4d 4122 3a22 6265 227d  [[{"LEMMA":"be"}
+0000f480: 2c20 7b22 504f 5322 3a22 4144 5022 7d20  , {"POS":"ADP"} 
+0000f490: 2c20 7b22 5441 4722 3a22 4e4e 227d 5d5d  , {"TAG":"NN"}]]
+0000f4a0: 2c20 2023 2062 6520 696e 2066 6f72 6365  ,  # be in force
+0000f4b0: 203d 3e20 7670 6e20 0a09 0922 766e 7022   => vpn ..."vnp"
+0000f4c0: 3a20 5b5b 7b22 504f 5322 3a22 5645 5242  : [[{"POS":"VERB
+0000f4d0: 222c 2254 4147 223a 207b 224e 4f54 5f49  ","TAG": {"NOT_I
+0000f4e0: 4e22 3a20 5b22 5642 4e22 5d7d 7d2c 207b  N": ["VBN"]}}, {
+0000f4f0: 2254 4147 223a 224e 4e22 7d2c 207b 2250  "TAG":"NN"}, {"P
+0000f500: 4f53 223a 2241 4450 227d 205d 5d2c 2020  OS":"ADP"} ]],  
+0000f510: 2320 6d61 6b65 2075 7365 206f 662c 206c  # make use of, l
+0000f520: 6179 2065 6d70 6861 7369 7320 6f6e 0a09  ay emphasis on..
+0000f530: 0922 7670 223a 205b 5b7b 2250 4f53 223a  ."vp": [[{"POS":
+0000f540: 2256 4552 4222 2c22 5441 4722 3a20 7b22  "VERB","TAG": {"
+0000f550: 4e4f 545f 494e 223a 205b 2256 424e 225d  NOT_IN": ["VBN"]
+0000f560: 7d7d 2c20 7b22 504f 5322 3a22 4144 5022  }}, {"POS":"ADP"
+0000f570: 7d20 5d5d 2c20 2023 2061 6269 6465 2062  } ]],  # abide b
+0000f580: 7920 7c20 6469 7374 696e 6775 6973 6820  y | distinguish 
+0000f590: 6672 6f6d 0a09 0922 7670 7022 3a20 5b5b  from..."vpp": [[
+0000f5a0: 7b22 504f 5322 3a22 5645 5242 222c 2254  {"POS":"VERB","T
+0000f5b0: 4147 223a 207b 224e 4f54 5f49 4e22 3a20  AG": {"NOT_IN": 
+0000f5c0: 5b22 5642 4e22 5d7d 7d2c 207b 2250 4f53  ["VBN"]}}, {"POS
+0000f5d0: 223a 2241 4450 227d 2c20 7b22 504f 5322  ":"ADP"}, {"POS"
+0000f5e0: 3a22 4144 5022 7d20 5d5d 2c20 2320 6c69  :"ADP"} ]], # li
+0000f5f0: 7665 2075 7020 746f 0a09 0922 7670 6722  ve up to..."vpg"
+0000f600: 3a20 5b5b 7b22 504f 5322 3a22 5645 5242  : [[{"POS":"VERB
+0000f610: 222c 2254 4147 223a 207b 224e 4f54 5f49  ","TAG": {"NOT_I
+0000f620: 4e22 3a20 5b22 5642 4e22 5d7d 7d2c 207b  N": ["VBN"]}}, {
+0000f630: 2250 4f53 223a 2241 4450 227d 2c20 7b22  "POS":"ADP"}, {"
+0000f640: 5441 4722 3a22 5642 4722 2c22 4445 5022  TAG":"VBG","DEP"
+0000f650: 3a22 7063 6f6d 7022 7d20 5d5d 2c20 2320  :"pcomp"} ]], # 
+0000f660: 696e 7369 7374 6564 206f 6e20 676f 696e  insisted on goin
+0000f670: 670a 0909 2270 6e22 3a20 5b5b 7b22 504f  g..."pn": [[{"PO
+0000f680: 5322 3a22 4144 5022 2c20 2244 4550 223a  S":"ADP", "DEP":
+0000f690: 2270 7265 7022 7d20 2c20 7b22 5441 4722  "prep"} , {"TAG"
+0000f6a0: 3a22 4e4e 222c 2022 4445 5022 3a22 706f  :"NN", "DEP":"po
+0000f6b0: 626a 227d 5d5d 2c20 2023 2062 7920 666f  bj"}]],  # by fo
+0000f6c0: 7263 650a 0909 2270 6e70 223a 205b 5b7b  rce..."pnp": [[{
+0000f6d0: 2250 4f53 223a 2241 4450 222c 2022 4445  "POS":"ADP", "DE
+0000f6e0: 5022 3a22 7072 6570 227d 202c 207b 2254  P":"prep"} , {"T
+0000f6f0: 4147 223a 224e 4e22 2c20 2244 4550 223a  AG":"NN", "DEP":
+0000f700: 2270 6f62 6a22 7d2c 207b 2250 4f53 223a  "pobj"}, {"POS":
+0000f710: 2241 4450 222c 2022 4445 5022 3a22 7072  "ADP", "DEP":"pr
+0000f720: 6570 227d 5d5d 2c20 2023 206f 6e20 6163  ep"}]],  # on ac
+0000f730: 636f 756e 7420 6f66 0a09 0922 6261 7076  count of..."bapv
+0000f740: 223a 205b 5b7b 224c 454d 4d41 223a 2262  ": [[{"LEMMA":"b
+0000f750: 6522 7d20 2c20 7b22 5441 4722 3a7b 2249  e"} , {"TAG":{"I
+0000f760: 4e22 3a20 5b22 4a4a 225d 7d7d 2c20 7b22  N": ["JJ"]}}, {"
+0000f770: 504f 5322 3a22 4144 5022 7d2c 207b 2250  POS":"ADP"}, {"P
+0000f780: 4f53 223a 2256 4552 4222 7d5d 5d2c 2020  OS":"VERB"}]],  
+0000f790: 2320 0a09 0922 6261 7476 223a 205b 5b7b  # ..."batv": [[{
+0000f7a0: 224c 454d 4d41 223a 2262 6522 7d20 2c20  "LEMMA":"be"} , 
+0000f7b0: 7b22 5441 4722 3a7b 2249 4e22 3a20 5b22  {"TAG":{"IN": ["
+0000f7c0: 4a4a 225d 7d7d 2c20 7b22 4c45 4d4d 4122  JJ"]}}, {"LEMMA"
+0000f7d0: 3a22 746f 227d 2c20 7b22 504f 5322 3a22  :"to"}, {"POS":"
+0000f7e0: 5645 5242 227d 5d5d 2c20 200a 0909 2262  VERB"}]],  ..."b
+0000f7f0: 6570 7622 3a20 5b5b 7b22 4c45 4d4d 4122  epv": [[{"LEMMA"
+0000f800: 3a22 6265 227d 202c 207b 2254 4147 223a  :"be"} , {"TAG":
+0000f810: 7b22 494e 223a 205b 2256 424e 225d 7d7d  {"IN": ["VBN"]}}
+0000f820: 2c20 7b22 504f 5322 3a22 4144 5022 7d2c  , {"POS":"ADP"},
+0000f830: 207b 2250 4f53 223a 2256 4552 4222 7d5d   {"POS":"VERB"}]
+0000f840: 5d2c 2020 2320 6265 2066 6f72 6365 6420  ],  # be forced 
+0000f850: 6f66 2067 6f69 6e67 202f 203f 2062 6570  of going / ? bep
+0000f860: 763f 200a 0909 2262 6574 7622 3a20 5b5b  v? ..."betv": [[
+0000f870: 7b22 4c45 4d4d 4122 3a22 6265 227d 202c  {"LEMMA":"be"} ,
+0000f880: 207b 2254 4147 223a 7b22 494e 223a 205b   {"TAG":{"IN": [
+0000f890: 2256 424e 225d 7d7d 2c20 7b22 4c45 4d4d  "VBN"]}}, {"LEMM
+0000f8a0: 4122 3a22 746f 227d 2c20 7b22 5441 4722  A":"to"}, {"TAG"
+0000f8b0: 3a22 5642 227d 5d5d 2c20 2023 2062 6520  :"VB"}]],  # be 
+0000f8c0: 636f 6e73 6964 6572 6564 2074 6f20 6265  considered to be
+0000f8d0: 2f67 6f0a 0909 2262 6170 223a 205b 5b7b  /go..."bap": [[{
+0000f8e0: 224c 454d 4d41 223a 2262 6522 7d20 2c20  "LEMMA":"be"} , 
+0000f8f0: 7b22 5441 4722 3a7b 2249 4e22 3a20 5b22  {"TAG":{"IN": ["
+0000f900: 4a4a 225d 7d7d 2c20 7b22 504f 5322 3a22  JJ"]}}, {"POS":"
+0000f910: 4144 5022 7d5d 5d2c 2023 6265 2069 676e  ADP"}]], #be ign
+0000f920: 6f72 616e 7420 6f66 0a09 0922 6265 7022  orant of..."bep"
+0000f930: 3a20 5b5b 7b22 4c45 4d4d 4122 3a22 6265  : [[{"LEMMA":"be
+0000f940: 227d 202c 207b 2254 4147 223a 7b22 494e  "} , {"TAG":{"IN
+0000f950: 223a 205b 2256 424e 225d 7d7d 2c20 7b22  ": ["VBN"]}}, {"
+0000f960: 504f 5322 3a22 4144 5022 7d5d 5d2c 2020  POS":"ADP"}]],  
+0000f970: 2320 6265 2066 6f72 6365 6420 746f 0a09  # be forced to..
+0000f980: 0922 766f 7022 3a20 5b5b 7b22 504f 5322  ."vop": [[{"POS"
+0000f990: 3a22 5645 5242 222c 2254 4147 223a 207b  :"VERB","TAG": {
+0000f9a0: 224e 4f54 5f49 4e22 3a20 5b22 5642 4e22  "NOT_IN": ["VBN"
+0000f9b0: 5d7d 7d20 2c20 7b22 5445 5854 223a 207b  ]}} , {"TEXT": {
+0000f9c0: 2252 4547 4558 223a 2022 5b61 2d7a 5d2b  "REGEX": "[a-z]+
+0000f9d0: 7365 6c66 2422 7d7d 2c20 7b22 504f 5322  self$"}}, {"POS"
+0000f9e0: 3a22 4144 5022 7d5d 5d2c 2023 7468 726f  :"ADP"}]], #thro
+0000f9f0: 7720 6f6e 6573 656c 6620 696e 746f 0a09  w oneself into..
+0000fa00: 0922 7674 7622 3a20 5b5b 7b22 504f 5322  ."vtv": [[{"POS"
+0000fa10: 3a22 5645 5242 222c 2254 4147 223a 207b  :"VERB","TAG": {
+0000fa20: 224e 4f54 5f49 4e22 3a20 5b22 5642 4e22  "NOT_IN": ["VBN"
+0000fa30: 5d7d 7d2c 207b 224c 454d 4d41 223a 2274  ]}}, {"LEMMA":"t
+0000fa40: 6f22 7d2c 207b 2250 4f53 223a 2256 4552  o"}, {"POS":"VER
+0000fa50: 4222 2c20 2244 4550 223a 2278 636f 6d70  B", "DEP":"xcomp
+0000fa60: 227d 205d 5d2c 200a 0909 2276 6722 3a20  "} ]], ..."vg": 
+0000fa70: 5b5b 7b22 504f 5322 3a22 5645 5242 222c  [[{"POS":"VERB",
+0000fa80: 2254 4147 223a 207b 224e 4f54 5f49 4e22  "TAG": {"NOT_IN"
+0000fa90: 3a20 5b22 5642 4e22 5d7d 7d2c 2020 7b22  : ["VBN"]}},  {"
+0000faa0: 5441 4722 3a22 5642 4722 2c20 2244 4550  TAG":"VBG", "DEP
+0000fab0: 223a 2278 636f 6d70 227d 205d 5d2c 200a  ":"xcomp"} ]], .
+0000fac0: 0909 2276 6470 6722 3a20 5b5b 7b22 504f  .."vdpg": [[{"PO
+0000fad0: 5322 3a22 5645 5242 227d 2c20 207b 2250  S":"VERB"},  {"P
+0000fae0: 4f53 223a 2241 4456 227d 202c 2020 7b22  OS":"ADV"} ,  {"
+0000faf0: 504f 5322 3a22 4144 5022 7d20 2c20 207b  POS":"ADP"} ,  {
+0000fb00: 2254 4147 223a 2256 4247 227d 205d 5d2c  "TAG":"VBG"} ]],
+0000fb10: 2020 2320 6c6f 6f6b 2066 6f72 7761 7264    # look forward
+0000fb20: 2074 6f20 7365 6569 6e67 0a09 097d 290a   to seeing...}).
+0000fb30: 0966 6f72 206e 616d 652c 2073 7461 7274  .for name, start
+0000fb40: 2c20 656e 6420 696e 2070 6f73 7461 675f  , end in postag_
+0000fb50: 6d61 7463 682e 6d61 7463 6865 7228 646f  match.matcher(do
+0000fb60: 6329 3a0a 0909 7472 793a 0a09 0909 7461  c):...try:....ta
+0000fb70: 6720 3d20 7370 6163 792e 6e6c 702e 766f  g = spacy.nlp.vo
+0000fb80: 6361 625b 6e61 6d65 5d2e 7465 7874 0a09  cab[name].text..
+0000fb90: 0909 6966 2069 7369 6e73 7461 6e63 6528  ..if isinstance(
+0000fba0: 6675 6e63 2c20 6469 6374 293a 2023 2074  func, dict): # t
+0000fbb0: 6167 202d 3e20 6c61 6d62 6461 200a 0909  ag -> lambda ...
+0000fbc0: 0909 6675 6e63 5b74 6167 5d28 646f 632c  ..func[tag](doc,
+0000fbd0: 2073 7461 7274 2c20 656e 642c 2074 6167   start, end, tag
+0000fbe0: 2920 6966 2074 6167 2069 6e20 6675 6e63  ) if tag in func
+0000fbf0: 2065 6c73 6520 7072 696e 7428 2249 6e76   else print("Inv
+0000fc00: 616c 6964 2074 6167 3a22 2c20 7461 672c  alid tag:", tag,
+0000fc10: 2064 6f63 5b73 7461 7274 3a65 6e64 5d2e   doc[start:end].
+0000fc20: 7465 7874 2920 0a09 0909 656c 7365 3a20  text) ....else: 
+0000fc30: 0a09 0909 0966 756e 6328 646f 632c 2073  .....func(doc, s
+0000fc40: 7461 7274 2c20 656e 642c 2074 6167 2920  tart, end, tag) 
+0000fc50: 2023 2069 7320 6120 6675 6e63 746f 722c   # is a functor,
+0000fc60: 2023 646f 632e 7370 616e 735b 6622 706f   #doc.spans[f"po
+0000fc70: 7374 6167 5b7b 7374 6172 747d 2c7b 656e  stag[{start},{en
+0000fc80: 647d 293a 7b74 6167 7d22 5d20 3d20 5370  d}):{tag}"] = Sp
+0000fc90: 616e 4772 6f75 7028 646f 632c 206e 616d  anGroup(doc, nam
+0000fca0: 653d 7461 672c 2073 7061 6e73 3d5b 2064  e=tag, spans=[ d
+0000fcb0: 6f63 5b73 7461 7274 203a 2065 6e64 5d20  oc[start : end] 
+0000fcc0: 5d2c 2061 7474 7273 3d7b 7d29 2023 6174  ], attrs={}) #at
+0000fcd0: 7472 7320 3d20 7b22 706f 7322 3a20 762e  trs = {"pos": v.
+0000fce0: 706f 735f 2c20 2274 6167 223a 2076 2e74  pos_, "tag": v.t
+0000fcf0: 6167 5f2c 2022 6465 7022 3a20 762e 6465  ag_, "dep": v.de
+0000fd00: 705f 2c20 226c 656d 6d61 223a 762e 6c65  p_, "lemma":v.le
+0000fd10: 6d6d 615f 2c20 2265 6e74 5f74 7970 6522  mma_, "ent_type"
+0000fd20: 3a20 2253 2e22 202b 2076 2e64 6570 5f20  : "S." + v.dep_ 
+0000fd30: 7d20 0a09 0965 7863 6570 7420 4578 6365  } ...except Exce
+0000fd40: 7074 696f 6e20 6173 2065 3a0a 0909 0970  ption as e:....p
+0000fd50: 7269 6e74 2028 2270 6f73 7461 675f 6d61  rint ("postag_ma
+0000fd60: 7463 6820 6578 3a22 2c20 652c 206e 616d  tch ex:", e, nam
+0000fd70: 652c 2073 7461 7274 2c20 656e 6429 200a  e, start, end) .
+0000fd80: 0a64 6566 2073 6b65 6e70 5f6d 6174 6368  .def skenp_match
+0000fd90: 2864 6f63 2c20 6675 6e63 3d6c 616d 6264  (doc, func=lambd
+0000fda0: 6120 646f 632c 7374 6172 742c 656e 642c  a doc,start,end,
+0000fdb0: 7461 673a 2064 6f63 2e73 7061 6e73 2e75  tag: doc.spans.u
+0000fdc0: 7064 6174 6528 7b66 2273 6b65 6e70 5b7b  pdate({f"skenp[{
+0000fdd0: 7374 6172 747d 2c7b 656e 647d 293a 7b74  start},{end}):{t
+0000fde0: 6167 7d22 3a20 5370 616e 4772 6f75 7028  ag}": SpanGroup(
+0000fdf0: 646f 632c 206e 616d 653d 7461 672c 2073  doc, name=tag, s
+0000fe00: 7061 6e73 3d5b 2064 6f63 5b73 7461 7274  pans=[ doc[start
+0000fe10: 203a 2065 6e64 5d20 5d2c 2061 7474 7273   : end] ], attrs
+0000fe20: 3d7b 7d29 207d 2029 293a 200a 0969 6620  ={}) } )): ..if 
+0000fe30: 6e6f 7420 6861 7361 7474 7228 736b 656e  not hasattr(sken
+0000fe40: 705f 6d61 7463 682c 2027 6d61 7463 6865  p_match, 'matche
+0000fe50: 7227 293a 2073 6b65 6e70 5f6d 6174 6368  r'): skenp_match
+0000fe60: 2e6d 6174 6368 6572 203d 2070 6872 6173  .matcher = phras
+0000fe70: 655f 6d61 7463 6865 7228 7b0a 0922 766e  e_matcher({.."vn
+0000fe80: 704e 223a 205b 5b7b 2250 4f53 223a 2256  pN": [[{"POS":"V
+0000fe90: 4552 4222 2c22 5441 4722 3a20 7b22 4e4f  ERB","TAG": {"NO
+0000fea0: 545f 494e 223a 205b 2256 424e 225d 7d7d  T_IN": ["VBN"]}}
+0000feb0: 2c20 7b22 454e 545f 5459 5045 223a 224e  , {"ENT_TYPE":"N
+0000fec0: 5022 7d2c 207b 2250 4f53 223a 7b22 494e  P"}, {"POS":{"IN
+0000fed0: 223a 205b 2241 4450 225d 7d7d 2c20 7b22  ": ["ADP"]}}, {"
+0000fee0: 454e 545f 5459 5045 223a 224e 5022 7d5d  ENT_TYPE":"NP"}]
+0000fef0: 5d2c 2020 2320 7265 6d69 6e64 205f 4e50  ],  # remind _NP
+0000ff00: 206f 6620 5f4e 5020 2c20 6272 696e 6720   of _NP , bring 
+0000ff10: 5f4e 5020 746f 206c 6966 650a 0922 766e  _NP to life.."vn
+0000ff20: 706e 223a 205b 5b7b 2250 4f53 223a 2256  pn": [[{"POS":"V
+0000ff30: 4552 4222 2c22 5441 4722 3a20 7b22 4e4f  ERB","TAG": {"NO
+0000ff40: 545f 494e 223a 205b 2256 424e 225d 7d7d  T_IN": ["VBN"]}}
+0000ff50: 2c20 7b22 454e 545f 5459 5045 223a 224e  , {"ENT_TYPE":"N
+0000ff60: 5022 7d2c 207b 2250 4f53 223a 7b22 494e  P"}, {"POS":{"IN
+0000ff70: 223a 205b 2241 4450 225d 7d7d 2c20 7b22  ": ["ADP"]}}, {"
+0000ff80: 5441 4722 3a22 4e4e 227d 5d5d 2c20 2023  TAG":"NN"}]],  #
+0000ff90: 2074 616b 6520 5f4e 5020 696e 746f 2061   take _NP into a
+0000ffa0: 6363 6f75 6e74 0a09 2276 706e 706e 223a  ccount.."vpnpn":
+0000ffb0: 205b 5b7b 2250 4f53 223a 2256 4552 4222   [[{"POS":"VERB"
+0000ffc0: 2c22 5441 4722 3a20 7b22 4e4f 545f 494e  ,"TAG": {"NOT_IN
+0000ffd0: 223a 205b 2256 424e 225d 7d7d 2c20 7b22  ": ["VBN"]}}, {"
+0000ffe0: 504f 5322 3a7b 2249 4e22 3a20 5b22 4144  POS":{"IN": ["AD
+0000fff0: 5022 5d7d 7d2c 207b 2245 4e54 5f54 5950  P"]}}, {"ENT_TYP
+00010000: 4522 3a22 4e50 227d 2c20 7b22 504f 5322  E":"NP"}, {"POS"
+00010010: 3a7b 2249 4e22 3a20 5b22 4144 5022 5d7d  :{"IN": ["ADP"]}
 00010020: 7d2c 207b 2245 4e54 5f54 5950 4522 3a22  }, {"ENT_TYPE":"
-00010030: 4e50 227d 205d 5d2c 2020 2320 4920 6b65  NP"} ]],  # I ke
-00010040: 6570 2069 6e20 6d69 6e64 2074 6865 2069  ep in mind the i
-00010050: 6e74 6572 636f 6e6e 6563 7465 646e 6573  nterconnectednes
-00010060: 732e 0a09 2276 6e22 3a20 5b5b 7b22 504f  s..."vn": [[{"PO
-00010070: 5322 3a22 5645 5242 227d 2c20 7b22 454e  S":"VERB"}, {"EN
-00010080: 545f 5459 5045 223a 224e 5022 2c20 2244  T_TYPE":"NP", "D
-00010090: 4550 223a 2264 6f62 6a22 7d20 5d5d 2c20  EP":"dobj"} ]], 
-000100a0: 0a09 2276 6e6e 223a 205b 5b7b 2250 4f53  .."vnn": [[{"POS
-000100b0: 223a 2256 4552 4222 7d2c 207b 2245 4e54  ":"VERB"}, {"ENT
-000100c0: 5f54 5950 4522 3a22 4e50 222c 2022 4445  _TYPE":"NP", "DE
-000100d0: 5022 3a22 646f 626a 227d 2c20 7b22 454e  P":"dobj"}, {"EN
-000100e0: 545f 5459 5045 223a 224e 5022 2c20 2244  T_TYPE":"NP", "D
-000100f0: 4550 223a 226f 7072 6422 7d20 5d5d 2c20  EP":"oprd"} ]], 
-00010100: 0a09 2276 6e61 223a 205b 5b7b 2250 4f53  .."vna": [[{"POS
-00010110: 223a 2256 4552 4222 7d2c 207b 2245 4e54  ":"VERB"}, {"ENT
-00010120: 5f54 5950 4522 3a22 4e50 222c 2022 4445  _TYPE":"NP", "DE
-00010130: 5022 3a22 646f 626a 227d 2c20 7b22 504f  P":"dobj"}, {"PO
-00010140: 5322 3a22 4144 4a22 2c20 2244 4550 223a  S":"ADJ", "DEP":
-00010150: 226f 7072 6422 7d20 5d5d 2c20 0a09 2276  "oprd"} ]], .."v
-00010160: 6e65 223a 205b 5b7b 2250 4f53 223a 2256  ne": [[{"POS":"V
-00010170: 4552 4222 7d2c 207b 2245 4e54 5f54 5950  ERB"}, {"ENT_TYP
-00010180: 4522 3a22 4e50 222c 2022 4445 5022 3a22  E":"NP", "DEP":"
-00010190: 646f 626a 227d 2c20 7b22 5441 4722 3a22  dobj"}, {"TAG":"
-000101a0: 5642 4e22 7d20 5d5d 2c20 2320 6c65 6176  VBN"} ]], # leav
-000101b0: 6520 6974 206b 6570 7420 0a09 2276 6e74  e it kept .."vnt
-000101c0: 6222 3a20 5b5b 7b22 504f 5322 3a22 5645  b": [[{"POS":"VE
-000101d0: 5242 222c 2254 4147 223a 207b 224e 4f54  RB","TAG": {"NOT
-000101e0: 5f49 4e22 3a20 5b22 5642 4e22 5d7d 7d2c  _IN": ["VBN"]}},
-000101f0: 207b 2245 4e54 5f54 5950 4522 3a22 4e50   {"ENT_TYPE":"NP
-00010200: 227d 2c20 7b22 4c45 4d4d 4122 3a22 746f  "}, {"LEMMA":"to
-00010210: 227d 202c 207b 224c 454d 4d41 223a 2262  "} , {"LEMMA":"b
-00010220: 6522 7d5d 5d2c 2023 2063 6f6e 7369 6465  e"}]], # conside
-00010230: 7220 5f4e 5020 5f4e 5020 7c20 5f4e 5020  r _NP _NP | _NP 
-00010240: 5f41 444a 207c 205f 4e50 2074 6f20 6265  _ADJ | _NP to be
-00010250: 200a 0922 766e 7476 223a 205b 5b7b 2250   .."vntv": [[{"P
-00010260: 4f53 223a 2256 4552 4222 2c22 5441 4722  OS":"VERB","TAG"
-00010270: 3a20 7b22 4e4f 545f 494e 223a 205b 2256  : {"NOT_IN": ["V
-00010280: 424e 225d 7d7d 2c20 7b22 454e 545f 5459  BN"]}}, {"ENT_TY
-00010290: 5045 223a 224e 5022 7d2c 207b 224c 454d  PE":"NP"}, {"LEM
-000102a0: 4d41 223a 2274 6f22 7d20 2c20 7b22 504f  MA":"to"} , {"PO
-000102b0: 5322 3a22 5645 5242 227d 5d5d 2c20 2320  S":"VERB"}]], # 
-000102c0: 5f66 6f72 6365 205f 4e50 2074 6f20 5f56  _force _NP to _V
-000102d0: 4552 420a 0922 766e 7462 6e22 3a20 5b5b  ERB.."vntbn": [[
-000102e0: 7b22 504f 5322 3a22 5645 5242 227d 2c20  {"POS":"VERB"}, 
-000102f0: 7b22 454e 545f 5459 5045 223a 224e 5022  {"ENT_TYPE":"NP"
-00010300: 7d2c 207b 224c 454d 4d41 223a 2274 6f22  }, {"LEMMA":"to"
-00010310: 7d20 2c20 7b22 4c45 4d4d 4122 3a22 6265  } , {"LEMMA":"be
-00010320: 227d 2c20 7b22 454e 545f 5459 5045 223a  "}, {"ENT_TYPE":
-00010330: 224e 5022 7d5d 5d2c 200a 0922 766e 7462  "NP"}]], .."vntb
-00010340: 6122 3a20 5b5b 7b22 504f 5322 3a22 5645  a": [[{"POS":"VE
-00010350: 5242 227d 2c20 7b22 454e 545f 5459 5045  RB"}, {"ENT_TYPE
-00010360: 223a 224e 5022 7d2c 207b 224c 454d 4d41  ":"NP"}, {"LEMMA
-00010370: 223a 2274 6f22 7d20 2c20 7b22 4c45 4d4d  ":"to"} , {"LEMM
-00010380: 4122 3a22 6265 227d 2c20 7b22 504f 5322  A":"be"}, {"POS"
-00010390: 3a22 4144 4a22 7d5d 5d2c 0a09 2276 6470  :"ADJ"}]],.."vdp
-000103a0: 6e22 3a20 5b5b 7b22 504f 5322 3a22 5645  n": [[{"POS":"VE
-000103b0: 5242 227d 2c20 207b 2250 4f53 223a 2241  RB"},  {"POS":"A
-000103c0: 4456 227d 202c 2020 7b22 504f 5322 3a22  DV"} ,  {"POS":"
-000103d0: 4144 5022 7d20 2c20 207b 2245 4e54 5f54  ADP"} ,  {"ENT_T
-000103e0: 5950 4522 3a22 4e50 227d 205d 5d2c 2020  YPE":"NP"} ]],  
-000103f0: 2320 6c6f 6f6b 2066 6f72 7761 7264 2074  # look forward t
-00010400: 6f20 5f4e 5020 7c20 6120 6272 6967 6874  o _NP | a bright
-00010410: 2066 7574 7572 6520 0a09 7d29 0a09 666f   future ..})..fo
-00010420: 7220 6e61 6d65 2c20 7374 6172 742c 2065  r name, start, e
-00010430: 6e64 2069 6e20 736b 656e 705f 6d61 7463  nd in skenp_matc
-00010440: 682e 6d61 7463 6865 7228 646f 6329 3a0a  h.matcher(doc):.
-00010450: 0909 7472 793a 0a09 0909 7461 6720 3d20  ..try:....tag = 
-00010460: 7370 6163 792e 6e6c 702e 766f 6361 625b  spacy.nlp.vocab[
-00010470: 6e61 6d65 5d2e 7465 7874 0a09 0909 6966  name].text....if
-00010480: 2069 7369 6e73 7461 6e63 6528 6675 6e63   isinstance(func
-00010490: 2c20 6469 6374 293a 2023 2074 6167 202d  , dict): # tag -
-000104a0: 3e20 6c61 6d62 6461 200a 0909 0909 6675  > lambda .....fu
-000104b0: 6e63 5b74 6167 5d28 646f 632c 2073 7461  nc[tag](doc, sta
-000104c0: 7274 2c20 656e 642c 2074 6167 2920 6966  rt, end, tag) if
-000104d0: 2074 6167 2069 6e20 6675 6e63 2065 6c73   tag in func els
-000104e0: 6520 7072 696e 7428 2249 6e76 616c 6964  e print("Invalid
-000104f0: 2074 6167 3a22 2c20 7461 672c 2064 6f63   tag:", tag, doc
-00010500: 5b73 7461 7274 3a65 6e64 5d2e 7465 7874  [start:end].text
-00010510: 2920 0a09 0909 656c 7365 3a20 0a09 0909  ) ....else: ....
-00010520: 0966 756e 6328 646f 632c 2073 7461 7274  .func(doc, start
-00010530: 2c20 656e 642c 2074 6167 2920 2320 646f  , end, tag) # do
-00010540: 632e 7370 616e 735b 6622 736b 656e 705b  c.spans[f"skenp[
-00010550: 7b73 7461 7274 7d2c 7b65 6e64 7d29 3a7b  {start},{end}):{
-00010560: 7461 677d 225d 203d 2053 7061 6e47 726f  tag}"] = SpanGro
-00010570: 7570 2864 6f63 2c20 6e61 6d65 3d74 6167  up(doc, name=tag
-00010580: 2c20 7370 616e 733d 5b20 646f 635b 7374  , spans=[ doc[st
-00010590: 6172 7420 3a20 656e 645d 205d 2c20 6174  art : end] ], at
-000105a0: 7472 733d 7b7d 2920 2361 7474 7273 203d  trs={}) #attrs =
-000105b0: 207b 2270 6f73 223a 2076 2e70 6f73 5f2c   {"pos": v.pos_,
-000105c0: 2022 7461 6722 3a20 762e 7461 675f 2c20   "tag": v.tag_, 
-000105d0: 2264 6570 223a 2076 2e64 6570 5f2c 2022  "dep": v.dep_, "
-000105e0: 6c65 6d6d 6122 3a76 2e6c 656d 6d61 5f2c  lemma":v.lemma_,
-000105f0: 2022 656e 745f 7479 7065 223a 2022 532e   "ent_type": "S.
-00010600: 2220 2b20 762e 6465 705f 207d 200a 0909  " + v.dep_ } ...
-00010610: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00010620: 2061 7320 653a 0a09 0909 7072 696e 7420   as e:....print 
-00010630: 2822 736b 656e 705f 6d61 7463 6820 6578  ("skenp_match ex
-00010640: 3a22 2c20 652c 206e 616d 652c 2073 7461  :", e, name, sta
-00010650: 7274 2c20 656e 6429 200a 0909 0965 7863  rt, end) ....exc
-00010660: 5f74 7970 652c 2065 7863 5f76 616c 7565  _type, exc_value
-00010670: 2c20 6578 635f 6f62 6a20 3d20 7379 732e  , exc_obj = sys.
-00010680: 6578 635f 696e 666f 2829 2009 0a09 0909  exc_info() .....
-00010690: 7472 6163 6562 6163 6b2e 7072 696e 745f  traceback.print_
-000106a0: 7462 2865 7863 5f6f 626a 290a 0a64 6566  tb(exc_obj)..def
-000106b0: 2074 7270 335f 6d61 7463 6828 646f 632c   trp3_match(doc,
-000106c0: 2066 756e 633d 6c61 6d62 6461 2064 6f63   func=lambda doc
-000106d0: 2c69 2c6a 2c6b 2c74 6167 3a20 646f 632e  ,i,j,k,tag: doc.
-000106e0: 7370 616e 732e 7570 6461 7465 287b 6622  spans.update({f"
-000106f0: 7472 7033 5b7b 697d 2c7b 6a7d 2c7b 6b7d  trp3[{i},{j},{k}
-00010700: 5d3a 7b74 6167 7d22 3a20 5370 616e 4772  ]:{tag}": SpanGr
-00010710: 6f75 7028 646f 632c 206e 616d 653d 7461  oup(doc, name=ta
-00010720: 672c 2073 7061 6e73 3d5b 2064 6f63 5b69  g, spans=[ doc[i
-00010730: 3a69 2b31 5d2c 2064 6f63 5b6a 3a6a 2b31  :i+1], doc[j:j+1
-00010740: 5d2c 2064 6f63 5b6b 3a6b 2b31 5d20 5d2c  ], doc[k:k+1] ],
-00010750: 2061 7474 7273 3d7b 2274 6167 223a 7461   attrs={"tag":ta
-00010760: 672c 2022 6922 3a69 2c22 6a22 3a6a 2c20  g, "i":i,"j":j, 
-00010770: 226b 223a 6b7d 2920 7d20 2929 3a0a 0969  "k":k}) } )):..i
-00010780: 6620 6e6f 7420 6861 7361 7474 7228 7472  f not hasattr(tr
-00010790: 7033 5f6d 6174 6368 2c20 276d 6174 6368  p3_match, 'match
-000107a0: 6572 2729 3a20 0a09 0974 7270 335f 6d61  er'): ...trp3_ma
-000107b0: 7463 682e 6d61 7463 6865 7220 3d20 4465  tch.matcher = De
-000107c0: 704d 6174 6368 6572 287b 0a09 0922 646f  pMatcher({..."do
-000107d0: 626a 2d61 6476 6d6f 6422 3a5b 207b 2252  bj-advmod":[ {"R
-000107e0: 4947 4854 5f49 4422 3a20 2276 222c 2020  IGHT_ID": "v",  
-000107f0: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
-00010800: 2250 4f53 223a 2022 5645 5242 227d 7d2c  "POS": "VERB"}},
-00010810: 7b22 4c45 4654 5f49 4422 3a20 2276 222c  {"LEFT_ID": "v",
-00010820: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
-00010830: 2252 4947 4854 5f49 4422 3a20 226e 222c  "RIGHT_ID": "n",
-00010840: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
-00010850: 2244 4550 223a 2022 646f 626a 227d 2020  "DEP": "dobj"}  
-00010860: 7d2c 207b 224c 4546 545f 4944 223a 2022  }, {"LEFT_ID": "
-00010870: 7622 2c20 2252 454c 5f4f 5022 3a20 223e  v", "REL_OP": ">
-00010880: 222c 2022 5249 4748 545f 4944 223a 2022  ", "RIGHT_ID": "
-00010890: 6164 7622 2c20 2252 4947 4854 5f41 5454  adv", "RIGHT_ATT
-000108a0: 5253 223a 207b 2244 4550 223a 2022 6164  RS": {"DEP": "ad
-000108b0: 766d 6f64 227d 7d5d 2c20 2320 7468 6520  vmod"}}], # the 
-000108c0: 6c61 7374 206f 6e65 202c 2069 7320 7468  last one , is th
-000108d0: 6520 4144 5620 0a09 0922 646f 626a 2d61  e ADV ..."dobj-a
-000108e0: 6d6f 6422 3a20 205b 207b 2252 4947 4854  mod":  [ {"RIGHT
-000108f0: 5f49 4422 3a20 2276 222c 2020 2252 4947  _ID": "v",  "RIG
-00010900: 4854 5f41 5454 5253 223a 207b 2250 4f53  HT_ATTRS": {"POS
-00010910: 223a 2022 5645 5242 227d 7d2c 7b22 4c45  ": "VERB"}},{"LE
-00010920: 4654 5f49 4422 3a20 2276 222c 2022 5245  FT_ID": "v", "RE
-00010930: 4c5f 4f50 223a 2022 3e22 2c20 2252 4947  L_OP": ">", "RIG
-00010940: 4854 5f49 4422 3a20 226e 222c 2252 4947  HT_ID": "n","RIG
-00010950: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
-00010960: 223a 2022 646f 626a 227d 2020 7d2c 207b  ": "dobj"}  }, {
-00010970: 224c 4546 545f 4944 223a 2022 6e22 2c20  "LEFT_ID": "n", 
-00010980: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
-00010990: 5249 4748 545f 4944 223a 2022 6122 2c20  RIGHT_ID": "a", 
+00010030: 4e50 227d 5d5d 2c20 2023 2076 6172 7920  NP"}]],  # vary 
+00010040: 6672 6f6d 205f 4e50 2074 6f20 5f4e 5020  from _NP to _NP 
+00010050: 0a09 2276 6e70 6522 3a20 5b5b 7b22 504f  .."vnpe": [[{"PO
+00010060: 5322 3a22 5645 5242 222c 2254 4147 223a  S":"VERB","TAG":
+00010070: 207b 224e 4f54 5f49 4e22 3a20 5b22 5642   {"NOT_IN": ["VB
+00010080: 4e22 5d7d 7d2c 207b 2245 4e54 5f54 5950  N"]}}, {"ENT_TYP
+00010090: 4522 3a22 4e50 227d 2c20 7b22 5441 4722  E":"NP"}, {"TAG"
+000100a0: 3a22 494e 227d 2c20 7b22 5441 4722 3a22  :"IN"}, {"TAG":"
+000100b0: 5642 4e22 7d5d 5d2c 2020 2320 7461 6b65  VBN"}]],  # take
+000100c0: 205f 4e50 2066 6f72 2f61 7320 6772 616e   _NP for/as gran
+000100d0: 7465 640a 0922 7670 706e 223a 205b 5b7b  ted.."vppn": [[{
+000100e0: 2250 4f53 223a 2256 4552 4222 7d2c 207b  "POS":"VERB"}, {
+000100f0: 2250 4f53 223a 2241 4450 227d 2c20 7b22  "POS":"ADP"}, {"
+00010100: 504f 5322 3a22 4144 5022 7d2c 207b 2245  POS":"ADP"}, {"E
+00010110: 4e54 5f54 5950 4522 3a22 4e50 227d 205d  NT_TYPE":"NP"} ]
+00010120: 5d2c 2020 2320 6c69 7665 2075 7020 746f  ],  # live up to
+00010130: 205f 4e50 0a09 2276 6470 6e22 3a20 5b5b   _NP.."vdpn": [[
+00010140: 7b22 504f 5322 3a22 5645 5242 227d 2c20  {"POS":"VERB"}, 
+00010150: 7b22 504f 5322 3a22 4144 5622 7d2c 207b  {"POS":"ADV"}, {
+00010160: 2250 4f53 223a 2241 4450 227d 2c20 7b22  "POS":"ADP"}, {"
+00010170: 454e 545f 5459 5045 223a 224e 5022 7d20  ENT_TYPE":"NP"} 
+00010180: 5d5d 2c20 2023 206c 6f6f 6b20 6261 636b  ]],  # look back
+00010190: 206f 6e20 5f4e 5020 0a09 2276 706e 6e22   on _NP .."vpnn"
+000101a0: 3a20 5b5b 7b22 504f 5322 3a22 5645 5242  : [[{"POS":"VERB
+000101b0: 227d 2c20 7b22 504f 5322 3a22 4144 5022  "}, {"POS":"ADP"
+000101c0: 7d2c 207b 2254 4147 223a 224e 4f55 4e22  }, {"TAG":"NOUN"
+000101d0: 7d2c 207b 2245 4e54 5f54 5950 4522 3a22  }, {"ENT_TYPE":"
+000101e0: 4e50 227d 205d 5d2c 2020 2320 4920 6b65  NP"} ]],  # I ke
+000101f0: 6570 2069 6e20 6d69 6e64 2074 6865 2069  ep in mind the i
+00010200: 6e74 6572 636f 6e6e 6563 7465 646e 6573  nterconnectednes
+00010210: 732e 0a09 2276 6e22 3a20 5b5b 7b22 504f  s..."vn": [[{"PO
+00010220: 5322 3a22 5645 5242 227d 2c20 7b22 454e  S":"VERB"}, {"EN
+00010230: 545f 5459 5045 223a 224e 5022 2c20 2244  T_TYPE":"NP", "D
+00010240: 4550 223a 2264 6f62 6a22 7d20 5d5d 2c20  EP":"dobj"} ]], 
+00010250: 0a09 2276 6e6e 223a 205b 5b7b 2250 4f53  .."vnn": [[{"POS
+00010260: 223a 2256 4552 4222 7d2c 207b 2245 4e54  ":"VERB"}, {"ENT
+00010270: 5f54 5950 4522 3a22 4e50 222c 2022 4445  _TYPE":"NP", "DE
+00010280: 5022 3a22 646f 626a 227d 2c20 7b22 454e  P":"dobj"}, {"EN
+00010290: 545f 5459 5045 223a 224e 5022 2c20 2244  T_TYPE":"NP", "D
+000102a0: 4550 223a 226f 7072 6422 7d20 5d5d 2c20  EP":"oprd"} ]], 
+000102b0: 0a09 2276 6e61 223a 205b 5b7b 2250 4f53  .."vna": [[{"POS
+000102c0: 223a 2256 4552 4222 7d2c 207b 2245 4e54  ":"VERB"}, {"ENT
+000102d0: 5f54 5950 4522 3a22 4e50 222c 2022 4445  _TYPE":"NP", "DE
+000102e0: 5022 3a22 646f 626a 227d 2c20 7b22 504f  P":"dobj"}, {"PO
+000102f0: 5322 3a22 4144 4a22 2c20 2244 4550 223a  S":"ADJ", "DEP":
+00010300: 226f 7072 6422 7d20 5d5d 2c20 0a09 2276  "oprd"} ]], .."v
+00010310: 6e65 223a 205b 5b7b 2250 4f53 223a 2256  ne": [[{"POS":"V
+00010320: 4552 4222 7d2c 207b 2245 4e54 5f54 5950  ERB"}, {"ENT_TYP
+00010330: 4522 3a22 4e50 222c 2022 4445 5022 3a22  E":"NP", "DEP":"
+00010340: 646f 626a 227d 2c20 7b22 5441 4722 3a22  dobj"}, {"TAG":"
+00010350: 5642 4e22 7d20 5d5d 2c20 2320 6c65 6176  VBN"} ]], # leav
+00010360: 6520 6974 206b 6570 7420 0a09 2276 6e74  e it kept .."vnt
+00010370: 6222 3a20 5b5b 7b22 504f 5322 3a22 5645  b": [[{"POS":"VE
+00010380: 5242 222c 2254 4147 223a 207b 224e 4f54  RB","TAG": {"NOT
+00010390: 5f49 4e22 3a20 5b22 5642 4e22 5d7d 7d2c  _IN": ["VBN"]}},
+000103a0: 207b 2245 4e54 5f54 5950 4522 3a22 4e50   {"ENT_TYPE":"NP
+000103b0: 227d 2c20 7b22 4c45 4d4d 4122 3a22 746f  "}, {"LEMMA":"to
+000103c0: 227d 202c 207b 224c 454d 4d41 223a 2262  "} , {"LEMMA":"b
+000103d0: 6522 7d5d 5d2c 2023 2063 6f6e 7369 6465  e"}]], # conside
+000103e0: 7220 5f4e 5020 5f4e 5020 7c20 5f4e 5020  r _NP _NP | _NP 
+000103f0: 5f41 444a 207c 205f 4e50 2074 6f20 6265  _ADJ | _NP to be
+00010400: 200a 0922 766e 7476 223a 205b 5b7b 2250   .."vntv": [[{"P
+00010410: 4f53 223a 2256 4552 4222 2c22 5441 4722  OS":"VERB","TAG"
+00010420: 3a20 7b22 4e4f 545f 494e 223a 205b 2256  : {"NOT_IN": ["V
+00010430: 424e 225d 7d7d 2c20 7b22 454e 545f 5459  BN"]}}, {"ENT_TY
+00010440: 5045 223a 224e 5022 7d2c 207b 224c 454d  PE":"NP"}, {"LEM
+00010450: 4d41 223a 2274 6f22 7d20 2c20 7b22 504f  MA":"to"} , {"PO
+00010460: 5322 3a22 5645 5242 227d 5d5d 2c20 2320  S":"VERB"}]], # 
+00010470: 5f66 6f72 6365 205f 4e50 2074 6f20 5f56  _force _NP to _V
+00010480: 4552 420a 0922 766e 7462 6e22 3a20 5b5b  ERB.."vntbn": [[
+00010490: 7b22 504f 5322 3a22 5645 5242 227d 2c20  {"POS":"VERB"}, 
+000104a0: 7b22 454e 545f 5459 5045 223a 224e 5022  {"ENT_TYPE":"NP"
+000104b0: 7d2c 207b 224c 454d 4d41 223a 2274 6f22  }, {"LEMMA":"to"
+000104c0: 7d20 2c20 7b22 4c45 4d4d 4122 3a22 6265  } , {"LEMMA":"be
+000104d0: 227d 2c20 7b22 454e 545f 5459 5045 223a  "}, {"ENT_TYPE":
+000104e0: 224e 5022 7d5d 5d2c 200a 0922 766e 7462  "NP"}]], .."vntb
+000104f0: 6122 3a20 5b5b 7b22 504f 5322 3a22 5645  a": [[{"POS":"VE
+00010500: 5242 227d 2c20 7b22 454e 545f 5459 5045  RB"}, {"ENT_TYPE
+00010510: 223a 224e 5022 7d2c 207b 224c 454d 4d41  ":"NP"}, {"LEMMA
+00010520: 223a 2274 6f22 7d20 2c20 7b22 4c45 4d4d  ":"to"} , {"LEMM
+00010530: 4122 3a22 6265 227d 2c20 7b22 504f 5322  A":"be"}, {"POS"
+00010540: 3a22 4144 4a22 7d5d 5d2c 0a09 2276 6470  :"ADJ"}]],.."vdp
+00010550: 6e22 3a20 5b5b 7b22 504f 5322 3a22 5645  n": [[{"POS":"VE
+00010560: 5242 227d 2c20 207b 2250 4f53 223a 2241  RB"},  {"POS":"A
+00010570: 4456 227d 202c 2020 7b22 504f 5322 3a22  DV"} ,  {"POS":"
+00010580: 4144 5022 7d20 2c20 207b 2245 4e54 5f54  ADP"} ,  {"ENT_T
+00010590: 5950 4522 3a22 4e50 227d 205d 5d2c 2020  YPE":"NP"} ]],  
+000105a0: 2320 6c6f 6f6b 2066 6f72 7761 7264 2074  # look forward t
+000105b0: 6f20 5f4e 5020 7c20 6120 6272 6967 6874  o _NP | a bright
+000105c0: 2066 7574 7572 6520 0a09 7d29 0a09 666f   future ..})..fo
+000105d0: 7220 6e61 6d65 2c20 7374 6172 742c 2065  r name, start, e
+000105e0: 6e64 2069 6e20 736b 656e 705f 6d61 7463  nd in skenp_matc
+000105f0: 682e 6d61 7463 6865 7228 646f 6329 3a0a  h.matcher(doc):.
+00010600: 0909 7472 793a 0a09 0909 7461 6720 3d20  ..try:....tag = 
+00010610: 7370 6163 792e 6e6c 702e 766f 6361 625b  spacy.nlp.vocab[
+00010620: 6e61 6d65 5d2e 7465 7874 0a09 0909 6966  name].text....if
+00010630: 2069 7369 6e73 7461 6e63 6528 6675 6e63   isinstance(func
+00010640: 2c20 6469 6374 293a 2023 2074 6167 202d  , dict): # tag -
+00010650: 3e20 6c61 6d62 6461 200a 0909 0909 6675  > lambda .....fu
+00010660: 6e63 5b74 6167 5d28 646f 632c 2073 7461  nc[tag](doc, sta
+00010670: 7274 2c20 656e 642c 2074 6167 2920 6966  rt, end, tag) if
+00010680: 2074 6167 2069 6e20 6675 6e63 2065 6c73   tag in func els
+00010690: 6520 7072 696e 7428 2249 6e76 616c 6964  e print("Invalid
+000106a0: 2074 6167 3a22 2c20 7461 672c 2064 6f63   tag:", tag, doc
+000106b0: 5b73 7461 7274 3a65 6e64 5d2e 7465 7874  [start:end].text
+000106c0: 2920 0a09 0909 656c 7365 3a20 0a09 0909  ) ....else: ....
+000106d0: 0966 756e 6328 646f 632c 2073 7461 7274  .func(doc, start
+000106e0: 2c20 656e 642c 2074 6167 2920 2320 646f  , end, tag) # do
+000106f0: 632e 7370 616e 735b 6622 736b 656e 705b  c.spans[f"skenp[
+00010700: 7b73 7461 7274 7d2c 7b65 6e64 7d29 3a7b  {start},{end}):{
+00010710: 7461 677d 225d 203d 2053 7061 6e47 726f  tag}"] = SpanGro
+00010720: 7570 2864 6f63 2c20 6e61 6d65 3d74 6167  up(doc, name=tag
+00010730: 2c20 7370 616e 733d 5b20 646f 635b 7374  , spans=[ doc[st
+00010740: 6172 7420 3a20 656e 645d 205d 2c20 6174  art : end] ], at
+00010750: 7472 733d 7b7d 2920 2361 7474 7273 203d  trs={}) #attrs =
+00010760: 207b 2270 6f73 223a 2076 2e70 6f73 5f2c   {"pos": v.pos_,
+00010770: 2022 7461 6722 3a20 762e 7461 675f 2c20   "tag": v.tag_, 
+00010780: 2264 6570 223a 2076 2e64 6570 5f2c 2022  "dep": v.dep_, "
+00010790: 6c65 6d6d 6122 3a76 2e6c 656d 6d61 5f2c  lemma":v.lemma_,
+000107a0: 2022 656e 745f 7479 7065 223a 2022 532e   "ent_type": "S.
+000107b0: 2220 2b20 762e 6465 705f 207d 200a 0909  " + v.dep_ } ...
+000107c0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+000107d0: 2061 7320 653a 0a09 0909 7072 696e 7420   as e:....print 
+000107e0: 2822 736b 656e 705f 6d61 7463 6820 6578  ("skenp_match ex
+000107f0: 3a22 2c20 652c 206e 616d 652c 2073 7461  :", e, name, sta
+00010800: 7274 2c20 656e 6429 200a 0909 0965 7863  rt, end) ....exc
+00010810: 5f74 7970 652c 2065 7863 5f76 616c 7565  _type, exc_value
+00010820: 2c20 6578 635f 6f62 6a20 3d20 7379 732e  , exc_obj = sys.
+00010830: 6578 635f 696e 666f 2829 2009 0a09 0909  exc_info() .....
+00010840: 7472 6163 6562 6163 6b2e 7072 696e 745f  traceback.print_
+00010850: 7462 2865 7863 5f6f 626a 290a 0a64 6566  tb(exc_obj)..def
+00010860: 2074 7270 335f 6d61 7463 6828 646f 632c   trp3_match(doc,
+00010870: 2066 756e 633d 6c61 6d62 6461 2064 6f63   func=lambda doc
+00010880: 2c69 2c6a 2c6b 2c74 6167 3a20 646f 632e  ,i,j,k,tag: doc.
+00010890: 7370 616e 732e 7570 6461 7465 287b 6622  spans.update({f"
+000108a0: 7472 7033 5b7b 697d 2c7b 6a7d 2c7b 6b7d  trp3[{i},{j},{k}
+000108b0: 5d3a 7b74 6167 7d22 3a20 5370 616e 4772  ]:{tag}": SpanGr
+000108c0: 6f75 7028 646f 632c 206e 616d 653d 7461  oup(doc, name=ta
+000108d0: 672c 2073 7061 6e73 3d5b 2064 6f63 5b69  g, spans=[ doc[i
+000108e0: 3a69 2b31 5d2c 2064 6f63 5b6a 3a6a 2b31  :i+1], doc[j:j+1
+000108f0: 5d2c 2064 6f63 5b6b 3a6b 2b31 5d20 5d2c  ], doc[k:k+1] ],
+00010900: 2061 7474 7273 3d7b 2274 6167 223a 7461   attrs={"tag":ta
+00010910: 672c 2022 6922 3a69 2c22 6a22 3a6a 2c20  g, "i":i,"j":j, 
+00010920: 226b 223a 6b7d 2920 7d20 2929 3a0a 0969  "k":k}) } )):..i
+00010930: 6620 6e6f 7420 6861 7361 7474 7228 7472  f not hasattr(tr
+00010940: 7033 5f6d 6174 6368 2c20 276d 6174 6368  p3_match, 'match
+00010950: 6572 2729 3a20 0a09 0974 7270 335f 6d61  er'): ...trp3_ma
+00010960: 7463 682e 6d61 7463 6865 7220 3d20 4465  tch.matcher = De
+00010970: 704d 6174 6368 6572 287b 0a09 0922 646f  pMatcher({..."do
+00010980: 626a 2d61 6476 6d6f 6422 3a5b 207b 2252  bj-advmod":[ {"R
+00010990: 4947 4854 5f49 4422 3a20 2276 222c 2020  IGHT_ID": "v",  
 000109a0: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
-000109b0: 2244 4550 223a 2022 616d 6f64 227d 7d5d  "DEP": "amod"}}]
-000109c0: 2c20 2320 312c 342c 3320 2074 6865 206c  , # 1,4,3  the l
-000109d0: 6173 7420 6f6e 6520 6973 2074 6865 2061  ast one is the a
-000109e0: 646a 200a 0909 226e 6261 223a 5b20 7b22  dj ..."nba":[ {"
-000109f0: 5249 4748 545f 4944 223a 2022 7622 2c22  RIGHT_ID": "v","
-00010a00: 5249 4748 545f 4154 5452 5322 3a20 7b22  RIGHT_ATTRS": {"
-00010a10: 4c45 4d4d 4122 3a20 2262 6522 7d7d 2c7b  LEMMA": "be"}},{
-00010a20: 224c 4546 545f 4944 223a 2022 7622 2c20  "LEFT_ID": "v", 
-00010a30: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
-00010a40: 5249 4748 545f 4944 223a 2022 7375 626a  RIGHT_ID": "subj
-00010a50: 6563 7422 2c20 2252 4947 4854 5f41 5454  ect", "RIGHT_ATT
-00010a60: 5253 223a 207b 2244 4550 223a 2022 6e73  RS": {"DEP": "ns
-00010a70: 7562 6a22 2c20 2250 4f53 223a 224e 4f55  ubj", "POS":"NOU
-00010a80: 4e22 7d7d 2c7b 224c 4546 545f 4944 223a  N"}},{"LEFT_ID":
-00010a90: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
-00010aa0: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
-00010ab0: 2022 6f62 6a65 6374 222c 2252 4947 4854   "object","RIGHT
-00010ac0: 5f41 5454 5253 223a 207b 2244 4550 223a  _ATTRS": {"DEP":
-00010ad0: 2022 6163 6f6d 7022 7d7d 5d2c 2020 2320   "acomp"}}],  # 
-00010ae0: 6661 7465 2069 7320 676f 6f64 2c20 6669  fate is good, fi
-00010af0: 6c6d 3a4e 4f55 4e3a 6e62 613a 4144 4a0a  lm:NOUN:nba:ADJ.
-00010b00: 0909 226e 626e 223a 5b20 7b22 5249 4748  .."nbn":[ {"RIGH
-00010b10: 545f 4944 223a 2022 7622 2c22 5249 4748  T_ID": "v","RIGH
-00010b20: 545f 4154 5452 5322 3a20 7b22 4c45 4d4d  T_ATTRS": {"LEMM
-00010b30: 4122 3a20 2262 6522 7d7d 2c7b 224c 4546  A": "be"}},{"LEF
-00010b40: 545f 4944 223a 2022 7622 2c20 2252 454c  T_ID": "v", "REL
-00010b50: 5f4f 5022 3a20 223e 222c 2022 5249 4748  _OP": ">", "RIGH
-00010b60: 545f 4944 223a 2022 7375 626a 6563 7422  T_ID": "subject"
-00010b70: 2c20 2252 4947 4854 5f41 5454 5253 223a  , "RIGHT_ATTRS":
-00010b80: 207b 2244 4550 223a 2022 6e73 7562 6a22   {"DEP": "nsubj"
-00010b90: 2c20 2250 4f53 223a 224e 4f55 4e22 7d7d  , "POS":"NOUN"}}
-00010ba0: 2c7b 224c 4546 545f 4944 223a 2022 7622  ,{"LEFT_ID": "v"
-00010bb0: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
-00010bc0: 2022 5249 4748 545f 4944 223a 2022 6f62   "RIGHT_ID": "ob
-00010bd0: 6a65 6374 222c 2252 4947 4854 5f41 5454  ject","RIGHT_ATT
-00010be0: 5253 223a 207b 2244 4550 223a 2022 6174  RS": {"DEP": "at
-00010bf0: 7472 222c 2022 504f 5322 3a22 4e4f 554e  tr", "POS":"NOUN
-00010c00: 227d 7d5d 2c20 2023 2073 6365 6e65 2069  "}}],  # scene i
-00010c10: 7320 6120 7374 6f72 790a 0909 226e 6263  s a story..."nbc
-00010c20: 223a 5b20 7b22 5249 4748 545f 4944 223a  ":[ {"RIGHT_ID":
-00010c30: 2022 7622 2c22 5249 4748 545f 4154 5452   "v","RIGHT_ATTR
-00010c40: 5322 3a20 7b22 4c45 4d4d 4122 3a20 2262  S": {"LEMMA": "b
-00010c50: 6522 7d7d 2c7b 224c 4546 545f 4944 223a  e"}},{"LEFT_ID":
-00010c60: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
-00010c70: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
-00010c80: 2022 7375 626a 6563 7422 2c20 2252 4947   "subject", "RIG
-00010c90: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
-00010ca0: 223a 2022 6e73 7562 6a22 7d7d 2c7b 224c  ": "nsubj"}},{"L
-00010cb0: 4546 545f 4944 223a 2022 7622 2c20 2252  EFT_ID": "v", "R
-00010cc0: 454c 5f4f 5022 3a20 223e 222c 2022 5249  EL_OP": ">", "RI
-00010cd0: 4748 545f 4944 223a 2022 636c 222c 2252  GHT_ID": "cl","R
-00010ce0: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
-00010cf0: 4550 223a 2022 6363 6f6d 7022 7d7d 5d2c  EP": "ccomp"}}],
-00010d00: 2020 2320 796f 7520 6172 6520 7768 6174    # you are what
-00010d10: 2079 6f75 2072 6561 640a 0909 2261 6476   you read..."adv
-00010d20: 636c 2d61 636f 6d70 223a 5b20 7b22 5249  cl-acomp":[ {"RI
-00010d30: 4748 545f 4944 223a 2022 7622 2c20 2022  GHT_ID": "v",  "
-00010d40: 5249 4748 545f 4154 5452 5322 3a20 7b22  RIGHT_ATTRS": {"
-00010d50: 504f 5322 3a20 2256 4552 4222 7d7d 2c20  POS": "VERB"}}, 
-00010d60: 7b22 4c45 4654 5f49 4422 3a20 2276 222c  {"LEFT_ID": "v",
-00010d70: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
-00010d80: 2252 4947 4854 5f49 4422 3a20 2263 6c76  "RIGHT_ID": "clv
-00010d90: 222c 2022 5249 4748 545f 4154 5452 5322  ", "RIGHT_ATTRS"
-00010da0: 3a20 7b22 4445 5022 3a20 2261 6476 636c  : {"DEP": "advcl
-00010db0: 227d 7d2c 7b22 4c45 4654 5f49 4422 3a20  "}},{"LEFT_ID": 
-00010dc0: 2263 6c76 222c 2022 5245 4c5f 4f50 223a  "clv", "REL_OP":
-00010dd0: 2022 3e22 2c20 2252 4947 4854 5f49 4422   ">", "RIGHT_ID"
-00010de0: 3a20 226f 626a 6563 7422 2c22 5249 4748  : "object","RIGH
-00010df0: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
-00010e00: 3a20 2261 636f 6d70 227d 7d5d 2c20 2023  : "acomp"}}],  #
-00010e10: 2022 5768 696c 6520 4920 7761 7320 7468   "While I was th
-00010e20: 7269 6c6c 6564 2074 6861 7420 6974 2063  rilled that it c
-00010e30: 7269 6564 2c20 4920 776f 7272 6965 6420  ried, I worried 
-00010e40: 7468 6174 2049 2077 6f75 6c64 2066 6169  that I would fai
-00010e50: 6c2e 0a09 0922 646f 626a 2d70 7274 223a  l...."dobj-prt":
-00010e60: 2020 5b20 7b22 5249 4748 545f 4944 223a    [ {"RIGHT_ID":
-00010e70: 2022 7622 2c20 2022 5249 4748 545f 4154   "v",  "RIGHT_AT
-00010e80: 5452 5322 3a20 7b22 504f 5322 3a20 2256  TRS": {"POS": "V
-00010e90: 4552 4222 7d7d 2c7b 224c 4546 545f 4944  ERB"}},{"LEFT_ID
-00010ea0: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
-00010eb0: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
-00010ec0: 223a 2022 7072 7422 2c22 5249 4748 545f  ": "prt","RIGHT_
-00010ed0: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
-00010ee0: 2270 7274 227d 2020 7d2c 207b 224c 4546  "prt"}  }, {"LEF
-00010ef0: 545f 4944 223a 2022 7622 2c20 2252 454c  T_ID": "v", "REL
-00010f00: 5f4f 5022 3a20 223e 222c 2022 5249 4748  _OP": ">", "RIGH
-00010f10: 545f 4944 223a 2022 6e22 2c20 2252 4947  T_ID": "n", "RIG
-00010f20: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
-00010f30: 223a 2022 646f 626a 222c 2022 504f 5322  ": "dobj", "POS"
-00010f40: 3a22 4e4f 554e 222c 2249 535f 414c 5048  :"NOUN","IS_ALPH
-00010f50: 4122 3a54 7275 652c 2249 535f 4c4f 5745  A":True,"IS_LOWE
-00010f60: 5222 3a54 7275 657d 7d5d 2c20 2320 7475  R":True}}], # tu
-00010f70: 726e 206f 6666 2074 6865 2072 6164 696f  rn off the radio
-00010f80: 200a 0909 2276 704e 223a 205b 207b 2252   ..."vpN": [ {"R
-00010f90: 4947 4854 5f49 4422 3a20 2276 222c 2020  IGHT_ID": "v",  
-00010fa0: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
-00010fb0: 2250 4f53 223a 2022 5645 5242 222c 2249  "POS": "VERB","I
-00010fc0: 535f 414c 5048 4122 3a54 7275 657d 7d2c  S_ALPHA":True}},
-00010fd0: 7b22 4c45 4654 5f49 4422 3a20 2276 222c  {"LEFT_ID": "v",
-00010fe0: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
-00010ff0: 2252 4947 4854 5f49 4422 3a20 2270 7265  "RIGHT_ID": "pre
-00011000: 7022 2c22 5249 4748 545f 4154 5452 5322  p","RIGHT_ATTRS"
-00011010: 3a20 7b22 4445 5022 3a20 2270 7265 7022  : {"DEP": "prep"
-00011020: 2c22 4953 5f4c 4f57 4552 223a 5472 7565  ,"IS_LOWER":True
-00011030: 2c22 4953 5f41 4c50 4841 223a 5472 7565  ,"IS_ALPHA":True
-00011040: 7d20 207d 2c20 7b22 4c45 4654 5f49 4422  }  }, {"LEFT_ID"
-00011050: 3a20 2270 7265 7022 2c20 2252 454c 5f4f  : "prep", "REL_O
-00011060: 5022 3a20 223e 222c 2022 5249 4748 545f  P": ">", "RIGHT_
-00011070: 4944 223a 2022 6e22 2c20 2252 4947 4854  ID": "n", "RIGHT
-00011080: 5f41 5454 5253 223a 207b 2244 4550 223a  _ATTRS": {"DEP":
-00011090: 2022 706f 626a 222c 2022 504f 5322 3a22   "pobj", "POS":"
-000110a0: 4e4f 554e 222c 2249 535f 414c 5048 4122  NOUN","IS_ALPHA"
-000110b0: 3a54 7275 657d 7d5d 2c20 2320 6a75 6d70  :True}}], # jump
-000110c0: 206f 7665 7220 7468 6520 646f 672c 2064   over the dog, d
-000110d0: 6966 6620 6672 6f6d 2063 6f6d 6520 696e  iff from come in
-000110e0: 746f 2066 6f72 6365 2f4e 4e0a 0909 7d29  to force/NN...})
-000110f0: 2020 2320 6e62 653f 206e 6278 203d 206e    # nbe? nbx = n
-00011100: 6261 202b 206e 6265 202b 206e 626e 0a09  ba + nbe + nbn..
-00011110: 666f 7220 6e61 6d65 2c20 6172 2069 6e20  for name, ar in 
-00011120: 7472 7033 5f6d 6174 6368 2e6d 6174 6368  trp3_match.match
-00011130: 6572 2864 6f63 293a 0a09 0974 7279 3a0a  er(doc):...try:.
-00011140: 0909 0974 6167 203d 2073 7061 6379 2e6e  ...tag = spacy.n
-00011150: 6c70 2e76 6f63 6162 5b6e 616d 655d 2e74  lp.vocab[name].t
-00011160: 6578 740a 0909 0969 2c6a 2c6b 203d 2061  ext....i,j,k = a
-00011170: 725b 303a 335d 200a 0909 0969 6620 6973  r[0:3] ....if is
-00011180: 696e 7374 616e 6365 2866 756e 632c 2064  instance(func, d
-00011190: 6963 7429 3a20 2320 7461 6720 2d3e 206c  ict): # tag -> l
-000111a0: 616d 6264 6120 0a09 0909 0966 756e 635b  ambda .....func[
-000111b0: 7461 675d 2864 6f63 2c20 692c 206a 2c20  tag](doc, i, j, 
-000111c0: 6b2c 2074 6167 2920 6966 2074 6167 2069  k, tag) if tag i
-000111d0: 6e20 6675 6e63 2065 6c73 6520 7072 696e  n func else prin
-000111e0: 7428 2249 6e76 616c 6964 2074 6167 3a22  t("Invalid tag:"
-000111f0: 2c20 7461 672c 2069 2c6a 2c6b 2029 0a09  , tag, i,j,k )..
-00011200: 0909 656c 7365 3a20 0a09 0909 0966 756e  ..else: .....fun
-00011210: 6328 646f 632c 2069 2c20 6a2c 206b 2c20  c(doc, i, j, k, 
-00011220: 7461 6729 2023 2064 6f63 2e73 7061 6e73  tag) # doc.spans
-00011230: 5b66 2274 7270 335b 7b69 7d2c 7b6a 7d2c  [f"trp3[{i},{j},
-00011240: 7b6b 7d5d 3a7b 7461 677d 225d 203d 2053  {k}]:{tag}"] = S
-00011250: 7061 6e47 726f 7570 2864 6f63 2c20 6e61  panGroup(doc, na
-00011260: 6d65 3d74 6167 2c20 7370 616e 733d 5b20  me=tag, spans=[ 
-00011270: 646f 635b 693a 692b 315d 2c20 646f 635b  doc[i:i+1], doc[
-00011280: 6a3a 6a2b 315d 2c20 646f 635b 6b3a 6b2b  j:j+1], doc[k:k+
-00011290: 315d 205d 2c20 6174 7472 733d 7b22 7461  1] ], attrs={"ta
-000112a0: 6722 3a74 6167 2c20 2269 223a 692c 226a  g":tag, "i":i,"j
-000112b0: 223a 6a2c 2022 6b22 3a6b 7d29 200a 0909  ":j, "k":k}) ...
-000112c0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-000112d0: 2061 7320 653a 0a09 0909 7072 696e 7420   as e:....print 
-000112e0: 2822 7472 7033 5f6d 6174 6368 2065 783a  ("trp3_match ex:
-000112f0: 222c 2065 2c20 6e61 6d65 2c20 6172 2920  ", e, name, ar) 
-00011300: 0a0a 7370 616e 5f4e 5020 3d20 6c61 6d62  ..span_NP = lamb
-00011310: 6461 2073 703a 2022 2022 2e6a 6f69 6e28  da sp: " ".join(
-00011320: 5b20 225f 4e50 2220 6966 2074 2e65 6e74  [ "_NP" if t.ent
-00011330: 5f74 7970 655f 203d 3d20 274e 5027 2065  _type_ == 'NP' e
-00011340: 6c73 6520 742e 7465 7874 2e6c 6f77 6572  lse t.text.lower
-00011350: 2829 2066 6f72 2074 2069 6e20 7370 5d29  () for t in sp])
-00011360: 2023 656c 7365 2066 225f 7b74 2e74 6167   #else f"_{t.tag
-00011370: 5f7d 2220 6966 2074 2e74 6167 5f20 696e  _}" if t.tag_ in
-00011380: 2028 2756 424e 2729 0a64 6566 2073 6b65   ('VBN').def ske
-00011390: 6e70 5f66 756e 635f 6b70 2864 6f63 2c20  np_func_kp(doc, 
-000113a0: 7374 6172 742c 2065 6e64 2c20 7461 6729  start, end, tag)
-000113b0: 3a20 2320 736b 656e 705f 6675 6e63 5f6b  : # skenp_func_k
-000113c0: 7009 3d20 6c61 6d62 6461 2064 6f63 2c20  p.= lambda doc, 
-000113d0: 7374 6172 742c 2065 6e64 2c20 7461 673a  start, end, tag:
-000113e0: 2064 6f63 2e75 7365 725f 6461 7461 2e75   doc.user_data.u
-000113f0: 7064 6174 6528 7b66 227b 7461 677d 3a7b  pdate({f"{tag}:{
-00011400: 646f 635b 7374 6172 745d 2e6c 656d 6d61  doc[start].lemma
-00011410: 5f7d 2022 202b 2073 7061 6e5f 4e50 2864  _} " + span_NP(d
-00011420: 6f63 5b73 7461 7274 2b31 3a65 6e64 5d29  oc[start+1:end])
-00011430: 203a 207b 2276 6c65 6d22 3a64 6f63 5b73   : {"vlem":doc[s
-00011440: 7461 7274 5d2e 6c65 6d6d 615f 2c20 2273  tart].lemma_, "s
-00011450: 7461 7274 223a 7374 6172 742c 2022 656e  tart":start, "en
-00011460: 6422 3a65 6e64 2c20 226e 6163 223a 205b  d":end, "nac": [
-00011470: 6622 7b64 6f63 5b73 7461 7274 5d2e 6c65  f"{doc[start].le
-00011480: 6d6d 615f 7d3a 5645 5242 3a7b 7461 677d  mma_}:VERB:{tag}
-00011490: 7c22 202b 7370 616e 5f4e 5028 646f 635b  |" +span_NP(doc[
-000114a0: 7374 6172 743a 656e 645d 2029 2c20 6622  start:end] ), f"
-000114b0: 7b64 6f63 5b73 7461 7274 5d2e 6c65 6d6d  {doc[start].lemm
-000114c0: 615f 7d3a 5645 5242 7c7b 7461 677d 222c  a_}:VERB|{tag}",
-000114d0: 2066 222a 3a56 4552 427c 7b74 6167 7d22   f"*:VERB|{tag}"
-000114e0: 5d7d 207d 2920 0a09 6e61 6320 3d20 5b66  ]} }) ..nac = [f
-000114f0: 227b 646f 635b 7374 6172 745d 2e6c 656d  "{doc[start].lem
-00011500: 6d61 5f7d 3a56 4552 423a 7b74 6167 7d7c  ma_}:VERB:{tag}|
-00011510: 2220 2b73 7061 6e5f 4e50 2864 6f63 5b73  " +span_NP(doc[s
-00011520: 7461 7274 3a65 6e64 5d20 292c 2066 227b  tart:end] ), f"{
-00011530: 646f 635b 7374 6172 745d 2e6c 656d 6d61  doc[start].lemma
-00011540: 5f7d 3a56 4552 427c 7b74 6167 7d22 2c20  _}:VERB|{tag}", 
-00011550: 6622 2a3a 5645 5242 7c7b 7461 677d 225d  f"*:VERB|{tag}"]
-00011560: 0a09 6966 2074 6167 2069 6e20 2827 766e  ..if tag in ('vn
-00011570: 706e 2729 3a20 2320 7461 6b65 205f 4e50  pn'): # take _NP
-00011580: 2069 6e74 6f20 6163 636f 756e 742c 2061   into account, a
-00011590: 6464 6564 2032 3032 332e 322e 3134 0a09  dded 2023.2.14..
-000115a0: 096e 6163 2e65 7874 656e 6428 5b66 227b  .nac.extend([f"{
-000115b0: 646f 635b 656e 642d 315d 2e74 6578 742e  doc[end-1].text.
-000115c0: 6c6f 7765 7228 297d 3a4e 4f55 4e3a 7b74  lower()}:NOUN:{t
-000115d0: 6167 7d7c 2220 2b64 6f63 5b73 7461 7274  ag}|" +doc[start
-000115e0: 5d2e 6c65 6d6d 615f 202b 2022 2022 202b  ].lemma_ + " " +
-000115f0: 2073 7061 6e5f 4e50 2864 6f63 5b73 7461   span_NP(doc[sta
-00011600: 7274 2b31 3a65 6e64 2d31 5d29 202b 2022  rt+1:end-1]) + "
-00011610: 2022 202b 2064 6f63 5b65 6e64 2d31 5d2e   " + doc[end-1].
-00011620: 7465 7874 2e6c 6f77 6572 2829 2c20 6622  text.lower(), f"
-00011630: 7b64 6f63 5b65 6e64 2d31 5d2e 7465 7874  {doc[end-1].text
-00011640: 2e6c 6f77 6572 2829 7d3a 4e4f 554e 7c7b  .lower()}:NOUN|{
-00011650: 7461 677d 222c 2066 222a 3a4e 4f55 4e7c  tag}", f"*:NOUN|
-00011660: 7b74 6167 7d22 2c20 6622 7b64 6f63 5b65  {tag}", f"{doc[e
-00011670: 6e64 2d31 5d2e 7465 7874 2e6c 6f77 6572  nd-1].text.lower
-00011680: 2829 7d2f 4e4f 554e 7c7b 7461 677d 3a5f  ()}/NOUN|{tag}:_
-00011690: 2220 2b64 6f63 5b73 7461 7274 5d2e 6c65  " +doc[start].le
-000116a0: 6d6d 615f 202b 2022 2022 202b 2073 7061  mma_ + " " + spa
-000116b0: 6e5f 4e50 2864 6f63 5b73 7461 7274 2b31  n_NP(doc[start+1
-000116c0: 3a65 6e64 2d31 5d29 202b 2022 2022 202b  :end-1]) + " " +
-000116d0: 2064 6f63 5b65 6e64 2d31 5d2e 7465 7874   doc[end-1].text
-000116e0: 2e6c 6f77 6572 2829 5d29 0a09 6966 2074  .lower()])..if t
-000116f0: 6167 2069 6e20 2822 766e 7065 2229 3a20  ag in ("vnpe"): 
-00011700: 2320 7461 6b65 205f 4e50 2066 6f72 2067  # take _NP for g
-00011710: 7261 6e74 6564 0a09 096e 6163 2e65 7874  ranted...nac.ext
-00011720: 656e 6428 5b66 227b 646f 635b 656e 642d  end([f"{doc[end-
-00011730: 315d 2e6c 656d 6d61 5f7d 3a56 4552 423a  1].lemma_}:VERB:
-00011740: 7b74 6167 7d7c 2220 2b73 7061 6e5f 4e50  {tag}|" +span_NP
-00011750: 2864 6f63 5b73 7461 7274 3a65 6e64 5d29  (doc[start:end])
-00011760: 2c20 6622 7b64 6f63 5b65 6e64 2d31 5d2e  , f"{doc[end-1].
-00011770: 6c65 6d6d 615f 7d3a 5645 5242 7c7b 7461  lemma_}:VERB|{ta
-00011780: 677d 222c 2066 222a 3a56 4552 427c 7b74  g}", f"*:VERB|{t
-00011790: 6167 7d22 2c20 0a09 0909 6622 7b64 6f63  ag}", ....f"{doc
-000117a0: 5b65 6e64 2d31 5d2e 6c65 6d6d 615f 7d2f  [end-1].lemma_}/
-000117b0: 5645 5242 7c76 6e70 653a 5f7b 646f 635b  VERB|vnpe:_{doc[
-000117c0: 7374 6172 745d 2e6c 656d 6d61 5f7d 205f  start].lemma_} _
-000117d0: 4e50 2022 202b 646f 635b 7374 6172 742b  NP " +doc[start+
-000117e0: 323a 656e 645d 2e74 6578 742e 6c6f 7765  2:end].text.lowe
-000117f0: 7228 292c 5d29 0a09 6966 2074 6167 2069  r(),])..if tag i
-00011800: 6e20 2822 766e 2229 3a20 6e61 632e 6578  n ("vn"): nac.ex
-00011810: 7465 6e64 285b 6622 7b64 6f63 5b73 7461  tend([f"{doc[sta
-00011820: 7274 5d2e 6c65 6d6d 615f 7d2f 5645 5242  rt].lemma_}/VERB
-00011830: 7c76 6e3a 5f7b 646f 635b 7374 6172 745d  |vn:_{doc[start]
-00011840: 2e6c 656d 6d61 5f7d 205f 4e50 225d 290a  .lemma_} _NP"]).
-00011850: 0969 6620 7461 6720 3d3d 2022 766e 6122  .if tag == "vna"
-00011860: 3a20 6e61 632e 6578 7465 6e64 285b 6622  : nac.extend([f"
-00011870: 7b64 6f63 5b73 7461 7274 5d2e 6c65 6d6d  {doc[start].lemm
-00011880: 615f 7d2f 5645 5242 7c76 6e61 3a5f 7b64  a_}/VERB|vna:_{d
-00011890: 6f63 5b73 7461 7274 5d2e 6c65 6d6d 615f  oc[start].lemma_
-000118a0: 7d20 5f4e 5020 5f41 444a 225d 290a 0969  } _NP _ADJ"])..i
-000118b0: 6620 7461 6720 696e 2028 2276 6e6e 2229  f tag in ("vnn")
-000118c0: 3a20 6e61 632e 6578 7465 6e64 285b 6622  : nac.extend([f"
-000118d0: 7b64 6f63 5b73 7461 7274 5d2e 6c65 6d6d  {doc[start].lemm
-000118e0: 615f 7d2f 5645 5242 7c76 6e6e 3a5f 7b64  a_}/VERB|vnn:_{d
-000118f0: 6f63 5b73 7461 7274 5d2e 6c65 6d6d 615f  oc[start].lemma_
-00011900: 7d20 5f4e 5020 5f4e 5022 5d29 0a09 6966  } _NP _NP"])..if
-00011910: 2074 6167 2069 6e20 2822 766e 6522 293a   tag in ("vne"):
-00011920: 206e 6163 2e65 7874 656e 6428 5b66 227b   nac.extend([f"{
-00011930: 646f 635b 7374 6172 745d 2e6c 656d 6d61  doc[start].lemma
-00011940: 5f7d 2f56 4552 427c 766e 653a 5f7b 646f  _}/VERB|vne:_{do
-00011950: 635b 7374 6172 745d 2e6c 656d 6d61 5f7d  c[start].lemma_}
-00011960: 205f 4e50 205f 5642 4e22 5d29 0a09 646f   _NP _VBN"])..do
-00011970: 632e 7573 6572 5f64 6174 612e 7570 6461  c.user_data.upda
-00011980: 7465 287b 6622 7b74 6167 7d3a 7b64 6f63  te({f"{tag}:{doc
-00011990: 5b73 7461 7274 5d2e 6c65 6d6d 615f 7d20  [start].lemma_} 
-000119a0: 2220 2b20 7370 616e 5f4e 5028 646f 635b  " + span_NP(doc[
-000119b0: 7374 6172 742b 313a 656e 645d 2920 3a20  start+1:end]) : 
-000119c0: 7b22 766c 656d 223a 646f 635b 7374 6172  {"vlem":doc[star
-000119d0: 745d 2e6c 656d 6d61 5f2c 2022 7374 6172  t].lemma_, "star
-000119e0: 7422 3a73 7461 7274 2c20 2265 6e64 223a  t":start, "end":
-000119f0: 656e 642c 2022 6e61 6322 3a6e 6163 7d20  end, "nac":nac} 
-00011a00: 7d29 0a0a 7472 7033 5f66 756e 635f 6b70  })..trp3_func_kp
-00011a10: 203d 207b 2023 6472 696e 6b3a 5645 5242   = { #drink:VERB
-00011a20: 3a64 6f62 6a3a 4e4f 554e 3a77 6174 6572  :dobj:NOUN:water
-00011a30: 3a61 6d6f 643a 4144 4a20 7361 6665 0a09  :amod:ADJ safe..
-00011a40: 2264 6f62 6a2d 6164 766d 6f64 223a 096c  "dobj-advmod":.l
-00011a50: 616d 6264 6120 646f 632c 2069 2c20 6a2c  ambda doc, i, j,
-00011a60: 206b 2c20 7461 673a 2020 646f 632e 7573   k, tag:  doc.us
-00011a70: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
-00011a80: 6622 646f 626a 2d61 6476 6d6f 643a 7b64  f"dobj-advmod:{d
-00011a90: 6f63 5b6b 5d2e 7465 7874 7d20 7b64 6f63  oc[k].text} {doc
-00011aa0: 5b69 5d2e 6c65 6d6d 615f 7d20 7b64 6f63  [i].lemma_} {doc
-00011ab0: 5b6a 5d2e 6c65 6d6d 615f 7d5b 7b69 7d2c  [j].lemma_}[{i},
-00011ac0: 7b6a 7d2c 7b6b 7d5d 223a 207b 2274 6167  {j},{k}]": {"tag
-00011ad0: 223a 7461 672c 2022 6672 6f6d 223a 2274  ":tag, "from":"t
-00011ae0: 7270 3322 202c 0a09 0909 0909 0922 6e61  rp3" ,......."na
-00011af0: 6322 3a5b 6622 7b64 6f63 5b69 5d2e 6c65  c":[f"{doc[i].le
-00011b00: 6d6d 615f 7d3a 7b64 6f63 5b69 5d2e 706f  mma_}:{doc[i].po
-00011b10: 735f 7d3a 7b64 6f63 5b6a 5d2e 6465 705f  s_}:{doc[j].dep_
-00011b20: 7d3a 7b64 6f63 5b6a 5d2e 706f 735f 7d3a  }:{doc[j].pos_}:
-00011b30: 7b64 6f63 5b6a 5d2e 6c65 6d6d 615f 7d3a  {doc[j].lemma_}:
-00011b40: 7b64 6f63 5b6b 5d2e 6465 705f 7d2d 7b64  {doc[k].dep_}-{d
-00011b50: 6f63 5b6b 5d2e 706f 735f 7d7c 7b64 6f63  oc[k].pos_}|{doc
-00011b60: 5b6b 5d2e 6c65 6d6d 615f 7d22 2c66 227b  [k].lemma_}",f"{
-00011b70: 646f 635b 695d 2e6c 656d 6d61 5f7d 3a7b  doc[i].lemma_}:{
-00011b80: 646f 635b 695d 2e70 6f73 5f7d 3a7b 646f  doc[i].pos_}:{do
-00011b90: 635b 6a5d 2e64 6570 5f7d 3a7b 646f 635b  c[j].dep_}:{doc[
-00011ba0: 6a5d 2e70 6f73 5f7d 3a7b 646f 635b 6a5d  j].pos_}:{doc[j]
-00011bb0: 2e6c 656d 6d61 5f7d 7c7b 646f 635b 6b5d  .lemma_}|{doc[k]
-00011bc0: 2e64 6570 5f7d 2d7b 646f 635b 6b5d 2e70  .dep_}-{doc[k].p
-00011bd0: 6f73 5f7d 225d 7d7d 292c 200a 0922 646f  os_}"]}}), .."do
-00011be0: 626a 2d61 6d6f 6422 3a09 6c61 6d62 6461  bj-amod":.lambda
-00011bf0: 2064 6f63 2c20 692c 206a 2c20 6b2c 2074   doc, i, j, k, t
-00011c00: 6167 3a20 2064 6f63 2e75 7365 725f 6461  ag:  doc.user_da
-00011c10: 7461 2e75 7064 6174 6528 7b66 2264 6f62  ta.update({f"dob
-00011c20: 6a2d 616d 6f64 3a7b 646f 635b 695d 2e6c  j-amod:{doc[i].l
-00011c30: 656d 6d61 5f7d 207b 646f 635b 6a5d 2e74  emma_} {doc[j].t
-00011c40: 6578 747d 207b 646f 635b 6b5d 2e6c 656d  ext} {doc[k].lem
-00011c50: 6d61 5f7d 5b7b 697d 2c7b 6a7d 2c7b 6b7d  ma_}[{i},{j},{k}
-00011c60: 5d22 3a20 7b22 7461 6722 3a74 6167 2c20  ]": {"tag":tag, 
-00011c70: 2266 726f 6d22 3a22 7472 7033 2220 2c0a  "from":"trp3" ,.
-00011c80: 0909 0909 0909 226e 6163 223a 5b66 227b  ......"nac":[f"{
-00011c90: 646f 635b 695d 2e6c 656d 6d61 5f7d 3a7b  doc[i].lemma_}:{
-00011ca0: 646f 635b 695d 2e70 6f73 5f7d 3a7b 646f  doc[i].pos_}:{do
-00011cb0: 635b 6a5d 2e64 6570 5f7d 3a7b 646f 635b  c[j].dep_}:{doc[
-00011cc0: 6a5d 2e70 6f73 5f7d 3a7b 646f 635b 6a5d  j].pos_}:{doc[j]
-00011cd0: 2e6c 656d 6d61 5f7d 3a7b 646f 635b 6b5d  .lemma_}:{doc[k]
-00011ce0: 2e64 6570 5f7d 2d7b 646f 635b 6b5d 2e70  .dep_}-{doc[k].p
-00011cf0: 6f73 5f7d 7c7b 646f 635b 6b5d 2e6c 656d  os_}|{doc[k].lem
-00011d00: 6d61 5f7d 222c 6622 7b64 6f63 5b69 5d2e  ma_}",f"{doc[i].
-00011d10: 6c65 6d6d 615f 7d3a 7b64 6f63 5b69 5d2e  lemma_}:{doc[i].
-00011d20: 706f 735f 7d3a 7b64 6f63 5b6a 5d2e 6465  pos_}:{doc[j].de
-00011d30: 705f 7d3a 7b64 6f63 5b6a 5d2e 706f 735f  p_}:{doc[j].pos_
-00011d40: 7d3a 7b64 6f63 5b6a 5d2e 6c65 6d6d 615f  }:{doc[j].lemma_
-00011d50: 7d7c 7b64 6f63 5b6b 5d2e 6465 705f 7d2d  }|{doc[k].dep_}-
-00011d60: 7b64 6f63 5b6b 5d2e 706f 735f 7d22 5d7d  {doc[k].pos_}"]}
-00011d70: 7d29 2c20 0a09 226e 6261 223a 0909 096c  }), .."nba":...l
-00011d80: 616d 6264 6120 646f 632c 2069 2c20 6a2c  ambda doc, i, j,
-00011d90: 206b 2c20 7461 673a 2020 646f 632e 7573   k, tag:  doc.us
-00011da0: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
-00011db0: 6622 6e62 613a 7b64 6f63 5b6a 5d2e 6c65  f"nba:{doc[j].le
-00011dc0: 6d6d 615f 7d20 7b64 6f63 5b6b 5d2e 7465  mma_} {doc[k].te
-00011dd0: 7874 7d5b 7b69 7d2c 7b6a 7d2c 7b6b 7d5d  xt}[{i},{j},{k}]
-00011de0: 223a 7b22 7461 6722 3a74 6167 2c20 2266  ":{"tag":tag, "f
-00011df0: 726f 6d22 3a22 7472 7033 222c 2023 2077  rom":"trp3", # w
-00011e00: 6865 6e20 7468 6572 6520 6973 206e 6f20  hen there is no 
-00011e10: 616d 6269 2c20 6e6f 206e 6565 6420 746f  ambi, no need to
-00011e20: 2061 6464 207e 200a 0909 0909 0909 226e   add ~ ......."n
-00011e30: 6163 223a 5b66 227b 646f 635b 6a5d 2e6c  ac":[f"{doc[j].l
-00011e40: 656d 6d61 5f7d 3a7b 646f 635b 6a5d 2e70  emma_}:{doc[j].p
-00011e50: 6f73 5f7d 3a7b 7461 677d 7c7b 646f 635b  os_}:{tag}|{doc[
-00011e60: 6b5d 2e6c 656d 6d61 5f7d 222c 6622 7b64  k].lemma_}",f"{d
-00011e70: 6f63 5b6a 5d2e 6c65 6d6d 615f 7d3a 7b64  oc[j].lemma_}:{d
-00011e80: 6f63 5b6a 5d2e 706f 735f 7d7c 7b74 6167  oc[j].pos_}|{tag
-00011e90: 7d22 2c66 227b 646f 635b 6b5d 2e6c 656d  }",f"{doc[k].lem
-00011ea0: 6d61 5f7d 3a7b 646f 635b 6b5d 2e70 6f73  ma_}:{doc[k].pos
-00011eb0: 5f7d 3a7b 7461 677d 7c7b 646f 635b 6a5d  _}:{tag}|{doc[j]
-00011ec0: 2e6c 656d 6d61 5f7d 222c 6622 7b64 6f63  .lemma_}",f"{doc
-00011ed0: 5b6b 5d2e 6c65 6d6d 615f 7d3a 7b64 6f63  [k].lemma_}:{doc
-00011ee0: 5b6b 5d2e 706f 735f 7d7c 7b74 6167 7d22  [k].pos_}|{tag}"
-00011ef0: 5d7d 7d29 2c20 0a09 226e 626e 223a 0909  ]}}), .."nbn":..
-00011f00: 096c 616d 6264 6120 646f 632c 2069 2c20  .lambda doc, i, 
-00011f10: 6a2c 206b 2c20 7461 673a 2020 646f 632e  j, k, tag:  doc.
-00011f20: 7573 6572 5f64 6174 612e 7570 6461 7465  user_data.update
-00011f30: 287b 6622 6e62 6e3a 7b64 6f63 5b6a 5d2e  ({f"nbn:{doc[j].
-00011f40: 6c65 6d6d 615f 7d20 7b64 6f63 5b6b 5d2e  lemma_} {doc[k].
-00011f50: 6c65 6d6d 615f 7d5b 7b69 7d2c 7b6a 7d2c  lemma_}[{i},{j},
-00011f60: 7b6b 7d5d 223a 7b22 7461 6722 3a74 6167  {k}]":{"tag":tag
-00011f70: 2c20 2266 726f 6d22 3a22 7472 7033 222c  , "from":"trp3",
-00011f80: 0a09 0909 0909 0922 6e61 6322 3a5b 6622  ......."nac":[f"
-00011f90: 7b64 6f63 5b6a 5d2e 6c65 6d6d 615f 7d3a  {doc[j].lemma_}:
-00011fa0: 7b64 6f63 5b6a 5d2e 706f 735f 7d3a 7b74  {doc[j].pos_}:{t
-00011fb0: 6167 7d7c 7b64 6f63 5b6b 5d2e 6c65 6d6d  ag}|{doc[k].lemm
-00011fc0: 615f 7d22 2c66 227b 646f 635b 6a5d 2e6c  a_}",f"{doc[j].l
-00011fd0: 656d 6d61 5f7d 3a7b 646f 635b 6a5d 2e70  emma_}:{doc[j].p
-00011fe0: 6f73 5f7d 7c7b 7461 677d 222c 6622 7b64  os_}|{tag}",f"{d
-00011ff0: 6f63 5b6b 5d2e 6c65 6d6d 615f 7d3a 7b64  oc[k].lemma_}:{d
-00012000: 6f63 5b6b 5d2e 706f 735f 7d3a 7e7b 7461  oc[k].pos_}:~{ta
-00012010: 677d 7c7b 646f 635b 6a5d 2e6c 656d 6d61  g}|{doc[j].lemma
-00012020: 5f7d 222c 6622 7b64 6f63 5b6b 5d2e 6c65  _}",f"{doc[k].le
-00012030: 6d6d 615f 7d3a 7b64 6f63 5b6b 5d2e 706f  mma_}:{doc[k].po
-00012040: 735f 7d7c 7e7b 7461 677d 225d 7d7d 292c  s_}|~{tag}"]}}),
-00012050: 200a 0922 6e62 6322 3a09 0909 6c61 6d62   .."nbc":...lamb
-00012060: 6461 2064 6f63 2c20 692c 206a 2c20 6b2c  da doc, i, j, k,
-00012070: 2074 6167 3a20 2064 6f63 2e75 7365 725f   tag:  doc.user_
-00012080: 6461 7461 2e75 7064 6174 6528 7b66 226e  data.update({f"n
-00012090: 6263 3a7b 646f 635b 6a5d 2e6c 656d 6d61  bc:{doc[j].lemma
-000120a0: 5f7d 205f 434c 5b7b 697d 2c7b 6a7d 2c7b  _} _CL[{i},{j},{
-000120b0: 6b7d 5d22 3a7b 2274 6167 223a 7461 672c  k}]":{"tag":tag,
-000120c0: 2022 6672 6f6d 223a 2274 7270 3322 2c0a   "from":"trp3",.
-000120d0: 0909 0909 0909 226e 6163 223a 5b66 227b  ......"nac":[f"{
-000120e0: 646f 635b 6a5d 2e6c 656d 6d61 5f7d 3a7b  doc[j].lemma_}:{
-000120f0: 646f 635b 6a5d 2e70 6f73 5f7d 7c7b 7461  doc[j].pos_}|{ta
-00012100: 677d 225d 7d7d 292c 200a 0922 6164 7663  g}"]}}), .."advc
-00012110: 6c2d 6163 6f6d 7022 3a09 6c61 6d62 6461  l-acomp":.lambda
-00012120: 2064 6f63 2c20 692c 206a 2c20 6b2c 2074   doc, i, j, k, t
-00012130: 6167 3a20 2064 6f63 2e75 7365 725f 6461  ag:  doc.user_da
-00012140: 7461 2e75 7064 6174 6528 7b66 2261 6476  ta.update({f"adv
-00012150: 636c 2d61 636f 6d70 3a7b 646f 635b 695d  cl-acomp:{doc[i]
-00012160: 2e6c 656d 6d61 5f7d 207b 646f 635b 6b5d  .lemma_} {doc[k]
-00012170: 2e74 6578 747d 5b7b 697d 2c7b 6a7d 2c7b  .text}[{i},{j},{
-00012180: 6b7d 5d22 3a7b 2274 6167 223a 7461 672c  k}]":{"tag":tag,
-00012190: 2022 6672 6f6d 223a 2274 7270 3322 2c0a   "from":"trp3",.
-000121a0: 0909 0909 0909 226e 6163 223a 5b66 227b  ......"nac":[f"{
-000121b0: 646f 635b 695d 2e6c 656d 6d61 5f7d 3a7b  doc[i].lemma_}:{
-000121c0: 646f 635b 695d 2e70 6f73 5f7d 3a61 6476  doc[i].pos_}:adv
-000121d0: 636c 2d61 636f 6d70 7c7b 646f 635b 6b5d  cl-acomp|{doc[k]
-000121e0: 2e74 6578 742e 6c6f 7765 7228 297d 222c  .text.lower()}",
-000121f0: 6622 7b64 6f63 5b6b 5d2e 7465 7874 2e6c  f"{doc[k].text.l
-00012200: 6f77 6572 2829 7d3a 7b64 6f63 5b6b 5d2e  ower()}:{doc[k].
-00012210: 7461 675f 2069 6620 646f 635b 6b5d 2e74  tag_ if doc[k].t
-00012220: 6167 5f20 3d3d 2027 5642 4e27 2065 6c73  ag_ == 'VBN' els
-00012230: 6520 646f 635b 6b5d 2e70 6f73 5f7d 3a7e  e doc[k].pos_}:~
-00012240: 6164 7663 6c2d 6163 6f6d 707c 7b64 6f63  advcl-acomp|{doc
-00012250: 5b69 5d2e 6c65 6d6d 615f 7d22 2c66 227b  [i].lemma_}",f"{
-00012260: 646f 635b 695d 2e6c 656d 6d61 5f7d 3a7b  doc[i].lemma_}:{
-00012270: 646f 635b 695d 2e70 6f73 5f7d 7c61 6476  doc[i].pos_}|adv
-00012280: 636c 2d61 636f 6d70 222c 6622 7b64 6f63  cl-acomp",f"{doc
-00012290: 5b6b 5d2e 7465 7874 2e6c 6f77 6572 2829  [k].text.lower()
-000122a0: 7d3a 7b64 6f63 5b6b 5d2e 7461 675f 2069  }:{doc[k].tag_ i
-000122b0: 6620 646f 635b 6b5d 2e74 6167 5f20 3d3d  f doc[k].tag_ ==
-000122c0: 2027 5642 4e27 2065 6c73 6520 646f 635b   'VBN' else doc[
-000122d0: 6b5d 2e70 6f73 5f7d 7c7e 6164 7663 6c2d  k].pos_}|~advcl-
-000122e0: 6163 6f6d 7022 5d7d 7d29 2c20 0a09 2264  acomp"]}}), .."d
-000122f0: 6f62 6a2d 7072 7422 3a09 096c 616d 6264  obj-prt":..lambd
-00012300: 6120 646f 632c 2069 2c20 6a2c 206b 2c20  a doc, i, j, k, 
-00012310: 7461 673a 2020 646f 632e 7573 6572 5f64  tag:  doc.user_d
-00012320: 6174 612e 7570 6461 7465 287b 6622 646f  ata.update({f"do
-00012330: 626a 2d70 7274 3a7b 646f 635b 695d 2e6c  bj-prt:{doc[i].l
-00012340: 656d 6d61 5f7d 5f7b 646f 635b 6a5d 2e6c  emma_}_{doc[j].l
-00012350: 656d 6d61 5f7d 207b 646f 635b 6b5d 2e6c  emma_} {doc[k].l
-00012360: 656d 6d61 5f7d 5b7b 697d 2c7b 6a7d 2c7b  emma_}[{i},{j},{
-00012370: 6b7d 5d22 3a7b 2274 6167 223a 7461 672c  k}]":{"tag":tag,
-00012380: 2022 6672 6f6d 223a 2274 7270 3322 2c0a   "from":"trp3",.
-00012390: 0909 0909 0909 226e 6163 223a 5b66 227b  ......"nac":[f"{
-000123a0: 646f 635b 695d 2e6c 656d 6d61 5f7d 5f7b  doc[i].lemma_}_{
-000123b0: 646f 635b 6a5d 2e6c 656d 6d61 5f7d 3a7b  doc[j].lemma_}:{
-000123c0: 646f 635b 695d 2e70 6f73 5f7d 3a64 6f62  doc[i].pos_}:dob
-000123d0: 6a3a 7b64 6f63 5b6b 5d2e 706f 735f 7d7c  j:{doc[k].pos_}|
-000123e0: 7b64 6f63 5b6b 5d2e 6c65 6d6d 615f 7d22  {doc[k].lemma_}"
-000123f0: 2c66 227b 646f 635b 6b5d 2e6c 656d 6d61  ,f"{doc[k].lemma
-00012400: 5f7d 3a7b 646f 635b 6b5d 2e70 6f73 5f7d  _}:{doc[k].pos_}
-00012410: 3a7e 646f 626a 3a7b 646f 635b 695d 2e70  :~dobj:{doc[i].p
-00012420: 6f73 5f7d 7c7b 646f 635b 695d 2e6c 656d  os_}|{doc[i].lem
-00012430: 6d61 5f7d 5f7b 646f 635b 6a5d 2e6c 656d  ma_}_{doc[j].lem
-00012440: 6d61 5f7d 222c 6622 7b64 6f63 5b69 5d2e  ma_}",f"{doc[i].
-00012450: 6c65 6d6d 615f 7d5f 7b64 6f63 5b6a 5d2e  lemma_}_{doc[j].
-00012460: 6c65 6d6d 615f 7d3a 7b64 6f63 5b69 5d2e  lemma_}:{doc[i].
-00012470: 706f 735f 7d7c 646f 626a 3a7b 646f 635b  pos_}|dobj:{doc[
-00012480: 6b5d 2e70 6f73 5f7d 222c 6622 7b64 6f63  k].pos_}",f"{doc
-00012490: 5b6b 5d2e 6c65 6d6d 615f 7d3a 7b64 6f63  [k].lemma_}:{doc
-000124a0: 5b6b 5d2e 706f 735f 7d7c 7e64 6f62 6a3a  [k].pos_}|~dobj:
-000124b0: 7b64 6f63 5b69 5d2e 706f 735f 7d22 5d7d  {doc[i].pos_}"]}
-000124c0: 7d29 2c20 0a09 2276 704e 223a 0909 096c  }), .."vpN":...l
-000124d0: 616d 6264 6120 646f 632c 2069 2c20 6a2c  ambda doc, i, j,
-000124e0: 206b 2c20 7461 673a 2020 646f 632e 7573   k, tag:  doc.us
-000124f0: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
-00012500: 6622 7670 4e3a 7b64 6f63 5b69 5d2e 6c65  f"vpN:{doc[i].le
-00012510: 6d6d 615f 7d20 7b64 6f63 5b6a 5d2e 7465  mma_} {doc[j].te
-00012520: 7874 7d20 7b64 6f63 5b6b 5d2e 7465 7874  xt} {doc[k].text
-00012530: 7d5b 7b69 7d2c 7b6a 7d2c 7b6b 7d5d 223a  }[{i},{j},{k}]":
-00012540: 7b22 7461 6722 3a74 6167 2c20 2266 726f  {"tag":tag, "fro
-00012550: 6d22 3a22 7472 7033 222c 2023 206a 756d  m":"trp3", # jum
-00012560: 7020 6f76 6572 2074 6865 2064 6f67 202f  p over the dog /
-00012570: 2063 6f6d 6520 696e 746f 2066 6f72 6365   come into force
-00012580: 2f76 706e 200a 0909 0909 0909 226e 6163  /vpn ......."nac
-00012590: 223a 5b66 227b 646f 635b 695d 2e6c 656d  ":[f"{doc[i].lem
-000125a0: 6d61 5f7d 3a7b 646f 635b 695d 2e70 6f73  ma_}:{doc[i].pos
-000125b0: 5f7d 3a76 704e 7c7b 646f 635b 6b5d 2e6c  _}:vpN|{doc[k].l
-000125c0: 656d 6d61 5f7d 222c 6622 7b64 6f63 5b69  emma_}",f"{doc[i
-000125d0: 5d2e 6c65 6d6d 615f 7d3a 7b64 6f63 5b69  ].lemma_}:{doc[i
-000125e0: 5d2e 706f 735f 7d7c 7670 4e22 2c66 227b  ].pos_}|vpN",f"{
-000125f0: 646f 635b 6b5d 2e6c 656d 6d61 5f7d 3a7b  doc[k].lemma_}:{
-00012600: 646f 635b 6b5d 2e70 6f73 5f7d 3a76 704e  doc[k].pos_}:vpN
-00012610: 7c7b 646f 635b 695d 2e6c 656d 6d61 5f7d  |{doc[i].lemma_}
-00012620: 207b 646f 635b 6a5d 2e6c 656d 6d61 5f7d   {doc[j].lemma_}
-00012630: 207b 646f 635b 6b5d 2e6c 656d 6d61 5f7d   {doc[k].lemma_}
-00012640: 222c 6622 7b64 6f63 5b6b 5d2e 6c65 6d6d  ",f"{doc[k].lemm
-00012650: 615f 7d3a 7b64 6f63 5b6b 5d2e 706f 735f  a_}:{doc[k].pos_
-00012660: 7d7c 7670 4e22 5d7d 7d29 2c20 0a09 7d0a  }|vpN"]}}), ..}.
-00012670: 0a64 6566 206b 705f 626f 726e 2864 6f63  .def kp_born(doc
-00012680: 2c20 6261 7365 3a62 6f6f 6c3d 5472 7565  , base:bool=True
-00012690: 293a 0a09 2727 2720 626f 726e 206b 7020  ):..''' born kp 
-000126a0: 746f 2075 7365 725f 6461 7461 202c 2020  to user_data ,  
-000126b0: 4e4e 533a 6b6e 6f77 6c65 6467 6573 2c20  NNS:knowledges, 
-000126c0: 206e 6265 3a66 6174 6520 7365 616c 6564   nbe:fate sealed
-000126d0: 2c20 2027 2727 0a09 6672 6f6d 2064 6963  ,  '''..from dic
-000126e0: 2e77 6f72 646c 6973 7420 696d 706f 7274  .wordlist import
-000126f0: 2077 6f72 646c 6973 7420 0a09 6966 2062   wordlist ..if b
-00012700: 6173 653a 0a09 095b 2064 6f63 2e75 7365  ase:...[ doc.use
-00012710: 725f 6461 7461 2e75 7064 6174 6528 7b66  r_data.update({f
-00012720: 227b 742e 706f 735f 7d3a 7b74 2e6c 656d  "{t.pos_}:{t.lem
-00012730: 6d61 5f7d 5b7b 742e 697d 5d22 3a20 7b22  ma_}[{t.i}]": {"
-00012740: 7479 7065 223a 2274 6f6b 222c 200a 0909  type":"tok", ...
-00012750: 0909 226e 6163 223a 5b66 227b 742e 706f  .."nac":[f"{t.po
-00012760: 735f 7d7c 7b74 2e6c 656d 6d61 5f7d 222c  s_}|{t.lemma_}",
-00012770: 2066 227b 742e 6c65 6d6d 615f 7d7c 7b74   f"{t.lemma_}|{t
-00012780: 2e70 6f73 5f7d 222c 2066 222a 7c7b 742e  .pos_}", f"*|{t.
-00012790: 706f 735f 7d22 2c20 6622 7b74 2e6c 656d  pos_}", f"{t.lem
-000127a0: 6d61 5f7d 3a7b 742e 706f 735f 7d7c 7b74  ma_}:{t.pos_}|{t
-000127b0: 2e74 6167 5f7d 222c 6622 2a3a 7b74 2e70  .tag_}",f"*:{t.p
-000127c0: 6f73 5f7d 7c7b 742e 7461 675f 7d22 2c20  os_}|{t.tag_}", 
-000127d0: 6622 7b74 2e6c 656d 6d61 5f7d 3a7b 742e  f"{t.lemma_}:{t.
-000127e0: 706f 735f 7d3a 7b74 2e74 6167 5f7d 7c7b  pos_}:{t.tag_}|{
-000127f0: 742e 7465 7874 2e6c 6f77 6572 2829 7d22  t.text.lower()}"
-00012800: 5d7d 2c20 0a09 0909 6622 7b74 2e74 6167  ]}, ....f"{t.tag
-00012810: 5f7d 3a7b 742e 7465 7874 2e6c 6f77 6572  _}:{t.text.lower
-00012820: 2829 7d5b 7b74 2e69 7d5d 223a 207b 2274  ()}[{t.i}]": {"t
-00012830: 7970 6522 3a22 746f 6b22 2c20 0a09 0909  ype":"tok", ....
-00012840: 0922 6e61 6322 3a5b 6622 7b74 2e74 6167  ."nac":[f"{t.tag
-00012850: 5f7d 7c7b 742e 7465 7874 2e6c 6f77 6572  _}|{t.text.lower
-00012860: 2829 7d22 2c20 6622 2a7c 7b74 2e74 6167  ()}", f"*|{t.tag
-00012870: 5f7d 225d 7d20 7d29 2066 6f72 2074 2069  _}"]} }) for t i
-00012880: 6e20 646f 6320 6966 2074 2e70 6f73 5f20  n doc if t.pos_ 
-00012890: 696e 2028 224e 4f55 4e22 2c22 5645 5242  in ("NOUN","VERB
-000128a0: 222c 2241 444a 222c 2241 4456 2229 2061  ","ADJ","ADV") a
-000128b0: 6e64 2074 2e69 735f 616c 7068 6120 5d0a  nd t.is_alpha ].
-000128c0: 0a09 095b 2064 6f63 2e75 7365 725f 6461  ...[ doc.user_da
-000128d0: 7461 2e75 7064 6174 6528 7b66 226e 6265  ta.update({f"nbe
-000128e0: 3a7b 742e 6c65 6d6d 615f 7d20 7b74 2e68  :{t.lemma_} {t.h
-000128f0: 6561 642e 7465 7874 2e6c 6f77 6572 2829  ead.text.lower()
-00012900: 7d5b 7b74 2e68 6561 642e 697d 2c7b 742e  }[{t.head.i},{t.
-00012910: 697d 5d22 3a20 7b22 7479 7065 223a 2274  i}]": {"type":"t
-00012920: 7270 222c 0a09 0909 276e 6163 273a 5b66  rp",....'nac':[f
-00012930: 227b 742e 6c65 6d6d 615f 7d3a 7b74 2e70  "{t.lemma_}:{t.p
-00012940: 6f73 5f7d 3a6e 6265 7c7b 742e 6865 6164  os_}:nbe|{t.head
-00012950: 2e74 6578 742e 6c6f 7765 7228 297d 222c  .text.lower()}",
-00012960: 2066 227b 742e 6c65 6d6d 615f 7d3a 7b74   f"{t.lemma_}:{t
-00012970: 2e70 6f73 5f7d 7c6e 6265 222c 2066 222a  .pos_}|nbe", f"*
-00012980: 3a7b 742e 706f 735f 7d7c 6e62 6522 2c20  :{t.pos_}|nbe", 
-00012990: 2023 2053 6d6f 6b69 6e67 2069 7320 6261   # Smoking is ba
-000129a0: 6e6e 6564 2e20 2f56 4247 0a09 0909 0966  nned. /VBG.....f
-000129b0: 227b 742e 6865 6164 2e74 6578 742e 6c6f  "{t.head.text.lo
-000129c0: 7765 7228 297d 3a7b 742e 7461 675f 7d3a  wer()}:{t.tag_}:
-000129d0: 6e62 657c 7b74 2e6c 656d 6d61 5f7d 222c  nbe|{t.lemma_}",
-000129e0: 2066 227b 742e 6865 6164 2e74 6578 742e   f"{t.head.text.
-000129f0: 6c6f 7765 7228 297d 3a7b 742e 7461 675f  lower()}:{t.tag_
-00012a00: 7d7c 6e62 6522 2c20 6622 2a3a 7b74 2e74  }|nbe", f"*:{t.t
-00012a10: 6167 5f7d 7c6e 6265 222c 5d20 7d20 7d29  ag_}|nbe",] } })
-00012a20: 2066 6f72 2074 2069 6e20 646f 6320 6966   for t in doc if
-00012a30: 2074 2e64 6570 5f20 3d3d 2027 6e73 7562   t.dep_ == 'nsub
-00012a40: 6a70 6173 7327 2061 6e64 2074 2e68 6561  jpass' and t.hea
-00012a50: 642e 7461 675f 203d 3d20 2756 424e 2720  d.tag_ == 'VBN' 
-00012a60: 5d20 2320 7468 6520 6661 7465 2069 7320  ] # the fate is 
-00012a70: 7365 616c 6564 2020 2f20 736d 696c 696e  sealed  / smilin
-00012a80: 6720 6973 2062 616e 6e65 6420 2e0a 0909  g is banned ....
-00012a90: 5b20 646f 632e 7573 6572 5f64 6174 612e  [ doc.user_data.
-00012aa0: 7570 6461 7465 287b 6622 7663 3a7b 742e  update({f"vc:{t.
-00012ab0: 6865 6164 2e6c 656d 6d61 5f7d 5b7b 742e  head.lemma_}[{t.
-00012ac0: 6865 6164 2e69 7d2c 7b74 2e69 7d5d 223a  head.i},{t.i}]":
-00012ad0: 207b 2274 7970 6522 3a22 7472 7022 2c20   {"type":"trp", 
-00012ae0: 276e 6163 273a 5b66 227b 742e 6865 6164  'nac':[f"{t.head
-00012af0: 2e6c 656d 6d61 5f7d 3a7b 742e 6865 6164  .lemma_}:{t.head
-00012b00: 2e70 6f73 5f7d 7c76 6322 2c20 6622 2a3a  .pos_}|vc", f"*:
-00012b10: 7b74 2e68 6561 642e 706f 735f 7d7c 7663  {t.head.pos_}|vc
-00012b20: 222c 2066 227b 742e 6865 6164 2e6c 656d  ", f"{t.head.lem
-00012b30: 6d61 5f7d 2f7b 742e 6865 6164 2e70 6f73  ma_}/{t.head.pos
-00012b40: 5f7d 7c76 633a 5f7b 742e 6865 6164 2e6c  _}|vc:_{t.head.l
-00012b50: 656d 6d61 5f7d 205f 434c 6363 6f6d 7022  emma_} _CLccomp"
-00012b60: 2c5d 207d 207d 2920 666f 7220 7420 696e  ,] } }) for t in
-00012b70: 2064 6f63 2069 6620 742e 6465 705f 203d   doc if t.dep_ =
-00012b80: 3d20 2763 636f 6d70 2720 616e 6420 742e  = 'ccomp' and t.
-00012b90: 6865 6164 2e70 6f73 5f20 3d3d 2027 5645  head.pos_ == 'VE
-00012ba0: 5242 2720 5d0a 0909 5b20 646f 632e 7573  RB' ]...[ doc.us
-00012bb0: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
-00012bc0: 6622 524f 4f54 2d7b 742e 7461 675f 7d3a  f"ROOT-{t.tag_}:
-00012bd0: 7b74 2e6c 656d 6d61 5f7d 5b7b 742e 697d  {t.lemma_}[{t.i}
-00012be0: 5d22 3a20 7b22 7479 7065 223a 2274 7270  ]": {"type":"trp
-00012bf0: 222c 226e 6163 223a 5b66 227b 742e 6c65  ","nac":[f"{t.le
-00012c00: 6d6d 615f 7d3a 7b74 2e70 6f73 5f7d 7c52  mma_}:{t.pos_}|R
-00012c10: 4f4f 5422 5d7d 207d 2920 666f 7220 7420  OOT"]} }) for t 
-00012c20: 696e 2064 6f63 2069 6620 742e 6465 705f  in doc if t.dep_
-00012c30: 203d 3d20 2752 4f4f 5427 205d 0a09 095b   == 'ROOT' ]...[
-00012c40: 2064 6f63 2e75 7365 725f 6461 7461 2e75   doc.user_data.u
-00012c50: 7064 6174 6528 7b66 2278 636f 6d70 2d7b  pdate({f"xcomp-{
-00012c60: 742e 6865 6164 2e70 6f73 5f7d 2d7b 742e  t.head.pos_}-{t.
-00012c70: 7461 675f 7d3a 7b74 2e68 6561 642e 6c65  tag_}:{t.head.le
-00012c80: 6d6d 615f 7d20 7b74 2e74 6578 747d 5b7b  mma_} {t.text}[{
-00012c90: 742e 6865 6164 2e69 7d2c 7b74 2e69 7d5d  t.head.i},{t.i}]
-00012ca0: 223a 207b 2274 7970 6522 3a22 7472 7022  ": {"type":"trp"
-00012cb0: 2c20 0a09 0909 226e 6163 223a 5b66 227b  , ...."nac":[f"{
-00012cc0: 742e 6865 6164 2e6c 656d 6d61 5f7d 3a7b  t.head.lemma_}:{
-00012cd0: 742e 6865 6164 2e70 6f73 5f7d 7c78 636f  t.head.pos_}|xco
-00012ce0: 6d70 3a7b 742e 7461 675f 7d22 2c20 6622  mp:{t.tag_}", f"
-00012cf0: 7b74 2e68 6561 642e 6c65 6d6d 615f 7d3a  {t.head.lemma_}:
-00012d00: 7b74 2e68 6561 642e 706f 735f 7d3a 7863  {t.head.pos_}:xc
-00012d10: 6f6d 703a 7b74 2e74 6167 5f7d 7c7b 742e  omp:{t.tag_}|{t.
-00012d20: 7465 7874 2e6c 6f77 6572 2829 7d22 2c0a  text.lower()}",.
-00012d30: 0909 0909 2020 2066 227b 742e 6c65 6d6d  ....   f"{t.lemm
-00012d40: 615f 7d3a 7b74 2e74 6167 5f7d 7c7e 7863  a_}:{t.tag_}|~xc
-00012d50: 6f6d 703a 7b74 2e68 6561 642e 706f 735f  omp:{t.head.pos_
-00012d60: 7d22 2c20 6622 7b74 2e6c 656d 6d61 5f7d  }", f"{t.lemma_}
-00012d70: 3a7b 742e 7461 675f 7d3a 7e78 636f 6d70  :{t.tag_}:~xcomp
-00012d80: 3a7b 742e 6865 6164 2e70 6f73 5f7d 7c7b  :{t.head.pos_}|{
-00012d90: 742e 6865 6164 2e6c 656d 6d61 5f7d 222c  t.head.lemma_}",
-00012da0: 200a 0909 0920 2020 2020 2020 6622 7b74   ....       f"{t
-00012db0: 2e6c 656d 6d61 5f7d 3a7b 742e 706f 735f  .lemma_}:{t.pos_
-00012dc0: 7d7c 7e78 636f 6d70 3a7b 742e 6865 6164  }|~xcomp:{t.head
-00012dd0: 2e70 6f73 5f7d 222c 2066 227b 742e 6c65  .pos_}", f"{t.le
-00012de0: 6d6d 615f 7d3a 7b74 2e70 6f73 5f7d 3a7e  mma_}:{t.pos_}:~
-00012df0: 7863 6f6d 703a 7b74 2e68 6561 642e 706f  xcomp:{t.head.po
-00012e00: 735f 7d7c 7b74 2e68 6561 642e 6c65 6d6d  s_}|{t.head.lemm
-00012e10: 615f 7d22 2c20 2320 6164 6465 6420 3230  a_}", # added 20
-00012e20: 332e 322e 3236 0a09 0909 0920 2020 6622  3.2.26.....   f"
-00012e30: 2a3a 7b74 2e68 6561 642e 706f 735f 7d7c  *:{t.head.pos_}|
-00012e40: 7863 6f6d 703a 7b74 2e74 6167 5f7d 222c  xcomp:{t.tag_}",
-00012e50: 2066 222a 3a7b 742e 706f 735f 7d7c 7e78   f"*:{t.pos_}|~x
-00012e60: 636f 6d70 3a7b 742e 6865 6164 2e70 6f73  comp:{t.head.pos
-00012e70: 5f7d 222c 5d20 7d20 7d29 200a 0909 0966  _}",] } }) ....f
-00012e80: 6f72 2074 2069 6e20 646f 6320 6966 2074  or t in doc if t
-00012e90: 2e64 6570 5f20 3d3d 2027 7863 6f6d 7027  .dep_ == 'xcomp'
-00012ea0: 2061 6e64 2074 2e70 6f73 5f20 3d3d 2027   and t.pos_ == '
-00012eb0: 5645 5242 2720 5d0a 0909 5b20 646f 632e  VERB' ]...[ doc.
-00012ec0: 7573 6572 5f64 6174 612e 7570 6461 7465  user_data.update
-00012ed0: 287b 6622 4e50 3a7b 7370 2e74 6578 742e  ({f"NP:{sp.text.
-00012ee0: 6c6f 7765 7228 297d 5b7b 7370 2e73 7461  lower()}[{sp.sta
-00012ef0: 7274 7d2c 7b73 702e 656e 647d 2922 3a20  rt},{sp.end})": 
-00012f00: 7b22 7479 7065 223a 2263 6875 6e6b 222c  {"type":"chunk",
-00012f10: 200a 0909 0922 6e61 6322 3a5b 6622 7b64   ...."nac":[f"{d
-00012f20: 6f63 5b73 702e 656e 642d 315d 2e6c 656d  oc[sp.end-1].lem
-00012f30: 6d61 5f7d 3a7b 646f 635b 7370 2e65 6e64  ma_}:{doc[sp.end
-00012f40: 2d31 5d2e 706f 735f 7d3a 4e50 7c7b 7370  -1].pos_}:NP|{sp
-00012f50: 2e74 6578 742e 6c6f 7765 7228 297d 222c  .text.lower()}",
-00012f60: 2066 227b 646f 635b 7370 2e65 6e64 2d31   f"{doc[sp.end-1
-00012f70: 5d2e 6c65 6d6d 615f 7d3a 7b64 6f63 5b73  ].lemma_}:{doc[s
-00012f80: 702e 656e 642d 315d 2e70 6f73 5f7d 7c4e  p.end-1].pos_}|N
-00012f90: 5022 0a09 0909 2c20 6622 2a3a 7b64 6f63  P"...., f"*:{doc
-00012fa0: 5b73 702e 656e 642d 315d 2e70 6f73 5f7d  [sp.end-1].pos_}
-00012fb0: 7c4e 5022 5d20 7d7d 2020 2920 0a09 0909  |NP"] }}  ) ....
-00012fc0: 666f 7220 7370 2069 6e20 646f 632e 6e6f  for sp in doc.no
-00012fd0: 756e 5f63 6875 6e6b 735d 2023 4e50 3a61  un_chunks] #NP:a
-00012fe0: 2062 6f6f 6b0a 0a09 0923 2061 6464 2074   book....# add t
-00012ff0: 7269 706c 6520 6b70 3a20 646f 626a 2d56  riple kp: dobj-V
-00013000: 4552 422d 4e4f 554e 3a6f 7065 6e20 646f  ERB-NOUN:open do
-00013010: 6f72 0a09 095b 2064 6f63 2e75 7365 725f  or...[ doc.user_
-00013020: 6461 7461 2e75 7064 6174 6528 7b66 227b  data.update({f"{
-00013030: 742e 6465 705f 7d2d 7b74 2e68 6561 642e  t.dep_}-{t.head.
-00013040: 706f 735f 7d2d 7b74 2e70 6f73 5f7d 3a7b  pos_}-{t.pos_}:{
-00013050: 742e 6865 6164 2e6c 656d 6d61 5f7d 207b  t.head.lemma_} {
-00013060: 742e 6c65 6d6d 615f 7d5b 7b74 2e68 6561  t.lemma_}[{t.hea
-00013070: 642e 697d 2c7b 742e 697d 5d22 3a20 7b22  d.i},{t.i}]": {"
-00013080: 7479 7065 223a 2274 7270 222c 0a09 0909  type":"trp",....
-00013090: 226e 6163 223a 5b66 227b 742e 6865 6164  "nac":[f"{t.head
-000130a0: 2e6c 656d 6d61 5f7d 3a7b 742e 6865 6164  .lemma_}:{t.head
-000130b0: 2e70 6f73 5f7d 3a7b 742e 6465 705f 7d7c  .pos_}:{t.dep_}|
-000130c0: 7b74 2e70 6f73 5f7d 222c 6622 7b74 2e68  {t.pos_}",f"{t.h
-000130d0: 6561 642e 6c65 6d6d 615f 7d3a 7b74 2e68  ead.lemma_}:{t.h
-000130e0: 6561 642e 706f 735f 7d7c 7b74 2e64 6570  ead.pos_}|{t.dep
-000130f0: 5f7d 3a7b 742e 706f 735f 7d22 2c20 6622  _}:{t.pos_}", f"
-00013100: 7b74 2e68 6561 642e 6c65 6d6d 615f 7d3a  {t.head.lemma_}:
-00013110: 7b74 2e68 6561 642e 706f 735f 7d3a 7b74  {t.head.pos_}:{t
-00013120: 2e64 6570 5f7d 3a7b 742e 706f 735f 7d7c  .dep_}:{t.pos_}|
-00013130: 7b74 2e6c 656d 6d61 5f7d 222c 0a09 0909  {t.lemma_}",....
-00013140: 0920 2020 6622 7b74 2e6c 656d 6d61 5f7d  .   f"{t.lemma_}
-00013150: 3a7b 742e 706f 735f 7d3a 7e7b 742e 6465  :{t.pos_}:~{t.de
-00013160: 705f 7d7c 7b74 2e68 6561 642e 706f 735f  p_}|{t.head.pos_
-00013170: 7d22 2c20 6622 7b74 2e6c 656d 6d61 5f7d  }", f"{t.lemma_}
-00013180: 3a7b 742e 706f 735f 7d7c 7e7b 742e 6465  :{t.pos_}|~{t.de
-00013190: 705f 7d3a 7b74 2e68 6561 642e 706f 735f  p_}:{t.head.pos_
-000131a0: 7d22 2c20 6622 7b74 2e6c 656d 6d61 5f7d  }", f"{t.lemma_}
-000131b0: 3a7b 742e 706f 735f 7d3a 7e7b 742e 6465  :{t.pos_}:~{t.de
-000131c0: 705f 7d3a 7b74 2e68 6561 642e 706f 735f  p_}:{t.head.pos_
-000131d0: 7d7c 7b74 2e68 6561 642e 6c65 6d6d 615f  }|{t.head.lemma_
-000131e0: 7d22 2c0a 0909 0909 2020 2066 222a 3a7b  }",.....   f"*:{
-000131f0: 742e 6865 6164 2e70 6f73 5f7d 7c7b 742e  t.head.pos_}|{t.
-00013200: 6465 705f 7d22 2c66 222a 3a7b 742e 706f  dep_}",f"*:{t.po
-00013210: 735f 7d7c 7e7b 742e 6465 705f 7d22 2c0a  s_}|~{t.dep_}",.
-00013220: 0909 095d 207d 207d 2920 0a09 0909 666f  ...] } }) ....fo
-00013230: 7220 7420 696e 2064 6f63 2069 6620 742e  r t in doc if t.
-00013240: 706f 735f 2069 6e20 2822 4e4f 554e 222c  pos_ in ("NOUN",
-00013250: 2256 4552 4222 2c22 4144 4a22 2c22 4144  "VERB","ADJ","AD
-00013260: 5622 2c22 4144 5022 2920 616e 6420 742e  V","ADP") and t.
-00013270: 6465 705f 206e 6f74 2069 6e20 2827 524f  dep_ not in ('RO
-00013280: 4f54 272c 2770 756e 6374 272c 2778 636f  OT','punct','xco
-00013290: 6d70 2729 2061 6e64 2074 2e69 735f 616c  mp') and t.is_al
-000132a0: 7068 6120 616e 6420 742e 6865 6164 2e69  pha and t.head.i
-000132b0: 735f 616c 7068 6120 616e 6420 742e 6c65  s_alpha and t.le
-000132c0: 6d6d 615f 2069 6e20 776f 7264 6c69 7374  mma_ in wordlist
-000132d0: 2020 616e 6420 742e 6865 6164 2e6c 656d    and t.head.lem
-000132e0: 6d61 5f20 696e 2077 6f72 646c 6973 745d  ma_ in wordlist]
-000132f0: 0a0a 0970 6f73 7461 675f 6d61 7463 6828  ...postag_match(
-00013300: 646f 632c 2070 6f73 7461 675f 6675 6e63  doc, postag_func
-00013310: 5f6b 7029 200a 0974 7270 335f 6d61 7463  _kp) ..trp3_matc
-00013320: 6828 646f 632c 2074 7270 335f 6675 6e63  h(doc, trp3_func
-00013330: 5f6b 7029 0a09 6d65 7267 655f 6e70 2864  _kp)..merge_np(d
-00013340: 6f63 2920 200a 0973 6b65 6e70 5f6d 6174  oc)  ..skenp_mat
-00013350: 6368 2864 6f63 2c20 736b 656e 705f 6675  ch(doc, skenp_fu
-00013360: 6e63 5f6b 7029 2020 236f 6e5f 7370 616e  nc_kp)  #on_span
-00013370: 2864 6f63 2c20 736b 656e 705f 6675 6e63  (doc, skenp_func
-00013380: 2c20 2773 6b65 6e70 5b27 290a 0972 6574  , 'skenp[')..ret
-00013390: 7572 6e20 646f 632e 7573 6572 5f64 6174  urn doc.user_dat
-000133a0: 610a 0a5b 7365 7461 7474 7228 6275 696c  a..[setattr(buil
-000133b0: 7469 6e73 2c20 6b2c 2076 2920 666f 7220  tins, k, v) for 
-000133c0: 6b2c 2076 2069 6e20 676c 6f62 616c 7328  k, v in globals(
-000133d0: 292e 6974 656d 7328 2920 6966 206e 6f74  ).items() if not
-000133e0: 206b 2e73 7461 7274 7377 6974 6828 225f   k.startswith("_
-000133f0: 2229 2061 6e64 206e 6f74 2027 2e27 2069  ") and not '.' i
-00013400: 6e20 6b20 616e 6420 6e6f 7420 6861 7361  n k and not hasa
-00013410: 7474 7228 6275 696c 7469 6e73 2c6b 2920  ttr(builtins,k) 
-00013420: 5d20 2373 6574 6174 7472 2862 7569 6c74  ] #setattr(built
-00013430: 696e 732c 2022 7370 6163 7922 2c20 7370  ins, "spacy", sp
-00013440: 6163 7929 0a69 6620 5f5f 6e61 6d65 5f5f  acy).if __name__
-00013450: 093d 3d20 275f 5f6d 6169 6e5f 5f27 3a20  .== '__main__': 
-00013460: 0a09 696d 706f 7274 2066 6972 652c 2070  ..import fire, p
-00013470: 6c61 7466 6f72 6d0a 095b 2070 7269 6e74  latform..[ print
-00013480: 2028 206b 702c 2069 7465 6d29 2066 6f72   ( kp, item) for
-00013490: 206b 702c 2069 7465 6d20 696e 206b 705f   kp, item in kp_
-000134a0: 626f 726e 2873 7061 6379 2e6e 6c70 2822  born(spacy.nlp("
-000134b0: 4920 7461 6b65 2069 7420 696e 746f 2061  I take it into a
-000134c0: 6363 6f75 6e74 2c20 616e 6420 4920 656e  ccount, and I en
-000134d0: 6a6f 7920 7377 696d 6d69 6e67 2e22 2929  joy swimming."))
-000134e0: 2e69 7465 6d73 2829 5d20 2069 6620 706c  .items()]  if pl
-000134f0: 6174 666f 726d 2e73 7973 7465 6d28 2920  atform.system() 
-00013500: 696e 2028 2757 696e 646f 7773 2729 2065  in ('Windows') e
-00013510: 6c73 6520 6669 7265 2e46 6972 6528 7b22  lse fire.Fire({"
-00013520: 7371 6c73 6922 3a73 716c 7369 2c20 2274  sqlsi":sqlsi, "t
-00013530: 6573 7422 3a74 6573 742c 2022 6573 5f73  est":test, "es_s
-00013540: 7562 6d69 7422 3a65 735f 7375 626d 6974  ubmit":es_submit
-00013550: 2c20 2266 6173 7474 6578 7422 3a66 6173  , "fasttext":fas
-00013560: 7474 6578 7420 7d29 0a0a 2370 7269 6e74  ttext })..#print
-00013570: 2873 6e74 6272 2822 5b5c 7538 6264 315c  (sntbr("[\u8bd1\
-00013580: 7536 3538 375d 5468 6520 3535 2d6b 696c  u6587]The 55-kil
-00013590: 6f6d 6574 7265 2048 6f6e 6720 4b6f 6e67  ometre Hong Kong
-000135a0: 205a 6875 6861 692d 4d61 6361 7520 4272   Zhuhai-Macau Br
-000135b0: 6964 6765 2069 7320 616e 2065 7874 7261  idge is an extra
-000135c0: 6f72 6469 6e61 7279 2065 6e67 696e 6565  ordinary enginee
-000135d0: 7269 6e67 2e20 4974 2069 7320 7468 6520  ring. It is the 
-000135e0: 776f 726c 6427 7320 6c6f 6e67 6573 7420  world's longest 
-000135f0: 7365 612d 6372 6f73 7369 6e67 2074 7261  sea-crossing tra
-00013600: 6e73 706f 7274 6174 696f 6e20 7379 7374  nsportation syst
-00013610: 656d 2063 6f6d 6269 6e69 6e67 2062 7269  em combining bri
-00013620: 6467 6573 2061 6e64 2074 756e 6e65 6c73  dges and tunnels
-00013630: 2c20 7768 6963 6820 6a6f 696e 7320 7468  , which joins th
-00013640: 6520 7468 7265 6520 6369 7469 6573 206f  e three cities o
-00013650: 6620 486f 6e67 204b 6f6e 6720 5a68 7568  f Hong Kong Zhuh
-00013660: 6169 2061 6e64 204d 6163 616f 2c20 6375  ai and Macao, cu
-00013670: 7474 696e 6720 7468 6520 7472 6176 656c  tting the travel
-00013680: 6c69 6e67 2074 696d 6520 616d 6f6e 6720  ling time among 
-00013690: 7468 656d 2066 726f 6d20 3320 686f 7572  them from 3 hour
-000136a0: 7320 746f 2033 3020 6d69 6e75 7465 732e  s to 30 minutes.
-000136b0: 2054 6865 2072 6569 6e66 6f72 6365 6420   The reinforced 
-000136c0: 636f 6e63 7265 7465 2062 7269 6467 6520  concrete bridge 
-000136d0: 7769 7468 2068 7567 6520 7370 616e 7320  with huge spans 
-000136e0: 6675 6c6c 7920 6e6f 7420 6f6e 6c79 2070  fully not only p
-000136f0: 726f 7665 7320 7468 6174 2043 6869 6e61  roves that China
-00013700: 2068 6173 2074 6865 2061 6269 6c69 7479   has the ability
-00013710: 2074 6f20 636f 6d70 6c65 7465 2074 6865   to complete the
-00013720: 2072 6563 6f72 642d 6272 6561 6b69 6e67   record-breaking
-00013730: 206d 6567 612d 636f 6e73 7472 7563 7469   mega-constructi
-00013740: 6f6e 2c20 6275 7420 616c 736f 2077 696c  on, but also wil
-00013750: 6c20 656e 6861 6e63 6520 7468 6520 7265  l enhance the re
-00013760: 6769 6f6e 616c 2069 6e74 6567 7261 7469  gional integrati
-00013770: 6f6e 2061 6e64 2062 6f6f 7374 2074 6865  on and boost the
-00013780: 2065 636f 6e6f 6d69 6320 6772 6f77 7468   economic growth
-00013790: 2e20 4974 2070 6c61 7973 2061 2063 7275  . It plays a cru
-000137a0: 6369 616c 2072 6f6c 6520 696e 2074 6865  cial role in the
-000137b0: 206f 7665 7261 6c6c 2070 6c61 6e20 746f   overall plan to
-000137c0: 2064 6576 656c 6f70 2043 6869 6e61 e280   develop China..
-000137d0: 9973 2047 7265 6174 2042 6179 2041 7265  .s Great Bay Are
-000137e0: 612c 2077 6869 6368 2043 6869 6e61 2069  a, which China i
-000137f0: 6e74 656e 6473 2074 6f20 7475 726e 2069  ntends to turn i
-00013800: 6e74 6f20 6f6e 6520 7269 7661 6c69 6e67  nto one rivaling
-00013810: 2074 686f 7365 206f 6620 5361 6e20 4672   those of San Fr
-00013820: 616e 6369 7363 6f2c 204e 6577 2059 6f72  ancisco, New Yor
-00013830: 6b20 616e 6420 546f 6b79 6f20 696e 2074  k and Tokyo in t
-00013840: 6572 6d73 206f 6620 7465 6368 6e6f 6c6f  erms of technolo
-00013850: 6769 6361 6c20 696e 6e6f 7661 7469 6f6e  gical innovation
-00013860: 2061 6e64 2065 636f 6e6f 6d69 6320 7072   and economic pr
-00013870: 6f73 7065 7269 7479 2e22 2c20 7769 7468  osperity.", with
-00013880: 5f70 6964 3d54 7275 6529 290a 2363 3a5c  _pid=True)).#c:\
-00013890: 7573 6572 735c 7a68 616e 675c 6170 7064  users\zhang\appd
-000138a0: 6174 615c 6c6f 6361 6c5c 7072 6f67 7261  ata\local\progra
-000138b0: 6d73 5c70 7974 686f 6e5c 7079 7468 6f6e  ms\python\python
-000138c0: 3338 5c6c 6962 5c73 6974 652d 7061 636b  38\lib\site-pack
-000138d0: 6167 6573 2020 0a23 2f68 6f6d 652f 7562  ages  .#/home/ub
-000138e0: 756e 7475 2f2e 6c6f 6361 6c2f 6c69 622f  untu/.local/lib/
-000138f0: 7079 7468 6f6e 332e 382f 7369 7465 2d70  python3.8/site-p
-00013900: 6163 6b61 6765 732f 656e 0a27 2727 0a3e  ackages/en.'''.>
-00013910: 3e3e 206d 6f64 656c 2827 6c67 2729 2e76  >> model('lg').v
-00013920: 6f63 6162 0a3c 7370 6163 792e 766f 6361  ocab.<spacy.voca
-00013930: 622e 566f 6361 6220 6f62 6a65 6374 2061  b.Vocab object a
-00013940: 7420 3078 3030 3030 3031 3334 3539 3135  t 0x000001345915
-00013950: 3441 3630 3e0a 3e3e 3e20 6c65 6e28 6d6f  4A60>.>>> len(mo
-00013960: 6465 6c28 276c 6727 292e 766f 6361 6229  del('lg').vocab)
-00013970: 0a37 3638 0a3e 3e3e 206c 656e 286d 6f64  .768.>>> len(mod
-00013980: 656c 2827 736d 2729 2e76 6f63 6162 290a  el('sm').vocab).
-00013990: 3736 370a 2727 27                        767.'''
+000109b0: 2250 4f53 223a 2022 5645 5242 227d 7d2c  "POS": "VERB"}},
+000109c0: 7b22 4c45 4654 5f49 4422 3a20 2276 222c  {"LEFT_ID": "v",
+000109d0: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
+000109e0: 2252 4947 4854 5f49 4422 3a20 226e 222c  "RIGHT_ID": "n",
+000109f0: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
+00010a00: 2244 4550 223a 2022 646f 626a 227d 2020  "DEP": "dobj"}  
+00010a10: 7d2c 207b 224c 4546 545f 4944 223a 2022  }, {"LEFT_ID": "
+00010a20: 7622 2c20 2252 454c 5f4f 5022 3a20 223e  v", "REL_OP": ">
+00010a30: 222c 2022 5249 4748 545f 4944 223a 2022  ", "RIGHT_ID": "
+00010a40: 6164 7622 2c20 2252 4947 4854 5f41 5454  adv", "RIGHT_ATT
+00010a50: 5253 223a 207b 2244 4550 223a 2022 6164  RS": {"DEP": "ad
+00010a60: 766d 6f64 227d 7d5d 2c20 2320 7468 6520  vmod"}}], # the 
+00010a70: 6c61 7374 206f 6e65 202c 2069 7320 7468  last one , is th
+00010a80: 6520 4144 5620 0a09 0922 646f 626a 2d61  e ADV ..."dobj-a
+00010a90: 6d6f 6422 3a20 205b 207b 2252 4947 4854  mod":  [ {"RIGHT
+00010aa0: 5f49 4422 3a20 2276 222c 2020 2252 4947  _ID": "v",  "RIG
+00010ab0: 4854 5f41 5454 5253 223a 207b 2250 4f53  HT_ATTRS": {"POS
+00010ac0: 223a 2022 5645 5242 227d 7d2c 7b22 4c45  ": "VERB"}},{"LE
+00010ad0: 4654 5f49 4422 3a20 2276 222c 2022 5245  FT_ID": "v", "RE
+00010ae0: 4c5f 4f50 223a 2022 3e22 2c20 2252 4947  L_OP": ">", "RIG
+00010af0: 4854 5f49 4422 3a20 226e 222c 2252 4947  HT_ID": "n","RIG
+00010b00: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
+00010b10: 223a 2022 646f 626a 227d 2020 7d2c 207b  ": "dobj"}  }, {
+00010b20: 224c 4546 545f 4944 223a 2022 6e22 2c20  "LEFT_ID": "n", 
+00010b30: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
+00010b40: 5249 4748 545f 4944 223a 2022 6122 2c20  RIGHT_ID": "a", 
+00010b50: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
+00010b60: 2244 4550 223a 2022 616d 6f64 227d 7d5d  "DEP": "amod"}}]
+00010b70: 2c20 2320 312c 342c 3320 2074 6865 206c  , # 1,4,3  the l
+00010b80: 6173 7420 6f6e 6520 6973 2074 6865 2061  ast one is the a
+00010b90: 646a 200a 0909 226e 6261 223a 5b20 7b22  dj ..."nba":[ {"
+00010ba0: 5249 4748 545f 4944 223a 2022 7622 2c22  RIGHT_ID": "v","
+00010bb0: 5249 4748 545f 4154 5452 5322 3a20 7b22  RIGHT_ATTRS": {"
+00010bc0: 4c45 4d4d 4122 3a20 2262 6522 7d7d 2c7b  LEMMA": "be"}},{
+00010bd0: 224c 4546 545f 4944 223a 2022 7622 2c20  "LEFT_ID": "v", 
+00010be0: 2252 454c 5f4f 5022 3a20 223e 222c 2022  "REL_OP": ">", "
+00010bf0: 5249 4748 545f 4944 223a 2022 7375 626a  RIGHT_ID": "subj
+00010c00: 6563 7422 2c20 2252 4947 4854 5f41 5454  ect", "RIGHT_ATT
+00010c10: 5253 223a 207b 2244 4550 223a 2022 6e73  RS": {"DEP": "ns
+00010c20: 7562 6a22 2c20 2250 4f53 223a 224e 4f55  ubj", "POS":"NOU
+00010c30: 4e22 7d7d 2c7b 224c 4546 545f 4944 223a  N"}},{"LEFT_ID":
+00010c40: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
+00010c50: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
+00010c60: 2022 6f62 6a65 6374 222c 2252 4947 4854   "object","RIGHT
+00010c70: 5f41 5454 5253 223a 207b 2244 4550 223a  _ATTRS": {"DEP":
+00010c80: 2022 6163 6f6d 7022 7d7d 5d2c 2020 2320   "acomp"}}],  # 
+00010c90: 6661 7465 2069 7320 676f 6f64 2c20 6669  fate is good, fi
+00010ca0: 6c6d 3a4e 4f55 4e3a 6e62 613a 4144 4a0a  lm:NOUN:nba:ADJ.
+00010cb0: 0909 226e 626e 223a 5b20 7b22 5249 4748  .."nbn":[ {"RIGH
+00010cc0: 545f 4944 223a 2022 7622 2c22 5249 4748  T_ID": "v","RIGH
+00010cd0: 545f 4154 5452 5322 3a20 7b22 4c45 4d4d  T_ATTRS": {"LEMM
+00010ce0: 4122 3a20 2262 6522 7d7d 2c7b 224c 4546  A": "be"}},{"LEF
+00010cf0: 545f 4944 223a 2022 7622 2c20 2252 454c  T_ID": "v", "REL
+00010d00: 5f4f 5022 3a20 223e 222c 2022 5249 4748  _OP": ">", "RIGH
+00010d10: 545f 4944 223a 2022 7375 626a 6563 7422  T_ID": "subject"
+00010d20: 2c20 2252 4947 4854 5f41 5454 5253 223a  , "RIGHT_ATTRS":
+00010d30: 207b 2244 4550 223a 2022 6e73 7562 6a22   {"DEP": "nsubj"
+00010d40: 2c20 2250 4f53 223a 224e 4f55 4e22 7d7d  , "POS":"NOUN"}}
+00010d50: 2c7b 224c 4546 545f 4944 223a 2022 7622  ,{"LEFT_ID": "v"
+00010d60: 2c20 2252 454c 5f4f 5022 3a20 223e 222c  , "REL_OP": ">",
+00010d70: 2022 5249 4748 545f 4944 223a 2022 6f62   "RIGHT_ID": "ob
+00010d80: 6a65 6374 222c 2252 4947 4854 5f41 5454  ject","RIGHT_ATT
+00010d90: 5253 223a 207b 2244 4550 223a 2022 6174  RS": {"DEP": "at
+00010da0: 7472 222c 2022 504f 5322 3a22 4e4f 554e  tr", "POS":"NOUN
+00010db0: 227d 7d5d 2c20 2023 2073 6365 6e65 2069  "}}],  # scene i
+00010dc0: 7320 6120 7374 6f72 790a 0909 226e 6263  s a story..."nbc
+00010dd0: 223a 5b20 7b22 5249 4748 545f 4944 223a  ":[ {"RIGHT_ID":
+00010de0: 2022 7622 2c22 5249 4748 545f 4154 5452   "v","RIGHT_ATTR
+00010df0: 5322 3a20 7b22 4c45 4d4d 4122 3a20 2262  S": {"LEMMA": "b
+00010e00: 6522 7d7d 2c7b 224c 4546 545f 4944 223a  e"}},{"LEFT_ID":
+00010e10: 2022 7622 2c20 2252 454c 5f4f 5022 3a20   "v", "REL_OP": 
+00010e20: 223e 222c 2022 5249 4748 545f 4944 223a  ">", "RIGHT_ID":
+00010e30: 2022 7375 626a 6563 7422 2c20 2252 4947   "subject", "RIG
+00010e40: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
+00010e50: 223a 2022 6e73 7562 6a22 7d7d 2c7b 224c  ": "nsubj"}},{"L
+00010e60: 4546 545f 4944 223a 2022 7622 2c20 2252  EFT_ID": "v", "R
+00010e70: 454c 5f4f 5022 3a20 223e 222c 2022 5249  EL_OP": ">", "RI
+00010e80: 4748 545f 4944 223a 2022 636c 222c 2252  GHT_ID": "cl","R
+00010e90: 4947 4854 5f41 5454 5253 223a 207b 2244  IGHT_ATTRS": {"D
+00010ea0: 4550 223a 2022 6363 6f6d 7022 7d7d 5d2c  EP": "ccomp"}}],
+00010eb0: 2020 2320 796f 7520 6172 6520 7768 6174    # you are what
+00010ec0: 2079 6f75 2072 6561 640a 0909 2261 6476   you read..."adv
+00010ed0: 636c 2d61 636f 6d70 223a 5b20 7b22 5249  cl-acomp":[ {"RI
+00010ee0: 4748 545f 4944 223a 2022 7622 2c20 2022  GHT_ID": "v",  "
+00010ef0: 5249 4748 545f 4154 5452 5322 3a20 7b22  RIGHT_ATTRS": {"
+00010f00: 504f 5322 3a20 2256 4552 4222 7d7d 2c20  POS": "VERB"}}, 
+00010f10: 7b22 4c45 4654 5f49 4422 3a20 2276 222c  {"LEFT_ID": "v",
+00010f20: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
+00010f30: 2252 4947 4854 5f49 4422 3a20 2263 6c76  "RIGHT_ID": "clv
+00010f40: 222c 2022 5249 4748 545f 4154 5452 5322  ", "RIGHT_ATTRS"
+00010f50: 3a20 7b22 4445 5022 3a20 2261 6476 636c  : {"DEP": "advcl
+00010f60: 227d 7d2c 7b22 4c45 4654 5f49 4422 3a20  "}},{"LEFT_ID": 
+00010f70: 2263 6c76 222c 2022 5245 4c5f 4f50 223a  "clv", "REL_OP":
+00010f80: 2022 3e22 2c20 2252 4947 4854 5f49 4422   ">", "RIGHT_ID"
+00010f90: 3a20 226f 626a 6563 7422 2c22 5249 4748  : "object","RIGH
+00010fa0: 545f 4154 5452 5322 3a20 7b22 4445 5022  T_ATTRS": {"DEP"
+00010fb0: 3a20 2261 636f 6d70 227d 7d5d 2c20 2023  : "acomp"}}],  #
+00010fc0: 2022 5768 696c 6520 4920 7761 7320 7468   "While I was th
+00010fd0: 7269 6c6c 6564 2074 6861 7420 6974 2063  rilled that it c
+00010fe0: 7269 6564 2c20 4920 776f 7272 6965 6420  ried, I worried 
+00010ff0: 7468 6174 2049 2077 6f75 6c64 2066 6169  that I would fai
+00011000: 6c2e 0a09 0922 646f 626a 2d70 7274 223a  l...."dobj-prt":
+00011010: 2020 5b20 7b22 5249 4748 545f 4944 223a    [ {"RIGHT_ID":
+00011020: 2022 7622 2c20 2022 5249 4748 545f 4154   "v",  "RIGHT_AT
+00011030: 5452 5322 3a20 7b22 504f 5322 3a20 2256  TRS": {"POS": "V
+00011040: 4552 4222 7d7d 2c7b 224c 4546 545f 4944  ERB"}},{"LEFT_ID
+00011050: 223a 2022 7622 2c20 2252 454c 5f4f 5022  ": "v", "REL_OP"
+00011060: 3a20 223e 222c 2022 5249 4748 545f 4944  : ">", "RIGHT_ID
+00011070: 223a 2022 7072 7422 2c22 5249 4748 545f  ": "prt","RIGHT_
+00011080: 4154 5452 5322 3a20 7b22 4445 5022 3a20  ATTRS": {"DEP": 
+00011090: 2270 7274 227d 2020 7d2c 207b 224c 4546  "prt"}  }, {"LEF
+000110a0: 545f 4944 223a 2022 7622 2c20 2252 454c  T_ID": "v", "REL
+000110b0: 5f4f 5022 3a20 223e 222c 2022 5249 4748  _OP": ">", "RIGH
+000110c0: 545f 4944 223a 2022 6e22 2c20 2252 4947  T_ID": "n", "RIG
+000110d0: 4854 5f41 5454 5253 223a 207b 2244 4550  HT_ATTRS": {"DEP
+000110e0: 223a 2022 646f 626a 222c 2022 504f 5322  ": "dobj", "POS"
+000110f0: 3a22 4e4f 554e 222c 2249 535f 414c 5048  :"NOUN","IS_ALPH
+00011100: 4122 3a54 7275 652c 2249 535f 4c4f 5745  A":True,"IS_LOWE
+00011110: 5222 3a54 7275 657d 7d5d 2c20 2320 7475  R":True}}], # tu
+00011120: 726e 206f 6666 2074 6865 2072 6164 696f  rn off the radio
+00011130: 200a 0909 2276 704e 223a 205b 207b 2252   ..."vpN": [ {"R
+00011140: 4947 4854 5f49 4422 3a20 2276 222c 2020  IGHT_ID": "v",  
+00011150: 2252 4947 4854 5f41 5454 5253 223a 207b  "RIGHT_ATTRS": {
+00011160: 2250 4f53 223a 2022 5645 5242 222c 2249  "POS": "VERB","I
+00011170: 535f 414c 5048 4122 3a54 7275 657d 7d2c  S_ALPHA":True}},
+00011180: 7b22 4c45 4654 5f49 4422 3a20 2276 222c  {"LEFT_ID": "v",
+00011190: 2022 5245 4c5f 4f50 223a 2022 3e22 2c20   "REL_OP": ">", 
+000111a0: 2252 4947 4854 5f49 4422 3a20 2270 7265  "RIGHT_ID": "pre
+000111b0: 7022 2c22 5249 4748 545f 4154 5452 5322  p","RIGHT_ATTRS"
+000111c0: 3a20 7b22 4445 5022 3a20 2270 7265 7022  : {"DEP": "prep"
+000111d0: 2c22 4953 5f4c 4f57 4552 223a 5472 7565  ,"IS_LOWER":True
+000111e0: 2c22 4953 5f41 4c50 4841 223a 5472 7565  ,"IS_ALPHA":True
+000111f0: 7d20 207d 2c20 7b22 4c45 4654 5f49 4422  }  }, {"LEFT_ID"
+00011200: 3a20 2270 7265 7022 2c20 2252 454c 5f4f  : "prep", "REL_O
+00011210: 5022 3a20 223e 222c 2022 5249 4748 545f  P": ">", "RIGHT_
+00011220: 4944 223a 2022 6e22 2c20 2252 4947 4854  ID": "n", "RIGHT
+00011230: 5f41 5454 5253 223a 207b 2244 4550 223a  _ATTRS": {"DEP":
+00011240: 2022 706f 626a 222c 2022 504f 5322 3a22   "pobj", "POS":"
+00011250: 4e4f 554e 222c 2249 535f 414c 5048 4122  NOUN","IS_ALPHA"
+00011260: 3a54 7275 657d 7d5d 2c20 2320 6a75 6d70  :True}}], # jump
+00011270: 206f 7665 7220 7468 6520 646f 672c 2064   over the dog, d
+00011280: 6966 6620 6672 6f6d 2063 6f6d 6520 696e  iff from come in
+00011290: 746f 2066 6f72 6365 2f4e 4e0a 0909 7d29  to force/NN...})
+000112a0: 2020 2320 6e62 653f 206e 6278 203d 206e    # nbe? nbx = n
+000112b0: 6261 202b 206e 6265 202b 206e 626e 0a09  ba + nbe + nbn..
+000112c0: 666f 7220 6e61 6d65 2c20 6172 2069 6e20  for name, ar in 
+000112d0: 7472 7033 5f6d 6174 6368 2e6d 6174 6368  trp3_match.match
+000112e0: 6572 2864 6f63 293a 0a09 0974 7279 3a0a  er(doc):...try:.
+000112f0: 0909 0974 6167 203d 2073 7061 6379 2e6e  ...tag = spacy.n
+00011300: 6c70 2e76 6f63 6162 5b6e 616d 655d 2e74  lp.vocab[name].t
+00011310: 6578 740a 0909 0969 2c6a 2c6b 203d 2061  ext....i,j,k = a
+00011320: 725b 303a 335d 200a 0909 0969 6620 6973  r[0:3] ....if is
+00011330: 696e 7374 616e 6365 2866 756e 632c 2064  instance(func, d
+00011340: 6963 7429 3a20 2320 7461 6720 2d3e 206c  ict): # tag -> l
+00011350: 616d 6264 6120 0a09 0909 0966 756e 635b  ambda .....func[
+00011360: 7461 675d 2864 6f63 2c20 692c 206a 2c20  tag](doc, i, j, 
+00011370: 6b2c 2074 6167 2920 6966 2074 6167 2069  k, tag) if tag i
+00011380: 6e20 6675 6e63 2065 6c73 6520 7072 696e  n func else prin
+00011390: 7428 2249 6e76 616c 6964 2074 6167 3a22  t("Invalid tag:"
+000113a0: 2c20 7461 672c 2069 2c6a 2c6b 2029 0a09  , tag, i,j,k )..
+000113b0: 0909 656c 7365 3a20 0a09 0909 0966 756e  ..else: .....fun
+000113c0: 6328 646f 632c 2069 2c20 6a2c 206b 2c20  c(doc, i, j, k, 
+000113d0: 7461 6729 2023 2064 6f63 2e73 7061 6e73  tag) # doc.spans
+000113e0: 5b66 2274 7270 335b 7b69 7d2c 7b6a 7d2c  [f"trp3[{i},{j},
+000113f0: 7b6b 7d5d 3a7b 7461 677d 225d 203d 2053  {k}]:{tag}"] = S
+00011400: 7061 6e47 726f 7570 2864 6f63 2c20 6e61  panGroup(doc, na
+00011410: 6d65 3d74 6167 2c20 7370 616e 733d 5b20  me=tag, spans=[ 
+00011420: 646f 635b 693a 692b 315d 2c20 646f 635b  doc[i:i+1], doc[
+00011430: 6a3a 6a2b 315d 2c20 646f 635b 6b3a 6b2b  j:j+1], doc[k:k+
+00011440: 315d 205d 2c20 6174 7472 733d 7b22 7461  1] ], attrs={"ta
+00011450: 6722 3a74 6167 2c20 2269 223a 692c 226a  g":tag, "i":i,"j
+00011460: 223a 6a2c 2022 6b22 3a6b 7d29 200a 0909  ":j, "k":k}) ...
+00011470: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00011480: 2061 7320 653a 0a09 0909 7072 696e 7420   as e:....print 
+00011490: 2822 7472 7033 5f6d 6174 6368 2065 783a  ("trp3_match ex:
+000114a0: 222c 2065 2c20 6e61 6d65 2c20 6172 2920  ", e, name, ar) 
+000114b0: 0a0a 7370 616e 5f4e 5020 3d20 6c61 6d62  ..span_NP = lamb
+000114c0: 6461 2073 703a 2022 2022 2e6a 6f69 6e28  da sp: " ".join(
+000114d0: 5b20 225f 4e50 2220 6966 2074 2e65 6e74  [ "_NP" if t.ent
+000114e0: 5f74 7970 655f 203d 3d20 274e 5027 2065  _type_ == 'NP' e
+000114f0: 6c73 6520 742e 7465 7874 2e6c 6f77 6572  lse t.text.lower
+00011500: 2829 2066 6f72 2074 2069 6e20 7370 5d29  () for t in sp])
+00011510: 2023 656c 7365 2066 225f 7b74 2e74 6167   #else f"_{t.tag
+00011520: 5f7d 2220 6966 2074 2e74 6167 5f20 696e  _}" if t.tag_ in
+00011530: 2028 2756 424e 2729 0a64 6566 2073 6b65   ('VBN').def ske
+00011540: 6e70 5f66 756e 635f 6b70 2864 6f63 2c20  np_func_kp(doc, 
+00011550: 7374 6172 742c 2065 6e64 2c20 7461 6729  start, end, tag)
+00011560: 3a20 2320 736b 656e 705f 6675 6e63 5f6b  : # skenp_func_k
+00011570: 7009 3d20 6c61 6d62 6461 2064 6f63 2c20  p.= lambda doc, 
+00011580: 7374 6172 742c 2065 6e64 2c20 7461 673a  start, end, tag:
+00011590: 2064 6f63 2e75 7365 725f 6461 7461 2e75   doc.user_data.u
+000115a0: 7064 6174 6528 7b66 227b 7461 677d 3a7b  pdate({f"{tag}:{
+000115b0: 646f 635b 7374 6172 745d 2e6c 656d 6d61  doc[start].lemma
+000115c0: 5f7d 2022 202b 2073 7061 6e5f 4e50 2864  _} " + span_NP(d
+000115d0: 6f63 5b73 7461 7274 2b31 3a65 6e64 5d29  oc[start+1:end])
+000115e0: 203a 207b 2276 6c65 6d22 3a64 6f63 5b73   : {"vlem":doc[s
+000115f0: 7461 7274 5d2e 6c65 6d6d 615f 2c20 2273  tart].lemma_, "s
+00011600: 7461 7274 223a 7374 6172 742c 2022 656e  tart":start, "en
+00011610: 6422 3a65 6e64 2c20 226e 6163 223a 205b  d":end, "nac": [
+00011620: 6622 7b64 6f63 5b73 7461 7274 5d2e 6c65  f"{doc[start].le
+00011630: 6d6d 615f 7d3a 5645 5242 3a7b 7461 677d  mma_}:VERB:{tag}
+00011640: 7c22 202b 7370 616e 5f4e 5028 646f 635b  |" +span_NP(doc[
+00011650: 7374 6172 743a 656e 645d 2029 2c20 6622  start:end] ), f"
+00011660: 7b64 6f63 5b73 7461 7274 5d2e 6c65 6d6d  {doc[start].lemm
+00011670: 615f 7d3a 5645 5242 7c7b 7461 677d 222c  a_}:VERB|{tag}",
+00011680: 2066 222a 3a56 4552 427c 7b74 6167 7d22   f"*:VERB|{tag}"
+00011690: 5d7d 207d 2920 0a09 6e61 6320 3d20 5b66  ]} }) ..nac = [f
+000116a0: 227b 646f 635b 7374 6172 745d 2e6c 656d  "{doc[start].lem
+000116b0: 6d61 5f7d 3a56 4552 423a 7b74 6167 7d7c  ma_}:VERB:{tag}|
+000116c0: 2220 2b73 7061 6e5f 4e50 2864 6f63 5b73  " +span_NP(doc[s
+000116d0: 7461 7274 3a65 6e64 5d20 292c 2066 227b  tart:end] ), f"{
+000116e0: 646f 635b 7374 6172 745d 2e6c 656d 6d61  doc[start].lemma
+000116f0: 5f7d 3a56 4552 427c 7b74 6167 7d22 2c20  _}:VERB|{tag}", 
+00011700: 6622 2a3a 5645 5242 7c7b 7461 677d 225d  f"*:VERB|{tag}"]
+00011710: 0a09 6966 2074 6167 2069 6e20 2827 766e  ..if tag in ('vn
+00011720: 706e 2729 3a20 2320 7461 6b65 205f 4e50  pn'): # take _NP
+00011730: 2069 6e74 6f20 6163 636f 756e 742c 2061   into account, a
+00011740: 6464 6564 2032 3032 332e 322e 3134 0a09  dded 2023.2.14..
+00011750: 096e 6163 2e65 7874 656e 6428 5b66 227b  .nac.extend([f"{
+00011760: 646f 635b 656e 642d 315d 2e74 6578 742e  doc[end-1].text.
+00011770: 6c6f 7765 7228 297d 3a4e 4f55 4e3a 7b74  lower()}:NOUN:{t
+00011780: 6167 7d7c 2220 2b64 6f63 5b73 7461 7274  ag}|" +doc[start
+00011790: 5d2e 6c65 6d6d 615f 202b 2022 2022 202b  ].lemma_ + " " +
+000117a0: 2073 7061 6e5f 4e50 2864 6f63 5b73 7461   span_NP(doc[sta
+000117b0: 7274 2b31 3a65 6e64 2d31 5d29 202b 2022  rt+1:end-1]) + "
+000117c0: 2022 202b 2064 6f63 5b65 6e64 2d31 5d2e   " + doc[end-1].
+000117d0: 7465 7874 2e6c 6f77 6572 2829 2c20 6622  text.lower(), f"
+000117e0: 7b64 6f63 5b65 6e64 2d31 5d2e 7465 7874  {doc[end-1].text
+000117f0: 2e6c 6f77 6572 2829 7d3a 4e4f 554e 7c7b  .lower()}:NOUN|{
+00011800: 7461 677d 222c 2066 222a 3a4e 4f55 4e7c  tag}", f"*:NOUN|
+00011810: 7b74 6167 7d22 2c20 6622 7b64 6f63 5b65  {tag}", f"{doc[e
+00011820: 6e64 2d31 5d2e 7465 7874 2e6c 6f77 6572  nd-1].text.lower
+00011830: 2829 7d2f 4e4f 554e 7c7b 7461 677d 3a5f  ()}/NOUN|{tag}:_
+00011840: 2220 2b64 6f63 5b73 7461 7274 5d2e 6c65  " +doc[start].le
+00011850: 6d6d 615f 202b 2022 2022 202b 2073 7061  mma_ + " " + spa
+00011860: 6e5f 4e50 2864 6f63 5b73 7461 7274 2b31  n_NP(doc[start+1
+00011870: 3a65 6e64 2d31 5d29 202b 2022 2022 202b  :end-1]) + " " +
+00011880: 2064 6f63 5b65 6e64 2d31 5d2e 7465 7874   doc[end-1].text
+00011890: 2e6c 6f77 6572 2829 5d29 0a09 6966 2074  .lower()])..if t
+000118a0: 6167 2069 6e20 2822 766e 7065 2229 3a20  ag in ("vnpe"): 
+000118b0: 2320 7461 6b65 205f 4e50 2066 6f72 2067  # take _NP for g
+000118c0: 7261 6e74 6564 0a09 096e 6163 2e65 7874  ranted...nac.ext
+000118d0: 656e 6428 5b66 227b 646f 635b 656e 642d  end([f"{doc[end-
+000118e0: 315d 2e6c 656d 6d61 5f7d 3a56 4552 423a  1].lemma_}:VERB:
+000118f0: 7b74 6167 7d7c 2220 2b73 7061 6e5f 4e50  {tag}|" +span_NP
+00011900: 2864 6f63 5b73 7461 7274 3a65 6e64 5d29  (doc[start:end])
+00011910: 2c20 6622 7b64 6f63 5b65 6e64 2d31 5d2e  , f"{doc[end-1].
+00011920: 6c65 6d6d 615f 7d3a 5645 5242 7c7b 7461  lemma_}:VERB|{ta
+00011930: 677d 222c 2066 222a 3a56 4552 427c 7b74  g}", f"*:VERB|{t
+00011940: 6167 7d22 2c20 0a09 0909 6622 7b64 6f63  ag}", ....f"{doc
+00011950: 5b65 6e64 2d31 5d2e 6c65 6d6d 615f 7d2f  [end-1].lemma_}/
+00011960: 5645 5242 7c76 6e70 653a 5f7b 646f 635b  VERB|vnpe:_{doc[
+00011970: 7374 6172 745d 2e6c 656d 6d61 5f7d 205f  start].lemma_} _
+00011980: 4e50 2022 202b 646f 635b 7374 6172 742b  NP " +doc[start+
+00011990: 323a 656e 645d 2e74 6578 742e 6c6f 7765  2:end].text.lowe
+000119a0: 7228 292c 5d29 0a09 6966 2074 6167 2069  r(),])..if tag i
+000119b0: 6e20 2822 766e 2229 3a20 6e61 632e 6578  n ("vn"): nac.ex
+000119c0: 7465 6e64 285b 6622 7b64 6f63 5b73 7461  tend([f"{doc[sta
+000119d0: 7274 5d2e 6c65 6d6d 615f 7d2f 5645 5242  rt].lemma_}/VERB
+000119e0: 7c76 6e3a 5f7b 646f 635b 7374 6172 745d  |vn:_{doc[start]
+000119f0: 2e6c 656d 6d61 5f7d 205f 4e50 225d 290a  .lemma_} _NP"]).
+00011a00: 0969 6620 7461 6720 3d3d 2022 766e 6122  .if tag == "vna"
+00011a10: 3a20 6e61 632e 6578 7465 6e64 285b 6622  : nac.extend([f"
+00011a20: 7b64 6f63 5b73 7461 7274 5d2e 6c65 6d6d  {doc[start].lemm
+00011a30: 615f 7d2f 5645 5242 7c76 6e61 3a5f 7b64  a_}/VERB|vna:_{d
+00011a40: 6f63 5b73 7461 7274 5d2e 6c65 6d6d 615f  oc[start].lemma_
+00011a50: 7d20 5f4e 5020 5f41 444a 225d 290a 0969  } _NP _ADJ"])..i
+00011a60: 6620 7461 6720 696e 2028 2276 6e6e 2229  f tag in ("vnn")
+00011a70: 3a20 6e61 632e 6578 7465 6e64 285b 6622  : nac.extend([f"
+00011a80: 7b64 6f63 5b73 7461 7274 5d2e 6c65 6d6d  {doc[start].lemm
+00011a90: 615f 7d2f 5645 5242 7c76 6e6e 3a5f 7b64  a_}/VERB|vnn:_{d
+00011aa0: 6f63 5b73 7461 7274 5d2e 6c65 6d6d 615f  oc[start].lemma_
+00011ab0: 7d20 5f4e 5020 5f4e 5022 5d29 0a09 6966  } _NP _NP"])..if
+00011ac0: 2074 6167 2069 6e20 2822 766e 6522 293a   tag in ("vne"):
+00011ad0: 206e 6163 2e65 7874 656e 6428 5b66 227b   nac.extend([f"{
+00011ae0: 646f 635b 7374 6172 745d 2e6c 656d 6d61  doc[start].lemma
+00011af0: 5f7d 2f56 4552 427c 766e 653a 5f7b 646f  _}/VERB|vne:_{do
+00011b00: 635b 7374 6172 745d 2e6c 656d 6d61 5f7d  c[start].lemma_}
+00011b10: 205f 4e50 205f 5642 4e22 5d29 0a09 646f   _NP _VBN"])..do
+00011b20: 632e 7573 6572 5f64 6174 612e 7570 6461  c.user_data.upda
+00011b30: 7465 287b 6622 7b74 6167 7d3a 7b64 6f63  te({f"{tag}:{doc
+00011b40: 5b73 7461 7274 5d2e 6c65 6d6d 615f 7d20  [start].lemma_} 
+00011b50: 2220 2b20 7370 616e 5f4e 5028 646f 635b  " + span_NP(doc[
+00011b60: 7374 6172 742b 313a 656e 645d 2920 3a20  start+1:end]) : 
+00011b70: 7b22 766c 656d 223a 646f 635b 7374 6172  {"vlem":doc[star
+00011b80: 745d 2e6c 656d 6d61 5f2c 2022 7374 6172  t].lemma_, "star
+00011b90: 7422 3a73 7461 7274 2c20 2265 6e64 223a  t":start, "end":
+00011ba0: 656e 642c 2022 6e61 6322 3a6e 6163 7d20  end, "nac":nac} 
+00011bb0: 7d29 0a0a 7472 7033 5f66 756e 635f 6b70  })..trp3_func_kp
+00011bc0: 203d 207b 2023 6472 696e 6b3a 5645 5242   = { #drink:VERB
+00011bd0: 3a64 6f62 6a3a 4e4f 554e 3a77 6174 6572  :dobj:NOUN:water
+00011be0: 3a61 6d6f 643a 4144 4a20 7361 6665 0a09  :amod:ADJ safe..
+00011bf0: 2264 6f62 6a2d 6164 766d 6f64 223a 096c  "dobj-advmod":.l
+00011c00: 616d 6264 6120 646f 632c 2069 2c20 6a2c  ambda doc, i, j,
+00011c10: 206b 2c20 7461 673a 2020 646f 632e 7573   k, tag:  doc.us
+00011c20: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
+00011c30: 6622 646f 626a 2d61 6476 6d6f 643a 7b64  f"dobj-advmod:{d
+00011c40: 6f63 5b6b 5d2e 7465 7874 7d20 7b64 6f63  oc[k].text} {doc
+00011c50: 5b69 5d2e 6c65 6d6d 615f 7d20 7b64 6f63  [i].lemma_} {doc
+00011c60: 5b6a 5d2e 6c65 6d6d 615f 7d5b 7b69 7d2c  [j].lemma_}[{i},
+00011c70: 7b6a 7d2c 7b6b 7d5d 223a 207b 2274 6167  {j},{k}]": {"tag
+00011c80: 223a 7461 672c 2022 6672 6f6d 223a 2274  ":tag, "from":"t
+00011c90: 7270 3322 202c 0a09 0909 0909 0922 6e61  rp3" ,......."na
+00011ca0: 6322 3a5b 6622 7b64 6f63 5b69 5d2e 6c65  c":[f"{doc[i].le
+00011cb0: 6d6d 615f 7d3a 7b64 6f63 5b69 5d2e 706f  mma_}:{doc[i].po
+00011cc0: 735f 7d3a 7b64 6f63 5b6a 5d2e 6465 705f  s_}:{doc[j].dep_
+00011cd0: 7d3a 7b64 6f63 5b6a 5d2e 706f 735f 7d3a  }:{doc[j].pos_}:
+00011ce0: 7b64 6f63 5b6a 5d2e 6c65 6d6d 615f 7d3a  {doc[j].lemma_}:
+00011cf0: 7b64 6f63 5b6b 5d2e 6465 705f 7d2d 7b64  {doc[k].dep_}-{d
+00011d00: 6f63 5b6b 5d2e 706f 735f 7d7c 7b64 6f63  oc[k].pos_}|{doc
+00011d10: 5b6b 5d2e 6c65 6d6d 615f 7d22 2c66 227b  [k].lemma_}",f"{
+00011d20: 646f 635b 695d 2e6c 656d 6d61 5f7d 3a7b  doc[i].lemma_}:{
+00011d30: 646f 635b 695d 2e70 6f73 5f7d 3a7b 646f  doc[i].pos_}:{do
+00011d40: 635b 6a5d 2e64 6570 5f7d 3a7b 646f 635b  c[j].dep_}:{doc[
+00011d50: 6a5d 2e70 6f73 5f7d 3a7b 646f 635b 6a5d  j].pos_}:{doc[j]
+00011d60: 2e6c 656d 6d61 5f7d 7c7b 646f 635b 6b5d  .lemma_}|{doc[k]
+00011d70: 2e64 6570 5f7d 2d7b 646f 635b 6b5d 2e70  .dep_}-{doc[k].p
+00011d80: 6f73 5f7d 225d 7d7d 292c 200a 0922 646f  os_}"]}}), .."do
+00011d90: 626a 2d61 6d6f 6422 3a09 6c61 6d62 6461  bj-amod":.lambda
+00011da0: 2064 6f63 2c20 692c 206a 2c20 6b2c 2074   doc, i, j, k, t
+00011db0: 6167 3a20 2064 6f63 2e75 7365 725f 6461  ag:  doc.user_da
+00011dc0: 7461 2e75 7064 6174 6528 7b66 2264 6f62  ta.update({f"dob
+00011dd0: 6a2d 616d 6f64 3a7b 646f 635b 695d 2e6c  j-amod:{doc[i].l
+00011de0: 656d 6d61 5f7d 207b 646f 635b 6a5d 2e74  emma_} {doc[j].t
+00011df0: 6578 747d 207b 646f 635b 6b5d 2e6c 656d  ext} {doc[k].lem
+00011e00: 6d61 5f7d 5b7b 697d 2c7b 6a7d 2c7b 6b7d  ma_}[{i},{j},{k}
+00011e10: 5d22 3a20 7b22 7461 6722 3a74 6167 2c20  ]": {"tag":tag, 
+00011e20: 2266 726f 6d22 3a22 7472 7033 2220 2c0a  "from":"trp3" ,.
+00011e30: 0909 0909 0909 226e 6163 223a 5b66 227b  ......"nac":[f"{
+00011e40: 646f 635b 695d 2e6c 656d 6d61 5f7d 3a7b  doc[i].lemma_}:{
+00011e50: 646f 635b 695d 2e70 6f73 5f7d 3a7b 646f  doc[i].pos_}:{do
+00011e60: 635b 6a5d 2e64 6570 5f7d 3a7b 646f 635b  c[j].dep_}:{doc[
+00011e70: 6a5d 2e70 6f73 5f7d 3a7b 646f 635b 6a5d  j].pos_}:{doc[j]
+00011e80: 2e6c 656d 6d61 5f7d 3a7b 646f 635b 6b5d  .lemma_}:{doc[k]
+00011e90: 2e64 6570 5f7d 2d7b 646f 635b 6b5d 2e70  .dep_}-{doc[k].p
+00011ea0: 6f73 5f7d 7c7b 646f 635b 6b5d 2e6c 656d  os_}|{doc[k].lem
+00011eb0: 6d61 5f7d 222c 6622 7b64 6f63 5b69 5d2e  ma_}",f"{doc[i].
+00011ec0: 6c65 6d6d 615f 7d3a 7b64 6f63 5b69 5d2e  lemma_}:{doc[i].
+00011ed0: 706f 735f 7d3a 7b64 6f63 5b6a 5d2e 6465  pos_}:{doc[j].de
+00011ee0: 705f 7d3a 7b64 6f63 5b6a 5d2e 706f 735f  p_}:{doc[j].pos_
+00011ef0: 7d3a 7b64 6f63 5b6a 5d2e 6c65 6d6d 615f  }:{doc[j].lemma_
+00011f00: 7d7c 7b64 6f63 5b6b 5d2e 6465 705f 7d2d  }|{doc[k].dep_}-
+00011f10: 7b64 6f63 5b6b 5d2e 706f 735f 7d22 5d7d  {doc[k].pos_}"]}
+00011f20: 7d29 2c20 0a09 226e 6261 223a 0909 096c  }), .."nba":...l
+00011f30: 616d 6264 6120 646f 632c 2069 2c20 6a2c  ambda doc, i, j,
+00011f40: 206b 2c20 7461 673a 2020 646f 632e 7573   k, tag:  doc.us
+00011f50: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
+00011f60: 6622 6e62 613a 7b64 6f63 5b6a 5d2e 6c65  f"nba:{doc[j].le
+00011f70: 6d6d 615f 7d20 7b64 6f63 5b6b 5d2e 7465  mma_} {doc[k].te
+00011f80: 7874 7d5b 7b69 7d2c 7b6a 7d2c 7b6b 7d5d  xt}[{i},{j},{k}]
+00011f90: 223a 7b22 7461 6722 3a74 6167 2c20 2266  ":{"tag":tag, "f
+00011fa0: 726f 6d22 3a22 7472 7033 222c 2023 2077  rom":"trp3", # w
+00011fb0: 6865 6e20 7468 6572 6520 6973 206e 6f20  hen there is no 
+00011fc0: 616d 6269 2c20 6e6f 206e 6565 6420 746f  ambi, no need to
+00011fd0: 2061 6464 207e 200a 0909 0909 0909 226e   add ~ ......."n
+00011fe0: 6163 223a 5b66 227b 646f 635b 6a5d 2e6c  ac":[f"{doc[j].l
+00011ff0: 656d 6d61 5f7d 3a7b 646f 635b 6a5d 2e70  emma_}:{doc[j].p
+00012000: 6f73 5f7d 3a7b 7461 677d 7c7b 646f 635b  os_}:{tag}|{doc[
+00012010: 6b5d 2e6c 656d 6d61 5f7d 222c 6622 7b64  k].lemma_}",f"{d
+00012020: 6f63 5b6a 5d2e 6c65 6d6d 615f 7d3a 7b64  oc[j].lemma_}:{d
+00012030: 6f63 5b6a 5d2e 706f 735f 7d7c 7b74 6167  oc[j].pos_}|{tag
+00012040: 7d22 2c66 227b 646f 635b 6b5d 2e6c 656d  }",f"{doc[k].lem
+00012050: 6d61 5f7d 3a7b 646f 635b 6b5d 2e70 6f73  ma_}:{doc[k].pos
+00012060: 5f7d 3a7b 7461 677d 7c7b 646f 635b 6a5d  _}:{tag}|{doc[j]
+00012070: 2e6c 656d 6d61 5f7d 222c 6622 7b64 6f63  .lemma_}",f"{doc
+00012080: 5b6b 5d2e 6c65 6d6d 615f 7d3a 7b64 6f63  [k].lemma_}:{doc
+00012090: 5b6b 5d2e 706f 735f 7d7c 7b74 6167 7d22  [k].pos_}|{tag}"
+000120a0: 5d7d 7d29 2c20 0a09 226e 626e 223a 0909  ]}}), .."nbn":..
+000120b0: 096c 616d 6264 6120 646f 632c 2069 2c20  .lambda doc, i, 
+000120c0: 6a2c 206b 2c20 7461 673a 2020 646f 632e  j, k, tag:  doc.
+000120d0: 7573 6572 5f64 6174 612e 7570 6461 7465  user_data.update
+000120e0: 287b 6622 6e62 6e3a 7b64 6f63 5b6a 5d2e  ({f"nbn:{doc[j].
+000120f0: 6c65 6d6d 615f 7d20 7b64 6f63 5b6b 5d2e  lemma_} {doc[k].
+00012100: 6c65 6d6d 615f 7d5b 7b69 7d2c 7b6a 7d2c  lemma_}[{i},{j},
+00012110: 7b6b 7d5d 223a 7b22 7461 6722 3a74 6167  {k}]":{"tag":tag
+00012120: 2c20 2266 726f 6d22 3a22 7472 7033 222c  , "from":"trp3",
+00012130: 0a09 0909 0909 0922 6e61 6322 3a5b 6622  ......."nac":[f"
+00012140: 7b64 6f63 5b6a 5d2e 6c65 6d6d 615f 7d3a  {doc[j].lemma_}:
+00012150: 7b64 6f63 5b6a 5d2e 706f 735f 7d3a 7b74  {doc[j].pos_}:{t
+00012160: 6167 7d7c 7b64 6f63 5b6b 5d2e 6c65 6d6d  ag}|{doc[k].lemm
+00012170: 615f 7d22 2c66 227b 646f 635b 6a5d 2e6c  a_}",f"{doc[j].l
+00012180: 656d 6d61 5f7d 3a7b 646f 635b 6a5d 2e70  emma_}:{doc[j].p
+00012190: 6f73 5f7d 7c7b 7461 677d 222c 6622 7b64  os_}|{tag}",f"{d
+000121a0: 6f63 5b6b 5d2e 6c65 6d6d 615f 7d3a 7b64  oc[k].lemma_}:{d
+000121b0: 6f63 5b6b 5d2e 706f 735f 7d3a 7e7b 7461  oc[k].pos_}:~{ta
+000121c0: 677d 7c7b 646f 635b 6a5d 2e6c 656d 6d61  g}|{doc[j].lemma
+000121d0: 5f7d 222c 6622 7b64 6f63 5b6b 5d2e 6c65  _}",f"{doc[k].le
+000121e0: 6d6d 615f 7d3a 7b64 6f63 5b6b 5d2e 706f  mma_}:{doc[k].po
+000121f0: 735f 7d7c 7e7b 7461 677d 225d 7d7d 292c  s_}|~{tag}"]}}),
+00012200: 200a 0922 6e62 6322 3a09 0909 6c61 6d62   .."nbc":...lamb
+00012210: 6461 2064 6f63 2c20 692c 206a 2c20 6b2c  da doc, i, j, k,
+00012220: 2074 6167 3a20 2064 6f63 2e75 7365 725f   tag:  doc.user_
+00012230: 6461 7461 2e75 7064 6174 6528 7b66 226e  data.update({f"n
+00012240: 6263 3a7b 646f 635b 6a5d 2e6c 656d 6d61  bc:{doc[j].lemma
+00012250: 5f7d 205f 434c 5b7b 697d 2c7b 6a7d 2c7b  _} _CL[{i},{j},{
+00012260: 6b7d 5d22 3a7b 2274 6167 223a 7461 672c  k}]":{"tag":tag,
+00012270: 2022 6672 6f6d 223a 2274 7270 3322 2c0a   "from":"trp3",.
+00012280: 0909 0909 0909 226e 6163 223a 5b66 227b  ......"nac":[f"{
+00012290: 646f 635b 6a5d 2e6c 656d 6d61 5f7d 3a7b  doc[j].lemma_}:{
+000122a0: 646f 635b 6a5d 2e70 6f73 5f7d 7c7b 7461  doc[j].pos_}|{ta
+000122b0: 677d 225d 7d7d 292c 200a 0922 6164 7663  g}"]}}), .."advc
+000122c0: 6c2d 6163 6f6d 7022 3a09 6c61 6d62 6461  l-acomp":.lambda
+000122d0: 2064 6f63 2c20 692c 206a 2c20 6b2c 2074   doc, i, j, k, t
+000122e0: 6167 3a20 2064 6f63 2e75 7365 725f 6461  ag:  doc.user_da
+000122f0: 7461 2e75 7064 6174 6528 7b66 2261 6476  ta.update({f"adv
+00012300: 636c 2d61 636f 6d70 3a7b 646f 635b 695d  cl-acomp:{doc[i]
+00012310: 2e6c 656d 6d61 5f7d 207b 646f 635b 6b5d  .lemma_} {doc[k]
+00012320: 2e74 6578 747d 5b7b 697d 2c7b 6a7d 2c7b  .text}[{i},{j},{
+00012330: 6b7d 5d22 3a7b 2274 6167 223a 7461 672c  k}]":{"tag":tag,
+00012340: 2022 6672 6f6d 223a 2274 7270 3322 2c0a   "from":"trp3",.
+00012350: 0909 0909 0909 226e 6163 223a 5b66 227b  ......"nac":[f"{
+00012360: 646f 635b 695d 2e6c 656d 6d61 5f7d 3a7b  doc[i].lemma_}:{
+00012370: 646f 635b 695d 2e70 6f73 5f7d 3a61 6476  doc[i].pos_}:adv
+00012380: 636c 2d61 636f 6d70 7c7b 646f 635b 6b5d  cl-acomp|{doc[k]
+00012390: 2e74 6578 742e 6c6f 7765 7228 297d 222c  .text.lower()}",
+000123a0: 6622 7b64 6f63 5b6b 5d2e 7465 7874 2e6c  f"{doc[k].text.l
+000123b0: 6f77 6572 2829 7d3a 7b64 6f63 5b6b 5d2e  ower()}:{doc[k].
+000123c0: 7461 675f 2069 6620 646f 635b 6b5d 2e74  tag_ if doc[k].t
+000123d0: 6167 5f20 3d3d 2027 5642 4e27 2065 6c73  ag_ == 'VBN' els
+000123e0: 6520 646f 635b 6b5d 2e70 6f73 5f7d 3a7e  e doc[k].pos_}:~
+000123f0: 6164 7663 6c2d 6163 6f6d 707c 7b64 6f63  advcl-acomp|{doc
+00012400: 5b69 5d2e 6c65 6d6d 615f 7d22 2c66 227b  [i].lemma_}",f"{
+00012410: 646f 635b 695d 2e6c 656d 6d61 5f7d 3a7b  doc[i].lemma_}:{
+00012420: 646f 635b 695d 2e70 6f73 5f7d 7c61 6476  doc[i].pos_}|adv
+00012430: 636c 2d61 636f 6d70 222c 6622 7b64 6f63  cl-acomp",f"{doc
+00012440: 5b6b 5d2e 7465 7874 2e6c 6f77 6572 2829  [k].text.lower()
+00012450: 7d3a 7b64 6f63 5b6b 5d2e 7461 675f 2069  }:{doc[k].tag_ i
+00012460: 6620 646f 635b 6b5d 2e74 6167 5f20 3d3d  f doc[k].tag_ ==
+00012470: 2027 5642 4e27 2065 6c73 6520 646f 635b   'VBN' else doc[
+00012480: 6b5d 2e70 6f73 5f7d 7c7e 6164 7663 6c2d  k].pos_}|~advcl-
+00012490: 6163 6f6d 7022 5d7d 7d29 2c20 0a09 2264  acomp"]}}), .."d
+000124a0: 6f62 6a2d 7072 7422 3a09 096c 616d 6264  obj-prt":..lambd
+000124b0: 6120 646f 632c 2069 2c20 6a2c 206b 2c20  a doc, i, j, k, 
+000124c0: 7461 673a 2020 646f 632e 7573 6572 5f64  tag:  doc.user_d
+000124d0: 6174 612e 7570 6461 7465 287b 6622 646f  ata.update({f"do
+000124e0: 626a 2d70 7274 3a7b 646f 635b 695d 2e6c  bj-prt:{doc[i].l
+000124f0: 656d 6d61 5f7d 5f7b 646f 635b 6a5d 2e6c  emma_}_{doc[j].l
+00012500: 656d 6d61 5f7d 207b 646f 635b 6b5d 2e6c  emma_} {doc[k].l
+00012510: 656d 6d61 5f7d 5b7b 697d 2c7b 6a7d 2c7b  emma_}[{i},{j},{
+00012520: 6b7d 5d22 3a7b 2274 6167 223a 7461 672c  k}]":{"tag":tag,
+00012530: 2022 6672 6f6d 223a 2274 7270 3322 2c0a   "from":"trp3",.
+00012540: 0909 0909 0909 226e 6163 223a 5b66 227b  ......"nac":[f"{
+00012550: 646f 635b 695d 2e6c 656d 6d61 5f7d 5f7b  doc[i].lemma_}_{
+00012560: 646f 635b 6a5d 2e6c 656d 6d61 5f7d 3a7b  doc[j].lemma_}:{
+00012570: 646f 635b 695d 2e70 6f73 5f7d 3a64 6f62  doc[i].pos_}:dob
+00012580: 6a3a 7b64 6f63 5b6b 5d2e 706f 735f 7d7c  j:{doc[k].pos_}|
+00012590: 7b64 6f63 5b6b 5d2e 6c65 6d6d 615f 7d22  {doc[k].lemma_}"
+000125a0: 2c66 227b 646f 635b 6b5d 2e6c 656d 6d61  ,f"{doc[k].lemma
+000125b0: 5f7d 3a7b 646f 635b 6b5d 2e70 6f73 5f7d  _}:{doc[k].pos_}
+000125c0: 3a7e 646f 626a 3a7b 646f 635b 695d 2e70  :~dobj:{doc[i].p
+000125d0: 6f73 5f7d 7c7b 646f 635b 695d 2e6c 656d  os_}|{doc[i].lem
+000125e0: 6d61 5f7d 5f7b 646f 635b 6a5d 2e6c 656d  ma_}_{doc[j].lem
+000125f0: 6d61 5f7d 222c 6622 7b64 6f63 5b69 5d2e  ma_}",f"{doc[i].
+00012600: 6c65 6d6d 615f 7d5f 7b64 6f63 5b6a 5d2e  lemma_}_{doc[j].
+00012610: 6c65 6d6d 615f 7d3a 7b64 6f63 5b69 5d2e  lemma_}:{doc[i].
+00012620: 706f 735f 7d7c 646f 626a 3a7b 646f 635b  pos_}|dobj:{doc[
+00012630: 6b5d 2e70 6f73 5f7d 222c 6622 7b64 6f63  k].pos_}",f"{doc
+00012640: 5b6b 5d2e 6c65 6d6d 615f 7d3a 7b64 6f63  [k].lemma_}:{doc
+00012650: 5b6b 5d2e 706f 735f 7d7c 7e64 6f62 6a3a  [k].pos_}|~dobj:
+00012660: 7b64 6f63 5b69 5d2e 706f 735f 7d22 5d7d  {doc[i].pos_}"]}
+00012670: 7d29 2c20 0a09 2276 704e 223a 0909 096c  }), .."vpN":...l
+00012680: 616d 6264 6120 646f 632c 2069 2c20 6a2c  ambda doc, i, j,
+00012690: 206b 2c20 7461 673a 2020 646f 632e 7573   k, tag:  doc.us
+000126a0: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
+000126b0: 6622 7670 4e3a 7b64 6f63 5b69 5d2e 6c65  f"vpN:{doc[i].le
+000126c0: 6d6d 615f 7d20 7b64 6f63 5b6a 5d2e 7465  mma_} {doc[j].te
+000126d0: 7874 7d20 7b64 6f63 5b6b 5d2e 7465 7874  xt} {doc[k].text
+000126e0: 7d5b 7b69 7d2c 7b6a 7d2c 7b6b 7d5d 223a  }[{i},{j},{k}]":
+000126f0: 7b22 7461 6722 3a74 6167 2c20 2266 726f  {"tag":tag, "fro
+00012700: 6d22 3a22 7472 7033 222c 2023 206a 756d  m":"trp3", # jum
+00012710: 7020 6f76 6572 2074 6865 2064 6f67 202f  p over the dog /
+00012720: 2063 6f6d 6520 696e 746f 2066 6f72 6365   come into force
+00012730: 2f76 706e 200a 0909 0909 0909 226e 6163  /vpn ......."nac
+00012740: 223a 5b66 227b 646f 635b 695d 2e6c 656d  ":[f"{doc[i].lem
+00012750: 6d61 5f7d 3a7b 646f 635b 695d 2e70 6f73  ma_}:{doc[i].pos
+00012760: 5f7d 3a76 704e 7c7b 646f 635b 6b5d 2e6c  _}:vpN|{doc[k].l
+00012770: 656d 6d61 5f7d 222c 6622 7b64 6f63 5b69  emma_}",f"{doc[i
+00012780: 5d2e 6c65 6d6d 615f 7d3a 7b64 6f63 5b69  ].lemma_}:{doc[i
+00012790: 5d2e 706f 735f 7d7c 7670 4e22 2c66 227b  ].pos_}|vpN",f"{
+000127a0: 646f 635b 6b5d 2e6c 656d 6d61 5f7d 3a7b  doc[k].lemma_}:{
+000127b0: 646f 635b 6b5d 2e70 6f73 5f7d 3a76 704e  doc[k].pos_}:vpN
+000127c0: 7c7b 646f 635b 695d 2e6c 656d 6d61 5f7d  |{doc[i].lemma_}
+000127d0: 207b 646f 635b 6a5d 2e6c 656d 6d61 5f7d   {doc[j].lemma_}
+000127e0: 207b 646f 635b 6b5d 2e6c 656d 6d61 5f7d   {doc[k].lemma_}
+000127f0: 222c 6622 7b64 6f63 5b6b 5d2e 6c65 6d6d  ",f"{doc[k].lemm
+00012800: 615f 7d3a 7b64 6f63 5b6b 5d2e 706f 735f  a_}:{doc[k].pos_
+00012810: 7d7c 7670 4e22 5d7d 7d29 2c20 0a09 7d0a  }|vpN"]}}), ..}.
+00012820: 0a64 6566 206b 705f 626f 726e 2864 6f63  .def kp_born(doc
+00012830: 2c20 6261 7365 3a62 6f6f 6c3d 5472 7565  , base:bool=True
+00012840: 293a 0a09 2727 2720 626f 726e 206b 7020  ):..''' born kp 
+00012850: 746f 2075 7365 725f 6461 7461 202c 2020  to user_data ,  
+00012860: 4e4e 533a 6b6e 6f77 6c65 6467 6573 2c20  NNS:knowledges, 
+00012870: 206e 6265 3a66 6174 6520 7365 616c 6564   nbe:fate sealed
+00012880: 2c20 2027 2727 0a09 6672 6f6d 2064 6963  ,  '''..from dic
+00012890: 2e77 6f72 646c 6973 7420 696d 706f 7274  .wordlist import
+000128a0: 2077 6f72 646c 6973 7420 0a09 6966 2062   wordlist ..if b
+000128b0: 6173 653a 0a09 095b 2064 6f63 2e75 7365  ase:...[ doc.use
+000128c0: 725f 6461 7461 2e75 7064 6174 6528 7b66  r_data.update({f
+000128d0: 227b 742e 706f 735f 7d3a 7b74 2e6c 656d  "{t.pos_}:{t.lem
+000128e0: 6d61 5f7d 5b7b 742e 697d 5d22 3a20 7b22  ma_}[{t.i}]": {"
+000128f0: 7479 7065 223a 2274 6f6b 222c 200a 0909  type":"tok", ...
+00012900: 0909 226e 6163 223a 5b66 227b 742e 706f  .."nac":[f"{t.po
+00012910: 735f 7d7c 7b74 2e6c 656d 6d61 5f7d 222c  s_}|{t.lemma_}",
+00012920: 2066 227b 742e 6c65 6d6d 615f 7d7c 7b74   f"{t.lemma_}|{t
+00012930: 2e70 6f73 5f7d 222c 2066 222a 7c7b 742e  .pos_}", f"*|{t.
+00012940: 706f 735f 7d22 2c20 6622 7b74 2e6c 656d  pos_}", f"{t.lem
+00012950: 6d61 5f7d 3a7b 742e 706f 735f 7d7c 7b74  ma_}:{t.pos_}|{t
+00012960: 2e74 6167 5f7d 222c 6622 2a3a 7b74 2e70  .tag_}",f"*:{t.p
+00012970: 6f73 5f7d 7c7b 742e 7461 675f 7d22 2c20  os_}|{t.tag_}", 
+00012980: 6622 7b74 2e6c 656d 6d61 5f7d 3a7b 742e  f"{t.lemma_}:{t.
+00012990: 706f 735f 7d3a 7b74 2e74 6167 5f7d 7c7b  pos_}:{t.tag_}|{
+000129a0: 742e 7465 7874 2e6c 6f77 6572 2829 7d22  t.text.lower()}"
+000129b0: 5d7d 2c20 0a09 0909 6622 7b74 2e74 6167  ]}, ....f"{t.tag
+000129c0: 5f7d 3a7b 742e 7465 7874 2e6c 6f77 6572  _}:{t.text.lower
+000129d0: 2829 7d5b 7b74 2e69 7d5d 223a 207b 2274  ()}[{t.i}]": {"t
+000129e0: 7970 6522 3a22 746f 6b22 2c20 0a09 0909  ype":"tok", ....
+000129f0: 0922 6e61 6322 3a5b 6622 7b74 2e74 6167  ."nac":[f"{t.tag
+00012a00: 5f7d 7c7b 742e 7465 7874 2e6c 6f77 6572  _}|{t.text.lower
+00012a10: 2829 7d22 2c20 6622 2a7c 7b74 2e74 6167  ()}", f"*|{t.tag
+00012a20: 5f7d 225d 7d20 7d29 2066 6f72 2074 2069  _}"]} }) for t i
+00012a30: 6e20 646f 6320 6966 2074 2e70 6f73 5f20  n doc if t.pos_ 
+00012a40: 696e 2028 224e 4f55 4e22 2c22 5645 5242  in ("NOUN","VERB
+00012a50: 222c 2241 444a 222c 2241 4456 2229 2061  ","ADJ","ADV") a
+00012a60: 6e64 2074 2e69 735f 616c 7068 6120 5d0a  nd t.is_alpha ].
+00012a70: 0a09 095b 2064 6f63 2e75 7365 725f 6461  ...[ doc.user_da
+00012a80: 7461 2e75 7064 6174 6528 7b66 226e 6265  ta.update({f"nbe
+00012a90: 3a7b 742e 6c65 6d6d 615f 7d20 7b74 2e68  :{t.lemma_} {t.h
+00012aa0: 6561 642e 7465 7874 2e6c 6f77 6572 2829  ead.text.lower()
+00012ab0: 7d5b 7b74 2e68 6561 642e 697d 2c7b 742e  }[{t.head.i},{t.
+00012ac0: 697d 5d22 3a20 7b22 7479 7065 223a 2274  i}]": {"type":"t
+00012ad0: 7270 222c 0a09 0909 276e 6163 273a 5b66  rp",....'nac':[f
+00012ae0: 227b 742e 6c65 6d6d 615f 7d3a 7b74 2e70  "{t.lemma_}:{t.p
+00012af0: 6f73 5f7d 3a6e 6265 7c7b 742e 6865 6164  os_}:nbe|{t.head
+00012b00: 2e74 6578 742e 6c6f 7765 7228 297d 222c  .text.lower()}",
+00012b10: 2066 227b 742e 6c65 6d6d 615f 7d3a 7b74   f"{t.lemma_}:{t
+00012b20: 2e70 6f73 5f7d 7c6e 6265 222c 2066 222a  .pos_}|nbe", f"*
+00012b30: 3a7b 742e 706f 735f 7d7c 6e62 6522 2c20  :{t.pos_}|nbe", 
+00012b40: 2023 2053 6d6f 6b69 6e67 2069 7320 6261   # Smoking is ba
+00012b50: 6e6e 6564 2e20 2f56 4247 0a09 0909 0966  nned. /VBG.....f
+00012b60: 227b 742e 6865 6164 2e74 6578 742e 6c6f  "{t.head.text.lo
+00012b70: 7765 7228 297d 3a7b 742e 7461 675f 7d3a  wer()}:{t.tag_}:
+00012b80: 6e62 657c 7b74 2e6c 656d 6d61 5f7d 222c  nbe|{t.lemma_}",
+00012b90: 2066 227b 742e 6865 6164 2e74 6578 742e   f"{t.head.text.
+00012ba0: 6c6f 7765 7228 297d 3a7b 742e 7461 675f  lower()}:{t.tag_
+00012bb0: 7d7c 6e62 6522 2c20 6622 2a3a 7b74 2e74  }|nbe", f"*:{t.t
+00012bc0: 6167 5f7d 7c6e 6265 222c 5d20 7d20 7d29  ag_}|nbe",] } })
+00012bd0: 2066 6f72 2074 2069 6e20 646f 6320 6966   for t in doc if
+00012be0: 2074 2e64 6570 5f20 3d3d 2027 6e73 7562   t.dep_ == 'nsub
+00012bf0: 6a70 6173 7327 2061 6e64 2074 2e68 6561  jpass' and t.hea
+00012c00: 642e 7461 675f 203d 3d20 2756 424e 2720  d.tag_ == 'VBN' 
+00012c10: 5d20 2320 7468 6520 6661 7465 2069 7320  ] # the fate is 
+00012c20: 7365 616c 6564 2020 2f20 736d 696c 696e  sealed  / smilin
+00012c30: 6720 6973 2062 616e 6e65 6420 2e0a 0909  g is banned ....
+00012c40: 5b20 646f 632e 7573 6572 5f64 6174 612e  [ doc.user_data.
+00012c50: 7570 6461 7465 287b 6622 7663 3a7b 742e  update({f"vc:{t.
+00012c60: 6865 6164 2e6c 656d 6d61 5f7d 5b7b 742e  head.lemma_}[{t.
+00012c70: 6865 6164 2e69 7d2c 7b74 2e69 7d5d 223a  head.i},{t.i}]":
+00012c80: 207b 2274 7970 6522 3a22 7472 7022 2c20   {"type":"trp", 
+00012c90: 276e 6163 273a 5b66 227b 742e 6865 6164  'nac':[f"{t.head
+00012ca0: 2e6c 656d 6d61 5f7d 3a7b 742e 6865 6164  .lemma_}:{t.head
+00012cb0: 2e70 6f73 5f7d 7c76 6322 2c20 6622 2a3a  .pos_}|vc", f"*:
+00012cc0: 7b74 2e68 6561 642e 706f 735f 7d7c 7663  {t.head.pos_}|vc
+00012cd0: 222c 2066 227b 742e 6865 6164 2e6c 656d  ", f"{t.head.lem
+00012ce0: 6d61 5f7d 2f7b 742e 6865 6164 2e70 6f73  ma_}/{t.head.pos
+00012cf0: 5f7d 7c76 633a 5f7b 742e 6865 6164 2e6c  _}|vc:_{t.head.l
+00012d00: 656d 6d61 5f7d 205f 434c 6363 6f6d 7022  emma_} _CLccomp"
+00012d10: 2c5d 207d 207d 2920 666f 7220 7420 696e  ,] } }) for t in
+00012d20: 2064 6f63 2069 6620 742e 6465 705f 203d   doc if t.dep_ =
+00012d30: 3d20 2763 636f 6d70 2720 616e 6420 742e  = 'ccomp' and t.
+00012d40: 6865 6164 2e70 6f73 5f20 3d3d 2027 5645  head.pos_ == 'VE
+00012d50: 5242 2720 5d0a 0909 5b20 646f 632e 7573  RB' ]...[ doc.us
+00012d60: 6572 5f64 6174 612e 7570 6461 7465 287b  er_data.update({
+00012d70: 6622 524f 4f54 2d7b 742e 7461 675f 7d3a  f"ROOT-{t.tag_}:
+00012d80: 7b74 2e6c 656d 6d61 5f7d 5b7b 742e 697d  {t.lemma_}[{t.i}
+00012d90: 5d22 3a20 7b22 7479 7065 223a 2274 7270  ]": {"type":"trp
+00012da0: 222c 226e 6163 223a 5b66 227b 742e 6c65  ","nac":[f"{t.le
+00012db0: 6d6d 615f 7d3a 7b74 2e70 6f73 5f7d 7c52  mma_}:{t.pos_}|R
+00012dc0: 4f4f 5422 5d7d 207d 2920 666f 7220 7420  OOT"]} }) for t 
+00012dd0: 696e 2064 6f63 2069 6620 742e 6465 705f  in doc if t.dep_
+00012de0: 203d 3d20 2752 4f4f 5427 205d 0a09 095b   == 'ROOT' ]...[
+00012df0: 2064 6f63 2e75 7365 725f 6461 7461 2e75   doc.user_data.u
+00012e00: 7064 6174 6528 7b66 2278 636f 6d70 2d7b  pdate({f"xcomp-{
+00012e10: 742e 6865 6164 2e70 6f73 5f7d 2d7b 742e  t.head.pos_}-{t.
+00012e20: 7461 675f 7d3a 7b74 2e68 6561 642e 6c65  tag_}:{t.head.le
+00012e30: 6d6d 615f 7d20 7b74 2e74 6578 747d 5b7b  mma_} {t.text}[{
+00012e40: 742e 6865 6164 2e69 7d2c 7b74 2e69 7d5d  t.head.i},{t.i}]
+00012e50: 223a 207b 2274 7970 6522 3a22 7472 7022  ": {"type":"trp"
+00012e60: 2c20 0a09 0909 226e 6163 223a 5b66 227b  , ...."nac":[f"{
+00012e70: 742e 6865 6164 2e6c 656d 6d61 5f7d 3a7b  t.head.lemma_}:{
+00012e80: 742e 6865 6164 2e70 6f73 5f7d 7c78 636f  t.head.pos_}|xco
+00012e90: 6d70 3a7b 742e 7461 675f 7d22 2c20 6622  mp:{t.tag_}", f"
+00012ea0: 7b74 2e68 6561 642e 6c65 6d6d 615f 7d3a  {t.head.lemma_}:
+00012eb0: 7b74 2e68 6561 642e 706f 735f 7d3a 7863  {t.head.pos_}:xc
+00012ec0: 6f6d 703a 7b74 2e74 6167 5f7d 7c7b 742e  omp:{t.tag_}|{t.
+00012ed0: 7465 7874 2e6c 6f77 6572 2829 7d22 2c0a  text.lower()}",.
+00012ee0: 0909 0909 2020 2066 227b 742e 6c65 6d6d  ....   f"{t.lemm
+00012ef0: 615f 7d3a 7b74 2e74 6167 5f7d 7c7e 7863  a_}:{t.tag_}|~xc
+00012f00: 6f6d 703a 7b74 2e68 6561 642e 706f 735f  omp:{t.head.pos_
+00012f10: 7d22 2c20 6622 7b74 2e6c 656d 6d61 5f7d  }", f"{t.lemma_}
+00012f20: 3a7b 742e 7461 675f 7d3a 7e78 636f 6d70  :{t.tag_}:~xcomp
+00012f30: 3a7b 742e 6865 6164 2e70 6f73 5f7d 7c7b  :{t.head.pos_}|{
+00012f40: 742e 6865 6164 2e6c 656d 6d61 5f7d 222c  t.head.lemma_}",
+00012f50: 200a 0909 0920 2020 2020 2020 6622 7b74   ....       f"{t
+00012f60: 2e6c 656d 6d61 5f7d 3a7b 742e 706f 735f  .lemma_}:{t.pos_
+00012f70: 7d7c 7e78 636f 6d70 3a7b 742e 6865 6164  }|~xcomp:{t.head
+00012f80: 2e70 6f73 5f7d 222c 2066 227b 742e 6c65  .pos_}", f"{t.le
+00012f90: 6d6d 615f 7d3a 7b74 2e70 6f73 5f7d 3a7e  mma_}:{t.pos_}:~
+00012fa0: 7863 6f6d 703a 7b74 2e68 6561 642e 706f  xcomp:{t.head.po
+00012fb0: 735f 7d7c 7b74 2e68 6561 642e 6c65 6d6d  s_}|{t.head.lemm
+00012fc0: 615f 7d22 2c20 2320 6164 6465 6420 3230  a_}", # added 20
+00012fd0: 332e 322e 3236 0a09 0909 0920 2020 6622  3.2.26.....   f"
+00012fe0: 2a3a 7b74 2e68 6561 642e 706f 735f 7d7c  *:{t.head.pos_}|
+00012ff0: 7863 6f6d 703a 7b74 2e74 6167 5f7d 222c  xcomp:{t.tag_}",
+00013000: 2066 222a 3a7b 742e 706f 735f 7d7c 7e78   f"*:{t.pos_}|~x
+00013010: 636f 6d70 3a7b 742e 6865 6164 2e70 6f73  comp:{t.head.pos
+00013020: 5f7d 222c 5d20 7d20 7d29 200a 0909 0966  _}",] } }) ....f
+00013030: 6f72 2074 2069 6e20 646f 6320 6966 2074  or t in doc if t
+00013040: 2e64 6570 5f20 3d3d 2027 7863 6f6d 7027  .dep_ == 'xcomp'
+00013050: 2061 6e64 2074 2e70 6f73 5f20 3d3d 2027   and t.pos_ == '
+00013060: 5645 5242 2720 5d0a 0909 5b20 646f 632e  VERB' ]...[ doc.
+00013070: 7573 6572 5f64 6174 612e 7570 6461 7465  user_data.update
+00013080: 287b 6622 4e50 3a7b 7370 2e74 6578 742e  ({f"NP:{sp.text.
+00013090: 6c6f 7765 7228 297d 5b7b 7370 2e73 7461  lower()}[{sp.sta
+000130a0: 7274 7d2c 7b73 702e 656e 647d 2922 3a20  rt},{sp.end})": 
+000130b0: 7b22 7479 7065 223a 2263 6875 6e6b 222c  {"type":"chunk",
+000130c0: 200a 0909 0922 6e61 6322 3a5b 6622 7b64   ...."nac":[f"{d
+000130d0: 6f63 5b73 702e 656e 642d 315d 2e6c 656d  oc[sp.end-1].lem
+000130e0: 6d61 5f7d 3a7b 646f 635b 7370 2e65 6e64  ma_}:{doc[sp.end
+000130f0: 2d31 5d2e 706f 735f 7d3a 4e50 7c7b 7370  -1].pos_}:NP|{sp
+00013100: 2e74 6578 742e 6c6f 7765 7228 297d 222c  .text.lower()}",
+00013110: 2066 227b 646f 635b 7370 2e65 6e64 2d31   f"{doc[sp.end-1
+00013120: 5d2e 6c65 6d6d 615f 7d3a 7b64 6f63 5b73  ].lemma_}:{doc[s
+00013130: 702e 656e 642d 315d 2e70 6f73 5f7d 7c4e  p.end-1].pos_}|N
+00013140: 5022 0a09 0909 2c20 6622 2a3a 7b64 6f63  P"...., f"*:{doc
+00013150: 5b73 702e 656e 642d 315d 2e70 6f73 5f7d  [sp.end-1].pos_}
+00013160: 7c4e 5022 5d20 7d7d 2020 2920 0a09 0909  |NP"] }}  ) ....
+00013170: 666f 7220 7370 2069 6e20 646f 632e 6e6f  for sp in doc.no
+00013180: 756e 5f63 6875 6e6b 735d 2023 4e50 3a61  un_chunks] #NP:a
+00013190: 2062 6f6f 6b0a 0a09 0923 2061 6464 2074   book....# add t
+000131a0: 7269 706c 6520 6b70 3a20 646f 626a 2d56  riple kp: dobj-V
+000131b0: 4552 422d 4e4f 554e 3a6f 7065 6e20 646f  ERB-NOUN:open do
+000131c0: 6f72 0a09 095b 2064 6f63 2e75 7365 725f  or...[ doc.user_
+000131d0: 6461 7461 2e75 7064 6174 6528 7b66 227b  data.update({f"{
+000131e0: 742e 6465 705f 7d2d 7b74 2e68 6561 642e  t.dep_}-{t.head.
+000131f0: 706f 735f 7d2d 7b74 2e70 6f73 5f7d 3a7b  pos_}-{t.pos_}:{
+00013200: 742e 6865 6164 2e6c 656d 6d61 5f7d 207b  t.head.lemma_} {
+00013210: 742e 6c65 6d6d 615f 7d5b 7b74 2e68 6561  t.lemma_}[{t.hea
+00013220: 642e 697d 2c7b 742e 697d 5d22 3a20 7b22  d.i},{t.i}]": {"
+00013230: 7479 7065 223a 2274 7270 222c 0a09 0909  type":"trp",....
+00013240: 226e 6163 223a 5b66 227b 742e 6865 6164  "nac":[f"{t.head
+00013250: 2e6c 656d 6d61 5f7d 3a7b 742e 6865 6164  .lemma_}:{t.head
+00013260: 2e70 6f73 5f7d 3a7b 742e 6465 705f 7d7c  .pos_}:{t.dep_}|
+00013270: 7b74 2e70 6f73 5f7d 222c 6622 7b74 2e68  {t.pos_}",f"{t.h
+00013280: 6561 642e 6c65 6d6d 615f 7d3a 7b74 2e68  ead.lemma_}:{t.h
+00013290: 6561 642e 706f 735f 7d7c 7b74 2e64 6570  ead.pos_}|{t.dep
+000132a0: 5f7d 3a7b 742e 706f 735f 7d22 2c20 6622  _}:{t.pos_}", f"
+000132b0: 7b74 2e68 6561 642e 6c65 6d6d 615f 7d3a  {t.head.lemma_}:
+000132c0: 7b74 2e68 6561 642e 706f 735f 7d3a 7b74  {t.head.pos_}:{t
+000132d0: 2e64 6570 5f7d 3a7b 742e 706f 735f 7d7c  .dep_}:{t.pos_}|
+000132e0: 7b74 2e6c 656d 6d61 5f7d 222c 0a09 0909  {t.lemma_}",....
+000132f0: 0920 2020 6622 7b74 2e6c 656d 6d61 5f7d  .   f"{t.lemma_}
+00013300: 3a7b 742e 706f 735f 7d3a 7e7b 742e 6465  :{t.pos_}:~{t.de
+00013310: 705f 7d7c 7b74 2e68 6561 642e 706f 735f  p_}|{t.head.pos_
+00013320: 7d22 2c20 6622 7b74 2e6c 656d 6d61 5f7d  }", f"{t.lemma_}
+00013330: 3a7b 742e 706f 735f 7d7c 7e7b 742e 6465  :{t.pos_}|~{t.de
+00013340: 705f 7d3a 7b74 2e68 6561 642e 706f 735f  p_}:{t.head.pos_
+00013350: 7d22 2c20 6622 7b74 2e6c 656d 6d61 5f7d  }", f"{t.lemma_}
+00013360: 3a7b 742e 706f 735f 7d3a 7e7b 742e 6465  :{t.pos_}:~{t.de
+00013370: 705f 7d3a 7b74 2e68 6561 642e 706f 735f  p_}:{t.head.pos_
+00013380: 7d7c 7b74 2e68 6561 642e 6c65 6d6d 615f  }|{t.head.lemma_
+00013390: 7d22 2c0a 0909 0909 2020 2066 222a 3a7b  }",.....   f"*:{
+000133a0: 742e 6865 6164 2e70 6f73 5f7d 7c7b 742e  t.head.pos_}|{t.
+000133b0: 6465 705f 7d22 2c66 222a 3a7b 742e 706f  dep_}",f"*:{t.po
+000133c0: 735f 7d7c 7e7b 742e 6465 705f 7d22 2c0a  s_}|~{t.dep_}",.
+000133d0: 0909 095d 207d 207d 2920 0a09 0909 666f  ...] } }) ....fo
+000133e0: 7220 7420 696e 2064 6f63 2069 6620 742e  r t in doc if t.
+000133f0: 706f 735f 2069 6e20 2822 4e4f 554e 222c  pos_ in ("NOUN",
+00013400: 2256 4552 4222 2c22 4144 4a22 2c22 4144  "VERB","ADJ","AD
+00013410: 5622 2c22 4144 5022 2920 616e 6420 742e  V","ADP") and t.
+00013420: 6465 705f 206e 6f74 2069 6e20 2827 524f  dep_ not in ('RO
+00013430: 4f54 272c 2770 756e 6374 272c 2778 636f  OT','punct','xco
+00013440: 6d70 2729 2061 6e64 2074 2e69 735f 616c  mp') and t.is_al
+00013450: 7068 6120 616e 6420 742e 6865 6164 2e69  pha and t.head.i
+00013460: 735f 616c 7068 6120 616e 6420 742e 6c65  s_alpha and t.le
+00013470: 6d6d 615f 2069 6e20 776f 7264 6c69 7374  mma_ in wordlist
+00013480: 2020 616e 6420 742e 6865 6164 2e6c 656d    and t.head.lem
+00013490: 6d61 5f20 696e 2077 6f72 646c 6973 745d  ma_ in wordlist]
+000134a0: 0a0a 0970 6f73 7461 675f 6d61 7463 6828  ...postag_match(
+000134b0: 646f 632c 2070 6f73 7461 675f 6675 6e63  doc, postag_func
+000134c0: 5f6b 7029 200a 0974 7270 335f 6d61 7463  _kp) ..trp3_matc
+000134d0: 6828 646f 632c 2074 7270 335f 6675 6e63  h(doc, trp3_func
+000134e0: 5f6b 7029 0a09 6d65 7267 655f 6e70 2864  _kp)..merge_np(d
+000134f0: 6f63 2920 200a 0973 6b65 6e70 5f6d 6174  oc)  ..skenp_mat
+00013500: 6368 2864 6f63 2c20 736b 656e 705f 6675  ch(doc, skenp_fu
+00013510: 6e63 5f6b 7029 2020 236f 6e5f 7370 616e  nc_kp)  #on_span
+00013520: 2864 6f63 2c20 736b 656e 705f 6675 6e63  (doc, skenp_func
+00013530: 2c20 2773 6b65 6e70 5b27 290a 0972 6574  , 'skenp[')..ret
+00013540: 7572 6e20 646f 632e 7573 6572 5f64 6174  urn doc.user_dat
+00013550: 610a 0a5b 7365 7461 7474 7228 6275 696c  a..[setattr(buil
+00013560: 7469 6e73 2c20 6b2c 2076 2920 666f 7220  tins, k, v) for 
+00013570: 6b2c 2076 2069 6e20 676c 6f62 616c 7328  k, v in globals(
+00013580: 292e 6974 656d 7328 2920 6966 206e 6f74  ).items() if not
+00013590: 206b 2e73 7461 7274 7377 6974 6828 225f   k.startswith("_
+000135a0: 2229 2061 6e64 206e 6f74 2027 2e27 2069  ") and not '.' i
+000135b0: 6e20 6b20 616e 6420 6e6f 7420 6861 7361  n k and not hasa
+000135c0: 7474 7228 6275 696c 7469 6e73 2c6b 2920  ttr(builtins,k) 
+000135d0: 5d20 2373 6574 6174 7472 2862 7569 6c74  ] #setattr(built
+000135e0: 696e 732c 2022 7370 6163 7922 2c20 7370  ins, "spacy", sp
+000135f0: 6163 7929 0a69 6620 5f5f 6e61 6d65 5f5f  acy).if __name__
+00013600: 093d 3d20 275f 5f6d 6169 6e5f 5f27 3a20  .== '__main__': 
+00013610: 0a09 696d 706f 7274 2066 6972 652c 2070  ..import fire, p
+00013620: 6c61 7466 6f72 6d0a 095b 2070 7269 6e74  latform..[ print
+00013630: 2028 206b 702c 2069 7465 6d29 2066 6f72   ( kp, item) for
+00013640: 206b 702c 2069 7465 6d20 696e 206b 705f   kp, item in kp_
+00013650: 626f 726e 2873 7061 6379 2e6e 6c70 2822  born(spacy.nlp("
+00013660: 4920 7461 6b65 2069 7420 696e 746f 2061  I take it into a
+00013670: 6363 6f75 6e74 2c20 616e 6420 4920 656e  ccount, and I en
+00013680: 6a6f 7920 7377 696d 6d69 6e67 2e22 2929  joy swimming."))
+00013690: 2e69 7465 6d73 2829 5d20 2069 6620 706c  .items()]  if pl
+000136a0: 6174 666f 726d 2e73 7973 7465 6d28 2920  atform.system() 
+000136b0: 696e 2028 2757 696e 646f 7773 2729 2065  in ('Windows') e
+000136c0: 6c73 6520 6669 7265 2e46 6972 6528 7b22  lse fire.Fire({"
+000136d0: 7371 6c73 6922 3a73 716c 7369 2c20 2274  sqlsi":sqlsi, "t
+000136e0: 6573 7422 3a74 6573 742c 2022 6573 5f73  est":test, "es_s
+000136f0: 7562 6d69 7422 3a65 735f 7375 626d 6974  ubmit":es_submit
+00013700: 2c20 2266 6173 7474 6578 7422 3a66 6173  , "fasttext":fas
+00013710: 7474 6578 7420 7d29 0a0a 2370 7269 6e74  ttext })..#print
+00013720: 2873 6e74 6272 2822 5b5c 7538 6264 315c  (sntbr("[\u8bd1\
+00013730: 7536 3538 375d 5468 6520 3535 2d6b 696c  u6587]The 55-kil
+00013740: 6f6d 6574 7265 2048 6f6e 6720 4b6f 6e67  ometre Hong Kong
+00013750: 205a 6875 6861 692d 4d61 6361 7520 4272   Zhuhai-Macau Br
+00013760: 6964 6765 2069 7320 616e 2065 7874 7261  idge is an extra
+00013770: 6f72 6469 6e61 7279 2065 6e67 696e 6565  ordinary enginee
+00013780: 7269 6e67 2e20 4974 2069 7320 7468 6520  ring. It is the 
+00013790: 776f 726c 6427 7320 6c6f 6e67 6573 7420  world's longest 
+000137a0: 7365 612d 6372 6f73 7369 6e67 2074 7261  sea-crossing tra
+000137b0: 6e73 706f 7274 6174 696f 6e20 7379 7374  nsportation syst
+000137c0: 656d 2063 6f6d 6269 6e69 6e67 2062 7269  em combining bri
+000137d0: 6467 6573 2061 6e64 2074 756e 6e65 6c73  dges and tunnels
+000137e0: 2c20 7768 6963 6820 6a6f 696e 7320 7468  , which joins th
+000137f0: 6520 7468 7265 6520 6369 7469 6573 206f  e three cities o
+00013800: 6620 486f 6e67 204b 6f6e 6720 5a68 7568  f Hong Kong Zhuh
+00013810: 6169 2061 6e64 204d 6163 616f 2c20 6375  ai and Macao, cu
+00013820: 7474 696e 6720 7468 6520 7472 6176 656c  tting the travel
+00013830: 6c69 6e67 2074 696d 6520 616d 6f6e 6720  ling time among 
+00013840: 7468 656d 2066 726f 6d20 3320 686f 7572  them from 3 hour
+00013850: 7320 746f 2033 3020 6d69 6e75 7465 732e  s to 30 minutes.
+00013860: 2054 6865 2072 6569 6e66 6f72 6365 6420   The reinforced 
+00013870: 636f 6e63 7265 7465 2062 7269 6467 6520  concrete bridge 
+00013880: 7769 7468 2068 7567 6520 7370 616e 7320  with huge spans 
+00013890: 6675 6c6c 7920 6e6f 7420 6f6e 6c79 2070  fully not only p
+000138a0: 726f 7665 7320 7468 6174 2043 6869 6e61  roves that China
+000138b0: 2068 6173 2074 6865 2061 6269 6c69 7479   has the ability
+000138c0: 2074 6f20 636f 6d70 6c65 7465 2074 6865   to complete the
+000138d0: 2072 6563 6f72 642d 6272 6561 6b69 6e67   record-breaking
+000138e0: 206d 6567 612d 636f 6e73 7472 7563 7469   mega-constructi
+000138f0: 6f6e 2c20 6275 7420 616c 736f 2077 696c  on, but also wil
+00013900: 6c20 656e 6861 6e63 6520 7468 6520 7265  l enhance the re
+00013910: 6769 6f6e 616c 2069 6e74 6567 7261 7469  gional integrati
+00013920: 6f6e 2061 6e64 2062 6f6f 7374 2074 6865  on and boost the
+00013930: 2065 636f 6e6f 6d69 6320 6772 6f77 7468   economic growth
+00013940: 2e20 4974 2070 6c61 7973 2061 2063 7275  . It plays a cru
+00013950: 6369 616c 2072 6f6c 6520 696e 2074 6865  cial role in the
+00013960: 206f 7665 7261 6c6c 2070 6c61 6e20 746f   overall plan to
+00013970: 2064 6576 656c 6f70 2043 6869 6e61 e280   develop China..
+00013980: 9973 2047 7265 6174 2042 6179 2041 7265  .s Great Bay Are
+00013990: 612c 2077 6869 6368 2043 6869 6e61 2069  a, which China i
+000139a0: 6e74 656e 6473 2074 6f20 7475 726e 2069  ntends to turn i
+000139b0: 6e74 6f20 6f6e 6520 7269 7661 6c69 6e67  nto one rivaling
+000139c0: 2074 686f 7365 206f 6620 5361 6e20 4672   those of San Fr
+000139d0: 616e 6369 7363 6f2c 204e 6577 2059 6f72  ancisco, New Yor
+000139e0: 6b20 616e 6420 546f 6b79 6f20 696e 2074  k and Tokyo in t
+000139f0: 6572 6d73 206f 6620 7465 6368 6e6f 6c6f  erms of technolo
+00013a00: 6769 6361 6c20 696e 6e6f 7661 7469 6f6e  gical innovation
+00013a10: 2061 6e64 2065 636f 6e6f 6d69 6320 7072   and economic pr
+00013a20: 6f73 7065 7269 7479 2e22 2c20 7769 7468  osperity.", with
+00013a30: 5f70 6964 3d54 7275 6529 290a 2363 3a5c  _pid=True)).#c:\
+00013a40: 7573 6572 735c 7a68 616e 675c 6170 7064  users\zhang\appd
+00013a50: 6174 615c 6c6f 6361 6c5c 7072 6f67 7261  ata\local\progra
+00013a60: 6d73 5c70 7974 686f 6e5c 7079 7468 6f6e  ms\python\python
+00013a70: 3338 5c6c 6962 5c73 6974 652d 7061 636b  38\lib\site-pack
+00013a80: 6167 6573 2020 0a23 2f68 6f6d 652f 7562  ages  .#/home/ub
+00013a90: 756e 7475 2f2e 6c6f 6361 6c2f 6c69 622f  untu/.local/lib/
+00013aa0: 7079 7468 6f6e 332e 382f 7369 7465 2d70  python3.8/site-p
+00013ab0: 6163 6b61 6765 732f 656e 0a27 2727 0a3e  ackages/en.'''.>
+00013ac0: 3e3e 206d 6f64 656c 2827 6c67 2729 2e76  >> model('lg').v
+00013ad0: 6f63 6162 0a3c 7370 6163 792e 766f 6361  ocab.<spacy.voca
+00013ae0: 622e 566f 6361 6220 6f62 6a65 6374 2061  b.Vocab object a
+00013af0: 7420 3078 3030 3030 3031 3334 3539 3135  t 0x000001345915
+00013b00: 3441 3630 3e0a 3e3e 3e20 6c65 6e28 6d6f  4A60>.>>> len(mo
+00013b10: 6465 6c28 276c 6727 292e 766f 6361 6229  del('lg').vocab)
+00013b20: 0a37 3638 0a3e 3e3e 206c 656e 286d 6f64  .768.>>> len(mod
+00013b30: 656c 2827 736d 2729 2e76 6f63 6162 290a  el('sm').vocab).
+00013b40: 3736 370a 2727 27                        767.'''
```

### Comparing `cikuu-2022.8.8/en/__main__.py` & `cikuu-2022.8.9/en/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/annotate.py` & `cikuu-2022.8.9/en/annotate.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/arc/__init__.py` & `cikuu-2022.8.9/en/arc/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/arc/sntjson-innodb.py` & `cikuu-2022.8.9/en/arc/sntjson-innodb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/arc/sntjson-naclite.py` & `cikuu-2022.8.9/en/arc/sntjson-naclite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/arc/sntjson-naclite0.py` & `cikuu-2022.8.9/en/arc/sntjson-naclite0.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/arc/sntjson-nacp-20230206.py` & `cikuu-2022.8.9/en/arc/sntjson-nacp-20230206.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/arc/sntjson-nacp-20230207.py` & `cikuu-2022.8.9/en/arc/sntjson-nacp-20230207.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4-cl.py` & `cikuu-2022.8.9/en/c4-cl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4-fts.py` & `cikuu-2022.8.9/en/c4-fts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4-gram-upload.py` & `cikuu-2022.8.9/en/c4-gram-upload.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4-gram.py` & `cikuu-2022.8.9/en/c4-gram.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4-grams.py` & `cikuu-2022.8.9/en/c4-grams.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4-np.py` & `cikuu-2022.8.9/en/c4-np.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4-trp.py` & `cikuu-2022.8.9/en/c4-trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4cl.py` & `cikuu-2022.8.9/en/c4cl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4gram-mysql.py` & `cikuu-2022.8.9/en/c4gram-mysql.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4gram-upsert.py` & `cikuu-2022.8.9/en/c4gram-upsert.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4gram.py` & `cikuu-2022.8.9/en/c4gram.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4gramcl.py` & `cikuu-2022.8.9/en/c4gramcl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4matcher.py` & `cikuu-2022.8.9/en/c4matcher.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4np.py` & `cikuu-2022.8.9/en/c4np.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4postag.py` & `cikuu-2022.8.9/en/c4postag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4skenp.py` & `cikuu-2022.8.9/en/c4skenp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4tree.py` & `cikuu-2022.8.9/en/c4tree.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4trp.py` & `cikuu-2022.8.9/en/c4trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/c4vp.py` & `cikuu-2022.8.9/en/c4vp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/clause.py` & `cikuu-2022.8.9/en/clause.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/dims.py` & `cikuu-2022.8.9/en/dims.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/docfts.py` & `cikuu-2022.8.9/en/docfts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/docjson.py` & `cikuu-2022.8.9/en/docjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/es-index.py` & `cikuu-2022.8.9/en/es-index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/esbulk.py` & `cikuu-2022.8.9/en/esbulk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/esfile.py` & `cikuu-2022.8.9/en/esfile.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/esjson.py` & `cikuu-2022.8.9/en/esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/exchunk.py` & `cikuu-2022.8.9/en/exchunk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/exphrase.py` & `cikuu-2022.8.9/en/exphrase.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/extrp.py` & `cikuu-2022.8.9/en/extrp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/havc.py` & `cikuu-2022.8.9/en/havc.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/kpsi.py` & `cikuu-2022.8.9/en/kpsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/lempostag.py` & `cikuu-2022.8.9/en/lempostag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/nacp-kvr.py` & `cikuu-2022.8.9/en/nacp-kvr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/nacp.py` & `cikuu-2022.8.9/en/nacp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/nlp-lit.py` & `cikuu-2022.8.9/en/nlp-lit.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/nlp-lmdb.py` & `cikuu-2022.8.9/en/nlp-lmdb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/postag.py` & `cikuu-2022.8.9/en/postag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/shav.py` & `cikuu-2022.8.9/en/shav.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/silite.py` & `cikuu-2022.8.9/en/silite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/snt-esjson.py` & `cikuu-2022.8.9/en/snt-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/snt-spacy.py` & `cikuu-2022.8.9/en/snt-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-fts.py` & `cikuu-2022.8.9/en/sntjson-fts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-kpsnt.py` & `cikuu-2022.8.9/en/sntjson-kpsnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-mysql.py` & `cikuu-2022.8.9/en/sntjson-mysql.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-nacp.py` & `cikuu-2022.8.9/en/sntjson-nacp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-parse-snt.py` & `cikuu-2022.8.9/en/sntjson-parse-snt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-si.py` & `cikuu-2022.8.9/en/sntjson-si.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-spacy.py` & `cikuu-2022.8.9/en/sntjson-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-topk.py` & `cikuu-2022.8.9/en/sntjson-topk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-tosnt.py` & `cikuu-2022.8.9/en/sntjson-tosnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-trpx.py` & `cikuu-2022.8.9/en/sntjson-trpx.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sntjson-vp.py` & `cikuu-2022.8.9/en/sntjson-vp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/spacybs-esjson.py` & `cikuu-2022.8.9/en/spacybs-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/spacybs.py` & `cikuu-2022.8.9/en/spacybs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/spider-esjson.py` & `cikuu-2022.8.9/en/spider-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/sqlsi.py` & `cikuu-2022.8.9/en/sqlsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/terms.py` & `cikuu-2022.8.9/en/terms.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/verbnet.py` & `cikuu-2022.8.9/en/verbnet.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/xsnt.py` & `cikuu-2022.8.9/en/xsnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/en/zset-load.py` & `cikuu-2022.8.9/en/zset-load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/gecdsk/__init__.py` & `cikuu-2022.8.9/gecdsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/gecdsk/essays.py` & `cikuu-2022.8.9/gecdsk/essays.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/gecdsk/paravs.py` & `cikuu-2022.8.9/gecdsk/paravs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/__init__.py` & `cikuu-2022.8.9/lit/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/common.py` & `cikuu-2022.8.9/lit/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/es/__init__.py` & `cikuu-2022.8.9/lit/es/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/es/index.py` & `cikuu-2022.8.9/lit/es/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/essay.py` & `cikuu-2022.8.9/lit/essay.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/fillmul.py` & `cikuu-2022.8.9/lit/fillmul.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/hello-pages.py` & `cikuu-2022.8.9/lit/hello-pages.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/index.py` & `cikuu-2022.8.9/lit/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/mock-scoring.py` & `cikuu-2022.8.9/lit/mock-scoring.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/penly/index.py` & `cikuu-2022.8.9/lit/penly/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/penly-resend.py` & `cikuu-2022.8.9/lit/penly-resend.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/redis-dump.py` & `cikuu-2022.8.9/lit/redis-dump.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/reorder.py` & `cikuu-2022.8.9/lit/reorder.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/restore.py` & `cikuu-2022.8.9/lit/restore.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/scoring.py` & `cikuu-2022.8.9/lit/scoring.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/single.py` & `cikuu-2022.8.9/lit/single.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/sntspolish.py` & `cikuu-2022.8.9/lit/sntspolish.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/sntupgrade.py` & `cikuu-2022.8.9/lit/sntupgrade.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/student-input.py` & `cikuu-2022.8.9/lit/student-input.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/teacher-admin.py` & `cikuu-2022.8.9/lit/teacher-admin.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/YULK.py` & `cikuu-2022.8.9/lit/yulk/YULK.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/common.py` & `cikuu-2022.8.9/lit/yulk/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/bipos.py` & `cikuu-2022.8.9/lit/yulk/func/bipos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/cola.py` & `cikuu-2022.8.9/lit/yulk/func/cola.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/common.py` & `cikuu-2022.8.9/lit/yulk/func/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/corpuslist.py` & `cikuu-2022.8.9/lit/yulk/func/corpuslist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/es.py` & `cikuu-2022.8.9/lit/yulk/func/es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/given-expect.py` & `cikuu-2022.8.9/lit/yulk/func/given-expect.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/gramx-single.py` & `cikuu-2022.8.9/lit/yulk/func/gramx-single.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/lemma.py` & `cikuu-2022.8.9/lit/yulk/func/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/lemvs.py` & `cikuu-2022.8.9/lit/yulk/func/lemvs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/pos.py` & `cikuu-2022.8.9/lit/yulk/func/pos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/posvs.py` & `cikuu-2022.8.9/lit/yulk/func/posvs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/style-in-mul.py` & `cikuu-2022.8.9/lit/yulk/func/style-in-mul.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/func/wordrank.py` & `cikuu-2022.8.9/lit/yulk/func/wordrank.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/index.py` & `cikuu-2022.8.9/lit/yulk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/lit/yulk/lemma.py` & `cikuu-2022.8.9/lit/yulk/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/pipe/__init__.py` & `cikuu-2022.8.9/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/pipe/__main__.py` & `cikuu-2022.8.9/pipe/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/pipe/redisgec8180.py` & `cikuu-2022.8.9/pipe/redisgec8180.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/pipe/xgecv1.py` & `cikuu-2022.8.9/pipe/xgecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/rabbitmq/__init__.py` & `cikuu-2022.8.9/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/redisr/__init__.py` & `cikuu-2022.8.9/redisr/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/redisr/glove-get.py` & `cikuu-2022.8.9/redisr/glove-get.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/redisr/glove.py` & `cikuu-2022.8.9/redisr/glove.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/redisr/sntvec-get.py` & `cikuu-2022.8.9/redisr/sntvec-get.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/sbert/__main__.py` & `cikuu-2022.8.9/sbert/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/sbert/hello.py` & `cikuu-2022.8.9/sbert/hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/sbert/redis-sntvec.py` & `cikuu-2022.8.9/sbert/redis-sntvec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/sbert/sntvec-so.py` & `cikuu-2022.8.9/sbert/sntvec-so.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/sbert/sntvec.py` & `cikuu-2022.8.9/sbert/sntvec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/setup.py` & `cikuu-2022.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time: 2022-2-13
 #############################################
  
 from setuptools import setup, find_packages
  
 setup(
   name = "cikuu",
-  version = "2022.8.8",
+  version = "2022.8.9",
   keywords = ("pip"),
   description = "cikuu tools",
   long_description = "add replace into soinit",
   license = "MIT Licence",
  
   url = "http://www.cikuu.com",
   author = "cikuu",
```

### Comparing `cikuu-2022.8.8/so/__init__.py` & `cikuu-2022.8.9/so/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 			"vp": { "type": "keyword"},
 			"ap": { "type": "keyword"},
 			"dp": { "type": "keyword"},
 			"kp": { "type": "keyword"},
 			"trp": { "type": "keyword"}, # open:VERB:dobj:NOUN:door
 			"cate": { "type": "keyword"},
 			"tail":{ "type": "keyword"},
-			"govpos":{ "type": "keyword"},
+			"govpos":{ "type": "keyword"}, "govlem":{ "type": "keyword"}, "govtag":{ "type": "keyword"},
 			"deppos":{ "type": "keyword"},
 			#"fd": { "type": "keyword"},
 			"si": {
 				   "type": "nested",
 				   "properties": {
 					  "s": {"type": "keyword"},
 					  "i": {"type": "integer"}
```

### Comparing `cikuu-2022.8.8/so/__main__.py` & `cikuu-2022.8.9/so/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/batch-dis.py` & `cikuu-2022.8.9/so/batch-dis.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/batch-sntspacy.py` & `cikuu-2022.8.9/so/batch-sntspacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/dis-bnc.py` & `cikuu-2022.8.9/so/dis-bnc.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/dis-eev.py` & `cikuu-2022.8.9/so/dis-eev.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/dis-essays.py` & `cikuu-2022.8.9/so/dis-essays.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/dis-folder.py` & `cikuu-2022.8.9/so/dis-folder.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/dis-tosnts.py` & `cikuu-2022.8.9/so/dis-tosnts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/dsk.py` & `cikuu-2022.8.9/so/dsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/dump-pos.py` & `cikuu-2022.8.9/so/dump-pos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/dump-trp.py` & `cikuu-2022.8.9/so/dump-trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/folder.py` & `cikuu-2022.8.9/so/folder.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/load.py` & `cikuu-2022.8.9/so/load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/loades.py` & `cikuu-2022.8.9/so/loades.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/so/tok-idf.py` & `cikuu-2022.8.9/so/tok-idf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/sqlite/__init__.py` & `cikuu-2022.8.9/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/__init__.py` & `cikuu-2022.8.9/util/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/__main__.py` & `cikuu-2022.8.9/util/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/annotate.py` & `cikuu-2022.8.9/util/annotate.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/bcp.py` & `cikuu-2022.8.9/util/bcp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/c4data.py` & `cikuu-2022.8.9/util/c4data.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/client-blpop.py` & `cikuu-2022.8.9/util/client-blpop.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/client-xwps.py` & `cikuu-2022.8.9/util/client-xwps.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/clientx.py` & `cikuu-2022.8.9/util/clientx.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/dsk-util.py` & `cikuu-2022.8.9/util/dsk-util.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/kvr.py` & `cikuu-2022.8.9/util/kvr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/mq.py` & `cikuu-2022.8.9/util/mq.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/nldp.py` & `cikuu-2022.8.9/util/nldp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/pubsub-sync.py` & `cikuu-2022.8.9/util/pubsub-sync.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/pubsub2api.py` & `cikuu-2022.8.9/util/pubsub2api.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/spider.py` & `cikuu-2022.8.9/util/spider.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/sqlitedict-load.py` & `cikuu-2022.8.9/util/sqlitedict-load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/wps-blpop.py` & `cikuu-2022.8.9/util/wps-blpop.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/wps.py` & `cikuu-2022.8.9/util/wps.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/xsnt-spacy.py` & `cikuu-2022.8.9/util/xsnt-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/xstream.py` & `cikuu-2022.8.9/util/xstream.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/xtest-params.py` & `cikuu-2022.8.9/util/xtest-params.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/util/xtest.py` & `cikuu-2022.8.9/util/xtest.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uviapp/__init__.py` & `cikuu-2022.8.9/uviapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/Jinja2-test.py` & `cikuu-2022.8.9/uvirun/Jinja2-test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/__init__.py` & `cikuu-2022.8.9/uvirun/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/__main__.py` & `cikuu-2022.8.9/uvirun/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/c4es.py` & `cikuu-2022.8.9/uvirun/c4es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/c4gramsi.py` & `cikuu-2022.8.9/uvirun/c4gramsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/cos_fastapi.py` & `cikuu-2022.8.9/uvirun/cos_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/demo_fastapi.py` & `cikuu-2022.8.9/uvirun/demo_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/dsk_fastapi.py` & `cikuu-2022.8.9/uvirun/dsk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/echart_fastapi.py` & `cikuu-2022.8.9/uvirun/echart_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/elastic_fastapi.py` & `cikuu-2022.8.9/uvirun/elastic_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant/__init__.py` & `cikuu-2022.8.9/uvirun/errant/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant/alignment.py` & `cikuu-2022.8.9/uvirun/errant/alignment.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant/annotator.py` & `cikuu-2022.8.9/uvirun/errant/annotator.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant/commands/compare_m2.py` & `cikuu-2022.8.9/uvirun/errant/commands/compare_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant/commands/m2_to_m2.py` & `cikuu-2022.8.9/uvirun/errant/commands/m2_to_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant/commands/parallel_to_m2.py` & `cikuu-2022.8.9/uvirun/errant/commands/parallel_to_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant/edit.py` & `cikuu-2022.8.9/uvirun/errant/edit.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant/en/classifier.py` & `cikuu-2022.8.9/uvirun/errant/en/classifier.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant/en/lancaster.py` & `cikuu-2022.8.9/uvirun/errant/en/lancaster.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant/en/merger.py` & `cikuu-2022.8.9/uvirun/errant/en/merger.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/errant_fastapi.py` & `cikuu-2022.8.9/uvirun/errant_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/es1_fastapi.py` & `cikuu-2022.8.9/uvirun/es1_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/es_fastapi.py` & `cikuu-2022.8.9/uvirun/es_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/essay_fastapi.py` & `cikuu-2022.8.9/uvirun/essay_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/exchunk_fastapi.py` & `cikuu-2022.8.9/uvirun/exchunk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/feishu_fastapi.py` & `cikuu-2022.8.9/uvirun/feishu_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/flair_fastapi.py` & `cikuu-2022.8.9/uvirun/flair_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/ftp.py` & `cikuu-2022.8.9/uvirun/ftp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/fusion_fastapi.py` & `cikuu-2022.8.9/uvirun/fusion_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/gec_fastapi.py` & `cikuu-2022.8.9/uvirun/gec_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/gec_fastapi_33000.py` & `cikuu-2022.8.9/uvirun/gec_fastapi_33000.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/gensim_fastapi.py` & `cikuu-2022.8.9/uvirun/gensim_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/gramx_fastapi.py` & `cikuu-2022.8.9/uvirun/gramx_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/hnswlib_fastapi.py` & `cikuu-2022.8.9/uvirun/hnswlib_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/kenlm_fastapi.py` & `cikuu-2022.8.9/uvirun/kenlm_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/kpsi_fastapi.py` & `cikuu-2022.8.9/uvirun/kpsi_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/kvr_dskdm.py` & `cikuu-2022.8.9/uvirun/kvr_dskdm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/kvr_dskdm1230.py` & `cikuu-2022.8.9/uvirun/kvr_dskdm1230.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/nldp_fastapi.py` & `cikuu-2022.8.9/uvirun/nldp_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/nltk_fastapi.py` & `cikuu-2022.8.9/uvirun/nltk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/nsp_fastapi.py` & `cikuu-2022.8.9/uvirun/nsp_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/penlykvr.py` & `cikuu-2022.8.9/uvirun/penlykvr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/sbert_fastapi.py` & `cikuu-2022.8.9/uvirun/sbert_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/spacy_fastapi.py` & `cikuu-2022.8.9/uvirun/spacy_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/textacy_fastapi.py` & `cikuu-2022.8.9/uvirun/textacy_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/trans_fastapi.py` & `cikuu-2022.8.9/uvirun/trans_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/unmasker_fastapi.py` & `cikuu-2022.8.9/uvirun/unmasker_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/util_fastapi.py` & `cikuu-2022.8.9/uvirun/util_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/uviredis.py` & `cikuu-2022.8.9/uvirun/uviredis.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.8/uvirun/yulk-nac.py` & `cikuu-2022.8.9/uvirun/yulk-nac.py`

 * *Files identical despite different names*

