# Comparing `tmp/Products.MeetingCommunes-4.2b8.tar.gz` & `tmp/Products.MeetingCommunes-4.2b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Products.MeetingCommunes-4.2b8.tar", last modified: Wed Jan  6 09:40:10 2021, max compression
+gzip compressed data, was "dist/Products.MeetingCommunes-4.2b9.tar", last modified: Tue Jan 26 08:21:58 2021, max compression
```

## Comparing `Products.MeetingCommunes-4.2b8.tar` & `Products.MeetingCommunes-4.2b9.tar`

### file list

```diff
@@ -1,677 +1,677 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      734 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/docs/LICENSE.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      156 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23826 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/PKG-INFO
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1800 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      972 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/README.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        6 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/version.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/templates/README.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/MeetingCommunes_remunarate_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      525 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      615 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    13880 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/import_data.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/MeetingCommunes_city_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/cahier.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      930 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    43257 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/council-oj.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10115 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/recapitulatif-tb.ods
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    29777 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/synthese-avis-df.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/README.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21681 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/council-rapport.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13144 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/recapitulatif-tb.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    33757 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/oj-avec-annexes.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    32919 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/avis-df.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23146 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/projet-deliberation.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9721 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/history.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    41439 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/deliberation.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    35253 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/oj.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    34495 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/pv.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    49889 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/council-pv.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/MeetingCommunes_zones_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     2034 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/cahier.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      631 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      505 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      610 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/MeetingCommunes_coges_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/templates/README.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/MeetingCommunes_ca_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      504 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/MeetingCommunes_coordinateOffice_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      535 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      622 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      174 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/templates/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/MeetingCommunes_testing_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2021 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      411 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      355 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1147 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/legalAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      492 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/cahier.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      742 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/financialAnalysis.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      614 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      504 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/import_data.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/MeetingCommunes_scresthome_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/demo/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      179 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/demo/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/demo/MeetingCommunes_demo_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/demo/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      702 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/cahier.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/MeetingCommunes_bdc_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      175 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      137 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/rolemap.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinanceseditor_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12541 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinanceseditor_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinancesmanager_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinancesmanager_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinances_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15078 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinances_workflow/definition.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      197 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/repositorytool.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/MeetingCommunes_financesadvice_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      163 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/types.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      301 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/propertiestool.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      166 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2686 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/types/meetingadvicefinances.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      680 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/templates/README.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/MeetingCommunes_codir_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      508 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      610 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      558 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/import_data.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/MeetingCommunes_negociation_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      106 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      423 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      926 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/skins.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      712 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/toolset.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      396 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/MeetingCommunes_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/portal_languages.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/MeetingCommunes_consultation_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      528 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      617 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      266 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/organizations.csv
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10527 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/meeting_assemblies.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22450 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-oj.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/recapitulatif-tb.ods
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    29777 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/synthese-avis-df.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12722 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-rapport.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12386 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/attendance-stats.ods
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9775 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_pv.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11565 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/recapitulatif-tb.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24690 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj-avec-annexes.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19464 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/avis-df.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10079 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_delib_recto_verso.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9685 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_delib.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12170 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/organizations-export.ods
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10369 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/styles1.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9721 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/history.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    32680 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/deliberation.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24233 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14862 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/votes.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12815 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/styles2.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17357 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/attendees.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23586 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/pv.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23009 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-pv.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    32626 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/deliberation_recto_verso.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13812 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/report.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14290 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/synthese-df-tb.ods
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13154 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/dashboard.ods
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24035 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj-avec-table-des-matieres.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      760 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/heldpositions.csv
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    46281 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/import_data.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      726 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/persons.csv
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/MeetingCommunes_examples_fr_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/cahier.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      574 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/deliberation_signed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/deliberation_to_sign.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      930 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     6674 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/import_data.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/MeetingCommunes_cadvice_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/cahier.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      623 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcsss/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcsss/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcsss/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcsss/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcsss/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      504 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcsss/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcsss/toolset.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcsss/MeetingCommunes_csss_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      609 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcsss/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/MeetingCommunes_cppt_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      474 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      609 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/portal_languages.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/MeetingCommunes_etat_major_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      482 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/portal_languages.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/MeetingCommunes_bourgmestre_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      493 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      616 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/portal_languages.xml
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     5503 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/import_data.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/MeetingCommunes_simple_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     2902 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/cahier.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/MeetingCommunes_cpas_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      930 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/templates/README.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/MeetingCommunes_ca_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      512 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/MeetingCommunes_sippt_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      478 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      610 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/templates/README.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/MeetingCommunes_executive_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      508 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      621 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      498 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/MeetingCommunes_audit_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      610 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/MeetingCommunes_volonteers_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      527 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      627 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      498 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/import_data.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/MeetingCommunes_wellbeing_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/positive.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/portal_languages.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/templates/README.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      502 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/import_data.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/toolset.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/MeetingCommunes_technicalcommittee_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      544 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/refresh.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      596 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      617 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_templates/checkFDAdviceIsTimedOut.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1696 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_templates/updateOldAssemblies.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      465 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_not_given_finance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      740 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_positive_finance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      680 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_cautious_finance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      697 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_positive_with_remarks_finance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_negative_finance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      708 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_not_required_finance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      343 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/cdld.gif
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_styles/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      348 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_styles/readme.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      189 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_styles/meetingcommunes.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1833 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3123 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    67852 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/adapters.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/migrations/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/migrations/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4638 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/migrations/migrate_to_4200.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1503 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/migrations/migrate_to_4_2.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7629 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/migrations/migrate_to_4_1.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1047 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      437 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testVotes.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1297 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testMeetingItem.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1354 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testContacts.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1018 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/helpers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7360 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomWorkflows.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    10826 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomMeeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1317 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testToolPloneMeeting.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    15153 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testWorkflows.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2923 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomUtils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1333 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testChangeItemOrderView.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1275 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testValidators.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1272 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testPortlets.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1216 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testUtils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1310 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testMeetingCategory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1259 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testFaceted.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1249 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testSearches.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4298 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomMeetingItem.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      996 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/MeetingCommunesTestCase.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1231 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testAnnexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1226 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testColumns.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1300 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testMeetingConfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      502 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testWFAdaptations.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1286 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testMeeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1350 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testAdvices.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3596 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomToolPloneMeeting.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/robot/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9578 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/robot/doc-fr.robot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    48125 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomViews.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2165 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomWFAdaptations.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1221 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testViews.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1263 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testSetup.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23067 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/importxml.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9865 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3386 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/force-language.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10619 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/ImportCategories.ods
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13233 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/importGroupsUsersAndRoles.ods
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25665 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/importxml-stesud.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    20593 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/import-csv-civadis.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15818 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/import-csv-olln.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10945 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/importGroups.ods
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/model/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/model/__init__.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      645 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/model/generate.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1342 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/model/pm_updates.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18502 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/model/MeetingCommunes.zargo
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3003 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/model/generate.conf
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21355 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/setuphandlers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8698 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3016 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5269 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1096 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/overrides.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30595 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/browser/overrides.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/nl/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4233 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2090 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12700 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1575 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2070 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/imio.history.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/de/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4346 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2090 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12761 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1666 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1400 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/imio.actionspanel.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12281 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/plone.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10863 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2732 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16821 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2299 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/imio.actionspanel.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5525 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2123 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12638 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1661 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4038 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/PloneMeeting.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/es/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4578 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2090 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13063 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1890 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/imio.actionspanel.po
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      307 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/sync_pos.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       76 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/EXTERNALS.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products.MeetingCommunes.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products.MeetingCommunes.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23826 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products.MeetingCommunes.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products.MeetingCommunes.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    36829 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products.MeetingCommunes.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products.MeetingCommunes.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      114 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products.MeetingCommunes.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/src/Products.MeetingCommunes.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      354 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1143 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19461 2021-01-06 09:40:10.000000 Products.MeetingCommunes-4.2b8/CHANGES.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      734 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/docs/LICENSE.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      341 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24599 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/PKG-INFO
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1800 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      972 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/README.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        6 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/version.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/templates/README.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/MeetingCommunes_remunarate_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      525 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      615 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    13880 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/import_data.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/MeetingCommunes_city_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/cahier.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      930 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    43257 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/council-oj.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10115 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/recapitulatif-tb.ods
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    29777 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/synthese-avis-df.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/README.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21681 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/council-rapport.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13144 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/recapitulatif-tb.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    33757 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/oj-avec-annexes.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    32919 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/avis-df.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23146 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/projet-deliberation.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9721 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/history.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    41439 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/deliberation.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    35253 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/oj.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    34495 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/pv.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    49889 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/council-pv.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/MeetingCommunes_zones_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     2034 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/cahier.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      631 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      505 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      610 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/MeetingCommunes_coges_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/templates/README.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/MeetingCommunes_ca_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      504 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/MeetingCommunes_coordinateOffice_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      535 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      622 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      174 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/templates/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/MeetingCommunes_testing_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2021 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      411 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/overheadAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/decisionAnnex.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/itemAnnex.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      355 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1147 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/legalAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      492 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/budgetAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/cahier.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      742 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/financialAnalysis.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      614 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      504 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/import_data.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/MeetingCommunes_scresthome_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/demo/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      179 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/demo/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/demo/MeetingCommunes_demo_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/demo/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      702 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/cahier.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/MeetingCommunes_bdc_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      175 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      137 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/rolemap.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinanceseditor_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12541 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinanceseditor_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinancesmanager_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinancesmanager_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinances_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15078 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinances_workflow/definition.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      197 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/repositorytool.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/MeetingCommunes_financesadvice_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      163 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/types.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      301 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/propertiestool.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      166 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2686 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/types/meetingadvicefinances.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      680 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/templates/README.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/MeetingCommunes_codir_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      508 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      610 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      558 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/import_data.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/MeetingCommunes_negociation_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      106 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      423 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/jsregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      926 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/skins.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      712 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/toolset.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      396 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/MeetingCommunes_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/portal_languages.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/MeetingCommunes_consultation_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      528 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      617 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      266 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/organizations.csv
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10527 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/meeting_assemblies.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22450 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-oj.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/recapitulatif-tb.ods
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    29777 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/synthese-avis-df.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12722 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-rapport.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12386 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/attendance-stats.ods
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9775 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_pv.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11565 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/recapitulatif-tb.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24690 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj-avec-annexes.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19464 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/avis-df.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10079 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_delib_recto_verso.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9685 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_delib.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12170 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/organizations-export.ods
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10369 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/styles1.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9721 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/history.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    32680 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/deliberation.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24233 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14862 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/votes.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12815 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/styles2.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17643 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/attendees.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23586 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/pv.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23009 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-pv.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    32626 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/deliberation_recto_verso.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13812 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/report.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14290 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/synthese-df-tb.ods
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13154 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/dashboard.ods
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24035 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj-avec-table-des-matieres.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      760 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/heldpositions.csv
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    46281 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/import_data.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      726 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/persons.csv
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/MeetingCommunes_examples_fr_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/cahier.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      574 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/deliberation_signed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/deliberation_to_sign.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      930 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     6674 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/import_data.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/MeetingCommunes_cadvice_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/cahier.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      623 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcsss/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcsss/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcsss/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcsss/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcsss/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      504 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcsss/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcsss/toolset.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcsss/MeetingCommunes_csss_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      609 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcsss/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/MeetingCommunes_cppt_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      474 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      609 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/portal_languages.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/MeetingCommunes_etat_major_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      482 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/portal_languages.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/MeetingCommunes_bourgmestre_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      493 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      616 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/portal_languages.xml
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     5503 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/import_data.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/MeetingCommunes_simple_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     2902 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/cahier.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/MeetingCommunes_cpas_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      930 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/templates/README.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/MeetingCommunes_ca_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      512 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/MeetingCommunes_sippt_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      478 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      610 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/templates/README.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/MeetingCommunes_executive_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      508 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      621 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      498 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/MeetingCommunes_audit_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      610 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/MeetingCommunes_volonteers_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      527 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      627 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      498 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/import_data.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/MeetingCommunes_wellbeing_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/positive.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/portal_languages.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/templates/README.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      502 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/import_data.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/toolset.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/MeetingCommunes_technicalcommittee_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      607 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      544 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/refresh.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      596 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      617 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_templates/checkFDAdviceIsTimedOut.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1696 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_templates/updateOldAssemblies.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      465 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_not_given_finance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      740 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_positive_finance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      680 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_cautious_finance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      697 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_positive_with_remarks_finance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_negative_finance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      708 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_not_required_finance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      343 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/cdld.gif
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_styles/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      348 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_styles/readme.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      189 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_styles/meetingcommunes.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1833 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3123 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    68105 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/migrations/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/migrations/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4638 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/migrations/migrate_to_4200.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1503 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/migrations/migrate_to_4_2.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7629 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/migrations/migrate_to_4_1.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1047 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      437 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testVotes.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1297 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testMeetingItem.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1354 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testContacts.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1018 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/helpers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7360 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomWorkflows.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    10826 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomMeeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1317 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testToolPloneMeeting.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    15153 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testWorkflows.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2923 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomUtils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1333 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testChangeItemOrderView.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1275 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testValidators.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1272 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testPortlets.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1216 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testUtils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1310 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testMeetingCategory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1259 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testFaceted.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1249 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testSearches.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4298 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomMeetingItem.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      996 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/MeetingCommunesTestCase.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1231 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testAnnexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1226 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testColumns.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1300 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testMeetingConfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      502 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testWFAdaptations.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1286 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testMeeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1350 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testAdvices.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3596 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomToolPloneMeeting.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/robot/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9578 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/robot/doc-fr.robot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    48125 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomViews.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2165 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomWFAdaptations.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1221 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testViews.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1263 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testSetup.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23067 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/importxml.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9865 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3386 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/force-language.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10619 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/ImportCategories.ods
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13233 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/importGroupsUsersAndRoles.ods
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25665 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/importxml-stesud.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    20593 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/import-csv-civadis.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15818 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/import-csv-olln.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10945 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/importGroups.ods
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/model/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/model/__init__.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      645 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/model/generate.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1342 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/model/pm_updates.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18502 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/model/MeetingCommunes.zargo
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3003 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/model/generate.conf
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21355 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/setuphandlers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8698 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3016 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5269 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1096 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/overrides.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30595 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/browser/overrides.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/nl/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4233 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2090 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12700 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1575 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2070 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/imio.history.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/de/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4346 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2090 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12761 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1666 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1400 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/imio.actionspanel.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12281 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/plone.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10863 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2732 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16821 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2299 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/imio.actionspanel.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5525 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2123 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12638 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1661 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4038 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/PloneMeeting.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/es/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4578 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2090 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13063 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1890 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/imio.actionspanel.po
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      307 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/sync_pos.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       76 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/EXTERNALS.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products.MeetingCommunes.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products.MeetingCommunes.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24599 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products.MeetingCommunes.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products.MeetingCommunes.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    36829 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products.MeetingCommunes.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products.MeetingCommunes.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      114 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products.MeetingCommunes.egg-info/requires.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/src/Products.MeetingCommunes.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      354 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1143 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19921 2021-01-26 08:21:58.000000 Products.MeetingCommunes-4.2b9/CHANGES.rst
```

### Comparing `Products.MeetingCommunes-4.2b8/docs/LICENSE.GPL` & `Products.MeetingCommunes-4.2b9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/docs/LICENSE.txt` & `Products.MeetingCommunes-4.2b9/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/PKG-INFO` & `Products.MeetingCommunes-4.2b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 Metadata-Version: 2.1
 Name: Products.MeetingCommunes
-Version: 4.2b8
+Version: 4.2b9
 Summary: Official meetings management for college and council of belgiancommunes (PloneMeeting extension profile)
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL
 Description: ========================
         Products.MeetingCommunes
         ========================
         
         ``Products.MeetingCommunes`` is a custom profile for ``Products.PloneMeeting``.
         
+        .. image:: https://coveralls.io/repos/github/IMIO/Products.MeetingCommunes/badge.svg?branch=master
+            :target: https://coveralls.io/github/IMIO/Products.MeetingCommunes?branch=master
+        
         Products.MeetingCommunes Changelog
         ==================================
         
         The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
         
         
+        4.2b9 (2021-01-26)
+        ------------------
+        
+        - Added 2 mores formatting examples for `view.print_attendees_by_type` in
+          `attendees.odt` template.
+          [aduchene]
+        - Changed uppercases in example_fr profile for `directory_position_types`.
+          [aduchene]
+        - Fixed `MeetingItemCommunesWorkflowActions._doWaitAdvices`, make sure
+          `MeetingItem.completeness` is set to `completeness_evaluation_asked_again`
+          when advices are asked for the second time (or more).
+          [gbastien]
+        
         4.2b8 (2021-01-06)
         ------------------
         
         - Added POD template that renders various votes on item.
           [gbastien]
         - Do no more ignore testVotes when executing tests.
           [gbastien]
```

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/__init__.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/README.txt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/README.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zremunarate/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zremunarate/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/images/cahier.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcity/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcity/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/council-oj.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/council-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/recapitulatif-tb.ods` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/recapitulatif-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/synthese-avis-df.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/synthese-avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/council-rapport.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/council-rapport.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/recapitulatif-tb.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/recapitulatif-tb.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/oj-avec-annexes.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/oj-avec-annexes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/avis-df.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/projet-deliberation.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/projet-deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/history.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/history.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/deliberation.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/oj.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/pv.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/templates/council-pv.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/templates/council-pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/images/cahier.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zones/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zones/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoges/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoges/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zag/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zag/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcoordinate_office/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcoordinate_office/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/cahier.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/images/financialAnalysis.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/testing/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/testing/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zscresthome/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zscresthome/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/images/cahier.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbdc/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbdc/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinanceseditor_workflow/definition.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinanceseditor_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinancesmanager_workflow/definition.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinancesmanager_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinances_workflow/definition.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows/meetingadvicefinances_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/types/meetingadvicefinances.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/types/meetingadvicefinances.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/financesadvice/workflows.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/financesadvice/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcodir/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcodir/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/znegotiation/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/znegotiation/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/skins.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/default/cssregistry.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zconsultation/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zconsultation/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/meeting_assemblies.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/meeting_assemblies.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-oj.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/recapitulatif-tb.ods` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/recapitulatif-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/synthese-avis-df.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/synthese-avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-rapport.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-rapport.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/attendance-stats.ods` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/attendance-stats.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_pv.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/recapitulatif-tb.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/recapitulatif-tb.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj-avec-annexes.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj-avec-annexes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/avis-df.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_delib_recto_verso.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_delib_recto_verso.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_delib.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/all_delib.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/organizations-export.ods` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/organizations-export.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/styles1.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/styles1.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/history.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/history.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/deliberation.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/votes.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/votes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/styles2.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/styles2.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/pv.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-pv.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/council-pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/deliberation_recto_verso.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/deliberation_recto_verso.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/report.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/report.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/synthese-df-tb.ods` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/synthese-df-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/dashboard.ods` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/dashboard.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj-avec-table-des-matieres.odt` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/templates/oj-avec-table-des-matieres.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/heldpositions.csv` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/heldpositions.csv`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/import_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -816,26 +816,26 @@
 data.usersOutsideGroups = [bourgmestre, conseiller]
 data.directory_position_types = [
     {'token': u'default',
      'name': u'(Utiliser le champ "Intitulé", non recommandé)'},
     {'token': u'administrateur',
      'name': u'Administrateur|Administrateurs|Administratrice|Administratrices'},
     {'token': u'alderman',
-     'name': u'échevin|échevins|échevine|échevines'},
-    {'name': u'1er échevin|1er échevins|1ère échevine|1ère échevines',
+     'name': u'Échevin|Échevins|Échevine|Échevines'},
+    {'name': u'1er Échevin|1er Échevins|1ère Échevine|1ère Échevines',
      'token': u'alderman-1'},
-    {'name': u'2ème échevin|2èmes échevins|2ème échevine|2èmes échevines',
+    {'name': u'2ème Échevin|2èmes Échevins|2ème Échevine|2èmes Échevines',
      'token': u'alderman-2'},
-    {'name': u'3ème échevin|3èmes échevins|3ème échevine|3èmes échevines',
+    {'name': u'3ème Échevin|3èmes Échevins|3ème Échevine|3èmes Échevines',
      'token': u'alderman-3'},
-    {'name': u'4ème échevin|4èmes échevins|4ème échevine|4èmes échevines',
+    {'name': u'4ème Échevin|4èmes Échevins|4ème Échevine|4èmes Échevines',
      'token': u'alderman-4'},
-    {'name': u'5ème échevin|5èmes échevins|5ème échevine|5èmes échevines',
+    {'name': u'5ème Échevin|5èmes Échevins|5ème Échevine|5èmes Échevines',
      'token': u'alderman-5'},
-    {'name': u'6ème échevin|6èmes échevins|6ème échevine|6èmes échevines',
+    {'name': u'6ème Échevin|6èmes Échevins|6ème Échevine|6èmes Échevines',
      'token': u'alderman-6'},
     {'token': u'bourgmestre',
      'name': u'Bourgmestre|Bourgmestres|Bourgmestre|Bourgmestres'},
     {'token': u'bourgmestreff',
      'name': u'Bourgmestre f.f.|Bourgmestres f.f.|Bourgmestre f.f.|Bourgmestres f.f.'},
     {'token': u'president',
      'name': u'Président|Présidents|Présidente|Présidentes'},
@@ -849,24 +849,24 @@
      'name': u'Conseiller|Conseillers|Conseillère|Conseillères'},
     {'token': u'conseiller-president',
      'name': u'Conseiller - Président|Conseillers - Présidents|'
         u'Conseillère - Présidente|Conseillères - Présidentes'},
     {'token': u'president-cpas',
      'name': u'Président du CPAS|Présidents du CPAS|Présidente du CPAS|Présidentes du CPAS'},
     {'token': u'dg',
-     'name': u'Directeur Général|Directeurs Généraux|'
-        u'Directrice Générale|Directrices Générales'},
+     'name': u'Directeur général|Directeurs généraux|'
+        u'Directrice générale|Directrices générales'},
     {'token': u'dgff',
-     'name': u'Directeur Général f.f.|Directeurs Généraux f.f.|'
-        u'Directrice Générale f.f.|Directrices Générales f.f.'},
+     'name': u'Directeur général f.f.|Directeurs généraux f.f.|'
+        u'Directrice générale f.f.|Directrices générales f.f.'},
     {'token': u'df',
-     'name': u'Directeur Financier|Directeurs Financiers|Directrice Financière|Directrices Financières'},
+     'name': u'Directeur financier|Directeurs financiers|Directrice financière|Directrices financières'},
     {'token': u'dfff',
-     'name': u'Directeur Financier f.f.|Directeurs Financiers f.f.|'
-        u'Directrice Financière f.f.|Directrices Financières f.f.'},
+     'name': u'Directeur financier f.f.|Directeurs financiers f.f.|'
+        u'Directrice financière f.f.|Directrices financières f.f.'},
     {'token': u'depute',
      'name': u'Député|Députés|Députée|Députées'},
     {'token': u'secretaire',
      'name': u'Secrétaire de séance|Secrétaires de séance|Secrétaire de séance|Secrétaires de séance'},
 ]
 contactsTemplate = PodTemplateDescriptor('contactsTemplate', 'Export', dashboard=True)
 contactsTemplate.odt_file = 'organizations-export.ods'
```

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/persons.csv` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/persons.csv`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/cahier.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/images/deliberation_signed.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/images/deliberation_signed.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/examples_fr/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/examples_fr/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/cahier.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_advice/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_advice/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcsss/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcsss/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcppt/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcppt/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zetat_major/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zetat_major/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zbourgmestre/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zbourgmestre/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/simple/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/simple/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/images/cahier.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcpas/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcpas/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zca/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zca/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zsippt/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zsippt/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zexecutive_office/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zexecutive_office/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zaudit/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zaudit/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/import_data.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zcommittee_volonteers/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/zwellbeing/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/zwellbeing/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/negative.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/legalAdvice.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/attach.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/budget.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/remarks.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/positive.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/import_steps.xml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles/ztechnicalcommittee/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/utils.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/utils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/testing.zcml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_templates/checkFDAdviceIsTimedOut.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_templates/checkFDAdviceIsTimedOut.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_templates/updateOldAssemblies.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_templates/updateOldAssemblies.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_positive_finance.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_positive_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_cautious_finance.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_cautious_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_positive_with_remarks_finance.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_positive_with_remarks_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_negative_finance.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_negative_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_not_required_finance.png` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/skins/meetingcommunes_images/advice_standard_not_required_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/testing.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/interfaces.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/adapters.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -953,29 +953,32 @@
 
     implements(IMeetingItemCommunesWorkflowActions)
     security = ClassSecurityInfo()
 
     def _will_ask_completeness_eval_again(self):
         ''' '''
         return 'completeness' in self.cfg.getUsedItemAttributes() and \
-            self.context.queryState() in finances_give_advice_states(self.cfg)
+            self.context.queryState() in finances_give_advice_states(self.cfg) and \
+            self.context.getCompleteness() in ['completeness_incomplete',
+                                               'completeness_evaluation_not_required']
 
     def _will_set_completeness_to_not_required(self):
         ''' '''
         return False
 
     def _doWaitAdvices(self):
         '''When advices are asked again and we use MeetingItem.completeness field,
            make sure the item completeness evaluation is asked again so advice is not
            addable/editable when item come back again to this state.'''
         if self._will_ask_completeness_eval_again():
             wfTool = api.portal.get_tool('portal_workflow')
             history = self.context.workflow_history[wfTool.getWorkflowsFor(self.context)[0].getId()][:-1]
             for event in history:
-                if event['action'] in ['wait_advices_from_proposed', 'wait_advices_from_prevalidated']:
+                # set completeness to asked_again if it is not the first time that advices are asked
+                if event['action'] and event['action'].startswith('wait_advices_from_'):
                     changeCompleteness = self.context.restrictedTraverse('@@change-item-completeness')
                     comment = translate('completeness_asked_again_by_app',
                                         domain='PloneMeeting',
                                         context=self.context.REQUEST)
                     # change completeness even if current user is not able to set it to
                     # 'completeness_evaluation_asked_again', here it is the application that set
                     # it automatically
```

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/migrations/migrate_to_4200.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/migrations/migrate_to_4200.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/migrations/migrate_to_4_2.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/migrations/migrate_to_4_2.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/migrations/migrate_to_4_1.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/migrations/migrate_to_4_1.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/__init__.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testMeetingItem.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testContacts.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testContacts.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/helpers.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomWorkflows.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomMeeting.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testToolPloneMeeting.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testWorkflows.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomUtils.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testChangeItemOrderView.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testValidators.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testPortlets.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testUtils.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testMeetingCategory.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testFaceted.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testSearches.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomMeetingItem.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/MeetingCommunesTestCase.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/MeetingCommunesTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testAnnexes.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testColumns.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testMeetingConfig.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testMeeting.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testAdvices.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomToolPloneMeeting.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/robot/doc-fr.robot` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/robot/doc-fr.robot`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomViews.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testCustomWFAdaptations.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testCustomWFAdaptations.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testViews.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/tests/testSetup.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/importxml.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/importxml.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/utils.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/utils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/force-language.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/force-language.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/ImportCategories.ods` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/ImportCategories.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/importGroupsUsersAndRoles.ods` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/importGroupsUsersAndRoles.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/importxml-stesud.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/importxml-stesud.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/import-csv-civadis.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/import-csv-civadis.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/import-csv-olln.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/import-csv-olln.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/Extensions/importGroups.ods` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/Extensions/importGroups.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/model/generate.sh` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/model/generate.sh`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/model/pm_updates.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/model/pm_updates.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/model/MeetingCommunes.zargo` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/model/MeetingCommunes.zargo`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/model/generate.conf` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/model/generate.conf`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/setuphandlers.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/profiles.zcml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/config.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/config.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/configure.zcml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/overrides.zcml` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/browser/overrides.py` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/browser/overrides.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/imio.history.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/plone.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/nl/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/imio.history.pot` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/imio.history.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/plone.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/de/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/imio.actionspanel.pot` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/plone.pot` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/imio.history.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/imio.history.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/plone.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/en/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/PloneMeeting.pot` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/PloneMeeting.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/imio.history.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/plone.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingCommunes-4.2b9/src/Products/MeetingCommunes/locales/es/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/src/Products.MeetingCommunes.egg-info/PKG-INFO` & `Products.MeetingCommunes-4.2b9/src/Products.MeetingCommunes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 Metadata-Version: 2.1
 Name: Products.MeetingCommunes
-Version: 4.2b8
+Version: 4.2b9
 Summary: Official meetings management for college and council of belgiancommunes (PloneMeeting extension profile)
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL
 Description: ========================
         Products.MeetingCommunes
         ========================
         
         ``Products.MeetingCommunes`` is a custom profile for ``Products.PloneMeeting``.
         
+        .. image:: https://coveralls.io/repos/github/IMIO/Products.MeetingCommunes/badge.svg?branch=master
+            :target: https://coveralls.io/github/IMIO/Products.MeetingCommunes?branch=master
+        
         Products.MeetingCommunes Changelog
         ==================================
         
         The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
         
         
+        4.2b9 (2021-01-26)
+        ------------------
+        
+        - Added 2 mores formatting examples for `view.print_attendees_by_type` in
+          `attendees.odt` template.
+          [aduchene]
+        - Changed uppercases in example_fr profile for `directory_position_types`.
+          [aduchene]
+        - Fixed `MeetingItemCommunesWorkflowActions._doWaitAdvices`, make sure
+          `MeetingItem.completeness` is set to `completeness_evaluation_asked_again`
+          when advices are asked for the second time (or more).
+          [gbastien]
+        
         4.2b8 (2021-01-06)
         ------------------
         
         - Added POD template that renders various votes on item.
           [gbastien]
         - Do no more ignore testVotes when executing tests.
           [gbastien]
```

### Comparing `Products.MeetingCommunes-4.2b8/src/Products.MeetingCommunes.egg-info/SOURCES.txt` & `Products.MeetingCommunes-4.2b9/src/Products.MeetingCommunes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCommunes-4.2b8/setup.py` & `Products.MeetingCommunes-4.2b9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '4.2b8'
+version = '4.2b9'
 
 setup(
     name='Products.MeetingCommunes',
     version=version,
     description="Official meetings management for college and council of belgian"
     "communes (PloneMeeting extension profile)",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
```

### Comparing `Products.MeetingCommunes-4.2b8/CHANGES.rst` & `Products.MeetingCommunes-4.2b9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 Products.MeetingCommunes Changelog
 ==================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
 
+4.2b9 (2021-01-26)
+------------------
+
+- Added 2 mores formatting examples for `view.print_attendees_by_type` in
+  `attendees.odt` template.
+  [aduchene]
+- Changed uppercases in example_fr profile for `directory_position_types`.
+  [aduchene]
+- Fixed `MeetingItemCommunesWorkflowActions._doWaitAdvices`, make sure
+  `MeetingItem.completeness` is set to `completeness_evaluation_asked_again`
+  when advices are asked for the second time (or more).
+  [gbastien]
+
 4.2b8 (2021-01-06)
 ------------------
 
 - Added POD template that renders various votes on item.
   [gbastien]
 - Do no more ignore testVotes when executing tests.
   [gbastien]
```

