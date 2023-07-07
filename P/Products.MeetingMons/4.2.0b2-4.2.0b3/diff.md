# Comparing `tmp/Products.MeetingMons-4.2.0b2.tar.gz` & `tmp/Products.MeetingMons-4.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.MeetingMons-4.2.0b2.tar", last modified: Fri Jul  7 07:40:15 2023, max compression
+gzip compressed data, was "Products.MeetingMons-4.2.0b3.tar", last modified: Fri Jul  7 08:42:03 2023, max compression
```

## Comparing `Products.MeetingMons-4.2.0b2.tar` & `Products.MeetingMons-4.2.0b3.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.840110 Products.MeetingMons-4.2.0b2/
--rw-rw-r--   0 adu       (1000) adu       (1000)     5873 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/CHANGES.rst
--rw-rw-r--   0 adu       (1000) adu       (1000)      354 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/MANIFEST.in
--rw-rw-r--   0 adu       (1000) adu       (1000)     6948 2023-07-07 07:40:15.840110 Products.MeetingMons-4.2.0b2/PKG-INFO
--rw-rw-r--   0 adu       (1000) adu       (1000)      530 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/README.rst
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.824109 Products.MeetingMons-4.2.0b2/docs/
--rw-rw-r--   0 adu       (1000) adu       (1000)    18092 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/docs/LICENSE.GPL
--rw-rw-r--   0 adu       (1000) adu       (1000)      730 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/docs/LICENSE.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)       38 2023-07-07 07:40:15.840110 Products.MeetingMons-4.2.0b2/setup.cfg
--rw-rw-r--   0 adu       (1000) adu       (1000)     1406 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/setup.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.824109 Products.MeetingMons-4.2.0b2/src/
--rw-rw-r--   0 adu       (1000) adu       (1000)       76 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/EXTERNALS.txt
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.824109 Products.MeetingMons-4.2.0b2/src/Products/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/Extensions/
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/Extensions/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     5076 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/Extensions/plonemeeting_portal_helpers.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1792 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)    29320 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/adapters.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/browser/
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/browser/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1232 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/browser/configure.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)    22569 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/browser/overrides.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     4507 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/browser/views.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     5978 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/config.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      703 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/configure.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)     2619 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/interfaces.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/
--rw-rw-r--   0 adu       (1000) adu       (1000)     5152 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/PloneMeeting.pot
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.824109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/fr/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)    12236 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     3778 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/fr/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     2397 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/fr/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 adu       (1000) adu       (1000)    14014 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     2461 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/imio.actionspanel.pot
--rw-rw-r--   0 adu       (1000) adu       (1000)     1839 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/imio.history.pot
--rw-rw-r--   0 adu       (1000) adu       (1000)    10271 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/plone.pot
--rwxrwxr-x   0 adu       (1000) adu       (1000)      307 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/sync_pos.sh
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/migrations/
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/migrations/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     4845 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/migrations/migrate_to_4200.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      949 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/migrations/migrate_to_4_1.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/model/
--rw-rw-r--   0 adu       (1000) adu       (1000)    25050 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/model/MeetingMons.zargo
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/model/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     3003 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/model/generate.conf
--rwxrwxr-x   0 adu       (1000) adu       (1000)      316 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/model/generate.sh
--rw-rw-r--   0 adu       (1000) adu       (1000)     3043 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/model/pm_updates.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     3343 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/overrides.zcml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/
--rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/MeetingMons_marker.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      184 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/browserlayer.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      708 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/cssregistry.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      722 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/import_steps.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      423 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/jsregistry.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      106 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      878 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/skins.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      167 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/toolset.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.824109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/workflows/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/workflows/meetingcollegemons_workflow/
--rw-rw-r--   0 adu       (1000) adu       (1000)    10865 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/workflows/meetingcollegemons_workflow/definition.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/workflows/meetingitemcollegemons_workflow/
--rw-rw-r--   0 adu       (1000) adu       (1000)    86659 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/workflows/meetingitemcollegemons_workflow/definition.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)     1078 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/workflows.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.828109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/
--rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/MeetingMons_Mons_marker.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.832110 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/
--rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/attach.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/budget.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/budgetAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/cahier.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/decisionAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/financialAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/itemAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      761 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/legalAdvice.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/legalAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      885 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/negative.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      305 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/nil.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/overheadAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      583 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/positive.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      705 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/remarks.png
--rwxrwxr-x   0 adu       (1000) adu       (1000)     6396 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/import_data.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)      882 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/import_steps.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.832110 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/
--rw-rw-r--   0 adu       (1000) adu       (1000)     7808 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/Agenda.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)     7808 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/Decisions.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)     7808 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/Item.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    25991 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/college-oj-avec-annexes.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    24918 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/college-oj.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    26258 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/college-pv.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    25892 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/council-oj.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    29270 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/council-pv.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    14259 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/council-rapport.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    24404 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/deliberation.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    19378 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/projet-deliberation.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    20947 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/synthese cdld.odt
--rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/toolset.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.832110 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/
--rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/MeetingMons_testing_marker.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.836109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/
--rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/attach.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/budget.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/cahier.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/financialAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/legalAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      411 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/negative.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1147 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/positive.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      355 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/remarks.png
--rwxrwxr-x   0 adu       (1000) adu       (1000)     6345 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/import_data.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)      578 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/import_steps.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      170 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/metadata.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.836109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/templates/
--rwxrwxr-x   0 adu       (1000) adu       (1000)    93772 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/templates/Agenda.odt
--rwxrwxr-x   0 adu       (1000) adu       (1000)    29171 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/templates/Decisions.odt
--rwxrwxr-x   0 adu       (1000) adu       (1000)    25438 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/templates/Item.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/templates/README.txt
--rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/toolset.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)     1400 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)     6246 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/setuphandlers.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.824109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.836109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/
--rw-rw-r--   0 adu       (1000) adu       (1000)      680 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_cautious_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_negative_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      465 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_not_given_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      708 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_not_required_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      740 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_positive_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      697 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_positive_with_remarks_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      343 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/cdld.gif
--rw-rw-r--   0 adu       (1000) adu       (1000)      680 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToBudgetImpactReviewer.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      613 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToDirector.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      626 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToDivisionHead.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToExtraordinaryBudget.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      608 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToOfficeManager.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      638 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToServiceHead.png
--rw-rw-r--   0 adu       (1000) adu       (1000)    45487 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/spinner.gif
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.836109 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_styles/
--rw-rw-r--   0 adu       (1000) adu       (1000)     1276 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_styles/meetingmons.css
--rw-rw-r--   0 adu       (1000) adu       (1000)      344 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_styles/readme.txt
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.840110 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/
--rw-rw-r--   0 adu       (1000) adu       (1000)      617 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/checkFDAdviceIsTimedOut.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     7590 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_edit.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)     9182 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_old_edit.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)    36740 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_old_view.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)    39817 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_view.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)     1701 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/updateOldAssemblies.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1100 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/testing.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      639 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/testing.zcml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.840110 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/
--rwxrwxr-x   0 adu       (1000) adu       (1000)     1564 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/MeetingMonsTestCase.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1047 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     5578 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/helpers.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1337 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testAdvices.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1632 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testAnnexes.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1320 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testChangeItemOrderView.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1213 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testColumns.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     5136 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testCustomMeetingItem.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     8349 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testCustomWorkflows.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1246 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testFaceted.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1276 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testMeeting.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1297 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testMeetingCategory.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1646 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testMeetingConfig.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)     1420 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testMeetingItem.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1259 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testPortlets.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     2381 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testSearches.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1250 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testSetup.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1393 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testToolPloneMeeting.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1203 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testUtils.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1262 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testValidators.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1208 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testViews.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     2743 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testWFAdaptations.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)    11545 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testWorkflows.py
--rw-rw-r--   0 adu       (1000) adu       (1000)       56 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 07:40:15.824109 Products.MeetingMons-4.2.0b2/src/Products.MeetingMons.egg-info/
--rw-rw-r--   0 adu       (1000) adu       (1000)     6948 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products.MeetingMons.egg-info/PKG-INFO
--rw-rw-r--   0 adu       (1000) adu       (1000)     8959 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products.MeetingMons.egg-info/SOURCES.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products.MeetingMons.egg-info/dependency_links.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products.MeetingMons.egg-info/namespace_packages.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products.MeetingMons.egg-info/not-zip-safe
--rw-rw-r--   0 adu       (1000) adu       (1000)      234 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products.MeetingMons.egg-info/requires.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-07-07 07:40:15.000000 Products.MeetingMons-4.2.0b2/src/Products.MeetingMons.egg-info/top_level.txt
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.533285 Products.MeetingMons-4.2.0b3/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5979 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/CHANGES.rst
+-rw-rw-r--   0 adu       (1000) adu       (1000)      354 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/MANIFEST.in
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7054 2023-07-07 08:42:03.533285 Products.MeetingMons-4.2.0b3/PKG-INFO
+-rw-rw-r--   0 adu       (1000) adu       (1000)      530 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/README.rst
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.517284 Products.MeetingMons-4.2.0b3/docs/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    18092 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/docs/LICENSE.GPL
+-rw-rw-r--   0 adu       (1000) adu       (1000)      730 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/docs/LICENSE.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)       38 2023-07-07 08:42:03.533285 Products.MeetingMons-4.2.0b3/setup.cfg
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1406 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/setup.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.517284 Products.MeetingMons-4.2.0b3/src/
+-rw-rw-r--   0 adu       (1000) adu       (1000)       76 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/EXTERNALS.txt
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.517284 Products.MeetingMons-4.2.0b3/src/Products/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.521285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.521285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/Extensions/
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/Extensions/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5076 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/Extensions/plonemeeting_portal_helpers.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1792 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)    29320 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/adapters.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.521285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/browser/
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/browser/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1236 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/browser/configure.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)    21593 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/browser/overrides.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4507 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/browser/views.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5978 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/config.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      703 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/configure.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2619 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/interfaces.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.521285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5152 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/PloneMeeting.pot
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.517284 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/fr/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.521285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    12236 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3778 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/fr/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2397 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/fr/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)    14014 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2461 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/imio.actionspanel.pot
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1839 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/imio.history.pot
+-rw-rw-r--   0 adu       (1000) adu       (1000)    10271 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/plone.pot
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      307 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/sync_pos.sh
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.521285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/migrations/
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/migrations/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4845 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/migrations/migrate_to_4200.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      949 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/migrations/migrate_to_4_1.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.521285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/model/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    25050 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/model/MeetingMons.zargo
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/model/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3003 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/model/generate.conf
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      316 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/model/generate.sh
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3043 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/model/pm_updates.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3343 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/overrides.zcml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.521285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.525285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/MeetingMons_marker.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      184 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/browserlayer.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      708 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/cssregistry.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      722 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/import_steps.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      423 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/jsregistry.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      106 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      878 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/skins.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      167 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/toolset.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.517284 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/workflows/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.525285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/workflows/meetingcollegemons_workflow/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    10865 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/workflows/meetingcollegemons_workflow/definition.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.525285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/workflows/meetingitemcollegemons_workflow/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    86659 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/workflows/meetingitemcollegemons_workflow/definition.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1078 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/workflows.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.525285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/MeetingMons_Mons_marker.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.525285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/attach.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/budget.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/budgetAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/cahier.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/decisionAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/financialAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/itemAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      761 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/legalAdvice.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/legalAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      885 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/negative.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      305 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/nil.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/overheadAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      583 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/positive.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      705 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/remarks.png
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     6396 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/import_data.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      882 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/import_steps.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.525285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7808 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/Agenda.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7808 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/Decisions.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7808 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/Item.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    25991 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/college-oj-avec-annexes.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    24918 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/college-oj.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    26258 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/college-pv.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    25892 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/council-oj.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    29270 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/council-pv.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    14259 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/council-rapport.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    24404 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/deliberation.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    19378 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/projet-deliberation.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    20947 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/synthese cdld.odt
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/toolset.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.525285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/MeetingMons_testing_marker.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.529285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/attach.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/budget.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/budgetAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/cahier.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/decisionAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/financialAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/itemAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/legalAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      411 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/negative.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/overheadAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1147 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/positive.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      355 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/remarks.png
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     6345 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/import_data.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      578 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/import_steps.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      170 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/metadata.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.529285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/templates/
+-rwxrwxr-x   0 adu       (1000) adu       (1000)    93772 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/templates/Agenda.odt
+-rwxrwxr-x   0 adu       (1000) adu       (1000)    29171 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/templates/Decisions.odt
+-rwxrwxr-x   0 adu       (1000) adu       (1000)    25438 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/templates/Item.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/templates/README.txt
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/toolset.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1400 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     6246 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/setuphandlers.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.517284 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.529285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      680 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_cautious_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_negative_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      465 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_not_given_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      708 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_not_required_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      740 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_positive_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      697 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_positive_with_remarks_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      343 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/cdld.gif
+-rw-rw-r--   0 adu       (1000) adu       (1000)      680 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToBudgetImpactReviewer.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      613 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToDirector.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      626 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToDivisionHead.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToExtraordinaryBudget.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      608 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToOfficeManager.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      638 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToServiceHead.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)    45487 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/spinner.gif
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.529285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_styles/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1276 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_styles/meetingmons.css
+-rw-rw-r--   0 adu       (1000) adu       (1000)      344 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_styles/readme.txt
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.529285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      617 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/checkFDAdviceIsTimedOut.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7590 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_edit.pt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     9182 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_old_edit.pt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    36740 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_old_view.pt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    39817 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_view.pt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1701 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/updateOldAssemblies.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1100 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/testing.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      639 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/testing.zcml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.533285 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     1564 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/MeetingMonsTestCase.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1047 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5578 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/helpers.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1337 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testAdvices.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1632 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testAnnexes.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1320 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testChangeItemOrderView.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1213 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testColumns.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5136 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testCustomMeetingItem.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     8349 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testCustomWorkflows.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1246 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testFaceted.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1276 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testMeeting.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1297 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testMeetingCategory.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1646 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testMeetingConfig.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     1420 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testMeetingItem.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1259 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testPortlets.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2381 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testSearches.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1250 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testSetup.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1393 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testToolPloneMeeting.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1203 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testUtils.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1262 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testValidators.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1208 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testViews.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2743 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testWFAdaptations.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)    11545 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testWorkflows.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)       56 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-07-07 08:42:03.517284 Products.MeetingMons-4.2.0b3/src/Products.MeetingMons.egg-info/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7054 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products.MeetingMons.egg-info/PKG-INFO
+-rw-rw-r--   0 adu       (1000) adu       (1000)     8959 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products.MeetingMons.egg-info/SOURCES.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products.MeetingMons.egg-info/dependency_links.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products.MeetingMons.egg-info/namespace_packages.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products.MeetingMons.egg-info/not-zip-safe
+-rw-rw-r--   0 adu       (1000) adu       (1000)      234 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products.MeetingMons.egg-info/requires.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-07-07 08:42:03.000000 Products.MeetingMons-4.2.0b3/src/Products.MeetingMons.egg-info/top_level.txt
```

### Comparing `Products.MeetingMons-4.2.0b2/CHANGES.rst` & `Products.MeetingMons-4.2.0b3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 Products.MeetingMons Changelog
 ==============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingMons/tags/
 The Products.MeetingMons version must be the same as the Products.PloneMeeting version
 
 
+4.2.0b3 (2023-07-07)
+--------------------
+
+- Fixed bad import and remove useless override.
+  [aduchene]
+
+
 4.2.0b2 (2023-07-07)
 --------------------
 
 - Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
   [gbastien]
 - Inherit from MeetingCommunes browser views
   [aduchene]
```

### Comparing `Products.MeetingMons-4.2.0b2/PKG-INFO` & `Products.MeetingMons-4.2.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingMons
-Version: 4.2.0b2
+Version: 4.2.0b3
 Summary: Official meetings management for college and council of Mons (PloneMeeting extension profile)
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: 
 Author-email: 
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -42,14 +42,21 @@
 Products.MeetingMons Changelog
 ==============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingMons/tags/
 The Products.MeetingMons version must be the same as the Products.PloneMeeting version
 
 
+4.2.0b3 (2023-07-07)
+--------------------
+
+- Fixed bad import and remove useless override.
+  [aduchene]
+
+
 4.2.0b2 (2023-07-07)
 --------------------
 
 - Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
   [gbastien]
 - Inherit from MeetingCommunes browser views
   [aduchene]
```

### Comparing `Products.MeetingMons-4.2.0b2/README.rst` & `Products.MeetingMons-4.2.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/docs/LICENSE.GPL` & `Products.MeetingMons-4.2.0b3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/docs/LICENSE.txt` & `Products.MeetingMons-4.2.0b3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/setup.py` & `Products.MeetingMons-4.2.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = '4.2.0b2'
+version = '4.2.0b3'
 
 setup(name='Products.MeetingMons',
       version=version,
       description="Official meetings management for college and council of Mons (PloneMeeting extension profile)",
       long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
       classifiers=[
         "Environment :: Web Environment",
```

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/Extensions/plonemeeting_portal_helpers.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/Extensions/plonemeeting_portal_helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/__init__.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/adapters.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/adapters.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/browser/configure.zcml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/browser/configure.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,23 @@
         layer="Products.PloneMeeting.interfaces.IPloneMeetingLayer"
         permission="zope2.View" />
 
 
     <!-- collective.documentgenerator helper view for MeetingItem -->
     <browser:page
         for="Products.PloneMeeting.interfaces.IMeetingItem"
-        class=".overrides.MCItemDocumentGenerationHelperView"
+        class=".overrides.MonsItemDocumentGenerationHelperView"
         permission="zope2.View"
         layer="Products.MeetingMons.interfaces.IMeetingMonsLayer"
         name="document_generation_helper_view"
      />
 
     <!-- collective.documentgenerator helper view for Meeting -->
     <browser:page
         for="Products.PloneMeeting.content.meeting.IMeeting"
-        class=".overrides.MCMeetingDocumentGenerationHelperView"
+        class=".overrides.MonsMeetingDocumentGenerationHelperView"
         permission="zope2.View"
         layer="Products.MeetingMons.interfaces.IMeetingMonsLayer"
         name="document_generation_helper_view"
      />
 
 </configure>
```

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/browser/overrides.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/browser/overrides.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 #
 # Copyright (c) 2016 by Imio.be
 #
 # GNU General Public License (GPL)
 #
 from collections import OrderedDict
 
-from Products.MeetingCommunes.browser.overrides import FolderDocumentGenerationHelperView
-from Products.MeetingCommunes.browser.overrides import ItemDocumentGenerationHelperView
-from Products.MeetingCommunes.browser.overrides import MeetingDocumentGenerationHelperView
+from Products.MeetingCommunes.browser.overrides import MCItemDocumentGenerationHelperView
+from Products.MeetingCommunes.browser.overrides import MCMeetingDocumentGenerationHelperView
 from imio.history.utils import getLastWFAction as getLastEvent
 from Products.PloneMeeting.utils import get_annexes
 
 from Products.CMFPlone.utils import safe_unicode
 from plone import api
 from plone.api.validation import mutually_exclusive_parameters
 
@@ -54,15 +53,15 @@
         res[-1] = res[-1].replace('<br />', '')
     else:
         return ''
     res.append('</p>')
     return ('\n'.join(res))
 
 
-class MCItemDocumentGenerationHelperView(ItemDocumentGenerationHelperView):
+class MonsItemDocumentGenerationHelperView(MCItemDocumentGenerationHelperView):
     """Specific printing methods used for item."""
 
     def printAllAnnexes(self, portal_types=['annex']):
         ''' Printing Method use in templates :
             return all viewable annexes for item '''
         res = []
         annexes = get_annexes(self.context, portal_types=portal_types)
@@ -285,15 +284,15 @@
         return res
 
     def get_creator_and_validator(self):
         res = {'creator': self.print_creator_name(), 'validator': self.print_validator_name()}
         return res
 
 
-class MCMeetingDocumentGenerationHelperView(MeetingDocumentGenerationHelperView):
+class MonsMeetingDocumentGenerationHelperView(MCMeetingDocumentGenerationHelperView):
     """Specific printing methods used for meeting."""
 
     def printFormatedMeetingAssembly(self, focus=''):
         ''' Printing Method use in templates :
             return formated assembly with 'absent', 'excused', ... '''
         if focus not in ('present', 'excuse', 'absent'):
             return ''
@@ -473,27 +472,8 @@
                 #last level
                 else:
                     keyid = '<h{0}>{1}</h{0}>'.format(i+1, category.Title())
                     if keyid not in res:
                          res[keyid] = []
                     res_key = keyid
             res[res_key].append(('{0}.{1}'.format(category_id, len(res[res_key])+1), item)) # start numbering to 1
-        return res
-
-
-class MCFolderDocumentGenerationHelperView(FolderDocumentGenerationHelperView):
-
-    def get_all_items_dghv_with_finance_advice(self, brains):
-        """
-        :param brains: the brains collection representing @Product.PloneMeeting.MeetingItem
-        :return: an array of dictionary with onnly the items linked to a finance advics which contains 2 keys
-                 itemView : the documentgenerator helper view of a MeetingItem.
-                 advice   : the data from a single advice linked to this MeetingItem as extracted with getAdviceDataFor.
-        """
-        res = []
-
-        tool = api.portal.get_tool('portal_plonemeeting')
-        cfg = tool.getMeetingConfig(self.context)
-        finance_advice_ids = cfg.adapted().getUsedFinanceGroupIds()
-        if finance_advice_ids:
-            res = self.get_all_items_dghv_with_advice(brains, finance_advice_ids)
         return res
```

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/browser/views.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/browser/views.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/config.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/config.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/configure.zcml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/interfaces.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/PloneMeeting.pot` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/PloneMeeting.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/fr/LC_MESSAGES/imio.history.po` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/imio.actionspanel.pot` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/imio.history.pot` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/locales/plone.pot` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/migrations/migrate_to_4200.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/migrations/migrate_to_4200.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/migrations/migrate_to_4_1.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/migrations/migrate_to_4_1.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/model/MeetingMons.zargo` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/model/MeetingMons.zargo`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/model/generate.conf` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/model/generate.conf`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/model/pm_updates.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/model/pm_updates.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/overrides.zcml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/cssregistry.xml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/import_steps.xml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/skins.xml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/workflows/meetingcollegemons_workflow/definition.xml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/workflows/meetingcollegemons_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/workflows/meetingitemcollegemons_workflow/definition.xml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/workflows/meetingitemcollegemons_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/default/workflows.xml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/attach.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/budget.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/cahier.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/financialAnalysis.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/legalAdvice.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/negative.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/overheadAnalysis.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/positive.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/images/remarks.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/import_data.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/import_steps.xml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/Agenda.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/Agenda.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/Decisions.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/Decisions.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/Item.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/Item.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/college-oj-avec-annexes.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/college-oj-avec-annexes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/college-oj.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/college-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/college-pv.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/college-pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/council-oj.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/council-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/council-pv.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/council-pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/council-rapport.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/council-rapport.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/deliberation.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/projet-deliberation.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/projet-deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/mons/templates/synthese cdld.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/mons/templates/synthese cdld.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/attach.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/budget.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/cahier.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/financialAnalysis.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/images/positive.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/import_data.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/import_steps.xml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/templates/Agenda.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/templates/Agenda.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/templates/Decisions.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/templates/Decisions.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles/testing/templates/Item.odt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles/testing/templates/Item.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/profiles.zcml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/setuphandlers.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_cautious_finance.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_cautious_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_negative_finance.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_negative_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_not_required_finance.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_not_required_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_positive_finance.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_positive_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_positive_with_remarks_finance.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/advice_standard_positive_with_remarks_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToBudgetImpactReviewer.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToBudgetImpactReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToDirector.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToDirector.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToDivisionHead.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToDivisionHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToExtraordinaryBudget.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToExtraordinaryBudget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToOfficeManager.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToOfficeManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/proposeToServiceHead.png` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/proposeToServiceHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_images/spinner.gif` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_images/spinner.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_styles/meetingmons.css` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_styles/meetingmons.css`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/checkFDAdviceIsTimedOut.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/checkFDAdviceIsTimedOut.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_edit.pt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_old_edit.pt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_old_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_old_view.pt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_old_view.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_view.pt` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/meetingitem_view.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/skins/meetingmons_templates/updateOldAssemblies.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/skins/meetingmons_templates/updateOldAssemblies.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/testing.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/testing.zcml` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/MeetingMonsTestCase.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/MeetingMonsTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/__init__.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/helpers.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testAdvices.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testAnnexes.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testChangeItemOrderView.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testColumns.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testCustomMeetingItem.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testCustomMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testCustomWorkflows.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testCustomWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testFaceted.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testMeeting.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testMeetingCategory.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testMeetingConfig.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testMeetingItem.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testPortlets.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testSearches.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testSetup.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testToolPloneMeeting.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testUtils.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testValidators.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testViews.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testWFAdaptations.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testWFAdaptations.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products/MeetingMons/tests/testWorkflows.py` & `Products.MeetingMons-4.2.0b3/src/Products/MeetingMons/tests/testWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingMons-4.2.0b2/src/Products.MeetingMons.egg-info/PKG-INFO` & `Products.MeetingMons-4.2.0b3/src/Products.MeetingMons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingMons
-Version: 4.2.0b2
+Version: 4.2.0b3
 Summary: Official meetings management for college and council of Mons (PloneMeeting extension profile)
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: 
 Author-email: 
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -42,14 +42,21 @@
 Products.MeetingMons Changelog
 ==============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingMons/tags/
 The Products.MeetingMons version must be the same as the Products.PloneMeeting version
 
 
+4.2.0b3 (2023-07-07)
+--------------------
+
+- Fixed bad import and remove useless override.
+  [aduchene]
+
+
 4.2.0b2 (2023-07-07)
 --------------------
 
 - Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
   [gbastien]
 - Inherit from MeetingCommunes browser views
   [aduchene]
```

### Comparing `Products.MeetingMons-4.2.0b2/src/Products.MeetingMons.egg-info/SOURCES.txt` & `Products.MeetingMons-4.2.0b3/src/Products.MeetingMons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

