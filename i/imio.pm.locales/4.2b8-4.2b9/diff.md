# Comparing `tmp/imio.pm.locales-4.2b8.tar.gz` & `tmp/imio.pm.locales-4.2b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.pm.locales-4.2b8.tar", last modified: Thu Jan 14 08:26:23 2021, max compression
+gzip compressed data, was "dist/imio.pm.locales-4.2b9.tar", last modified: Fri Jul 16 07:24:57 2021, max compression
```

## Comparing `imio.pm.locales-4.2b8.tar` & `imio.pm.locales-4.2b9.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1247 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/dev.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      190 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/svn.ignore
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       72 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22555 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/PKG-INFO
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22555 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5711 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       37 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       47 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/not-zip-safe
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      317 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      673 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.iconifiedcategory.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1478 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/README.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1567 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/eea.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3099 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.documentgenerator.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1076 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.behavior.talcondition.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      926 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.eeafaceted.batchactions.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      770 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.iconifiedcategory.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2965 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.eeafaceted.z3ctable.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16139 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/datagridfield.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   241503 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.contact.core.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2905 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24842 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7013 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      547 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.annex.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2818 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/imio.history.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3101 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.eeafaceted.z3ctable.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1066 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.eeafaceted.batchactions.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      729 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.contact.core.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1567 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/eea.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3099 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.documentgenerator.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1076 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.behavior.talcondition.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      926 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.eeafaceted.batchactions.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      770 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.iconifiedcategory.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2965 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.eeafaceted.z3ctable.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16204 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/datagridfield.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   261313 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.contact.core.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2905 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25006 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7651 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      547 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.annex.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1214 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.behavior.talcondition.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16011 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/datagridfield.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4852 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/imio.actionspanel.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23213 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/plone.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1433 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/eea.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1922 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/eea.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5498 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.documentgenerator.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1498 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.behavior.talcondition.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1122 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      878 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3636 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    27102 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/datagridfield.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   373321 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      821 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.contact.core.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4364 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30967 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7986 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      572 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.annex.po
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)       60 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/merge_generated.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3234 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.documentgenerator.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1918 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/eea.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5257 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.documentgenerator.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1444 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.behavior.talcondition.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1063 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      834 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.iconifiedcategory.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3470 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24194 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/datagridfield.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   340344 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.contact.core.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4178 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28894 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7437 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      563 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.annex.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   224680 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/PloneMeeting.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1567 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/eea.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3099 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.documentgenerator.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1076 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.behavior.talcondition.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      926 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.eeafaceted.batchactions.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      770 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.iconifiedcategory.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2965 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.eeafaceted.z3ctable.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19842 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/datagridfield.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   278813 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.contact.core.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2905 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26830 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7997 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      547 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.annex.po
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      582 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/sync_pos.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      416 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/src/imio/pm/locales/locales/imio.annex.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9674 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/ez_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/MANIFEST.in
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3070 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/base.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/versions-dev.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1407 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5706 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/bootstrap.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      166 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/versions-base.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18069 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/CHANGES.rst
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      119 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/buildout.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      383 2021-01-14 08:26:23.000000 imio.pm.locales-4.2b8/Makefile
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      166 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/versions-base.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      317 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      547 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.annex.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26894 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1076 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.behavior.talcondition.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   279558 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7997 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.contact.core.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3952 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      770 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.iconifiedcategory.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      926 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.eeafaceted.batchactions.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22584 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/datagridfield.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3099 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.documentgenerator.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1620 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/eea.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2905 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1214 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.behavior.talcondition.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2818 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/imio.history.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   228131 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/PloneMeeting.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1486 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/eea.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4088 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.eeafaceted.z3ctable.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      563 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.annex.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    28958 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1444 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.behavior.talcondition.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   346815 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7437 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.contact.core.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4367 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      834 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.iconifiedcategory.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1063 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26936 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/datagridfield.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5257 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.documentgenerator.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1971 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/eea.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4178 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23268 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/plone.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4852 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/imio.actionspanel.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18753 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/datagridfield.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      673 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.iconifiedcategory.pot
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)       60 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/merge_generated.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      416 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/imio.annex.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      547 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.annex.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25070 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1076 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.behavior.talcondition.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   263217 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7651 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.contact.core.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3952 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      770 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.iconifiedcategory.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      926 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.eeafaceted.batchactions.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18946 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/datagridfield.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3099 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.documentgenerator.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1620 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/eea.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2905 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1066 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.eeafaceted.batchactions.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3234 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.documentgenerator.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      729 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.contact.core.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1478 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/README.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      572 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.annex.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    31033 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1498 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.behavior.talcondition.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   380223 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7986 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      821 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.contact.core.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4968 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      878 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1115 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    31668 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/datagridfield.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5498 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.documentgenerator.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1985 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/eea.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4364 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.history.po
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      582 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/sync_pos.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      547 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.annex.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24906 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1076 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.behavior.talcondition.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   244475 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7013 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.contact.core.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3952 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      770 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.iconifiedcategory.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      926 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.eeafaceted.batchactions.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18881 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/datagridfield.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3099 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.documentgenerator.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1620 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/eea.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2905 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/locales/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/pm/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       37 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26306 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5711 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       47 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/requires.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1247 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/dev.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/versions-dev.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5706 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/bootstrap.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9674 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/ez_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1407 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26306 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21268 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/CHANGES.rst
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3070 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/base.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       72 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      190 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/svn.ignore
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      383 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/Makefile
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2021-07-16 07:24:57.000000 imio.pm.locales-4.2b9/setup.cfg
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      119 2021-07-16 07:24:56.000000 imio.pm.locales-4.2b9/buildout.cfg
```

### Comparing `imio.pm.locales-4.2b8/dev.cfg` & `imio.pm.locales-4.2b9/dev.cfg`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/PKG-INFO` & `imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.pm.locales
-Version: 4.2b8
+Version: 4.2b9
 Summary: Locales for PloneMeeting
 Home-page: https://github.com/IMIO/imio.pm.locales
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL
 Description: README.rst
         ==========
@@ -12,14 +12,83 @@
         These are the locales for Products.PloneMeeting
         
         
         Changelog
         =========
         
         
+        4.2b9 (2021-07-16)
+        ------------------
+        
+        - Added translations for `Not completed votes` and `Completed votes`.
+          [gbastien]
+        - Removed single quotes for `meeting_state_changed_default_mail_body`.
+          [aduchene]
+        - Added translations now that `Preferred meeting date` column is abbreviated.
+          [gbastien]
+        - Renamed msgid `You cannot delete the default item template, but you can deactivate it if necessary!` to
+          `You cannot delete or move the default item template, but you can deactivate it if necessary!`.
+          [gbastien]
+        - Added translations for `copy_groups_help_msg`.
+          [gbastien]
+        - Adapted translations now that Meeting was moved from AT to DX.
+          [gbastien]
+        - Added translations regarding the `Committees` management.
+          [gbastien]
+        - Changed default translation for `move_item_to_given_position`.
+          [gbastien]
+        - Added translations for annexes faceted filter vocabulary.
+          [gbastien]
+        - Added translation for `required_groupsInCharge_ko`.
+          [gbastien]
+        - Include `item_url` in `holidays_removed_date_in_use_error` translation.
+          [gbastien]
+        - Added translation related to advice behavior that changed (delay no more reinitialized for a given advice).
+          [gbastien]
+        - Removed msgids beginning with `list_type_` in the `PloneMeeting` domain, seem no more used.
+          [gbastien]
+        - Added translations related to `Redefine attendee position on item`.
+          [gbastien]
+        - Changed translation for `no_shown_items` from `No visible item for now.`
+          to `You do not have access to these items.`.
+          [gbastien]
+        - Added translation for warning displayed on the meeting view when `assembly/signatures` are not correct.
+          [gbastien]
+        - More accurate translation for `Meeting.meeting_number` and `Meeting.first_item_number`
+          description, explaining it is managed by the application.
+          [gbastien]
+        - Added translations for new static columns selectable in `MeetingConfig.meetingColumns`.
+          [gbastien]
+        - Added translations for `not_confidential_annexes`.
+          [gbastien]
+        - Added translations for `Read more/Read less`, removed useless translation
+          `This is an extract of the comment, access full comment if necessary...`.
+          [gbastien]
+        - Added translation for `marginal_notes_column`.
+          [gbastien]
+        - Added translation for `not_able_to_find_meeting_to_present_item_into`.
+          [gbastien]
+        - Added translations for `error_default_poll_type_must_be_among_used_poll_types`,
+          `error_first_linked_vote_used_vote_values_must_be_among_used_vote_values` and
+          `error_next_linked_votes_used_vote_values_must_be_among_used_vote_values`.
+          [gbastien]
+        - Added translation for `title_meetingmanagers_notes`.
+          [gbastien]
+        - Added translation for `MeetingConfig.enabledAnnexesBatchActions`.
+          [gbastien]
+        - Adapted translations for `MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup`
+          and `MeetingConfig.includeGroupsInChargeDefinedOnCategory` fields description
+          now that, when enabled, selected `groupsInCharge` will be stored on the item.
+          [gbastien]
+        - Completed french translation for the help message about copy groups on the item view.
+          [gbastien]
+        - Added translations for `MeetingConfig.selectableRedefinedPositionTypes` and
+          `directory.position_types` invariant `removed_redefined_position_type_in_use_error` error message.
+          [gbastien]
+        
         4.2b8 (2021-01-14)
         ------------------
         
         - Accurate french translation for `Position type to use as label for the signature.`.
           [gbastien]
         
         4.2b7 (2021-01-06)
```

### Comparing `imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/PKG-INFO` & `imio.pm.locales-4.2b9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.pm.locales
-Version: 4.2b8
+Version: 4.2b9
 Summary: Locales for PloneMeeting
 Home-page: https://github.com/IMIO/imio.pm.locales
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL
 Description: README.rst
         ==========
@@ -12,14 +12,83 @@
         These are the locales for Products.PloneMeeting
         
         
         Changelog
         =========
         
         
+        4.2b9 (2021-07-16)
+        ------------------
+        
+        - Added translations for `Not completed votes` and `Completed votes`.
+          [gbastien]
+        - Removed single quotes for `meeting_state_changed_default_mail_body`.
+          [aduchene]
+        - Added translations now that `Preferred meeting date` column is abbreviated.
+          [gbastien]
+        - Renamed msgid `You cannot delete the default item template, but you can deactivate it if necessary!` to
+          `You cannot delete or move the default item template, but you can deactivate it if necessary!`.
+          [gbastien]
+        - Added translations for `copy_groups_help_msg`.
+          [gbastien]
+        - Adapted translations now that Meeting was moved from AT to DX.
+          [gbastien]
+        - Added translations regarding the `Committees` management.
+          [gbastien]
+        - Changed default translation for `move_item_to_given_position`.
+          [gbastien]
+        - Added translations for annexes faceted filter vocabulary.
+          [gbastien]
+        - Added translation for `required_groupsInCharge_ko`.
+          [gbastien]
+        - Include `item_url` in `holidays_removed_date_in_use_error` translation.
+          [gbastien]
+        - Added translation related to advice behavior that changed (delay no more reinitialized for a given advice).
+          [gbastien]
+        - Removed msgids beginning with `list_type_` in the `PloneMeeting` domain, seem no more used.
+          [gbastien]
+        - Added translations related to `Redefine attendee position on item`.
+          [gbastien]
+        - Changed translation for `no_shown_items` from `No visible item for now.`
+          to `You do not have access to these items.`.
+          [gbastien]
+        - Added translation for warning displayed on the meeting view when `assembly/signatures` are not correct.
+          [gbastien]
+        - More accurate translation for `Meeting.meeting_number` and `Meeting.first_item_number`
+          description, explaining it is managed by the application.
+          [gbastien]
+        - Added translations for new static columns selectable in `MeetingConfig.meetingColumns`.
+          [gbastien]
+        - Added translations for `not_confidential_annexes`.
+          [gbastien]
+        - Added translations for `Read more/Read less`, removed useless translation
+          `This is an extract of the comment, access full comment if necessary...`.
+          [gbastien]
+        - Added translation for `marginal_notes_column`.
+          [gbastien]
+        - Added translation for `not_able_to_find_meeting_to_present_item_into`.
+          [gbastien]
+        - Added translations for `error_default_poll_type_must_be_among_used_poll_types`,
+          `error_first_linked_vote_used_vote_values_must_be_among_used_vote_values` and
+          `error_next_linked_votes_used_vote_values_must_be_among_used_vote_values`.
+          [gbastien]
+        - Added translation for `title_meetingmanagers_notes`.
+          [gbastien]
+        - Added translation for `MeetingConfig.enabledAnnexesBatchActions`.
+          [gbastien]
+        - Adapted translations for `MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup`
+          and `MeetingConfig.includeGroupsInChargeDefinedOnCategory` fields description
+          now that, when enabled, selected `groupsInCharge` will be stored on the item.
+          [gbastien]
+        - Completed french translation for the help message about copy groups on the item view.
+          [gbastien]
+        - Added translations for `MeetingConfig.selectableRedefinedPositionTypes` and
+          `directory.position_types` invariant `removed_redefined_position_type_in_use_error` error message.
+          [gbastien]
+        
         4.2b8 (2021-01-14)
         ------------------
         
         - Accurate french translation for `Position type to use as label for the signature.`.
           [gbastien]
         
         4.2b7 (2021-01-06)
```

### Comparing `imio.pm.locales-4.2b8/src/imio.pm.locales.egg-info/SOURCES.txt` & `imio.pm.locales-4.2b9/src/imio.pm.locales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.iconifiedcategory.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.iconifiedcategory.pot`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/README.txt` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/README.txt`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/eea.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/eea.po`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 
 msgid "Category"
 msgstr ""
 
 msgid "Classifier"
 msgstr ""
 
+#. Default: "Committee"
+msgid "Committee"
+msgstr ""
+
 #. Default: "Copy groups"
 msgid "Copy groups"
 msgstr ""
 
 msgid "Created"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.documentgenerator.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.documentgenerator.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.behavior.talcondition.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.behavior.talcondition.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.eeafaceted.batchactions.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.eeafaceted.batchactions.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.iconifiedcategory.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.iconifiedcategory.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.eeafaceted.z3ctable.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po`

 * *Files 24% similar despite different names*

```diff
@@ -10,130 +10,174 @@
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: DOMAIN\n"
 
+#. Default: "Approval date (in the 'Title' column)"
+msgid "approval_date_column"
+msgstr ""
+
+#. Default: "Authority notice (in the 'Title' column)"
+msgid "authority_notice_column"
+msgstr ""
+
 #. Default: "Budgetary informations (in the 'Purpose' column)"
 msgid "budget_infos_column"
+msgstr "Budgetary informations (in the 'Purpose' column)"
+
+#. Default: "Convocation date (in the 'Title' column)"
+msgid "convocation_date_column"
 msgstr ""
 
 #. Default: "End date (in the 'Title' column)"
-msgid "endDate_column"
+msgid "end_date_column"
+msgstr ""
+
+#. Default: "First item number (in the 'Title' column)"
+msgid "first_item_number_column"
 msgstr ""
 
 #. Default: "Advices"
 msgid "header_advices"
-msgstr ""
+msgstr "Advices"
 
 #. Default: "Associated groups acronym"
 msgid "header_associated_groups_acronym"
-msgstr ""
+msgstr "Associated groups acronym"
 
 #. Default: "Associated groups acronym help"
 msgid "header_associated_groups_acronym_help"
 msgstr ""
 
+#. Default: "Committees"
+msgid "header_committees_index"
+msgstr ""
+
+#. Default: "Committees acronym"
+msgid "header_committees_index_acronym"
+msgstr ""
+
+#. Default: "Committees acronym help"
+msgid "header_committees_index_acronym_help"
+msgstr ""
+
 #. Default: "Associated groups"
 msgid "header_getAssociatedGroups"
-msgstr ""
+msgstr "Associated groups"
 
 #. Default: "Associated groups help"
 msgid "header_getAssociatedGroups_help"
 msgstr ""
 
 #. Default: "Category"
 msgid "header_getCategory"
-msgstr ""
+msgstr "Category"
 
 #. Default: "Groups in charge"
 msgid "header_getGroupsInCharge"
-msgstr ""
+msgstr "Groups in charge"
 
 #. Default: "Groups in charge help"
 msgid "header_getGroupsInCharge_help"
 msgstr ""
 
 #. Default: "Item is signed?"
 msgid "header_getItemIsSigned"
-msgstr ""
+msgstr "Item is signed?"
 
 #. Default: "&nbsp;&nbsp;&nbsp;"
 msgid "header_getItemNumber"
-msgstr ""
-
-#. Default: "Preferred meeting"
-msgid "header_getPreferredMeetingDate"
-msgstr ""
+msgstr " "
 
 #. Default: "Proposing group"
 msgid "header_getProposingGroup"
-msgstr ""
+msgstr "Proposing group"
 
 #. Default: "Proposing group help"
 msgid "header_getProposingGroup_help"
 msgstr ""
 
 #. Default: "Classifier"
 msgid "header_getRawClassifier"
-msgstr ""
+msgstr "Classifier"
 
 #. Default: "Groups in charge acronym"
 msgid "header_groups_in_charge_acronym"
-msgstr ""
+msgstr "Groups in charge acronym"
 
 #. Default: "Groups in charge acronym help"
 msgid "header_groups_in_charge_acronym_help"
 msgstr ""
 
 #. Default: "Meeting"
-msgid "header_linkedMeetingDate"
+msgid "header_meeting_date"
 msgstr ""
 
 #. Default: "Poll type"
 msgid "header_pollType"
+msgstr "Poll type"
+
+#. Default: "P. meeting"
+msgid "header_preferred_meeting_date"
+msgstr ""
+
+#. Default: "Preferred meeting"
+msgid "header_preferred_meeting_date_help"
 msgstr ""
 
 #. Default: "Privacy"
 msgid "header_privacy"
-msgstr ""
+msgstr "Privacy"
 
 #. Default: "Proposing group acronym"
 msgid "header_proposing_group_acronym"
-msgstr ""
+msgstr "Proposing group acronym"
 
 #. Default: "Proposing group acronym help"
 msgid "header_proposing_group_acronym_help"
 msgstr ""
 
 #. Default: "Purpose"
 msgid "header_purpose"
-msgstr ""
+msgstr "Purpose"
 
 #. Default: "Review state"
 msgid "header_review_state_title"
-msgstr ""
+msgstr "Review state"
 
 #. Default: "Review state title (will use review state title and not id)"
 msgid "header_review_state_title_descr"
-msgstr ""
+msgstr "Review state title (will use review state title and not id)"
 
 #. Default: "To discuss?"
 msgid "header_toDiscuss"
-msgstr ""
+msgstr "To discuss?"
 
 #. Default: "Item reference (in the 'Purpose' column)"
 msgid "item_reference_column"
-msgstr ""
+msgstr "Item reference (in the 'Purpose' column)"
 
 #. Default: "Labels (in the 'Purpose' column)"
 msgid "labels_column"
+msgstr "Labels (in the 'Purpose' column)"
+
+#. Default: "Marginal notes (in the 'Purpose' column)"
+msgid "marginal_notes_column"
+msgstr ""
+
+#. Default: "Meeting number (in the 'Title' column)"
+msgid "meeting_number_column"
 msgstr ""
 
 #. Default: "Place (in the 'Title' column)"
 msgid "place_column"
+msgstr "Place (in the 'Title' column)"
+
+#. Default: "Place other (in the 'Title' column)"
+msgid "place_other_column"
 msgstr ""
 
 #. Default: "Start date (in the 'Title' column)"
-msgid "startDate_column"
+msgid "start_date_column"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/datagridfield.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/datagridfield.pot`

 * *Files 4% similar despite different names*

```diff
@@ -1,367 +1,444 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: PloneMeeting\n"
 "POT-Creation-Date: 2014-01-09 12:30-100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
-"Domain: DOMAIN\n"
+"Domain: datagridfield\n"
 
-#. Default: "Available on"
-msgid "Available on"
+#. Default: "Identifier (row_id)"
+msgid "Custom adviser row id"
 msgstr ""
 
-#. Default: "Full label"
-msgid "Config group full label"
+#. Default: "Organization"
+msgid "Custom adviser organization"
 msgstr ""
 
-#. Default: "Label"
-msgid "Config group label"
+#. Default: "Advice will be automatically asked if"
+msgid "Custom adviser gives automatic advice on"
 msgstr ""
 
-#. Default: "Identifier (row_id)"
-msgid "Config group row id"
+#. Default: "Specify here a TAL expression that will return True if the advice of the group must be automatically asked on an item.  We receive \"item\" as the meeting item to give an advice on, \"org\" and \"org_uid\" as the organization (organization UID) that will have to give the advice.  WARNING if the group of advisers linked to this group is empty, it will no be considered, despite the result of the TAL expression.  This advice will NOT be askable manually in the user interface, it is only asked automatically by the application.  If this advice should not be asked automatically, leave this field blank."
+msgid "gives_auto_advice_on_col_description"
 msgstr ""
 
-#. Default: "Advice with delay label"
-msgid "Custom adviser delay label"
+#. Default: "Automatic asked advice help message"
+msgid "Custom adviser gives automatic advice on help message"
 msgstr ""
 
-#. Default: "Advice will be automatically asked if"
-msgid "Custom adviser gives automatic advice on"
+#. Default: "If you want a specific help message to be displayed on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The message will appear between brackets after the message \"This advice has been automatically asked by the application\"."
+msgid "gives_auto_advice_on_help_message_col_description"
 msgstr ""
 
-#. Default: "Automatic asked advice help message"
-msgid "Custom adviser gives automatic advice on help message"
+#. Default: "Rule activated for item created from"
+msgid "Rule activated for item created from"
 msgstr ""
 
-#. Default: "Organization"
-msgid "Custom adviser organization"
+#. Default: "This configuration will be applied on item created from the defined date (defined date included).  Please respect following format : YYYY/MM/DD (year 4 digits/month 2 digits/day 2 digits).  This date will avoid older items created before to be affected, especially when updating every advices thru the \"Update all advices\" action."
+msgid "for_item_created_from_col_description"
 msgstr ""
 
-#. Default: "Identifier (row_id)"
-msgid "Custom adviser row id"
+#. Default: "Rule activated for item created until"
+msgid "Rule activated for item created until"
+msgstr ""
+
+#. Default: "This configuration will be applied on item created until the defined date (defined date must be in the future and will not be included).  Please respect following format : YYYY/MM/DD (year 4 digits/month 2 digits/day 2 digits).  This date will avoid newer items created after to be affected, especially when updating every advices thru the \"Update all advices\" action. This date will be only settable once, when set, this can not be changed anymore."
+msgid "for_item_created_until_col_description"
 msgstr ""
 
 #. Default: "Delay for giving advice"
 msgid "Delay for giving advice"
 msgstr ""
 
+#. Default: "Enter the delay the adviser will have to give his advice. If it is not considered as an automatically asked advice (nothing defined in the \"Advice will be automatically asked if\" column), the advice will be selectable in the \"Ask advice to\" list on the item edit form. A delay is a single digit (like \"5\" or \"10\"). If no delay is relevant for this advice, leave this field blank. If several delays are possible for the same advice, you have to define several rows with exactly the same content excepted the delay."
+msgid "delay_col_description"
+msgstr ""
+
 #. Default: "Delay left alert"
 msgid "Delay left alert"
 msgstr ""
 
-#. Default: "Enter a short label that will be displayed in the application.  This will be translated by the application if possible.  If you want to colorize this new list type on the meeting view, you will need to do this using CSS like it is the case for \"late\" items."
-msgid "Enter a short label that will be displayed in the application.  This will be translated by the application if possible.  If you want to colorize this new list type on the meeting view, you will need to do this using CSS like it is the case for 'late' items."
+#. Default: "Enter the treshold beyond wich an alert must be shown regarding left delay.  This will be shown in the UI with a particular color and if activated, a mail notification could be send in this case. Enter a single digit (like \"5\" or \"10\") lower than actual \"Delay\". If no treshold is relevant for this advice, leave this field blank."
+msgid "delay_left_alert_col_description"
 msgstr ""
 
-#. Default: "Enter an internal identifier, use only lowercase letters."
-msgid "Enter an internal identifier, use only lowercase letters."
+#. Default: "Available on"
+msgid "Available on"
 msgstr ""
 
-#. Default: "Enter the full label that will be useable if necessary like in produced documents."
-msgid "Enter the full label that will be useable if necessary like in produced documents."
+#. Default: "Specify here a TAL expression that will restrict or allow the use of this advice to some condition.  We receive \"item\" as the meeting item to give an advice on and \"mayEdit\", a boolean to know if current user may edit the item.  A special expression is available to protect a row that should only be available thru the \"Change delay\" action, it is : \"python: item.REQUEST.get('managing_available_delays', False)\".  This can not be used if something is defined in the \"Advice will be automatically asked if\" column of this advice, but for optional delay-aware advice or for delay-aware advices linked to an automatic advice (using the \"Is linked to previous row?\" column)"
+msgid "available_on_col_description"
 msgstr ""
 
-#. Default: "Enter the label that will be displayed in the application."
-msgid "Enter the label that will be displayed in the application."
+#. Default: "Advice with delay label"
+msgid "Custom adviser delay label"
+msgstr ""
+
+#. Default: "If you want a specific label to be displayed on the label displayed in the \"Advice to give\" list on the item edit form and on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The label will appear between brackets after the message \"Name of the group - delay of X days\"."
+msgid "delay_label_col_description"
+msgstr ""
+
+#. Default: "Meeting config"
+msgid "Meeting config to clone to Meeting config"
+msgstr ""
+
+#. Default: "The meeting config the item of this meeting config will be sendable to."
+msgid "The meeting config the item of this meeting config will be sendable to."
+msgstr ""
+
+#. Default: "Meeting config to clone to Trigger workflow transitions until"
+msgid "Meeting config to clone to Trigger workflow transitions until"
+msgstr ""
+
+#. Default: "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field \"States in which an item will be automatically sent to selected other meeting configurations\" here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the \"Transitions for presenting an item\" you defined in the \"Workflows\" tab of the meeting configuration the item will be sent to."
+msgid "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field 'States in which an item will be automatically sent to selected other meeting configurations' here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the 'Transitions for presenting an item' you defined in the 'Workflows' tab of the meeting configuration the item will be sent to."
 msgstr ""
 
 #. Default: "Date"
 msgid "Holiday date"
 msgstr ""
 
-#. Default: "If the inserting method \"on list types\" is used, will this list type be taken into account while inserting the item in the meeting?"
-msgid "If the inserting method \"on list types\" is used, will this list type be taken into account while inserting the item in the meeting?"
+#. Default: "Please use following format : YYYY/MM/DD.  Dates must be sorted (from older to newer)."
+msgid "holiday_date_col_descr"
 msgstr ""
 
-#. Default: "Inserting method"
-msgid "Inserting method"
+#. Default: "Title"
+msgid "Sub type title"
 msgstr ""
 
-#. Default: "Set to \"Yes\" if you want to make a logical link between a row and the previous one.  This will manage the fact of easily being able to change a delay for an asked advice.  The linked rows will make the user being able to select between those different delays in the advice vizualisation popup.  This is only relevant for delay-aware advices, to link differents delays together."
-msgid "Is linked to previous row description"
+#. Default: "Predefined title"
+msgid "Sub type predefined title"
 msgstr ""
 
-#. Default: "Is linked to previous row?"
-msgid "Is linked to previous row?"
+#. Default: "Correspondences while sent to other meeting configs"
+msgid "Sub type correspondences while sent to other meeting configs"
 msgstr ""
 
-#. Default: "Item WF validation levels back transition"
-msgid "Item WF validation levels back transition"
+#. Default: "Please look the help message of the field \"Correspondences while sent to other meeting configs\" here above.  Simply note that if nothing is defined here, the value defined in the field above will be used."
+msgid "Sub type correspondences while sent to other meeting configs description."
 msgstr ""
 
-#. Default: "Item WF validation levels back transition description."
-msgid "Item WF validation levels back transition description."
+#. Default: "Default value of the \"Confidential ?\" attribute of created annexes"
+msgid "Sub type confidentiality of created annexes"
 msgstr ""
 
-#. Default: "Item WF validation levels back transition title"
-msgid "Item WF validation levels back transition title"
+#. Default: "Please look the help message of the field \"Default value of the 'Confidential ?' attribute of created annexes\" here above.  Simply note that if nothing is defined here, the value defined in the field above will be used."
+msgid "Sub type confidentiality of created annexes description."
 msgstr ""
 
-#. Default: "Item WF validation levels back transition title description."
-msgid "Item WF validation levels back transition title description."
+#. Default: "Active?"
+msgid "Sub type is active?"
 msgstr ""
 
-#. Default: "Item WF validation levels enabled"
-msgid "Item WF validation levels enabled"
+#. Default: "Is linked to previous row?"
+msgid "Is linked to previous row?"
 msgstr ""
 
-#. Default: "Item WF validation levels enabled description."
-msgid "Item WF validation levels enabled description."
+#. Default: "Set to \"Yes\" if you want to make a logical link between a row and the previous one.  This will manage the fact of easily being able to change a delay for an asked advice.  The linked rows will make the user being able to select between those different delays in the advice vizualisation popup.  This is only relevant for delay-aware advices, to link differents delays together."
+msgid "Is linked to previous row description"
 msgstr ""
 
-#. Default: "Item WF validation levels extra suffixes"
-msgid "Item WF validation levels extra suffixes"
+#. Default: "Inserting method"
+msgid "Inserting method"
 msgstr ""
 
-#. Default: "Item WF validation levels extra suffixes description."
-msgid "Item WF validation levels extra suffixes description."
+#. Default: "Select the inserting method, methods will be applied in given order, you can not select twice same inserting method."
+msgid "Select the inserting method, methods will be applied in given order, you can not select twice same inserting method."
 msgstr ""
 
-#. Default: "Item WF validation levels leading transition"
-msgid "Item WF validation levels leading transition"
+#. Default: "Reverse?"
+msgid "Reverse inserting method?"
 msgstr ""
 
-#. Default: "Item WF validation levels leading transition description."
-msgid "Item WF validation levels leading transition description."
+#. Default: "Reverse order of selected inserting method?"
+msgid "Reverse order of selected inserting method?"
 msgstr ""
 
-#. Default: "Item WF validation levels leading transition title"
-msgid "Item WF validation levels leading transition title"
+#. Default: "Transition"
+msgid "On transition field transform transition"
 msgstr ""
 
-#. Default: "Item WF validation levels leading transition title description."
-msgid "Item WF validation levels leading transition title description."
+#. Default: "The transition that will trigger the field transform."
+msgid "The transition that will trigger the field transform."
 msgstr ""
 
-#. Default: "Item WF validation levels state"
-msgid "Item WF validation levels state"
+#. Default: "Field name"
+msgid "On transition field transform field name"
 msgstr ""
 
-#. Default: "Item WF validation levels state description."
-msgid "Item WF validation levels state description."
+#. Default: "The item field that will be transformed."
+msgid "The item field that will be transformed."
 msgstr ""
 
-#. Default: "Item WF validation levels state title"
-msgid "Item WF validation levels state title"
+#. Default: "TAL expression"
+msgid "On transition field transform TAL expression"
 msgstr ""
 
-#. Default: "Item WF validation levels state title description."
-msgid "Item WF validation levels state title description."
+#. Default: "The TAL expression.  Element \"here\" represent the item.  This expression MUST return valid HTML or it will not behave properly on the item."
+msgid "The TAL expression.  Element 'here' represent the item.  This expression MUST return valid HTML or it will not behave properly on the item."
 msgstr ""
 
-#. Default: "Item WF validation levels suffix"
-msgid "Item WF validation levels suffix"
+#. Default: "Transition triggered on the meeting"
+msgid "On meeting transition item action to execute meeting transition"
 msgstr ""
 
-#. Default: "Item WF validation levels suffix description."
-msgid "Item WF validation levels suffix description."
+#. Default: " "
+msgid "The transition triggered on the meeting."
+msgstr ""
+
+#. Default: "Transition to trigger on every items of the meeting"
+msgid "On meeting transition item action to execute item action"
+msgstr ""
+
+#. Default: " "
+msgid "The action that will be executed on every items of the meeting."
+msgstr ""
+
+#. Default: "On meeting transition item action to execute tal expression"
+msgid "On meeting transition item action to execute tal expression"
+msgstr ""
+
+#. Default: " "
+msgid "The action to execute when 'Execute given action' is selected in column 'Item action'."
 msgstr ""
 
 #. Default: "List type identifier"
 msgid "List type identifier"
 msgstr ""
 
+#. Default: "Enter an internal identifier, use only lowercase letters."
+msgid "Enter an internal identifier, use only lowercase letters."
+msgstr ""
+
 #. Default: "List type label"
 msgid "List type label"
 msgstr ""
 
+#. Default: "Enter a short label that will be displayed in the application.  This will be translated by the application if possible.  If you want to colorize this new list type on the meeting view, you will need to do this using CSS like it is the case for \"late\" items."
+msgid "Enter a short label that will be displayed in the application.  This will be translated by the application if possible.  If you want to colorize this new list type on the meeting view, you will need to do this using CSS like it is the case for 'late' items."
+msgstr ""
+
 #. Default: "List type used_in_inserting_method"
 msgid "List type used_in_inserting_method"
 msgstr ""
 
-#. Default: "Meeting config"
-msgid "Meeting config to clone to Meeting config"
+#. Default: "If the inserting method \"on list types\" is used, will this list type be taken into account while inserting the item in the meeting?"
+msgid "If the inserting method \"on list types\" is used, will this list type be taken into account while inserting the item in the meeting?"
 msgstr ""
 
-#. Default: "Meeting config to clone to Trigger workflow transitions until"
-msgid "Meeting config to clone to Trigger workflow transitions until"
+#. Default: "Identifier (row_id)"
+msgid "Config group row id"
 msgstr ""
 
-#. Default: "Transition to trigger on every items of the meeting"
-msgid "On meeting transition item action to execute item action"
+#. Default: "Label"
+msgid "Config group label"
 msgstr ""
 
-#. Default: "Transition triggered on the meeting"
-msgid "On meeting transition item action to execute meeting transition"
+#. Default: "Enter the label that will be displayed in the application."
+msgid "Enter the label that will be displayed in the application."
 msgstr ""
 
-#. Default: "On meeting transition item action to execute tal expression"
-msgid "On meeting transition item action to execute tal expression"
+#. Default: "Full label"
+msgid "Config group full label"
 msgstr ""
 
-#. Default: "TAL expression"
-msgid "On transition field transform TAL expression"
+#. Default: "Enter the full label that will be useable if necessary like in produced documents."
+msgid "Enter the full label that will be useable if necessary like in produced documents."
 msgstr ""
 
-#. Default: "Field name"
-msgid "On transition field transform field name"
+#. Default: "Power observer label"
+msgid "Power observer label"
 msgstr ""
 
-#. Default: "Transition"
-msgid "On transition field transform transition"
+#. Default: "Power observer label description"
+msgid "power_observers_label_col_description"
+msgstr ""
+
+#. Default: "Power observer item viewable states"
+msgid "Power observer item viewable states"
+msgstr ""
+
+#. Default: "Power observer item viewable states description"
+msgid "power_observers_item_states_col_description"
 msgstr ""
 
 #. Default: "Power observer item access TAL expression"
 msgid "Power observer item access TAL expression"
 msgstr ""
 
-#. Default: "Power observer item viewable states"
-msgid "Power observer item viewable states"
+#. Default: "Power observer item access TAL expression description"
+msgid "power_observers_item_access_on_col_description"
 msgstr ""
 
-#. Default: "Power observer label"
-msgid "Power observer label"
+#. Default: "Power observer meeting viewable states"
+msgid "Power observer meeting viewable states"
+msgstr ""
+
+#. Default: "Power observer meeting viewable states description"
+msgid "power_observers_meeting_states_col_description"
 msgstr ""
 
 #. Default: "Power observer meeting access TAL expression"
 msgid "Power observer meeting access TAL expression"
 msgstr ""
 
-#. Default: "Power observer meeting viewable states"
-msgid "Power observer meeting viewable states"
+#. Default: "Power observer meeting access TAL expression description"
+msgid "power_observers_meeting_access_on_col_description"
 msgstr ""
 
-#. Default: "Reverse?"
-msgid "Reverse inserting method?"
+#. Default: "Item WF validation levels state"
+msgid "Item WF validation levels state"
 msgstr ""
 
-#. Default: "Reverse order of selected inserting method?"
-msgid "Reverse order of selected inserting method?"
+#. Default: "Item WF validation levels state description."
+msgid "Item WF validation levels state description."
 msgstr ""
 
-#. Default: "Rule activated for item created from"
-msgid "Rule activated for item created from"
+#. Default: "Item WF validation levels state title"
+msgid "Item WF validation levels state title"
 msgstr ""
 
-#. Default: "Rule activated for item created until"
-msgid "Rule activated for item created until"
+#. Default: "Item WF validation levels state title description."
+msgid "Item WF validation levels state title description."
 msgstr ""
 
-#. Default: "Select the inserting method, methods will be applied in given order, you can not select twice same inserting method."
-msgid "Select the inserting method, methods will be applied in given order, you can not select twice same inserting method."
+#. Default: "Item WF validation levels leading transition"
+msgid "Item WF validation levels leading transition"
 msgstr ""
 
-#. Default: "Default value of the \"Confidential ?\" attribute of created annexes"
-msgid "Sub type confidentiality of created annexes"
+#. Default: "Item WF validation levels leading transition description."
+msgid "Item WF validation levels leading transition description."
 msgstr ""
 
-#. Default: "Please look the help message of the field \"Default value of the 'Confidential ?' attribute of created annexes\" here above.  Simply note that if nothing is defined here, the value defined in the field above will be used."
-msgid "Sub type confidentiality of created annexes description."
+#. Default: "Item WF validation levels leading transition title"
+msgid "Item WF validation levels leading transition title"
 msgstr ""
 
-#. Default: "Correspondences while sent to other meeting configs"
-msgid "Sub type correspondences while sent to other meeting configs"
+#. Default: "Item WF validation levels leading transition title description."
+msgid "Item WF validation levels leading transition title description."
 msgstr ""
 
-#. Default: "Please look the help message of the field \"Correspondences while sent to other meeting configs\" here above.  Simply note that if nothing is defined here, the value defined in the field above will be used."
-msgid "Sub type correspondences while sent to other meeting configs description."
+#. Default: "Item WF validation levels back transition"
+msgid "Item WF validation levels back transition"
 msgstr ""
 
-#. Default: "Active?"
-msgid "Sub type is active?"
+#. Default: "Item WF validation levels back transition description."
+msgid "Item WF validation levels back transition description."
 msgstr ""
 
-#. Default: "Predefined title"
-msgid "Sub type predefined title"
+#. Default: "Item WF validation levels back transition title"
+msgid "Item WF validation levels back transition title"
 msgstr ""
 
-#. Default: "Title"
-msgid "Sub type title"
+#. Default: "Item WF validation levels back transition title description."
+msgid "Item WF validation levels back transition title description."
 msgstr ""
 
-#. Default: "The TAL expression.  Element \"here\" represent the item.  This expression MUST return valid HTML or it will not behave properly on the item."
-msgid "The TAL expression.  Element 'here' represent the item.  This expression MUST return valid HTML or it will not behave properly on the item."
+#. Default: "Item WF validation levels suffix"
+msgid "Item WF validation levels suffix"
 msgstr ""
 
-#. Default: " "
-msgid "The action that will be executed on every items of the meeting."
+#. Default: "Item WF validation levels suffix description."
+msgid "Item WF validation levels suffix description."
 msgstr ""
 
-#. Default: " "
-msgid "The action to execute when 'Execute given action' is selected in column 'Item action'."
+#. Default: "Item WF validation levels extra suffixes"
+msgid "Item WF validation levels extra suffixes"
 msgstr ""
 
-#. Default: "The item field that will be transformed."
-msgid "The item field that will be transformed."
+#. Default: "Item WF validation levels extra suffixes description."
+msgid "Item WF validation levels extra suffixes description."
 msgstr ""
 
-#. Default: "The meeting config the item of this meeting config will be sendable to."
-msgid "The meeting config the item of this meeting config will be sendable to."
+#. Default: "Item WF validation levels enabled"
+msgid "Item WF validation levels enabled"
 msgstr ""
 
-#. Default: "The transition that will trigger the field transform."
-msgid "The transition that will trigger the field transform."
+#. Default: "Item WF validation levels enabled description."
+msgid "Item WF validation levels enabled description."
 msgstr ""
 
-#. Default: " "
-msgid "The transition triggered on the meeting."
+#. Default: "Committee row id"
+msgid "Committee row id"
 msgstr ""
 
-#. Default: "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field \"States in which an item will be automatically sent to selected other meeting configurations\" here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the \"Transitions for presenting an item\" you defined in the \"Workflows\" tab of the meeting configuration the item will be sent to."
-msgid "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field 'States in which an item will be automatically sent to selected other meeting configurations' here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the 'Transitions for presenting an item' you defined in the 'Workflows' tab of the meeting configuration the item will be sent to."
+#. Default: "Committee label"
+msgid "Committee label"
 msgstr ""
 
-#. Default: "Specify here a TAL expression that will restrict or allow the use of this advice to some condition.  We receive \"item\" as the meeting item to give an advice on and \"mayEdit\", a boolean to know if current user may edit the item.  A special expression is available to protect a row that should only be available thru the \"Change delay\" action, it is : \"python: item.REQUEST.get('managing_available_delays', False)\".  This can not be used if something is defined in the \"Advice will be automatically asked if\" column of this advice, but for optional delay-aware advice or for delay-aware advices linked to an automatic advice (using the \"Is linked to previous row?\" column)"
-msgid "available_on_col_description"
+#. Default: "Committee acronym"
+msgid "Committee acronym"
 msgstr ""
 
-#. Default: "Enter the delay the adviser will have to give his advice. If it is not considered as an automatically asked advice (nothing defined in the \"Advice will be automatically asked if\" column), the advice will be selectable in the \"Ask advice to\" list on the item edit form. A delay is a single digit (like \"5\" or \"10\"). If no delay is relevant for this advice, leave this field blank. If several delays are possible for the same advice, you have to define several rows with exactly the same content excepted the delay."
-msgid "delay_col_description"
+#. Default: "Committee default place"
+msgid "Committee default place"
 msgstr ""
 
-#. Default: "If you want a specific label to be displayed on the label displayed in the \"Advice to give\" list on the item edit form and on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The label will appear between brackets after the message \"Name of the group - delay of X days\"."
-msgid "delay_label_col_description"
+#. Default: "Committee default assembly"
+msgid "Committee default assembly"
 msgstr ""
 
-#. Default: "Enter the treshold beyond wich an alert must be shown regarding left delay.  This will be shown in the UI with a particular color and if activated, a mail notification could be send in this case. Enter a single digit (like \"5\" or \"10\") lower than actual \"Delay\". If no treshold is relevant for this advice, leave this field blank."
-msgid "delay_left_alert_col_description"
+#. Default: "Committee default signatures"
+msgid "Committee default signatures"
 msgstr ""
 
-#. Default: "This configuration will be applied on item created from the defined date (defined date included).  Please respect following format : YYYY/MM/DD (year 4 digits/month 2 digits/day 2 digits).  This date will avoid older items created before to be affected, especially when updating every advices thru the \"Update all advices\" action."
-msgid "for_item_created_from_col_description"
+#. Default: "Committee default attendees"
+msgid "Committee default attendees"
 msgstr ""
 
-#. Default: "This configuration will be applied on item created until the defined date (defined date must be in the future and will not be included).  Please respect following format : YYYY/MM/DD (year 4 digits/month 2 digits/day 2 digits).  This date will avoid newer items created after to be affected, especially when updating every advices thru the \"Update all advices\" action. This date will be only settable once, when set, this can not be changed anymore."
-msgid "for_item_created_until_col_description"
+#. Default: "Committee default signatories"
+msgid "Committee default signatories"
 msgstr ""
 
-#. Default: "Specify here a TAL expression that will return True if the advice of the group must be automatically asked on an item.  We receive \"item\" as the meeting item to give an advice on, \"org\" and \"org_uid\" as the organization (organization UID) that will have to give the advice.  WARNING if the group of advisers linked to this group is empty, it will no be considered, despite the result of the TAL expression.  This advice will NOT be askable manually in the user interface, it is only asked automatically by the application.  If this advice should not be asked automatically, leave this field blank."
-msgid "gives_auto_advice_on_col_description"
+#. Default: "Committee using groups"
+msgid "Committee using groups"
 msgstr ""
 
-#. Default: "If you want a specific help message to be displayed on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The message will appear between brackets after the message \"This advice has been automatically asked by the application\"."
-msgid "gives_auto_advice_on_help_message_col_description"
+#. Default: "Committee auto from"
+msgid "Committee auto from"
 msgstr ""
 
-#. Default: "Please use following format : YYYY/MM/DD.  Dates must be sorted (from older to newer)."
-msgid "holiday_date_col_descr"
+#. Default: "Committee supplements"
+msgid "Committee supplements"
 msgstr ""
 
-#. Default: "Power observer item access TAL expression description"
-msgid "power_observers_item_access_on_col_description"
+#. Default: "Committee enabled?"
+msgid "Committee enabled?"
 msgstr ""
 
-#. Default: "Power observer item viewable states description"
-msgid "power_observers_item_states_col_description"
+#. Default: "Used when creating a new meeting if field \"Place\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_place_col_description"
 msgstr ""
 
-#. Default: "Power observer label description"
-msgid "power_observers_label_col_description"
+#. Default: "Used when creating a new meeting if field \"Assembly\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_assembly_col_description"
 msgstr ""
 
-#. Default: "Power observer meeting access TAL expression description"
-msgid "power_observers_meeting_access_on_col_description"
+#. Default: "Used when creating a new meeting if field \"Signatures\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatures_col_description"
 msgstr ""
 
-#. Default: "Power observer meeting viewable states description"
-msgid "power_observers_meeting_states_col_description"
+#. Default: "Used when creating a new meeting if field \"Attendees\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_attendees_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Signatories\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatories_col_description"
+msgstr ""
+
+#. Default: "Used to restrict availability of a committee on the item committees selection box.  This may only be used when column \"auto_from\" is not used."
+msgid "committees_using_groups_col_description"
+msgstr ""
+
+#. Default: "Used to automatically determinate the committee for the item, the field \"Committees\" will not appear on the item when editing it (except for MeetingManagers).  This may only be used when column \"using_groups\" is not used."
+msgid "committees_auto_from_col_description"
+msgstr ""
+
+#. Default: "Will generate new values on item \"Committees\" field when necessary to manage supplements (items added to meeting after committees convocation were sent).  This will only be useable by MeetingManagers."
+msgid "committees_supplements_col_description"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/PloneMeeting.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/PloneMeeting.po`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 msgid "${term_title} (Not selected in plonegroup)"
 msgstr ""
 
 #. Default: "(Nobody)"
 msgid "(Nobody)"
 msgstr ""
 
+#. Default: "(None)"
+msgid "(None)"
+msgstr ""
+
 #. Default: "Add PloneMeeting Portlet"
 msgid "Add PloneMeeting Portlet"
 msgstr "Voeg plonemeeting Portlet toe"
 
 #. Default: "Add Todo Portlet"
 msgid "Add Todo Portlet"
 msgstr "Voeg ToDo Portlet toe"
@@ -157,14 +161,18 @@
 msgid "Attendee has been set signatory."
 msgstr ""
 
 #. Default: "Attendee is no more defined as item signatory."
 msgid "Attendee is no more defined as item signatory."
 msgstr ""
 
+#. Default: "Attendee position has been redefined."
+msgid "Attendee position has been redefined."
+msgstr ""
+
 #. Default: "Back to the MeetingConfig"
 msgid "Back to the MeetingConfig"
 msgstr ""
 
 #. Default: "Back to the item"
 msgid "Back to the item"
 msgstr ""
@@ -241,14 +249,18 @@
 msgid "Close"
 msgstr ""
 
 #. Default: "Comment"
 msgid "Comment"
 msgstr ""
 
+#. Default: "Completed votes"
+msgid "Completed votes"
+msgstr ""
+
 #. Default: "Contacts fields"
 msgid "Contacts fields"
 msgstr ""
 
 #. Default: "Copy PloneMeeting"
 msgid "Copy PloneMeeting"
 msgstr "Copy Plone Meeting"
@@ -469,38 +481,14 @@
 msgid "If you need to use this person data in the application like for example scanned signature or telephone number, select it here."
 msgstr ""
 
 #. Default: "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 msgid "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 msgstr ""
 
-#. Default: "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
 # plone.app.querystring
 #. Default: "Informations about advices on an item"
 msgid "Informations about advices on an item"
 msgstr ""
 
 #. Default: "Inherited advice action"
 msgid "Inherited advice action"
@@ -740,22 +728,30 @@
 msgid "None"
 msgstr ""
 
 #. Default: "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 msgid "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 msgstr ""
 
+#. Default: "Not completed votes"
+msgid "Not completed votes"
+msgstr ""
+
 #. Default: "Not present type"
 msgid "Not present type"
 msgstr ""
 
 #. Default: "Not voter"
 msgid "Not voter"
 msgstr ""
 
+#. Default: "Nothing selected in the configuration to be displayed."
+msgid "Nothing selected in the configuration to be displayed."
+msgstr ""
+
 #. Default: "Nothing to display when item is not presented into a meeting."
 msgid "Nothing to display when item is not presented into a meeting."
 msgstr ""
 
 #. Default: "Nothing to display."
 msgid "Nothing to display."
 msgstr ""
@@ -784,14 +780,18 @@
 msgid "Ordered groups"
 msgstr ""
 
 #. Default: "Original meeting signatory"
 msgid "Original meeting signatory"
 msgstr ""
 
+#. Default: "Original position"
+msgid "Original position"
+msgstr ""
+
 #. Default: "POD template to annex"
 msgid "POD template to annex"
 msgstr ""
 
 #. Default: "Please check item number ${item_number} at ${item_url}."
 msgid "Please check item number ${item_number} at ${item_url}."
 msgstr ""
@@ -825,22 +825,14 @@
 msgid "PloneMeeting_inAndOutMoves"
 msgstr ""
 
 #. Default: "Observations"
 msgid "PloneMeeting_itemObservations"
 msgstr "Opmerkingen"
 
-#. Default: "Observations"
-msgid "PloneMeeting_itemObservations2"
-msgstr "Opmerkingen"
-
-#. Default: "Absents"
-msgid "PloneMeeting_label_absents"
-msgstr ""
-
 # MeetingGroup
 #. Default: "Acronym"
 msgid "PloneMeeting_label_acronym"
 msgstr "Acroniem"
 
 #. Default: "Confidential advice annexes are visible for"
 msgid "PloneMeeting_label_adviceAnnexConfidentialVisibleFor"
@@ -878,50 +870,26 @@
 msgid "PloneMeeting_label_annexToPrintMode"
 msgstr ""
 
 #. Default: "Answers"
 msgid "PloneMeeting_label_answerers"
 msgstr ""
 
-#. Default: "Meeting approval date"
-msgid "PloneMeeting_label_approvalDate"
-msgstr ""
-
 #. Default: "As copy group on"
 msgid "PloneMeeting_label_asCopyGroupOn"
 msgstr ""
 
-#. Default: "Default assembly"
-msgid "PloneMeeting_label_assembly"
-msgstr ""
-
-#. Default: "Default assembly staves"
-msgid "PloneMeeting_label_assemblyStaves"
-msgstr ""
-
 #. Default: "Associated group(s)"
 msgid "PloneMeeting_label_associatedGroups"
 msgstr "Geassiocieerde group(en)"
 
-#. Default: "Attendees"
-msgid "PloneMeeting_label_attendees"
-msgstr ""
-
-#. Default: "Authority notice"
-msgid "PloneMeeting_label_authorityNotice"
-msgstr ""
-
 #. Default: "Columns to display for items available for a meeting"
 msgid "PloneMeeting_label_availableItemsListVisibleColumns"
 msgstr ""
 
-#. Default: "Items"
-msgid "PloneMeeting_label_body"
-msgstr "Agendapunten"
-
 #. Default: "Default value for the \"budget information\" field"
 msgid "PloneMeeting_label_budgetDefault"
 msgstr ""
 
 #. Default: "Budgetary informations"
 msgid "PloneMeeting_label_budgetInfos"
 msgstr ""
@@ -950,14 +918,18 @@
 msgid "PloneMeeting_label_classifier"
 msgstr ""
 
 #. Default: "Observations for the committee"
 msgid "PloneMeeting_label_committeeObservations"
 msgstr ""
 
+#. Default: "Committees"
+msgid "PloneMeeting_label_committees"
+msgstr ""
+
 #. Default: "Completeness"
 msgid "PloneMeeting_label_completeness"
 msgstr ""
 
 #. Default: "Group of meeting configurations"
 msgid "PloneMeeting_label_configGroup"
 msgstr ""
@@ -974,18 +946,14 @@
 msgid "PloneMeeting_label_configVersion"
 msgstr "Identificatie van deze meeting configuratie"
 
 #. Default: "Contents to keep when item sent to another configuration"
 msgid "PloneMeeting_label_contentsKeptOnSentToOtherMC"
 msgstr ""
 
-#. Default: "Meeting convocation date"
-msgid "PloneMeeting_label_convocationDate"
-msgstr ""
-
 #. Default: "Copy groups"
 msgid "PloneMeeting_label_copyGroups"
 msgstr "Kopieer groep"
 
 #. Default: "Css classes to hide"
 msgid "PloneMeeting_label_cssClassesToHide"
 msgstr ""
@@ -1002,26 +970,14 @@
 msgid "PloneMeeting_label_dashboardMeetingAvailableItemsFilters"
 msgstr ""
 
 #. Default: "Advanced filters to show on \"Items of a meeting\""
 msgid "PloneMeeting_label_dashboardMeetingLinkedItemsFilters"
 msgstr ""
 
-#. Default: "Date"
-msgid "PloneMeeting_label_date"
-msgstr "Datum"
-
-#. Default: "Deadline for validating late items"
-msgid "PloneMeeting_label_deadlineFreeze"
-msgstr ""
-
-#. Default: "Deadline for validating items"
-msgid "PloneMeeting_label_deadlinePublish"
-msgstr ""
-
 #. Default: "Decision"
 msgid "PloneMeeting_label_decision"
 msgstr "Beslissing"
 
 #. Default: "Decision (end)"
 msgid "PloneMeeting_label_decisionEnd"
 msgstr ""
@@ -1058,26 +1014,18 @@
 msgid "PloneMeeting_label_delayUnavailableEndDays"
 msgstr ""
 
 #. Default: "Description"
 msgid "PloneMeeting_label_description"
 msgstr "Beschrijving"
 
-#. Default: "Description in the second language"
-msgid "PloneMeeting_label_description2"
-msgstr ""
-
 #. Default: "Detailed description"
 msgid "PloneMeeting_label_detailedDescription"
 msgstr ""
 
-#. Default: "Detailed description"
-msgid "PloneMeeting_label_detailedDescription2"
-msgstr ""
-
 #. Default: "Display available items to"
 msgid "PloneMeeting_label_displayAvailableItemsTo"
 msgstr ""
 
 #. Default: "Emergency"
 msgid "PloneMeeting_label_emergency"
 msgstr ""
@@ -1102,46 +1050,30 @@
 msgid "PloneMeeting_label_enableScanDocs"
 msgstr ""
 
 #. Default: "Enable user preferences"
 msgid "PloneMeeting_label_enableUserPreferences"
 msgstr ""
 
-#. Default: "Effective end date and hour"
-msgid "PloneMeeting_label_endDate"
-msgstr "Effektieve einddatum en -uur"
+#. Default: "Enabled annexes batch actions"
+msgid "PloneMeeting_label_enabledAnnexesBatchActions"
+msgstr ""
 
 #. Default: "Enforce advice mandatoriness"
 msgid "PloneMeeting_label_enforceAdviceMandatoriness"
 msgstr ""
 
-#. Default: "Excused"
-msgid "PloneMeeting_label_excused"
-msgstr ""
-
-#. Default: "Extraordinary session?"
-msgid "PloneMeeting_label_extraordinarySession"
-msgstr ""
-
-#. Default: "Number of the first item contained in this meeting"
-msgid "PloneMeeting_label_firstItemNumber"
-msgstr "Nummer van het eerste item dat de meeting bevat"
-
 #. Default: "First linked vote values"
 msgid "PloneMeeting_label_firstLinkedVoteUsedVoteValues"
 msgstr ""
 
 #. Default: "Name of the folder linked to this configuration"
 msgid "PloneMeeting_label_folderTitle"
 msgstr "Naam van de folder gekoppeld aan deze configuratie"
 
-#. Default: "Default deadline for validating late items for a given meeting"
-msgid "PloneMeeting_label_freezeDeadlineDefault"
-msgstr ""
-
 #. Default: "Email of the functional administrator"
 msgid "PloneMeeting_label_functionalAdminEmail"
 msgstr "Email van de funktionele administrator"
 
 #. Default: "Name of the functional administrator"
 msgid "PloneMeeting_label_functionalAdminName"
 msgstr "Email van de funktionele administrator"
@@ -1182,18 +1114,14 @@
 msgid "PloneMeeting_label_historizeItemDataWhenAdviceIsGiven"
 msgstr ""
 
 #. Default: "Item attributes for which history must be kept"
 msgid "PloneMeeting_label_historizedItemAttributes"
 msgstr ""
 
-#. Default: "Meeting attributes for which history must be kept"
-msgid "PloneMeeting_label_historizedMeetingAttributes"
-msgstr ""
-
 #. Default: "Holidays"
 msgid "PloneMeeting_label_holidays"
 msgstr ""
 
 #. Default: "Include groups in charge defined on category"
 msgid "PloneMeeting_label_includeGroupsInChargeDefinedOnCategory"
 msgstr ""
@@ -1371,18 +1299,14 @@
 msgid "PloneMeeting_label_itemWithGivenAdviceIsNotDeletable"
 msgstr ""
 
 #. Default: "Workflow that dictates the life cycle of every item into this configuration"
 msgid "PloneMeeting_label_itemWorkflow"
 msgstr ""
 
-#. Default: "Items"
-msgid "PloneMeeting_label_items"
-msgstr "Items"
-
 #. Default: "Columns to display for items within a meeting"
 #, fuzzy
 msgid "PloneMeeting_label_itemsListVisibleColumns"
 msgstr "Aantal weer te geven kolommen voor een tabelweergave van items"
 
 #. Default: "Fields of the items to show/hide in the dashboards"
 msgid "PloneMeeting_label_itemsListVisibleFields"
@@ -1473,18 +1397,14 @@
 msgid "PloneMeeting_label_meetingColumns"
 msgstr ""
 
 #. Default: "Interface allowing to use a specific Zope3 adapter for modifying the conditions defined on the transitions of the meeting workflow"
 msgid "PloneMeeting_label_meetingConditionsInterface"
 msgstr ""
 
-#. Default: "Identifier of the configuration's version that is linked to this meeting"
-msgid "PloneMeeting_label_meetingConfigVersion"
-msgstr ""
-
 #. Default: "Meeting configs to clone items to"
 msgid "PloneMeeting_label_meetingConfigsToCloneTo"
 msgstr ""
 
 #. Default: "Title of the folder created in each user folder"
 #, fuzzy
 msgid "PloneMeeting_label_meetingFolderTitle"
@@ -1502,58 +1422,38 @@
 msgid "PloneMeeting_label_meetingManagersNotesEnd"
 msgstr ""
 
 #. Default: "MeetingManagers notes (suite)"
 msgid "PloneMeeting_label_meetingManagersNotesSuite"
 msgstr ""
 
-#. Default: "Meeting number (sequence number automatically attributed)"
-msgid "PloneMeeting_label_meetingNumber"
-msgstr "Nummer van de vergadering (sequentieel nummer dat automatisch wordt toegekend)"
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations"
-msgstr "Opmerkingen"
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations2"
-msgstr "Opmerkingen"
-
 #. Default: "States of the meeting to insert an item into from everywhere"
 msgid "PloneMeeting_label_meetingPresentItemWhenNoCurrentMeetingStates"
 msgstr ""
 
 #. Default: "Meeting transition that triggers the insertion of this item as a recurring item"
 msgid "PloneMeeting_label_meetingTransitionInsertingMe"
 msgstr "De overgang van de vergadering die de toevoeging van dit punt als terugkomend punt teweegbrengt"
 
 #. Default: "Workflow that dictates the life cycle of every meeting into this configuration"
 msgid "PloneMeeting_label_meetingWorkflow"
 msgstr "Werkschema dat de levenscyclus van elke vergadering in deze configuratie dicteert"
 
-#. Default: "End date for meeting first part"
-msgid "PloneMeeting_label_midDate"
-msgstr ""
-
 #. Default: "Model adaptations"
 msgid "PloneMeeting_label_modelAdaptations"
 msgstr ""
 
 #. Default: "Motivation"
 msgid "PloneMeeting_label_motivation"
 msgstr ""
 
 #. Default: "Next linked votes values"
 msgid "PloneMeeting_label_nextLinkedVotesUsedVoteValues"
 msgstr ""
 
-#. Default: "Non attendees"
-msgid "PloneMeeting_label_nonAttendees"
-msgstr ""
-
 #. Default: "Actions to execute on items of a meeting when a transition is triggered on that meeting"
 msgid "PloneMeeting_label_onMeetingTransitionItemActionToExecute"
 msgstr ""
 
 #. Default: "Transforms to apply to rich text fields of an item after a workflow transition"
 msgid "PloneMeeting_label_onTransitionFieldTransforms"
 msgstr ""
@@ -1570,14 +1470,18 @@
 msgid "PloneMeeting_label_oralQuestion"
 msgstr ""
 
 #. Default: "Associated organizations order"
 msgid "PloneMeeting_label_orderedAssociatedOrganizations"
 msgstr ""
 
+#. Default: "Attendees selectable for committees"
+msgid "PloneMeeting_label_orderedCommitteeContacts"
+msgstr ""
+
 #. Default: "Selectable assembly members"
 msgid "PloneMeeting_label_orderedContacts"
 msgstr ""
 
 #. Default: "Ordered groups in charge"
 msgid "PloneMeeting_label_orderedGroupsInCharge"
 msgstr ""
@@ -1602,18 +1506,14 @@
 msgid "PloneMeeting_label_otherMeetingConfigsClonableToPrivacy"
 msgstr ""
 
 #. Default: "Owner of a annex decision may delete it when item is no more editable?"
 msgid "PloneMeeting_label_ownerMayDeleteAnnexDecision"
 msgstr ""
 
-#. Default: "Place"
-msgid "PloneMeeting_label_place"
-msgstr "Lokatie"
-
 #. Default: "Meeting places"
 msgid "PloneMeeting_label_places"
 msgstr ""
 
 #. Default: "Poll type"
 msgid "PloneMeeting_label_pollType"
 msgstr ""
@@ -1626,42 +1526,18 @@
 msgid "PloneMeeting_label_powerAdvisersGroups"
 msgstr ""
 
 #. Default: "Manage power observers"
 msgid "PloneMeeting_label_powerObservers"
 msgstr ""
 
-#. Default: "Date"
-msgid "PloneMeeting_label_preMeetingDate"
-msgstr ""
-
-#. Default: "Default date for the pre-meeting"
-msgid "PloneMeeting_label_preMeetingDateDefault"
-msgstr ""
-
-#. Default: "Place"
-msgid "PloneMeeting_label_preMeetingPlace"
-msgstr ""
-
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations"
-msgstr ""
-
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations2"
-msgstr ""
-
 #. Default: "Previous item"
 msgid "PloneMeeting_label_predecessor"
 msgstr ""
 
-#. Default: "Predefined title in the second language"
-msgid "PloneMeeting_label_predefinedTitle2"
-msgstr ""
-
 #. Default: "Preferred meeting"
 msgid "PloneMeeting_label_preferredMeeting"
 msgstr "Aangewezen vergadering"
 
 #. Default: "Privacy"
 msgid "PloneMeeting_label_privacy"
 msgstr ""
@@ -1670,38 +1546,26 @@
 msgid "PloneMeeting_label_proposingGroup"
 msgstr "Voorstellende groep"
 
 #. Default: "Proposing group (Group in charge)"
 msgid "PloneMeeting_label_proposingGroupWithGroupInCharge"
 msgstr ""
 
-#. Default: "Observations for public meeting"
-msgid "PloneMeeting_label_publicMeetingObservations"
-msgstr ""
-
 #. Default: "Public URL"
 msgid "PloneMeeting_label_publicUrl"
 msgstr ""
 
-#. Default: "Default deadline for validating items for a given meeting"
-msgid "PloneMeeting_label_publishDeadlineDefault"
-msgstr ""
-
 #. Default: "Questions"
 msgid "PloneMeeting_label_questioners"
 msgstr ""
 
 #. Default: "Item states into which events will be recorded in item's history"
 msgid "PloneMeeting_label_recordItemHistoryStates"
 msgstr ""
 
-#. Default: "Meeting states into which events will be recorded in meeting's history"
-msgid "PloneMeeting_label_recordMeetingHistoryStates"
-msgstr ""
-
 #. Default: "Redirect to the next meeting"
 msgid "PloneMeeting_label_redirectToNextMeeting"
 msgstr ""
 
 #. Default: "Remove annexes previews on meeting closure"
 msgid "PloneMeeting_label_removeAnnexesPreviewsOnMeetingClosure"
 msgstr ""
@@ -1718,30 +1582,30 @@
 msgid "PloneMeeting_label_restrictAccessToSecretItemsTo"
 msgstr ""
 
 #. Default: "\"Restrict users\" mode"
 msgid "PloneMeeting_label_restrictUsers"
 msgstr ""
 
-#. Default: "Observations for the secret meeting"
-msgid "PloneMeeting_label_secretMeetingObservations"
-msgstr ""
-
 #. Default: "Selectable advisers"
 msgid "PloneMeeting_label_selectableAdvisers"
 msgstr ""
 
 #. Default: "Groups that can be in copy for an item"
 msgid "PloneMeeting_label_selectableCopyGroups"
 msgstr "Groepen die in kopie voor een punt kunnen zijn"
 
 #. Default: "Selectable privacies"
 msgid "PloneMeeting_label_selectablePrivacies"
 msgstr ""
 
+#. Default: "Restrict selectable redefined position types to following positions"
+msgid "PloneMeeting_label_selectableRedefinedPositionTypes"
+msgstr ""
+
 #. Default: "Is group selectable in the plonegroup configuration panel?"
 msgid "PloneMeeting_label_selectable_for_plonegroup"
 msgstr ""
 
 #. Default: "Send to authority?"
 msgid "PloneMeeting_label_sendToAuthority"
 msgstr ""
@@ -1754,26 +1618,18 @@
 msgid "PloneMeeting_label_showItemKeywordsTargets"
 msgstr ""
 
 #. Default: "Signatories"
 msgid "PloneMeeting_label_signatories"
 msgstr ""
 
-#. Default: "Default signatures"
-msgid "PloneMeeting_label_signatures"
-msgstr "Standaard handtekeningen"
-
 #. Default: "Sort the tags alphabetically"
 msgid "PloneMeeting_label_sortAllItemTags"
 msgstr "De tags alfabetisch sorteren"
 
-#. Default: "Effective start date and hour"
-msgid "PloneMeeting_label_startDate"
-msgstr "Effektieve startdatum en startuur"
-
 #. Default: "Meeting file sub types"
 msgid "PloneMeeting_label_subTypes"
 msgstr ""
 
 #. Default: "Taken over by"
 msgid "PloneMeeting_label_takenOverBy"
 msgstr ""
@@ -1782,23 +1638,14 @@
 msgid "PloneMeeting_label_templateUsingGroups"
 msgstr ""
 
 #. Default: "Checklist"
 msgid "PloneMeeting_label_textCheckList"
 msgstr ""
 
-# Meeting
-#. Default: "Title"
-msgid "PloneMeeting_label_title"
-msgstr "Titel"
-
-#. Default: "Title in the second language"
-msgid "PloneMeeting_label_title2"
-msgstr ""
-
 #. Default: "To discuss ?"
 msgid "PloneMeeting_label_toDiscuss"
 msgstr "Te bespreken ?"
 
 #. Default: "Default value of the \"toDiscuss\" attribute for normal items"
 #, fuzzy
 msgid "PloneMeeting_label_toDiscussDefault"
@@ -1921,38 +1768,38 @@
 msgid "PloneMeeting_label_xhtmlTransformTypes"
 msgstr ""
 
 #. Default: "Reinitialise meeting number every year?"
 msgid "PloneMeeting_label_yearlyInitMeetingNumber"
 msgstr ""
 
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations"
-msgstr "Opmerkingen"
-
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations2"
-msgstr "Opmerkingen"
-
 #. Default: "Notes"
 msgid "PloneMeeting_notes"
 msgstr ""
 
 #. Default: "Document templates"
 msgid "PodTemplates"
 msgstr "Dokument templates"
 
 #. Default: "Position type"
 msgid "Position type"
 msgstr ""
 
+#. Default: "Position type to use"
+msgid "Position type to use"
+msgstr ""
+
 #. Default: "Position type to use as label for the signature."
 msgid "Position type to use as label for the signature."
 msgstr ""
 
+#. Default: "Position type to use for the attendee on this item."
+msgid "Position type to use for the attendee on this item."
+msgstr ""
+
 #. Default: "Preview detailed advice"
 msgid "Preview detailed advice"
 msgstr ""
 
 #. Default: "Preview of annexes were deleted upon meeting closure."
 msgid "Preview of annexes were deleted upon meeting closure."
 msgstr ""
@@ -1962,14 +1809,26 @@
 msgid "Previous review state"
 msgstr ""
 
 #. Default: "Recurring items"
 msgid "RecurringItems"
 msgstr "Voorgedefinieerde punten"
 
+#. Default: "Redefine position for this attendee for this item"
+msgid "Redefine position for this attendee for this item"
+msgstr ""
+
+#. Default: "Redefined attendee position was removed."
+msgid "Redefined attendee position was removed."
+msgstr ""
+
+#. Default: "Redefined position"
+msgid "Redefined position"
+msgstr ""
+
 #. Default: "References of contained items have been updated."
 msgid "References of contained items have been updated."
 msgstr ""
 
 #. Default: "Reinitiatlize delay"
 msgid "Reinitiatlize delay"
 msgstr ""
@@ -1986,14 +1845,18 @@
 msgid "Remove inherited advice"
 msgstr ""
 
 #. Default: "Remove inherited advice and ask advice locally"
 msgid "Remove inherited advice and ask advice locally"
 msgstr ""
 
+#. Default: "Remove redefined attendee position for this item"
+msgid "Remove redefined attendee position for this item"
+msgstr ""
+
 #. Default: "Represented organizations"
 msgid "Represented organizations"
 msgstr ""
 
 #. Default: "Searches"
 msgid "Searches"
 msgstr ""
@@ -2046,14 +1909,18 @@
 msgid "Signature number"
 msgstr ""
 
 #. Default: "Signature position type"
 msgid "Signature position type"
 msgstr ""
 
+#. Default: "Specify a number to which this will be applied. Field default is current item number."
+msgid "Specify a number to which this will be applied. Field default is current item number."
+msgstr ""
+
 #. Default: "state"
 msgid "State"
 msgstr "Staat "
 
 #. Default: "Style templates"
 msgid "Style templates"
 msgstr ""
@@ -2097,14 +1964,18 @@
 msgstr ""
 
 # plone.app.querystring
 #. Default: "The item, advice or meeting previous review state"
 msgid "The item, advice or meeting previous review state"
 msgstr ""
 
+#. Default: "The position of this attendee was changed for the ${number} following item(s)"
+msgid "The position of this attendee was changed for the ${number} following item(s)"
+msgstr ""
+
 #. Default: "There was an error during annex conversion, please contact system administrator."
 msgid "There was an error during annex conversion, please contact system administrator."
 msgstr ""
 
 #. Default: "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
 msgid "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
 msgstr ""
@@ -2145,18 +2016,14 @@
 msgid "This automatic advice has been asked by the application (shown by his title not being between brackets)"
 msgstr ""
 
 #. Default: "This copy group was set automatically by the application"
 msgid "This copy group was set automatically by the application"
 msgstr ""
 
-#. Default: "This is an extract of the comment, access full comment if necessary..."
-msgid "This is an extract of the comment, access full comment if necessary..."
-msgstr ""
-
 #. Default: "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 msgid "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 msgstr ""
 
 #. Default: "This label can not be removed as it is used by some items, for example ${item_url}"
 msgid "This label can not be removed as it is used by some items, for example ${item_url}"
 msgstr ""
@@ -2238,16 +2105,16 @@
 msgid "Votes are not completed for following ${number} ${polltype} item(s)"
 msgstr ""
 
 #. Default: "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 msgid "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 msgstr ""
 
-#. Default: "You cannot delete the default item template, but you can deactivate it if necessary!"
-msgid "You cannot delete the default item template, but you can deactivate it if necessary!"
+#. Default: "You cannot delete or move the default item template, but you can deactivate it if necessary!"
+msgid "You cannot delete or move the default item template, but you can deactivate it if necessary!"
 msgstr ""
 
 #. Default: "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 msgid "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 msgstr ""
 
 #. Default: "Not grouped meeting configurations"
@@ -2480,76 +2347,76 @@
 msgid "annexAdded_mail_subject"
 msgstr "${portalTitle} - ${meetingTitle} - An annex was just added to an item."
 
 #. Default: "If an annex is marked as \"Confidential\" by a meeting manager, following selected profiles will not be able to see it."
 msgid "annex_confidential_for_descr"
 msgstr ""
 
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item."
-msgid "annex_is_confidential_no"
+#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" could not be kept because it was not possible to find a corresponding annex type in the destination meeting configuration, please contact system administrator."
+msgid "annex_not_kept_because_no_available_annex_type_warning"
 msgstr ""
 
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item.  Click on the image to set it as confidential."
-msgid "annex_is_confidential_no_edit"
+#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" was not kept because using a scan_id, please contact system administrator."
+msgid "annex_not_kept_because_using_scan_id"
 msgstr ""
 
-#. Default: "The annex is confidential."
-msgid "annex_is_confidential_yes"
+#. Default: "Select for each optional annexes attributes which are only displayed or editable by MeetingManagers.  If an attribute is only displayed to MeetingManagers it will be automatically considered as only editable by MeetingManagers as well."
+msgid "annex_restrict_shown_and_editable_attributes_descr"
 msgstr ""
 
-#. Default: "The annex is confidential.  Click on the image to set it as not confidential."
-msgid "annex_is_confidential_yes_edit"
+#. Default: "Confidential"
+msgid "annex_term_confidential"
 msgstr ""
 
-#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" could not be kept because it was not possible to find a corresponding annex type in the destination meeting configuration, please contact system administrator."
-msgid "annex_not_kept_because_no_available_annex_type_warning"
+#. Default: "Not confidential"
+msgid "annex_term_not_confidential"
 msgstr ""
 
-#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" was not kept because using a scan_id, please contact system administrator."
-msgid "annex_not_kept_because_using_scan_id"
+#. Default: "Not publishable"
+msgid "annex_term_not_publishable"
 msgstr ""
 
-#. Default: "Select for each optional annexes attributes which are only displayed or editable by MeetingManagers.  If an attribute is only displayed to MeetingManagers it will be automatically considered as only editable by MeetingManagers as well."
-msgid "annex_restrict_shown_and_editable_attributes_descr"
+#. Default: "Not to print"
+msgid "annex_term_not_to_print"
 msgstr ""
 
-#. Default: "Title"
-msgid "annex_title"
-msgstr "Titel"
-
-#. Default: "The annex is not printable because it can not be converted (unsupported format or error during conversion).  Please use common office formats."
-msgid "annex_to_print_disabled"
+#. Default: "Not to sign"
+msgid "annex_term_not_to_sign"
 msgstr ""
 
-#. Default: "Automated (annexes are printed by the application)"
-msgid "annex_to_print_mode_automated"
+#. Default: "Publishable"
+msgid "annex_term_publishable"
 msgstr ""
 
-#. Default: "If print functionnality is enabled for annexes and an annex is set \"to print\", select here the to print mode that will be used : \"Manual\", means that the to print is just defined for information and that the printing process will be handled manually or \"Automated\", in this case, the application will generate a printable format for the annex (converted to images) so it can be inserted in a generated document."
-msgid "annex_to_print_mode_descr"
+#. Default: "Signed"
+msgid "annex_term_signed"
 msgstr ""
 
-#. Default: "For information (annexes are printed manually)"
-msgid "annex_to_print_mode_info"
+#. Default: "To print"
+msgid "annex_term_to_print"
 msgstr ""
 
-#. Default: "The annex will not be printed."
-msgid "annex_to_print_no"
+#. Default: "To sign"
+msgid "annex_term_to_sign"
 msgstr ""
 
-#. Default: "The annex will not be printed. Click on the image to print it."
-msgid "annex_to_print_no_edit"
+#. Default: "Title"
+msgid "annex_title"
+msgstr "Titel"
+
+#. Default: "Automated (annexes are printed by the application)"
+msgid "annex_to_print_mode_automated"
 msgstr ""
 
-#. Default: "The annex will be printed."
-msgid "annex_to_print_yes"
+#. Default: "If print functionnality is enabled for annexes and an annex is set \"to print\", select here the to print mode that will be used : \"Manual\", means that the to print is just defined for information and that the printing process will be handled manually or \"Automated\", in this case, the application will generate a printable format for the annex (converted to images) so it can be inserted in a generated document."
+msgid "annex_to_print_mode_descr"
 msgstr ""
 
-#. Default: "The annex will be printed. Click on the image not to print it."
-msgid "annex_to_print_yes_edit"
+#. Default: "For information (annexes are printed manually)"
+msgid "annex_to_print_mode_info"
 msgstr ""
 
 #. Default: "Annex type"
 msgid "annex_type"
 msgstr "Type van de bijlage"
 
 #. Default: "Every item may be associated with a series of annexes. Some annexes may be specifically tied to the decision taken on the item. You can consult and modify here the annex types that are defined within this meeting configuration. An annex type is defined by a title, an icon (preferably of 16x16 pixels) and a predefined title. When users want to associate an annex to an item, they may choose, in a dropdown list, an annex type among those defined here and upload a file."
@@ -2576,24 +2443,16 @@
 msgid "annexes_preview_disabled"
 msgstr ""
 
 #. Default: "<span style='color: green;'>Annexes preview is enabled in the ${documentviewer_url}.</span>"
 msgid "annexes_preview_enabled"
 msgstr ""
 
-#. Default: "Signed annexes"
-msgid "annexes_signed_term"
-msgstr ""
-
-#. Default: "Annexes to print"
-msgid "annexes_to_print_term"
-msgstr ""
-
-#. Default: "Annexes to sign"
-msgid "annexes_to_sign_term"
+#. Default: "Annexes types are hidden by default, you can ${force_display} of it (may take some time)."
+msgid "annexes_types_force_display_descr"
 msgstr ""
 
 #. Default: "Application users"
 msgid "app_users"
 msgstr ""
 
 #. Default: "Are you sure?"
@@ -2628,18 +2487,14 @@
 msgid "assemblyMember"
 msgstr ""
 
 #. Default: "Absents as defined on the linked meeting"
 msgid "assembly_absents_defined_on_meeting"
 msgstr ""
 
-#. Default: "Define here people that were absents (not excused) for the meeting"
-msgid "assembly_absents_meeting_descr"
-msgstr ""
-
 #. Default: "Assembly and signatures"
 msgid "assembly_and_signatures"
 msgstr ""
 
 #. Default: "Assembly as defined on the linked meeting"
 msgid "assembly_defined_on_meeting"
 msgstr ""
@@ -2648,26 +2503,18 @@
 msgid "assembly_descr"
 msgstr ""
 
 #. Default: "Excused as defined on the linked meeting"
 msgid "assembly_excused_defined_on_meeting"
 msgstr ""
 
-#. Default: "Define here people that were excused for the meeting"
-msgid "assembly_excused_meeting_descr"
-msgstr ""
-
 #. Default: "Guests as defined on the linked meeting"
 msgid "assembly_guests_defined_on_meeting"
 msgstr ""
 
-#. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
-msgid "assembly_meeting_descr"
-msgstr ""
-
 #. Default: "Using attribute(s) \"itemExcused\" and/or \"itemAbsents\" requires the use of attribute \"assembly\"."
 msgid "assembly_required"
 msgstr ""
 
 #. Default: "Define here the default assembly staves (for example you may type a list of names and first names separated by colons or new lines) that will be automatically selected on newly created meetings."
 msgid "assembly_staves_descr"
 msgstr ""
@@ -2758,14 +2605,18 @@
 msgid "budgetimpacteditors"
 msgstr ""
 
 #. Default: "You can not access this item"
 msgid "can_not_access_this_item"
 msgstr ""
 
+#. Default: "Assembly and signatures : you can not use same signature number several times."
+msgid "can_not_define_several_same_signature_number"
+msgstr ""
+
 #. Default: "You can not define two rows for the same meeting configuration!"
 msgid "can_not_define_two_rows_for_same_meeting_config"
 msgstr ""
 
 #. Default: "You can not remove/disable a function that is used by an item in the configuration.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_config_meetingitem"
 msgstr ""
@@ -2774,30 +2625,34 @@
 msgid "can_not_delete_plone_group_meetingconfig"
 msgstr ""
 
 #. Default: "You can not remove/disable a function that is used by an item in the application.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_meetingitem"
 msgstr ""
 
-#. Default: "You can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
 msgid "can_not_remove_attendee_redefined_on_items"
 msgstr ""
 
-#. Default: "You can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
 msgid "can_not_remove_public_voter_voted_on_items"
 msgstr ""
 
-#. Default: "You can not unselect a voter that already voted on a secret vote item."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a secret vote item."
 msgid "can_not_remove_secret_voter_voted_on_items"
 msgstr ""
 
 #. Default: "This item can no more be returned to the meeting managers because the meeting is in a state not authorizing it (${meetingState})."
 msgid "can_not_return_to_meeting_because_of_meeting_state"
 msgstr ""
 
+#. Default: "You can not select \"No committee\" and a committee."
+msgid "can_not_select_no_committee_and_committee"
+msgstr ""
+
 #. Default: "You can not select an adviser that is already displayed on the item as an inherited advice.  If you need to ask this advice again, you need to remove the inherited advice (as a MeetingManager or a Manager) then select advice again."
 msgid "can_not_select_optional_adviser_same_group_as_inherited"
 msgstr ""
 
 #. Default: "You can not select several values for the same group.  Please select a single value for the same group among available ones."
 msgid "can_not_select_several_optional_advisers_same_group"
 msgstr ""
@@ -2831,18 +2686,14 @@
 msgid "categories_descr"
 msgstr "Every item, within this meeting configuration, can only belong to one category. Those categories are defined here (by a title and a description). The order into which they appear in this folder is important. Indeed, if we make the assumption that you desire it (it depends on a parameter you may modify in the 'data' section), when an item is added to a meeting, it can be inserted at the end of the items belonging to the same category, those items being themselves inserted at a place that corresponds to the position of their category among the list of categories defined here. That being said, if you tell PloneMeeting that you want to use the PloneMeeting groups as categories (another parameter of the 'data' section), the categories defined here will be ignored."
 
 #. Default: "the \"Folder contents view\""
 msgid "categories_folder_contents_view"
 msgstr ""
 
-#. Default: "force display"
-msgid "categories_force_display"
-msgstr ""
-
 #. Default: "You can ${force_display} of every categories (may take some time)."
 msgid "categories_force_display_descr"
 msgstr ""
 
 #. Default: "You may use the ${folder_contents_link} to manage elements order."
 msgid "categories_use_folder_contents"
 msgstr ""
@@ -2991,14 +2842,34 @@
 msgid "clone_to"
 msgstr ""
 
 #. Default: "Your configuration says can not correct this closed meeting, contact your system administrator if you want to change this."
 msgid "closed_meeting_not_correctable_by_config"
 msgstr ""
 
+#. Default: "${title} (${number}&nbsp;s.)"
+msgid "committee_title_with_abbr_suppl"
+msgstr ""
+
+#. Default: "${title} (${number}&nbsp;supplement)"
+msgid "committee_title_with_suppl"
+msgstr ""
+
+#. Default: "Committees"
+msgid "committees"
+msgstr ""
+
+#. Default: "Define committees that will be useable on meetings and items (you also need to enable \"Committees\" on the meeting in the [Data] tab). This will show a \"Committees\" table on the meeting and will be also managed on the item. <br />There are 2 ways to manage committees on the item, either manually or automatically:<ul><li>Manually: just define committees, this will create a multiselection box on the item and users may select it.  It is possible to use the column \"Restrict to\" to define which proposing groups will be able to select the committee;</li><li>Automatically: use the column \"Auto from\" to define which committees to associate to the item depending on proposing group, category or classifier. A MeetingManager is nevertheless able to edit the committee on the item.</li></ul>. These 2 ways are mutually exclusive, if you select values in the \"auto_from\" columb here under, the \"Automatic\" mode will be used."
+msgid "committees_descr"
+msgstr ""
+
+#. Default: "Using a \"Committees\" field requires the use of attribute \"Committees (committees)\"."
+msgid "committees_required"
+msgstr ""
+
 #. Default: "Complete"
 msgid "completeness_complete"
 msgstr ""
 
 #. Default: "Evaluation asked again"
 msgid "completeness_evaluation_asked_again"
 msgstr ""
@@ -3084,14 +2955,18 @@
 msgid "copyGroups_mail_body"
 msgstr ""
 
 #. Default: "${meetingConfigTitle} - You have been carbon copied - ${itemTitle}"
 msgid "copyGroups_mail_subject"
 msgstr ""
 
+#. Default: "These groups will have read access to the item in following states: ${states}.\nWhen icon is green, this means that copy groups have access to the item.\nWhen the label \"[auto]\" is displayed next to the group title, it means that the group was set as copy group automatically by the application."
+msgid "copy_groups_help_msg"
+msgstr ""
+
 #. Default: " "
 msgid "copy_groups_item_descr"
 msgstr "Selekteer hier de groepen die in staat zullen zijn dit punt te zien"
 
 #. Default: "The cloned item could not be presented to a meeting in the \"${destMeetingConfigTitle}\" configuration, no suitable meeting could be found."
 msgid "could_not_present_item_no_meeting_accepting_items"
 msgstr ""
@@ -3278,14 +3153,34 @@
 msgid "delay_of_x_days"
 msgstr ""
 
 #. Default: "Select here the days a computed delay can not ends with.  If a computed delay is ending on one of selected week day, the delay will be extend to next available day.  <span style='color: red;'>If you change this parameter, do not forget to run \"Update items and meetings\"!</span>"
 msgid "delay_unavailable_end_days_descr"
 msgstr ""
 
+#. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
+msgid "descr_assembly"
+msgstr ""
+
+#. Default: "<span style='color: red;'>WARNING, this field is managed by the application and it's value will be \"-1\" until the meeting is frozen, then it will be computed automatically. Do only change it manually when necessary (in general this should never happen). This field is only editable and viewable by meeting managers</span>"
+msgid "descr_config_field_reserved_to_meeting_managers"
+msgstr ""
+
+#. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
+msgid "descr_field_reserved_to_meeting_managers"
+msgstr ""
+
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
+msgid "descr_field_vieawable_by_everyone"
+msgstr ""
+
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
+msgid "descr_field_vieawable_by_everyone_once_meeting_decided"
+msgstr ""
+
 #. Default: "You are just able to see visible elements here. Please consult the \"manage\" box here opposite."
 msgid "description_only_see_visible_items"
 msgstr ""
 
 #. Default: "By default only MeetingManagers will see the available items panel on a meeting as long as the meeting is accepting items.  This let's you show this panel to selected profiles.  Note that if you enable this, the meeting view will be displayed slower."
 msgid "display_available_items_to_descr"
 msgstr ""
@@ -3382,14 +3277,22 @@
 msgid "enable_scan_docs_descr"
 msgstr ""
 
 #. Default: "If you check this box, users will be able to access a screen for modifying their preferences. While powerful, some may think it exposes too much complexity to users."
 msgid "enable_user_preferences_descr"
 msgstr ""
 
+#. Default: "Select the batch actions that will be displayed on the table listing annexes"
+msgid "enabled_annexes_batch_actions_descr"
+msgstr ""
+
+#. Default: "The meeting end date must occur after the start date and meeting date."
+msgid "end_date_before_meeting_date"
+msgstr ""
+
 #. Default: "When advice mandatoriness is enforced, an item can't be inserted into a meeting unless all mandatory advices are given and positive."
 msgid "enforce_advice_mandatoriness_descr"
 msgstr ""
 
 #. Default: "You can not encode more than ${max_voters} voters."
 msgid "error_can_not_encode_more_than_max_voters"
 msgstr ""
@@ -3410,14 +3313,30 @@
 msgid "error_certified_signatures_invalid_dates"
 msgstr ""
 
 #. Default: "Signatures must be ordered by signature number, please check and order signature using the arrows on the right of the table."
 msgid "error_certified_signatures_order"
 msgstr ""
 
+#. Default: "You can not remove a configuration that was already used, removed configuration \"${committee_label}\" is used for example by item at ${url}.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committee_row_id_removed_already_used"
+msgstr ""
+
+#. Default: "You can not define values for the \"auto_from\" and \"using_groups\" columns, their use is multually exclusive.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committees_mutually_exclusive_auto_from_and_using_groups"
+msgstr ""
+
+#. Default: "Default poll type must be among used poll types"
+msgid "error_default_poll_type_must_be_among_used_poll_types"
+msgstr ""
+
+#. Default: "First linked vote used votes values must be among used vote values"
+msgid "error_first_linked_vote_used_vote_values_must_be_among_used_vote_values"
+msgstr ""
+
 #. Default: "You may not remove a list type that is currently used by an item, check for example : ${url}."
 msgid "error_list_types_identifier_removed_already_used"
 msgstr ""
 
 #. Default: "You may not remove the default list types (\"normal\" and \"late\")."
 msgid "error_list_types_missing_default"
 msgstr ""
@@ -3426,14 +3345,22 @@
 msgid "error_list_types_same_identifier"
 msgstr ""
 
 #. Default: "You may only use lowercase letters for identifier."
 msgid "error_list_types_wrong_identifier_format"
 msgstr ""
 
+#. Default: "Next linked votes used vote values must be among used vote values"
+msgid "error_next_linked_votes_used_vote_values_must_be_among_used_vote_values"
+msgstr ""
+
+#. Default: "Some selected values are no more selectable (no more selected in the \"Ordered committees contacts\" field), please check value \"${hp_title}\".  You can not select \"No committee\" and a committee.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_value_removed_used_in_committees_field"
+msgstr ""
+
 #. Default: "An advice was added or updated on an item (notify the \"Creators\")"
 msgid "event_add_advice"
 msgstr ""
 
 #. Default: "An advice was added or updated on an item (notify the \"Owner\")"
 msgid "event_add_advice_owner"
 msgstr ""
@@ -3545,28 +3472,36 @@
 msgid "fastedit_save_changes"
 msgstr ""
 
 #. Default: "Please fill this field."
 msgid "field_required"
 msgstr "Vul dit, alstublieft."
 
-#. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
-msgid "field_reserved_to_meeting_managers_descr"
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once item is decided</span>"
+msgid "field_vieawable_by_everyone_once_item_decided_descr"
 msgstr ""
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
-msgid "field_vieawable_by_everyone_descr"
+#. Default: "Assembly and signatures"
+msgid "fieldset_assembly"
 msgstr ""
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once item is decided</span>"
-msgid "field_vieawable_by_everyone_once_item_decided_descr"
+#. Default: "Committees"
+msgid "fieldset_committees"
 msgstr ""
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
-msgid "field_vieawable_by_everyone_once_meeting_decided_descr"
+#. Default: "Dates and data"
+msgid "fieldset_dates_and_data"
+msgstr ""
+
+#. Default: "Informations"
+msgid "fieldset_informations"
+msgstr ""
+
+#. Default: "Parameters"
+msgid "fieldset_parameters"
 msgstr ""
 
 #. Default: "Please choose a file by clicking on the \"Browse\" button."
 #, fuzzy
 msgid "file_required"
 msgstr "Gelieve een bestand te kiezen door te klikken op de 'Bladeren' knop."
 
@@ -3579,20 +3514,16 @@
 msgstr ""
 
 #. Default: "In the application folder of every member, a sub-folder is created for each meeting configuration. The name of this sub-folder is defined here."
 #, fuzzy
 msgid "folder_title_descr"
 msgstr "In the PloneMeeting folder of every member, a sub-folder is created for each meeting configuration. The name of this sub-folder is defined here."
 
-#. Default: "For the administrator only"
-msgid "for_admin_only"
-msgstr "Enkel toegankelijk voor de beheerder"
-
-#. Default: "Specify here the deadline for validating late items to be inserted in a given meeting.  Leave the field empty not to use this functionality."
-msgid "freeze_deadline_default_descr"
+#. Default: "force display"
+msgid "force_display"
 msgstr ""
 
 #. Default: "<p>PloneMeeting body in HTML format.</p>"
 msgid "front_page_body"
 msgstr ""
 
 #. Default: "Manage here your official meetings."
@@ -3693,14 +3624,18 @@
 msgstr ""
 
 # Other
 #. Default: "Check/uncheck items"
 msgid "helpSelectItemsIcon"
 msgstr ""
 
+#. Default: "This is the date the advice was originally given, this will change when the advice will be considered \"Given\" in a state where it is no more editable"
+msgid "help_given_on_before_started_on"
+msgstr ""
+
 #. Default: "No preview available because this type of file can not be converted.  Please use common office formats.  You can download the file, look in the \"actions\" column."
 msgid "help_no_preview_available"
 msgstr ""
 
 #. Default: "No preview available because there was an error during conversion to a previewable format.  Please contact system administrator that will have access to more debugging informations."
 msgid "help_no_preview_available_conversion_error"
 msgstr ""
@@ -3741,18 +3676,14 @@
 msgid "historize_item_data_when_advice_is_given_descr"
 msgstr ""
 
 #. Default: "For every field you select here, the application will keep track of any change on any item, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
 msgid "historized_item_attrs_descr"
 msgstr ""
 
-#. Default: "For every field you select here, the application will keep track of any change on any meeting, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
-msgid "historized_meeting_attrs_descr"
-msgstr ""
-
 #. Default: "See changes"
 msgid "history_changes"
 msgstr ""
 
 #. Default: "Deleted by ${userName}"
 msgid "history_delete"
 msgstr ""
@@ -3769,15 +3700,15 @@
 msgid "holidays_date_not_ascending_error"
 msgstr ""
 
 #. Default: "These dates will be used to compute advices delays.  <span style='color: red;'>If you change this parameter and modified dates are interacting with some existing advice delays, do not forget to run \"Update items and meetings\"!</span>"
 msgid "holidays_descr"
 msgstr ""
 
-#. Default: "You removed a date that is currently in use!"
+#. Default: "You removed a date that is currently in use! Check item at ${item_url}"
 msgid "holidays_removed_date_in_use_error"
 msgstr ""
 
 #. Default: "There are not enough holidays defined in the configuration.  These days are used for advice delay computation.  This warning appear when last holiday defined in the configuration is in less than 60 days. Contact you system administrator if necessary."
 msgid "holidays_warning_message"
 msgstr ""
 
@@ -3797,14 +3728,18 @@
 msgid "hs_name"
 msgstr "Naam"
 
 #. Default: "This application allows you to manage your official meetings."
 msgid "hs_welcome_body"
 msgstr ""
 
+#. Default: "iA.Delib documentation"
+msgid "iA.Delib documentation"
+msgstr ""
+
 #. Default: "Azur"
 msgid "icon_color_azur"
 msgstr ""
 
 #. Default: "Black"
 msgid "icon_color_black"
 msgstr ""
@@ -4417,38 +4352,26 @@
 
 # Mails (item-related)
 #. Default: "${meetingConfigTitle} - A \"late\" item has been validated."
 #, fuzzy
 msgid "lateItem_mail_subject"
 msgstr "${portalTitle} A 'late' item has been validated."
 
-#. Default: "Items presented tardily"
-msgid "late_presented_items"
-msgstr "Items voorgesteld na de vergadering werden gepubliceerd."
-
 #. Default: "--- Do nothing, let the item in the workflow initial state ---"
 msgid "let_item_in_initial_state"
 msgstr ""
 
 #. Default: "Linked items (${auto_linked_items})"
 msgid "linked_items"
 msgstr ""
 
 #. Default: "Linked items, ${auto_linked_items} automatically and ${manually_linked_items} manually"
 msgid "linked_items_with_manually_linked_items"
 msgstr ""
 
-#. Default: "Late"
-msgid "list_type_late"
-msgstr ""
-
-#. Default: "Normal"
-msgid "list_type_normal"
-msgstr ""
-
 #. Default: "Types of list of items that will be available when an item is linked to a meeting."
 msgid "list_types_descr"
 msgstr ""
 
 #. Default: "Size"
 msgid "listingheader_size"
 msgstr "Grootte"
@@ -4546,36 +4469,16 @@
 msgid "meeting_annex_confidential_visible_for_descr"
 msgstr ""
 
 #. Default: "Choose here which page will be shown after logon."
 msgid "meeting_app_default_view_descr"
 msgstr "Choose here which page will be shown after logon."
 
-#. Default: "Assembly"
-msgid "meeting_assembly"
-msgstr "Vergadering"
-
-#. Default: "Absents"
-msgid "meeting_assemblyAbsents"
-msgstr ""
-
-#. Default: "Excused"
-msgid "meeting_assemblyExcused"
-msgstr ""
-
-#. Default: "Guests"
-msgid "meeting_assemblyGuests"
-msgstr ""
-
-#. Default: "Proxies"
-msgid "meeting_assemblyProxies"
-msgstr ""
-
-#. Default: "Staves"
-msgid "meeting_assemblyStaves"
+#. Default: "Meeting assembly (${number_of_attendees}) and signatories (${number_of_signatories})"
+msgid "meeting_attendees_and_signatories"
 msgstr ""
 
 #. Default: "Choose here which columns to display when listing meetings (ie, when displaying the list of available meetings or decisions, or when performing custom searches)."
 msgid "meeting_columns_descr"
 msgstr ""
 
 #. Default: "Similarly to interfaces defined for items, the conditions expressed on the transitions of the meeting workflow may be configured through the development of another Plone product into which you must:<ul><li>create a Python interface that inherits from interface Products.PloneMeeting.interfaces.IMeetingWorkflowConditions (you must enter the full package name of this interface in the field below);</li><li>create and declare in ZCML an adapter that adapts the interface  Products.PloneMeeting.interfaces.IMeeting to the interface you have defined in the previous step.</li></ul>Your adapter may inherit from the default adapter Products.PloneMeeting.Meeting.MeetingWorkflowConditions: it will allow you to override only methods for which you want an altered behaviour. All the methods proposed by the interface Products.PloneMeeting.interfaces.IMeetingWorkflowConditions are documented."
@@ -4621,22 +4524,14 @@
 msgid "meeting_organizations"
 msgstr ""
 
 #. Default: "When an item is inserted in a meeting from everywhere (so not when on a meeting view), this will take the very next meeting still accepting items.  Define here states to take into account to get this very next meeting."
 msgid "meeting_present_item_when_no_current_meeting_states_descr"
 msgstr ""
 
-#. Default: "Signatories"
-msgid "meeting_signatories"
-msgstr ""
-
-#. Default: "Signatures"
-msgid "meeting_signatures"
-msgstr ""
-
 #. Default: "You can consult this meeting at ${objectUrl}."
 msgid "meeting_state_changed_default_mail_body"
 msgstr ""
 
 # Mails (meeting-related)
 # Default translation for mails sent upon meeting transition
 # This default is used if no accurate translation can be found. We will try for example to translate
@@ -4728,26 +4623,18 @@
 msgid "metadata"
 msgstr ""
 
 #. Default: "Select here some standard adaptations that can be applied to data structures."
 msgid "model_adaptations_descr"
 msgstr ""
 
-#. Default: "Move the item down"
-msgid "move_item_down"
-msgstr "Verplaats het punt naar beneden"
-
-#. Default: "Move item to given position"
+#. Default: "Save item number (you may also use the [Enter] key)"
 msgid "move_item_to_given_position"
 msgstr ""
 
-#. Default: "Move the item up"
-msgid "move_item_up"
-msgstr "Verplaats het punt naar boven"
-
 #. Default: "Moves this item to the position that precedes the number you have introduced besides. If you want to move the item at the end of the list, specify the number of the last item plus one."
 msgid "move_several"
 msgstr "Moves this item to the position that precedes the number you have introduced besides. If you want to move the item at the end of the list, specify the number of the last item plus one."
 
 #. Default: "Negative"
 msgid "negative"
 msgstr "negatief"
@@ -4764,34 +4651,42 @@
 msgid "nil"
 msgstr "visa"
 
 #. Default: "No annex is currently defined for this element."
 msgid "no_annexes"
 msgstr "Geen bijlage wordt momenteel bepaald voor dit punt."
 
-#. Default: "No annexes to print"
-msgid "no_annexes_to_print_term"
-msgstr ""
-
-#. Default: "Annexes not to sign"
-msgid "no_annexes_to_sign_term"
-msgstr ""
-
 #. Default: "Attributes \"assembly\" and \"attendees\" can't be used together."
 msgid "no_assembly_and_attendees"
 msgstr ""
 
 #. Default: "No category is currently defined."
 msgid "no_category"
 msgstr "Geen categorie wordt momenteel bepaald."
 
 #. Default: "No classifier is currently defined."
 msgid "no_classifier"
 msgstr ""
 
+#. Default: "NC"
+msgid "no_committee_term_title_acronym"
+msgstr ""
+
+#. Default: "No committee"
+msgid "no_committee_term_title_label"
+msgstr ""
+
+#. Default: "Attributes \"committees_assembly\" and \"committees_attendees\" can't be used together."
+msgid "no_committees_assembly_and_committees_attendees"
+msgstr ""
+
+#. Default: "Attributes \"committees_sigantures\" and \"committees_signatories\" can't be used together."
+msgid "no_committees_signatures_and_committees_signatories"
+msgstr ""
+
 #. Default: "None"
 msgid "no_config_group"
 msgstr ""
 
 #. Default: "No emergency"
 msgid "no_emergency"
 msgstr ""
@@ -4816,31 +4711,28 @@
 msgid "no_meeting_file_type"
 msgstr "Geen bijlagetype wordt momenteel bepaald."
 
 #. Default: "No special user is currently defined."
 msgid "no_meeting_user"
 msgstr ""
 
-#. Default: "No items."
-msgid "no_meetingitems"
-msgstr "Geen punten."
-
 #. Default: "No POD template is currently defined."
 msgid "no_pod_folder"
 msgstr ""
 
 #. Default: "Attributes \"proposingGroupWithGroupInCharge\" and \"groupsInCharge\" can't be used together."
 msgid "no_proposingGroupWithGroupInCharge_and_groupsInCharge"
 msgstr ""
 
 #. Default: "No recurring item is currently defined."
 msgid "no_recurring_item"
 msgstr "Geen terugkomend punt wordt momenteel bepaald."
 
-#. Default: "No visible item for now."
+#. Default: "You do not have access to these items."
+#, fuzzy
 msgid "no_shown_items"
 msgstr "Momenteel geen zichtbaar punt."
 
 #. Default: "Attributes \"signatures\" and \"signatories\" can't be used together."
 msgid "no_signatories_and_signatures"
 msgstr ""
 
@@ -4868,14 +4760,22 @@
 msgid "normal"
 msgstr ""
 
 #. Default: "You are a registered user but your account has not been activated yet. Please contact the system administrator."
 msgid "notPloneMeetingUser"
 msgstr ""
 
+#. Default: "Not able to find a meeting to present this item into.  Only meetings in the future are taken into account, check configuration if necessary"
+msgid "not_able_to_find_meeting_to_present_item_into"
+msgstr ""
+
+#. Default: "Not confidential annexes"
+msgid "not_confidential_annexes"
+msgstr ""
+
 #. Default: "Not given yet"
 msgid "not_given"
 msgstr ""
 
 #. Default: "Not to be cloned to anywhere"
 msgid "not_to_be_cloned_to_term"
 msgstr ""
@@ -4892,14 +4792,22 @@
 msgid "nothing_to_do"
 msgstr ""
 
 #. Default: "notify users able to view the element"
 msgid "notify_users_able_to_view_element"
 msgstr ""
 
+#. Default: "${number}st"
+msgid "num_part_st"
+msgstr ""
+
+#. Default: "${number}th"
+msgid "num_part_th"
+msgstr ""
+
 #. Default: "Total number of voters"
 msgid "number_of_voters"
 msgstr ""
 
 #. Default: "Observer"
 msgid "observer"
 msgstr "Waarnemer"
@@ -4908,14 +4816,18 @@
 msgid "observers"
 msgstr "Waarnemers"
 
 #. Default: "Follow all associated groups order"
 msgid "on_all_associated_groups"
 msgstr ""
 
+#. Default: "Follow all committees order"
+msgid "on_all_committees"
+msgstr ""
+
 #. Default: "Follow all groups order"
 msgid "on_all_groups"
 msgstr ""
 
 #. Default: "Follow categories order"
 msgid "on_categories"
 msgstr ""
@@ -4996,14 +4908,18 @@
 msgid "oral_question_item_descr"
 msgstr ""
 
 #. Default: "If this field is left empty, selectable associated organizations are every organizations selected in the plonegroup configuration panel.  Here you may select associated organizations in a particular order including organizations that are not selected in the plonegroup configuration panel.  This is only relevant if the 'Associated groups' field is enabled on items."
 msgid "ordered_associated_organizations_descr"
 msgstr ""
 
+#. Default: "Select here attendees that will be selectable in the \"Attendees\" column of defined committees here under.  <span style='color: red;'>If you select/unselect values, you need to save first then edit again for these values to appear/disappear if field \"Committees\" here under.</span>"
+msgid "ordered_committee_contacts_descr"
+msgstr ""
+
 #. Default: "Select here contacts that will be usable to manage meeting attendees.  The contacts order defined here will be the default order when creating a new meeting."
 msgid "ordered_contacts_descr"
 msgstr ""
 
 #. Default: "If this field is left empty, selectable groups in charge are every organizations selected in the plonegroup configuration panel.  Here you may select groups in charge in a particular order.  This is only relevant if the 'Groups in charge' field is enabled on items."
 msgid "ordered_groups_in_charge_descr"
 msgstr ""
@@ -5036,20 +4952,24 @@
 msgid "owner_may_delete_annex_decision_descr"
 msgstr ""
 
 #. Default: "Mark this person absent for this item"
 msgid "person_byebye"
 msgstr ""
 
-#. Default: "Remove this person from absents for this item"
-msgid "person_welcome"
+#. Default: "Redefine position for attendee for this item"
+msgid "person_redefine_attendee_position"
 msgstr ""
 
-#. Default: "Please encode this other place."
-msgid "place_other_required"
+#. Default: "Remove redefined position for attendee for this item"
+msgid "person_remove_redefined_attendee_position"
+msgstr ""
+
+#. Default: "Remove this person from absents for this item"
+msgid "person_welcome"
 msgstr ""
 
 #. Default: "Enter here some default places where meetings occur. There must be one place per line. The first one will be the default one."
 msgid "places_descr"
 msgstr ""
 
 #. Default: "You are about to delete this meeting and all included items. Are you sure?"
@@ -5245,22 +5165,14 @@
 msgid "powerobservers"
 msgstr ""
 
 #. Default: "The preparatory meeting must occur before the meeting."
 msgid "pre_date_after_meeting_date"
 msgstr ""
 
-#. Default: "Preparatory meeting"
-msgid "pre_meeting"
-msgstr ""
-
-#. Default: "Specify here the date of the pre-meeting, relative to its meeting, in the same format as fields above.  Leave the field empty not to use this functionality."
-msgid "pre_meeting_date_default_descr"
-msgstr ""
-
 #. Default: "If this is a normal item and you want it to be inserted in any availale meeting, just select \"No preference\" value.  Selecting a date is for 2 usecases : this will make the item not presentable to the meetings before selected one, or if the selected meeting is \"frozen\", this will make current item considered as \"late\" item presentable in the selected frozen meeting.  Indeed, the only way to insert an item in a frozen meeting is to select this meeting as preferred meeting."
 msgid "preferred_meeting_descr"
 msgstr ""
 
 #. Default: "Pre-validator"
 msgid "prereviewer"
 msgstr "Pre-validator"
@@ -5305,32 +5217,32 @@
 msgid "public"
 msgstr ""
 
 #. Default: "Public meeting (heading)"
 msgid "public_heading"
 msgstr ""
 
-#. Default: "Specify here the deadline for validating items to be inserted in a given meeting. You need to express this deadline relative to the meeting date. For example, \"5.9:30\" (do not type quotes) means: \"5 days before the meeting date, at 9:30.\".  Leave the field empty not to use this functionality."
-msgid "publish_deadline_default_descr"
-msgstr ""
-
 #. Default: "Publishable (displayed)"
 msgid "publishable_display"
 msgstr ""
 
 #. Default: "Publishable (editable)"
 msgid "publishable_edit"
 msgstr ""
 
-#. Default: "Select here the item states into which some events related to the item (like annex creations or deletions) will be stored in the item's history."
-msgid "record_item_history_states_descr"
+#. Default: "Read less"
+msgid "read_less"
+msgstr ""
+
+#. Default: "Read more"
+msgid "read_more"
 msgstr ""
 
-#. Default: "Select here the meeting states into which some events related to the meeting will be stored in the meeting's history."
-msgid "record_meeting_history_states_descr"
+#. Default: "Select here the item states into which some events related to the item (like annex creations or deletions) will be stored in the item's history."
+msgid "record_item_history_states_descr"
 msgstr ""
 
 #. Default: "The recurring item specified in the subject of this email could not be inserted in a meeting. Maybe does it lack some important information (a text for the decision, for example) while the meeting is in an \"advanced\" state (it is already \"decided\", for instance). More information can be found in the log file of your Zope instance."
 #, fuzzy
 msgid "recurringItemWorkflowError_mail_body"
 msgstr "The recurring item specified in the subject of this email could not be inserted in a meeting. Maybe does it lack some important information (a text for the decision, for example) while the meeting is in an 'advanced' state (it is already 'decided', for instance). More information can be found in the log file of your Zope instance."
 
@@ -5379,26 +5291,34 @@
 msgid "remove_several_items"
 msgstr ""
 
 #. Default: "Selected items have been removed from the meeting."
 msgid "remove_several_items_done"
 msgstr ""
 
-#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by \"${hp_url}\"!"
+#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by held position at \"${hp_url}\"!"
 msgid "removed_position_type_in_use_error"
 msgstr ""
 
+#. Default: "You can not remove a position type that was used as redefined position for an attendee on an item, you removed \"${removed_position_type}\", check attendees on item at \"${item_url}\"!"
+msgid "removed_redefined_position_type_in_use_error"
+msgstr ""
+
 #. Default: "A category must be selected on this item so it may evolve in the workflow"
 msgid "required_category_ko"
 msgstr ""
 
 #. Default: "A classifier must be selected on this item so it may evolve in the workflow"
 msgid "required_classifier_ko"
 msgstr ""
 
+#. Default: "A group in charge must be selected on this item so it may evolve in the workflow"
+msgid "required_groupsInCharge_ko"
+msgstr ""
+
 #. Default: "Check the box if access to secret items must be restricted.  This will let only users for which an explicit access to the item has been given, access the item.  It will be the case so for members of the proposing groups, power users (Managers, MeetingManagers, power observers), copy groups and advisers.  Only activate this if necessary, it could be the case if you have a state where everything is accessible by everyone (like a \"published\" state for items) but where you want \"secret\" items not to be accessible by everyone."
 msgid "restrict_access_to_secret_items_descr"
 msgstr ""
 
 #. Default: "Restrict access to secret items to description"
 msgid "restrict_access_to_secret_items_to_descr"
 msgstr ""
@@ -5581,14 +5501,18 @@
 msgid "selectable_for_plonegroup_descr"
 msgstr ""
 
 #. Default: "Select here privacies that will be selectable by users editing items of this configuration.  If \"on privacy\" is used in the \"Sort order(s) to apply when adding an item to a meeting\" field, it is the order of values selected here that will be used."
 msgid "selectable_privacies_descr"
 msgstr ""
 
+#. Default: "Select here position types that will be selectable when redefining the position of an attendee for an item.  If nothing selected (default), then any position types is selectable."
+msgid "selectable_redefined_position_types_descr"
+msgstr ""
+
 #. Default: "Check the box if item needs to be send to authority, if so, a line will be automatically printed in the item deliberation document."
 msgid "send_to_authority_descr"
 msgstr ""
 
 #. Default: "Unable to send this item to the ${meetingConfigTitle} meetingConfig because the user to create the item to does not have a personal folder in this meetingConfig.  If necessary, the concerned user can connect for this folder to be created automatically."
 msgid "sendto_inexistent_destfolder_error"
 msgstr ""
@@ -5635,18 +5559,14 @@
 msgid "show_or_hide_details"
 msgstr "Toon / verberg details"
 
 #. Default: "Show / hide poll type observations"
 msgid "show_or_hide_pollTypeObservations"
 msgstr ""
 
-#. Default: "Signatures"
-msgid "signatures"
-msgstr "Handtekeningen"
-
 #. Default: "Signatures as defined on the linked meeting"
 msgid "signatures_defined_on_meeting"
 msgstr ""
 
 #. Default: "Define here the default signatures that will be automatically selected on newly created meetings. Use 2 lines by signature, one for the function and one for the signatory name. This will be applicable only if you use attribute \"Signatures\" for meetings."
 #, fuzzy
 msgid "signatures_descr"
@@ -5660,14 +5580,22 @@
 msgid "signed_edit"
 msgstr ""
 
 #. Default: "Check this box if you want to sort the tags in alphabetic order."
 msgid "sort_all_item_tags_descr"
 msgstr "Check this box if you want to sort the tags in alphabetic order."
 
+#. Default: "The meeting start date must occur before the end date."
+msgid "start_date_after_end_date"
+msgstr ""
+
+#. Default: "The meeting start date must occur after the meeting date."
+msgid "start_date_before_meeting_date"
+msgstr ""
+
 #. Default: "Store as annex of type ${annex_type_title}"
 msgid "store_as_annex_type_title"
 msgstr ""
 
 #. Default: "Not allowed to add annex in this element."
 msgid "store_podtemplate_as_annex_can_not_add_annex"
 msgstr ""
@@ -5761,21 +5689,217 @@
 msgstr ""
 
 #. Default: "This item is NOT an oral question"
 msgid "this_item_is_not_an_oral_question"
 msgstr ""
 
 #. Default: "Extraordinary session"
-msgid "this_meeting_is_extraodrinary_session"
+msgid "this_meeting_is_extraordinary_session"
+msgstr ""
+
+#. Default: "Absents"
+msgid "title_absents"
+msgstr ""
+
+#. Default: "Approval date"
+msgid "title_approval_date"
+msgstr ""
+
+#. Default: "Assembly"
+msgid "title_assembly"
+msgstr ""
+
+#. Default: "Assembly absents"
+msgid "title_assembly_absents"
+msgstr ""
+
+#. Default: "Assembly excused"
+msgid "title_assembly_excused"
+msgstr ""
+
+#. Default: "Assembly guests"
+msgid "title_assembly_guests"
+msgstr ""
+
+#. Default: "Assembly observations"
+msgid "title_assembly_observations"
+msgstr ""
+
+#. Default: "Assembly proxies"
+msgid "title_assembly_proxies"
+msgstr ""
+
+#. Default: "Assembly staves"
+msgid "title_assembly_staves"
+msgstr ""
+
+#. Default: "Attendees"
+msgid "title_attendees"
+msgstr ""
+
+#. Default: "Authority notice"
+msgid "title_authority_notice"
+msgstr ""
+
+#. Default: "Committees"
+msgid "title_committees"
+msgstr ""
+
+#. Default: "Assembly"
+msgid "title_committees_assembly"
+msgstr ""
+
+#. Default: "Attendees"
+msgid "title_committees_attendees"
+msgstr ""
+
+#. Default: "Convocation date"
+msgid "title_committees_convocation_date"
+msgstr ""
+
+#. Default: "Date"
+msgid "title_committees_date"
+msgstr ""
+
+#. Default: "Committees observations"
+msgid "title_committees_observations"
+msgstr ""
+
+#. Default: "Place"
+msgid "title_committees_place"
+msgstr ""
+
+#. Default: "Committee"
+msgid "title_committees_row_id"
+msgstr ""
+
+#. Default: "Signatories"
+msgid "title_committees_signatories"
+msgstr ""
+
+#. Default: "Signatures"
+msgid "title_committees_signatures"
+msgstr ""
+
+#. Default: "Convocation date"
+msgid "title_convocation_date"
+msgstr ""
+
+#. Default: "Date"
+msgid "title_date"
+msgstr ""
+
+#. Default: "Default assembly"
+msgid "title_default_assembly"
+msgstr ""
+
+#. Default: "Default assembly staves"
+msgid "title_default_assembly_staves"
+msgstr ""
+
+#. Default: "Default signatures"
+msgid "title_default_signatures"
+msgstr ""
+
+#. Default: "End date"
+msgid "title_end_date"
+msgstr ""
+
+#. Default: "Excused"
+msgid "title_excused"
+msgstr ""
+
+#. Default: "Extraordinary session"
+msgid "title_extraordinary_session"
+msgstr ""
+
+#. Default: "First item number (managed automatically when meeting is frozen)"
+msgid "title_first_item_number"
+msgstr ""
+
+#. Default: "In and out moves"
+msgid "title_in_and_out_moves"
+msgstr ""
+
+#. Default: "Meeting number"
+msgid "title_meeting_number"
+msgstr ""
+
+#. Default: "Meeting managers notes"
+msgid "title_meetingmanagers_notes"
+msgstr ""
+
+#. Default: "Mid date"
+msgid "title_mid_date"
+msgstr ""
+
+#. Default: "Non attendees"
+msgid "title_non_attendees"
+msgstr ""
+
+#. Default: "Notes"
+msgid "title_notes"
+msgstr ""
+
+#. Default: "Observations"
+msgid "title_observations"
+msgstr ""
+
+#. Default: "Place"
+msgid "title_place"
+msgstr ""
+
+#. Default: "Other place"
+msgid "title_place_other"
+msgstr ""
+
+#. Default: "Pre meeting date"
+msgid "title_pre_meeting_date"
+msgstr ""
+
+#. Default: "Pre meeting place"
+msgid "title_pre_meeting_place"
+msgstr ""
+
+#. Default: "Pre observations"
+msgid "title_pre_observations"
+msgstr ""
+
+#. Default: "Public meeting observations"
+msgid "title_public_meeting_observations"
+msgstr ""
+
+#. Default: "Replacements"
+msgid "title_replacements"
 msgstr ""
 
 #. Default: "A title is required."
 msgid "title_required"
 msgstr "Een titel is vereist."
 
+#. Default: "Secret meeting observations"
+msgid "title_secret_meeting_observations"
+msgstr ""
+
+#. Default: "Signatories"
+msgid "title_signatories"
+msgstr ""
+
+#. Default: "Signatures"
+msgid "title_signatures"
+msgstr ""
+
+#. Default: "Start date"
+msgid "title_start_date"
+msgstr ""
+
+#. Default: "Votes observations"
+msgid "title_votes_observations"
+msgstr ""
+
 #. Default: "Ask this advice again (current advice will be historized)"
 msgid "to_advice_asked_again"
 msgstr ""
 
 #. Default: "To be printed (displayed)"
 msgid "to_be_printed_display"
 msgstr ""
@@ -5964,18 +6088,14 @@
 msgid "used_poll_types_descr"
 msgstr ""
 
 #. Default: "Specify here what vote values are in use in this meeting configuration."
 msgid "used_vote_values_descr"
 msgstr ""
 
-#. Default: "Users"
-msgid "users"
-msgstr "gebruikers"
-
 #. Default: "If you do not select anything, every users will be displayed."
 msgid "users_hidden_in_dashboard_filter_descr"
 msgstr ""
 
 #. Default: "When an advice is \"given\" and no more editable by the advisers, so when it was set in a state where advisers may not edit it anymore, it is automatically versioned. Depending on the configuration, if advice may be given when the item is still editable by the proposing group, it may be necessary to versionate advice if it was given (but still editable by advisers) and the item was edited. For example, advices are giveable when item is \"itemcreated\", a state where item may still be edited by the proposing group. If it is the case, check this box, it will ensure that the advice is versioned when the item is edited if necessary (so if it was not already versioned since last advice edition).  If you have a specific state \"waiting advice\" where proposing group is not able to edit the item, this box may be left unchecked."
 msgid "versionate_advice_if_given_and_item_modified_descr"
 msgstr ""
@@ -6081,14 +6201,15 @@
 msgstr ""
 
 #. Default: "There are ${numberOfVoters} voters for this item."
 msgid "voter_count"
 msgstr ""
 
 #. Default: "Votes"
+#, fuzzy
 msgid "votes"
 msgstr "Stemmen"
 
 #. Default: "You can choose here who will effectively encode the votes. Several choices are possible."
 msgid "votes_encoder_descr"
 msgstr ""
 
@@ -6292,14 +6413,22 @@
 msgid "wait_msg"
 msgstr ""
 
 #. Default: "You are currently adding an organization outside \"My organization\", please make sure this is correct.  If you want to create a new group that will be able the create items, give advices, you need to add it directly under \"My organization\"."
 msgid "warning_adding_org_outside_own_org"
 msgstr ""
 
+#. Default: "Advice is currently \"Asked again\" do not forget to change value of field \"Advice type\" to another value than \"Asked again\""
+msgid "warning_advice_asked_again_need_to_change_advice_type"
+msgstr ""
+
+#. Default: "Warning, there is a problem with encoded data for assembly and signatures, please check especially that signatories are correctly defined"
+msgid "warning_assembly_and_signatures"
+msgstr ""
+
 #. Default: "Warning: if you modify the title or description and save this form, all given advices will be invalidated."
 msgid "warning_invalidate_advices"
 msgstr ""
 
 #. Default: "If you modify this field, all given advices will be invalidated."
 msgid "warning_invalidate_advices_fastedit"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.contact.core.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.contact.core.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.history.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/plone.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/plone.po`

 * *Files 0% similar despite different names*

```diff
@@ -562,14 +562,18 @@
 msgid "close"
 msgstr "Sluiten"
 
 #. Default: "Closed"
 msgid "closed"
 msgstr "Gesloten"
 
+#. Default: "Committees"
+msgid "committees"
+msgstr ""
+
 #. Default: "Confirm"
 msgid "confirm"
 msgstr "Bevestig"
 
 #. Default: "Confirmed"
 msgid "confirmed"
 msgstr "Bevestigd"
@@ -1000,14 +1004,15 @@
 msgstr "Bevestigen"
 
 #. Default: "Validated"
 msgid "validated"
 msgstr "Bevestigd"
 
 #. Default: "Votes"
+#, fuzzy
 msgid "votes"
 msgstr "stemmen"
 
 #. Default: "Ask advices"
 msgid "wait_advices_from"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.actionspanel.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.annex.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.annex.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/imio.history.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.eeafaceted.batchactions.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.eeafaceted.batchactions.pot`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.contact.core.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.contact.core.pot`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/eea.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/eea.po`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 
 msgid "Category"
 msgstr ""
 
 msgid "Classifier"
 msgstr ""
 
+#. Default: "Committee"
+msgid "Committee"
+msgstr ""
+
 #. Default: "Copy groups"
 msgid "Copy groups"
 msgstr ""
 
 msgid "Created"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.documentgenerator.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.documentgenerator.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.behavior.talcondition.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.behavior.talcondition.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.eeafaceted.batchactions.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.eeafaceted.batchactions.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.iconifiedcategory.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.iconifiedcategory.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/datagridfield.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/datagridfield.po`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,62 @@
 "Domain: datagridfield\n"
 "X-Is-Fallback-For: de-be de-at de-li de-lu de-ch de-de\n"
 
 #. Default: "Available on"
 msgid "Available on"
 msgstr ""
 
+#. Default: "Committee acronym"
+msgid "Committee acronym"
+msgstr ""
+
+#. Default: "Committee auto from"
+msgid "Committee auto from"
+msgstr ""
+
+#. Default: "Committee default assembly"
+msgid "Committee default assembly"
+msgstr ""
+
+#. Default: "Committee default attendees"
+msgid "Committee default attendees"
+msgstr ""
+
+#. Default: "Committee default place"
+msgid "Committee default place"
+msgstr ""
+
+#. Default: "Committee default signatories"
+msgid "Committee default signatories"
+msgstr ""
+
+#. Default: "Committee default signatures"
+msgid "Committee default signatures"
+msgstr ""
+
+#. Default: "Committee enabled?"
+msgid "Committee enabled?"
+msgstr ""
+
+#. Default: "Committee label"
+msgid "Committee label"
+msgstr ""
+
+#. Default: "Committee row id"
+msgid "Committee row id"
+msgstr ""
+
+#. Default: "Committee supplements"
+msgid "Committee supplements"
+msgstr ""
+
+#. Default: "Committee using groups"
+msgid "Committee using groups"
+msgstr ""
+
 #. Default: "Full label"
 msgid "Config group full label"
 msgstr ""
 
 #. Default: "Label"
 msgid "Config group label"
 msgstr ""
@@ -311,14 +359,46 @@
 msgid "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field 'States in which an item will be automatically sent to selected other meeting configurations' here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the 'Transitions for presenting an item' you defined in the 'Workflows' tab of the meeting configuration the item will be sent to."
 msgstr ""
 
 #. Default: "Specify here a TAL expression that will restrict or allow the use of this advice to some condition.  We receive \"item\" as the meeting item to give an advice on and \"mayEdit\", a boolean to know if current user may edit the item.  A special expression is available to protect a row that should only be available thru the \"Change delay\" action, it is : \"python: item.REQUEST.get('managing_available_delays', False)\".  This can not be used if something is defined in the \"Advice will be automatically asked if\" column of this advice, but for optional delay-aware advice or for delay-aware advices linked to an automatic advice (using the \"Is linked to previous row?\" column)"
 msgid "available_on_col_description"
 msgstr ""
 
+#. Default: "Used to automatically determinate the committee for the item, the field \"Committees\" will not appear on the item when editing it (except for MeetingManagers).  This may only be used when column \"using_groups\" is not used."
+msgid "committees_auto_from_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Assembly\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_assembly_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Attendees\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_attendees_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Place\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_place_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Signatories\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatories_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Signatures\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatures_col_description"
+msgstr ""
+
+#. Default: "Will generate new values on item \"Committees\" field when necessary to manage supplements (items added to meeting after committees convocation were sent).  This will only be useable by MeetingManagers."
+msgid "committees_supplements_col_description"
+msgstr ""
+
+#. Default: "Used to restrict availability of a committee on the item committees selection box.  This may only be used when column \"auto_from\" is not used."
+msgid "committees_using_groups_col_description"
+msgstr ""
+
 #. Default: "Enter the delay the adviser will have to give his advice. If it is not considered as an automatically asked advice (nothing defined in the \"Advice will be automatically asked if\" column), the advice will be selectable in the \"Ask advice to\" list on the item edit form. A delay is a single digit (like \"5\" or \"10\"). If no delay is relevant for this advice, leave this field blank. If several delays are possible for the same advice, you have to define several rows with exactly the same content excepted the delay."
 msgid "delay_col_description"
 msgstr ""
 
 #. Default: "If you want a specific label to be displayed on the label displayed in the \"Advice to give\" list on the item edit form and on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The label will appear between brackets after the message \"Name of the group - delay of X days\"."
 msgid "delay_label_col_description"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/PloneMeeting.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/PloneMeeting.po`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 msgid "${term_title} (Not selected in plonegroup)"
 msgstr ""
 
 #. Default: "(Nobody)"
 msgid "(Nobody)"
 msgstr ""
 
+#. Default: "(None)"
+msgid "(None)"
+msgstr ""
+
 #. Default: "Add PloneMeeting Portlet"
 msgid "Add PloneMeeting Portlet"
 msgstr "PloneMeeting Portlet hinzufügen"
 
 #. Default: "Add Todo Portlet"
 msgid "Add Todo Portlet"
 msgstr "Zu erledigen Portlet hinzufügen"
@@ -156,14 +160,18 @@
 msgid "Attendee has been set signatory."
 msgstr ""
 
 #. Default: "Attendee is no more defined as item signatory."
 msgid "Attendee is no more defined as item signatory."
 msgstr ""
 
+#. Default: "Attendee position has been redefined."
+msgid "Attendee position has been redefined."
+msgstr ""
+
 #. Default: "Back to the MeetingConfig"
 msgid "Back to the MeetingConfig"
 msgstr ""
 
 #. Default: "Back to the item"
 msgid "Back to the item"
 msgstr ""
@@ -240,14 +248,18 @@
 msgid "Close"
 msgstr ""
 
 #. Default: "Comment"
 msgid "Comment"
 msgstr ""
 
+#. Default: "Completed votes"
+msgid "Completed votes"
+msgstr ""
+
 #. Default: "Contacts fields"
 msgid "Contacts fields"
 msgstr ""
 
 #. Default: "Copy PloneMeeting"
 msgid "Copy PloneMeeting"
 msgstr "Kopiere TOP"
@@ -468,38 +480,14 @@
 msgid "If you need to use this person data in the application like for example scanned signature or telephone number, select it here."
 msgstr ""
 
 #. Default: "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 msgid "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 msgstr ""
 
-#. Default: "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
 # plone.app.querystring
 #. Default: "Informations about advices on an item"
 msgid "Informations about advices on an item"
 msgstr ""
 
 #. Default: "Inherited advice action"
 msgid "Inherited advice action"
@@ -739,22 +727,30 @@
 msgid "None"
 msgstr ""
 
 #. Default: "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 msgid "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 msgstr ""
 
+#. Default: "Not completed votes"
+msgid "Not completed votes"
+msgstr ""
+
 #. Default: "Not present type"
 msgid "Not present type"
 msgstr ""
 
 #. Default: "Not voter"
 msgid "Not voter"
 msgstr ""
 
+#. Default: "Nothing selected in the configuration to be displayed."
+msgid "Nothing selected in the configuration to be displayed."
+msgstr ""
+
 #. Default: "Nothing to display when item is not presented into a meeting."
 msgid "Nothing to display when item is not presented into a meeting."
 msgstr ""
 
 #. Default: "Nothing to display."
 msgid "Nothing to display."
 msgstr ""
@@ -783,14 +779,18 @@
 msgid "Ordered groups"
 msgstr ""
 
 #. Default: "Original meeting signatory"
 msgid "Original meeting signatory"
 msgstr ""
 
+#. Default: "Original position"
+msgid "Original position"
+msgstr ""
+
 #. Default: "POD template to annex"
 msgid "POD template to annex"
 msgstr ""
 
 #. Default: "Please check item number ${item_number} at ${item_url}."
 msgid "Please check item number ${item_number} at ${item_url}."
 msgstr ""
@@ -824,22 +824,14 @@
 msgid "PloneMeeting_inAndOutMoves"
 msgstr ""
 
 #. Default: "Observations"
 msgid "PloneMeeting_itemObservations"
 msgstr "Beobachtungen"
 
-#. Default: "Observations"
-msgid "PloneMeeting_itemObservations2"
-msgstr "Beobachtungen"
-
-#. Default: "Absents"
-msgid "PloneMeeting_label_absents"
-msgstr "Abwesende"
-
 # MeetingGroup
 #. Default: "Acronym"
 msgid "PloneMeeting_label_acronym"
 msgstr "Akronym"
 
 #. Default: "Confidential advice annexes are visible for"
 msgid "PloneMeeting_label_adviceAnnexConfidentialVisibleFor"
@@ -877,50 +869,26 @@
 msgid "PloneMeeting_label_annexToPrintMode"
 msgstr ""
 
 #. Default: "Answers"
 msgid "PloneMeeting_label_answerers"
 msgstr ""
 
-#. Default: "Meeting approval date"
-msgid "PloneMeeting_label_approvalDate"
-msgstr ""
-
 #. Default: "As copy group on"
 msgid "PloneMeeting_label_asCopyGroupOn"
 msgstr ""
 
-#. Default: "Default assembly"
-msgid "PloneMeeting_label_assembly"
-msgstr "Standard-Versammlung"
-
-#. Default: "Default assembly staves"
-msgid "PloneMeeting_label_assemblyStaves"
-msgstr ""
-
 #. Default: "Associated group(s)"
 msgid "PloneMeeting_label_associatedGroups"
 msgstr "Zugehörige Gruppe(n)"
 
-#. Default: "Attendees"
-msgid "PloneMeeting_label_attendees"
-msgstr "Teilnehmer"
-
-#. Default: "Authority notice"
-msgid "PloneMeeting_label_authorityNotice"
-msgstr ""
-
 #. Default: "Columns to display for items available for a meeting"
 msgid "PloneMeeting_label_availableItemsListVisibleColumns"
 msgstr ""
 
-#. Default: "Items"
-msgid "PloneMeeting_label_body"
-msgstr "TOP"
-
 #. Default: "Default value for the \"budget information\" field"
 #, fuzzy
 msgid "PloneMeeting_label_budgetDefault"
 msgstr "Standardwert für das Feld 'Budget Informationen'"
 
 #. Default: "Budgetary informations"
 msgid "PloneMeeting_label_budgetInfos"
@@ -950,14 +918,18 @@
 msgid "PloneMeeting_label_classifier"
 msgstr ""
 
 #. Default: "Observations for the committee"
 msgid "PloneMeeting_label_committeeObservations"
 msgstr ""
 
+#. Default: "Committees"
+msgid "PloneMeeting_label_committees"
+msgstr ""
+
 #. Default: "Completeness"
 msgid "PloneMeeting_label_completeness"
 msgstr ""
 
 #. Default: "Group of meeting configurations"
 msgid "PloneMeeting_label_configGroup"
 msgstr ""
@@ -974,18 +946,14 @@
 msgid "PloneMeeting_label_configVersion"
 msgstr "Bezeichnung dieser Sitzungs-Konfiguration"
 
 #. Default: "Contents to keep when item sent to another configuration"
 msgid "PloneMeeting_label_contentsKeptOnSentToOtherMC"
 msgstr ""
 
-#. Default: "Meeting convocation date"
-msgid "PloneMeeting_label_convocationDate"
-msgstr ""
-
 #. Default: "Copy groups"
 msgid "PloneMeeting_label_copyGroups"
 msgstr "Gruppen in Kopie"
 
 #. Default: "Css classes to hide"
 msgid "PloneMeeting_label_cssClassesToHide"
 msgstr ""
@@ -1002,26 +970,14 @@
 msgid "PloneMeeting_label_dashboardMeetingAvailableItemsFilters"
 msgstr ""
 
 #. Default: "Advanced filters to show on \"Items of a meeting\""
 msgid "PloneMeeting_label_dashboardMeetingLinkedItemsFilters"
 msgstr ""
 
-#. Default: "Date"
-msgid "PloneMeeting_label_date"
-msgstr "Datum"
-
-#. Default: "Deadline for validating late items"
-msgid "PloneMeeting_label_deadlineFreeze"
-msgstr "Frist um verspätete TOP zu validieren"
-
-#. Default: "Deadline for validating items"
-msgid "PloneMeeting_label_deadlinePublish"
-msgstr "Frist um TOP zu validieren"
-
 #. Default: "Decision"
 msgid "PloneMeeting_label_decision"
 msgstr "Beschluss"
 
 #. Default: "Decision (end)"
 msgid "PloneMeeting_label_decisionEnd"
 msgstr ""
@@ -1058,26 +1014,18 @@
 msgid "PloneMeeting_label_delayUnavailableEndDays"
 msgstr ""
 
 #. Default: "Description"
 msgid "PloneMeeting_label_description"
 msgstr "Beschreibung"
 
-#. Default: "Description in the second language"
-msgid "PloneMeeting_label_description2"
-msgstr ""
-
 #. Default: "Detailed description"
 msgid "PloneMeeting_label_detailedDescription"
 msgstr "Detaillierte Beschreibung"
 
-#. Default: "Detailed description"
-msgid "PloneMeeting_label_detailedDescription2"
-msgstr "Detaillierte Beschreibung"
-
 #. Default: "Display available items to"
 msgid "PloneMeeting_label_displayAvailableItemsTo"
 msgstr ""
 
 #. Default: "Emergency"
 msgid "PloneMeeting_label_emergency"
 msgstr ""
@@ -1102,46 +1050,30 @@
 msgid "PloneMeeting_label_enableScanDocs"
 msgstr ""
 
 #. Default: "Enable user preferences"
 msgid "PloneMeeting_label_enableUserPreferences"
 msgstr ""
 
-#. Default: "Effective end date and hour"
-msgid "PloneMeeting_label_endDate"
-msgstr "Tatsächliches Enddatum und Enduhrzeit"
+#. Default: "Enabled annexes batch actions"
+msgid "PloneMeeting_label_enabledAnnexesBatchActions"
+msgstr ""
 
 #. Default: "Enforce advice mandatoriness"
 msgid "PloneMeeting_label_enforceAdviceMandatoriness"
 msgstr "Verpflichtende Kommentare erzwingen"
 
-#. Default: "Excused"
-msgid "PloneMeeting_label_excused"
-msgstr "Entschuldigt"
-
-#. Default: "Extraordinary session?"
-msgid "PloneMeeting_label_extraordinarySession"
-msgstr ""
-
-#. Default: "Number of the first item contained in this meeting"
-msgid "PloneMeeting_label_firstItemNumber"
-msgstr "Nummer des ersten TOP in dieser Sitzung"
-
 #. Default: "First linked vote values"
 msgid "PloneMeeting_label_firstLinkedVoteUsedVoteValues"
 msgstr ""
 
 #. Default: "Name of the folder linked to this configuration"
 msgid "PloneMeeting_label_folderTitle"
 msgstr "Name des Ordners der mit dieser Konfiguration verknüpft ist"
 
-#. Default: "Default deadline for validating late items for a given meeting"
-msgid "PloneMeeting_label_freezeDeadlineDefault"
-msgstr "Standardfrist um verspätete TOP für eine spezifische Sitzung zu validieren"
-
 #. Default: "Email of the functional administrator"
 msgid "PloneMeeting_label_functionalAdminEmail"
 msgstr "Email des Technischen Administrators"
 
 #. Default: "Name of the functional administrator"
 msgid "PloneMeeting_label_functionalAdminName"
 msgstr "Name des Technischen Administrators"
@@ -1182,18 +1114,14 @@
 msgid "PloneMeeting_label_historizeItemDataWhenAdviceIsGiven"
 msgstr ""
 
 #. Default: "Item attributes for which history must be kept"
 msgid "PloneMeeting_label_historizedItemAttributes"
 msgstr ""
 
-#. Default: "Meeting attributes for which history must be kept"
-msgid "PloneMeeting_label_historizedMeetingAttributes"
-msgstr ""
-
 #. Default: "Holidays"
 msgid "PloneMeeting_label_holidays"
 msgstr ""
 
 #. Default: "Include groups in charge defined on category"
 msgid "PloneMeeting_label_includeGroupsInChargeDefinedOnCategory"
 msgstr ""
@@ -1371,18 +1299,14 @@
 msgid "PloneMeeting_label_itemWithGivenAdviceIsNotDeletable"
 msgstr ""
 
 #. Default: "Workflow that dictates the life cycle of every item into this configuration"
 msgid "PloneMeeting_label_itemWorkflow"
 msgstr "Arbeitsablauf den jeder TOP in dieser Konfiguration durchlaufen muss"
 
-#. Default: "Items"
-msgid "PloneMeeting_label_items"
-msgstr "TOP"
-
 #. Default: "Columns to display for items within a meeting"
 #, fuzzy
 msgid "PloneMeeting_label_itemsListVisibleColumns"
 msgstr "Spalten die in TOP-Tabellen angezeigt werden können"
 
 #. Default: "Fields of the items to show/hide in the dashboards"
 msgid "PloneMeeting_label_itemsListVisibleFields"
@@ -1473,18 +1397,14 @@
 msgid "PloneMeeting_label_meetingColumns"
 msgstr "Anzuzeigende Spalten in Sitzungs-Listen"
 
 #. Default: "Interface allowing to use a specific Zope3 adapter for modifying the conditions defined on the transitions of the meeting workflow"
 msgid "PloneMeeting_label_meetingConditionsInterface"
 msgstr "Interface das es erlaubt einen speziellen Zope 3-Adapter zu verwenden um die Bedingungen für Statusübergänge im Sitzungs-Arbeitsablauf anzupassen."
 
-#. Default: "Identifier of the configuration's version that is linked to this meeting"
-msgid "PloneMeeting_label_meetingConfigVersion"
-msgstr "Bezeichnung der Version der Konfiguration die mit dieser Sitzung verknüpft ist."
-
 #. Default: "Meeting configs to clone items to"
 msgid "PloneMeeting_label_meetingConfigsToCloneTo"
 msgstr ""
 
 #. Default: "Title of the folder created in each user folder"
 #, fuzzy
 msgid "PloneMeeting_label_meetingFolderTitle"
@@ -1502,58 +1422,38 @@
 msgid "PloneMeeting_label_meetingManagersNotesEnd"
 msgstr ""
 
 #. Default: "MeetingManagers notes (suite)"
 msgid "PloneMeeting_label_meetingManagersNotesSuite"
 msgstr ""
 
-#. Default: "Meeting number (sequence number automatically attributed)"
-msgid "PloneMeeting_label_meetingNumber"
-msgstr "Sitzungsnummer (autmatische zugeordnete Sequenznummer)"
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations"
-msgstr "Beobachtungen"
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations2"
-msgstr "Beobachtungen"
-
 #. Default: "States of the meeting to insert an item into from everywhere"
 msgid "PloneMeeting_label_meetingPresentItemWhenNoCurrentMeetingStates"
 msgstr ""
 
 #. Default: "Meeting transition that triggers the insertion of this item as a recurring item"
 msgid "PloneMeeting_label_meetingTransitionInsertingMe"
 msgstr "Statusübergang der Sitzung der das Einfügen dieses TOPs als sich wiederholenden TOP auslöst."
 
 #. Default: "Workflow that dictates the life cycle of every meeting into this configuration"
 msgid "PloneMeeting_label_meetingWorkflow"
 msgstr "Arbeitsablauf den jede Sitzung in dieser Konfiguration durchlaufen muss"
 
-#. Default: "End date for meeting first part"
-msgid "PloneMeeting_label_midDate"
-msgstr ""
-
 #. Default: "Model adaptations"
 msgid "PloneMeeting_label_modelAdaptations"
 msgstr "Anpassung an das Datenmodell"
 
 #. Default: "Motivation"
 msgid "PloneMeeting_label_motivation"
 msgstr ""
 
 #. Default: "Next linked votes values"
 msgid "PloneMeeting_label_nextLinkedVotesUsedVoteValues"
 msgstr ""
 
-#. Default: "Non attendees"
-msgid "PloneMeeting_label_nonAttendees"
-msgstr ""
-
 #. Default: "Actions to execute on items of a meeting when a transition is triggered on that meeting"
 msgid "PloneMeeting_label_onMeetingTransitionItemActionToExecute"
 msgstr ""
 
 #. Default: "Transforms to apply to rich text fields of an item after a workflow transition"
 msgid "PloneMeeting_label_onTransitionFieldTransforms"
 msgstr ""
@@ -1570,14 +1470,18 @@
 msgid "PloneMeeting_label_oralQuestion"
 msgstr "Ist dieser TOP ist eine mündliche Anfrage?"
 
 #. Default: "Associated organizations order"
 msgid "PloneMeeting_label_orderedAssociatedOrganizations"
 msgstr ""
 
+#. Default: "Attendees selectable for committees"
+msgid "PloneMeeting_label_orderedCommitteeContacts"
+msgstr ""
+
 #. Default: "Selectable assembly members"
 msgid "PloneMeeting_label_orderedContacts"
 msgstr ""
 
 #. Default: "Ordered groups in charge"
 msgid "PloneMeeting_label_orderedGroupsInCharge"
 msgstr ""
@@ -1602,18 +1506,14 @@
 msgid "PloneMeeting_label_otherMeetingConfigsClonableToPrivacy"
 msgstr ""
 
 #. Default: "Owner of a annex decision may delete it when item is no more editable?"
 msgid "PloneMeeting_label_ownerMayDeleteAnnexDecision"
 msgstr ""
 
-#. Default: "Place"
-msgid "PloneMeeting_label_place"
-msgstr "Ort"
-
 #. Default: "Meeting places"
 msgid "PloneMeeting_label_places"
 msgstr "Sitzungsräume"
 
 #. Default: "Poll type"
 msgid "PloneMeeting_label_pollType"
 msgstr ""
@@ -1626,42 +1526,18 @@
 msgid "PloneMeeting_label_powerAdvisersGroups"
 msgstr ""
 
 #. Default: "Manage power observers"
 msgid "PloneMeeting_label_powerObservers"
 msgstr ""
 
-#. Default: "Date"
-msgid "PloneMeeting_label_preMeetingDate"
-msgstr "Datum"
-
-#. Default: "Default date for the pre-meeting"
-msgid "PloneMeeting_label_preMeetingDateDefault"
-msgstr "Standarddatum für die vorbereitende Sitzung"
-
-#. Default: "Place"
-msgid "PloneMeeting_label_preMeetingPlace"
-msgstr "Ort"
-
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations"
-msgstr "Bemerkungen zur vorbereitenden Sitzung"
-
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations2"
-msgstr "Bemerkungen zur vorbereitenden Sitzung"
-
 #. Default: "Previous item"
 msgid "PloneMeeting_label_predecessor"
 msgstr "Vorlage"
 
-#. Default: "Predefined title in the second language"
-msgid "PloneMeeting_label_predefinedTitle2"
-msgstr ""
-
 #. Default: "Preferred meeting"
 msgid "PloneMeeting_label_preferredMeeting"
 msgstr "Bevorzugte Sitzung"
 
 #. Default: "Privacy"
 msgid "PloneMeeting_label_privacy"
 msgstr "Vertraulichkeitsstufe"
@@ -1670,38 +1546,26 @@
 msgid "PloneMeeting_label_proposingGroup"
 msgstr "Vorschlagende Gruppe"
 
 #. Default: "Proposing group (Group in charge)"
 msgid "PloneMeeting_label_proposingGroupWithGroupInCharge"
 msgstr ""
 
-#. Default: "Observations for public meeting"
-msgid "PloneMeeting_label_publicMeetingObservations"
-msgstr ""
-
 #. Default: "Public URL"
 msgid "PloneMeeting_label_publicUrl"
 msgstr "Öffentliche URL"
 
-#. Default: "Default deadline for validating items for a given meeting"
-msgid "PloneMeeting_label_publishDeadlineDefault"
-msgstr "Standardfrist um TOP für eine spezifische Sitzung zu validieren"
-
 #. Default: "Questions"
 msgid "PloneMeeting_label_questioners"
 msgstr ""
 
 #. Default: "Item states into which events will be recorded in item's history"
 msgid "PloneMeeting_label_recordItemHistoryStates"
 msgstr "Stati der TOP für welche die Speicherung der History aktiviert ist"
 
-#. Default: "Meeting states into which events will be recorded in meeting's history"
-msgid "PloneMeeting_label_recordMeetingHistoryStates"
-msgstr ""
-
 #. Default: "Redirect to the next meeting"
 msgid "PloneMeeting_label_redirectToNextMeeting"
 msgstr ""
 
 #. Default: "Remove annexes previews on meeting closure"
 msgid "PloneMeeting_label_removeAnnexesPreviewsOnMeetingClosure"
 msgstr ""
@@ -1719,30 +1583,30 @@
 msgstr ""
 
 #. Default: "\"Restrict users\" mode"
 #, fuzzy
 msgid "PloneMeeting_label_restrictUsers"
 msgstr "'Eingeschränkter Benutzer' Modus"
 
-#. Default: "Observations for the secret meeting"
-msgid "PloneMeeting_label_secretMeetingObservations"
-msgstr ""
-
 #. Default: "Selectable advisers"
 msgid "PloneMeeting_label_selectableAdvisers"
 msgstr ""
 
 #. Default: "Groups that can be in copy for an item"
 msgid "PloneMeeting_label_selectableCopyGroups"
 msgstr "Gruppen welche eine Kopie für diesen TOP erhalten können"
 
 #. Default: "Selectable privacies"
 msgid "PloneMeeting_label_selectablePrivacies"
 msgstr ""
 
+#. Default: "Restrict selectable redefined position types to following positions"
+msgid "PloneMeeting_label_selectableRedefinedPositionTypes"
+msgstr ""
+
 #. Default: "Is group selectable in the plonegroup configuration panel?"
 msgid "PloneMeeting_label_selectable_for_plonegroup"
 msgstr ""
 
 #. Default: "Send to authority?"
 msgid "PloneMeeting_label_sendToAuthority"
 msgstr ""
@@ -1755,26 +1619,18 @@
 msgid "PloneMeeting_label_showItemKeywordsTargets"
 msgstr ""
 
 #. Default: "Signatories"
 msgid "PloneMeeting_label_signatories"
 msgstr ""
 
-#. Default: "Default signatures"
-msgid "PloneMeeting_label_signatures"
-msgstr "Standard-Unterschriften"
-
 #. Default: "Sort the tags alphabetically"
 msgid "PloneMeeting_label_sortAllItemTags"
 msgstr "Tags alphabetisch sortieren"
 
-#. Default: "Effective start date and hour"
-msgid "PloneMeeting_label_startDate"
-msgstr "Effektives Startdatum und Startuhrzeit"
-
 #. Default: "Meeting file sub types"
 msgid "PloneMeeting_label_subTypes"
 msgstr ""
 
 #. Default: "Taken over by"
 msgid "PloneMeeting_label_takenOverBy"
 msgstr ""
@@ -1783,23 +1639,14 @@
 msgid "PloneMeeting_label_templateUsingGroups"
 msgstr ""
 
 #. Default: "Checklist"
 msgid "PloneMeeting_label_textCheckList"
 msgstr ""
 
-# Meeting
-#. Default: "Title"
-msgid "PloneMeeting_label_title"
-msgstr "Titel"
-
-#. Default: "Title in the second language"
-msgid "PloneMeeting_label_title2"
-msgstr ""
-
 #. Default: "To discuss ?"
 msgid "PloneMeeting_label_toDiscuss"
 msgstr "Zu diskutieren?"
 
 #. Default: "Default value of the \"toDiscuss\" attribute for normal items"
 #, fuzzy
 msgid "PloneMeeting_label_toDiscussDefault"
@@ -1924,38 +1771,38 @@
 msgid "PloneMeeting_label_xhtmlTransformTypes"
 msgstr "Arten der Veränderungen für Richtext Felder"
 
 #. Default: "Reinitialise meeting number every year?"
 msgid "PloneMeeting_label_yearlyInitMeetingNumber"
 msgstr ""
 
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations"
-msgstr "Beobachtungen"
-
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations2"
-msgstr "Beobachtungen"
-
 #. Default: "Notes"
 msgid "PloneMeeting_notes"
 msgstr ""
 
 #. Default: "Document templates"
 msgid "PodTemplates"
 msgstr "Dokumentvorlagen"
 
 #. Default: "Position type"
 msgid "Position type"
 msgstr ""
 
+#. Default: "Position type to use"
+msgid "Position type to use"
+msgstr ""
+
 #. Default: "Position type to use as label for the signature."
 msgid "Position type to use as label for the signature."
 msgstr ""
 
+#. Default: "Position type to use for the attendee on this item."
+msgid "Position type to use for the attendee on this item."
+msgstr ""
+
 #. Default: "Preview detailed advice"
 msgid "Preview detailed advice"
 msgstr ""
 
 #. Default: "Preview of annexes were deleted upon meeting closure."
 msgid "Preview of annexes were deleted upon meeting closure."
 msgstr ""
@@ -1965,14 +1812,26 @@
 msgid "Previous review state"
 msgstr ""
 
 #. Default: "Recurring items"
 msgid "RecurringItems"
 msgstr "Sich wiederholende TOP"
 
+#. Default: "Redefine position for this attendee for this item"
+msgid "Redefine position for this attendee for this item"
+msgstr ""
+
+#. Default: "Redefined attendee position was removed."
+msgid "Redefined attendee position was removed."
+msgstr ""
+
+#. Default: "Redefined position"
+msgid "Redefined position"
+msgstr ""
+
 #. Default: "References of contained items have been updated."
 msgid "References of contained items have been updated."
 msgstr ""
 
 #. Default: "Reinitiatlize delay"
 msgid "Reinitiatlize delay"
 msgstr ""
@@ -1989,14 +1848,18 @@
 msgid "Remove inherited advice"
 msgstr ""
 
 #. Default: "Remove inherited advice and ask advice locally"
 msgid "Remove inherited advice and ask advice locally"
 msgstr ""
 
+#. Default: "Remove redefined attendee position for this item"
+msgid "Remove redefined attendee position for this item"
+msgstr ""
+
 #. Default: "Represented organizations"
 msgid "Represented organizations"
 msgstr ""
 
 #. Default: "Searches"
 msgid "Searches"
 msgstr ""
@@ -2049,14 +1912,18 @@
 msgid "Signature number"
 msgstr ""
 
 #. Default: "Signature position type"
 msgid "Signature position type"
 msgstr ""
 
+#. Default: "Specify a number to which this will be applied. Field default is current item number."
+msgid "Specify a number to which this will be applied. Field default is current item number."
+msgstr ""
+
 #. Default: "state"
 msgid "State"
 msgstr "Status"
 
 #. Default: "Style templates"
 msgid "Style templates"
 msgstr ""
@@ -2100,14 +1967,18 @@
 msgstr ""
 
 # plone.app.querystring
 #. Default: "The item, advice or meeting previous review state"
 msgid "The item, advice or meeting previous review state"
 msgstr ""
 
+#. Default: "The position of this attendee was changed for the ${number} following item(s)"
+msgid "The position of this attendee was changed for the ${number} following item(s)"
+msgstr ""
+
 #. Default: "There was an error during annex conversion, please contact system administrator."
 msgid "There was an error during annex conversion, please contact system administrator."
 msgstr ""
 
 #. Default: "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
 msgid "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
 msgstr ""
@@ -2148,18 +2019,14 @@
 msgid "This automatic advice has been asked by the application (shown by his title not being between brackets)"
 msgstr ""
 
 #. Default: "This copy group was set automatically by the application"
 msgid "This copy group was set automatically by the application"
 msgstr ""
 
-#. Default: "This is an extract of the comment, access full comment if necessary..."
-msgid "This is an extract of the comment, access full comment if necessary..."
-msgstr ""
-
 #. Default: "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 msgid "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 msgstr ""
 
 #. Default: "This label can not be removed as it is used by some items, for example ${item_url}"
 msgid "This label can not be removed as it is used by some items, for example ${item_url}"
 msgstr ""
@@ -2241,16 +2108,16 @@
 msgid "Votes are not completed for following ${number} ${polltype} item(s)"
 msgstr ""
 
 #. Default: "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 msgid "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 msgstr ""
 
-#. Default: "You cannot delete the default item template, but you can deactivate it if necessary!"
-msgid "You cannot delete the default item template, but you can deactivate it if necessary!"
+#. Default: "You cannot delete or move the default item template, but you can deactivate it if necessary!"
+msgid "You cannot delete or move the default item template, but you can deactivate it if necessary!"
 msgstr ""
 
 #. Default: "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 msgid "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 msgstr ""
 
 #. Default: "Not grouped meeting configurations"
@@ -2486,76 +2353,76 @@
 msgid "annexAdded_mail_subject"
 msgstr "${portalTitle} - ${meetingTitle} - Ein Anhang wurde gerade zu einem TOP zugefügt."
 
 #. Default: "If an annex is marked as \"Confidential\" by a meeting manager, following selected profiles will not be able to see it."
 msgid "annex_confidential_for_descr"
 msgstr ""
 
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item."
-msgid "annex_is_confidential_no"
+#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" could not be kept because it was not possible to find a corresponding annex type in the destination meeting configuration, please contact system administrator."
+msgid "annex_not_kept_because_no_available_annex_type_warning"
 msgstr ""
 
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item.  Click on the image to set it as confidential."
-msgid "annex_is_confidential_no_edit"
+#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" was not kept because using a scan_id, please contact system administrator."
+msgid "annex_not_kept_because_using_scan_id"
 msgstr ""
 
-#. Default: "The annex is confidential."
-msgid "annex_is_confidential_yes"
+#. Default: "Select for each optional annexes attributes which are only displayed or editable by MeetingManagers.  If an attribute is only displayed to MeetingManagers it will be automatically considered as only editable by MeetingManagers as well."
+msgid "annex_restrict_shown_and_editable_attributes_descr"
 msgstr ""
 
-#. Default: "The annex is confidential.  Click on the image to set it as not confidential."
-msgid "annex_is_confidential_yes_edit"
+#. Default: "Confidential"
+msgid "annex_term_confidential"
 msgstr ""
 
-#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" could not be kept because it was not possible to find a corresponding annex type in the destination meeting configuration, please contact system administrator."
-msgid "annex_not_kept_because_no_available_annex_type_warning"
+#. Default: "Not confidential"
+msgid "annex_term_not_confidential"
 msgstr ""
 
-#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" was not kept because using a scan_id, please contact system administrator."
-msgid "annex_not_kept_because_using_scan_id"
+#. Default: "Not publishable"
+msgid "annex_term_not_publishable"
 msgstr ""
 
-#. Default: "Select for each optional annexes attributes which are only displayed or editable by MeetingManagers.  If an attribute is only displayed to MeetingManagers it will be automatically considered as only editable by MeetingManagers as well."
-msgid "annex_restrict_shown_and_editable_attributes_descr"
+#. Default: "Not to print"
+msgid "annex_term_not_to_print"
 msgstr ""
 
-#. Default: "Title"
-msgid "annex_title"
-msgstr "Titel"
-
-#. Default: "The annex is not printable because it can not be converted (unsupported format or error during conversion).  Please use common office formats."
-msgid "annex_to_print_disabled"
+#. Default: "Not to sign"
+msgid "annex_term_not_to_sign"
 msgstr ""
 
-#. Default: "Automated (annexes are printed by the application)"
-msgid "annex_to_print_mode_automated"
+#. Default: "Publishable"
+msgid "annex_term_publishable"
 msgstr ""
 
-#. Default: "If print functionnality is enabled for annexes and an annex is set \"to print\", select here the to print mode that will be used : \"Manual\", means that the to print is just defined for information and that the printing process will be handled manually or \"Automated\", in this case, the application will generate a printable format for the annex (converted to images) so it can be inserted in a generated document."
-msgid "annex_to_print_mode_descr"
+#. Default: "Signed"
+msgid "annex_term_signed"
 msgstr ""
 
-#. Default: "For information (annexes are printed manually)"
-msgid "annex_to_print_mode_info"
+#. Default: "To print"
+msgid "annex_term_to_print"
 msgstr ""
 
-#. Default: "The annex will not be printed."
-msgid "annex_to_print_no"
+#. Default: "To sign"
+msgid "annex_term_to_sign"
 msgstr ""
 
-#. Default: "The annex will not be printed. Click on the image to print it."
-msgid "annex_to_print_no_edit"
+#. Default: "Title"
+msgid "annex_title"
+msgstr "Titel"
+
+#. Default: "Automated (annexes are printed by the application)"
+msgid "annex_to_print_mode_automated"
 msgstr ""
 
-#. Default: "The annex will be printed."
-msgid "annex_to_print_yes"
+#. Default: "If print functionnality is enabled for annexes and an annex is set \"to print\", select here the to print mode that will be used : \"Manual\", means that the to print is just defined for information and that the printing process will be handled manually or \"Automated\", in this case, the application will generate a printable format for the annex (converted to images) so it can be inserted in a generated document."
+msgid "annex_to_print_mode_descr"
 msgstr ""
 
-#. Default: "The annex will be printed. Click on the image not to print it."
-msgid "annex_to_print_yes_edit"
+#. Default: "For information (annexes are printed manually)"
+msgid "annex_to_print_mode_info"
 msgstr ""
 
 #. Default: "Annex type"
 msgid "annex_type"
 msgstr "Typ des Anhangs"
 
 #. Default: "Every item may be associated with a series of annexes. Some annexes may be specifically tied to the decision taken on the item. You can consult and modify here the annex types that are defined within this meeting configuration. An annex type is defined by a title, an icon (preferably of 16x16 pixels) and a predefined title. When users want to associate an annex to an item, they may choose, in a dropdown list, an annex type among those defined here and upload a file."
@@ -2582,24 +2449,16 @@
 msgid "annexes_preview_disabled"
 msgstr ""
 
 #. Default: "<span style='color: green;'>Annexes preview is enabled in the ${documentviewer_url}.</span>"
 msgid "annexes_preview_enabled"
 msgstr ""
 
-#. Default: "Signed annexes"
-msgid "annexes_signed_term"
-msgstr ""
-
-#. Default: "Annexes to print"
-msgid "annexes_to_print_term"
-msgstr ""
-
-#. Default: "Annexes to sign"
-msgid "annexes_to_sign_term"
+#. Default: "Annexes types are hidden by default, you can ${force_display} of it (may take some time)."
+msgid "annexes_types_force_display_descr"
 msgstr ""
 
 #. Default: "Application users"
 msgid "app_users"
 msgstr ""
 
 #. Default: "Are you sure?"
@@ -2635,18 +2494,14 @@
 msgid "assemblyMember"
 msgstr "Sitzungsteilnehmer"
 
 #. Default: "Absents as defined on the linked meeting"
 msgid "assembly_absents_defined_on_meeting"
 msgstr ""
 
-#. Default: "Define here people that were absents (not excused) for the meeting"
-msgid "assembly_absents_meeting_descr"
-msgstr ""
-
 #. Default: "Assembly and signatures"
 msgid "assembly_and_signatures"
 msgstr ""
 
 #. Default: "Assembly as defined on the linked meeting"
 msgid "assembly_defined_on_meeting"
 msgstr ""
@@ -2656,26 +2511,18 @@
 msgid "assembly_descr"
 msgstr "Definieren Sie hier die Standardsitzungsteilnehmer (Sie können zum Beispiel eine Liste von Nach- und Vornamen getrennt durch Semikolons oder Zeilenumbrüche eingeben) diese werden im 'Versammlung'-Feld jeder neu erstellten Sitzung automatisch eingefügt. Wenn Sie eine strukturiertere Art benötigen um Sitzungsteilnehmer zu verwalten wie abwesend, anwesend und entschuldigt, füllen Sie dieses Feld nicht aus. Erstellen Sie dann im Tab 'Daten', spezielle Benutzer, die verschiedene Attribute haben können wie Sitzungsteilnehmer, Unterschreiben, Abstimmen. Diese können dann in den Sitzungen ausgewählt werden."
 
 #. Default: "Excused as defined on the linked meeting"
 msgid "assembly_excused_defined_on_meeting"
 msgstr ""
 
-#. Default: "Define here people that were excused for the meeting"
-msgid "assembly_excused_meeting_descr"
-msgstr ""
-
 #. Default: "Guests as defined on the linked meeting"
 msgid "assembly_guests_defined_on_meeting"
 msgstr ""
 
-#. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
-msgid "assembly_meeting_descr"
-msgstr ""
-
 #. Default: "Using attribute(s) \"itemExcused\" and/or \"itemAbsents\" requires the use of attribute \"assembly\"."
 msgid "assembly_required"
 msgstr ""
 
 #. Default: "Define here the default assembly staves (for example you may type a list of names and first names separated by colons or new lines) that will be automatically selected on newly created meetings."
 msgid "assembly_staves_descr"
 msgstr ""
@@ -2766,14 +2613,18 @@
 msgid "budgetimpacteditors"
 msgstr ""
 
 #. Default: "You can not access this item"
 msgid "can_not_access_this_item"
 msgstr ""
 
+#. Default: "Assembly and signatures : you can not use same signature number several times."
+msgid "can_not_define_several_same_signature_number"
+msgstr ""
+
 #. Default: "You can not define two rows for the same meeting configuration!"
 msgid "can_not_define_two_rows_for_same_meeting_config"
 msgstr ""
 
 #. Default: "You can not remove/disable a function that is used by an item in the configuration.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_config_meetingitem"
 msgstr ""
@@ -2782,30 +2633,34 @@
 msgid "can_not_delete_plone_group_meetingconfig"
 msgstr ""
 
 #. Default: "You can not remove/disable a function that is used by an item in the application.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_meetingitem"
 msgstr ""
 
-#. Default: "You can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
 msgid "can_not_remove_attendee_redefined_on_items"
 msgstr ""
 
-#. Default: "You can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
 msgid "can_not_remove_public_voter_voted_on_items"
 msgstr ""
 
-#. Default: "You can not unselect a voter that already voted on a secret vote item."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a secret vote item."
 msgid "can_not_remove_secret_voter_voted_on_items"
 msgstr ""
 
 #. Default: "This item can no more be returned to the meeting managers because the meeting is in a state not authorizing it (${meetingState})."
 msgid "can_not_return_to_meeting_because_of_meeting_state"
 msgstr ""
 
+#. Default: "You can not select \"No committee\" and a committee."
+msgid "can_not_select_no_committee_and_committee"
+msgstr ""
+
 #. Default: "You can not select an adviser that is already displayed on the item as an inherited advice.  If you need to ask this advice again, you need to remove the inherited advice (as a MeetingManager or a Manager) then select advice again."
 msgid "can_not_select_optional_adviser_same_group_as_inherited"
 msgstr ""
 
 #. Default: "You can not select several values for the same group.  Please select a single value for the same group among available ones."
 msgid "can_not_select_several_optional_advisers_same_group"
 msgstr ""
@@ -2839,18 +2694,14 @@
 msgid "categories_descr"
 msgstr "Jeder TOP in dieser Sitzungs-Konfiguration kann nur zu einer Kategorie gehören. Die Kategorien werden hier mit einem Titel und einer Beschreibung definiert. Die Reihenfolge in der sie in diesem Ordner erscheinen ist wichtig. XXX"
 
 #. Default: "the \"Folder contents view\""
 msgid "categories_folder_contents_view"
 msgstr ""
 
-#. Default: "force display"
-msgid "categories_force_display"
-msgstr ""
-
 #. Default: "You can ${force_display} of every categories (may take some time)."
 msgid "categories_force_display_descr"
 msgstr ""
 
 #. Default: "You may use the ${folder_contents_link} to manage elements order."
 msgid "categories_use_folder_contents"
 msgstr ""
@@ -3000,14 +2851,34 @@
 msgid "clone_to"
 msgstr ""
 
 #. Default: "Your configuration says can not correct this closed meeting, contact your system administrator if you want to change this."
 msgid "closed_meeting_not_correctable_by_config"
 msgstr ""
 
+#. Default: "${title} (${number}&nbsp;s.)"
+msgid "committee_title_with_abbr_suppl"
+msgstr ""
+
+#. Default: "${title} (${number}&nbsp;supplement)"
+msgid "committee_title_with_suppl"
+msgstr ""
+
+#. Default: "Committees"
+msgid "committees"
+msgstr ""
+
+#. Default: "Define committees that will be useable on meetings and items (you also need to enable \"Committees\" on the meeting in the [Data] tab). This will show a \"Committees\" table on the meeting and will be also managed on the item. <br />There are 2 ways to manage committees on the item, either manually or automatically:<ul><li>Manually: just define committees, this will create a multiselection box on the item and users may select it.  It is possible to use the column \"Restrict to\" to define which proposing groups will be able to select the committee;</li><li>Automatically: use the column \"Auto from\" to define which committees to associate to the item depending on proposing group, category or classifier. A MeetingManager is nevertheless able to edit the committee on the item.</li></ul>. These 2 ways are mutually exclusive, if you select values in the \"auto_from\" columb here under, the \"Automatic\" mode will be used."
+msgid "committees_descr"
+msgstr ""
+
+#. Default: "Using a \"Committees\" field requires the use of attribute \"Committees (committees)\"."
+msgid "committees_required"
+msgstr ""
+
 #. Default: "Complete"
 msgid "completeness_complete"
 msgstr ""
 
 #. Default: "Evaluation asked again"
 msgid "completeness_evaluation_asked_again"
 msgstr ""
@@ -3094,14 +2965,18 @@
 msgid "copyGroups_mail_body"
 msgstr ""
 
 #. Default: "${meetingConfigTitle} - You have been carbon copied - ${itemTitle}"
 msgid "copyGroups_mail_subject"
 msgstr ""
 
+#. Default: "These groups will have read access to the item in following states: ${states}.\nWhen icon is green, this means that copy groups have access to the item.\nWhen the label \"[auto]\" is displayed next to the group title, it means that the group was set as copy group automatically by the application."
+msgid "copy_groups_help_msg"
+msgstr ""
+
 #. Default: " "
 msgid "copy_groups_item_descr"
 msgstr "Wählen Sie hier die Gruppen welche diesen TOP sehen soll"
 
 #. Default: "The cloned item could not be presented to a meeting in the \"${destMeetingConfigTitle}\" configuration, no suitable meeting could be found."
 msgid "could_not_present_item_no_meeting_accepting_items"
 msgstr ""
@@ -3288,14 +3163,34 @@
 msgid "delay_of_x_days"
 msgstr ""
 
 #. Default: "Select here the days a computed delay can not ends with.  If a computed delay is ending on one of selected week day, the delay will be extend to next available day.  <span style='color: red;'>If you change this parameter, do not forget to run \"Update items and meetings\"!</span>"
 msgid "delay_unavailable_end_days_descr"
 msgstr ""
 
+#. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
+msgid "descr_assembly"
+msgstr ""
+
+#. Default: "<span style='color: red;'>WARNING, this field is managed by the application and it's value will be \"-1\" until the meeting is frozen, then it will be computed automatically. Do only change it manually when necessary (in general this should never happen). This field is only editable and viewable by meeting managers</span>"
+msgid "descr_config_field_reserved_to_meeting_managers"
+msgstr ""
+
+#. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
+msgid "descr_field_reserved_to_meeting_managers"
+msgstr ""
+
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
+msgid "descr_field_vieawable_by_everyone"
+msgstr ""
+
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
+msgid "descr_field_vieawable_by_everyone_once_meeting_decided"
+msgstr ""
+
 #. Default: "You are just able to see visible elements here. Please consult the \"manage\" box here opposite."
 #, fuzzy
 msgid "description_only_see_visible_items"
 msgstr "Sie können sichtbare Elemente nur hier sehen."
 
 #. Default: "By default only MeetingManagers will see the available items panel on a meeting as long as the meeting is accepting items.  This let's you show this panel to selected profiles.  Note that if you enable this, the meeting view will be displayed slower."
 msgid "display_available_items_to_descr"
@@ -3394,14 +3289,22 @@
 msgid "enable_scan_docs_descr"
 msgstr ""
 
 #. Default: "If you check this box, users will be able to access a screen for modifying their preferences. While powerful, some may think it exposes too much complexity to users."
 msgid "enable_user_preferences_descr"
 msgstr ""
 
+#. Default: "Select the batch actions that will be displayed on the table listing annexes"
+msgid "enabled_annexes_batch_actions_descr"
+msgstr ""
+
+#. Default: "The meeting end date must occur after the start date and meeting date."
+msgid "end_date_before_meeting_date"
+msgstr ""
+
 #. Default: "When advice mandatoriness is enforced, an item can't be inserted into a meeting unless all mandatory advices are given and positive."
 msgid "enforce_advice_mandatoriness_descr"
 msgstr "Wenn die Pflichtkommentare eingerichtet sind, kann ein TOP errst zu einer Sitzung hinzugefügt werden, wenn alle Kommentare abgegeben und positiv sind. "
 
 #. Default: "You can not encode more than ${max_voters} voters."
 msgid "error_can_not_encode_more_than_max_voters"
 msgstr ""
@@ -3422,14 +3325,30 @@
 msgid "error_certified_signatures_invalid_dates"
 msgstr ""
 
 #. Default: "Signatures must be ordered by signature number, please check and order signature using the arrows on the right of the table."
 msgid "error_certified_signatures_order"
 msgstr ""
 
+#. Default: "You can not remove a configuration that was already used, removed configuration \"${committee_label}\" is used for example by item at ${url}.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committee_row_id_removed_already_used"
+msgstr ""
+
+#. Default: "You can not define values for the \"auto_from\" and \"using_groups\" columns, their use is multually exclusive.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committees_mutually_exclusive_auto_from_and_using_groups"
+msgstr ""
+
+#. Default: "Default poll type must be among used poll types"
+msgid "error_default_poll_type_must_be_among_used_poll_types"
+msgstr ""
+
+#. Default: "First linked vote used votes values must be among used vote values"
+msgid "error_first_linked_vote_used_vote_values_must_be_among_used_vote_values"
+msgstr ""
+
 #. Default: "You may not remove a list type that is currently used by an item, check for example : ${url}."
 msgid "error_list_types_identifier_removed_already_used"
 msgstr ""
 
 #. Default: "You may not remove the default list types (\"normal\" and \"late\")."
 msgid "error_list_types_missing_default"
 msgstr ""
@@ -3438,14 +3357,22 @@
 msgid "error_list_types_same_identifier"
 msgstr ""
 
 #. Default: "You may only use lowercase letters for identifier."
 msgid "error_list_types_wrong_identifier_format"
 msgstr ""
 
+#. Default: "Next linked votes used vote values must be among used vote values"
+msgid "error_next_linked_votes_used_vote_values_must_be_among_used_vote_values"
+msgstr ""
+
+#. Default: "Some selected values are no more selectable (no more selected in the \"Ordered committees contacts\" field), please check value \"${hp_title}\".  You can not select \"No committee\" and a committee.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_value_removed_used_in_committees_field"
+msgstr ""
+
 #. Default: "An advice was added or updated on an item (notify the \"Creators\")"
 #, fuzzy
 msgid "event_add_advice"
 msgstr "Es wurde ein Kommentar zu einem TOP veröffentlicht oder aktualisiert."
 
 #. Default: "An advice was added or updated on an item (notify the \"Owner\")"
 msgid "event_add_advice_owner"
@@ -3562,28 +3489,36 @@
 msgid "fastedit_save_changes"
 msgstr ""
 
 #. Default: "Please fill this field."
 msgid "field_required"
 msgstr "Bitte füllen Sie dieses Feld aus."
 
-#. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
-msgid "field_reserved_to_meeting_managers_descr"
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once item is decided</span>"
+msgid "field_vieawable_by_everyone_once_item_decided_descr"
 msgstr ""
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
-msgid "field_vieawable_by_everyone_descr"
+#. Default: "Assembly and signatures"
+msgid "fieldset_assembly"
 msgstr ""
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once item is decided</span>"
-msgid "field_vieawable_by_everyone_once_item_decided_descr"
+#. Default: "Committees"
+msgid "fieldset_committees"
 msgstr ""
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
-msgid "field_vieawable_by_everyone_once_meeting_decided_descr"
+#. Default: "Dates and data"
+msgid "fieldset_dates_and_data"
+msgstr ""
+
+#. Default: "Informations"
+msgid "fieldset_informations"
+msgstr ""
+
+#. Default: "Parameters"
+msgid "fieldset_parameters"
 msgstr ""
 
 #. Default: "Please choose a file by clicking on the \"Browse\" button."
 #, fuzzy
 msgid "file_required"
 msgstr "Bitte wählen Sie eine Datei aus indem Sie auf den 'Durchsuchen'-Knopf klicken."
 
@@ -3596,21 +3531,17 @@
 msgstr ""
 
 #. Default: "In the application folder of every member, a sub-folder is created for each meeting configuration. The name of this sub-folder is defined here."
 #, fuzzy
 msgid "folder_title_descr"
 msgstr "Im PloneMeeting-Ordner jedes Nutzers wird für jede Sitzungs-Konfiguration ein Unterordner erstellt. Der Name dieses Unterordners wird hier definiert."
 
-#. Default: "For the administrator only"
-msgid "for_admin_only"
-msgstr "Nur für den Administrator"
-
-#. Default: "Specify here the deadline for validating late items to be inserted in a given meeting.  Leave the field empty not to use this functionality."
-msgid "freeze_deadline_default_descr"
-msgstr "Spezifizieren Sie hier die Frist um verspätete TOP in eine definierte Sitzung hinzufügen zu können"
+#. Default: "force display"
+msgid "force_display"
+msgstr ""
 
 #. Default: "<p>PloneMeeting body in HTML format.</p>"
 msgid "front_page_body"
 msgstr ""
 
 #. Default: "Manage here your official meetings."
 msgid "front_page_description"
@@ -3714,14 +3645,18 @@
 msgstr ""
 
 # Other
 #. Default: "Check/uncheck items"
 msgid "helpSelectItemsIcon"
 msgstr ""
 
+#. Default: "This is the date the advice was originally given, this will change when the advice will be considered \"Given\" in a state where it is no more editable"
+msgid "help_given_on_before_started_on"
+msgstr ""
+
 #. Default: "No preview available because this type of file can not be converted.  Please use common office formats.  You can download the file, look in the \"actions\" column."
 msgid "help_no_preview_available"
 msgstr ""
 
 #. Default: "No preview available because there was an error during conversion to a previewable format.  Please contact system administrator that will have access to more debugging informations."
 msgid "help_no_preview_available_conversion_error"
 msgstr ""
@@ -3762,18 +3697,14 @@
 msgid "historize_item_data_when_advice_is_given_descr"
 msgstr ""
 
 #. Default: "For every field you select here, the application will keep track of any change on any item, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
 msgid "historized_item_attrs_descr"
 msgstr ""
 
-#. Default: "For every field you select here, the application will keep track of any change on any meeting, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
-msgid "historized_meeting_attrs_descr"
-msgstr ""
-
 #. Default: "See changes"
 msgid "history_changes"
 msgstr ""
 
 #. Default: "Deleted by ${userName}"
 msgid "history_delete"
 msgstr ""
@@ -3790,15 +3721,15 @@
 msgid "holidays_date_not_ascending_error"
 msgstr ""
 
 #. Default: "These dates will be used to compute advices delays.  <span style='color: red;'>If you change this parameter and modified dates are interacting with some existing advice delays, do not forget to run \"Update items and meetings\"!</span>"
 msgid "holidays_descr"
 msgstr ""
 
-#. Default: "You removed a date that is currently in use!"
+#. Default: "You removed a date that is currently in use! Check item at ${item_url}"
 msgid "holidays_removed_date_in_use_error"
 msgstr ""
 
 #. Default: "There are not enough holidays defined in the configuration.  These days are used for advice delay computation.  This warning appear when last holiday defined in the configuration is in less than 60 days. Contact you system administrator if necessary."
 msgid "holidays_warning_message"
 msgstr ""
 
@@ -3819,14 +3750,18 @@
 msgstr ""
 
 #. Default: "This application allows you to manage your official meetings."
 #, fuzzy
 msgid "hs_welcome_body"
 msgstr "Dieser Site ermöglicht Ihnen ihre offiziellen Sitzungen zu verwalten. "
 
+#. Default: "iA.Delib documentation"
+msgid "iA.Delib documentation"
+msgstr ""
+
 #. Default: "Azur"
 msgid "icon_color_azur"
 msgstr ""
 
 #. Default: "Black"
 msgid "icon_color_black"
 msgstr ""
@@ -4448,38 +4383,26 @@
 
 # Mails (item-related)
 #. Default: "${meetingConfigTitle} - A \"late\" item has been validated."
 #, fuzzy
 msgid "lateItem_mail_subject"
 msgstr "${portalTitle} - Ein 'verspäteter' TOP wurde bestätigt."
 
-#. Default: "Items presented tardily"
-msgid "late_presented_items"
-msgstr "TOP die nach der Veröffentlichung der Sitzung präsentiert wurden"
-
 #. Default: "--- Do nothing, let the item in the workflow initial state ---"
 msgid "let_item_in_initial_state"
 msgstr ""
 
 #. Default: "Linked items (${auto_linked_items})"
 msgid "linked_items"
 msgstr ""
 
 #. Default: "Linked items, ${auto_linked_items} automatically and ${manually_linked_items} manually"
 msgid "linked_items_with_manually_linked_items"
 msgstr ""
 
-#. Default: "Late"
-msgid "list_type_late"
-msgstr ""
-
-#. Default: "Normal"
-msgid "list_type_normal"
-msgstr ""
-
 #. Default: "Types of list of items that will be available when an item is linked to a meeting."
 msgid "list_types_descr"
 msgstr ""
 
 #. Default: "Size"
 msgid "listingheader_size"
 msgstr "Größe"
@@ -4578,36 +4501,16 @@
 msgid "meeting_annex_confidential_visible_for_descr"
 msgstr ""
 
 #. Default: "Choose here which page will be shown after logon."
 msgid "meeting_app_default_view_descr"
 msgstr "Wählen Sie hier aus welche Seite nach dem Einloggen angezeigt werden soll."
 
-#. Default: "Assembly"
-msgid "meeting_assembly"
-msgstr "Sitzung"
-
-#. Default: "Absents"
-msgid "meeting_assemblyAbsents"
-msgstr ""
-
-#. Default: "Excused"
-msgid "meeting_assemblyExcused"
-msgstr ""
-
-#. Default: "Guests"
-msgid "meeting_assemblyGuests"
-msgstr ""
-
-#. Default: "Proxies"
-msgid "meeting_assemblyProxies"
-msgstr ""
-
-#. Default: "Staves"
-msgid "meeting_assemblyStaves"
+#. Default: "Meeting assembly (${number_of_attendees}) and signatories (${number_of_signatories})"
+msgid "meeting_attendees_and_signatories"
 msgstr ""
 
 #. Default: "Choose here which columns to display when listing meetings (ie, when displaying the list of available meetings or decisions, or when performing custom searches)."
 msgid "meeting_columns_descr"
 msgstr "Wählen Sie hier die Spalten aus, die Sie bei den Sitzungs-Listen anzeigen wollen (z.B., bei der Liste der vorhandenen Sitzung oder Beschlüsse, oder bei Benutzerdefinierten Suchen)."
 
 #. Default: "Similarly to interfaces defined for items, the conditions expressed on the transitions of the meeting workflow may be configured through the development of another Plone product into which you must:<ul><li>create a Python interface that inherits from interface Products.PloneMeeting.interfaces.IMeetingWorkflowConditions (you must enter the full package name of this interface in the field below);</li><li>create and declare in ZCML an adapter that adapts the interface  Products.PloneMeeting.interfaces.IMeeting to the interface you have defined in the previous step.</li></ul>Your adapter may inherit from the default adapter Products.PloneMeeting.Meeting.MeetingWorkflowConditions: it will allow you to override only methods for which you want an altered behaviour. All the methods proposed by the interface Products.PloneMeeting.interfaces.IMeetingWorkflowConditions are documented."
@@ -4653,22 +4556,14 @@
 msgid "meeting_organizations"
 msgstr ""
 
 #. Default: "When an item is inserted in a meeting from everywhere (so not when on a meeting view), this will take the very next meeting still accepting items.  Define here states to take into account to get this very next meeting."
 msgid "meeting_present_item_when_no_current_meeting_states_descr"
 msgstr ""
 
-#. Default: "Signatories"
-msgid "meeting_signatories"
-msgstr "Unterzeichner"
-
-#. Default: "Signatures"
-msgid "meeting_signatures"
-msgstr "Unterschrift"
-
 #. Default: "You can consult this meeting at ${objectUrl}."
 msgid "meeting_state_changed_default_mail_body"
 msgstr ""
 
 # Mails (meeting-related)
 # Default translation for mails sent upon meeting transition
 # This default is used if no accurate translation can be found. We will try for example to translate
@@ -4760,26 +4655,18 @@
 msgid "metadata"
 msgstr "Metadaten"
 
 #. Default: "Select here some standard adaptations that can be applied to data structures."
 msgid "model_adaptations_descr"
 msgstr "Wählen Sie hier einige Standard Anpassungen die an die Datenstruktur angewendet werden können"
 
-#. Default: "Move the item down"
-msgid "move_item_down"
-msgstr "TOP nach unten bewegen"
-
-#. Default: "Move item to given position"
+#. Default: "Save item number (you may also use the [Enter] key)"
 msgid "move_item_to_given_position"
 msgstr ""
 
-#. Default: "Move the item up"
-msgid "move_item_up"
-msgstr "TOP nach oben bewegen"
-
 #. Default: "Moves this item to the position that precedes the number you have introduced besides. If you want to move the item at the end of the list, specify the number of the last item plus one."
 msgid "move_several"
 msgstr "Bewegt den TOP zu der Position die Sie angegeben haben. Wenn Sie den TOP zum Ende der Liste bewegen wollen, geben Sie die Nummer des letzten TOPs an plus eins ein."
 
 #. Default: "Negative"
 msgid "negative"
 msgstr "Negativ"
@@ -4796,35 +4683,43 @@
 msgid "nil"
 msgstr "Null"
 
 #. Default: "No annex is currently defined for this element."
 msgid "no_annexes"
 msgstr "Für diesen TOP ist kein Anhang vorhanden."
 
-#. Default: "No annexes to print"
-msgid "no_annexes_to_print_term"
-msgstr ""
-
-#. Default: "Annexes not to sign"
-msgid "no_annexes_to_sign_term"
-msgstr ""
-
 #. Default: "Attributes \"assembly\" and \"attendees\" can't be used together."
 #, fuzzy
 msgid "no_assembly_and_attendees"
 msgstr "Die Attribute 'Standard Sitzungsteilnehmer' und 'Anwesende' können nicht gleichzeitig benutzt werden."
 
 #. Default: "No category is currently defined."
 msgid "no_category"
 msgstr "Derzeit ist keine Kategorie definiert."
 
 #. Default: "No classifier is currently defined."
 msgid "no_classifier"
 msgstr ""
 
+#. Default: "NC"
+msgid "no_committee_term_title_acronym"
+msgstr ""
+
+#. Default: "No committee"
+msgid "no_committee_term_title_label"
+msgstr ""
+
+#. Default: "Attributes \"committees_assembly\" and \"committees_attendees\" can't be used together."
+msgid "no_committees_assembly_and_committees_attendees"
+msgstr ""
+
+#. Default: "Attributes \"committees_sigantures\" and \"committees_signatories\" can't be used together."
+msgid "no_committees_signatures_and_committees_signatories"
+msgstr ""
+
 #. Default: "None"
 msgid "no_config_group"
 msgstr ""
 
 #. Default: "No emergency"
 msgid "no_emergency"
 msgstr ""
@@ -4849,31 +4744,28 @@
 msgid "no_meeting_file_type"
 msgstr "Derzeit ist kein Typ für Anhänge definiert."
 
 #. Default: "No special user is currently defined."
 msgid "no_meeting_user"
 msgstr "Derzeit ist kein Spezieller Benutzer definiert."
 
-#. Default: "No items."
-msgid "no_meetingitems"
-msgstr "Keine TOP."
-
 #. Default: "No POD template is currently defined."
 msgid "no_pod_folder"
 msgstr "Es ist zurzeit keine POD-Vorlage definiert"
 
 #. Default: "Attributes \"proposingGroupWithGroupInCharge\" and \"groupsInCharge\" can't be used together."
 msgid "no_proposingGroupWithGroupInCharge_and_groupsInCharge"
 msgstr ""
 
 #. Default: "No recurring item is currently defined."
 msgid "no_recurring_item"
 msgstr "Derzeit sind keine wiederkehrenden TOP definiert."
 
-#. Default: "No visible item for now."
+#. Default: "You do not have access to these items."
+#, fuzzy
 msgid "no_shown_items"
 msgstr "Im Moment keine sichtbaren TOP."
 
 #. Default: "Attributes \"signatures\" and \"signatories\" can't be used together."
 #, fuzzy
 msgid "no_signatories_and_signatures"
 msgstr "Die Attribute 'Unterschriften' und 'Unterzeichner' können nicht gleichzeitig benutzt werden."
@@ -4902,14 +4794,22 @@
 msgid "normal"
 msgstr ""
 
 #. Default: "You are a registered user but your account has not been activated yet. Please contact the system administrator."
 msgid "notPloneMeetingUser"
 msgstr "Sie sind ein registrierter Benutzer aber Ihr Konto wurde noch nicht aktiviert. Kontaktieren Sie bitte den Administrator."
 
+#. Default: "Not able to find a meeting to present this item into.  Only meetings in the future are taken into account, check configuration if necessary"
+msgid "not_able_to_find_meeting_to_present_item_into"
+msgstr ""
+
+#. Default: "Not confidential annexes"
+msgid "not_confidential_annexes"
+msgstr ""
+
 #. Default: "Not given yet"
 msgid "not_given"
 msgstr "Noch nicht abgegeben"
 
 #. Default: "Not to be cloned to anywhere"
 msgid "not_to_be_cloned_to_term"
 msgstr ""
@@ -4926,14 +4826,22 @@
 msgid "nothing_to_do"
 msgstr "Nichts zu unternehmen."
 
 #. Default: "notify users able to view the element"
 msgid "notify_users_able_to_view_element"
 msgstr ""
 
+#. Default: "${number}st"
+msgid "num_part_st"
+msgstr ""
+
+#. Default: "${number}th"
+msgid "num_part_th"
+msgstr ""
+
 #. Default: "Total number of voters"
 msgid "number_of_voters"
 msgstr ""
 
 #. Default: "Observer"
 msgid "observer"
 msgstr ""
@@ -4942,14 +4850,18 @@
 msgid "observers"
 msgstr "Beobachter"
 
 #. Default: "Follow all associated groups order"
 msgid "on_all_associated_groups"
 msgstr ""
 
+#. Default: "Follow all committees order"
+msgid "on_all_committees"
+msgstr ""
+
 #. Default: "Follow all groups order"
 msgid "on_all_groups"
 msgstr "Der Gruppensortierung folgen"
 
 #. Default: "Follow categories order"
 msgid "on_categories"
 msgstr "Der Kategoriensortierung folgen"
@@ -5031,14 +4943,18 @@
 msgid "oral_question_item_descr"
 msgstr ""
 
 #. Default: "If this field is left empty, selectable associated organizations are every organizations selected in the plonegroup configuration panel.  Here you may select associated organizations in a particular order including organizations that are not selected in the plonegroup configuration panel.  This is only relevant if the 'Associated groups' field is enabled on items."
 msgid "ordered_associated_organizations_descr"
 msgstr ""
 
+#. Default: "Select here attendees that will be selectable in the \"Attendees\" column of defined committees here under.  <span style='color: red;'>If you select/unselect values, you need to save first then edit again for these values to appear/disappear if field \"Committees\" here under.</span>"
+msgid "ordered_committee_contacts_descr"
+msgstr ""
+
 #. Default: "Select here contacts that will be usable to manage meeting attendees.  The contacts order defined here will be the default order when creating a new meeting."
 msgid "ordered_contacts_descr"
 msgstr ""
 
 #. Default: "If this field is left empty, selectable groups in charge are every organizations selected in the plonegroup configuration panel.  Here you may select groups in charge in a particular order.  This is only relevant if the 'Groups in charge' field is enabled on items."
 msgid "ordered_groups_in_charge_descr"
 msgstr ""
@@ -5071,22 +4987,26 @@
 msgid "owner_may_delete_annex_decision_descr"
 msgstr ""
 
 #. Default: "Mark this person absent for this item"
 msgid "person_byebye"
 msgstr ""
 
+#. Default: "Redefine position for attendee for this item"
+msgid "person_redefine_attendee_position"
+msgstr ""
+
+#. Default: "Remove redefined position for attendee for this item"
+msgid "person_remove_redefined_attendee_position"
+msgstr ""
+
 #. Default: "Remove this person from absents for this item"
 msgid "person_welcome"
 msgstr ""
 
-#. Default: "Please encode this other place."
-msgid "place_other_required"
-msgstr "Geben Sie bitte einen Namen für diesen anderen Ort an."
-
 #. Default: "Enter here some default places where meetings occur. There must be one place per line. The first one will be the default one."
 msgid "places_descr"
 msgstr "Geben Sie hier einige feste Orte ein wo Sitzungen stattfinden. Pro Linie ein Ort. Der erste Ort ist der Standard Ort."
 
 #. Default: "You are about to delete this meeting and all included items. Are you sure?"
 msgid "plonemeeting_delete_meeting_confirm_message"
 msgstr "Sie sind dabei diese Sitzung und alle sich darin befindende TOP zu löschen. Sind Sie sicher?"
@@ -5282,22 +5202,14 @@
 msgid "powerobservers"
 msgstr ""
 
 #. Default: "The preparatory meeting must occur before the meeting."
 msgid "pre_date_after_meeting_date"
 msgstr "Die vorbereitende Sitzung muss vor der Sitzung stattfinden."
 
-#. Default: "Preparatory meeting"
-msgid "pre_meeting"
-msgstr "Vorbereitende Sitzung"
-
-#. Default: "Specify here the date of the pre-meeting, relative to its meeting, in the same format as fields above.  Leave the field empty not to use this functionality."
-msgid "pre_meeting_date_default_descr"
-msgstr "Definieren Sie hier das Datum der Vorbereitungssitzung, relativ zur betroffenen Sitzung, im selben Format wie die Felder hier oben."
-
 #. Default: "If this is a normal item and you want it to be inserted in any availale meeting, just select \"No preference\" value.  Selecting a date is for 2 usecases : this will make the item not presentable to the meetings before selected one, or if the selected meeting is \"frozen\", this will make current item considered as \"late\" item presentable in the selected frozen meeting.  Indeed, the only way to insert an item in a frozen meeting is to select this meeting as preferred meeting."
 msgid "preferred_meeting_descr"
 msgstr ""
 
 #. Default: "Pre-validator"
 msgid "prereviewer"
 msgstr ""
@@ -5342,35 +5254,34 @@
 msgid "public"
 msgstr ""
 
 #. Default: "Public meeting (heading)"
 msgid "public_heading"
 msgstr ""
 
-#. Default: "Specify here the deadline for validating items to be inserted in a given meeting. You need to express this deadline relative to the meeting date. For example, \"5.9:30\" (do not type quotes) means: \"5 days before the meeting date, at 9:30.\".  Leave the field empty not to use this functionality."
-#, fuzzy
-msgid "publish_deadline_default_descr"
-msgstr "Definieren Sie hier die Frist bis wann TOP validiert sein müssen um in eine Sitzung aufgenommen werden zu können. Diese Frist muss realtiv zum Datum der Sitzung eingegeben werden. Z.B., '5.9:30' (Ohne Anführungszeichen eintragen) bedeutet '5 Tage vor dem Sitzungsdatum, um 9:30 Uhr'."
-
 #. Default: "Publishable (displayed)"
 msgid "publishable_display"
 msgstr ""
 
 #. Default: "Publishable (editable)"
 msgid "publishable_edit"
 msgstr ""
 
+#. Default: "Read less"
+msgid "read_less"
+msgstr ""
+
+#. Default: "Read more"
+msgid "read_more"
+msgstr ""
+
 #. Default: "Select here the item states into which some events related to the item (like annex creations or deletions) will be stored in the item's history."
 msgid "record_item_history_states_descr"
 msgstr "Wählen sie hier die Stati der TOP für welche einige Ereignisse relativ zum TOP (wie das anhägen oder löchen von Anlagen), in der TOP-History gespeichert werden."
 
-#. Default: "Select here the meeting states into which some events related to the meeting will be stored in the meeting's history."
-msgid "record_meeting_history_states_descr"
-msgstr ""
-
 #. Default: "The recurring item specified in the subject of this email could not be inserted in a meeting. Maybe does it lack some important information (a text for the decision, for example) while the meeting is in an \"advanced\" state (it is already \"decided\", for instance). More information can be found in the log file of your Zope instance."
 #, fuzzy
 msgid "recurringItemWorkflowError_mail_body"
 msgstr "Der sich wiederholende TOP im Betreff dieser E-Mail konnte nicht in eine Sitzung eingefügt werden. Vielleicht fehlen noch wichtige Informationen (ein Text für den Beschluss zum Beispiel) während die Sitzung in einem fortgeschrittenen Status ist (zum Beispiel schon 'entschieden'). Mehr Informationen können in der log-Datei Ihrer Zope-Instanz finden."
 
 #. Default: "${portalTitle} - A problem occurred while inserting a recurring into a meeting - ${itemTitle}"
 #, fuzzy
@@ -5417,26 +5328,34 @@
 msgid "remove_several_items"
 msgstr ""
 
 #. Default: "Selected items have been removed from the meeting."
 msgid "remove_several_items_done"
 msgstr ""
 
-#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by \"${hp_url}\"!"
+#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by held position at \"${hp_url}\"!"
 msgid "removed_position_type_in_use_error"
 msgstr ""
 
+#. Default: "You can not remove a position type that was used as redefined position for an attendee on an item, you removed \"${removed_position_type}\", check attendees on item at \"${item_url}\"!"
+msgid "removed_redefined_position_type_in_use_error"
+msgstr ""
+
 #. Default: "A category must be selected on this item so it may evolve in the workflow"
 msgid "required_category_ko"
 msgstr ""
 
 #. Default: "A classifier must be selected on this item so it may evolve in the workflow"
 msgid "required_classifier_ko"
 msgstr ""
 
+#. Default: "A group in charge must be selected on this item so it may evolve in the workflow"
+msgid "required_groupsInCharge_ko"
+msgstr ""
+
 #. Default: "Check the box if access to secret items must be restricted.  This will let only users for which an explicit access to the item has been given, access the item.  It will be the case so for members of the proposing groups, power users (Managers, MeetingManagers, power observers), copy groups and advisers.  Only activate this if necessary, it could be the case if you have a state where everything is accessible by everyone (like a \"published\" state for items) but where you want \"secret\" items not to be accessible by everyone."
 msgid "restrict_access_to_secret_items_descr"
 msgstr ""
 
 #. Default: "Restrict access to secret items to description"
 msgid "restrict_access_to_secret_items_to_descr"
 msgstr ""
@@ -5620,14 +5539,18 @@
 msgid "selectable_for_plonegroup_descr"
 msgstr ""
 
 #. Default: "Select here privacies that will be selectable by users editing items of this configuration.  If \"on privacy\" is used in the \"Sort order(s) to apply when adding an item to a meeting\" field, it is the order of values selected here that will be used."
 msgid "selectable_privacies_descr"
 msgstr ""
 
+#. Default: "Select here position types that will be selectable when redefining the position of an attendee for an item.  If nothing selected (default), then any position types is selectable."
+msgid "selectable_redefined_position_types_descr"
+msgstr ""
+
 #. Default: "Check the box if item needs to be send to authority, if so, a line will be automatically printed in the item deliberation document."
 msgid "send_to_authority_descr"
 msgstr ""
 
 #. Default: "Unable to send this item to the ${meetingConfigTitle} meetingConfig because the user to create the item to does not have a personal folder in this meetingConfig.  If necessary, the concerned user can connect for this folder to be created automatically."
 msgid "sendto_inexistent_destfolder_error"
 msgstr ""
@@ -5674,18 +5597,14 @@
 msgid "show_or_hide_details"
 msgstr "Anzeigen / Verstecken von Details"
 
 #. Default: "Show / hide poll type observations"
 msgid "show_or_hide_pollTypeObservations"
 msgstr ""
 
-#. Default: "Signatures"
-msgid "signatures"
-msgstr "Unterschriften"
-
 #. Default: "Signatures as defined on the linked meeting"
 msgid "signatures_defined_on_meeting"
 msgstr ""
 
 #. Default: "Define here the default signatures that will be automatically selected on newly created meetings. Use 2 lines by signature, one for the function and one for the signatory name. This will be applicable only if you use attribute \"Signatures\" for meetings."
 #, fuzzy
 msgid "signatures_descr"
@@ -5699,14 +5618,22 @@
 msgid "signed_edit"
 msgstr ""
 
 #. Default: "Check this box if you want to sort the tags in alphabetic order."
 msgid "sort_all_item_tags_descr"
 msgstr "Markieren Sie dieses Kästchen wenn Sie die Tags in alphabetischer Reihenfolge angezeigt bekommen wollen."
 
+#. Default: "The meeting start date must occur before the end date."
+msgid "start_date_after_end_date"
+msgstr ""
+
+#. Default: "The meeting start date must occur after the meeting date."
+msgid "start_date_before_meeting_date"
+msgstr ""
+
 #. Default: "Store as annex of type ${annex_type_title}"
 msgid "store_as_annex_type_title"
 msgstr ""
 
 #. Default: "Not allowed to add annex in this element."
 msgid "store_podtemplate_as_annex_can_not_add_annex"
 msgstr ""
@@ -5800,21 +5727,217 @@
 msgstr ""
 
 #. Default: "This item is NOT an oral question"
 msgid "this_item_is_not_an_oral_question"
 msgstr "Dieser TOP ist KEINE mündliche Frage"
 
 #. Default: "Extraordinary session"
-msgid "this_meeting_is_extraodrinary_session"
+msgid "this_meeting_is_extraordinary_session"
+msgstr ""
+
+#. Default: "Absents"
+msgid "title_absents"
+msgstr ""
+
+#. Default: "Approval date"
+msgid "title_approval_date"
+msgstr ""
+
+#. Default: "Assembly"
+msgid "title_assembly"
+msgstr ""
+
+#. Default: "Assembly absents"
+msgid "title_assembly_absents"
+msgstr ""
+
+#. Default: "Assembly excused"
+msgid "title_assembly_excused"
+msgstr ""
+
+#. Default: "Assembly guests"
+msgid "title_assembly_guests"
+msgstr ""
+
+#. Default: "Assembly observations"
+msgid "title_assembly_observations"
+msgstr ""
+
+#. Default: "Assembly proxies"
+msgid "title_assembly_proxies"
+msgstr ""
+
+#. Default: "Assembly staves"
+msgid "title_assembly_staves"
+msgstr ""
+
+#. Default: "Attendees"
+msgid "title_attendees"
+msgstr ""
+
+#. Default: "Authority notice"
+msgid "title_authority_notice"
+msgstr ""
+
+#. Default: "Committees"
+msgid "title_committees"
+msgstr ""
+
+#. Default: "Assembly"
+msgid "title_committees_assembly"
+msgstr ""
+
+#. Default: "Attendees"
+msgid "title_committees_attendees"
+msgstr ""
+
+#. Default: "Convocation date"
+msgid "title_committees_convocation_date"
+msgstr ""
+
+#. Default: "Date"
+msgid "title_committees_date"
+msgstr ""
+
+#. Default: "Committees observations"
+msgid "title_committees_observations"
+msgstr ""
+
+#. Default: "Place"
+msgid "title_committees_place"
+msgstr ""
+
+#. Default: "Committee"
+msgid "title_committees_row_id"
+msgstr ""
+
+#. Default: "Signatories"
+msgid "title_committees_signatories"
+msgstr ""
+
+#. Default: "Signatures"
+msgid "title_committees_signatures"
+msgstr ""
+
+#. Default: "Convocation date"
+msgid "title_convocation_date"
+msgstr ""
+
+#. Default: "Date"
+msgid "title_date"
+msgstr ""
+
+#. Default: "Default assembly"
+msgid "title_default_assembly"
+msgstr ""
+
+#. Default: "Default assembly staves"
+msgid "title_default_assembly_staves"
+msgstr ""
+
+#. Default: "Default signatures"
+msgid "title_default_signatures"
+msgstr ""
+
+#. Default: "End date"
+msgid "title_end_date"
+msgstr ""
+
+#. Default: "Excused"
+msgid "title_excused"
+msgstr ""
+
+#. Default: "Extraordinary session"
+msgid "title_extraordinary_session"
+msgstr ""
+
+#. Default: "First item number (managed automatically when meeting is frozen)"
+msgid "title_first_item_number"
+msgstr ""
+
+#. Default: "In and out moves"
+msgid "title_in_and_out_moves"
+msgstr ""
+
+#. Default: "Meeting number"
+msgid "title_meeting_number"
+msgstr ""
+
+#. Default: "Meeting managers notes"
+msgid "title_meetingmanagers_notes"
+msgstr ""
+
+#. Default: "Mid date"
+msgid "title_mid_date"
+msgstr ""
+
+#. Default: "Non attendees"
+msgid "title_non_attendees"
+msgstr ""
+
+#. Default: "Notes"
+msgid "title_notes"
+msgstr ""
+
+#. Default: "Observations"
+msgid "title_observations"
+msgstr ""
+
+#. Default: "Place"
+msgid "title_place"
+msgstr ""
+
+#. Default: "Other place"
+msgid "title_place_other"
+msgstr ""
+
+#. Default: "Pre meeting date"
+msgid "title_pre_meeting_date"
+msgstr ""
+
+#. Default: "Pre meeting place"
+msgid "title_pre_meeting_place"
+msgstr ""
+
+#. Default: "Pre observations"
+msgid "title_pre_observations"
+msgstr ""
+
+#. Default: "Public meeting observations"
+msgid "title_public_meeting_observations"
+msgstr ""
+
+#. Default: "Replacements"
+msgid "title_replacements"
 msgstr ""
 
 #. Default: "A title is required."
 msgid "title_required"
 msgstr "Ein Titel wird benötigt."
 
+#. Default: "Secret meeting observations"
+msgid "title_secret_meeting_observations"
+msgstr ""
+
+#. Default: "Signatories"
+msgid "title_signatories"
+msgstr ""
+
+#. Default: "Signatures"
+msgid "title_signatures"
+msgstr ""
+
+#. Default: "Start date"
+msgid "title_start_date"
+msgstr ""
+
+#. Default: "Votes observations"
+msgid "title_votes_observations"
+msgstr ""
+
 #. Default: "Ask this advice again (current advice will be historized)"
 msgid "to_advice_asked_again"
 msgstr ""
 
 #. Default: "To be printed (displayed)"
 msgid "to_be_printed_display"
 msgstr ""
@@ -6008,18 +6131,14 @@
 msgid "used_poll_types_descr"
 msgstr ""
 
 #. Default: "Specify here what vote values are in use in this meeting configuration."
 msgid "used_vote_values_descr"
 msgstr "Legen Sie hier fest welche Abstimmungsmöglichkeiten für dieses Sitzungskonfiguration bestehen."
 
-#. Default: "Users"
-msgid "users"
-msgstr "Benutzer"
-
 #. Default: "If you do not select anything, every users will be displayed."
 msgid "users_hidden_in_dashboard_filter_descr"
 msgstr ""
 
 #. Default: "When an advice is \"given\" and no more editable by the advisers, so when it was set in a state where advisers may not edit it anymore, it is automatically versioned. Depending on the configuration, if advice may be given when the item is still editable by the proposing group, it may be necessary to versionate advice if it was given (but still editable by advisers) and the item was edited. For example, advices are giveable when item is \"itemcreated\", a state where item may still be edited by the proposing group. If it is the case, check this box, it will ensure that the advice is versioned when the item is edited if necessary (so if it was not already versioned since last advice edition).  If you have a specific state \"waiting advice\" where proposing group is not able to edit the item, this box may be left unchecked."
 msgid "versionate_advice_if_given_and_item_modified_descr"
 msgstr ""
@@ -6125,14 +6244,15 @@
 msgstr ""
 
 #. Default: "There are ${numberOfVoters} voters for this item."
 msgid "voter_count"
 msgstr "${numberOfVoters} Stimmberechtigte"
 
 #. Default: "Votes"
+#, fuzzy
 msgid "votes"
 msgstr "Abstimmungen"
 
 #. Default: "You can choose here who will effectively encode the votes. Several choices are possible."
 msgid "votes_encoder_descr"
 msgstr "Sie können hier auswählen wer letzendlich die Abstimmungen einpflegt. Mehrfachauswahl ist möglich."
 
@@ -6336,14 +6456,22 @@
 msgid "wait_msg"
 msgstr ""
 
 #. Default: "You are currently adding an organization outside \"My organization\", please make sure this is correct.  If you want to create a new group that will be able the create items, give advices, you need to add it directly under \"My organization\"."
 msgid "warning_adding_org_outside_own_org"
 msgstr ""
 
+#. Default: "Advice is currently \"Asked again\" do not forget to change value of field \"Advice type\" to another value than \"Asked again\""
+msgid "warning_advice_asked_again_need_to_change_advice_type"
+msgstr ""
+
+#. Default: "Warning, there is a problem with encoded data for assembly and signatures, please check especially that signatories are correctly defined"
+msgid "warning_assembly_and_signatures"
+msgstr ""
+
 #. Default: "Warning: if you modify the title or description and save this form, all given advices will be invalidated."
 msgid "warning_invalidate_advices"
 msgstr "Achtung: wenn Sie den Titel oder die Beschreibung ändern und diese Änderungen speichern, werden alle schon abgegebenen Kommentare ungültig."
 
 #. Default: "If you modify this field, all given advices will be invalidated."
 msgid "warning_invalidate_advices_fastedit"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.contact.core.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.contact.core.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.history.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/plone.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/plone.po`

 * *Files 1% similar despite different names*

```diff
@@ -559,14 +559,18 @@
 msgid "close"
 msgstr "Schließen"
 
 #. Default: "Closed"
 msgid "closed"
 msgstr "Geschlossen"
 
+#. Default: "Committees"
+msgid "committees"
+msgstr ""
+
 #. Default: "Confirm"
 msgid "confirm"
 msgstr "Bestätigen"
 
 #. Default: "Confirmed"
 msgid "confirmed"
 msgstr "Bestätigt"
@@ -997,14 +1001,15 @@
 msgstr "Validieren"
 
 #. Default: "Validated"
 msgid "validated"
 msgstr "Validiert"
 
 #. Default: "Votes"
+#, fuzzy
 msgid "votes"
 msgstr "Abstimmungen"
 
 #. Default: "Ask advices"
 msgid "wait_advices_from"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.actionspanel.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.annex.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/imio.annex.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.behavior.talcondition.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.behavior.talcondition.pot`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/datagridfield.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/datagridfield.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,364 +1,447 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PloneMeeting\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "POT-Creation-Date: 2014-01-09 12:30-100\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
-"Domain: datagridfield\n"
+"Domain: DOMAIN\n"
 
-#. Default: "Identifier (row_id)"
-msgid "Custom adviser row id"
+#. Default: "Available on"
+msgid "Available on"
 msgstr ""
 
-#. Default: "Organization"
-msgid "Custom adviser organization"
+#. Default: "Committee acronym"
+msgid "Committee acronym"
 msgstr ""
 
-#. Default: "Advice will be automatically asked if"
-msgid "Custom adviser gives automatic advice on"
+#. Default: "Committee auto from"
+msgid "Committee auto from"
 msgstr ""
 
-#. Default: "Specify here a TAL expression that will return True if the advice of the group must be automatically asked on an item.  We receive \"item\" as the meeting item to give an advice on, \"org\" and \"org_uid\" as the organization (organization UID) that will have to give the advice.  WARNING if the group of advisers linked to this group is empty, it will no be considered, despite the result of the TAL expression.  This advice will NOT be askable manually in the user interface, it is only asked automatically by the application.  If this advice should not be asked automatically, leave this field blank."
-msgid "gives_auto_advice_on_col_description"
+#. Default: "Committee default assembly"
+msgid "Committee default assembly"
 msgstr ""
 
-#. Default: "Automatic asked advice help message"
-msgid "Custom adviser gives automatic advice on help message"
+#. Default: "Committee default attendees"
+msgid "Committee default attendees"
 msgstr ""
 
-#. Default: "If you want a specific help message to be displayed on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The message will appear between brackets after the message \"This advice has been automatically asked by the application\"."
-msgid "gives_auto_advice_on_help_message_col_description"
+#. Default: "Committee default place"
+msgid "Committee default place"
 msgstr ""
 
-#. Default: "Rule activated for item created from"
-msgid "Rule activated for item created from"
+#. Default: "Committee default signatories"
+msgid "Committee default signatories"
 msgstr ""
 
-#. Default: "This configuration will be applied on item created from the defined date (defined date included).  Please respect following format : YYYY/MM/DD (year 4 digits/month 2 digits/day 2 digits).  This date will avoid older items created before to be affected, especially when updating every advices thru the \"Update all advices\" action."
-msgid "for_item_created_from_col_description"
+#. Default: "Committee default signatures"
+msgid "Committee default signatures"
 msgstr ""
 
-#. Default: "Rule activated for item created until"
-msgid "Rule activated for item created until"
+#. Default: "Committee enabled?"
+msgid "Committee enabled?"
 msgstr ""
 
-#. Default: "This configuration will be applied on item created until the defined date (defined date must be in the future and will not be included).  Please respect following format : YYYY/MM/DD (year 4 digits/month 2 digits/day 2 digits).  This date will avoid newer items created after to be affected, especially when updating every advices thru the \"Update all advices\" action. This date will be only settable once, when set, this can not be changed anymore."
-msgid "for_item_created_until_col_description"
+#. Default: "Committee label"
+msgid "Committee label"
 msgstr ""
 
-#. Default: "Delay for giving advice"
-msgid "Delay for giving advice"
+#. Default: "Committee row id"
+msgid "Committee row id"
 msgstr ""
 
-#. Default: "Enter the delay the adviser will have to give his advice. If it is not considered as an automatically asked advice (nothing defined in the \"Advice will be automatically asked if\" column), the advice will be selectable in the \"Ask advice to\" list on the item edit form. A delay is a single digit (like \"5\" or \"10\"). If no delay is relevant for this advice, leave this field blank. If several delays are possible for the same advice, you have to define several rows with exactly the same content excepted the delay."
-msgid "delay_col_description"
+#. Default: "Committee supplements"
+msgid "Committee supplements"
 msgstr ""
 
-#. Default: "Delay left alert"
-msgid "Delay left alert"
+#. Default: "Committee using groups"
+msgid "Committee using groups"
 msgstr ""
 
-#. Default: "Enter the treshold beyond wich an alert must be shown regarding left delay.  This will be shown in the UI with a particular color and if activated, a mail notification could be send in this case. Enter a single digit (like \"5\" or \"10\") lower than actual \"Delay\". If no treshold is relevant for this advice, leave this field blank."
-msgid "delay_left_alert_col_description"
+#. Default: "Full label"
+msgid "Config group full label"
 msgstr ""
 
-#. Default: "Available on"
-msgid "Available on"
+#. Default: "Label"
+msgid "Config group label"
 msgstr ""
 
-#. Default: "Specify here a TAL expression that will restrict or allow the use of this advice to some condition.  We receive \"item\" as the meeting item to give an advice on and \"mayEdit\", a boolean to know if current user may edit the item.  A special expression is available to protect a row that should only be available thru the \"Change delay\" action, it is : \"python: item.REQUEST.get('managing_available_delays', False)\".  This can not be used if something is defined in the \"Advice will be automatically asked if\" column of this advice, but for optional delay-aware advice or for delay-aware advices linked to an automatic advice (using the \"Is linked to previous row?\" column)"
-msgid "available_on_col_description"
+#. Default: "Identifier (row_id)"
+msgid "Config group row id"
 msgstr ""
 
 #. Default: "Advice with delay label"
 msgid "Custom adviser delay label"
 msgstr ""
 
-#. Default: "If you want a specific label to be displayed on the label displayed in the \"Advice to give\" list on the item edit form and on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The label will appear between brackets after the message \"Name of the group - delay of X days\"."
-msgid "delay_label_col_description"
+#. Default: "Advice will be automatically asked if"
+msgid "Custom adviser gives automatic advice on"
 msgstr ""
 
-#. Default: "Meeting config"
-msgid "Meeting config to clone to Meeting config"
+#. Default: "Automatic asked advice help message"
+msgid "Custom adviser gives automatic advice on help message"
 msgstr ""
 
-#. Default: "The meeting config the item of this meeting config will be sendable to."
-msgid "The meeting config the item of this meeting config will be sendable to."
+#. Default: "Organization"
+msgid "Custom adviser organization"
 msgstr ""
 
-#. Default: "Meeting config to clone to Trigger workflow transitions until"
-msgid "Meeting config to clone to Trigger workflow transitions until"
+#. Default: "Identifier (row_id)"
+msgid "Custom adviser row id"
 msgstr ""
 
-#. Default: "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field \"States in which an item will be automatically sent to selected other meeting configurations\" here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the \"Transitions for presenting an item\" you defined in the \"Workflows\" tab of the meeting configuration the item will be sent to."
-msgid "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field 'States in which an item will be automatically sent to selected other meeting configurations' here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the 'Transitions for presenting an item' you defined in the 'Workflows' tab of the meeting configuration the item will be sent to."
+#. Default: "Delay for giving advice"
+msgid "Delay for giving advice"
 msgstr ""
 
-#. Default: "Date"
-msgid "Holiday date"
+#. Default: "Delay left alert"
+msgid "Delay left alert"
 msgstr ""
 
-#. Default: "Please use following format : YYYY/MM/DD.  Dates must be sorted (from older to newer)."
-msgid "holiday_date_col_descr"
+#. Default: "Enter a short label that will be displayed in the application.  This will be translated by the application if possible.  If you want to colorize this new list type on the meeting view, you will need to do this using CSS like it is the case for \"late\" items."
+msgid "Enter a short label that will be displayed in the application.  This will be translated by the application if possible.  If you want to colorize this new list type on the meeting view, you will need to do this using CSS like it is the case for 'late' items."
 msgstr ""
 
-#. Default: "Title"
-msgid "Sub type title"
+#. Default: "Enter an internal identifier, use only lowercase letters."
+msgid "Enter an internal identifier, use only lowercase letters."
 msgstr ""
 
-#. Default: "Predefined title"
-msgid "Sub type predefined title"
+#. Default: "Enter the full label that will be useable if necessary like in produced documents."
+msgid "Enter the full label that will be useable if necessary like in produced documents."
 msgstr ""
 
-#. Default: "Correspondences while sent to other meeting configs"
-msgid "Sub type correspondences while sent to other meeting configs"
+#. Default: "Enter the label that will be displayed in the application."
+msgid "Enter the label that will be displayed in the application."
 msgstr ""
 
-#. Default: "Please look the help message of the field \"Correspondences while sent to other meeting configs\" here above.  Simply note that if nothing is defined here, the value defined in the field above will be used."
-msgid "Sub type correspondences while sent to other meeting configs description."
+#. Default: "Date"
+msgid "Holiday date"
 msgstr ""
 
-#. Default: "Default value of the \"Confidential ?\" attribute of created annexes"
-msgid "Sub type confidentiality of created annexes"
+#. Default: "If the inserting method \"on list types\" is used, will this list type be taken into account while inserting the item in the meeting?"
+msgid "If the inserting method \"on list types\" is used, will this list type be taken into account while inserting the item in the meeting?"
 msgstr ""
 
-#. Default: "Please look the help message of the field \"Default value of the 'Confidential ?' attribute of created annexes\" here above.  Simply note that if nothing is defined here, the value defined in the field above will be used."
-msgid "Sub type confidentiality of created annexes description."
+#. Default: "Inserting method"
+msgid "Inserting method"
 msgstr ""
 
-#. Default: "Active?"
-msgid "Sub type is active?"
+#. Default: "Set to \"Yes\" if you want to make a logical link between a row and the previous one.  This will manage the fact of easily being able to change a delay for an asked advice.  The linked rows will make the user being able to select between those different delays in the advice vizualisation popup.  This is only relevant for delay-aware advices, to link differents delays together."
+msgid "Is linked to previous row description"
 msgstr ""
 
 #. Default: "Is linked to previous row?"
 msgid "Is linked to previous row?"
 msgstr ""
 
-#. Default: "Set to \"Yes\" if you want to make a logical link between a row and the previous one.  This will manage the fact of easily being able to change a delay for an asked advice.  The linked rows will make the user being able to select between those different delays in the advice vizualisation popup.  This is only relevant for delay-aware advices, to link differents delays together."
-msgid "Is linked to previous row description"
+#. Default: "Item WF validation levels back transition"
+msgid "Item WF validation levels back transition"
 msgstr ""
 
-#. Default: "Inserting method"
-msgid "Inserting method"
+#. Default: "Item WF validation levels back transition description."
+msgid "Item WF validation levels back transition description."
 msgstr ""
 
-#. Default: "Select the inserting method, methods will be applied in given order, you can not select twice same inserting method."
-msgid "Select the inserting method, methods will be applied in given order, you can not select twice same inserting method."
+#. Default: "Item WF validation levels back transition title"
+msgid "Item WF validation levels back transition title"
 msgstr ""
 
-#. Default: "Reverse?"
-msgid "Reverse inserting method?"
+#. Default: "Item WF validation levels back transition title description."
+msgid "Item WF validation levels back transition title description."
 msgstr ""
 
-#. Default: "Reverse order of selected inserting method?"
-msgid "Reverse order of selected inserting method?"
+#. Default: "Item WF validation levels enabled"
+msgid "Item WF validation levels enabled"
 msgstr ""
 
-#. Default: "Transition"
-msgid "On transition field transform transition"
+#. Default: "Item WF validation levels enabled description."
+msgid "Item WF validation levels enabled description."
 msgstr ""
 
-#. Default: "The transition that will trigger the field transform."
-msgid "The transition that will trigger the field transform."
+#. Default: "Item WF validation levels extra suffixes"
+msgid "Item WF validation levels extra suffixes"
 msgstr ""
 
-#. Default: "Field name"
-msgid "On transition field transform field name"
+#. Default: "Item WF validation levels extra suffixes description."
+msgid "Item WF validation levels extra suffixes description."
 msgstr ""
 
-#. Default: "The item field that will be transformed."
-msgid "The item field that will be transformed."
+#. Default: "Item WF validation levels leading transition"
+msgid "Item WF validation levels leading transition"
 msgstr ""
 
-#. Default: "TAL expression"
-msgid "On transition field transform TAL expression"
+#. Default: "Item WF validation levels leading transition description."
+msgid "Item WF validation levels leading transition description."
 msgstr ""
 
-#. Default: "The TAL expression.  Element \"here\" represent the item.  This expression MUST return valid HTML or it will not behave properly on the item."
-msgid "The TAL expression.  Element 'here' represent the item.  This expression MUST return valid HTML or it will not behave properly on the item."
+#. Default: "Item WF validation levels leading transition title"
+msgid "Item WF validation levels leading transition title"
 msgstr ""
 
-#. Default: "Transition triggered on the meeting"
-msgid "On meeting transition item action to execute meeting transition"
+#. Default: "Item WF validation levels leading transition title description."
+msgid "Item WF validation levels leading transition title description."
 msgstr ""
 
-#. Default: " "
-msgid "The transition triggered on the meeting."
+#. Default: "Item WF validation levels state"
+msgid "Item WF validation levels state"
 msgstr ""
 
-#. Default: "Transition to trigger on every items of the meeting"
-msgid "On meeting transition item action to execute item action"
+#. Default: "Item WF validation levels state description."
+msgid "Item WF validation levels state description."
 msgstr ""
 
-#. Default: " "
-msgid "The action that will be executed on every items of the meeting."
+#. Default: "Item WF validation levels state title"
+msgid "Item WF validation levels state title"
 msgstr ""
 
-#. Default: "On meeting transition item action to execute tal expression"
-msgid "On meeting transition item action to execute tal expression"
+#. Default: "Item WF validation levels state title description."
+msgid "Item WF validation levels state title description."
 msgstr ""
 
-#. Default: " "
-msgid "The action to execute when 'Execute given action' is selected in column 'Item action'."
+#. Default: "Item WF validation levels suffix"
+msgid "Item WF validation levels suffix"
 msgstr ""
 
-#. Default: "List type identifier"
-msgid "List type identifier"
+#. Default: "Item WF validation levels suffix description."
+msgid "Item WF validation levels suffix description."
 msgstr ""
 
-#. Default: "Enter an internal identifier, use only lowercase letters."
-msgid "Enter an internal identifier, use only lowercase letters."
+#. Default: "List type identifier"
+msgid "List type identifier"
 msgstr ""
 
 #. Default: "List type label"
 msgid "List type label"
 msgstr ""
 
-#. Default: "Enter a short label that will be displayed in the application.  This will be translated by the application if possible.  If you want to colorize this new list type on the meeting view, you will need to do this using CSS like it is the case for \"late\" items."
-msgid "Enter a short label that will be displayed in the application.  This will be translated by the application if possible.  If you want to colorize this new list type on the meeting view, you will need to do this using CSS like it is the case for 'late' items."
-msgstr ""
-
 #. Default: "List type used_in_inserting_method"
 msgid "List type used_in_inserting_method"
 msgstr ""
 
-#. Default: "If the inserting method \"on list types\" is used, will this list type be taken into account while inserting the item in the meeting?"
-msgid "If the inserting method \"on list types\" is used, will this list type be taken into account while inserting the item in the meeting?"
+#. Default: "Meeting config"
+msgid "Meeting config to clone to Meeting config"
 msgstr ""
 
-#. Default: "Identifier (row_id)"
-msgid "Config group row id"
+#. Default: "Meeting config to clone to Trigger workflow transitions until"
+msgid "Meeting config to clone to Trigger workflow transitions until"
 msgstr ""
 
-#. Default: "Label"
-msgid "Config group label"
+#. Default: "Transition to trigger on every items of the meeting"
+msgid "On meeting transition item action to execute item action"
 msgstr ""
 
-#. Default: "Enter the label that will be displayed in the application."
-msgid "Enter the label that will be displayed in the application."
+#. Default: "Transition triggered on the meeting"
+msgid "On meeting transition item action to execute meeting transition"
 msgstr ""
 
-#. Default: "Full label"
-msgid "Config group full label"
+#. Default: "On meeting transition item action to execute tal expression"
+msgid "On meeting transition item action to execute tal expression"
 msgstr ""
 
-#. Default: "Enter the full label that will be useable if necessary like in produced documents."
-msgid "Enter the full label that will be useable if necessary like in produced documents."
+#. Default: "TAL expression"
+msgid "On transition field transform TAL expression"
 msgstr ""
 
-#. Default: "Power observer label"
-msgid "Power observer label"
+#. Default: "Field name"
+msgid "On transition field transform field name"
 msgstr ""
 
-#. Default: "Power observer label description"
-msgid "power_observers_label_col_description"
+#. Default: "Transition"
+msgid "On transition field transform transition"
 msgstr ""
 
-#. Default: "Power observer item viewable states"
-msgid "Power observer item viewable states"
+#. Default: "Power observer item access TAL expression"
+msgid "Power observer item access TAL expression"
 msgstr ""
 
-#. Default: "Power observer item viewable states description"
-msgid "power_observers_item_states_col_description"
+#. Default: "Power observer item viewable states"
+msgid "Power observer item viewable states"
 msgstr ""
 
-#. Default: "Power observer item access TAL expression"
-msgid "Power observer item access TAL expression"
+#. Default: "Power observer label"
+msgid "Power observer label"
 msgstr ""
 
-#. Default: "Power observer item access TAL expression description"
-msgid "power_observers_item_access_on_col_description"
+#. Default: "Power observer meeting access TAL expression"
+msgid "Power observer meeting access TAL expression"
 msgstr ""
 
 #. Default: "Power observer meeting viewable states"
 msgid "Power observer meeting viewable states"
 msgstr ""
 
-#. Default: "Power observer meeting viewable states description"
-msgid "power_observers_meeting_states_col_description"
+#. Default: "Reverse?"
+msgid "Reverse inserting method?"
 msgstr ""
 
-#. Default: "Power observer meeting access TAL expression"
-msgid "Power observer meeting access TAL expression"
+#. Default: "Reverse order of selected inserting method?"
+msgid "Reverse order of selected inserting method?"
 msgstr ""
 
-#. Default: "Power observer meeting access TAL expression description"
-msgid "power_observers_meeting_access_on_col_description"
+#. Default: "Rule activated for item created from"
+msgid "Rule activated for item created from"
 msgstr ""
 
-#. Default: "Item WF validation levels state"
-msgid "Item WF validation levels state"
+#. Default: "Rule activated for item created until"
+msgid "Rule activated for item created until"
 msgstr ""
 
-#. Default: "Item WF validation levels state description."
-msgid "Item WF validation levels state description."
+#. Default: "Select the inserting method, methods will be applied in given order, you can not select twice same inserting method."
+msgid "Select the inserting method, methods will be applied in given order, you can not select twice same inserting method."
 msgstr ""
 
-#. Default: "Item WF validation levels state title"
-msgid "Item WF validation levels state title"
+#. Default: "Default value of the \"Confidential ?\" attribute of created annexes"
+msgid "Sub type confidentiality of created annexes"
 msgstr ""
 
-#. Default: "Item WF validation levels state title description."
-msgid "Item WF validation levels state title description."
+#. Default: "Please look the help message of the field \"Default value of the 'Confidential ?' attribute of created annexes\" here above.  Simply note that if nothing is defined here, the value defined in the field above will be used."
+msgid "Sub type confidentiality of created annexes description."
 msgstr ""
 
-#. Default: "Item WF validation levels leading transition"
-msgid "Item WF validation levels leading transition"
+#. Default: "Correspondences while sent to other meeting configs"
+msgid "Sub type correspondences while sent to other meeting configs"
 msgstr ""
 
-#. Default: "Item WF validation levels leading transition description."
-msgid "Item WF validation levels leading transition description."
+#. Default: "Please look the help message of the field \"Correspondences while sent to other meeting configs\" here above.  Simply note that if nothing is defined here, the value defined in the field above will be used."
+msgid "Sub type correspondences while sent to other meeting configs description."
 msgstr ""
 
-#. Default: "Item WF validation levels leading transition title"
-msgid "Item WF validation levels leading transition title"
+#. Default: "Active?"
+msgid "Sub type is active?"
 msgstr ""
 
-#. Default: "Item WF validation levels leading transition title description."
-msgid "Item WF validation levels leading transition title description."
+#. Default: "Predefined title"
+msgid "Sub type predefined title"
 msgstr ""
 
-#. Default: "Item WF validation levels back transition"
-msgid "Item WF validation levels back transition"
+#. Default: "Title"
+msgid "Sub type title"
 msgstr ""
 
-#. Default: "Item WF validation levels back transition description."
-msgid "Item WF validation levels back transition description."
+#. Default: "The TAL expression.  Element \"here\" represent the item.  This expression MUST return valid HTML or it will not behave properly on the item."
+msgid "The TAL expression.  Element 'here' represent the item.  This expression MUST return valid HTML or it will not behave properly on the item."
 msgstr ""
 
-#. Default: "Item WF validation levels back transition title"
-msgid "Item WF validation levels back transition title"
+#. Default: " "
+msgid "The action that will be executed on every items of the meeting."
 msgstr ""
 
-#. Default: "Item WF validation levels back transition title description."
-msgid "Item WF validation levels back transition title description."
+#. Default: " "
+msgid "The action to execute when 'Execute given action' is selected in column 'Item action'."
 msgstr ""
 
-#. Default: "Item WF validation levels suffix"
-msgid "Item WF validation levels suffix"
+#. Default: "The item field that will be transformed."
+msgid "The item field that will be transformed."
 msgstr ""
 
-#. Default: "Item WF validation levels suffix description."
-msgid "Item WF validation levels suffix description."
+#. Default: "The meeting config the item of this meeting config will be sendable to."
+msgid "The meeting config the item of this meeting config will be sendable to."
 msgstr ""
 
-#. Default: "Item WF validation levels extra suffixes"
-msgid "Item WF validation levels extra suffixes"
+#. Default: "The transition that will trigger the field transform."
+msgid "The transition that will trigger the field transform."
 msgstr ""
 
-#. Default: "Item WF validation levels extra suffixes description."
-msgid "Item WF validation levels extra suffixes description."
+#. Default: " "
+msgid "The transition triggered on the meeting."
 msgstr ""
 
-#. Default: "Item WF validation levels enabled"
-msgid "Item WF validation levels enabled"
+#. Default: "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field \"States in which an item will be automatically sent to selected other meeting configurations\" here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the \"Transitions for presenting an item\" you defined in the \"Workflows\" tab of the meeting configuration the item will be sent to."
+msgid "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field 'States in which an item will be automatically sent to selected other meeting configurations' here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the 'Transitions for presenting an item' you defined in the 'Workflows' tab of the meeting configuration the item will be sent to."
 msgstr ""
 
-#. Default: "Item WF validation levels enabled description."
-msgid "Item WF validation levels enabled description."
+#. Default: "Specify here a TAL expression that will restrict or allow the use of this advice to some condition.  We receive \"item\" as the meeting item to give an advice on and \"mayEdit\", a boolean to know if current user may edit the item.  A special expression is available to protect a row that should only be available thru the \"Change delay\" action, it is : \"python: item.REQUEST.get('managing_available_delays', False)\".  This can not be used if something is defined in the \"Advice will be automatically asked if\" column of this advice, but for optional delay-aware advice or for delay-aware advices linked to an automatic advice (using the \"Is linked to previous row?\" column)"
+msgid "available_on_col_description"
+msgstr ""
+
+#. Default: "Used to automatically determinate the committee for the item, the field \"Committees\" will not appear on the item when editing it (except for MeetingManagers).  This may only be used when column \"using_groups\" is not used."
+msgid "committees_auto_from_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Assembly\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_assembly_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Attendees\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_attendees_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Place\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_place_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Signatories\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatories_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Signatures\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatures_col_description"
+msgstr ""
+
+#. Default: "Will generate new values on item \"Committees\" field when necessary to manage supplements (items added to meeting after committees convocation were sent).  This will only be useable by MeetingManagers."
+msgid "committees_supplements_col_description"
+msgstr ""
+
+#. Default: "Used to restrict availability of a committee on the item committees selection box.  This may only be used when column \"auto_from\" is not used."
+msgid "committees_using_groups_col_description"
+msgstr ""
+
+#. Default: "Enter the delay the adviser will have to give his advice. If it is not considered as an automatically asked advice (nothing defined in the \"Advice will be automatically asked if\" column), the advice will be selectable in the \"Ask advice to\" list on the item edit form. A delay is a single digit (like \"5\" or \"10\"). If no delay is relevant for this advice, leave this field blank. If several delays are possible for the same advice, you have to define several rows with exactly the same content excepted the delay."
+msgid "delay_col_description"
+msgstr ""
+
+#. Default: "If you want a specific label to be displayed on the label displayed in the \"Advice to give\" list on the item edit form and on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The label will appear between brackets after the message \"Name of the group - delay of X days\"."
+msgid "delay_label_col_description"
+msgstr ""
+
+#. Default: "Enter the treshold beyond wich an alert must be shown regarding left delay.  This will be shown in the UI with a particular color and if activated, a mail notification could be send in this case. Enter a single digit (like \"5\" or \"10\") lower than actual \"Delay\". If no treshold is relevant for this advice, leave this field blank."
+msgid "delay_left_alert_col_description"
+msgstr ""
+
+#. Default: "This configuration will be applied on item created from the defined date (defined date included).  Please respect following format : YYYY/MM/DD (year 4 digits/month 2 digits/day 2 digits).  This date will avoid older items created before to be affected, especially when updating every advices thru the \"Update all advices\" action."
+msgid "for_item_created_from_col_description"
+msgstr ""
+
+#. Default: "This configuration will be applied on item created until the defined date (defined date must be in the future and will not be included).  Please respect following format : YYYY/MM/DD (year 4 digits/month 2 digits/day 2 digits).  This date will avoid newer items created after to be affected, especially when updating every advices thru the \"Update all advices\" action. This date will be only settable once, when set, this can not be changed anymore."
+msgid "for_item_created_until_col_description"
+msgstr ""
+
+#. Default: "Specify here a TAL expression that will return True if the advice of the group must be automatically asked on an item.  We receive \"item\" as the meeting item to give an advice on, \"org\" and \"org_uid\" as the organization (organization UID) that will have to give the advice.  WARNING if the group of advisers linked to this group is empty, it will no be considered, despite the result of the TAL expression.  This advice will NOT be askable manually in the user interface, it is only asked automatically by the application.  If this advice should not be asked automatically, leave this field blank."
+msgid "gives_auto_advice_on_col_description"
+msgstr ""
+
+#. Default: "If you want a specific help message to be displayed on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The message will appear between brackets after the message \"This advice has been automatically asked by the application\"."
+msgid "gives_auto_advice_on_help_message_col_description"
+msgstr ""
+
+#. Default: "Please use following format : YYYY/MM/DD.  Dates must be sorted (from older to newer)."
+msgid "holiday_date_col_descr"
+msgstr ""
+
+#. Default: "Power observer item access TAL expression description"
+msgid "power_observers_item_access_on_col_description"
+msgstr ""
+
+#. Default: "Power observer item viewable states description"
+msgid "power_observers_item_states_col_description"
+msgstr ""
+
+#. Default: "Power observer label description"
+msgid "power_observers_label_col_description"
+msgstr ""
+
+#. Default: "Power observer meeting access TAL expression description"
+msgid "power_observers_meeting_access_on_col_description"
+msgstr ""
+
+#. Default: "Power observer meeting viewable states description"
+msgid "power_observers_meeting_states_col_description"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/imio.actionspanel.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/plone.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/plone.pot`

 * *Files 0% similar despite different names*

```diff
@@ -560,14 +560,18 @@
 msgid "mail"
 msgstr ""
 
 #. Default: "Advices and access"
 msgid "advices"
 msgstr ""
 
+#. Default: "Committees"
+msgid "committees"
+msgstr ""
+
 #. Default: "Votes"
 msgid "votes"
 msgstr ""
 
 #. Default: "Users"
 msgid "users"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/eea.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/eea.pot`

 * *Files 11% similar despite different names*

```diff
@@ -103,7 +103,11 @@
 #. Default: "Copy groups"
 msgid "Copy groups"
 msgstr ""
 
 #. Default: "To discuss?"
 msgid "To discuss?"
 msgstr ""
+
+#. Default: "Committee"
+msgid "Committee"
+msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/eea.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/eea.po`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 
 msgid "Category"
 msgstr "Catégorie"
 
 msgid "Classifier"
 msgstr "Classificateur"
 
+#. Default: "Committee"
+msgid "Committee"
+msgstr "Commission"
+
 #. Default: "Copy groups"
 msgid "Copy groups"
 msgstr "En copie"
 
 msgid "Created"
 msgstr "Créé le"
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.documentgenerator.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.documentgenerator.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.behavior.talcondition.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.behavior.talcondition.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 #. Default: "Store POD template as annex for selected elements"
 msgid "Store POD template as annex for selected elements"
 msgstr "Annexer un document généré aux éléments sélectionnés"
 
 #. Default: "Update accessed of selected elements"
 msgid "Update accesses for selected elements"
-msgstr "Mettre à jour les accès des éléments sélectionnés"
+msgstr "Mettre à jour les accès des éléments par lot"
 
 #. Default: "Store relevant POD template as annex"
 msgid "store-items-template-as-annex-batch-action-but"
 msgstr "Annexer un document généré"
 
 #. Default: "Update accesses"
 msgid "update-local-roles-batch-action-but"
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/datagridfield.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/datagridfield.po`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,62 @@
 "Domain: datagridfield\n"
 "X-is-fallback-for: fr-be fr-ca fr-lu fr-mc fr-ch fr-fr\n"
 
 #. Default: "Available on"
 msgid "Available on"
 msgstr "Disponible si"
 
+#. Default: "Committee acronym"
+msgid "Committee acronym"
+msgstr "Acronyme"
+
+#. Default: "Committee auto from"
+msgid "Committee auto from"
+msgstr "Automatiquement si"
+
+#. Default: "Committee default assembly"
+msgid "Committee default assembly"
+msgstr "Assemblée par défaut"
+
+#. Default: "Committee default attendees"
+msgid "Committee default attendees"
+msgstr "Présents par défaut"
+
+#. Default: "Committee default place"
+msgid "Committee default place"
+msgstr "Lieu par défaut"
+
+#. Default: "Committee default signatories"
+msgid "Committee default signatories"
+msgstr "Signataires par défaut"
+
+#. Default: "Committee default signatures"
+msgid "Committee default signatures"
+msgstr "Signatures par défaut"
+
+#. Default: "Committee enabled?"
+msgid "Committee enabled?"
+msgstr "Activé?"
+
+#. Default: "Committee label"
+msgid "Committee label"
+msgstr "Libellé"
+
+#. Default: "Committee row id"
+msgid "Committee row id"
+msgstr "Identifiant"
+
+#. Default: "Committee supplements"
+msgid "Committee supplements"
+msgstr "Suppléments"
+
+#. Default: "Committee using groups"
+msgid "Committee using groups"
+msgstr "Restreindre à"
+
 #. Default: "Full label"
 msgid "Config group full label"
 msgstr "Libellé complet"
 
 #. Default: "Label"
 msgid "Config group label"
 msgstr "Libellé"
@@ -311,14 +359,46 @@
 msgid "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field 'States in which an item will be automatically sent to selected other meeting configurations' here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the 'Transitions for presenting an item' you defined in the 'Workflows' tab of the meeting configuration the item will be sent to."
 msgstr "Lorsque le point a été envoyé vers l'autre type de séance, il est créé dans son état initial.  Si le point a été envoyé vers l'autre type de séance automatiquement (dépendant des états sélectionnés ci-dessous dans le champ \"Etats dans lesquels un point sera automatiquement envoyé vers les autres configurations de séances\") ou s'il est envoyé manuellement par un gestionnaire de séances, certaines transitions supplémentaires peuvent être exécutées de sorte que le point soit mis dans l'état voulu. Sélectionnez jusqu'à quelle transition cela sera effectué (la transition sélectionnée sera également exécutée). Ceci nécessite que les \"Transitions pour présenter un point\" définies dans l'onglet \"Workflows\" du type de séance vers lequel le point sera envoyé soit correctement définies."
 
 #. Default: "Specify here a TAL expression that will restrict or allow the use of this advice to some condition.  We receive \"item\" as the meeting item to give an advice on and \"mayEdit\", a boolean to know if current user may edit the item.  A special expression is available to protect a row that should only be available thru the \"Change delay\" action, it is : \"python: item.REQUEST.get('managing_available_delays', False)\".  This can not be used if something is defined in the \"Advice will be automatically asked if\" column of this advice, but for optional delay-aware advice or for delay-aware advices linked to an automatic advice (using the \"Is linked to previous row?\" column)"
 msgid "available_on_col_description"
 msgstr "Spécifiez une expression TAL qui permet de restreindre ou d'accorder l'utilisation de certaines valeurs pour cet avis à certains utilisateurs.  Les éléments \"item\" (point) et \"mayEdit\" (un booléen qui est True si utilisateur courant peut éditer le point) sont utilisables dans l'expression.  Si une valeur ne doit pouvoir être utilisée que via l'action \"Changer le délai\" (icône horloge grise) d'un avis, l'expression à utiliser est : \"python: item.REQUEST.get('managing_available_delays', False)\".  Vous ne pouvez pas renseigner une expression dans cette colonne si une expression est définie dans la colonne \"L'avis sera automatiquement demandé si\" de la même ligne de configuration mais vous pouvez l'utiliser avec les avis optionnels ou les lignes liées à un avis automatique (c'est-à-dire si la colonne \"Lié à la ligne précédente?\" est utilisée sur un avis automatique)"
 
+#. Default: "Used to automatically determinate the committee for the item, the field \"Committees\" will not appear on the item when editing it (except for MeetingManagers).  This may only be used when column \"using_groups\" is not used."
+msgid "committees_auto_from_col_description"
+msgstr "Active le mode \"automatique\" pour déterminer les commissions d'un point, le champ permettant de sélectionner les commissions n'apparaîtra pas lors de l'édition du point (sauf pour les gestionnaires de séances). Ce paramètre ne peut pas être utilisé avec le paramètre \"Restreindre à\"."
+
+#. Default: "Used when creating a new meeting if field \"Assembly\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_assembly_col_description"
+msgstr "Utilisé à la création d'une nouvelle séance si la paramère \"Assemblée (committees_assembly)\" est activé sur les séances. N'impacte pas les séances déjà créées."
+
+#. Default: "Used when creating a new meeting if field \"Attendees\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_attendees_col_description"
+msgstr "Utilisé à la création d'une nouvelle séance si la paramère \"Présents (committees_attendees)\" est activé sur les séances. N'impacte pas les séances déjà créées."
+
+#. Default: "Used when creating a new meeting if field \"Place\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_place_col_description"
+msgstr "Utilisé à la création d'une nouvelle séance si la paramère \"Lieu (committees_place)\" est activé sur les séances. N'impacte pas les séances déjà créées."
+
+#. Default: "Used when creating a new meeting if field \"Signatories\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatories_col_description"
+msgstr "Utilisé à la création d'une nouvelle séance si la paramère \"Signataires (committees_signatories)\" est activé sur les séances. N'impacte pas les séances déjà créées."
+
+#. Default: "Used when creating a new meeting if field \"Signatures\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatures_col_description"
+msgstr "Utilisé à la création d'une nouvelle séance si la paramère \"Signatures (committees_signatures)\" est activé sur les séances. N'impacte pas les séances déjà créées."
+
+#. Default: "Will generate new values on item \"Committees\" field when necessary to manage supplements (items added to meeting after committees convocation were sent).  This will only be useable by MeetingManagers."
+msgid "committees_supplements_col_description"
+msgstr "Permet de gérer les suppléments pour les commissions. Ces valeurs peuvent être sélectionnées sur le point uniquement par les gestionnaires de séances."
+
+#. Default: "Used to restrict availability of a committee on the item committees selection box.  This may only be used when column \"auto_from\" is not used."
+msgid "committees_using_groups_col_description"
+msgstr "Si le mode \"automatique\" n'est pas activé, le champ permettant de sélectionner les commissions apparaîtra lors de l'édition du point, ceci permet de restreindre les valeurs sélectionnables en fonction du groupe proposant du point. Ce paramètre ne peut pas être utilisé avec le paramètre \"Automatiquement si\"."
+
 #. Default: "Enter the delay the adviser will have to give his advice. If it is not considered as an automatically asked advice (nothing defined in the \"Advice will be automatically asked if\" column), the advice will be selectable in the \"Ask advice to\" list on the item edit form. A delay is a single digit (like \"5\" or \"10\"). If no delay is relevant for this advice, leave this field blank. If several delays are possible for the same advice, you have to define several rows with exactly the same content excepted the delay."
 msgid "delay_col_description"
 msgstr "Spécifiez le délai en nombre de jours francs que le groupe aura pour rendre son avis. Si cet avis n'est pas considéré comme un avis automatique (rien n'a été défini dans la colonne \"L'avis sera automatiquement demandé si\"), l'avis sera sélectionnable dans la liste déroulante \"Demander l'avis de\" sur le formulaire d'édition d'un point. Un délai est encodé sous forme d'un nombre unique (par exemple \"5\" ou \"10\"). Si cet avis n'a pas de notion de délai, laissez ce champ vide. Si plusieurs délais sont relevants pour cet avis, créez autant de lignes que nécessaire."
 
 #. Default: "If you want a specific label to be displayed on the label displayed in the \"Advice to give\" list on the item edit form and on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The label will appear between brackets after the message \"Name of the group - delay of X days\"."
 msgid "delay_label_col_description"
 msgstr "Si vous souhaitez qu'un libellé soit affiché à côté de la valeur affichée dans la liste déroulante \"Demander l'avis de\" sur le formulaire d'édition d'un point ainsi qu'au survol du \"?\" affiché dans l'interface utilisateur à côté du titre d'un avis demandé, entrez-le ici.  Ce message apparaîtra entre parenthèses après le message \"Nom du groupe qui doit rendre l'avis - délai de X jours\".  Ce libellé doit être le plus concis possible."
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/PloneMeeting.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 msgid "${term_title} (Not selected in plonegroup)"
 msgstr "${term_title} (Non sélectionné dans plonegroup)"
 
 #. Default: "(Nobody)"
 msgid "(Nobody)"
 msgstr "(Personne)"
 
+#. Default: "(None)"
+msgid "(None)"
+msgstr "(Aucune)"
+
 #. Default: "Add PloneMeeting Portlet"
 msgid "Add PloneMeeting Portlet"
 msgstr "Ajout d'un portlet 'PloneMeeting'"
 
 #. Default: "Add Todo Portlet"
 msgid "Add Todo Portlet"
 msgstr "Ajout d'un portlet 'à faire'"
@@ -156,14 +160,18 @@
 msgid "Attendee has been set signatory."
 msgstr "Le membre est désormais signataire pour ce point."
 
 #. Default: "Attendee is no more defined as item signatory."
 msgid "Attendee is no more defined as item signatory."
 msgstr "Le membre a été enlevé des signataires pour ce point."
 
+#. Default: "Attendee position has been redefined."
+msgid "Attendee position has been redefined."
+msgstr "La fonction du membre a été redéfinie pour ce point."
+
 #. Default: "Back to the MeetingConfig"
 msgid "Back to the MeetingConfig"
 msgstr "Retourner sur la Configuration de séance"
 
 #. Default: "Back to the item"
 msgid "Back to the item"
 msgstr "Retourner sur le point"
@@ -240,14 +248,18 @@
 msgid "Close"
 msgstr "Fermer"
 
 #. Default: "Comment"
 msgid "Comment"
 msgstr "Commentaire"
 
+#. Default: "Completed votes"
+msgid "Completed votes"
+msgstr "Votes complétés"
+
 #. Default: "Contacts fields"
 msgid "Contacts fields"
 msgstr "Champs utilisant des contacts"
 
 #. Default: "Copy PloneMeeting"
 msgid "Copy PloneMeeting"
 msgstr "Copier points"
@@ -468,38 +480,14 @@
 msgid "If you need to use this person data in the application like for example scanned signature or telephone number, select it here."
 msgstr "Utile afin de pouvoir utiliser les données de cette personne, comme par exemple la signature scannée ou le numéro de téléphone."
 
 #. Default: "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 msgid "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 msgstr "Si vous spécifiez un numéro, les valeurs définies ci-dessus seront appliquées à partir du point courant jusqu'au point ayant ce numéro.  Laissez ce champ vide pour appliquer uniquement sur le point courant."
 
-#. Default: "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgstr "Encodez le numéro du point jusqu'auquel ce membre doit être marqué comme absent.  Laissez le champ vide pour le marquer absent uniquement pour le point en cours."
-
-#. Default: "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgstr "Encodez le numéro du point jusqu'auquel ce membre doit être enlevé des non participants.  Laissez le champ vide pour l'enlever des non participants uniquement pour le point en cours."
-
-#. Default: "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgstr "Encodez le numéro du point jusqu'auquel ce membre doit être enlevé des absents.  Laissez le champ vide pour l'enlever des absents uniquement pour le point en cours."
-
-#. Default: "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgstr "Encodez le numéro du point jusqu'auquel ce membre doit être marqué comme non participant.  Laissez le champ vide pour le marquer non participant uniquement pour le point en cours."
-
-#. Default: "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgstr "Encodez le numéro du point jusqu'auquel ce membre doit être marqué comme signataire.  Laissez le champ vide pour le marquer signataire uniquement pour le point en cours."
-
-#. Default: "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgstr "Encodez le numéro du point jusqu'auquel ce membre doit être enlevé des signataires.  Laissez le champ vide pour l'enlever seulement des signataires du point en cours."
-
 # plone.app.querystring
 #. Default: "Informations about advices on an item"
 msgid "Informations about advices on an item"
 msgstr "Les informations concernant les avis sur un point"
 
 #. Default: "Inherited advice action"
 msgid "Inherited advice action"
@@ -739,22 +727,30 @@
 msgid "None"
 msgstr "Aucun"
 
 #. Default: "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 msgid "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 msgstr "Impossible d'ajouter un vote lié car des valeurs incompatibles ont déjà été encodées sur le vote courant"
 
+#. Default: "Not completed votes"
+msgid "Not completed votes"
+msgstr "Votes non complétés"
+
 #. Default: "Not present type"
 msgid "Not present type"
 msgstr "Type d'absence"
 
 #. Default: "Not voter"
 msgid "Not voter"
 msgstr "Non votant"
 
+#. Default: "Nothing selected in the configuration to be displayed."
+msgid "Nothing selected in the configuration to be displayed."
+msgstr "Aucun champ sélectionné dans la configuration."
+
 #. Default: "Nothing to display when item is not presented into a meeting."
 msgid "Nothing to display when item is not presented into a meeting."
 msgstr "Rien à afficher tant que le point n'est pas présenté dans une séance."
 
 #. Default: "Nothing to display."
 msgid "Nothing to display."
 msgstr "Rien à afficher."
@@ -783,14 +779,18 @@
 msgid "Ordered groups"
 msgstr "Ordre des groupes"
 
 #. Default: "Original meeting signatory"
 msgid "Original meeting signatory"
 msgstr "Signataire défini sur la séance"
 
+#. Default: "Original position"
+msgid "Original position"
+msgstr "Fonction sur la séance"
+
 #. Default: "POD template to annex"
 msgid "POD template to annex"
 msgstr "Modèle de document à annexer"
 
 #. Default: "Please check item number ${item_number} at ${item_url}."
 msgid "Please check item number ${item_number} at ${item_url}."
 msgstr "Vérifiez le point numéro \"${item_number}\" (${item_url})."
@@ -823,23 +823,14 @@
 msgid "PloneMeeting_inAndOutMoves"
 msgstr "Entrées et sorties (assemblée)"
 
 #. Default: "Observations"
 msgid "PloneMeeting_itemObservations"
 msgstr "Observations"
 
-#. Default: "Observations"
-msgid "PloneMeeting_itemObservations2"
-msgstr "Observations"
-
-# MeetingGroup
-#. Default: "Absents"
-msgid "PloneMeeting_label_absents"
-msgstr "Absents (non excusés)"
-
 #. Default: "Acronym"
 msgid "PloneMeeting_label_acronym"
 msgstr "Acronyme"
 
 #. Default: "Confidential advice annexes are visible for"
 msgid "PloneMeeting_label_adviceAnnexConfidentialVisibleFor"
 msgstr "Les annexes confidentielles des avis sont visible par"
@@ -876,50 +867,26 @@
 msgid "PloneMeeting_label_annexToPrintMode"
 msgstr "Mode d'impression des annexes"
 
 #. Default: "Answers"
 msgid "PloneMeeting_label_answerers"
 msgstr "Réponses"
 
-#. Default: "Meeting approval date"
-msgid "PloneMeeting_label_approvalDate"
-msgstr "Date d'approbation de la séance"
-
 #. Default: "As copy group on"
 msgid "PloneMeeting_label_asCopyGroupOn"
 msgstr "Le groupe sera automatiquement mis en copie d'un point si"
 
-#. Default: "Default assembly"
-msgid "PloneMeeting_label_assembly"
-msgstr "Assemblée par défaut"
-
-#. Default: "Default assembly staves"
-msgid "PloneMeeting_label_assemblyStaves"
-msgstr "Assistants par défaut"
-
 #. Default: "Associated group(s)"
 msgid "PloneMeeting_label_associatedGroups"
 msgstr "Groupes associés"
 
-#. Default: "Attendees"
-msgid "PloneMeeting_label_attendees"
-msgstr "Présents"
-
-#. Default: "Authority notice"
-msgid "PloneMeeting_label_authorityNotice"
-msgstr "Avis de tutelle"
-
 #. Default: "Columns to display for items available for a meeting"
 msgid "PloneMeeting_label_availableItemsListVisibleColumns"
 msgstr "Colonnes à afficher pour les points disponibles pour une séance"
 
-#. Default: "Items"
-msgid "PloneMeeting_label_body"
-msgstr "Points"
-
 #. Default: "Default value for the \"budget information\" field"
 msgid "PloneMeeting_label_budgetDefault"
 msgstr "Valeur par défaut du champ \"Informations budgétaires\""
 
 #. Default: "Budgetary informations"
 msgid "PloneMeeting_label_budgetInfos"
 msgstr "Informations budgétaires"
@@ -948,14 +915,18 @@
 msgid "PloneMeeting_label_classifier"
 msgstr "Classificateur"
 
 #. Default: "Observations for the committee"
 msgid "PloneMeeting_label_committeeObservations"
 msgstr "Observations pour les commissions"
 
+#. Default: "Committees"
+msgid "PloneMeeting_label_committees"
+msgstr "Commissions"
+
 #. Default: "Completeness"
 msgid "PloneMeeting_label_completeness"
 msgstr "Complétude"
 
 #. Default: "Group of meeting configurations"
 msgid "PloneMeeting_label_configGroup"
 msgstr "Groupe de Configurations de séance"
@@ -972,18 +943,14 @@
 msgid "PloneMeeting_label_configVersion"
 msgstr "Identifiant de la version de cette configuration"
 
 #. Default: "Contents to keep when item sent to another configuration"
 msgid "PloneMeeting_label_contentsKeptOnSentToOtherMC"
 msgstr "Éléments à garder lors de l'envoi vers une autre configuration de séance"
 
-#. Default: "Meeting convocation date"
-msgid "PloneMeeting_label_convocationDate"
-msgstr "Date de convocation"
-
 #. Default: "Copy groups"
 msgid "PloneMeeting_label_copyGroups"
 msgstr "Groupes en copie (lecture seule)"
 
 #. Default: "Css classes to hide"
 msgid "PloneMeeting_label_cssClassesToHide"
 msgstr "Classes Css à cacher"
@@ -1000,26 +967,14 @@
 msgid "PloneMeeting_label_dashboardMeetingAvailableItemsFilters"
 msgstr "Filtres avancés à afficher pour les \"Points disponibles\" d'une séance"
 
 #. Default: "Advanced filters to show on \"Items of a meeting\""
 msgid "PloneMeeting_label_dashboardMeetingLinkedItemsFilters"
 msgstr "Filtres avancés à afficher pour les points présentés dans une séance"
 
-#. Default: "Date"
-msgid "PloneMeeting_label_date"
-msgstr "Date"
-
-#. Default: "Deadline for validating late items"
-msgid "PloneMeeting_label_deadlineFreeze"
-msgstr "Echéance pour valider les points en urgence"
-
-#. Default: "Deadline for validating items"
-msgid "PloneMeeting_label_deadlinePublish"
-msgstr "Echéance pour valider les points"
-
 #. Default: "Decision"
 msgid "PloneMeeting_label_decision"
 msgstr "Décision"
 
 #. Default: "Decision (end)"
 msgid "PloneMeeting_label_decisionEnd"
 msgstr "Décision (fin)"
@@ -1056,26 +1011,18 @@
 msgid "PloneMeeting_label_delayUnavailableEndDays"
 msgstr "Un délai ne peut pas se terminer les jours suivants"
 
 #. Default: "Description"
 msgid "PloneMeeting_label_description"
 msgstr "Description"
 
-#. Default: "Description in the second language"
-msgid "PloneMeeting_label_description2"
-msgstr "Description dans la seconde langue"
-
 #. Default: "Detailed description"
 msgid "PloneMeeting_label_detailedDescription"
 msgstr "Description détaillée"
 
-#. Default: "Detailed description"
-msgid "PloneMeeting_label_detailedDescription2"
-msgstr "Description détaillée"
-
 #. Default: "Display available items to"
 msgid "PloneMeeting_label_displayAvailableItemsTo"
 msgstr "Afficher les points disponibles sur une séance aux"
 
 #. Default: "Emergency"
 msgid "PloneMeeting_label_emergency"
 msgstr "Urgence"
@@ -1100,46 +1047,30 @@
 msgid "PloneMeeting_label_enableScanDocs"
 msgstr "Activer le scanning de documents"
 
 #. Default: "Enable user preferences"
 msgid "PloneMeeting_label_enableUserPreferences"
 msgstr "Activer les préférences utilisateur"
 
-#. Default: "Effective end date and hour"
-msgid "PloneMeeting_label_endDate"
-msgstr "Date et heure effective de fin"
+#. Default: "Enabled annexes batch actions"
+msgid "PloneMeeting_label_enabledAnnexesBatchActions"
+msgstr "Actions par lot activées sur les annexes"
 
 #. Default: "Enforce advice mandatoriness"
 msgid "PloneMeeting_label_enforceAdviceMandatoriness"
 msgstr "Appliquer le caractère obligatoire des avis"
 
-#. Default: "Excused"
-msgid "PloneMeeting_label_excused"
-msgstr "Excusés"
-
-#. Default: "Extraordinary session?"
-msgid "PloneMeeting_label_extraordinarySession"
-msgstr "Séance extraordinaire?"
-
-#. Default: "Number of the first item contained in this meeting"
-msgid "PloneMeeting_label_firstItemNumber"
-msgstr "Numéro du premier point de cette séance"
-
 #. Default: "First linked vote values"
 msgid "PloneMeeting_label_firstLinkedVoteUsedVoteValues"
 msgstr "Valeurs de votes utilisables sur le premier vote lié"
 
 #. Default: "Name of the folder linked to this configuration"
 msgid "PloneMeeting_label_folderTitle"
 msgstr "Nom du répertoire lié à cette configuration"
 
-#. Default: "Default deadline for validating late items for a given meeting"
-msgid "PloneMeeting_label_freezeDeadlineDefault"
-msgstr "Echéance par défaut pour valider les points en urgence pour une séance donnée"
-
 #. Default: "Email of the functional administrator"
 msgid "PloneMeeting_label_functionalAdminEmail"
 msgstr "Courriel de l'administrateur fonctionnel"
 
 #. Default: "Name of the functional administrator"
 msgid "PloneMeeting_label_functionalAdminName"
 msgstr "Nom de l'administrateur fonctionnel"
@@ -1180,18 +1111,14 @@
 msgid "PloneMeeting_label_historizeItemDataWhenAdviceIsGiven"
 msgstr "Historiser les informations essentielles du point lorsqu'un avis est rendu"
 
 #. Default: "Item attributes for which history must be kept"
 msgid "PloneMeeting_label_historizedItemAttributes"
 msgstr "Attributs des points pour lesquels l'historique doit être conservé"
 
-#. Default: "Meeting attributes for which history must be kept"
-msgid "PloneMeeting_label_historizedMeetingAttributes"
-msgstr "Attributs des séances pour lesquels l'historique doit être conservé"
-
 #. Default: "Holidays"
 msgid "PloneMeeting_label_holidays"
 msgstr "Jours fériés"
 
 #. Default: "Include groups in charge defined on category"
 msgid "PloneMeeting_label_includeGroupsInChargeDefinedOnCategory"
 msgstr "Inclure les groupes en charge définis sur la catégorie du point"
@@ -1369,18 +1296,14 @@
 msgid "PloneMeeting_label_itemWithGivenAdviceIsNotDeletable"
 msgstr "Empêcher qu'un point sur lequel des avis ont été rendus soit supprimé?"
 
 #. Default: "Workflow that dictates the life cycle of every item into this configuration"
 msgid "PloneMeeting_label_itemWorkflow"
 msgstr "Workflow gouvernant le cycle de vie de chaque point de cette configuration"
 
-#. Default: "Items"
-msgid "PloneMeeting_label_items"
-msgstr "Points"
-
 #. Default: "Columns to display for items within a meeting"
 msgid "PloneMeeting_label_itemsListVisibleColumns"
 msgstr "Colonnes à afficher pour les points présentés dans une séance"
 
 #. Default: "Fields of the items to show/hide in the dashboards"
 msgid "PloneMeeting_label_itemsListVisibleFields"
 msgstr "Champs des points à Afficher/masquer dans les tableaux de bords"
@@ -1469,18 +1392,14 @@
 msgid "PloneMeeting_label_meetingColumns"
 msgstr "Colonnes à afficher sur les listes de séances"
 
 #. Default: "Interface allowing to use a specific Zope3 adapter for modifying the conditions defined on the transitions of the meeting workflow"
 msgid "PloneMeeting_label_meetingConditionsInterface"
 msgstr "Interface permettant d'utiliser un adapter Zope3 spécifique pour modifier les conditions définies sur les transitions du workflow gouvernant les séances"
 
-#. Default: "Identifier of the configuration's version that is linked to this meeting"
-msgid "PloneMeeting_label_meetingConfigVersion"
-msgstr "Identifiant de la version de la configuration liée à cette séance"
-
 #. Default: "Meeting configs to clone items to"
 msgid "PloneMeeting_label_meetingConfigsToCloneTo"
 msgstr "Configurations de séance vers lesquelles les points de cette configuration de séance peuvent être envoyés"
 
 #. Default: "Title of the folder created in each user folder"
 msgid "PloneMeeting_label_meetingFolderTitle"
 msgstr "Titre du répertoire créé dans chaque répertoire d'utilisateur"
@@ -1497,58 +1416,38 @@
 msgid "PloneMeeting_label_meetingManagersNotesEnd"
 msgstr "Notes gestionnaires de séances (fin)"
 
 #. Default: "MeetingManagers notes (suite)"
 msgid "PloneMeeting_label_meetingManagersNotesSuite"
 msgstr "Notes gestionnaires de séances (suite)"
 
-#. Default: "Meeting number (sequence number automatically attributed)"
-msgid "PloneMeeting_label_meetingNumber"
-msgstr "Numéro de séance (il s'agit d'un numéro de séquence attribué automatiquement)"
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations"
-msgstr "Observations"
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations2"
-msgstr "Observations"
-
 #. Default: "States of the meeting to insert an item into from everywhere"
 msgid "PloneMeeting_label_meetingPresentItemWhenNoCurrentMeetingStates"
 msgstr "États des séances pris en compte pour déterminer la séance dans laquelle doit être présenté un point (lorsque le gestionnaire de séance n'est pas sur une séance)"
 
 #. Default: "Meeting transition that triggers the insertion of this item as a recurring item"
 msgid "PloneMeeting_label_meetingTransitionInsertingMe"
 msgstr "Transition de la séance qui déclenche l'ajout de ce point en tant que point récurrent"
 
 #. Default: "Workflow that dictates the life cycle of every meeting into this configuration"
 msgid "PloneMeeting_label_meetingWorkflow"
 msgstr "Workflow gouvernant le cycle de vie de chaque séance de cette configuration"
 
-#. Default: "End date for meeting first part"
-msgid "PloneMeeting_label_midDate"
-msgstr "Date de fin de la première partie"
-
 #. Default: "Model adaptations"
 msgid "PloneMeeting_label_modelAdaptations"
 msgstr "Adaptations au modèle de données"
 
 #. Default: "Motivation"
 msgid "PloneMeeting_label_motivation"
 msgstr "Motivation"
 
 #. Default: "Next linked votes values"
 msgid "PloneMeeting_label_nextLinkedVotesUsedVoteValues"
 msgstr "Valeurs de vote utilisables sur les votes liés suivants"
 
-#. Default: "Non attendees"
-msgid "PloneMeeting_label_nonAttendees"
-msgstr "Non participants"
-
 #. Default: "Actions to execute on items of a meeting when a transition is triggered on that meeting"
 msgid "PloneMeeting_label_onMeetingTransitionItemActionToExecute"
 msgstr "Actions à exécuter sur les points d'une séance lorsqu'une transition est déclenchée sur cette séance"
 
 #. Default: "Transforms to apply to rich text fields of an item after a workflow transition"
 msgid "PloneMeeting_label_onTransitionFieldTransforms"
 msgstr "Adaptations à appliquer aux zones de texte riche d'un point lors d'une transition de workflow"
@@ -1565,14 +1464,18 @@
 msgid "PloneMeeting_label_oralQuestion"
 msgstr "Ce point est une question orale ?"
 
 #. Default: "Associated organizations order"
 msgid "PloneMeeting_label_orderedAssociatedOrganizations"
 msgstr "Groupes associés sélectionnables sur les points"
 
+#. Default: "Attendees selectable for committees"
+msgid "PloneMeeting_label_orderedCommitteeContacts"
+msgstr "Membres d'assemblée des commissions sélectionnables"
+
 #. Default: "Selectable assembly members"
 msgid "PloneMeeting_label_orderedContacts"
 msgstr "Membres d'assemblée sélectionnables"
 
 #. Default: "Ordered groups in charge"
 msgid "PloneMeeting_label_orderedGroupsInCharge"
 msgstr "Groupes en charge sélectionnables sur les points"
@@ -1595,19 +1498,15 @@
 
 #. Default: "Leave unchecked if item is public"
 msgid "PloneMeeting_label_otherMeetingConfigsClonableToPrivacy"
 msgstr "Non coché = séance publique"
 
 #. Default: "Owner of a annex decision may delete it when item is no more editable?"
 msgid "PloneMeeting_label_ownerMayDeleteAnnexDecision"
-msgstr "L'utilisateur ayant ajouté une 'annexe après décision' peut la supprimer lorsque le point n'est plus éditable?"
-
-#. Default: "Place"
-msgid "PloneMeeting_label_place"
-msgstr "Lieu"
+msgstr "L'utilisateur ayant ajouté une \"Annexe (après décision)\" peut la supprimer lorsque le point n'est plus éditable?"
 
 #. Default: "Meeting places"
 msgid "PloneMeeting_label_places"
 msgstr "Lieux pour les séances"
 
 #. Default: "Poll type"
 msgid "PloneMeeting_label_pollType"
@@ -1621,42 +1520,18 @@
 msgid "PloneMeeting_label_powerAdvisersGroups"
 msgstr "Groupes considérés comme \"Super émetteurs d'avis\""
 
 #. Default: "Manage power observers"
 msgid "PloneMeeting_label_powerObservers"
 msgstr "Configuration des \"Super observateurs\""
 
-#. Default: "Date"
-msgid "PloneMeeting_label_preMeetingDate"
-msgstr "Date"
-
-#. Default: "Default date for the pre-meeting"
-msgid "PloneMeeting_label_preMeetingDateDefault"
-msgstr "Date par défaut pour la séance préparatoire"
-
-#. Default: "Place"
-msgid "PloneMeeting_label_preMeetingPlace"
-msgstr "Lieu"
-
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations"
-msgstr "Observations pour la réunion préparatoire"
-
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations2"
-msgstr "Observations pour la réunion préparatoire"
-
 #. Default: "Previous item"
 msgid "PloneMeeting_label_predecessor"
 msgstr "Point précédent"
 
-#. Default: "Predefined title in the second language"
-msgid "PloneMeeting_label_predefinedTitle2"
-msgstr "Titre prédéfini dans la seconde langue"
-
 #. Default: "Preferred meeting"
 msgid "PloneMeeting_label_preferredMeeting"
 msgstr "Séance souhaitée"
 
 #. Default: "Privacy"
 msgid "PloneMeeting_label_privacy"
 msgstr "Niveau de confidentialité"
@@ -1665,38 +1540,26 @@
 msgid "PloneMeeting_label_proposingGroup"
 msgstr "Groupe proposant"
 
 #. Default: "Proposing group (Group in charge)"
 msgid "PloneMeeting_label_proposingGroupWithGroupInCharge"
 msgstr "Groupe proposant (Groupe en charge)"
 
-#. Default: "Observations for public meeting"
-msgid "PloneMeeting_label_publicMeetingObservations"
-msgstr "Observations pour la séance publique"
-
 #. Default: "Public URL"
 msgid "PloneMeeting_label_publicUrl"
 msgstr "URL publique"
 
-#. Default: "Default deadline for validating items for a given meeting"
-msgid "PloneMeeting_label_publishDeadlineDefault"
-msgstr "Échéance par défaut pour valider les points pour une séance donnée"
-
 #. Default: "Questions"
 msgid "PloneMeeting_label_questioners"
 msgstr "Questions"
 
 #. Default: "Item states into which events will be recorded in item's history"
 msgid "PloneMeeting_label_recordItemHistoryStates"
 msgstr "États des points dans lesquels l'historisation est active"
 
-#. Default: "Meeting states into which events will be recorded in meeting's history"
-msgid "PloneMeeting_label_recordMeetingHistoryStates"
-msgstr "États des séances dans lesquels l'historisation est active"
-
 #. Default: "Redirect to the next meeting"
 msgid "PloneMeeting_label_redirectToNextMeeting"
 msgstr "Rediriger vers la prochaine séance les"
 
 #. Default: "Remove annexes previews on meeting closure"
 msgid "PloneMeeting_label_removeAnnexesPreviewsOnMeetingClosure"
 msgstr "Supprimer les prévisualisations des annexes lors de la clôture de la séance"
@@ -1713,30 +1576,30 @@
 msgid "PloneMeeting_label_restrictAccessToSecretItemsTo"
 msgstr "Restreindre l'accès aux points à huis clos aux"
 
 #. Default: "\"Restrict users\" mode"
 msgid "PloneMeeting_label_restrictUsers"
 msgstr "Mode \"Utilisateurs restreints\""
 
-#. Default: "Observations for the secret meeting"
-msgid "PloneMeeting_label_secretMeetingObservations"
-msgstr "Observations pour le huis clos"
-
 #. Default: "Selectable advisers"
 msgid "PloneMeeting_label_selectableAdvisers"
 msgstr "Groupes auxquels un avis optionnel pourra être demandé"
 
 #. Default: "Groups that can be in copy for an item"
 msgid "PloneMeeting_label_selectableCopyGroups"
 msgstr "Groupes qui pourront être mis en copie"
 
 #. Default: "Selectable privacies"
 msgid "PloneMeeting_label_selectablePrivacies"
 msgstr "Niveaux de confidentialité utilisés"
 
+#. Default: "Restrict selectable redefined position types to following positions"
+msgid "PloneMeeting_label_selectableRedefinedPositionTypes"
+msgstr "Restreindre les types de fonctions sélectionnables lors du changement de la fonction d'un membre d'assemblée pour un point aux fonctions suivantes"
+
 #. Default: "Is group selectable in the plonegroup configuration panel?"
 msgid "PloneMeeting_label_selectable_for_plonegroup"
 msgstr "Groupe sélectionnable dans la Configuration des groupes plone via contact?"
 
 #. Default: "Send to authority?"
 msgid "PloneMeeting_label_sendToAuthority"
 msgstr "À transmettre à la tutelle?"
@@ -1749,26 +1612,18 @@
 msgid "PloneMeeting_label_showItemKeywordsTargets"
 msgstr "Montrer les cibles possibles pour les mots-clé de recherches de points"
 
 #. Default: "Signatories"
 msgid "PloneMeeting_label_signatories"
 msgstr "Signataires"
 
-#. Default: "Default signatures"
-msgid "PloneMeeting_label_signatures"
-msgstr "Signatures par défaut"
-
 #. Default: "Sort the tags alphabetically"
 msgid "PloneMeeting_label_sortAllItemTags"
 msgstr "Trier les marqueurs par ordre alphabétique"
 
-#. Default: "Effective start date and hour"
-msgid "PloneMeeting_label_startDate"
-msgstr "Date et heure effective de début"
-
 #. Default: "Meeting file sub types"
 msgid "PloneMeeting_label_subTypes"
 msgstr "Sous-types de fichier"
 
 #. Default: "Taken over by"
 msgid "PloneMeeting_label_takenOverBy"
 msgstr "Pris en charge par"
@@ -1777,23 +1632,14 @@
 msgid "PloneMeeting_label_templateUsingGroups"
 msgstr "Restreindre ce modèle de point aux groupes suivants"
 
 #. Default: "Checklist"
 msgid "PloneMeeting_label_textCheckList"
 msgstr "Checklist"
 
-# Meeting
-#. Default: "Title"
-msgid "PloneMeeting_label_title"
-msgstr "Titre"
-
-#. Default: "Title in the second language"
-msgid "PloneMeeting_label_title2"
-msgstr "Titre dans la seconde langue"
-
 #. Default: "To discuss ?"
 msgid "PloneMeeting_label_toDiscuss"
 msgstr "À évoquer en séance?"
 
 #. Default: "Default value of the \"toDiscuss\" attribute for normal items"
 msgid "PloneMeeting_label_toDiscussDefault"
 msgstr "Valeur par défaut de l'attribut \"A évoquer en séance?\" pour les points normaux"
@@ -1914,38 +1760,38 @@
 msgid "PloneMeeting_label_xhtmlTransformTypes"
 msgstr "Types de transformations pour les champs de texte riche"
 
 #. Default: "Reinitialise meeting number every year?"
 msgid "PloneMeeting_label_yearlyInitMeetingNumber"
 msgstr "Réinitialiser le numéro de séance chaque année?"
 
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations"
-msgstr "Observations"
-
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations2"
-msgstr "Observations"
-
 #. Default: "Notes"
 msgid "PloneMeeting_notes"
 msgstr "Notes et interpellations"
 
 #. Default: "Document templates"
 msgid "PodTemplates"
 msgstr "Modèles de documents"
 
 #. Default: "Position type"
 msgid "Position type"
 msgstr "Type de fonction"
 
+#. Default: "Position type to use"
+msgid "Position type to use"
+msgstr "Fonction à utiliser"
+
 #. Default: "Position type to use as label for the signature."
 msgid "Position type to use as label for the signature."
 msgstr "Sélectionnez la fonction qui sera utilisée sur la signature affichée dans les documents générés. Par défaut le \"Type de fonction secondaire\" défini sur la fonction occupée est sélectionné, si vide le \"Type de fonction\" sera alors sélectionné."
 
+#. Default: "Position type to use for the attendee on this item."
+msgid "Position type to use for the attendee on this item."
+msgstr "Sélectionnez la fonction qui sera utilisée pour ce membre d'assemblée sur ce point."
+
 #. Default: "Preview detailed advice"
 msgid "Preview detailed advice"
 msgstr "Prévisualiser l'avis complet"
 
 #. Default: "Preview of annexes were deleted upon meeting closure."
 msgid "Preview of annexes were deleted upon meeting closure."
 msgstr "Les prévisualisations des annexes de tous les points ont été supprimées lors de la clôture de la séance."
@@ -1955,14 +1801,26 @@
 msgid "Previous review state"
 msgstr "État précédent"
 
 #. Default: "Recurring items"
 msgid "RecurringItems"
 msgstr "Points récurrents"
 
+#. Default: "Redefine position for this attendee for this item"
+msgid "Redefine position for this attendee for this item"
+msgstr "Changer la fonction de ce membre pour ce point"
+
+#. Default: "Redefined attendee position was removed."
+msgid "Redefined attendee position was removed."
+msgstr "Le membre utilise à nouveau sa fonction définie sur la séance pour ce point."
+
+#. Default: "Redefined position"
+msgid "Redefined position"
+msgstr "Fonction pour le point"
+
 #. Default: "References of contained items have been updated."
 msgid "References of contained items have been updated."
 msgstr "La référence des points a été mise à jour."
 
 #. Default: "Reinitiatlize delay"
 msgid "Reinitiatlize delay"
 msgstr "Réinitialiser le délai pour cet avis"
@@ -1979,14 +1837,18 @@
 msgid "Remove inherited advice"
 msgstr "Enlever l'avis hérité"
 
 #. Default: "Remove inherited advice and ask advice locally"
 msgid "Remove inherited advice and ask advice locally"
 msgstr "Enlever l'avis hérité et demander l'avis à nouveau sur ce point"
 
+#. Default: "Remove redefined attendee position for this item"
+msgid "Remove redefined attendee position for this item"
+msgstr "Enlever la fonction redéfinie pour ce membre pour ce point"
+
 #. Default: "Represented organizations"
 msgid "Represented organizations"
 msgstr "Organisations représentées"
 
 #. Default: "Searches"
 msgid "Searches"
 msgstr "Recherches"
@@ -2039,14 +1901,18 @@
 msgid "Signature number"
 msgstr "Numéro de signature"
 
 #. Default: "Signature position type"
 msgid "Signature position type"
 msgstr "Fonction pour la signature"
 
+#. Default: "Specify a number to which this will be applied. Field default is current item number."
+msgid "Specify a number to which this will be applied. Field default is current item number."
+msgstr "Encodez le numéro du point jusqu'auquel appliquer ce changement.  <br/>Ce champ contient par défaut le numéro du point en cours."
+
 #. Default: "state"
 msgid "State"
 msgstr "État"
 
 #. Default: "Style templates"
 msgid "Style templates"
 msgstr "Modèles de style"
@@ -2090,14 +1956,18 @@
 msgstr "Le point que vous avez essayé de prendre en charge a été pris en charge entretemps par ${fullname}.  Vous pouvez maintenant le prendre en charge à sa place si vous êtes sûr qu'il ne le gère pas déjà."
 
 # plone.app.querystring
 #. Default: "The item, advice or meeting previous review state"
 msgid "The item, advice or meeting previous review state"
 msgstr "L'état du WF précdent pour le point, l'avis ou la séance"
 
+#. Default: "The position of this attendee was changed for the ${number} following item(s)"
+msgid "The position of this attendee was changed for the ${number} following item(s)"
+msgstr "La fonction de ce participant a été redéfinie pour ${number} point(s)"
+
 #. Default: "There was an error during annex conversion, please contact system administrator."
 msgid "There was an error during annex conversion, please contact system administrator."
 msgstr "Une erreur est survenue pendant la conversion de l'annexe.  Contactez votre administrateur système."
 
 #. Default: "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
 msgid "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
 msgstr "Une erreur est survenue en essayant de définir cette annexe comme 'à imprimer'.  Le message d'erreur est : ${error}.  Contactez votre administrateur système."
@@ -2138,18 +2008,14 @@
 msgid "This automatic advice has been asked by the application (shown by his title not being between brackets)"
 msgstr "Cet avis a été automatiquement demandé par l'application (montré par le fait que le titre n'est pas entre parenthèses)"
 
 #. Default: "This copy group was set automatically by the application"
 msgid "This copy group was set automatically by the application"
 msgstr "Ce groupe a été mis en copie automatiquement par l'application"
 
-#. Default: "This is an extract of the comment, access full comment if necessary..."
-msgid "This is an extract of the comment, access full comment if necessary..."
-msgstr "Ceci est un aperçu, consultez l'avis complet si nécessaire..."
-
 #. Default: "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 msgid "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 msgstr "Ce point n'est pas visible par les émetteurs d'avis de ce groupe dans son état actuel (${item_review_state})."
 
 #. Default: "This label can not be removed as it is used by some items, for example ${item_url}"
 msgid "This label can not be removed as it is used by some items, for example ${item_url}"
 msgstr "Cette étiquette ne peut pas être supprimée car elle est utilisées par certains points, par exemple ${item_url}"
@@ -2231,17 +2097,17 @@
 msgid "Votes are not completed for following ${number} ${polltype} item(s)"
 msgstr "Votes à scrutin ${polltype} non complétés pour ${number} point(s)"
 
 #. Default: "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 msgid "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 msgstr "Vous êtes sur le point de changer le délai de cet avis pour ${new_advice_delay} jours, vous pouvez entrer un commentaire si nécessaire."
 
-#. Default: "You cannot delete the default item template, but you can deactivate it if necessary!"
-msgid "You cannot delete the default item template, but you can deactivate it if necessary!"
-msgstr "Vous ne pouvez pas supprimer le modèle de point par défaut, mais vous pouvez le désactiver si nécessaire!"
+#. Default: "You cannot delete or move the default item template, but you can deactivate it if necessary!"
+msgid "You cannot delete or move the default item template, but you can deactivate it if necessary!"
+msgstr "Vous ne pouvez pas supprimer ou déplacer le modèle de point par défaut, mais vous pouvez le désactiver si nécessaire!"
 
 #. Default: "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 msgid "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 msgstr "Vous ne pouvez pas supprimer la fonction occupée \"${held_position_title}\" car elle est utilisée par l'élement \"${obj_url}\" !"
 
 #. Default: "Not grouped meeting configurations"
 msgid "_no_config_group_"
@@ -2471,78 +2337,78 @@
 msgid "annexAdded_mail_subject"
 msgstr "${meetingConfigTitle} - ${meetingTitle} - Une annexe vient d'être ajoutée à un point."
 
 #. Default: "If an annex is marked as \"Confidential\" by a meeting manager, following selected profiles will not be able to see it."
 msgid "annex_confidential_for_descr"
 msgstr "Si une annexe est marquée comme \"Confidentielle\" par un gestionnaire des séances, les profils sélectionnés ci-dessous ne pourront pas la voir."
 
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item."
-msgid "annex_is_confidential_no"
-msgstr "Cette annexe n'est pas confidentielle et sera visible par toute personne ayant accès au point."
-
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item.  Click on the image to set it as confidential."
-msgid "annex_is_confidential_no_edit"
-msgstr "Cette annexe n'est pas confidentielle et sera visible par toute personne ayant accès au point.  Cliquez sur l'image pour rendre l'annexe confidentielle."
-
-#. Default: "The annex is confidential."
-msgid "annex_is_confidential_yes"
-msgstr "Cette annexe est confidentielle."
-
-#. Default: "The annex is confidential.  Click on the image to set it as not confidential."
-msgid "annex_is_confidential_yes_edit"
-msgstr "Cette annexe est confidentielle.  Cliquez sur l'image pour rendre l'annexe non confidentielle."
-
 #. Default: "The item was duplicated but the annex with title \"${annexTitle}\" could not be kept because it was not possible to find a corresponding annex type in the destination meeting configuration, please contact system administrator."
 msgid "annex_not_kept_because_no_available_annex_type_warning"
 msgstr "Le point a été dupliqué mais l'annexe ayant le titre \"${annexTitle}\" n'a pas été gardée car aucun type d'annexe n'a pu être utilisé dans la configuration de séance de destination, contactez votre administrateur système."
 
 #. Default: "The item was duplicated but the annex with title \"${annexTitle}\" was not kept because using a scan_id, please contact system administrator."
 msgid "annex_not_kept_because_using_scan_id"
 msgstr "Le point a été dupliqué mais l'annexe ayant le titre \"${annexTitle}\" n'a pas été gardée car elle intègre un QR code qui doit rester unique, contactez votre administrateur système si nécessaire."
 
 #. Default: "Select for each optional annexes attributes which are only displayed or editable by MeetingManagers.  If an attribute is only displayed to MeetingManagers it will be automatically considered as only editable by MeetingManagers as well."
 msgid "annex_restrict_shown_and_editable_attributes_descr"
 msgstr "Sélectionnez ici pour les attributs activables sur les annexes, lesquels seront affichés ou éditables seulement par les gestionnaires de séances."
 
+#. Default: "Confidential"
+msgid "annex_term_confidential"
+msgstr "Confidentiel"
+
+#. Default: "Not confidential"
+msgid "annex_term_not_confidential"
+msgstr "Non confidentiel"
+
+#. Default: "Not publishable"
+msgid "annex_term_not_publishable"
+msgstr "Non publiable"
+
+#. Default: "Not to print"
+msgid "annex_term_not_to_print"
+msgstr "Pas à imprimer"
+
+#. Default: "Not to sign"
+msgid "annex_term_not_to_sign"
+msgstr "Pas à signer"
+
+#. Default: "Publishable"
+msgid "annex_term_publishable"
+msgstr "Publiable"
+
+#. Default: "Signed"
+msgid "annex_term_signed"
+msgstr "Signé"
+
+#. Default: "To print"
+msgid "annex_term_to_print"
+msgstr "À imprimer"
+
+#. Default: "To sign"
+msgid "annex_term_to_sign"
+msgstr "À signer"
+
 #. Default: "Title"
 msgid "annex_title"
 msgstr "Titre"
 
-#. Default: "The annex is not printable because it can not be converted (unsupported format or error during conversion).  Please use common office formats."
-msgid "annex_to_print_disabled"
-msgstr "L'annexe ne peut être convertie dans un format imprimable (format non pris en charge ou erreur lors de la conversion).  Utilisez des formats bureautiques courants tels que .doc, .xls, .odt, ..."
-
 #. Default: "Automated (annexes are printed by the application)"
 msgid "annex_to_print_mode_automated"
 msgstr "Automatisé (les annexes sont imprimées par l'application)"
 
 #. Default: "If print functionnality is enabled for annexes and an annex is set \"to print\", select here the to print mode that will be used : \"Manual\", means that the to print is just defined for information and that the printing process will be handled manually or \"Automated\", in this case, the application will generate a printable format for the annex (converted to images) so it can be inserted in a generated document."
 msgid "annex_to_print_mode_descr"
 msgstr "Si l'option \"à imprimer?\" est activée pour les annexes, ceci permet de définir le mode d'impression qui sera appliqué lorsqu'une annexe est définie \"à imprimer\" : soit le mode \"Pour information\", dans ce cas les annexes à imprimer le seront manuellement et l'application ne gère rien à ce niveau, soit \"Automatisé\", dans ce cas l'application génèrera un format imprimable pour les annexes (converties en images) afin qu'elles puissent être insérées lors de la génération de divers documents."
 
 #. Default: "For information (annexes are printed manually)"
 msgid "annex_to_print_mode_info"
 msgstr "Pour information (les annexes sont imprimées manuellement)"
 
-#. Default: "The annex will not be printed."
-msgid "annex_to_print_no"
-msgstr "L'annexe ne sera pas imprimée."
-
-#. Default: "The annex will not be printed. Click on the image to print it."
-msgid "annex_to_print_no_edit"
-msgstr "L'annexe ne sera pas imprimée. Cliquez sur l'image pour que l'annexe soit imprimée."
-
-#. Default: "The annex will be printed."
-msgid "annex_to_print_yes"
-msgstr "L'annexe sera imprimée."
-
-#. Default: "The annex will be printed. Click on the image not to print it."
-msgid "annex_to_print_yes_edit"
-msgstr "L'annexe sera imprimée. Cliquez sur l'image pour que l'annexe ne soit pas imprimée."
-
 #. Default: "Annex type"
 msgid "annex_type"
 msgstr "Type d'annexe"
 
 #. Default: "Every item may be associated with a series of annexes. Some annexes may be specifically tied to the decision taken on the item. You can consult and modify here the annex types that are defined within this meeting configuration. An annex type is defined by a title, an icon (preferably of 16x16 pixels) and a predefined title. When users want to associate an annex to an item, they may choose, in a dropdown list, an annex type among those defined here and upload a file."
 msgid "annex_types_descr"
 msgstr "À chaque point, avis et séances vous pouvez associer une série d'annexes. Vous pouvez consulter et modifier ici les types d'annexes définis pour cette configuration de séance. Un type d'annexe se définit par un titre, une icône (16x16 pixels de préférence) et un titre prédéfini. Lorsque des utilisateurs veulent associer une annexe à un point, ils peuvent choisir, dans une liste déroulante, un type d'annexe parmi ceux qui sont définis ici et uploader un fichier. Concernant les annexes aux points, certaines de ces annexes peuvent être spécifiquement liées à la décision découlant du point."
@@ -2567,37 +2433,29 @@
 msgid "annexes_preview_disabled"
 msgstr "<span style='color: red;'>La prévisualisation des annexes est désactivée dans les '${documentviewer_url}' (la case 'Convertir automatiquement' n'est pas cochée).</span>"
 
 #. Default: "<span style='color: green;'>Annexes preview is enabled in the ${documentviewer_url}.</span>"
 msgid "annexes_preview_enabled"
 msgstr "<span style='color: green;'>La prévisualisation des annexes est activée dans les '${documentviewer_url}' (la case 'Convertir automatiquement' est cochée).</span>"
 
-#. Default: "Signed annexes"
-msgid "annexes_signed_term"
-msgstr "Annexes signées"
-
-#. Default: "Annexes to print"
-msgid "annexes_to_print_term"
-msgstr "Annexes à imprimer"
-
-#. Default: "Annexes to sign"
-msgid "annexes_to_sign_term"
-msgstr "Annexes à signer"
+#. Default: "Annexes types are hidden by default, you can ${force_display} of it (may take some time)."
+msgid "annexes_types_force_display_descr"
+msgstr "Les types d'annexes sont cachés par défaut, vous pouvez cependant en ${force_display} (ceci peut prendre un certain temps en fonction du nombre de types d'annexes)."
 
 #. Default: "Application users"
 msgid "app_users"
 msgstr "Utilisateurs de l'application (créateurs, validateurs, ...)"
 
 #. Default: "Are you sure?"
 msgid "are_you_sure"
 msgstr "Êtes-vous sûr de vouloir effectuer cette action?"
 
 #. Default: "Specify here a TAL expression that will return a list of Plone group suffixes (for example : ['creators', 'reviewers', ]) if the group needs to be automatically selected as copyGroup for an item.  We receive \"item\" as the meeting item and \"isCreated\" that is only True when the item is in the creation process (not while being edited after).  WARNING, if the \"suffix\" returned by the expression is not in the list of selectable copy groups of the meeting config, it will not be selected.  The expression could look like : \"python: item.getProposingGroup() == 'samplegroup' and ['reviewers', ] or []\""
 msgid "as_copy_group_on_descr"
-msgstr "Spécifiez une expression TAL qui retourne une liste de suffixes de groupes Plone (par exemple ['creators', 'reviewers', ]) qui devront être automatiquement sélectionnés comme groupes en copie d'un point.  L'expression est évaluée à chaque modification du point (création et éditions suivantes).  L'élément \"item\" (point) est utilisable dans l'expression ainsi que \"isCreated\" qui est \"True\" uniquement lorsque le point est en création (\"False\" lors des éditions suivantes). ATTENTION: si le groupe Plone lié au suffixe n'est pas défini dans la liste des \"Groupes qui pourront être mis en copie\" sur la \"Configuration de séance\" du point, le groupe ne sera pas mis en copie et ce, quel que soit le résultat de l'expression.  Exemple d'expression : \"python: item.getProposingGroup() == 'samplegroup' and ['reviewers', ] or []\""
+msgstr "Spécifiez une expression TAL qui retourne une liste de suffixes de groupes Plone (par exemple ['creators', 'reviewers', ]) qui devront être automatiquement sélectionnés comme groupes en copie d'un point.  L'expression est évaluée à chaque modification du point (création et éditions suivantes).  L'élément \"item\" (point) est utilisable dans l'expression ainsi que \"isCreated\" qui est \"True\" uniquement lorsque le point est en création (\"False\" lors des éditions suivantes). ATTENTION, si le groupe Plone lié au suffixe n'est pas défini dans la liste des \"Groupes qui pourront être mis en copie\" sur la \"Configuration de séance\" du point, le groupe ne sera pas mis en copie et ce, quel que soit le résultat de l'expression.  Exemple d'expression : \"python: item.getProposingGroup() == 'samplegroup' and ['reviewers', ] or []\""
 
 #. Default: "As recurring item"
 msgid "as_recurring_item"
 msgstr "Comme point récurrent"
 
 #. Default: "The item is entitled \"${itemNumber} - ${itemTitle}\". You can access this item here: ${objectUrl}."
 msgid "askDiscussItem_mail_body"
@@ -2619,18 +2477,14 @@
 msgid "assemblyMember"
 msgstr "Membre d'assemblée"
 
 #. Default: "Absents as defined on the linked meeting"
 msgid "assembly_absents_defined_on_meeting"
 msgstr "Absents définis sur la séance"
 
-#. Default: "Define here people that were absents (not excused) for the meeting"
-msgid "assembly_absents_meeting_descr"
-msgstr "Définissez ici les membres absents (non excusés) pour la séance"
-
 #. Default: "Assembly and signatures"
 msgid "assembly_and_signatures"
 msgstr "Assemblée et signatures"
 
 #. Default: "Assembly as defined on the linked meeting"
 msgid "assembly_defined_on_meeting"
 msgstr "Assemblée définie sur la séance"
@@ -2639,33 +2493,25 @@
 msgid "assembly_descr"
 msgstr "Définissez ici l'assemblée par défaut, par exemple, une liste de noms et prénoms séparés par des virgules ou des retours à la ligne, qui sera automatiquement reprise sur chaque séance <span style='color:red;'>nouvellement créée, les changements apportés à ce champ n'impacte pas les séances déjà créées.</span> Ceci fonctionnera uniquement si vous utilisez l'attribut \"Assemblée (assembly)\" sur les séances."
 
 #. Default: "Excused as defined on the linked meeting"
 msgid "assembly_excused_defined_on_meeting"
 msgstr "Excusés définis sur la séance"
 
-#. Default: "Define here people that were excused for the meeting"
-msgid "assembly_excused_meeting_descr"
-msgstr "Définissez ici les personnes excusées pour la séance"
-
 #. Default: "Guests as defined on the linked meeting"
 msgid "assembly_guests_defined_on_meeting"
 msgstr "Invités définis sur la séance"
 
-#. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
-msgid "assembly_meeting_descr"
-msgstr "Ajoutez des double crochets [[ ]] autour des personnes absentes, par exemple : [[Mr. Untel Didier]] si vous n'utilisez pas les champs \"Excusés\" et \"Absents\""
-
 #. Default: "Using attribute(s) \"itemExcused\" and/or \"itemAbsents\" requires the use of attribute \"assembly\"."
 msgid "assembly_required"
 msgstr "L'usage de(s) l'(les) attribut(s) \"Excusés (itemExcused)\" et/ou \"Absents (itemAbsents)\" requiert celui de l'attribut \"Assemblée (assembly)\"."
 
 #. Default: "Define here the default assembly staves (for example you may type a list of names and first names separated by colons or new lines) that will be automatically selected on newly created meetings."
 msgid "assembly_staves_descr"
-msgstr "Définissez ici les assistants défaut, par exemple, une liste de noms et prénoms séparés par des virgules ou des retours à la ligne, qui sera automatiquement reprise sur chaque séance <span style='color:red;'>nouvellement créée, les changements apportés à ce champ n'impacte pas les séances déjà créées.</span> Ceci fonctionnera uniquement si vous utilisez l'attribut \"Assistants (assemblyStaves)\" sur les séances."
+msgstr "Définissez ici les assistants défaut, par exemple, une liste de noms et prénoms séparés par des virgules ou des retours à la ligne, qui sera automatiquement reprise sur chaque séance <span style='color:red;'>nouvellement créée, les changements apportés à ce champ n'impacte pas les séances déjà créées.</span> Ceci fonctionnera uniquement si vous utilisez l'attribut \"Assistants (assembly_staves)\" sur les séances."
 
 #. Default: " "
 msgid "associated_group_item_descr"
 msgstr " "
 
 # values of sortingMethodOnAddItem
 #. Default: "At the end"
@@ -2748,14 +2594,18 @@
 msgid "budgetimpacteditors"
 msgstr "Gestionnaires d'informations budgétaires"
 
 #. Default: "You can not access this item"
 msgid "can_not_access_this_item"
 msgstr "Vous ne pouvez pas accéder à ce point"
 
+#. Default: "Assembly and signatures : you can not use same signature number several times."
+msgid "can_not_define_several_same_signature_number"
+msgstr "Assemblée et signatures : vous ne pouvez pas utiliser le même numéro de signature plusieurs fois."
+
 #. Default: "You can not define two rows for the same meeting configuration!"
 msgid "can_not_define_two_rows_for_same_meeting_config"
 msgstr "Vous ne pouvez pas définir 2 lignes pour le même type de séance!"
 
 #. Default: "You can not remove/disable a function that is used by an item in the configuration.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_config_meetingitem"
 msgstr "Vous ne pouvez pas supprimer/désactiver une fonction qui est utilisée par un point d'une configuration.  Vérifiez ${item_url}."
@@ -2764,30 +2614,34 @@
 msgid "can_not_delete_plone_group_meetingconfig"
 msgstr "Vous ne pouvez pas supprimer/désactiver une fonction qui est utilisée par une configuration.  Vérifiez ${cfg_title}."
 
 #. Default: "You can not remove/disable a function that is used by an item in the application.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_meetingitem"
 msgstr "Vous ne pouvez pas supprimer/désactiver une fonction qui est utilisée par un point dans l'application.  Vérifiez ${item_url}."
 
-#. Default: "You can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
 msgid "can_not_remove_attendee_redefined_on_items"
-msgstr "Vous ne pouvez pas désélectionner un membre d'assemblée qui a été redéfini ou utilisé sur un point de la séance (absents, excusés, votes, ...).  Vérifiez \"${attendee_title}\"."
+msgstr "Assemblée et signatures : vous ne pouvez pas désélectionner un membre d'assemblée qui a été redéfini ou utilisé sur un point de la séance (absents, excusés, votes, ...).  Vérifiez \"${attendee_title}\"."
 
-#. Default: "You can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
 msgid "can_not_remove_public_voter_voted_on_items"
-msgstr "Vous ne pouvez pas désélectionner un votant qui a déjà voté sur un point à scrutin public.  Vérifiez \"${attendee_title}\"."
+msgstr "Assemblée et signatures : vous ne pouvez pas désélectionner un votant qui a déjà voté sur un point à scrutin public.  Vérifiez \"${attendee_title}\"."
 
-#. Default: "You can not unselect a voter that already voted on a secret vote item."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a secret vote item."
 msgid "can_not_remove_secret_voter_voted_on_items"
-msgstr "Vous ne pouvez pas désélectionner un votant qui a déjà voté sur un point à scrutin secret."
+msgstr "Assemblée et signatures : vous ne pouvez pas désélectionner un votant qui a déjà voté sur un point à scrutin secret."
 
 #. Default: "This item can no more be returned to the meeting managers because the meeting is in a state not authorizing it (${meetingState})."
 msgid "can_not_return_to_meeting_because_of_meeting_state"
 msgstr "Ce point ne peut plus être renvoyé vers les gestionnaires de séance car la séance dans laquelle ce point est présenté est dans un état qui ne l'autorise pas (${meetingState})."
 
+#. Default: "You can not select \"No committee\" and a committee."
+msgid "can_not_select_no_committee_and_committee"
+msgstr "Vous ne pouvez pas sélectionner \"Ne passe pas en commission\" et une commission."
+
 #. Default: "You can not select an adviser that is already displayed on the item as an inherited advice.  If you need to ask this advice again, you need to remove the inherited advice (as a MeetingManager or a Manager) then select advice again."
 msgid "can_not_select_optional_adviser_same_group_as_inherited"
 msgstr "Vous ne pouvez pas sélectionner un avis qui est déjà hérité sur le point. Si vous devez demander cet avis à nouveau, vous devez d'abord utiliser l'action \"Enlever l'avis hérité\" sur l'avis en tant que gestionnaire de séances ou administrateur de l'application."
 
 #. Default: "You can not select several values for the same group.  Please select a single value for the same group among available ones."
 msgid "can_not_select_several_optional_advisers_same_group"
 msgstr "Vous ne pouvez pas sélectionner plusieurs avis optionnels pour le même groupe.  Sélectionnez un type d'avis pour le même groupe parmi ceux disponibles."
@@ -2820,21 +2674,17 @@
 msgid "categories_descr"
 msgstr "Chaque point, au sein de cette configuration de séance, peut appartenir à une et une seule catégorie. Ces catégories sont définies ici (par un titre et une description). L'ordre dans lequel elles sont reprises dans ce répertoire est important. En effet, pour autant que vous le désiriez (un paramètre définit cela dans la section \"Données\"), lors de l'ajout d'un point à une séance, celui-ci peut s'insérer à la suite des points appartenant à la même catégorie, ceux-ci étant déjà insérés à l'endroit correspondant à la position de leur catégorie parmi la liste des catégories définies ici. Ceci dit, si vous spécifiez que vous voulez utiliser les groupes comme catégories (un autre paramètre de la section \"Données\"), les catégories définies ici ne seront pas utilisées."
 
 #. Default: "the \"Folder contents view\""
 msgid "categories_folder_contents_view"
 msgstr "la vue \"Contenus\""
 
-#. Default: "force display"
-msgid "categories_force_display"
-msgstr "forcer l'affichage"
-
 #. Default: "You can ${force_display} of every categories (may take some time)."
 msgid "categories_force_display_descr"
-msgstr "Vous pouvez ${force_display} des catégories (ceci peut prendre un certain temps)."
+msgstr "Vous pouvez ${force_display} des catégories (ceci peut prendre un certain temps en fonction du nombre de catégories)."
 
 #. Default: "You may use the ${folder_contents_link} to manage elements order."
 msgid "categories_use_folder_contents"
 msgstr "Vous pouvez utiliser ${folder_contents_link} pour gérer l'ordre des éléments."
 
 #. Default: "Choose here some identifier for your category."
 msgid "category_category_id_descr"
@@ -2980,14 +2830,34 @@
 msgid "clone_to"
 msgstr "Envoyer vers ${meetingConfigTitle}"
 
 #. Default: "Your configuration says can not correct this closed meeting, contact your system administrator if you want to change this."
 msgid "closed_meeting_not_correctable_by_config"
 msgstr "Vous ne pouvez pas corriger une séance clôturée, contactez votre administrateur système qui pourra le faire ou changer la configuration afin que vous puissiez le faire."
 
+#. Default: "${title} (${number}&nbsp;s.)"
+msgid "committee_title_with_abbr_suppl"
+msgstr "${title} (${number}&nbsp;s.)"
+
+#. Default: "${title} (${number}&nbsp;supplement)"
+msgid "committee_title_with_suppl"
+msgstr "${title} (${number}&nbsp;supplément)"
+
+#. Default: "Committees"
+msgid "committees"
+msgstr "Commissions"
+
+#. Default: "Define committees that will be useable on meetings and items (you also need to enable \"Committees\" on the meeting in the [Data] tab). This will show a \"Committees\" table on the meeting and will be also managed on the item. <br />There are 2 ways to manage committees on the item, either manually or automatically:<ul><li>Manually: just define committees, this will create a multiselection box on the item and users may select it.  It is possible to use the column \"Restrict to\" to define which proposing groups will be able to select the committee;</li><li>Automatically: use the column \"Auto from\" to define which committees to associate to the item depending on proposing group, category or classifier. A MeetingManager is nevertheless able to edit the committee on the item.</li></ul>. These 2 ways are mutually exclusive, if you select values in the \"auto_from\" columb here under, the \"Automatic\" mode will be used."
+msgid "committees_descr"
+msgstr "Définissez les commissions qui pourront être utilisées sur les séances et points (vous devez également activer le champ \"Commissions\" dans le champ \"Attributs utilisés pour caractériser une séance\" de l'onglet \"[Données]\").  Les commissions seront affichées sur la séance, et elles pourront être encodées sur les points.<br />Il y a 2 manières de gérer les commissions sur les points, soit <b>manuellement</b> ou <b>automatiquement</b> :<ul><li><b>Manuellement</b>: les commissions définies génèrent une liste à choix multiple sur le point.  Il est possible de restreindre ces choix via la colonne \"Restreindre à\" en sélectionnant les groupes proposant qui pourront sélectionner la commission;</li><li><b>Automatiquement</b>: aucun champ n'est affiché sur le point, les commissions seront automatiquement sélectionnées sur les points en fonction de ce qui est sélectionné dans la colonne \"Automatiquement pour\" (donc en fonction du groupe proposant, de la catégorie ou du classificateur sélectionné sur le point). Seul un gestionnaire de séances pourra éditer cette valeur sur les points.</li></ul>Ces 2 modes de fonctionnement sont incompatibles, le mode \"Automatique\" sera activé si vous renseignez des valeurs dans la colonne \"Automatiquement si\"."
+
+#. Default: "Using a \"Committees\" field requires the use of attribute \"Committees (committees)\"."
+msgid "committees_required"
+msgstr "L'usage d'un attribut lié aux \"Commissions\" requiert l'activation du champ \"Commissions (committees)\"."
+
 #. Default: "Complete"
 msgid "completeness_complete"
 msgstr "Le point est complet"
 
 #. Default: "Evaluation asked again"
 msgid "completeness_evaluation_asked_again"
 msgstr "Évaluation demandée à nouveau"
@@ -3062,24 +2932,31 @@
 
 #. Default: "The decision annexes"
 msgid "content_kept_decision_annexes"
 msgstr "Les annexes (après décision)"
 
 #. Default: "Select here contents of original item that will be kept when sending an item to another meeting configuration.  If you select \"The advices\", advices will be inherited from original item, this mean that advices from original item will be displayed readonly on the new item but actually, informations are taken from original item.  You can also select advices to keep in \"Advices to keep when item is sent to another configuration\" field below."
 msgid "contents_kept_on_sent_to_other_mc_descr"
-msgstr "Sélectionnez ici les éléments à garder lors de l'envoi d'un point vers un autre type de séance.  Si vous sélectionnez de garder \"Les avis\", ils seront \"hérités\" du point original, ceci signifie que les avis seront affichés en lecture seule sur le nouveau point, mais les informations seront reprises du point original.  Vous pouvez sélectionner les avis à garder ci-dessous dans le champ \"Avis à garder lors de l'envoi d'un point vers une autre configuration de séance\"."
+msgstr "Sélectionnez ici les éléments à garder lors de l'envoi d'un point vers un autre type de séance.  Si vous sélectionnez de garder \"Les avis\", ils seront \"hérités\" du point original, cela signifie que les avis seront affichés en lecture seule sur le nouveau point, mais les informations seront reprises du point original.  Vous pouvez sélectionner les avis à garder ci-dessous dans le champ \"Avis à garder lors de l'envoi d'un point vers une autre configuration de séance\"."
 
 #. Default: "The item is entitled \"${itemTitle}\". You can access this item here: ${objectUrl}."
 msgid "copyGroups_mail_body"
 msgstr "L'objet du point est \"${itemTitle}\". Accédez au point ici: ${objectUrl}."
 
 #. Default: "${meetingConfigTitle} - You have been carbon copied - ${itemTitle}"
 msgid "copyGroups_mail_subject"
 msgstr "${meetingConfigTitle} - Vous avez été mis en copie - ${itemTitle}"
 
+#. Default: "These groups will have read access to the item in following states: ${states}.\nWhen icon is green, this means that copy groups have access to the item.\nWhen the label \"[auto]\" is displayed next to the group title, it means that the group was set as copy group automatically by the application."
+msgid "copy_groups_help_msg"
+msgstr ""
+"Les groupes en copie auront accès en lecture seule au point dans les états suivants: ${states}.\n"
+"L'icône \"?\" apparaît en vert lorsque les groupes en copie ont accès au point.\n"
+"Si le libellé \"[auto]\"est affiché à la suite du titre du groupe en copie, cela signifie qu'il a été mis en copie automatiquement par l'application."
+
 #. Default: " "
 msgid "copy_groups_item_descr"
 msgstr " "
 
 #. Default: "The cloned item could not be presented to a meeting in the \"${destMeetingConfigTitle}\" configuration, no suitable meeting could be found."
 msgid "could_not_present_item_no_meeting_accepting_items"
 msgstr "Le point envoyé au \"${destMeetingConfigTitle}\" n'a pas pu être présenté dans une séance car aucune séance appropriée n'a pu être trouvée."
@@ -3266,14 +3143,34 @@
 msgid "delay_of_x_days"
 msgstr "Délai de ${delay} jour(s)"
 
 #. Default: "Select here the days a computed delay can not ends with.  If a computed delay is ending on one of selected week day, the delay will be extend to next available day.  <span style='color: red;'>If you change this parameter, do not forget to run \"Update items and meetings\"!</span>"
 msgid "delay_unavailable_end_days_descr"
 msgstr "Sélectionnez les jours indisponibles comme dernier jour d'un délai.  Si un délai calculé tombe sur un des jours sélectionnés, le délai sera automatiquement prolongé au prochain jour disponible.  <span style='color: red;'>Si vous modifiez ce paramètre, n'oubliez pas d'exécuter \"Mettre à jour les points et séances\"!</span>"
 
+#. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
+msgid "descr_assembly"
+msgstr "Ajoutez des double crochets [[ ]] autour des personnes absentes, par exemple : [[Mr. Untel Didier]] si vous n'utilisez pas les champs \"Excusés\" et \"Absents\""
+
+#. Default: "<span style='color: red;'>WARNING, this field is managed by the application and it's value will be \"-1\" until the meeting is frozen, then it will be computed automatically. Do only change it manually when necessary (in general this should never happen). This field is only editable and viewable by meeting managers</span>"
+msgid "descr_config_field_reserved_to_meeting_managers"
+msgstr "<span style='color: red;'>ATTENTION, ce champ est géré par l'application et sa valeur sera \"-1\" tant que la séance n'aura pas été gelée. Ne changez cette valeur que si un décallage survient et prévenez votre administrateur système. Ce champ n'est visible et éditable que par les gestionnaires de séances</span>"
+
+#. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
+msgid "descr_field_reserved_to_meeting_managers"
+msgstr "<span style='color: red;'>Ce champ n'est visible et éditable que par les gestionnaires de séances</span>"
+
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
+msgid "descr_field_vieawable_by_everyone"
+msgstr "<span style='color: green;'>Ce champ n'est éditable que par les gestionnaires de séances mais visible de tous</span>"
+
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
+msgid "descr_field_vieawable_by_everyone_once_meeting_decided"
+msgstr "<span style='color: green;'>Ce champ n'est éditable que par les gestionnaires de séances, consultable par les super observateurs ayant accès à la séance et <strong>consultable par tout le monde seulement lorsque la séance est décidée</strong></span>"
+
 #. Default: "You are just able to see visible elements here. Please consult the \"manage\" box here opposite."
 msgid "description_only_see_visible_items"
 msgstr "Vous êtes seulement autorisé à consulter les éléments visibles.  Utilisez la boîte \"Gestion\" ci-contre pour consulter le contenu que vous pouvez voir."
 
 #. Default: "By default only MeetingManagers will see the available items panel on a meeting as long as the meeting is accepting items.  This let's you show this panel to selected profiles.  Note that if you enable this, the meeting view will be displayed slower."
 msgid "display_available_items_to_descr"
 msgstr "Par défaut, seuls les gestionnaires de séances voient les points disponibles sur une séance, tant que la séance n'est pas clôturée. <span style='color: red;'>Notez qu'activer ceci rend l'affichage d'une séance plus lent pour les profils sélectionnés.</span>"
@@ -3370,14 +3267,22 @@
 msgid "enable_scan_docs_descr"
 msgstr "Cochez la case si vous utilisez la fonctionnalité de scanning de documents."
 
 #. Default: "If you check this box, users will be able to access a screen for modifying their preferences. While powerful, some may think it exposes too much complexity to users."
 msgid "enable_user_preferences_descr"
 msgstr "Si vous cochez cette case, les utilisateurs pourront accéder à un écran permettant de modifier leurs préférences. Bien que puissant, cet écran peut être perçu comme confrontant l'utilisateur à une trop grande complexité."
 
+#. Default: "Select the batch actions that will be displayed on the table listing annexes"
+msgid "enabled_annexes_batch_actions_descr"
+msgstr "Sélectionnez les actions par lot qui apparaîtront dans l'onglet \"Annexes\" et qui pourront être appliquées sur les annexes sélectionnées."
+
+#. Default: "The meeting end date must occur after the start date and meeting date."
+msgid "end_date_before_meeting_date"
+msgstr "La date de fin ne peut pas être avant la date de début ou la date de la séance."
+
 #. Default: "When advice mandatoriness is enforced, an item can't be inserted into a meeting unless all mandatory advices are given and positive."
 msgid "enforce_advice_mandatoriness_descr"
 msgstr "Quand le caractère obligatoire des avis est d'application, un point ne peut être inséré dans une séance à moins que tous les avis obligatoires n'aient été rendus et soient positifs."
 
 #. Default: "You can not encode more than ${max_voters} voters."
 msgid "error_can_not_encode_more_than_max_voters"
 msgstr "Vous ne pouvez pas encoder plus de ${max_voters} votes."
@@ -3398,14 +3303,30 @@
 msgid "error_certified_signatures_invalid_dates"
 msgstr "Veuillez vérifier les dates encodées à la ligne ${row_number}.  Utilisez le format \"AAAA/MM/JJ\", vérifiez que les dates encodées sont valides et que la date de début est bien inférieure ou égale à la date de fin."
 
 #. Default: "Signatures must be ordered by signature number, please check and order signature using the arrows on the right of the table."
 msgid "error_certified_signatures_order"
 msgstr "Les signatures doivent être ordonnées par numéro de signature, vérifiez les numéros de signatures et utilisez les flèches à la droite du tableau pour les ordonner correctement."
 
+#. Default: "You can not remove a configuration that was already used, removed configuration \"${committee_label}\" is used for example by item at ${url}.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committee_row_id_removed_already_used"
+msgstr "Vous ne pouvez pas supprimer une configuration qui a déjà été utilisée.  La configuration \"${committee_label}\" est utilisée par exemple par le point ${url}.  Si vous avez perdu les valeurs encodées, annulez l'édition et éditez à nouveau."
+
+#. Default: "You can not define values for the \"auto_from\" and \"using_groups\" columns, their use is multually exclusive.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committees_mutually_exclusive_auto_from_and_using_groups"
+msgstr "Vous ne pouvez définir de valeurs pour les colonnes \"Restreindre à\" et \"Défini automatiquement si\", ces 2 colonnes sont mutuellement exclusives.  Si vous avez perdu les valeurs encodées, annulez l'édition et éditez à nouveau."
+
+#. Default: "Default poll type must be among used poll types"
+msgid "error_default_poll_type_must_be_among_used_poll_types"
+msgstr "Vous ne pouvez utiliser que des valeurs sélectionnées dans le champ \"Modes de scrutin utilisés\"."
+
+#. Default: "First linked vote used votes values must be among used vote values"
+msgid "error_first_linked_vote_used_vote_values_must_be_among_used_vote_values"
+msgstr "Vous ne pouvez utiliser que des valeurs sélectionnées dans le champ \"Valeurs de votes utilisées\"."
+
 #. Default: "You may not remove a list type that is currently used by an item, check for example : ${url}."
 msgid "error_list_types_identifier_removed_already_used"
 msgstr "Vous ne pouvez pas supprimer un type de point qui est déjà utilisé (le type de point supprimé est utilisé par : ${url})."
 
 #. Default: "You may not remove the default list types (\"normal\" and \"late\")."
 msgid "error_list_types_missing_default"
 msgstr "Vous ne pouvez pas supprimer un des types de point par défaut (\"normal\" et \"late\")."
@@ -3414,14 +3335,22 @@
 msgid "error_list_types_same_identifier"
 msgstr "Vous ne pouvez pas utiliser le même identifiant plusieurs fois."
 
 #. Default: "You may only use lowercase letters for identifier."
 msgid "error_list_types_wrong_identifier_format"
 msgstr "Vous ne pouvez utiliser que des lettres minuscules pour l'identifiant."
 
+#. Default: "Next linked votes used vote values must be among used vote values"
+msgid "error_next_linked_votes_used_vote_values_must_be_among_used_vote_values"
+msgstr "Vous ne pouvez utiliser que des valeurs sélectionnées dans le champ \"Valeurs de votes utilisées\"."
+
+#. Default: "Some selected values are no more selectable (no more selected in the \"Ordered committees contacts\" field), please check value \"${hp_title}\".  You can not select \"No committee\" and a committee.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_value_removed_used_in_committees_field"
+msgstr "Vous ne pouvez utiliser que des valeurs sélectionnées dans le champ \"Membres d'assemblée des commissions sélectionnables\", vérifiez la valeur \"${hp_title}\". Si vous avez perdu les valeurs encodées, annulez l'édition et éditez à nouveau."
+
 #. Default: "An advice was added or updated on an item (notify the \"Creators\")"
 msgid "event_add_advice"
 msgstr "Un avis sur un point a été rendu ou modifié (prévient les créateurs du groupe proposant du point)"
 
 #. Default: "An advice was added or updated on an item (notify the \"Owner\")"
 msgid "event_add_advice_owner"
 msgstr "Un avis sur un point a été rendu ou modifié (prévient l'auteur du point)"
@@ -3530,53 +3459,57 @@
 msgid "fastedit_save_changes"
 msgstr "Enregistrer les changements"
 
 #. Default: "Please fill this field."
 msgid "field_required"
 msgstr "Veuillez remplir ce champ."
 
-#. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
-msgid "field_reserved_to_meeting_managers_descr"
-msgstr "<span style='color: red;'>Ce champ n'est visible et éditable que par les gestionnaires de séances</span>"
-
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
-msgid "field_vieawable_by_everyone_descr"
-msgstr "<span style='color: green;'>Ce champ n'est éditable que par les gestionnaires de séances mais visible de tous</span>"
-
 #. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once item is decided</span>"
 msgid "field_vieawable_by_everyone_once_item_decided_descr"
 msgstr "<span style='color: green;'>Ce champ n'est éditable que par les gestionnaires de séances, consultable par les super observateurs ayant accès au point et <strong>consultable par tout le monde seulement lorsque le point est décidé</strong></span>"
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
-msgid "field_vieawable_by_everyone_once_meeting_decided_descr"
-msgstr "<span style='color: green;'>Ce champ n'est éditable que par les gestionnaires de séances, consultable par les super observateurs ayant accès à la séance et <strong>consultable par tout le monde seulement lorsque la séance est décidée</strong></span>"
+#. Default: "Assembly and signatures"
+msgid "fieldset_assembly"
+msgstr "Assemblée et signatures"
+
+#. Default: "Committees"
+msgid "fieldset_committees"
+msgstr "Commissions"
+
+#. Default: "Dates and data"
+msgid "fieldset_dates_and_data"
+msgstr "Dates et données"
+
+#. Default: "Informations"
+msgid "fieldset_informations"
+msgstr "Informations"
+
+#. Default: "Parameters"
+msgid "fieldset_parameters"
+msgstr "Paramètres avancés"
 
 #. Default: "Please choose a file by clicking on the \"Browse\" button."
 msgid "file_required"
 msgstr "Veuillez sélectionner un fichier en cliquant sur le bouton \"Parcourir\"."
 
 #. Default: "While using linked vote values, select here values that will be selectable for the first linked vote value"
 msgid "first_linked_vote_used_vote_values_descr"
-msgstr "Lorsque vous liez des votre entre eux, sélectionnez les valeurs de votes qui pourront être utilisée sur le premier vote lié"
+msgstr "Lorsque vous liez des votre entre eux, sélectionnez les valeurs de votes qui pourront être utilisées sur le premier vote lié"
 
 #. Default: "Please respect order of transitions sequence to present an item, the first given transition is not a transition leaving the item workflow initial state."
 msgid "first_transition_must_leave_wf_initial_state"
 msgstr "Respectez bien l'ordre des transitions menant à l'état 'présenté', la première transition renseignée n'est pas une transition qui part de l'état initial du workflow du point."
 
 #. Default: "In the application folder of every member, a sub-folder is created for each meeting configuration. The name of this sub-folder is defined here."
 msgid "folder_title_descr"
 msgstr "Dans le répertoire de chaque utilisateur, un sous-répertoire par configuration de séance est créé. Le nom de ce sous-répertoire se définit ici."
 
-#. Default: "For the administrator only"
-msgid "for_admin_only"
-msgstr "Éditable par les administrateurs de l'application uniquement"
-
-#. Default: "Specify here the deadline for validating late items to be inserted in a given meeting.  Leave the field empty not to use this functionality."
-msgid "freeze_deadline_default_descr"
-msgstr "Spécifiez ici l'échéance pour valider des points à insérer en urgence dans une séance donnée.  Laissez le champ vide si vous ne souhaitez pas utiliser cette fonctionnalité."
+#. Default: "force display"
+msgid "force_display"
+msgstr "forcer l'affichage"
 
 #. Default: "<p>PloneMeeting body in HTML format.</p>"
 msgid "front_page_body"
 msgstr "<p>Avant de tester, nous vous recommandons de lire la <span class=\"link-external\"><a target=\"_blank\" href=\"http://www.imio.be/support/documentation/manual/plonemeeting41\">documentation</a></span> qui explique en détails le fonctionnement du logiciel. Ce manuel évolue constamment.</p>"
 
 #. Default: "Manage here your official meetings."
 msgid "front_page_description"
@@ -3676,14 +3609,18 @@
 msgstr "Sous-types d'annexes"
 
 # Other
 #. Default: "Check/uncheck items"
 msgid "helpSelectItemsIcon"
 msgstr "Cocher/décocher les points"
 
+#. Default: "This is the date the advice was originally given, this will change when the advice will be considered \"Given\" in a state where it is no more editable"
+msgid "help_given_on_before_started_on"
+msgstr "Lorsqu'un avis est \"Demandé à nouveau\" la date affichée sous \"Rendu le\" est la date de remise de l'avis original.  Cette date sera adaptée lorsqu'un nouvel avis aura été rendu"
+
 #. Default: "No preview available because this type of file can not be converted.  Please use common office formats.  You can download the file, look in the \"actions\" column."
 msgid "help_no_preview_available"
 msgstr "Aucune prévisualisation pour cette annexe car ce type de fichier ne peut être converti correctement.  Utilisez un format bureautique courant (.doc, .xls, .odt, ...).  Vous pouvez cependant télécharger cette annexe en utilisant l'action \"Télécharger\" dans la colonne \"Actions\"."
 
 #. Default: "No preview available because there was an error during conversion to a previewable format.  Please contact system administrator that will have access to more debugging informations."
 msgid "help_no_preview_available_conversion_error"
 msgstr "Aucune prévisualisation pour cette annexe car une erreur est survenue pendant la conversion.  Contactez votre administrateur système qui aura accès à davantage d'informations concernant cette erreur."
@@ -3724,18 +3661,14 @@
 msgid "historize_item_data_when_advice_is_given_descr"
 msgstr "Lorsqu'un avis est officiellement rendu, c'est-à-dire lorsqu'il quitte l'état dans lequel les émetteurs d'avis peuvent encoder cet avis, ce dernier est historisé.  Si vous cochez cette case, les informations essentielles du point (titre et champs de rexte riche) seront également historisées avec l'avis."
 
 #. Default: "For every field you select here, the application will keep track of any change on any item, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
 msgid "historized_item_attrs_descr"
 msgstr "Pour chaque champ que vous sélectionnez ici, l'application conservera la trace de tout changement sur chaque point qui est dans un des états listés ci-dessous.  <span style='color: red;'>Cette fonctionnalité est toujours dans un status \"BETA\", vous pourriez rencontrer un comportement étrange lors de l'utilisation.  Cette fonctionnalité sera complètement retravaillée dans une prochaine version.</span>"
 
-#. Default: "For every field you select here, the application will keep track of any change on any meeting, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
-msgid "historized_meeting_attrs_descr"
-msgstr "Pour chaque champ que vous sélectionnez ici, l'application conservera la trace de tout changement sur chaque séance qui est dans un des états listés ci-dessous.  <span style='color: red;'>Cette fonctionnalité est toujours dans un status \"BETA\", vous pourriez rencontrer un comportement étrange lors de l'utilisation.  Cette fonctionnalité sera complètement retravaillée dans une prochaine version.</span>"
-
 #. Default: "See changes"
 msgid "history_changes"
 msgstr "Voir les changements"
 
 #. Default: "Deleted by ${userName}"
 msgid "history_delete"
 msgstr "Supprimé par ${userName}"
@@ -3752,17 +3685,17 @@
 msgid "holidays_date_not_ascending_error"
 msgstr "Les dates doivent être définies de manière ascendante, de la plus ancienne à la plus récente."
 
 #. Default: "These dates will be used to compute advices delays.  <span style='color: red;'>If you change this parameter and modified dates are interacting with some existing advice delays, do not forget to run \"Update items and meetings\"!</span>"
 msgid "holidays_descr"
 msgstr "Ces dates seront utilisées lors du calcul des délais des avis.  <span style='color: red;'>Si vous modifiez ce paramètre et que les dates modifiées peuvent changer le délai d'un avis existant, n'oubliez pas d'exécuter \"Mettre à jour les points et séances\"!</span>"
 
-#. Default: "You removed a date that is currently in use!"
+#. Default: "You removed a date that is currently in use! Check item at ${item_url}"
 msgid "holidays_removed_date_in_use_error"
-msgstr "Vous ne pouvez pas supprimer une date qui est/a été utilisée!"
+msgstr "Vous ne pouvez pas supprimer une date qui est/a été utilisée! Vérifiez par exemple ${item_url}"
 
 #. Default: "There are not enough holidays defined in the configuration.  These days are used for advice delay computation.  This warning appear when last holiday defined in the configuration is in less than 60 days. Contact you system administrator if necessary."
 msgid "holidays_warning_message"
 msgstr "Il n'y a plus suffisamment de jours fériés définis dans la configuration. Ces jours sont utilisés dans le calcul du délai des avis.  Ce message apparaît lorsque le dernier jour défini dans la configuration est dans moins de 60 jours.  Contactez votre administrateur système si nécessaire."
 
 #. Default: "Wrong date format, please use following format : \"YYYY/MM/DD\"."
 msgid "holidays_wrong_date_format_error"
@@ -3780,14 +3713,18 @@
 msgid "hs_name"
 msgstr "Nom"
 
 #. Default: "This application allows you to manage your official meetings."
 msgid "hs_welcome_body"
 msgstr "Cette application vous permet de gérer vos séances délibératoires."
 
+#. Default: "iA.Delib documentation"
+msgid "iA.Delib documentation"
+msgstr "Documentation iA.Délib"
+
 #. Default: "Azur"
 msgid "icon_color_azur"
 msgstr "Azur"
 
 #. Default: "Black"
 msgid "icon_color_black"
 msgstr "Noire"
@@ -3922,19 +3859,19 @@
 
 #. Default: "To use this functionnality, it is necessary that the icon \"${iconname}\" that will trigger the action exists.  Please creates it before continuing..."
 msgid "iconname_does_not_exist"
 msgstr "Pour utiliser cette fonctionnalité, il est nécessaire que l'icône \"${iconname}\" qui sera utilisée pour déclencher l'action existe.  Veuillez la créer."
 
 #. Default: "If checked, the groups in charge selected on the category of the item will be taken into account."
 msgid "include_groups_in_charge_defined_on_category_descr"
-msgstr "Les groupes en charge définis sur la catégorie du point seront pris en compte par l'application (ordre des points sur séance par groupe en charge, accès aux points par les groupes en charge, accès aux annexes confidentielles, ...)"
+msgstr "Les groupes en charge définis sur la catégorie et/ou le classificateur seront stockés sur le point."
 
 #. Default: "If checked, the groups in charge selected on the proposing group of the item will be taken into account."
 msgid "include_groups_in_charge_defined_on_proposing_group_descr"
-msgstr "Les groupes en charge définis sur le groupe proposant du point seront pris en compte par l'application (ordre des points sur séance par groupe en charge, accès aux points par les groupes en charge, accès aux annexes confidentielles, ...)"
+msgstr "Les groupes en charge définis sur le groupe proposant seront stockés sur le point."
 
 #. Default: "By default, only MeetingManagers may remove an inherited advice as long as item is editable.  If checked, this will give the advisers the possibility to remove an advice of their adviser groups when the item is in a state defined in the \"Item states allowing to modify or delete advices\" field here above."
 msgid "inherited_advice_removeable_by_adviser_descr"
 msgstr "Par défaut, seuls les gestionnaires de séances peuvent enlever un avis hérité tant que le point est éditable.  Si la case est cochée, les émetteurs d'avis auront la possibilité de supprimer un avis hérité rendu par leur groupe tant que le point est dans un des états définis dans le champ \"États des points dans lesquels on peut modifier ou supprimer un avis donné\" ci-dessus."
 
 #. Default: "You can not select another inserting method together with the \"At the end\" inserting method."
 msgid "inserting_methods_at_the_end_not_alone_error"
@@ -4394,38 +4331,26 @@
 msgstr "L'objet du point est \"${itemTitle}\". Accédez au point ici: ${objectUrl}."
 
 # Mails (item-related)
 #. Default: "${meetingConfigTitle} - A \"late\" item has been validated."
 msgid "lateItem_mail_subject"
 msgstr "${meetingConfigTitle} - Un point en urgence vient d'être validé."
 
-#. Default: "Items presented tardily"
-msgid "late_presented_items"
-msgstr "Points présentés en urgence"
-
 #. Default: "--- Do nothing, let the item in the workflow initial state ---"
 msgid "let_item_in_initial_state"
 msgstr "--- Ne rien faire, laisser le point dans son état initial ---"
 
 #. Default: "Linked items (${auto_linked_items})"
 msgid "linked_items"
 msgstr "Points liés (${auto_linked_items})"
 
 #. Default: "Linked items, ${auto_linked_items} automatically and ${manually_linked_items} manually"
 msgid "linked_items_with_manually_linked_items"
 msgstr "Points liés, ${auto_linked_items} automatiquement et ${manually_linked_items} manuellement"
 
-#. Default: "Late"
-msgid "list_type_late"
-msgstr "En retard"
-
-#. Default: "Normal"
-msgid "list_type_normal"
-msgstr "Normal"
-
 #. Default: "Types of list of items that will be available when an item is linked to a meeting."
 msgid "list_types_descr"
 msgstr "Types de liste de points qui seront disponibles lorsqu'un point est dans une séance."
 
 #. Default: "Size"
 msgid "listingheader_size"
 msgstr "Taille"
@@ -4508,51 +4433,31 @@
 
 #. Default: "Update all items and meetings of this meeting configuration"
 msgid "mc_update_all_local_roles"
 msgstr "Mettre à jour les points et séances de cette configuration de séance"
 
 #. Default: "Warning: this will update every items and meetings of this configuration, it is only relevant if the field of the configuration that you changed specifies that you need to use this action.  If you only made little changes like adding or removing a state in a field, as an administrator, it is possible to update items and meetings from the dashboards.  To do this, select elements that need to be updated and use the \"Update\" batch action."
 msgid "mc_update_all_local_roles_warning"
-msgstr "Attention: ceci va mettre à jour tous les points et séances et n'est utile que si vous avez changé un paramètre dans cette configuration de séance pour lequel il est spécifié dans la description du champ qu'il faudra mettre à jour les points et séances.  S'il s'agit de petits changements, comme l'ajout ou suppression d'un état dans un champ, il est possible, en tant qu'administrateur, de ne mettre à jour que les points et séances impactées depuis les tableaux de bord.  Pour ce faire, filtrez les points ou séances pour obtenir les éléments à mettre à jour et utilisez l'action par lot \"Mettre à jour\"."
+msgstr "Attention, ceci va mettre à jour tous les points et séances et n'est utile que si vous avez changé un paramètre dans cette configuration de séance pour lequel il est spécifié dans la description du champ qu'il faudra mettre à jour les points et séances.  S'il s'agit de petits changements, comme l'ajout ou suppression d'un état dans un champ, il est possible, en tant qu'administrateur, de ne mettre à jour que les points et séances impactées depuis les tableaux de bord.  Pour ce faire, filtrez les points ou séances pour obtenir les éléments à mettre à jour et utilisez l'action par lot \"Mettre à jour\"."
 
 #. Default: "Similarly to the preceding field, all the actions that are triggered when a meeting goes from one state to another are configurable through the development of another Plone product into which you must:<ul><li>create a Python interface that inherits from interface Products.PloneMeeting.interfaces.IMeetingWorkflowActions (you must enter the full package name of this interface in the field below);</li><li>create and declare in ZCML an adapter that adapts the interface  Products.PloneMeeting.interfaces.IMeeting to the interface you have defined in the previous step.</li></ul>Your adapter may inherit from the default adapter Products.PloneMeeting.Meeting.MeetingWorkflowActions: it will allow you to override only methods for which you want an altered behaviour. All the methods proposed by the interface Products.PloneMeeting.interfaces.IMeetingWorkflowActions are documented."
 msgid "meeting_actions_interface_descr"
 msgstr "À l'instar du champ précédent, toutes les actions qui sont déclenchées lorsqu'une séance passe d'un état à un autre sont configurables via le développement d'un produit Plone tiers dans lequel vous devez:<ul><li>créer une interface Python qui hérite de l'interface Products.PloneMeeting.interfaces.IMeetingWorkflowActions (c'est le nom complet de cette interface que vous devez spécifier dans ce champ);</li><li>créer et déclarer en ZCML un adapter qui adapte l'interface Products.PloneMeeting.interfaces.IMeeting vers l'interface que vous avez définie au point précédent.</li></ul>Vous pouvez faire hériter votre adapter de l'adapter par défaut Products.PloneMeeting.Meeting.MeetingWorkflowActions: cela vous permettra de remplacer ou overrider uniquement les méthodes pour lesquelles vous voulez un comportement différent. Toutes les méthodes proposées par l'interface Products.PloneMeeting.interfaces.IMeetingWorkflowActions sont documentées."
 
 #. Default: "Select here profiles of users that will be able to see an annex added to a meeting that is set confidential.  <span style='color: red;'>If you change this and there are existing confidential annexes, please run the action \"Update categorized elements\" in the \"Meeting annnex types\" configuration.</span>"
 msgid "meeting_annex_confidential_visible_for_descr"
 msgstr "Sélectionnez ici les profils d'utilisateurs qui pourront voir les annexes ajoutées à des séances et définies comme confidentielles.  <span style='color: red;'>Si vous changez ces valeurs et que des annexes confidentielles existent, exécutez l'action \"Mise à jour des éléments catégorisés\" dans la configuration des \"Annexes aux séances\".</span>"
 
 #. Default: "Choose here which page will be shown after logon."
 msgid "meeting_app_default_view_descr"
 msgstr "Choisissez ici la page qui s'affiche directement après connexion."
 
-#. Default: "Assembly"
-msgid "meeting_assembly"
-msgstr "Assemblée"
-
-#. Default: "Absents"
-msgid "meeting_assemblyAbsents"
-msgstr "Absents"
-
-#. Default: "Excused"
-msgid "meeting_assemblyExcused"
-msgstr "Excusés"
-
-#. Default: "Guests"
-msgid "meeting_assemblyGuests"
-msgstr "Invités"
-
-#. Default: "Proxies"
-msgid "meeting_assemblyProxies"
-msgstr "Procurations"
-
-#. Default: "Staves"
-msgid "meeting_assemblyStaves"
-msgstr "Assistants"
+#. Default: "Meeting assembly (${number_of_attendees}) and signatories (${number_of_signatories})"
+msgid "meeting_attendees_and_signatories"
+msgstr "Assemblée (${number_of_attendees}) et signataires (${number_of_signatories})"
 
 #. Default: "Choose here which columns to display when listing meetings (ie, when displaying the list of available meetings or decisions, or when performing custom searches)."
 msgid "meeting_columns_descr"
 msgstr "Choisissez ici les colonnes à afficher sur les listes de séances (par exemple, sur la liste des séances disponibles ou passées, ou encore sur des résultats de recherches avancées)."
 
 #. Default: "Similarly to interfaces defined for items, the conditions expressed on the transitions of the meeting workflow may be configured through the development of another Plone product into which you must:<ul><li>create a Python interface that inherits from interface Products.PloneMeeting.interfaces.IMeetingWorkflowConditions (you must enter the full package name of this interface in the field below);</li><li>create and declare in ZCML an adapter that adapts the interface  Products.PloneMeeting.interfaces.IMeeting to the interface you have defined in the previous step.</li></ul>Your adapter may inherit from the default adapter Products.PloneMeeting.Meeting.MeetingWorkflowConditions: it will allow you to override only methods for which you want an altered behaviour. All the methods proposed by the interface Products.PloneMeeting.interfaces.IMeetingWorkflowConditions are documented."
 msgid "meeting_conditions_interface_descr"
@@ -4594,25 +4499,17 @@
 msgid "meeting_organizations"
 msgstr "Organisations"
 
 #. Default: "When an item is inserted in a meeting from everywhere (so not when on a meeting view), this will take the very next meeting still accepting items.  Define here states to take into account to get this very next meeting."
 msgid "meeting_present_item_when_no_current_meeting_states_descr"
 msgstr "Lorsqu'un gestionnaire de séance souhaite présenter un point dans une séance sans être sur la vue de la séance, donc par exemple lorsqu'il est sur la vue d'un point, via l'action 'Présenter', ou lorsqu'il est dans les tableaux de bords, le point sera présenté automatiquement dans la prochaine séance (dont la date est dans le futur) dans laquelle des points peuvent toujours être présentés et dont l'état est un des états sélectionnés ici."
 
-#. Default: "Signatories"
-msgid "meeting_signatories"
-msgstr "Signataires"
-
-#. Default: "Signatures"
-msgid "meeting_signatures"
-msgstr "Signatures"
-
 #. Default: "You can consult this meeting at ${objectUrl}."
 msgid "meeting_state_changed_default_mail_body"
-msgstr "Vous pouvez accéder à la séance ici: '${objectUrl}'."
+msgstr "Vous pouvez accéder à la séance ici: ${objectUrl}."
 
 # Mails (meeting-related)
 # Default translation for mails sent upon meeting transition
 # This default is used if no accurate translation can be found. We will try for example to translate
 # meeting_state_changed_decided_mail_subject, if not found (by default), we use meeting_state_changed_default_mail_subject.
 # This way we can have specific mail message for each different transition
 #. Default: "${meetingConfigTitle} - Meeting in state \"${meetingState}\" - ${meetingTitle}"
@@ -4697,25 +4594,17 @@
 msgid "metadata"
 msgstr "Méta-données"
 
 #. Default: "Select here some standard adaptations that can be applied to data structures."
 msgid "model_adaptations_descr"
 msgstr "Sélectionnez ici quelques jeux de modifications que l'on peut appliquer aux structures de données."
 
-#. Default: "Move the item down"
-msgid "move_item_down"
-msgstr "Déplacer le point vers le bas"
-
-#. Default: "Move item to given position"
+#. Default: "Save item number (you may also use the [Enter] key)"
 msgid "move_item_to_given_position"
-msgstr "Déplacer le point au numéro encodé"
-
-#. Default: "Move the item up"
-msgid "move_item_up"
-msgstr "Déplacer le point vers le haut"
+msgstr "Sauvegarder le numéro du point (vous pouvez aussi utiliser la touche [Enter])"
 
 #. Default: "Moves this item to the position that precedes the number you have introduced besides. If you want to move the item at the end of the list, specify the number of the last item plus one."
 msgid "move_several"
 msgstr "Déplace ce point à la position qui précède le numéro que vous introduisez ci-contre. Pour déplacer le point en fin de liste, spécifiez un de plus que le numéro du dernier point."
 
 #. Default: "Negative"
 msgid "negative"
@@ -4733,34 +4622,42 @@
 msgid "nil"
 msgstr "Néant"
 
 #. Default: "No annex is currently defined for this element."
 msgid "no_annexes"
 msgstr "Aucune."
 
-#. Default: "No annexes to print"
-msgid "no_annexes_to_print_term"
-msgstr "Aucune annexe à imprimer"
-
-#. Default: "Annexes not to sign"
-msgid "no_annexes_to_sign_term"
-msgstr "Annexes à ne pas signer"
-
 #. Default: "Attributes \"assembly\" and \"attendees\" can't be used together."
 msgid "no_assembly_and_attendees"
-msgstr "Les attributs \"assemblée\" et \"présents\" ne peuvent être utilisés ensemble."
+msgstr "Les attributs \"Assemblée (assembly)\" et \"Présents (attendees)\" ne peuvent être utilisés ensemble."
 
 #. Default: "No category is currently defined."
 msgid "no_category"
 msgstr "Aucune catégorie n'est actuellement définie."
 
 #. Default: "No classifier is currently defined."
 msgid "no_classifier"
 msgstr "Aucun classificateur n'est actuellement défini."
 
+#. Default: "NC"
+msgid "no_committee_term_title_acronym"
+msgstr "NoComm"
+
+#. Default: "No committee"
+msgid "no_committee_term_title_label"
+msgstr "Ne passe pas en commission"
+
+#. Default: "Attributes \"committees_assembly\" and \"committees_attendees\" can't be used together."
+msgid "no_committees_assembly_and_committees_attendees"
+msgstr "Les attributs \"Assemblée (committees_assembly)\" et \"Présents (committees_attendees)\" ne peuvent être utilisés ensemble."
+
+#. Default: "Attributes \"committees_sigantures\" and \"committees_signatories\" can't be used together."
+msgid "no_committees_signatures_and_committees_signatories"
+msgstr "Les attributs \"Signatures (committees_signatures)\" et \"Présents (committees_attendees)\" ne peuvent être utilisés ensemble."
+
 #. Default: "None"
 msgid "no_config_group"
 msgstr "Aucun"
 
 #. Default: "No emergency"
 msgid "no_emergency"
 msgstr "Aucune urgence souhaitée"
@@ -4785,33 +4682,29 @@
 msgid "no_meeting_file_type"
 msgstr "Aucun type d'annexe n'est actuellement défini."
 
 #. Default: "No special user is currently defined."
 msgid "no_meeting_user"
 msgstr "Aucun utilisateur spécial n'est actuellement défini."
 
-#. Default: "No items."
-msgid "no_meetingitems"
-msgstr "Pas de points."
-
 #. Default: "No POD template is currently defined."
 msgid "no_pod_folder"
 msgstr "Aucun modèle de document défini pour le moment."
 
 #. Default: "Attributes \"proposingGroupWithGroupInCharge\" and \"groupsInCharge\" can't be used together."
 msgid "no_proposingGroupWithGroupInCharge_and_groupsInCharge"
 msgstr "Les attributs \"Groupe proposant (Groupe en charge) (proposingGroupWithGroupInCharge)\" et \"Groupes en charge (groupsInCharge)\" ne peuvent être utilisés ensemble."
 
 #. Default: "No recurring item is currently defined."
 msgid "no_recurring_item"
 msgstr "Aucun point récurrent n'est actuellement défini."
 
-#. Default: "No visible item for now."
+#. Default: "You do not have access to these items."
 msgid "no_shown_items"
-msgstr "Pas de point visible pour le moment."
+msgstr "Vous n'avez pas accès à ces points."
 
 #. Default: "Attributes \"signatures\" and \"signatories\" can't be used together."
 msgid "no_signatories_and_signatures"
 msgstr "Les attributs \"signatures\" et \"signataires\" ne peuvent être utilisés ensemble."
 
 #. Default: "No style POD template is currently defined."
 msgid "no_style_pod_folder"
@@ -4837,14 +4730,22 @@
 msgid "normal"
 msgstr "Point normal"
 
 #. Default: "You are a registered user but your account has not been activated yet. Please contact the system administrator."
 msgid "notPloneMeetingUser"
 msgstr "Vous êtes un utilisateur enregistré mais votre compte n'a pas encore été activé. Veuillez contacter l'administrateur."
 
+#. Default: "Not able to find a meeting to present this item into.  Only meetings in the future are taken into account, check configuration if necessary"
+msgid "not_able_to_find_meeting_to_present_item_into"
+msgstr "Impossible de déterminer une séance dans laquelle présenter ce point.  Seules les séances dans le futur sont prises en compte, présentez le point depuis la séance souhaitée ou vérifiez la configuration si nécessaire"
+
+#. Default: "Not confidential annexes"
+msgid "not_confidential_annexes"
+msgstr "Annexes (non confidentielles)"
+
 #. Default: "Not given yet"
 msgid "not_given"
 msgstr "Non rendu"
 
 #. Default: "Not to be cloned to anywhere"
 msgid "not_to_be_cloned_to_term"
 msgstr "Pas à envoyer"
@@ -4861,14 +4762,22 @@
 msgid "nothing_to_do"
 msgstr "Rien à faire."
 
 #. Default: "notify users able to view the element"
 msgid "notify_users_able_to_view_element"
 msgstr "prévient les utilisateurs capables de voir l'élément"
 
+#. Default: "${number}st"
+msgid "num_part_st"
+msgstr "${number}er"
+
+#. Default: "${number}th"
+msgid "num_part_th"
+msgstr "${number}ème"
+
 #. Default: "Total number of voters"
 msgid "number_of_voters"
 msgstr "Votants"
 
 #. Default: "Observer"
 msgid "observer"
 msgstr "Observateur"
@@ -4877,14 +4786,18 @@
 msgid "observers"
 msgstr "Observateurs"
 
 #. Default: "Follow all associated groups order"
 msgid "on_all_associated_groups"
 msgstr "Suivre l'ordre de tous les groupes associés"
 
+#. Default: "Follow all committees order"
+msgid "on_all_committees"
+msgstr "Suivre l'ordre de toutes les commissions"
+
 #. Default: "Follow all groups order"
 msgid "on_all_groups"
 msgstr "Suivre l'ordre de tous les groupes"
 
 #. Default: "Follow categories order"
 msgid "on_categories"
 msgstr "Suivre l'ordre des catégories"
@@ -4965,14 +4878,18 @@
 msgid "oral_question_item_descr"
 msgstr " "
 
 #. Default: "If this field is left empty, selectable associated organizations are every organizations selected in the plonegroup configuration panel.  Here you may select associated organizations in a particular order including organizations that are not selected in the plonegroup configuration panel.  This is only relevant if the 'Associated groups' field is enabled on items."
 msgid "ordered_associated_organizations_descr"
 msgstr "Par défaut, les groupes associés sélectionnables sur un point seront toutes les organisations sélectionnées dans le panneau de configuration de plonegroup.  Définissez ici les organisations qui pourront être sélectionnées sur les points, y compris les organisations qui ne sont pas sélectionnées dans le panneau de configuration de plonegroup. Ceci n'est utile que si vous utilisez le champ \"Groupes associés (associatedGroups)\" sur les points."
 
+#. Default: "Select here attendees that will be selectable in the \"Attendees\" column of defined committees here under.  <span style='color: red;'>If you select/unselect values, you need to save first then edit again for these values to appear/disappear if field \"Committees\" here under.</span>"
+msgid "ordered_committee_contacts_descr"
+msgstr "Sélectionnez les contacts qui seront utilisés comme membres d'assemblée pour les commissions (ainsi que pour la colonne \"Présents par défaut / Signataires par défaut\" ci-dessous).  <span style='color: red;'>Attention, si vous (dé)séléctionnez des valeurs, vous devrez d'abord sauvegarder et éditer la configuration à nouveau pour qu'elles apparaissent/disparaissent des \"Commissions\" ci-dessous.</span>"
+
 #. Default: "Select here contacts that will be usable to manage meeting attendees.  The contacts order defined here will be the default order when creating a new meeting."
 msgid "ordered_contacts_descr"
 msgstr "Sélectionnez les contacts qui seront utilisés comme membres d'assemblée pour les séances, c'est-à-dire les éléments de type \"Fonction occupée\" pour lesquels la valeur \"Membre d'assemblée\" est sélectionnée dans le champ \"Utilisé comme\".  L'ordre sélectionné ici sera celui repris par défaut sur chaque séance <span style='color:red;'>nouvellement créée, les changements apportés à ce champ n'impacte pas les séances déjà créées.</span> Ceci fonctionnera uniquement si vous utilisez l'attribut \"Présents (attendees)\" sur les séances."
 
 #. Default: "If this field is left empty, selectable groups in charge are every organizations selected in the plonegroup configuration panel.  Here you may select groups in charge in a particular order.  This is only relevant if the 'Groups in charge' field is enabled on items."
 msgid "ordered_groups_in_charge_descr"
 msgstr "Par défaut, les groupes en charge sélectionnables sur un point seront toutes les organisations sélectionnées dans le panneau de configuration de plonegroup. Vous pouvez changer cela en définissant ici les groupes en charge ainsi que l'ordre à utiliser. Ceci n'est utile que si vous utilisez le champ \"Groupes en charge (groupsInCharge)\" sur les points."
@@ -5005,22 +4922,26 @@
 msgid "owner_may_delete_annex_decision_descr"
 msgstr "Si vous cochez cette case, l'utilisateur ayant ajouté une annexe à la décision lorsque le point n'est plus éditable pourra la supprimer, sinon, seul un administrateur pourra la supprimer.  Un utilisateur ayant la main sur le point (point éditable) pourra continuer à gérer toutes les annexes (ajout/modification/suppression)."
 
 #. Default: "Mark this person absent for this item"
 msgid "person_byebye"
 msgstr "Marquer ce membre absent pour ce point"
 
+#. Default: "Redefine position for attendee for this item"
+msgid "person_redefine_attendee_position"
+msgstr "Changer la fonction de ce membre pour ce point"
+
+#. Default: "Remove redefined position for attendee for this item"
+msgid "person_remove_redefined_attendee_position"
+msgstr "Enlever la fonction redéfinie pour ce membre pour ce point"
+
 #. Default: "Remove this person from absents for this item"
 msgid "person_welcome"
 msgstr "Enlever ce membre des absents pour ce point"
 
-#. Default: "Please encode this other place."
-msgid "place_other_required"
-msgstr "Veuillez donner un nom pour cet autre lieu."
-
 #. Default: "Enter here some default places where meetings occur. There must be one place per line. The first one will be the default one."
 msgid "places_descr"
 msgstr "Spécifiez ici quelques lieux de prédilection pour la tenue des séances. Il doit y avoir un lieu par ligne. Le premier lieu sera le lieu par défaut."
 
 #. Default: "You are about to delete this meeting and all included items. Are you sure?"
 msgid "plonemeeting_delete_meeting_confirm_message"
 msgstr "Etes-vous certain de vouloir supprimer cette séance ET tous ses points?"
@@ -5035,15 +4956,15 @@
 
 #. Default: "Check Pod templates"
 msgid "pm_check_pod_templates"
 msgstr "Vérifier les modèles Pod"
 
 #. Default: "Warning: the action \"Check Pod templates\" will check that every Pod templates defined in the configuration are working correctly."
 msgid "pm_check_pod_templates_warning"
-msgstr "Attention: l'action \"Vérifier les modèles Pod\" va vérifier que les modèles définis dans la partie \"[Documents]\" de cette configuration fonctionnent correctement."
+msgstr "Attention, l'action \"Vérifier les modèles Pod\" va vérifier que les modèles définis dans la partie \"[Documents]\" de cette configuration fonctionnent correctement."
 
 #. Default: "Configuration of deliberations"
 msgid "pm_configuration"
 msgstr "Configuration des délibérations"
 
 #. Default: "Convert annexes for preview"
 msgid "pm_convert_annexes"
@@ -5075,63 +4996,63 @@
 
 #. Default: "Invalidate all cache in the application"
 msgid "pm_invalidate_all_cache"
 msgstr "Invalider le cache applicatif"
 
 #. Default: "Warning: this will invalidate all cache used in the application, this could lead to application being slow for some minutes until cache is recomputed for currently connected users but is harmless and must be done when changes impacting application header (tabs) are made or if any weirdness occurs (no access to new tabs, ...)."
 msgid "pm_invalidate_all_cache_warning"
-msgstr "Attention: ceci va invalider tout le cache utilisé dans l'application (vocabulaires, portlets, cache navigateur utilisateurs, ...) et pourrait provoquer quelques lenteurs pendant quelques minutes le temps qu'il soit recalculé chez les différents utilisateurs.  Cette action est sans danger et doit être opérée si des changements impactent l'entête (onglets) de l'application ou si des bizarreries apparaissent (pas d'accès à un élément de configuration créé ou modifié, ...)."
+msgstr "Attention, ceci va invalider tout le cache utilisé dans l'application (vocabulaires, portlets, cache navigateur utilisateurs, ...) et pourrait provoquer quelques lenteurs pendant quelques minutes le temps qu'il soit recalculé chez les différents utilisateurs.  Cette action est sans danger et doit être opérée si des changements impactent l'entête (onglets) de l'application ou si des bizarreries apparaissent (pas d'accès à un élément de configuration créé ou modifié, ...)."
 
 #. Default: "Modification date"
 msgid "pm_modification_date"
 msgstr "Modifié le"
 
 #. Default: "Remove annexes previews of items in closed meetings"
 msgid "pm_remove_annexes_previews"
 msgstr "Supprimer les prévisualisations des annexes des points dans les séances clôturée"
 
 #. Default: "Warning: take care that launching these proceedings may take time, depending on the number of existing elements!  Do not launch during period of high use!"
 msgid "pm_tool_updates_warning"
-msgstr "Attention: ces opérations peuvent prendre du temps en fonction du nombre d'éléments existants!  Ne pas lancer dans une période de forte utilisation!"
+msgstr "Attention, ces opérations peuvent prendre du temps en fonction du nombre d'éléments existants!  Ne pas lancer dans une période de forte utilisation!"
 
 #. Default: "Initialize every existing advice confidentiality"
 msgid "pm_update_advice_confidentiality"
 msgstr "Initialiser la confidentialité des avis existants"
 
 #. Default: "Warning: the action \"Initialize existing advices confidentiality\" will initialize every existing advice confidentiality to what is defined as default value in this meeting configuration (check the field \"Advice confidentiality default value\" of the \"Advices and access\" tab)."
 msgid "pm_update_advice_confidentiality_warning"
-msgstr "Attention : l'action \"Initialiser la confidentialité des avis existants\" va initialiser la confidentialité de tous les avis existants pour cette configuration de séance à la valeur par défaut définie pour la confidentialité d'un avis (vérifiez le champ \"Valeur par défaut du champ 'Confidentiel?' des avis créés\" dans l'onglet \"Avis et accès\")."
+msgstr "Attention, l'action \"Initialiser la confidentialité des avis existants\" va initialiser la confidentialité de tous les avis existants pour cette configuration de séance à la valeur par défaut définie pour la confidentialité d'un avis (vérifiez le champ \"Valeur par défaut du champ 'Confidentiel?' des avis créés\" dans l'onglet \"Avis et accès\")."
 
 #. Default: "Update all items and meetings of every meeting configurations"
 msgid "pm_update_all_local_roles"
 msgstr "Mettre à jour les points et séances de toutes les configurations de séance"
 
 #. Default: "Warning: this will update every items and meetings of every configurations.  This action is also available per meeting configuration, if you only changed parameters in one meeting configuration, just execute the action on this meeting configuration!"
 msgid "pm_update_all_local_roles_warning"
-msgstr "Attention: ceci mettra à jour les points et séances pour toutes les configurations de séances.  Cette action est également disponible par configuration de séance, si vous avez changé un paramètre dans une configuration de séance en particulier, utilisez l'action sur la configuration de séance.  Enfin, l'action par lot \"Mettre à jour les accès\" disponible dans les tableaux de bord de points et séances pour les administrateurs permet d'effectuer la même mise à jour si vous savez quels points et séances sont impactés."
+msgstr "Attention, ceci mettra à jour les points et séances pour toutes les configurations de séances.  Cette action est également disponible par configuration de séance, si vous avez changé un paramètre dans une configuration de séance en particulier, utilisez l'action sur la configuration de séance.  Enfin, l'action par lot \"Mettre à jour les accès\" disponible dans les tableaux de bord de points et séances pour les administrateurs permet d'effectuer la même mise à jour si vous savez quels points et séances sont impactés."
 
 #. Default: "Initialize every existing annex confidentiality"
 msgid "pm_update_annex_confidentiality"
 msgstr "Initialiser la confidentialité des annexes existantes"
 
 #. Default: "Warning: the action \"Initialize existing annexes confidentiality\" will initialize every existing annex confidentiality to what is defined in the corresponding annex type (check the \"Annex types\" in the \"Data\" tab)."
 msgid "pm_update_annex_confidentiality_warning"
-msgstr "Attention : l'action \"Initialiser la confidentialité des annexes existantes\" va initialiser la confidentialité de toutes les annexes existantes pour cette configuration de séance à la valeur par défaut définie sur le \"Type d'annexe\" correspondant (vérifiez les \"Types d'annexes\" dans l'onglet \"Données\")."
+msgstr "Attention, l'action \"Initialiser la confidentialité des annexes existantes\" va initialiser la confidentialité de toutes les annexes existantes pour cette configuration de séance à la valeur par défaut définie sur le \"Type d'annexe\" correspondant (vérifiez les \"Types d'annexes\" dans l'onglet \"Données\")."
 
 #. Default: "Update annex indexes"
 msgid "pm_update_annex_indexes"
 msgstr "Recalculer les index des annexes"
 
 #. Default: "Initialize personal label on existing items"
 msgid "pm_update_personal_labels"
 msgstr "Initialiser l'étiquette sur les points existants"
 
 #. Default: "Warning: the action \"Initialize personal labels\" will activate selected labels on every existing items that were last modified before given number of days for every users able to see these items."
 msgid "pm_update_personal_labels_warning"
-msgstr "Attention : l'action \"Initialiser l'étiquette sur les points existants\" va activer l'étiquette sélectionnée sur tous les points existants qui n'ont plus été modifiés depuis le nombre de jours choisi, et ce, pour tous les utilisateurs qui peuvent voir ces points."
+msgstr "Attention, l'action \"Initialiser l'étiquette sur les points existants\" va activer l'étiquette sélectionnée sur tous les points existants qui n'ont plus été modifiés depuis le nombre de jours choisi, et ce, pour tous les utilisateurs qui peuvent voir ces points."
 
 #. Default: "Please consult the attached document."
 msgid "podItemByMail_mail_body"
 msgstr "Veuillez consulter le fichier joint."
 
 #. Default: "${meetingConfigTitle} - ${podTemplateTitle} - ${objectTitle}."
 msgid "podItemByMail_mail_subject"
@@ -5211,23 +5132,15 @@
 
 #. Default: "Power observers"
 msgid "powerobservers"
 msgstr "Super observateurs"
 
 #. Default: "The preparatory meeting must occur before the meeting."
 msgid "pre_date_after_meeting_date"
-msgstr "La réunion préparatoire doit survenir avant la réunion."
-
-#. Default: "Preparatory meeting"
-msgid "pre_meeting"
-msgstr "Réunion préparatoire"
-
-#. Default: "Specify here the date of the pre-meeting, relative to its meeting, in the same format as fields above.  Leave the field empty not to use this functionality."
-msgid "pre_meeting_date_default_descr"
-msgstr "Spécifiez ici la date de la séance préparatoire, par rapport à la date de la séance, dans le même format que les champs ci-dessus.  Laissez le champ vide si vous ne souhaitez pas utiliser cette fonctionnalité."
+msgstr "La date de séance préparatoire doit être avant la date de séance."
 
 #. Default: "If this is a normal item and you want it to be inserted in any availale meeting, just select \"No preference\" value.  Selecting a date is for 2 usecases : this will make the item not presentable to the meetings before selected one, or if the selected meeting is \"frozen\", this will make current item considered as \"late\" item presentable in the selected frozen meeting.  Indeed, the only way to insert an item in a frozen meeting is to select this meeting as preferred meeting."
 msgid "preferred_meeting_descr"
 msgstr "Si vous laissez la valeur \"Pas de préférence\", le point pourra être présenté dans n'importe quelle séance \"En création\" mais ne pourra pas être présenté \"En urgence\" dans une séance \"Gelée\".  Deux fonctonnalités sont activées lorsqu'une séance est sélectionnée: premièrement le point ne pourra pas être présenté dans une séance avant celle sélectionnée, ensuite, le point pourra y être présenté quel que soit l'état de celle-ci (\"En création\", \"Gelée\", ...) et notamment en tant que point \"En urgence\" dès que la séance sera \"Gelée\"."
 
 #. Default: "Pre-validator"
 msgid "prereviewer"
@@ -5273,34 +5186,34 @@
 msgid "public"
 msgstr "Séance publique"
 
 #. Default: "Public meeting (heading)"
 msgid "public_heading"
 msgstr "Séance publique (entête)"
 
-#. Default: "Specify here the deadline for validating items to be inserted in a given meeting. You need to express this deadline relative to the meeting date. For example, \"5.9:30\" (do not type quotes) means: \"5 days before the meeting date, at 9:30.\".  Leave the field empty not to use this functionality."
-msgid "publish_deadline_default_descr"
-msgstr "Spécifiez ici l'échéance pour valider des points à insérer dans une séance donnée. Vous devez exprimer cette échéance comme étant relative à la date de la séance. Par exemple, \"5.9:30\" (n'encodez pas d'apostrophes) signifie \"5 jours avant la date de la séance, à 9:30\".  Laissez le champ vide si vous ne souhaitez pas utiliser cette fonctionnalité."
-
 #. Default: "Publishable (displayed)"
 msgid "publishable_display"
 msgstr "Publiable (affiché seulement aux gestionnaires de séances)"
 
 #. Default: "Publishable (editable)"
 msgid "publishable_edit"
 msgstr "Publiable (éditable seulement par les gestionnaires de séances)"
 
+#. Default: "Read less"
+msgid "read_less"
+msgstr "Cacher le texte"
+
+#. Default: "Read more"
+msgid "read_more"
+msgstr "Lire la suite"
+
 #. Default: "Select here the item states into which some events related to the item (like annex creations or deletions) will be stored in the item's history."
 msgid "record_item_history_states_descr"
 msgstr "Sélectionnez ici les états des points dans lesquels certains événements relatifs aux points (comme la création ou la suppression d'annexes) seront stockés dans leur historique."
 
-#. Default: "Select here the meeting states into which some events related to the meeting will be stored in the meeting's history."
-msgid "record_meeting_history_states_descr"
-msgstr "Sélectionnez ici les états des séances dans lesquels l'historisation sera activée."
-
 #. Default: "The recurring item specified in the subject of this email could not be inserted in a meeting. Maybe does it lack some important information (a text for the decision, for example) while the meeting is in an \"advanced\" state (it is already \"decided\", for instance). More information can be found in the log file of your Zope instance."
 msgid "recurringItemWorkflowError_mail_body"
 msgstr "Le point récurrent spécifié dans le sujet de ce courriel n'a pas pu être présenté dans une séance. Peut-être ne dispose-t-il pas de suffisemment d'informations (un texte pour la décision, par exemple) pour être ajouté à la séance, celle-ci pouvant se trouver dans un état \"avancé\" (décidée, par exemple). Plus d'info dans le log de votre instance Zope."
 
 #. Default: "${portalTitle} - A problem occurred while inserting a recurring into a meeting - ${itemTitle}"
 msgid "recurringItemWorkflowError_mail_subject"
 msgstr "${portalTitle} - Problème survenu lors de l'insertion d'un point récurrent dans une séance - ${itemTitle}"
@@ -5345,26 +5258,34 @@
 msgid "remove_several_items"
 msgstr "Retirer tous les points sélectionnés."
 
 #. Default: "Selected items have been removed from the meeting."
 msgid "remove_several_items_done"
 msgstr "Les points sélectionnés ont été retirés de la séance."
 
-#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by \"${hp_url}\"!"
+#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by held position at \"${hp_url}\"!"
 msgid "removed_position_type_in_use_error"
-msgstr "Vous ne pouvez pas supprimer un type de fonction utilisé, le type de fonction supprimé \"${removed_position_type}\" est utilisé par \"${hp_url}\"!"
+msgstr "Vous ne pouvez pas supprimer un type de fonction utilisé, le type de fonction supprimé \"${removed_position_type}\" est utilisé par la fonction occupée \"${hp_url}\"!"
+
+#. Default: "You can not remove a position type that was used as redefined position for an attendee on an item, you removed \"${removed_position_type}\", check attendees on item at \"${item_url}\"!"
+msgid "removed_redefined_position_type_in_use_error"
+msgstr "Vous ne pouvez pas supprimer un type de fonction utilisé comme fonction redéfinie pour un membre d'assemblée pour un point, le type de fonction supprimé \"${removed_position_type}\" est utilisé par un membre d'assemblée sur le point \"${item_url}\"!"
 
 #. Default: "A category must be selected on this item so it may evolve in the workflow"
 msgid "required_category_ko"
 msgstr "Une catégorie doit être sélectionnée sur ce point afin qu'il puisse continuer à évoluer dans le workflow"
 
 #. Default: "A classifier must be selected on this item so it may evolve in the workflow"
 msgid "required_classifier_ko"
 msgstr "Un classificateur doit être sélectionné sur ce point afin qu'il puisse continuer à évoluer dans le workflow"
 
+#. Default: "A group in charge must be selected on this item so it may evolve in the workflow"
+msgid "required_groupsInCharge_ko"
+msgstr "Un groupe en charge doit être sélectionné sur ce point afin qu'il puisse continuer à évoluer dans le workflow"
+
 #. Default: "Check the box if access to secret items must be restricted.  This will let only users for which an explicit access to the item has been given, access the item.  It will be the case so for members of the proposing groups, power users (Managers, MeetingManagers, power observers), copy groups and advisers.  Only activate this if necessary, it could be the case if you have a state where everything is accessible by everyone (like a \"published\" state for items) but where you want \"secret\" items not to be accessible by everyone."
 msgid "restrict_access_to_secret_items_descr"
 msgstr "Si vous cochez cette case, l'accès aux points \"à huis clos\" sera restreint pour certains utilisateurs.  Ceci permet de spécifier que les points à huis clos ne doivent être accessible qu'aux personnes ayant reçu un accès explicite au point : les super utilisteurs (administrateurs, gestionnaires de séances, super observateurs), les membres du groupe proposant, les groupes en copies et les émetteurs d'avis (dont l'avis est demandé sur le point).  Par défaut, cette fonctionnalité est désactivée, à n'activer que si nécessaire, par exemple dans le cas où vous avez un état sur le point qui est accessible à tous (par exemple \"publié\") mais que vous souhaitez malgré tout que les points à huis clos ne soient accessible que de manière explicite."
 
 #. Default: "Restrict access to secret items to description"
 msgid "restrict_access_to_secret_items_to_descr"
 msgstr "Sélectionnez les profils d'utilisateurs qui seront restreint quand à l'accès aux points à huis-clos. Sera pris en compte si le paramaètre précédent (Restreindre l'accès aux points à huis clos?) est coché."
@@ -5546,14 +5467,18 @@
 msgid "selectable_for_plonegroup_descr"
 msgstr "Décocher cette case si cette organisation est ajoutée dans un autre but que celui de créer les sous-groupes Plone relatifs permettant à cette organization d'utiliser l'application."
 
 #. Default: "Select here privacies that will be selectable by users editing items of this configuration.  If \"on privacy\" is used in the \"Sort order(s) to apply when adding an item to a meeting\" field, it is the order of values selected here that will be used."
 msgid "selectable_privacies_descr"
 msgstr "Spécifiez ici les niveaux de confidentialité qui pourront être sélectionnés lors de l'édition d'un point.  Si \"Par niveau de confidentialité\" est sélectionné dans \"Méthode(s) de tri lors de l'ajout d'un point dans une séance\", c'est l'ordre des niveaux de confidentialité sélectionnés ici qui sera utilisé."
 
+#. Default: "Select here position types that will be selectable when redefining the position of an attendee for an item.  If nothing selected (default), then any position types is selectable."
+msgid "selectable_redefined_position_types_descr"
+msgstr "Sélectionnez les types de fonctions qui pourront être utilisées lors de l'utilisation de la fonctionnalité \"Changer la fonction de ce membre pour ce point\".  Si rien n'est sélectionné (comportement par défaut), tous les types de fonctions pourront être choisis."
+
 #. Default: "Check the box if item needs to be send to authority, if so, a line will be automatically printed in the item deliberation document."
 msgid "send_to_authority_descr"
 msgstr "Cochez la case si ce point doit être soumis à l'autorité de tutelle."
 
 #. Default: "Unable to send this item to the ${meetingConfigTitle} meetingConfig because the user to create the item to does not have a personal folder in this meetingConfig.  If necessary, the concerned user can connect for this folder to be created automatically."
 msgid "sendto_inexistent_destfolder_error"
 msgstr "Impossible d'envoyer ce point vers le type de séance ${meetingConfigTitle} car l'utilisateur n'a pas d'espace dans cet autre type de séance.  Il est nécessaire que l'utilisateur concerné se connecte à l'application pour que cet espace soit créé automatiquement."
@@ -5599,18 +5524,14 @@
 msgid "show_or_hide_details"
 msgstr "Afficher / masquer les détails"
 
 #. Default: "Show / hide poll type observations"
 msgid "show_or_hide_pollTypeObservations"
 msgstr "Afficher / masquer les \"Observations sur le mode de scrutin\""
 
-#. Default: "Signatures"
-msgid "signatures"
-msgstr "Signatures"
-
 #. Default: "Signatures as defined on the linked meeting"
 msgid "signatures_defined_on_meeting"
 msgstr "Signatures définies sur la séance"
 
 #. Default: "Define here the default signatures that will be automatically selected on newly created meetings. Use 2 lines by signature, one for the function and one for the signatory name. This will be applicable only if you use attribute \"Signatures\" for meetings."
 msgid "signatures_descr"
 msgstr "Définissez ici les signatures par défaut qui seront automatiquement sélectionnées sur chaque séance <span style='color:red;'>nouvellement créée, les changements apportés à ce champ n'impacte pas les séances déjà créées.</span> Utilisez 2 lignes par signature, une ligne pour la fonction et une ligne pour le nom du signataire. Ceci fonctionnera uniquement si vous utilisez l'attribut \"Signatures (signatures)\" sur les séances."
@@ -5623,14 +5544,22 @@
 msgid "signed_edit"
 msgstr "À signer/Signé (éditable seulement par les gestionnaires de séances)"
 
 #. Default: "Check this box if you want to sort the tags in alphabetic order."
 msgid "sort_all_item_tags_descr"
 msgstr "Cochez cette case si vous voulez que les marqueurs soient triés par ordre alphabétique."
 
+#. Default: "The meeting start date must occur before the end date."
+msgid "start_date_after_end_date"
+msgstr "La date de début doit être avant la date de fin."
+
+#. Default: "The meeting start date must occur after the meeting date."
+msgid "start_date_before_meeting_date"
+msgstr "La date de début de la séance ne peut pas être avant la date de séance."
+
 #. Default: "Store as annex of type ${annex_type_title}"
 msgid "store_as_annex_type_title"
 msgstr "Stocker en tant qu'annexe de type \"${annex_type_title}\""
 
 #. Default: "Not allowed to add annex in this element."
 msgid "store_podtemplate_as_annex_can_not_add_annex"
 msgstr "Vous n'avez pas la permission d'ajouter une annexe à cet élément."
@@ -5724,21 +5653,217 @@
 msgstr "Ce point est une question orale"
 
 #. Default: "This item is NOT an oral question"
 msgid "this_item_is_not_an_oral_question"
 msgstr "Ce point N'EST PAS une question orale"
 
 #. Default: "Extraordinary session"
-msgid "this_meeting_is_extraodrinary_session"
+msgid "this_meeting_is_extraordinary_session"
 msgstr "Séance extraordinaire"
 
+#. Default: "Absents"
+msgid "title_absents"
+msgstr "Absents (non excusés)"
+
+#. Default: "Approval date"
+msgid "title_approval_date"
+msgstr "Date d'approbation"
+
+#. Default: "Assembly"
+msgid "title_assembly"
+msgstr "Assemblée"
+
+#. Default: "Assembly absents"
+msgid "title_assembly_absents"
+msgstr "Absents"
+
+#. Default: "Assembly excused"
+msgid "title_assembly_excused"
+msgstr "Excusés"
+
+#. Default: "Assembly guests"
+msgid "title_assembly_guests"
+msgstr "Invités"
+
+#. Default: "Assembly observations"
+msgid "title_assembly_observations"
+msgstr "Observations (assemblée et signatures)"
+
+#. Default: "Assembly proxies"
+msgid "title_assembly_proxies"
+msgstr "Procurations"
+
+#. Default: "Assembly staves"
+msgid "title_assembly_staves"
+msgstr "Assistants"
+
+#. Default: "Attendees"
+msgid "title_attendees"
+msgstr "Présents"
+
+#. Default: "Authority notice"
+msgid "title_authority_notice"
+msgstr "Avis de tutelle"
+
+#. Default: "Committees"
+msgid "title_committees"
+msgstr "Commissions"
+
+#. Default: "Assembly"
+msgid "title_committees_assembly"
+msgstr "Assemblée"
+
+#. Default: "Attendees"
+msgid "title_committees_attendees"
+msgstr "Présents"
+
+#. Default: "Convocation date"
+msgid "title_committees_convocation_date"
+msgstr "Date de convocation"
+
+#. Default: "Date"
+msgid "title_committees_date"
+msgstr "Date"
+
+#. Default: "Committees observations"
+msgid "title_committees_observations"
+msgstr "Observations (commissions)"
+
+#. Default: "Place"
+msgid "title_committees_place"
+msgstr "Lieu"
+
+#. Default: "Committee"
+msgid "title_committees_row_id"
+msgstr "Commission"
+
+#. Default: "Signatories"
+msgid "title_committees_signatories"
+msgstr "Signataires"
+
+#. Default: "Signatures"
+msgid "title_committees_signatures"
+msgstr "Signatures"
+
+#. Default: "Convocation date"
+msgid "title_convocation_date"
+msgstr "Date de convocation"
+
+#. Default: "Date"
+msgid "title_date"
+msgstr "Date"
+
+#. Default: "Default assembly"
+msgid "title_default_assembly"
+msgstr "Assemblée par défaut"
+
+#. Default: "Default assembly staves"
+msgid "title_default_assembly_staves"
+msgstr "Assistants par défaut"
+
+#. Default: "Default signatures"
+msgid "title_default_signatures"
+msgstr "Signatures par défaut"
+
+#. Default: "End date"
+msgid "title_end_date"
+msgstr "Date et heure de fin"
+
+#. Default: "Excused"
+msgid "title_excused"
+msgstr "Excusés"
+
+#. Default: "Extraordinary session"
+msgid "title_extraordinary_session"
+msgstr "Séance extraordinaire?"
+
+#. Default: "First item number (managed automatically when meeting is frozen)"
+msgid "title_first_item_number"
+msgstr "Numéro du premier point de cette séance (géré automatiquement par l'application lors du gel de la séance)"
+
+#. Default: "In and out moves"
+msgid "title_in_and_out_moves"
+msgstr "Entrées et sorties (assemblée)"
+
+#. Default: "Meeting number"
+msgid "title_meeting_number"
+msgstr "Numéro de séance (géré automatiquement par l'application lors du gel de la séance)"
+
+#. Default: "Meeting managers notes"
+msgid "title_meetingmanagers_notes"
+msgstr "Notes gestionnaires de séances"
+
+#. Default: "Mid date"
+msgid "title_mid_date"
+msgstr "Date et heure de fin de la première partie"
+
+#. Default: "Non attendees"
+msgid "title_non_attendees"
+msgstr "Non participants"
+
+#. Default: "Notes"
+msgid "title_notes"
+msgstr "Notes et interpellations"
+
+#. Default: "Observations"
+msgid "title_observations"
+msgstr "Observations"
+
+#. Default: "Place"
+msgid "title_place"
+msgstr "Lieu"
+
+#. Default: "Other place"
+msgid "title_place_other"
+msgstr "Lieu (\"Autre\")"
+
+#. Default: "Pre meeting date"
+msgid "title_pre_meeting_date"
+msgstr "Date (séance préparatoire)"
+
+#. Default: "Pre meeting place"
+msgid "title_pre_meeting_place"
+msgstr "Lieu (séance préparatoire)"
+
+#. Default: "Pre observations"
+msgid "title_pre_observations"
+msgstr "Observations (séance préparatoire)"
+
+#. Default: "Public meeting observations"
+msgid "title_public_meeting_observations"
+msgstr "Observations (séance publique)"
+
+#. Default: "Replacements"
+msgid "title_replacements"
+msgstr "Remplacé par"
+
 #. Default: "A title is required."
 msgid "title_required"
 msgstr "Veuillez spécifier un objet."
 
+#. Default: "Secret meeting observations"
+msgid "title_secret_meeting_observations"
+msgstr "Observations (huis clos)"
+
+#. Default: "Signatories"
+msgid "title_signatories"
+msgstr "Signataires"
+
+#. Default: "Signatures"
+msgid "title_signatures"
+msgstr "Signatures"
+
+#. Default: "Start date"
+msgid "title_start_date"
+msgstr "Date et heure de début"
+
+#. Default: "Votes observations"
+msgid "title_votes_observations"
+msgstr "Observations (votes)"
+
 #. Default: "Ask this advice again (current advice will be historized)"
 msgid "to_advice_asked_again"
 msgstr "Demander cet avis à nouveau (l'avis actuel sera historisé)"
 
 #. Default: "To be printed (displayed)"
 msgid "to_be_printed_display"
 msgstr "À imprimer (affiché seulement aux gestionnaires de séances)"
@@ -5919,18 +6044,14 @@
 msgid "used_poll_types_descr"
 msgstr "Spécifiez ici quels modes de scrutin vous voulez utiliser."
 
 #. Default: "Specify here what vote values are in use in this meeting configuration."
 msgid "used_vote_values_descr"
 msgstr "Spécifiez ici quelles valeurs de vote sont utilisées dans cette configuration de séance."
 
-#. Default: "Users"
-msgid "users"
-msgstr "Utilisateurs"
-
 #. Default: "If you do not select anything, every users will be displayed."
 msgid "users_hidden_in_dashboard_filter_descr"
 msgstr "Si vous ne sélectionnez rien (par défaut), tous les utilisateurs seront affichés.  Ceci impacte les filtres affichant des utilisateurs tels que les filtres 'Auteur' ou 'Pris en charge'."
 
 #. Default: "When an advice is \"given\" and no more editable by the advisers, so when it was set in a state where advisers may not edit it anymore, it is automatically versioned. Depending on the configuration, if advice may be given when the item is still editable by the proposing group, it may be necessary to versionate advice if it was given (but still editable by advisers) and the item was edited. For example, advices are giveable when item is \"itemcreated\", a state where item may still be edited by the proposing group. If it is the case, check this box, it will ensure that the advice is versioned when the item is edited if necessary (so if it was not already versioned since last advice edition).  If you have a specific state \"waiting advice\" where proposing group is not able to edit the item, this box may be left unchecked."
 msgid "versionate_advice_if_given_and_item_modified_descr"
 msgstr "Lorsqu'un avis est \"rendu\" et qu'il n'est plus éditable par les émetteurs d'avis, donc qu'il a été mis dans un état où les émetteurs d'avis ne peuvent plus l'éditer, il est automatiquement versionné. Si dans votre configuration, un avis peut être rendu alors que le point peut toujours être édité par le groupe proposant, il peut être nécessaire de versionner l'avis lors de l'édition du point. Par exemple si les avis peuvent être rendus lorsque le point est 'en création', le groupe proposant peut éditer le point. Dans ce cas, cochez cette case, ceci permettra de s'assurer que l'avis est versionné avant toute modification du point. Si par contre vous avez un état dans votre workflow du type \"en attente des avis\" dans lequel le groupe proposant ne peut pas éditer le point, vous pouvez décocher cette case."
@@ -6247,25 +6368,33 @@
 msgid "wait_msg"
 msgstr "Patientez s'il vous plaît..."
 
 #. Default: "You are currently adding an organization outside \"My organization\", please make sure this is correct.  If you want to create a new group that will be able the create items, give advices, you need to add it directly under \"My organization\"."
 msgid "warning_adding_org_outside_own_org"
 msgstr "Vous êtes en train d'ajouter une organisation en dehors de \"Mon organisation\", est ce bien ce que vous souhaitez faire?  Si vous souhaitez créer un nouveau groupe qui pourra créer des points, émettre des avis, ... vous devez l'ajouter directement sous \"Mon organisation\" (utilisez l'icône présente dans la boîte \"Recherches\" ci-contre, à côté du libellé \"Organisations\")."
 
+#. Default: "Advice is currently \"Asked again\" do not forget to change value of field \"Advice type\" to another value than \"Asked again\""
+msgid "warning_advice_asked_again_need_to_change_advice_type"
+msgstr "L'avis est actuellement \"Demandé à nouveau\", lors de l'édition, n'oubliez pas de choisir une autre valeur pour l'avis dans le champ \"Type d'avis\" ou l'avis sera toujours considéré comme \"Demandé à nouveau\""
+
+#. Default: "Warning, there is a problem with encoded data for assembly and signatures, please check especially that signatories are correctly defined"
+msgid "warning_assembly_and_signatures"
+msgstr "Attention, veuillez vérifier les données encodées pour l'assemblée et les signatures, vérifiez notamment que la ou les signature(s) sont correctement définie(s)"
+
 #. Default: "Warning: if you modify the title or description and save this form, all given advices will be invalidated."
 msgid "warning_invalidate_advices"
-msgstr "Attention: si vous modifiez une donnée et cliquez sur le bouton 'Enregister' au bas du formulaire, tous les avis déjà donnés sur ce point seront invalidés!  Pour ne pas invalider les avis, cliquez sur le bouton 'Annuler' au bas du formulaire."
+msgstr "Attention, si vous modifiez une donnée et cliquez sur le bouton 'Enregister' au bas du formulaire, tous les avis déjà donnés sur ce point seront invalidés!  Pour ne pas invalider les avis, cliquez sur le bouton 'Annuler' au bas du formulaire."
 
 #. Default: "If you modify this field, all given advices will be invalidated."
 msgid "warning_invalidate_advices_fastedit"
 msgstr "Si vous modifiez ce champ, tous les avis seront invalidés!"
 
 #. Default: "Warning: if you add an annex through this form or if you delete an annex, all advices given on this item will be invalidated."
 msgid "warning_invalidate_advices_with_annex"
-msgstr "Attention: si vous ajoutez ou supprimez une annexe, tous les avis déjà donnés sur ce point seront invalidés."
+msgstr "Attention, si vous ajoutez ou supprimez une annexe, tous les avis déjà donnés sur ce point seront invalidés."
 
 #. Default: "DO NOT CHANGE PARAMETERS DEFINED IN THIS SECTION UNLESS YOU ARE REALLY SURE WHAT YOU ARE DOING!"
 msgid "warning_meetingconfig_edit_section_descr"
 msgstr "NE CHANGEZ LES PARAMETRES DEFINIS DANS CETTE SECTION QUE SI VOUS ETES ABSOLUMENT CERTAIN DE CE QUE VOUS FAITES!"
 
 #. Default: "This transition was automatically triggered by the application."
 msgid "wf_transition_triggered_by_application"
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.contact.core.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/collective.contact.core.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.history.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/plone.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/plone.po`

 * *Files 0% similar despite different names*

```diff
@@ -540,14 +540,18 @@
 msgid "close"
 msgstr "Clôturer"
 
 #. Default: "Closed"
 msgid "closed"
 msgstr "Clôturée"
 
+#. Default: "Committees"
+msgid "committees"
+msgstr "Commissions"
+
 #. Default: "Confirm"
 msgid "confirm"
 msgstr "Confirmer"
 
 #. Default: "Confirmed"
 msgid "confirmed"
 msgstr "Confirmé"
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.annex.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/fr/LC_MESSAGES/imio.annex.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/collective.documentgenerator.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/collective.documentgenerator.pot`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/eea.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/eea.po`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 
 msgid "Category"
 msgstr "Category"
 
 msgid "Classifier"
 msgstr "Classifier"
 
+#. Default: "Committee"
+msgid "Committee"
+msgstr ""
+
 #. Default: "Copy groups"
 msgid "Copy groups"
 msgstr "Copy groups"
 
 msgid "Created"
 msgstr "Created"
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.documentgenerator.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.documentgenerator.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.behavior.talcondition.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.behavior.talcondition.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.iconifiedcategory.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.iconifiedcategory.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/datagridfield.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/datagridfield.po`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,62 @@
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: DOMAIN\n"
 
 #. Default: "Available on"
 msgid "Available on"
 msgstr "Available on"
 
+#. Default: "Committee acronym"
+msgid "Committee acronym"
+msgstr ""
+
+#. Default: "Committee auto from"
+msgid "Committee auto from"
+msgstr ""
+
+#. Default: "Committee default assembly"
+msgid "Committee default assembly"
+msgstr ""
+
+#. Default: "Committee default attendees"
+msgid "Committee default attendees"
+msgstr ""
+
+#. Default: "Committee default place"
+msgid "Committee default place"
+msgstr ""
+
+#. Default: "Committee default signatories"
+msgid "Committee default signatories"
+msgstr ""
+
+#. Default: "Committee default signatures"
+msgid "Committee default signatures"
+msgstr ""
+
+#. Default: "Committee enabled?"
+msgid "Committee enabled?"
+msgstr ""
+
+#. Default: "Committee label"
+msgid "Committee label"
+msgstr ""
+
+#. Default: "Committee row id"
+msgid "Committee row id"
+msgstr ""
+
+#. Default: "Committee supplements"
+msgid "Committee supplements"
+msgstr ""
+
+#. Default: "Committee using groups"
+msgid "Committee using groups"
+msgstr ""
+
 #. Default: "Full label"
 msgid "Config group full label"
 msgstr "Full label"
 
 #. Default: "Label"
 msgid "Config group label"
 msgstr "Label"
@@ -310,14 +358,46 @@
 msgid "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field 'States in which an item will be automatically sent to selected other meeting configurations' here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the 'Transitions for presenting an item' you defined in the 'Workflows' tab of the meeting configuration the item will be sent to."
 msgstr "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field \"States in which an item will be automatically sent to selected other meeting configurations\" here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the \"Transitions for presenting an item\" you defined in the \"Workflows\" tab of the meeting configuration the item will be sent to."
 
 #. Default: "Specify here a TAL expression that will restrict or allow the use of this advice to some condition.  We receive \"item\" as the meeting item to give an advice on and \"mayEdit\", a boolean to know if current user may edit the item.  A special expression is available to protect a row that should only be available thru the \"Change delay\" action, it is : \"python: item.REQUEST.get('managing_available_delays', False)\".  This can not be used if something is defined in the \"Advice will be automatically asked if\" column of this advice, but for optional delay-aware advice or for delay-aware advices linked to an automatic advice (using the \"Is linked to previous row?\" column)"
 msgid "available_on_col_description"
 msgstr "Specify here a TAL expression that will restrict or allow the use of this advice to some condition.  We receive \"item\" as the meeting item to give an advice on and \"mayEdit\", a boolean to know if current user may edit the item.  A special expression is available to protect a row that should only be available thru the \"Change delay\" action, it is : \"python: item.REQUEST.get('managing_available_delays', False)\".  This can not be used if something is defined in the \"Advice will be automatically asked if\" column of this advice, but for optional delay-aware advice or for delay-aware advices linked to an automatic advice (using the \"Is linked to previous row?\" column)"
 
+#. Default: "Used to automatically determinate the committee for the item, the field \"Committees\" will not appear on the item when editing it (except for MeetingManagers).  This may only be used when column \"using_groups\" is not used."
+msgid "committees_auto_from_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Assembly\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_assembly_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Attendees\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_attendees_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Place\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_place_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Signatories\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatories_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Signatures\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatures_col_description"
+msgstr ""
+
+#. Default: "Will generate new values on item \"Committees\" field when necessary to manage supplements (items added to meeting after committees convocation were sent).  This will only be useable by MeetingManagers."
+msgid "committees_supplements_col_description"
+msgstr ""
+
+#. Default: "Used to restrict availability of a committee on the item committees selection box.  This may only be used when column \"auto_from\" is not used."
+msgid "committees_using_groups_col_description"
+msgstr ""
+
 #. Default: "Enter the delay the adviser will have to give his advice. If it is not considered as an automatically asked advice (nothing defined in the \"Advice will be automatically asked if\" column), the advice will be selectable in the \"Ask advice to\" list on the item edit form. A delay is a single digit (like \"5\" or \"10\"). If no delay is relevant for this advice, leave this field blank. If several delays are possible for the same advice, you have to define several rows with exactly the same content excepted the delay."
 msgid "delay_col_description"
 msgstr "Enter the delay the adviser will have to give his advice. If it is not considered as an automatically asked advice (nothing defined in the \"Advice will be automatically asked if\" column), the advice will be selectable in the \"Ask advice to\" list on the item edit form. A delay is a single digit (like \"5\" or \"10\"). If no delay is relevant for this advice, leave this field blank. If several delays are possible for the same advice, you have to define several rows with exactly the same content excepted the delay."
 
 #. Default: "If you want a specific label to be displayed on the label displayed in the \"Advice to give\" list on the item edit form and on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The label will appear between brackets after the message \"Name of the group - delay of X days\"."
 msgid "delay_label_col_description"
 msgstr "If you want a specific label to be displayed on the label displayed in the \"Advice to give\" list on the item edit form and on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The label will appear between brackets after the message \"Name of the group - delay of X days\"."
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/PloneMeeting.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/PloneMeeting.po`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 msgid "${term_title} (Not selected in plonegroup)"
 msgstr "${term_title} (Not selected in plonegroup)"
 
 #. Default: "(Nobody)"
 msgid "(Nobody)"
 msgstr "(Nobody)"
 
+#. Default: "(None)"
+msgid "(None)"
+msgstr "(None)"
+
 #. Default: "Add PloneMeeting Portlet"
 msgid "Add PloneMeeting Portlet"
 msgstr "Add PloneMeeting Portlet"
 
 #. Default: "Add Todo Portlet"
 msgid "Add Todo Portlet"
 msgstr "Add Todo Portlet"
@@ -156,14 +160,18 @@
 msgid "Attendee has been set signatory."
 msgstr "Attendee has been set signatory."
 
 #. Default: "Attendee is no more defined as item signatory."
 msgid "Attendee is no more defined as item signatory."
 msgstr "Attendee is no more defined as item signatory."
 
+#. Default: "Attendee position has been redefined."
+msgid "Attendee position has been redefined."
+msgstr "Attendee position has been redefined."
+
 #. Default: "Back to the MeetingConfig"
 msgid "Back to the MeetingConfig"
 msgstr "Back to the MeetingConfig"
 
 #. Default: "Back to the item"
 msgid "Back to the item"
 msgstr "Back to the item"
@@ -240,14 +248,18 @@
 msgid "Close"
 msgstr "Close"
 
 #. Default: "Comment"
 msgid "Comment"
 msgstr "Commentaire"
 
+#. Default: "Completed votes"
+msgid "Completed votes"
+msgstr "Completed votes"
+
 #. Default: "Contacts fields"
 msgid "Contacts fields"
 msgstr "Contacts fields"
 
 #. Default: "Copy PloneMeeting"
 msgid "Copy PloneMeeting"
 msgstr "Copy PloneMeeting"
@@ -468,38 +480,14 @@
 msgid "If you need to use this person data in the application like for example scanned signature or telephone number, select it here."
 msgstr "If you need to use this person data in the application like for example scanned signature or telephone number, select it here."
 
 #. Default: "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 msgid "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 msgstr "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 
-#. Default: "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgstr "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-
-#. Default: "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgstr "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-
-#. Default: "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgstr "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-
-#. Default: "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgstr "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-
-#. Default: "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgstr "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-
-#. Default: "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgstr "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-
 # plone.app.querystring
 #. Default: "Informations about advices on an item"
 msgid "Informations about advices on an item"
 msgstr "Informations about advices on an item"
 
 #. Default: "Inherited advice action"
 msgid "Inherited advice action"
@@ -511,15 +499,15 @@
 
 #. Default: "It is not possible to add annexes because no file types is defined, please contact system administrator."
 msgid "It is not possible to add annexes because no file types is defined, please contact system administrator."
 msgstr "It is not possible to add annexes because no file types is defined, please contact system administrator."
 
 #. Default: "Item \"${item_title}\" could not be presented!"
 msgid "Item \"${item_title}\" could not be presented!"
-msgstr ""
+msgstr "Item \"${item_title}\" could not be presented!"
 
 #. Default: "Item absents to apply"
 msgid "Item absents to apply"
 msgstr "Item absents to apply"
 
 #. Default: "Item action delete"
 msgid "Item action delete"
@@ -677,27 +665,27 @@
 
 #. Default: "Items"
 msgid "Meeting items"
 msgstr "Items"
 
 #. Default: "Meeting signatory not used, another signatory with same signature number is used"
 msgid "Meeting signatory not used, another signatory with same signature number is used"
-msgstr ""
+msgstr "Meeting signatory not used, another signatory with same signature number is used"
 
 #. Default: "Users"
 msgid "Meeting users"
 msgstr "Meeting users"
 
 #. Default: "Advice"
 msgid "MeetingAdvice"
 msgstr "Advice"
 
 #. Default: "Category"
 msgid "MeetingCategory"
-msgstr ""
+msgstr "Category"
 
 #. Default: "Meetings"
 msgid "Meetings"
 msgstr "Meetings"
 
 #. Default: "Modified since (in days, default to 30 days)"
 msgid "Modified since (in days, default to 30 days)"
@@ -739,22 +727,30 @@
 msgid "None"
 msgstr "None"
 
 #. Default: "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 msgid "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 msgstr "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 
+#. Default: "Not completed votes"
+msgid "Not completed votes"
+msgstr "Not completed votes"
+
 #. Default: "Not present type"
 msgid "Not present type"
 msgstr "Not present type"
 
 #. Default: "Not voter"
 msgid "Not voter"
 msgstr "Not voter"
 
+#. Default: "Nothing selected in the configuration to be displayed."
+msgid "Nothing selected in the configuration to be displayed."
+msgstr "Nothing selected in the configuration to be displayed."
+
 #. Default: "Nothing to display when item is not presented into a meeting."
 msgid "Nothing to display when item is not presented into a meeting."
 msgstr "Nothing to display when item is not presented into a meeting."
 
 #. Default: "Nothing to display."
 msgid "Nothing to display."
 msgstr "Nothing to display."
@@ -783,14 +779,18 @@
 msgid "Ordered groups"
 msgstr "Ordered groups"
 
 #. Default: "Original meeting signatory"
 msgid "Original meeting signatory"
 msgstr "Original meeting signatory"
 
+#. Default: "Original position"
+msgid "Original position"
+msgstr "Original position"
+
 #. Default: "POD template to annex"
 msgid "POD template to annex"
 msgstr "POD template to annex"
 
 #. Default: "Please check item number ${item_number} at ${item_url}."
 msgid "Please check item number ${item_number} at ${item_url}."
 msgstr "Please check item number ${item_number} at ${item_url}."
@@ -823,23 +823,14 @@
 msgid "PloneMeeting_inAndOutMoves"
 msgstr "Assembly in and out movements"
 
 #. Default: "Observations"
 msgid "PloneMeeting_itemObservations"
 msgstr "Observations"
 
-#. Default: "Observations"
-msgid "PloneMeeting_itemObservations2"
-msgstr "Observations"
-
-# MeetingGroup
-#. Default: "Absents"
-msgid "PloneMeeting_label_absents"
-msgstr "Absents (not excused)"
-
 #. Default: "Acronym"
 msgid "PloneMeeting_label_acronym"
 msgstr "Acronym"
 
 #. Default: "Confidential advice annexes are visible for"
 msgid "PloneMeeting_label_adviceAnnexConfidentialVisibleFor"
 msgstr "PloneMeeting_label_adviceAnnexConfidentialVisibleFor"
@@ -876,50 +867,26 @@
 msgid "PloneMeeting_label_annexToPrintMode"
 msgstr "PloneMeeting_label_annexToPrintMode"
 
 #. Default: "Answers"
 msgid "PloneMeeting_label_answerers"
 msgstr "Answers"
 
-#. Default: "Meeting approval date"
-msgid "PloneMeeting_label_approvalDate"
-msgstr "Meeting approval date"
-
 #. Default: "As copy group on"
 msgid "PloneMeeting_label_asCopyGroupOn"
 msgstr "As copy group on"
 
-#. Default: "Default assembly"
-msgid "PloneMeeting_label_assembly"
-msgstr "Default assembly"
-
-#. Default: "Default assembly staves"
-msgid "PloneMeeting_label_assemblyStaves"
-msgstr "Default assembly staves"
-
 #. Default: "Associated group(s)"
 msgid "PloneMeeting_label_associatedGroups"
 msgstr "Associated group(s)"
 
-#. Default: "Attendees"
-msgid "PloneMeeting_label_attendees"
-msgstr "Attendees"
-
-#. Default: "Authority notice"
-msgid "PloneMeeting_label_authorityNotice"
-msgstr "Authority notice"
-
 #. Default: "Columns to display for items available for a meeting"
 msgid "PloneMeeting_label_availableItemsListVisibleColumns"
 msgstr "Columns to display for items available for a meeting"
 
-#. Default: "Items"
-msgid "PloneMeeting_label_body"
-msgstr "Items"
-
 #. Default: "Default value for the \"budget information\" field"
 msgid "PloneMeeting_label_budgetDefault"
 msgstr "Default value for the \"budget information\" field"
 
 #. Default: "Budgetary informations"
 msgid "PloneMeeting_label_budgetInfos"
 msgstr "Budgetary informations"
@@ -948,14 +915,18 @@
 msgid "PloneMeeting_label_classifier"
 msgstr "Classifier"
 
 #. Default: "Observations for the committee"
 msgid "PloneMeeting_label_committeeObservations"
 msgstr "Observations for the committee"
 
+#. Default: "Committees"
+msgid "PloneMeeting_label_committees"
+msgstr "Committees"
+
 #. Default: "Completeness"
 msgid "PloneMeeting_label_completeness"
 msgstr "Completeness"
 
 #. Default: "Group of meeting configurations"
 msgid "PloneMeeting_label_configGroup"
 msgstr "Group of meeting configurations"
@@ -972,18 +943,14 @@
 msgid "PloneMeeting_label_configVersion"
 msgstr "Identifier of this meeting configuration"
 
 #. Default: "Contents to keep when item sent to another configuration"
 msgid "PloneMeeting_label_contentsKeptOnSentToOtherMC"
 msgstr "Contents to keep when item sent to another configuration"
 
-#. Default: "Meeting convocation date"
-msgid "PloneMeeting_label_convocationDate"
-msgstr "Convocation date"
-
 #. Default: "Copy groups"
 msgid "PloneMeeting_label_copyGroups"
 msgstr "Copy groups"
 
 #. Default: "Css classes to hide"
 msgid "PloneMeeting_label_cssClassesToHide"
 msgstr "Css classes to hide"
@@ -1000,26 +967,14 @@
 msgid "PloneMeeting_label_dashboardMeetingAvailableItemsFilters"
 msgstr "Advanced filters to show on \"Available items\""
 
 #. Default: "Advanced filters to show on \"Items of a meeting\""
 msgid "PloneMeeting_label_dashboardMeetingLinkedItemsFilters"
 msgstr "Advanced filters to show on \"Items of a meeting\""
 
-#. Default: "Date"
-msgid "PloneMeeting_label_date"
-msgstr "Date"
-
-#. Default: "Deadline for validating late items"
-msgid "PloneMeeting_label_deadlineFreeze"
-msgstr "Deadline for validating late items"
-
-#. Default: "Deadline for validating items"
-msgid "PloneMeeting_label_deadlinePublish"
-msgstr "Deadline for validating items"
-
 #. Default: "Decision"
 msgid "PloneMeeting_label_decision"
 msgstr "Decision"
 
 #. Default: "Decision (end)"
 msgid "PloneMeeting_label_decisionEnd"
 msgstr "Decision (end)"
@@ -1056,26 +1011,18 @@
 msgid "PloneMeeting_label_delayUnavailableEndDays"
 msgstr "Delay can not end following days"
 
 #. Default: "Description"
 msgid "PloneMeeting_label_description"
 msgstr "Description"
 
-#. Default: "Description in the second language"
-msgid "PloneMeeting_label_description2"
-msgstr "Description in the second language"
-
 #. Default: "Detailed description"
 msgid "PloneMeeting_label_detailedDescription"
 msgstr "Detailed description"
 
-#. Default: "Detailed description"
-msgid "PloneMeeting_label_detailedDescription2"
-msgstr "Detailed description"
-
 #. Default: "Display available items to"
 msgid "PloneMeeting_label_displayAvailableItemsTo"
 msgstr "Display available items to"
 
 #. Default: "Emergency"
 msgid "PloneMeeting_label_emergency"
 msgstr "Emergency"
@@ -1100,46 +1047,30 @@
 msgid "PloneMeeting_label_enableScanDocs"
 msgstr "Enable documents scanning"
 
 #. Default: "Enable user preferences"
 msgid "PloneMeeting_label_enableUserPreferences"
 msgstr "Enable user preferences"
 
-#. Default: "Effective end date and hour"
-msgid "PloneMeeting_label_endDate"
-msgstr "Effective end date and hour"
+#. Default: "Enabled annexes batch actions"
+msgid "PloneMeeting_label_enabledAnnexesBatchActions"
+msgstr "Enabled annexes batch actions"
 
 #. Default: "Enforce advice mandatoriness"
 msgid "PloneMeeting_label_enforceAdviceMandatoriness"
 msgstr "Enforce advice mandatoriness"
 
-#. Default: "Excused"
-msgid "PloneMeeting_label_excused"
-msgstr "Excused"
-
-#. Default: "Extraordinary session?"
-msgid "PloneMeeting_label_extraordinarySession"
-msgstr "Extraordinary session?"
-
-#. Default: "Number of the first item contained in this meeting"
-msgid "PloneMeeting_label_firstItemNumber"
-msgstr "Number of the first item contained in this meeting"
-
 #. Default: "First linked vote values"
 msgid "PloneMeeting_label_firstLinkedVoteUsedVoteValues"
 msgstr "First linked vote values"
 
 #. Default: "Name of the folder linked to this configuration"
 msgid "PloneMeeting_label_folderTitle"
 msgstr "Name of the folder linked to this configuration"
 
-#. Default: "Default deadline for validating late items for a given meeting"
-msgid "PloneMeeting_label_freezeDeadlineDefault"
-msgstr "Default deadline for validating late items for a given meeting"
-
 #. Default: "Email of the functional administrator"
 msgid "PloneMeeting_label_functionalAdminEmail"
 msgstr "Email of the functional administrator"
 
 #. Default: "Name of the functional administrator"
 msgid "PloneMeeting_label_functionalAdminName"
 msgstr "Name of the functional administrator"
@@ -1180,18 +1111,14 @@
 msgid "PloneMeeting_label_historizeItemDataWhenAdviceIsGiven"
 msgstr "Historize item data when an advice is given"
 
 #. Default: "Item attributes for which history must be kept"
 msgid "PloneMeeting_label_historizedItemAttributes"
 msgstr "Item attributes for which history must be kept"
 
-#. Default: "Meeting attributes for which history must be kept"
-msgid "PloneMeeting_label_historizedMeetingAttributes"
-msgstr "Meeting attributes for which history must be kept"
-
 #. Default: "Holidays"
 msgid "PloneMeeting_label_holidays"
 msgstr "Holidays"
 
 #. Default: "Include groups in charge defined on category"
 msgid "PloneMeeting_label_includeGroupsInChargeDefinedOnCategory"
 msgstr "Include groups in charge defined on category"
@@ -1369,37 +1296,33 @@
 msgid "PloneMeeting_label_itemWithGivenAdviceIsNotDeletable"
 msgstr "An item containing given advice is not deletable"
 
 #. Default: "Workflow that dictates the life cycle of every item into this configuration"
 msgid "PloneMeeting_label_itemWorkflow"
 msgstr "Workflow that dictates the life cycle of every item into this configuration"
 
-#. Default: "Items"
-msgid "PloneMeeting_label_items"
-msgstr "Items"
-
 #. Default: "Columns to display for items within a meeting"
 msgid "PloneMeeting_label_itemsListVisibleColumns"
 msgstr "Columns to display for items within a meeting"
 
 #. Default: "Fields of the items to show/hide in the dashboards"
 msgid "PloneMeeting_label_itemsListVisibleFields"
 msgstr "Fields of the items to show/hide in the dashboards"
 
 #. Default: "Fields to display on not visible linked items"
 msgid "PloneMeeting_label_itemsNotViewableVisibleFields"
-msgstr ""
+msgstr "Fields to display on not visible linked items"
 
 #. Default: "Fields to display on not visible linked items if"
 msgid "PloneMeeting_label_itemsNotViewableVisibleFieldsTALExpr"
-msgstr ""
+msgstr "Fields to display on not visible linked items if"
 
 #. Default: "Fields to display on visible linked items"
 msgid "PloneMeeting_label_itemsVisibleFields"
-msgstr ""
+msgstr "Fields to display on visible linked items"
 
 #. Default: "Keep access to item when an advice"
 msgid "PloneMeeting_label_keepAccessToItemWhenAdvice"
 msgstr "Keep access to item when an advice"
 
 #. Default: "Keep info \"to print?\" of annexes when duplicating items"
 msgid "PloneMeeting_label_keepOriginalToPrintOfClonedItems"
@@ -1469,18 +1392,14 @@
 msgid "PloneMeeting_label_meetingColumns"
 msgstr "Columns to display in lists of meetings"
 
 #. Default: "Interface allowing to use a specific Zope3 adapter for modifying the conditions defined on the transitions of the meeting workflow"
 msgid "PloneMeeting_label_meetingConditionsInterface"
 msgstr "Interface allowing to use a specific Zope3 adapter for modifying the conditions defined on the transitions of the meeting workflow"
 
-#. Default: "Identifier of the configuration's version that is linked to this meeting"
-msgid "PloneMeeting_label_meetingConfigVersion"
-msgstr "Identifier of the configuration's version that is linked to this meeting"
-
 #. Default: "Meeting configs to clone items to"
 msgid "PloneMeeting_label_meetingConfigsToCloneTo"
 msgstr "Meeting configs to clone items to"
 
 #. Default: "Title of the folder created in each user folder"
 msgid "PloneMeeting_label_meetingFolderTitle"
 msgstr "Title of the folder created in each user folder"
@@ -1497,58 +1416,38 @@
 msgid "PloneMeeting_label_meetingManagersNotesEnd"
 msgstr "MeetingManagers notes (end)"
 
 #. Default: "MeetingManagers notes (suite)"
 msgid "PloneMeeting_label_meetingManagersNotesSuite"
 msgstr "MeetingManagers notes (suite)"
 
-#. Default: "Meeting number (sequence number automatically attributed)"
-msgid "PloneMeeting_label_meetingNumber"
-msgstr "Meeting number (sequence number automatically attributed)"
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations"
-msgstr "Observations"
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations2"
-msgstr "Observations"
-
 #. Default: "States of the meeting to insert an item into from everywhere"
 msgid "PloneMeeting_label_meetingPresentItemWhenNoCurrentMeetingStates"
 msgstr "States of the meeting to insert an item into from everywhere"
 
 #. Default: "Meeting transition that triggers the insertion of this item as a recurring item"
 msgid "PloneMeeting_label_meetingTransitionInsertingMe"
 msgstr "Meeting transition that triggers the insertion of this item as a recurring item"
 
 #. Default: "Workflow that dictates the life cycle of every meeting into this configuration"
 msgid "PloneMeeting_label_meetingWorkflow"
 msgstr "Workflow that dictates the life cycle of every meeting into this configuration"
 
-#. Default: "End date for meeting first part"
-msgid "PloneMeeting_label_midDate"
-msgstr "End date for meeting first part"
-
 #. Default: "Model adaptations"
 msgid "PloneMeeting_label_modelAdaptations"
 msgstr "Model adaptations"
 
 #. Default: "Motivation"
 msgid "PloneMeeting_label_motivation"
 msgstr "Motivation"
 
 #. Default: "Next linked votes values"
 msgid "PloneMeeting_label_nextLinkedVotesUsedVoteValues"
 msgstr "Next linked votes values"
 
-#. Default: "Non attendees"
-msgid "PloneMeeting_label_nonAttendees"
-msgstr "Non attendees"
-
 #. Default: "Actions to execute on items of a meeting when a transition is triggered on that meeting"
 msgid "PloneMeeting_label_onMeetingTransitionItemActionToExecute"
 msgstr "Actions à exécuter sur les points d'une séance lorsqu'une transition est déclenchée sur cette séance"
 
 #. Default: "Transforms to apply to rich text fields of an item after a workflow transition"
 msgid "PloneMeeting_label_onTransitionFieldTransforms"
 msgstr "Transforms to apply to rich text fields of an item after a workflow transition"
@@ -1565,14 +1464,18 @@
 msgid "PloneMeeting_label_oralQuestion"
 msgstr "Oral question ?"
 
 #. Default: "Associated organizations order"
 msgid "PloneMeeting_label_orderedAssociatedOrganizations"
 msgstr "Associated organizations order"
 
+#. Default: "Attendees selectable for committees"
+msgid "PloneMeeting_label_orderedCommitteeContacts"
+msgstr "Attendees selectable for committees"
+
 #. Default: "Selectable assembly members"
 msgid "PloneMeeting_label_orderedContacts"
 msgstr "Selectable assembly members"
 
 #. Default: "Ordered groups in charge"
 msgid "PloneMeeting_label_orderedGroupsInCharge"
 msgstr "Ordered groups in charge"
@@ -1597,18 +1500,14 @@
 msgid "PloneMeeting_label_otherMeetingConfigsClonableToPrivacy"
 msgstr "Leave unchecked if item is public"
 
 #. Default: "Owner of a annex decision may delete it when item is no more editable?"
 msgid "PloneMeeting_label_ownerMayDeleteAnnexDecision"
 msgstr "Owner of a annex decision may delete it when item is no more editable?"
 
-#. Default: "Place"
-msgid "PloneMeeting_label_place"
-msgstr "Place"
-
 #. Default: "Meeting places"
 msgid "PloneMeeting_label_places"
 msgstr "Meeting places"
 
 #. Default: "Poll type"
 msgid "PloneMeeting_label_pollType"
 msgstr "Poll type"
@@ -1621,42 +1520,18 @@
 msgid "PloneMeeting_label_powerAdvisersGroups"
 msgstr "Groups to consider as \"Power advisers\""
 
 #. Default: "Manage power observers"
 msgid "PloneMeeting_label_powerObservers"
 msgstr "Manage power observers"
 
-#. Default: "Date"
-msgid "PloneMeeting_label_preMeetingDate"
-msgstr "Date"
-
-#. Default: "Default date for the pre-meeting"
-msgid "PloneMeeting_label_preMeetingDateDefault"
-msgstr "Default date for the pre-meeting"
-
-#. Default: "Place"
-msgid "PloneMeeting_label_preMeetingPlace"
-msgstr "Place"
-
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations"
-msgstr "Observations for the preparatory meeting"
-
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations2"
-msgstr "Observations for the preparatory meeting"
-
 #. Default: "Previous item"
 msgid "PloneMeeting_label_predecessor"
 msgstr "Previous item"
 
-#. Default: "Predefined title in the second language"
-msgid "PloneMeeting_label_predefinedTitle2"
-msgstr "Predefined title in the second language"
-
 #. Default: "Preferred meeting"
 msgid "PloneMeeting_label_preferredMeeting"
 msgstr "Preferred meeting"
 
 #. Default: "Privacy"
 msgid "PloneMeeting_label_privacy"
 msgstr "Privacy"
@@ -1665,38 +1540,26 @@
 msgid "PloneMeeting_label_proposingGroup"
 msgstr "Proposing group"
 
 #. Default: "Proposing group (Group in charge)"
 msgid "PloneMeeting_label_proposingGroupWithGroupInCharge"
 msgstr "Proposing group (Group in charge)"
 
-#. Default: "Observations for public meeting"
-msgid "PloneMeeting_label_publicMeetingObservations"
-msgstr "Observations for public meeting"
-
 #. Default: "Public URL"
 msgid "PloneMeeting_label_publicUrl"
 msgstr "Public URL"
 
-#. Default: "Default deadline for validating items for a given meeting"
-msgid "PloneMeeting_label_publishDeadlineDefault"
-msgstr "Default deadline for validating items for a given meeting"
-
 #. Default: "Questions"
 msgid "PloneMeeting_label_questioners"
 msgstr "Questions"
 
 #. Default: "Item states into which events will be recorded in item's history"
 msgid "PloneMeeting_label_recordItemHistoryStates"
 msgstr "Item states into which events will be recorded in item's history"
 
-#. Default: "Meeting states into which events will be recorded in meeting's history"
-msgid "PloneMeeting_label_recordMeetingHistoryStates"
-msgstr "Meeting states into which events will be recorded in meeting's history"
-
 #. Default: "Redirect to the next meeting"
 msgid "PloneMeeting_label_redirectToNextMeeting"
 msgstr "Redirect to the next meeting"
 
 #. Default: "Remove annexes previews on meeting closure"
 msgid "PloneMeeting_label_removeAnnexesPreviewsOnMeetingClosure"
 msgstr "Remove annexes previews on meeting closure"
@@ -1713,30 +1576,30 @@
 msgid "PloneMeeting_label_restrictAccessToSecretItemsTo"
 msgstr "Restrict access to secret items to"
 
 #. Default: "\"Restrict users\" mode"
 msgid "PloneMeeting_label_restrictUsers"
 msgstr "\"Restrict users\" mode"
 
-#. Default: "Observations for the secret meeting"
-msgid "PloneMeeting_label_secretMeetingObservations"
-msgstr "Observations for the secret meeting"
-
 #. Default: "Selectable advisers"
 msgid "PloneMeeting_label_selectableAdvisers"
 msgstr "Selectable advisers"
 
 #. Default: "Groups that can be in copy for an item"
 msgid "PloneMeeting_label_selectableCopyGroups"
 msgstr "Groups that can be in copy for an item"
 
 #. Default: "Selectable privacies"
 msgid "PloneMeeting_label_selectablePrivacies"
 msgstr "Selectable privacies"
 
+#. Default: "Restrict selectable redefined position types to following positions"
+msgid "PloneMeeting_label_selectableRedefinedPositionTypes"
+msgstr "Restrict selectable redefined position types to following positions"
+
 #. Default: "Is group selectable in the plonegroup configuration panel?"
 msgid "PloneMeeting_label_selectable_for_plonegroup"
 msgstr "Is group selectable in the plonegroup configuration panel?"
 
 #. Default: "Send to authority?"
 msgid "PloneMeeting_label_sendToAuthority"
 msgstr "Send to authority?"
@@ -1749,26 +1612,18 @@
 msgid "PloneMeeting_label_showItemKeywordsTargets"
 msgstr "Show possible targets for item keywords"
 
 #. Default: "Signatories"
 msgid "PloneMeeting_label_signatories"
 msgstr "Signatories"
 
-#. Default: "Default signatures"
-msgid "PloneMeeting_label_signatures"
-msgstr "Default signatures"
-
 #. Default: "Sort the tags alphabetically"
 msgid "PloneMeeting_label_sortAllItemTags"
 msgstr "Sort the tags alphabetically"
 
-#. Default: "Effective start date and hour"
-msgid "PloneMeeting_label_startDate"
-msgstr "Effective start date and hour"
-
 #. Default: "Meeting file sub types"
 msgid "PloneMeeting_label_subTypes"
 msgstr "Meeting file sub types"
 
 #. Default: "Taken over by"
 msgid "PloneMeeting_label_takenOverBy"
 msgstr "Taken over by"
@@ -1777,23 +1632,14 @@
 msgid "PloneMeeting_label_templateUsingGroups"
 msgstr "Restrict usage of this template to following groups"
 
 #. Default: "Checklist"
 msgid "PloneMeeting_label_textCheckList"
 msgstr "Checklist"
 
-# Meeting
-#. Default: "Title"
-msgid "PloneMeeting_label_title"
-msgstr "Title"
-
-#. Default: "Title in the second language"
-msgid "PloneMeeting_label_title2"
-msgstr "Title in the second language"
-
 #. Default: "To discuss ?"
 msgid "PloneMeeting_label_toDiscuss"
 msgstr "To discuss ?"
 
 #. Default: "Default value of the \"toDiscuss\" attribute for normal items"
 msgid "PloneMeeting_label_toDiscussDefault"
 msgstr "Default value of the \"toDiscuss\" attribute for normal items"
@@ -1914,37 +1760,37 @@
 msgid "PloneMeeting_label_xhtmlTransformTypes"
 msgstr "Rich text transform types"
 
 #. Default: "Reinitialise meeting number every year?"
 msgid "PloneMeeting_label_yearlyInitMeetingNumber"
 msgstr "Reinitialise meeting number every year?"
 
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations"
-msgstr "Observations"
-
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations2"
-msgstr "Observations"
-
 #. Default: "Notes"
 msgid "PloneMeeting_notes"
 msgstr "Notes"
 
 #. Default: "Document templates"
 msgid "PodTemplates"
 msgstr "Document templates"
 
 #. Default: "Position type"
 msgid "Position type"
 msgstr "Position type"
 
+#. Default: "Position type to use"
+msgid "Position type to use"
+msgstr "Position type to use"
+
 #. Default: "Position type to use as label for the signature."
 msgid "Position type to use as label for the signature."
-msgstr ""
+msgstr "Position type to use as label for the signature."
+
+#. Default: "Position type to use for the attendee on this item."
+msgid "Position type to use for the attendee on this item."
+msgstr "Position type to use for the attendee on this item."
 
 #. Default: "Preview detailed advice"
 msgid "Preview detailed advice"
 msgstr "Preview detailed advice"
 
 #. Default: "Preview of annexes were deleted upon meeting closure."
 msgid "Preview of annexes were deleted upon meeting closure."
@@ -1955,14 +1801,26 @@
 msgid "Previous review state"
 msgstr "Previous review state"
 
 #. Default: "Recurring items"
 msgid "RecurringItems"
 msgstr "Recurring items"
 
+#. Default: "Redefine position for this attendee for this item"
+msgid "Redefine position for this attendee for this item"
+msgstr "Redefine position for this attendee for this item"
+
+#. Default: "Redefined attendee position was removed."
+msgid "Redefined attendee position was removed."
+msgstr "Redefined attendee position was removed."
+
+#. Default: "Redefined position"
+msgid "Redefined position"
+msgstr "Redefined position"
+
 #. Default: "References of contained items have been updated."
 msgid "References of contained items have been updated."
 msgstr "References of contained items have been updated."
 
 #. Default: "Reinitiatlize delay"
 msgid "Reinitiatlize delay"
 msgstr "Reinitiatlize delay"
@@ -1979,14 +1837,18 @@
 msgid "Remove inherited advice"
 msgstr "Remove inherited advice"
 
 #. Default: "Remove inherited advice and ask advice locally"
 msgid "Remove inherited advice and ask advice locally"
 msgstr "Remove inherited advice and ask advice locally"
 
+#. Default: "Remove redefined attendee position for this item"
+msgid "Remove redefined attendee position for this item"
+msgstr "Remove redefined attendee position for this item"
+
 #. Default: "Represented organizations"
 msgid "Represented organizations"
 msgstr "Represented organizations"
 
 #. Default: "Searches"
 msgid "Searches"
 msgstr "Searches"
@@ -2037,15 +1899,19 @@
 
 #. Default: "Signature number"
 msgid "Signature number"
 msgstr "Signature number"
 
 #. Default: "Signature position type"
 msgid "Signature position type"
-msgstr ""
+msgstr "Signature position type"
+
+#. Default: "Specify a number to which this will be applied. Field default is current item number."
+msgid "Specify a number to which this will be applied. Field default is current item number."
+msgstr "Specify a number to which this will be applied. Field default is current item number."
 
 #. Default: "state"
 msgid "State"
 msgstr "State"
 
 #. Default: "Style templates"
 msgid "Style templates"
@@ -2090,14 +1956,18 @@
 msgstr "The item you tried to take over was already taken over in between by ${fullname}. You can take it over now if you are sure that the other user do not handle it."
 
 # plone.app.querystring
 #. Default: "The item, advice or meeting previous review state"
 msgid "The item, advice or meeting previous review state"
 msgstr "The item, advice or meeting previous review state"
 
+#. Default: "The position of this attendee was changed for the ${number} following item(s)"
+msgid "The position of this attendee was changed for the ${number} following item(s)"
+msgstr "The position of this attendee was changed for the ${number} following item(s)"
+
 #. Default: "There was an error during annex conversion, please contact system administrator."
 msgid "There was an error during annex conversion, please contact system administrator."
 msgstr "There was an error during annex conversion, please contact system administrator."
 
 #. Default: "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
 msgid "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
 msgstr "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
@@ -2138,18 +2008,14 @@
 msgid "This automatic advice has been asked by the application (shown by his title not being between brackets)"
 msgstr "This automatic advice has been asked by the application (shown by his title not being between brackets)"
 
 #. Default: "This copy group was set automatically by the application"
 msgid "This copy group was set automatically by the application"
 msgstr "This copy group was set automatically by the application"
 
-#. Default: "This is an extract of the comment, access full comment if necessary..."
-msgid "This is an extract of the comment, access full comment if necessary..."
-msgstr "This is an extract of the comment, access full comment if necessary..."
-
 #. Default: "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 msgid "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 msgstr "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 
 #. Default: "This label can not be removed as it is used by some items, for example ${item_url}"
 msgid "This label can not be removed as it is used by some items, for example ${item_url}"
 msgstr "This label can not be removed as it is used by some items, for example ${item_url}"
@@ -2231,17 +2097,17 @@
 msgid "Votes are not completed for following ${number} ${polltype} item(s)"
 msgstr "Votes are not completed for following ${number} ${polltype} item(s)"
 
 #. Default: "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 msgid "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 msgstr "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 
-#. Default: "You cannot delete the default item template, but you can deactivate it if necessary!"
-msgid "You cannot delete the default item template, but you can deactivate it if necessary!"
-msgstr "You cannot delete the default item template, but you can deactivate it if necessary!"
+#. Default: "You cannot delete or move the default item template, but you can deactivate it if necessary!"
+msgid "You cannot delete or move the default item template, but you can deactivate it if necessary!"
+msgstr "You cannot delete or move the default item template, but you can deactivate it if necessary!"
 
 #. Default: "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 msgid "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 msgstr "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 
 #. Default: "Not grouped meeting configurations"
 msgid "_no_config_group_"
@@ -2471,78 +2337,78 @@
 msgid "annexAdded_mail_subject"
 msgstr "${meetingConfigTitle} - ${meetingTitle} - An annex was just added to an item."
 
 #. Default: "If an annex is marked as \"Confidential\" by a meeting manager, following selected profiles will not be able to see it."
 msgid "annex_confidential_for_descr"
 msgstr "If an annex is marked as \"Confidential\" by a meeting manager, following selected profiles will not be able to see it."
 
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item."
-msgid "annex_is_confidential_no"
-msgstr "The annex is not confidential and will be visible by everybody who has access to this item."
-
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item.  Click on the image to set it as confidential."
-msgid "annex_is_confidential_no_edit"
-msgstr "The annex is not confidential and will be visible by everybody who has access to this item.  Click on the image to set it as confidential."
-
-#. Default: "The annex is confidential."
-msgid "annex_is_confidential_yes"
-msgstr "The annex is confidential."
-
-#. Default: "The annex is confidential.  Click on the image to set it as not confidential."
-msgid "annex_is_confidential_yes_edit"
-msgstr "The annex is confidential.  Click on the image to set it as not confidential."
-
 #. Default: "The item was duplicated but the annex with title \"${annexTitle}\" could not be kept because it was not possible to find a corresponding annex type in the destination meeting configuration, please contact system administrator."
 msgid "annex_not_kept_because_no_available_annex_type_warning"
 msgstr "The item was duplicated but the annex with title \"${annexTitle}\" could not be kept because it was not possible to find a corresponding annex type in the destination meeting configuration, please contact system administrator."
 
 #. Default: "The item was duplicated but the annex with title \"${annexTitle}\" was not kept because using a scan_id, please contact system administrator."
 msgid "annex_not_kept_because_using_scan_id"
 msgstr "The item was duplicated but the annex with title \"${annexTitle}\" was not kept because using a scan_id, please contact system administrator."
 
 #. Default: "Select for each optional annexes attributes which are only displayed or editable by MeetingManagers.  If an attribute is only displayed to MeetingManagers it will be automatically considered as only editable by MeetingManagers as well."
 msgid "annex_restrict_shown_and_editable_attributes_descr"
 msgstr "Select for each optional annexes attributes which are only displayed or editable by MeetingManagers.  If an attribute is only displayed to MeetingManagers it will be automatically considered as only editable by MeetingManagers as well."
 
+#. Default: "Confidential"
+msgid "annex_term_confidential"
+msgstr "Confidential"
+
+#. Default: "Not confidential"
+msgid "annex_term_not_confidential"
+msgstr "Not confidential"
+
+#. Default: "Not publishable"
+msgid "annex_term_not_publishable"
+msgstr "Not publishable"
+
+#. Default: "Not to print"
+msgid "annex_term_not_to_print"
+msgstr "Not to print"
+
+#. Default: "Not to sign"
+msgid "annex_term_not_to_sign"
+msgstr "Not to sign"
+
+#. Default: "Publishable"
+msgid "annex_term_publishable"
+msgstr "Publishable"
+
+#. Default: "Signed"
+msgid "annex_term_signed"
+msgstr "Signed"
+
+#. Default: "To print"
+msgid "annex_term_to_print"
+msgstr "To print"
+
+#. Default: "To sign"
+msgid "annex_term_to_sign"
+msgstr "To sign"
+
 #. Default: "Title"
 msgid "annex_title"
 msgstr "Title"
 
-#. Default: "The annex is not printable because it can not be converted (unsupported format or error during conversion).  Please use common office formats."
-msgid "annex_to_print_disabled"
-msgstr "The annex is not printable because it can not be converted (unsupported format or error during conversion).  Please use common office formats."
-
 #. Default: "Automated (annexes are printed by the application)"
 msgid "annex_to_print_mode_automated"
 msgstr "Automated (annexes are printed by the application)"
 
 #. Default: "If print functionnality is enabled for annexes and an annex is set \"to print\", select here the to print mode that will be used : \"Manual\", means that the to print is just defined for information and that the printing process will be handled manually or \"Automated\", in this case, the application will generate a printable format for the annex (converted to images) so it can be inserted in a generated document."
 msgid "annex_to_print_mode_descr"
 msgstr "If print functionnality is enabled for annexes and an annex is set \"to print\", select here the to print mode that will be used : 'Manual', means that the to print is just defined for information and that the printing process will be handled manually or 'Automated', in this case, the application will generate a printable format for the annex (converted to images) so it can be inserted in a generated document."
 
 #. Default: "For information (annexes are printed manually)"
 msgid "annex_to_print_mode_info"
 msgstr "For information (annexes are printed manually)"
 
-#. Default: "The annex will not be printed."
-msgid "annex_to_print_no"
-msgstr "The annex will not be printed."
-
-#. Default: "The annex will not be printed. Click on the image to print it."
-msgid "annex_to_print_no_edit"
-msgstr "The annex will not be printed. Click on the image to print it."
-
-#. Default: "The annex will be printed."
-msgid "annex_to_print_yes"
-msgstr "The annex will be printed."
-
-#. Default: "The annex will be printed. Click on the image not to print it."
-msgid "annex_to_print_yes_edit"
-msgstr "The annex will be printed. Click on the image not to print it."
-
 #. Default: "Annex type"
 msgid "annex_type"
 msgstr "Annex type"
 
 #. Default: "Every item may be associated with a series of annexes. Some annexes may be specifically tied to the decision taken on the item. You can consult and modify here the annex types that are defined within this meeting configuration. An annex type is defined by a title, an icon (preferably of 16x16 pixels) and a predefined title. When users want to associate an annex to an item, they may choose, in a dropdown list, an annex type among those defined here and upload a file."
 msgid "annex_types_descr"
 msgstr "Every item may be associated with a series of annexes. Some annexes may be specifically tied to the decision taken on the item. You can consult and modify here the annex types that are defined within this meeting configuration. An annex type is defined by a title, an icon (preferably of 16x16 pixels) and a predefined title. When users want to associate an annex to an item, they may choose, in a dropdown list, an annex type among those defined here and upload a file."
@@ -2567,25 +2433,17 @@
 msgid "annexes_preview_disabled"
 msgstr "<span style='color: red;'>Annexes preview is disabled in the ${documentviewer_url}.</span>"
 
 #. Default: "<span style='color: green;'>Annexes preview is enabled in the ${documentviewer_url}.</span>"
 msgid "annexes_preview_enabled"
 msgstr "<span style='color: green;'>Annexes preview is enabled in the ${documentviewer_url}.</span>"
 
-#. Default: "Signed annexes"
-msgid "annexes_signed_term"
-msgstr "Signed annexes"
-
-#. Default: "Annexes to print"
-msgid "annexes_to_print_term"
-msgstr "Annexes to print"
-
-#. Default: "Annexes to sign"
-msgid "annexes_to_sign_term"
-msgstr "Annexes to sign"
+#. Default: "Annexes types are hidden by default, you can ${force_display} of it (may take some time)."
+msgid "annexes_types_force_display_descr"
+msgstr "Annexes types are hidden by default, you can ${force_display} of it (may take some time)."
 
 #. Default: "Application users"
 msgid "app_users"
 msgstr "Application users"
 
 #. Default: "Are you sure?"
 msgid "are_you_sure"
@@ -2619,18 +2477,14 @@
 msgid "assemblyMember"
 msgstr "Assembly member"
 
 #. Default: "Absents as defined on the linked meeting"
 msgid "assembly_absents_defined_on_meeting"
 msgstr "Absents as defined on the linked meeting"
 
-#. Default: "Define here people that were absents (not excused) for the meeting"
-msgid "assembly_absents_meeting_descr"
-msgstr "Define here people that were absents (not excused) for the meeting"
-
 #. Default: "Assembly and signatures"
 msgid "assembly_and_signatures"
 msgstr "Assembly and signatures"
 
 #. Default: "Assembly as defined on the linked meeting"
 msgid "assembly_defined_on_meeting"
 msgstr "Assembly as defined on the linked meeting"
@@ -2639,26 +2493,18 @@
 msgid "assembly_descr"
 msgstr "Define here the default assembly (for example you may type a list of names and first names separated by colons or new lines) that will be automatically selected on newly created meetings. If you want a more structured way to define attendees, absents and excused people on a meeting, do not fill this field, create, in the tab \"data\", special users having characteristic \"assembly member\" and select, in the same tab, \"attendees\", \"absents\" and/or \"excused\" attributes as attributes used for a meeting."
 
 #. Default: "Excused as defined on the linked meeting"
 msgid "assembly_excused_defined_on_meeting"
 msgstr "Excused as defined on the linked meeting"
 
-#. Default: "Define here people that were excused for the meeting"
-msgid "assembly_excused_meeting_descr"
-msgstr "Define here people that were excused for the meeting"
-
 #. Default: "Guests as defined on the linked meeting"
 msgid "assembly_guests_defined_on_meeting"
 msgstr "Guests as defined on the linked meeting"
 
-#. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
-msgid "assembly_meeting_descr"
-msgstr "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
-
 #. Default: "Using attribute(s) \"itemExcused\" and/or \"itemAbsents\" requires the use of attribute \"assembly\"."
 msgid "assembly_required"
 msgstr "Using attribute(s) \"itemExcused\" and/or \"itemAbsents\" requires the use of attribute \"assembly\"."
 
 #. Default: "Define here the default assembly staves (for example you may type a list of names and first names separated by colons or new lines) that will be automatically selected on newly created meetings."
 msgid "assembly_staves_descr"
 msgstr "Define here the default assembly staves (for example you may type a list of names and first names separated by colons or new lines) that will be automatically selected on newly created meetings."
@@ -2748,14 +2594,18 @@
 msgid "budgetimpacteditors"
 msgstr "Budget impact editors"
 
 #. Default: "You can not access this item"
 msgid "can_not_access_this_item"
 msgstr "You can not access this item"
 
+#. Default: "Assembly and signatures : you can not use same signature number several times."
+msgid "can_not_define_several_same_signature_number"
+msgstr "Assembly and signatures : you can not use same signature number several times."
+
 #. Default: "You can not define two rows for the same meeting configuration!"
 msgid "can_not_define_two_rows_for_same_meeting_config"
 msgstr "You can not define two rows for the same meeting configuration!"
 
 #. Default: "You can not remove/disable a function that is used by an item in the configuration.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_config_meetingitem"
 msgstr "You can not remove/disable a function that is used by an item in the configuration.  Please check ${item_url}."
@@ -2764,30 +2614,34 @@
 msgid "can_not_delete_plone_group_meetingconfig"
 msgstr "You can not remove/disable a function that is used by a parameter of a configuration.  Please check ${cfg_title}."
 
 #. Default: "You can not remove/disable a function that is used by an item in the application.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_meetingitem"
 msgstr "You can not remove/disable a function that is used by an item in the application.  Please check ${item_url}."
 
-#. Default: "You can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
 msgid "can_not_remove_attendee_redefined_on_items"
-msgstr "You can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
+msgstr "Assembly and signatures : you can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
 
-#. Default: "You can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
 msgid "can_not_remove_public_voter_voted_on_items"
-msgstr "You can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
+msgstr "Assembly and signatures : you can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
 
-#. Default: "You can not unselect a voter that already voted on a secret vote item."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a secret vote item."
 msgid "can_not_remove_secret_voter_voted_on_items"
-msgstr "You can not unselect a voter that already voted on a secret vote item."
+msgstr "Assembly and signatures : you can not unselect a voter that already voted on a secret vote item."
 
 #. Default: "This item can no more be returned to the meeting managers because the meeting is in a state not authorizing it (${meetingState})."
 msgid "can_not_return_to_meeting_because_of_meeting_state"
 msgstr "This item can no more be returned to the meeting managers because the meeting is in a state not authorizing it (${meetingState})."
 
+#. Default: "You can not select \"No committee\" and a committee."
+msgid "can_not_select_no_committee_and_committee"
+msgstr "You can not select \"No committee\" and a committee."
+
 #. Default: "You can not select an adviser that is already displayed on the item as an inherited advice.  If you need to ask this advice again, you need to remove the inherited advice (as a MeetingManager or a Manager) then select advice again."
 msgid "can_not_select_optional_adviser_same_group_as_inherited"
 msgstr "You can not select an adviser that is already displayed on the item as an inherited advice.  If you need to ask this advice again, you need to remove the inherited advice (as a MeetingManager or a Manager) then select advice again."
 
 #. Default: "You can not select several values for the same group.  Please select a single value for the same group among available ones."
 msgid "can_not_select_several_optional_advisers_same_group"
 msgstr "You can not select several values for the same group.  Please select a single value for the same group among available ones."
@@ -2820,18 +2674,14 @@
 msgid "categories_descr"
 msgstr "Every item, within this meeting configuration, can only belong to one category. Those categories are defined here (by a title and a description). The order into which they appear in this folder is important. Indeed, if we make the assumption that you desire it (it depends on a parameter you may modify in the \"data\" section), when an item is added to a meeting, it can be inserted at the end of the items belonging to the same category, those items being themselves inserted at a place that corresponds to the position of their category among the list of categories defined here. That being said, if you tell that you want to use the groups as categories (another parameter of the \"data\" section), the categories defined here will be ignored."
 
 #. Default: "the \"Folder contents view\""
 msgid "categories_folder_contents_view"
 msgstr "the \"Folder contents view\""
 
-#. Default: "force display"
-msgid "categories_force_display"
-msgstr "force display"
-
 #. Default: "You can ${force_display} of every categories (may take some time)."
 msgid "categories_force_display_descr"
 msgstr "You can ${force_display} of every categories (may take some time)."
 
 #. Default: "You may use the ${folder_contents_link} to manage elements order."
 msgid "categories_use_folder_contents"
 msgstr "You may use the ${folder_contents_link} to manage elements order."
@@ -2980,14 +2830,34 @@
 msgid "clone_to"
 msgstr "Clone to ${meetingConfigTitle}"
 
 #. Default: "Your configuration says can not correct this closed meeting, contact your system administrator if you want to change this."
 msgid "closed_meeting_not_correctable_by_config"
 msgstr "Your configuration says can not correct this closed meeting, contact your system administrator if you want to change this."
 
+#. Default: "${title} (${number}&nbsp;s.)"
+msgid "committee_title_with_abbr_suppl"
+msgstr "${title} (${number}&nbsp;s.)"
+
+#. Default: "${title} (${number}&nbsp;supplement)"
+msgid "committee_title_with_suppl"
+msgstr "${title} (${number}&nbsp;supplement)"
+
+#. Default: "Committees"
+msgid "committees"
+msgstr "Committees"
+
+#. Default: "Define committees that will be useable on meetings and items (you also need to enable \"Committees\" on the meeting in the [Data] tab). This will show a \"Committees\" table on the meeting and will be also managed on the item. <br />There are 2 ways to manage committees on the item, either manually or automatically:<ul><li>Manually: just define committees, this will create a multiselection box on the item and users may select it.  It is possible to use the column \"Restrict to\" to define which proposing groups will be able to select the committee;</li><li>Automatically: use the column \"Auto from\" to define which committees to associate to the item depending on proposing group, category or classifier. A MeetingManager is nevertheless able to edit the committee on the item.</li></ul>. These 2 ways are mutually exclusive, if you select values in the \"auto_from\" columb here under, the \"Automatic\" mode will be used."
+msgid "committees_descr"
+msgstr "Define committees that will be useable on meetings and items (you also need to enable \"Committees\" on the meeting in the [Data] tab). This will show a \"Committees\" table on the meeting and will be also managed on the item. <br />There are 2 ways to manage committees on the item, either manually or automatically:<ul><li>Manually: just define committees, this will create a multiselection box on the item and users may select it.  It is possible to use the column \"Restrict to\" to define which proposing groups will be able to select the committee;</li><li>Automatically: use the column \"Auto from\" to define which committees to associate to the item depending on proposing group, category or classifier. A MeetingManager is nevertheless able to edit the committee on the item.</li></ul>. These 2 ways are mutually exclusive, if you select values in the \"auto_from\" columb here under, the \"Automatic\" mode will be used."
+
+#. Default: "Using a \"Committees\" field requires the use of attribute \"Committees (committees)\"."
+msgid "committees_required"
+msgstr "Using a \"Committees\" field requires the use of attribute \"Committees (committees)\"."
+
 #. Default: "Complete"
 msgid "completeness_complete"
 msgstr "Complete"
 
 #. Default: "Evaluation asked again"
 msgid "completeness_evaluation_asked_again"
 msgstr "Evaluation asked again"
@@ -3072,14 +2942,21 @@
 msgid "copyGroups_mail_body"
 msgstr "The item is entitled \"${itemTitle}\". You can access this item here: ${objectUrl}."
 
 #. Default: "${meetingConfigTitle} - You have been carbon copied - ${itemTitle}"
 msgid "copyGroups_mail_subject"
 msgstr "${meetingConfigTitle} - You have been carbon copied - ${itemTitle}"
 
+#. Default: "These groups will have read access to the item in following states: ${states}.\nWhen icon is green, this means that copy groups have access to the item.\nWhen the label \"[auto]\" is displayed next to the group title, it means that the group was set as copy group automatically by the application."
+msgid "copy_groups_help_msg"
+msgstr ""
+"These groups will have read access to the item in following states: ${states}.\n"
+"When icon is green, this means that copy groups have access to the item.\n"
+"When the label \"[auto]\" is displayed next to the group title, it means that the group was set as copy group automatically by the application."
+
 #. Default: " "
 msgid "copy_groups_item_descr"
 msgstr "Select here groups that will be able to see this item"
 
 #. Default: "The cloned item could not be presented to a meeting in the \"${destMeetingConfigTitle}\" configuration, no suitable meeting could be found."
 msgid "could_not_present_item_no_meeting_accepting_items"
 msgstr "The cloned item could not be presented to a meeting in the \"${destMeetingConfigTitle}\" configuration, no suitable meeting could be found."
@@ -3266,14 +3143,34 @@
 msgid "delay_of_x_days"
 msgstr "Delay of ${delay} clear day(s)"
 
 #. Default: "Select here the days a computed delay can not ends with.  If a computed delay is ending on one of selected week day, the delay will be extend to next available day.  <span style='color: red;'>If you change this parameter, do not forget to run \"Update items and meetings\"!</span>"
 msgid "delay_unavailable_end_days_descr"
 msgstr "Select here the days a computed delay can not ends with.  If a computed delay is ending on one of selected week day, the delay will be extend to next available day.  <span style='color: red;'>If you change this parameter, do not forget to run \"Update items and meetings\"!</span>"
 
+#. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
+msgid "descr_assembly"
+msgstr "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
+
+#. Default: "<span style='color: red;'>WARNING, this field is managed by the application and it's value will be \"-1\" until the meeting is frozen, then it will be computed automatically. Do only change it manually when necessary (in general this should never happen). This field is only editable and viewable by meeting managers</span>"
+msgid "descr_config_field_reserved_to_meeting_managers"
+msgstr "<span style='color: red;'>WARNING, this field is managed by the application and it's value will be \"-1\" until the meeting is frozen, then it will be computed automatically. Do only change it manually when necessary (in general this should never happen). This field is only editable and viewable by meeting managers</span>"
+
+#. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
+msgid "descr_field_reserved_to_meeting_managers"
+msgstr "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
+
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
+msgid "descr_field_vieawable_by_everyone"
+msgstr "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
+
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
+msgid "descr_field_vieawable_by_everyone_once_meeting_decided"
+msgstr "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
+
 #. Default: "You are just able to see visible elements here. Please consult the \"manage\" box here opposite."
 msgid "description_only_see_visible_items"
 msgstr "You are just able to see visible elements here. Please consult the \"manage\" box here opposite."
 
 #. Default: "By default only MeetingManagers will see the available items panel on a meeting as long as the meeting is accepting items.  This let's you show this panel to selected profiles.  Note that if you enable this, the meeting view will be displayed slower."
 msgid "display_available_items_to_descr"
 msgstr "By default only MeetingManagers will see the available items panel on a meeting as long as the meeting is accepting items.  This let's you show this panel to selected profiles.  Note that if you enable this, the meeting view will be displayed slower."
@@ -3370,14 +3267,22 @@
 msgid "enable_scan_docs_descr"
 msgstr "Check this box if you use the documents scanning functionnality."
 
 #. Default: "If you check this box, users will be able to access a screen for modifying their preferences. While powerful, some may think it exposes too much complexity to users."
 msgid "enable_user_preferences_descr"
 msgstr "If you check this box, users will be able to access a screen for modifying their preferences. While powerful, some may think it exposes too much complexity to users."
 
+#. Default: "Select the batch actions that will be displayed on the table listing annexes"
+msgid "enabled_annexes_batch_actions_descr"
+msgstr "Select the batch actions that will be displayed on the table listing annexes"
+
+#. Default: "The meeting end date must occur after the start date and meeting date."
+msgid "end_date_before_meeting_date"
+msgstr "The meeting end date must occur after the start date and meeting date."
+
 #. Default: "When advice mandatoriness is enforced, an item can't be inserted into a meeting unless all mandatory advices are given and positive."
 msgid "enforce_advice_mandatoriness_descr"
 msgstr "When advice mandatoriness is enforced, an item can't be inserted into a meeting unless all mandatory advices are given and positive."
 
 #. Default: "You can not encode more than ${max_voters} voters."
 msgid "error_can_not_encode_more_than_max_voters"
 msgstr "You can not encode more than ${max_voters} voters."
@@ -3398,14 +3303,30 @@
 msgid "error_certified_signatures_invalid_dates"
 msgstr "Please make sure encoded dates are valid at row number ${row_number}.  Use format \"YYYY/MM/DD\", make sure date are valid and that date from is lower or equals to date to."
 
 #. Default: "Signatures must be ordered by signature number, please check and order signature using the arrows on the right of the table."
 msgid "error_certified_signatures_order"
 msgstr "Signatures must be ordered by signature number, please check and order signature using the arrows on the right of the table."
 
+#. Default: "You can not remove a configuration that was already used, removed configuration \"${committee_label}\" is used for example by item at ${url}.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committee_row_id_removed_already_used"
+msgstr "You can not remove a configuration that was already used, removed configuration \"${committee_label}\" is used for example by item at ${url}.  If you lost encoded values, just cancel edition and edit again correctly."
+
+#. Default: "You can not define values for the \"auto_from\" and \"using_groups\" columns, their use is multually exclusive.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committees_mutually_exclusive_auto_from_and_using_groups"
+msgstr "You can not define values for the \"auto_from\" and \"using_groups\" columns, their use is multually exclusive.  If you lost encoded values, just cancel edition and edit again correctly."
+
+#. Default: "Default poll type must be among used poll types"
+msgid "error_default_poll_type_must_be_among_used_poll_types"
+msgstr "Default poll type must be among used poll types"
+
+#. Default: "First linked vote used votes values must be among used vote values"
+msgid "error_first_linked_vote_used_vote_values_must_be_among_used_vote_values"
+msgstr "First linked vote used votes values must be among used vote values"
+
 #. Default: "You may not remove a list type that is currently used by an item, check for example : ${url}."
 msgid "error_list_types_identifier_removed_already_used"
 msgstr "You may not remove a list type that is currently used by an item, check for example : ${url}."
 
 #. Default: "You may not remove the default list types (\"normal\" and \"late\")."
 msgid "error_list_types_missing_default"
 msgstr "You may not remove the default list types (\"normal\" and \"late\")."
@@ -3414,14 +3335,22 @@
 msgid "error_list_types_same_identifier"
 msgstr "You may not use the same identifier several times."
 
 #. Default: "You may only use lowercase letters for identifier."
 msgid "error_list_types_wrong_identifier_format"
 msgstr "You may only use lowercase letters for identifier."
 
+#. Default: "Next linked votes used vote values must be among used vote values"
+msgid "error_next_linked_votes_used_vote_values_must_be_among_used_vote_values"
+msgstr "Next linked votes used vote values must be among used vote values"
+
+#. Default: "Some selected values are no more selectable (no more selected in the \"Ordered committees contacts\" field), please check value \"${hp_title}\".  You can not select \"No committee\" and a committee.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_value_removed_used_in_committees_field"
+msgstr "Some selected values are no more selectable (no more selected in the \"Ordered committees contacts\" field), please check value \"${hp_title}\".  You can not select \"No committee\" and a committee.  If you lost encoded values, just cancel edition and edit again correctly."
+
 #. Default: "An advice was added or updated on an item (notify the \"Creators\")"
 msgid "event_add_advice"
 msgstr "An advice was added or updated on an item (notify the \"Creators\")"
 
 #. Default: "An advice was added or updated on an item (notify the \"Owner\")"
 msgid "event_add_advice_owner"
 msgstr "An advice was added or updated on an item (notify the \"Owner\")"
@@ -3530,29 +3459,37 @@
 msgid "fastedit_save_changes"
 msgstr "Save changes."
 
 #. Default: "Please fill this field."
 msgid "field_required"
 msgstr "Please fill this field."
 
-#. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
-msgid "field_reserved_to_meeting_managers_descr"
-msgstr "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
-
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
-msgid "field_vieawable_by_everyone_descr"
-msgstr "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
-
 #. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once item is decided</span>"
 msgid "field_vieawable_by_everyone_once_item_decided_descr"
 msgstr "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once item is decided</span>"
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
-msgid "field_vieawable_by_everyone_once_meeting_decided_descr"
-msgstr "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
+#. Default: "Assembly and signatures"
+msgid "fieldset_assembly"
+msgstr "Assembly and signatures"
+
+#. Default: "Committees"
+msgid "fieldset_committees"
+msgstr "Committees"
+
+#. Default: "Dates and data"
+msgid "fieldset_dates_and_data"
+msgstr "Dates and data"
+
+#. Default: "Informations"
+msgid "fieldset_informations"
+msgstr "Informations"
+
+#. Default: "Parameters"
+msgid "fieldset_parameters"
+msgstr "Parameters"
 
 #. Default: "Please choose a file by clicking on the \"Browse\" button."
 msgid "file_required"
 msgstr "Please choose a file by clicking on the \"Browse\" button."
 
 #. Default: "While using linked vote values, select here values that will be selectable for the first linked vote value"
 msgid "first_linked_vote_used_vote_values_descr"
@@ -3562,21 +3499,17 @@
 msgid "first_transition_must_leave_wf_initial_state"
 msgstr "Please respect order of transitions sequence to present an item, the first given transition is not a transition leaving the item workflow initial state."
 
 #. Default: "In the application folder of every member, a sub-folder is created for each meeting configuration. The name of this sub-folder is defined here."
 msgid "folder_title_descr"
 msgstr "In the application folder of every member, a sub-folder is created for each meeting configuration. The name of this sub-folder is defined here."
 
-#. Default: "For the administrator only"
-msgid "for_admin_only"
-msgstr "For the administrator only"
-
-#. Default: "Specify here the deadline for validating late items to be inserted in a given meeting.  Leave the field empty not to use this functionality."
-msgid "freeze_deadline_default_descr"
-msgstr "Specify here the deadline for validating late items to be inserted in a given meeting.  Leave the field empty not to use this functionnality."
+#. Default: "force display"
+msgid "force_display"
+msgstr "force display"
 
 #. Default: "<p>PloneMeeting body in HTML format.</p>"
 msgid "front_page_body"
 msgstr "<p>PloneMeeting body in HTML format.</p>"
 
 #. Default: "Manage here your official meetings."
 msgid "front_page_description"
@@ -3676,14 +3609,18 @@
 msgstr "Subtypes"
 
 # Other
 #. Default: "Check/uncheck items"
 msgid "helpSelectItemsIcon"
 msgstr "Check/uncheck items"
 
+#. Default: "This is the date the advice was originally given, this will change when the advice will be considered \"Given\" in a state where it is no more editable"
+msgid "help_given_on_before_started_on"
+msgstr "This is the date the advice was originally given, this will change when the advice will be considered \"Given\" in a state where it is no more editable"
+
 #. Default: "No preview available because this type of file can not be converted.  Please use common office formats.  You can download the file, look in the \"actions\" column."
 msgid "help_no_preview_available"
 msgstr "No preview available because this type of file can not be converted.  Please use common office formats.  You can download the file, look in the \"actions\" column."
 
 #. Default: "No preview available because there was an error during conversion to a previewable format.  Please contact system administrator that will have access to more debugging informations."
 msgid "help_no_preview_available_conversion_error"
 msgstr "No preview available because there was an error during conversion to a previewable format.  Please contact system administrator that will have access to more debugging informations."
@@ -3724,18 +3661,14 @@
 msgid "historize_item_data_when_advice_is_given_descr"
 msgstr "When an advice is given, so when it switch to a state where adviser may not advice it anymore, it is historized.  If you chek this box, every relevant item data (title and rich text fields) will be historized together with the advice."
 
 #. Default: "For every field you select here, the application will keep track of any change on any item, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
 msgid "historized_item_attrs_descr"
 msgstr "For every field you select here, the application will keep track of any change on any item, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
 
-#. Default: "For every field you select here, the application will keep track of any change on any meeting, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
-msgid "historized_meeting_attrs_descr"
-msgstr "For every field you select here, the application will keep track of any change on any meeting, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
-
 #. Default: "See changes"
 msgid "history_changes"
 msgstr "See changes"
 
 #. Default: "Deleted by ${userName}"
 msgid "history_delete"
 msgstr "Deleted by ${userName}"
@@ -3752,17 +3685,17 @@
 msgid "holidays_date_not_ascending_error"
 msgstr "Defined date must be defined by ascending order, from older date at the top to newer date at the bottom."
 
 #. Default: "These dates will be used to compute advices delays.  <span style='color: red;'>If you change this parameter and modified dates are interacting with some existing advice delays, do not forget to run \"Update items and meetings\"!</span>"
 msgid "holidays_descr"
 msgstr "These dates will be used to compute advices delays.  <span style='color: red;'>If you change this parameter and modified dates are interacting with some existing advice delays, do not forget to run \"Update items and meetings\"!</span>"
 
-#. Default: "You removed a date that is currently in use!"
+#. Default: "You removed a date that is currently in use! Check item at ${item_url}"
 msgid "holidays_removed_date_in_use_error"
-msgstr "You removed a date that is currently in use!"
+msgstr "You removed a date that is currently in use! Check item at ${item_url}"
 
 #. Default: "There are not enough holidays defined in the configuration.  These days are used for advice delay computation.  This warning appear when last holiday defined in the configuration is in less than 60 days. Contact you system administrator if necessary."
 msgid "holidays_warning_message"
 msgstr "There are not enough holidays defined in the configuration.  These days are used for advice delay computation.  This warning appear when last holiday defined in the configuration is in less than 60 days. Contact you system administrator if necessary."
 
 #. Default: "Wrong date format, please use following format : \"YYYY/MM/DD\"."
 msgid "holidays_wrong_date_format_error"
@@ -3780,14 +3713,18 @@
 msgid "hs_name"
 msgstr "Name"
 
 #. Default: "This application allows you to manage your official meetings."
 msgid "hs_welcome_body"
 msgstr "This application allows you to manage your official meetings."
 
+#. Default: "iA.Delib documentation"
+msgid "iA.Delib documentation"
+msgstr "iA.Delib documentation"
+
 #. Default: "Azur"
 msgid "icon_color_azur"
 msgstr "Azur"
 
 #. Default: "Black"
 msgid "icon_color_black"
 msgstr "Black"
@@ -4311,23 +4248,23 @@
 
 #. Default: "Select here fields of the item that will be show/hidden when a user will click on the \"Show/hide details\" label in the application.  This will affect every listing of items, so classic listings and the meetings view."
 msgid "items_list_visible_fields_descr"
 msgstr "Select here fields of the item that will be show/hidden when a user will click on the \"Show/hide details\" label in the application.  This will affect every listing of items, so classic listings and the meetings view."
 
 #. Default: "When consulting not viewable linked items of an item, some extra fields may be shown if it is selected here.  This let's you show some choosen informations on linked items that are not accessible to the current user."
 msgid "items_not_viewable_visible_fields_descr"
-msgstr ""
+msgstr "When consulting not viewable linked items of an item, some extra fields may be shown if it is selected here.  This let's you show some choosen informations on linked items that are not accessible to the current user."
 
 #. Default: "Specify here a TAL expression that will enable the functionnality of showing some fields when linked items are not viewable by the current user."
 msgid "items_not_viewable_visible_fields_tal_expr_descr"
-msgstr ""
+msgstr "Specify here a TAL expression that will enable the functionnality of showing some fields when linked items are not viewable by the current user."
 
 #. Default: "When consulting linked items of an item, some extra fields may be shown if it is selected here."
 msgid "items_visible_fields_descr"
-msgstr ""
+msgstr "When consulting linked items of an item, some extra fields may be shown if it is selected here."
 
 #. Default: "Item templates managers"
 msgid "itemtemplatesmanagers"
 msgstr "Item templates managers"
 
 #. Default: "Use values defined in the \"Item states allowing to define advices\" field"
 msgid "keep_access_to_item_when_advice_default"
@@ -4394,38 +4331,26 @@
 msgstr "The item is entitled \"${itemTitle}\". You can access this item here: ${objectUrl}."
 
 # Mails (item-related)
 #. Default: "${meetingConfigTitle} - A \"late\" item has been validated."
 msgid "lateItem_mail_subject"
 msgstr "${meetingConfigTitle} - A \"late\" item has been validated."
 
-#. Default: "Items presented tardily"
-msgid "late_presented_items"
-msgstr "Items presented tardily"
-
 #. Default: "--- Do nothing, let the item in the workflow initial state ---"
 msgid "let_item_in_initial_state"
 msgstr "--- Do nothing, let the item in the workflow initial state ---"
 
 #. Default: "Linked items (${auto_linked_items})"
 msgid "linked_items"
 msgstr "Linked items (${auto_linked_items})"
 
 #. Default: "Linked items, ${auto_linked_items} automatically and ${manually_linked_items} manually"
 msgid "linked_items_with_manually_linked_items"
 msgstr "Linked items, ${auto_linked_items} automatically and ${manually_linked_items} manually"
 
-#. Default: "Late"
-msgid "list_type_late"
-msgstr "Late"
-
-#. Default: "Normal"
-msgid "list_type_normal"
-msgstr "Normal"
-
 #. Default: "Types of list of items that will be available when an item is linked to a meeting."
 msgid "list_types_descr"
 msgstr "Types of list of items that will be available when an item is linked to a meeting."
 
 #. Default: "Size"
 msgid "listingheader_size"
 msgstr "Size"
@@ -4522,37 +4447,17 @@
 msgid "meeting_annex_confidential_visible_for_descr"
 msgstr "Select here profiles of users that will be able to see an annex added to a meeting that is set confidential.  <span style='color: red;'>If you change this and there are existing confidential annexes, please run the action \"Update categorized elements\" in the \"Meeting annnex types\" configuration.</span>"
 
 #. Default: "Choose here which page will be shown after logon."
 msgid "meeting_app_default_view_descr"
 msgstr "Choose here which page will be shown after logon."
 
-#. Default: "Assembly"
-msgid "meeting_assembly"
-msgstr "Assembly"
-
-#. Default: "Absents"
-msgid "meeting_assemblyAbsents"
-msgstr "Absents"
-
-#. Default: "Excused"
-msgid "meeting_assemblyExcused"
-msgstr "Excused"
-
-#. Default: "Guests"
-msgid "meeting_assemblyGuests"
-msgstr "Guests"
-
-#. Default: "Proxies"
-msgid "meeting_assemblyProxies"
-msgstr "Proxies"
-
-#. Default: "Staves"
-msgid "meeting_assemblyStaves"
-msgstr "Staves"
+#. Default: "Meeting assembly (${number_of_attendees}) and signatories (${number_of_signatories})"
+msgid "meeting_attendees_and_signatories"
+msgstr "Meeting assembly (${number_of_attendees}) and signatories (${number_of_signatories})"
 
 #. Default: "Choose here which columns to display when listing meetings (ie, when displaying the list of available meetings or decisions, or when performing custom searches)."
 msgid "meeting_columns_descr"
 msgstr "Choose here which columns to display when listing meetings (ie, when displaying the list of available meetings or decisions, or when performing custom searches)."
 
 #. Default: "Similarly to interfaces defined for items, the conditions expressed on the transitions of the meeting workflow may be configured through the development of another Plone product into which you must:<ul><li>create a Python interface that inherits from interface Products.PloneMeeting.interfaces.IMeetingWorkflowConditions (you must enter the full package name of this interface in the field below);</li><li>create and declare in ZCML an adapter that adapts the interface  Products.PloneMeeting.interfaces.IMeeting to the interface you have defined in the previous step.</li></ul>Your adapter may inherit from the default adapter Products.PloneMeeting.Meeting.MeetingWorkflowConditions: it will allow you to override only methods for which you want an altered behaviour. All the methods proposed by the interface Products.PloneMeeting.interfaces.IMeetingWorkflowConditions are documented."
 msgid "meeting_conditions_interface_descr"
@@ -4595,22 +4500,14 @@
 msgid "meeting_organizations"
 msgstr "Organizations"
 
 #. Default: "When an item is inserted in a meeting from everywhere (so not when on a meeting view), this will take the very next meeting still accepting items.  Define here states to take into account to get this very next meeting."
 msgid "meeting_present_item_when_no_current_meeting_states_descr"
 msgstr "When an item is inserted in a meeting from everywhere (so not when on a meeting view), this will take the very next meeting still accepting items.  Define here states to take into account to get this very next meeting."
 
-#. Default: "Signatories"
-msgid "meeting_signatories"
-msgstr "Signatories"
-
-#. Default: "Signatures"
-msgid "meeting_signatures"
-msgstr "Signatures"
-
 #. Default: "You can consult this meeting at ${objectUrl}."
 msgid "meeting_state_changed_default_mail_body"
 msgstr "You can consult this meeting at ${objectUrl}."
 
 # Mails (meeting-related)
 # Default translation for mails sent upon meeting transition
 # This default is used if no accurate translation can be found. We will try for example to translate
@@ -4698,25 +4595,17 @@
 msgid "metadata"
 msgstr "Metadata"
 
 #. Default: "Select here some standard adaptations that can be applied to data structures."
 msgid "model_adaptations_descr"
 msgstr "Select here some standard adaptations that can be applied to data structures."
 
-#. Default: "Move the item down"
-msgid "move_item_down"
-msgstr "Move the item down"
-
-#. Default: "Move item to given position"
+#. Default: "Save item number (you may also use the [Enter] key)"
 msgid "move_item_to_given_position"
-msgstr "Move item to given position"
-
-#. Default: "Move the item up"
-msgid "move_item_up"
-msgstr "Move the item up"
+msgstr "Save item number (you may also use the [Enter] key)"
 
 #. Default: "Moves this item to the position that precedes the number you have introduced besides. If you want to move the item at the end of the list, specify the number of the last item plus one."
 msgid "move_several"
 msgstr "Moves this item to the position that precedes the number you have introduced besides. If you want to move the item at the end of the list, specify the number of the last item plus one."
 
 #. Default: "Negative"
 msgid "negative"
@@ -4734,34 +4623,42 @@
 msgid "nil"
 msgstr "Nil"
 
 #. Default: "No annex is currently defined for this element."
 msgid "no_annexes"
 msgstr "No annex is currently defined for this element."
 
-#. Default: "No annexes to print"
-msgid "no_annexes_to_print_term"
-msgstr "No annexes to print"
-
-#. Default: "Annexes not to sign"
-msgid "no_annexes_to_sign_term"
-msgstr "Annexes not to sign"
-
 #. Default: "Attributes \"assembly\" and \"attendees\" can't be used together."
 msgid "no_assembly_and_attendees"
 msgstr "Attributes \"assembly\" and \"attendees\" can't be used together."
 
 #. Default: "No category is currently defined."
 msgid "no_category"
 msgstr "No category is currently defined."
 
 #. Default: "No classifier is currently defined."
 msgid "no_classifier"
 msgstr "No classifier is currently defined."
 
+#. Default: "NC"
+msgid "no_committee_term_title_acronym"
+msgstr "NC"
+
+#. Default: "No committee"
+msgid "no_committee_term_title_label"
+msgstr "No committee"
+
+#. Default: "Attributes \"committees_assembly\" and \"committees_attendees\" can't be used together."
+msgid "no_committees_assembly_and_committees_attendees"
+msgstr "Attributes \"committees_assembly\" and \"committees_attendees\" can't be used together."
+
+#. Default: "Attributes \"committees_sigantures\" and \"committees_signatories\" can't be used together."
+msgid "no_committees_signatures_and_committees_signatories"
+msgstr "Attributes \"committees_sigantures\" and \"committees_signatories\" can't be used together."
+
 #. Default: "None"
 msgid "no_config_group"
 msgstr "None"
 
 #. Default: "No emergency"
 msgid "no_emergency"
 msgstr "No emergency"
@@ -4786,33 +4683,29 @@
 msgid "no_meeting_file_type"
 msgstr "No annex type is currently defined."
 
 #. Default: "No special user is currently defined."
 msgid "no_meeting_user"
 msgstr "No special user is currently defined."
 
-#. Default: "No items."
-msgid "no_meetingitems"
-msgstr "No items."
-
 #. Default: "No POD template is currently defined."
 msgid "no_pod_folder"
 msgstr "No POD template is currently defined."
 
 #. Default: "Attributes \"proposingGroupWithGroupInCharge\" and \"groupsInCharge\" can't be used together."
 msgid "no_proposingGroupWithGroupInCharge_and_groupsInCharge"
 msgstr "Attributes \"proposingGroupWithGroupInCharge\" and \"groupsInCharge\" can't be used together."
 
 #. Default: "No recurring item is currently defined."
 msgid "no_recurring_item"
 msgstr "No recurring item is currently defined."
 
-#. Default: "No visible item for now."
+#. Default: "You do not have access to these items."
 msgid "no_shown_items"
-msgstr "No visible item for now."
+msgstr "You do not have access to these items."
 
 #. Default: "Attributes \"signatures\" and \"signatories\" can't be used together."
 msgid "no_signatories_and_signatures"
 msgstr "Attributes \"signatures\" and \"signatories\" can't be used together."
 
 #. Default: "No style POD template is currently defined."
 msgid "no_style_pod_folder"
@@ -4838,14 +4731,22 @@
 msgid "normal"
 msgstr "Normal item"
 
 #. Default: "You are a registered user but your account has not been activated yet. Please contact the system administrator."
 msgid "notPloneMeetingUser"
 msgstr "You are a registered user but your account has not been activated yet. Please contact the system administrator."
 
+#. Default: "Not able to find a meeting to present this item into.  Only meetings in the future are taken into account, check configuration if necessary"
+msgid "not_able_to_find_meeting_to_present_item_into"
+msgstr "Not able to find a meeting to present this item into.  Only meetings in the future are taken into account, check configuration if necessary"
+
+#. Default: "Not confidential annexes"
+msgid "not_confidential_annexes"
+msgstr "Not confidential annexes"
+
 #. Default: "Not given yet"
 msgid "not_given"
 msgstr "Not given yet"
 
 #. Default: "Not to be cloned to anywhere"
 msgid "not_to_be_cloned_to_term"
 msgstr "Not to be cloned to anywhere"
@@ -4862,14 +4763,22 @@
 msgid "nothing_to_do"
 msgstr "Nothing to do."
 
 #. Default: "notify users able to view the element"
 msgid "notify_users_able_to_view_element"
 msgstr "notify users able to view the element"
 
+#. Default: "${number}st"
+msgid "num_part_st"
+msgstr "${number}st"
+
+#. Default: "${number}th"
+msgid "num_part_th"
+msgstr "${number}th"
+
 #. Default: "Total number of voters"
 msgid "number_of_voters"
 msgstr "Total number of voters"
 
 #. Default: "Observer"
 msgid "observer"
 msgstr "Observer"
@@ -4878,14 +4787,18 @@
 msgid "observers"
 msgstr "Observers"
 
 #. Default: "Follow all associated groups order"
 msgid "on_all_associated_groups"
 msgstr "Follow all associated groups order"
 
+#. Default: "Follow all committees order"
+msgid "on_all_committees"
+msgstr "Follow all committees order"
+
 #. Default: "Follow all groups order"
 msgid "on_all_groups"
 msgstr "Follow all groups order"
 
 #. Default: "Follow categories order"
 msgid "on_categories"
 msgstr "Follow categories order"
@@ -4966,14 +4879,18 @@
 msgid "oral_question_item_descr"
 msgstr " "
 
 #. Default: "If this field is left empty, selectable associated organizations are every organizations selected in the plonegroup configuration panel.  Here you may select associated organizations in a particular order including organizations that are not selected in the plonegroup configuration panel.  This is only relevant if the 'Associated groups' field is enabled on items."
 msgid "ordered_associated_organizations_descr"
 msgstr "If this field is left empty, selectable associated organizations are every organizations selected in the plonegroup configuration panel.  Here you may select associated organizations in a particular order including organizations that are not selected in the plonegroup configuration panel.  This is only relevant if the 'Associated groups' field is enabled on items."
 
+#. Default: "Select here attendees that will be selectable in the \"Attendees\" column of defined committees here under.  <span style='color: red;'>If you select/unselect values, you need to save first then edit again for these values to appear/disappear if field \"Committees\" here under.</span>"
+msgid "ordered_committee_contacts_descr"
+msgstr "Select here attendees that will be selectable in the \"Attendees\" column of defined committees here under.  <span style='color: red;'>If you select/unselect values, you need to save first then edit again for these values to appear/disappear if field \"Committees\" here under.</span>"
+
 #. Default: "Select here contacts that will be usable to manage meeting attendees.  The contacts order defined here will be the default order when creating a new meeting."
 msgid "ordered_contacts_descr"
 msgstr "Select here contacts that will be usable to manage meeting attendees.  The contacts order defined here will be the default order when creating a new meeting."
 
 #. Default: "If this field is left empty, selectable groups in charge are every organizations selected in the plonegroup configuration panel.  Here you may select groups in charge in a particular order.  This is only relevant if the 'Groups in charge' field is enabled on items."
 msgid "ordered_groups_in_charge_descr"
 msgstr "If this field is left empty, selectable groups in charge are every organizations selected in the plonegroup configuration panel.  Here you may select groups in charge in a particular order.  This is only relevant if the 'Groups in charge' field is enabled on items."
@@ -5006,22 +4923,26 @@
 msgid "owner_may_delete_annex_decision_descr"
 msgstr "If checked, the user that created an annexDecision will be able to remove it even if the item is no more editable, if not checked, only a Manager will be able to remove an annexDecision when the item is no more editable."
 
 #. Default: "Mark this person absent for this item"
 msgid "person_byebye"
 msgstr "Mark this person absent for this item"
 
+#. Default: "Redefine position for attendee for this item"
+msgid "person_redefine_attendee_position"
+msgstr "Redefine position for attendee for this item"
+
+#. Default: "Remove redefined position for attendee for this item"
+msgid "person_remove_redefined_attendee_position"
+msgstr "Remove redefined position for attendee for this item"
+
 #. Default: "Remove this person from absents for this item"
 msgid "person_welcome"
 msgstr "Remove this person from absents for this item"
 
-#. Default: "Please encode this other place."
-msgid "place_other_required"
-msgstr "Please encode this other place."
-
 #. Default: "Enter here some default places where meetings occur. There must be one place per line. The first one will be the default one."
 msgid "places_descr"
 msgstr "Enter here some default places where meetings occur. There must be one place per line. The first one will be the default one."
 
 #. Default: "You are about to delete this meeting and all included items. Are you sure?"
 msgid "plonemeeting_delete_meeting_confirm_message"
 msgstr "You are about to delete this meeting and all included items. Are you sure?"
@@ -5214,22 +5135,14 @@
 msgid "powerobservers"
 msgstr "Power observers"
 
 #. Default: "The preparatory meeting must occur before the meeting."
 msgid "pre_date_after_meeting_date"
 msgstr "The preparatory meeting must occur before the meeting."
 
-#. Default: "Preparatory meeting"
-msgid "pre_meeting"
-msgstr "Preparatory meeting"
-
-#. Default: "Specify here the date of the pre-meeting, relative to its meeting, in the same format as fields above.  Leave the field empty not to use this functionality."
-msgid "pre_meeting_date_default_descr"
-msgstr "Specify here the date of the pre-meeting, relative to its meeting, in the same format as fields above.  Leave the field emtpy no to use the functionnality."
-
 #. Default: "If this is a normal item and you want it to be inserted in any availale meeting, just select \"No preference\" value.  Selecting a date is for 2 usecases : this will make the item not presentable to the meetings before selected one, or if the selected meeting is \"frozen\", this will make current item considered as \"late\" item presentable in the selected frozen meeting.  Indeed, the only way to insert an item in a frozen meeting is to select this meeting as preferred meeting."
 msgid "preferred_meeting_descr"
 msgstr "If this is a normal item and you want it to be inserted in any availale meeting, just select \"No preference\" value.  Selecting a date is for 2 usecases : this will make the item not presentable to the meetings before selected one, or if the selected meeting is \"frozen\", this will make current item considered as \"late\" item presentable in the selected frozen meeting.  Indeed, the only way to insert an item in a frozen meeting is to select this meeting as preferred meeting."
 
 #. Default: "Pre-validator"
 msgid "prereviewer"
 msgstr "Pre-validator"
@@ -5274,34 +5187,34 @@
 msgid "public"
 msgstr "Public meeting"
 
 #. Default: "Public meeting (heading)"
 msgid "public_heading"
 msgstr "Public meeting (heading)"
 
-#. Default: "Specify here the deadline for validating items to be inserted in a given meeting. You need to express this deadline relative to the meeting date. For example, \"5.9:30\" (do not type quotes) means: \"5 days before the meeting date, at 9:30.\".  Leave the field empty not to use this functionality."
-msgid "publish_deadline_default_descr"
-msgstr "Specify here the deadline for validating items to be inserted in a given meeting. You need to express this deadline relative to the meeting date. For example, \"5.9:30\" (do not type quotes) means: \"5 days before the meeting date, at 9:30.\".  Leave the field empty not to use this functionality."
-
 #. Default: "Publishable (displayed)"
 msgid "publishable_display"
 msgstr "Publishable (displayed)"
 
 #. Default: "Publishable (editable)"
 msgid "publishable_edit"
 msgstr "Publishable (editable)"
 
+#. Default: "Read less"
+msgid "read_less"
+msgstr "Read less"
+
+#. Default: "Read more"
+msgid "read_more"
+msgstr "Read more"
+
 #. Default: "Select here the item states into which some events related to the item (like annex creations or deletions) will be stored in the item's history."
 msgid "record_item_history_states_descr"
 msgstr "Select here the item states into which some events related to the item (like annex creations or deletions) will be stored in the item's history."
 
-#. Default: "Select here the meeting states into which some events related to the meeting will be stored in the meeting's history."
-msgid "record_meeting_history_states_descr"
-msgstr "Select here the meeting states into which some events related to the meeting will be stored in the meeting's history."
-
 #. Default: "The recurring item specified in the subject of this email could not be inserted in a meeting. Maybe does it lack some important information (a text for the decision, for example) while the meeting is in an \"advanced\" state (it is already \"decided\", for instance). More information can be found in the log file of your Zope instance."
 msgid "recurringItemWorkflowError_mail_body"
 msgstr "The recurring item specified in the subject of this email could not be inserted in a meeting. Maybe does it lack some important information (a text for the decision, for example) while the meeting is in an \"advanced\" state (it is already \"decided\", for instance). More information can be found in the log file of your Zope instance."
 
 #. Default: "${portalTitle} - A problem occurred while inserting a recurring into a meeting - ${itemTitle}"
 msgid "recurringItemWorkflowError_mail_subject"
 msgstr "${portalTitle} - A problem occurred while inserting a recurring into a meeting - ${itemTitle}"
@@ -5346,26 +5259,34 @@
 msgid "remove_several_items"
 msgstr "remove all selected items at once."
 
 #. Default: "Selected items have been removed from the meeting."
 msgid "remove_several_items_done"
 msgstr "Selected items have been removed from the meeting."
 
-#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by \"${hp_url}\"!"
+#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by held position at \"${hp_url}\"!"
 msgid "removed_position_type_in_use_error"
-msgstr "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by \"${hp_url}\"!"
+msgstr "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by held position at \"${hp_url}\"!"
+
+#. Default: "You can not remove a position type that was used as redefined position for an attendee on an item, you removed \"${removed_position_type}\", check attendees on item at \"${item_url}\"!"
+msgid "removed_redefined_position_type_in_use_error"
+msgstr "You can not remove a position type that was used as redefined position for an attendee on an item, you removed \"${removed_position_type}\", check attendees on item at \"${item_url}\"!"
 
 #. Default: "A category must be selected on this item so it may evolve in the workflow"
 msgid "required_category_ko"
 msgstr "A category must be selected on this item so it may evolve in the workflow"
 
 #. Default: "A classifier must be selected on this item so it may evolve in the workflow"
 msgid "required_classifier_ko"
 msgstr "A classifier must be selected on this item so it may evolve in the workflow"
 
+#. Default: "A group in charge must be selected on this item so it may evolve in the workflow"
+msgid "required_groupsInCharge_ko"
+msgstr "A group in charge must be selected on this item so it may evolve in the workflow"
+
 #. Default: "Check the box if access to secret items must be restricted.  This will let only users for which an explicit access to the item has been given, access the item.  It will be the case so for members of the proposing groups, power users (Managers, MeetingManagers, power observers), copy groups and advisers.  Only activate this if necessary, it could be the case if you have a state where everything is accessible by everyone (like a \"published\" state for items) but where you want \"secret\" items not to be accessible by everyone."
 msgid "restrict_access_to_secret_items_descr"
 msgstr "Check the box if access to secret items must be restricted.  This will let only users for which an explicit access to the item has been given, access the item.  It will be the case so for members of the proposing groups, power users (Managers, MeetingManagers, power observers), copy groups and advisers.  Only activate this if necessary, it could be the case if you have a state where everything is accessible by everyone (like a \"published\" state for items) but where you want \"secret\" items not to be accessible by everyone."
 
 #. Default: "Restrict access to secret items to description"
 msgid "restrict_access_to_secret_items_to_descr"
 msgstr "Restrict access to secret items to description"
@@ -5547,14 +5468,18 @@
 msgid "selectable_for_plonegroup_descr"
 msgstr "Uncheck this box if this organization is added for another purpose than creating Plone subgroups so it can use the application."
 
 #. Default: "Select here privacies that will be selectable by users editing items of this configuration.  If \"on privacy\" is used in the \"Sort order(s) to apply when adding an item to a meeting\" field, it is the order of values selected here that will be used."
 msgid "selectable_privacies_descr"
 msgstr "Select here privacies that will be selectable by users editing items of this configuration.  If \"on privacy\" is used in the \"Sort order(s) to apply when adding an item to a meeting\" field, it is the order of values selected here that will be used."
 
+#. Default: "Select here position types that will be selectable when redefining the position of an attendee for an item.  If nothing selected (default), then any position types is selectable."
+msgid "selectable_redefined_position_types_descr"
+msgstr "Select here position types that will be selectable when redefining the position of an attendee for an item.  If nothing selected (default), then any position types is selectable."
+
 #. Default: "Check the box if item needs to be send to authority, if so, a line will be automatically printed in the item deliberation document."
 msgid "send_to_authority_descr"
 msgstr "Check the box if item needs to be send to authority, if so, a line will be automatically printed in the item deliberation document."
 
 #. Default: "Unable to send this item to the ${meetingConfigTitle} meetingConfig because the user to create the item to does not have a personal folder in this meetingConfig.  If necessary, the concerned user can connect for this folder to be created automatically."
 msgid "sendto_inexistent_destfolder_error"
 msgstr "Unable to send this item to the ${meetingConfigTitle} meetingConfig because the user to create the item to does not have a personal folder in this meetingConfig.  If necessary, the concerned user can connect for this folder to be created automatically."
@@ -5600,18 +5525,14 @@
 msgid "show_or_hide_details"
 msgstr "Show / hide details"
 
 #. Default: "Show / hide poll type observations"
 msgid "show_or_hide_pollTypeObservations"
 msgstr "Show / hide poll type observations"
 
-#. Default: "Signatures"
-msgid "signatures"
-msgstr "Signatures"
-
 #. Default: "Signatures as defined on the linked meeting"
 msgid "signatures_defined_on_meeting"
 msgstr "Signatures as defined on the linked meeting"
 
 #. Default: "Define here the default signatures that will be automatically selected on newly created meetings. Use 2 lines by signature, one for the function and one for the signatory name. This will be applicable only if you use attribute \"Signatures\" for meetings."
 msgid "signatures_descr"
 msgstr "Define here the default signatures that will be automatically selected on newly created meetings. Use 2 lines by signature, one for the function and one for the signatory name. This will be applicable only if you use attribute \"Signatures\" for meetings."
@@ -5624,14 +5545,22 @@
 msgid "signed_edit"
 msgstr "Signed (editable)"
 
 #. Default: "Check this box if you want to sort the tags in alphabetic order."
 msgid "sort_all_item_tags_descr"
 msgstr "Check this box if you want to sort the tags in alphabetic order."
 
+#. Default: "The meeting start date must occur before the end date."
+msgid "start_date_after_end_date"
+msgstr "The meeting start date must occur before the end date."
+
+#. Default: "The meeting start date must occur after the meeting date."
+msgid "start_date_before_meeting_date"
+msgstr "The meeting start date must occur after the meeting date."
+
 #. Default: "Store as annex of type ${annex_type_title}"
 msgid "store_as_annex_type_title"
 msgstr "Store as annex of type ${annex_type_title}"
 
 #. Default: "Not allowed to add annex in this element."
 msgid "store_podtemplate_as_annex_can_not_add_annex"
 msgstr "Not allowed to add annex in this element."
@@ -5725,21 +5654,217 @@
 msgstr "This item is an oral question"
 
 #. Default: "This item is NOT an oral question"
 msgid "this_item_is_not_an_oral_question"
 msgstr "This item is NOT an oral question"
 
 #. Default: "Extraordinary session"
-msgid "this_meeting_is_extraodrinary_session"
+msgid "this_meeting_is_extraordinary_session"
 msgstr "Extraordinary session"
 
+#. Default: "Absents"
+msgid "title_absents"
+msgstr "Absents"
+
+#. Default: "Approval date"
+msgid "title_approval_date"
+msgstr "Approval date"
+
+#. Default: "Assembly"
+msgid "title_assembly"
+msgstr "Assembly"
+
+#. Default: "Assembly absents"
+msgid "title_assembly_absents"
+msgstr "Assembly absents"
+
+#. Default: "Assembly excused"
+msgid "title_assembly_excused"
+msgstr "Assembly excused"
+
+#. Default: "Assembly guests"
+msgid "title_assembly_guests"
+msgstr "Assembly guests"
+
+#. Default: "Assembly observations"
+msgid "title_assembly_observations"
+msgstr "Assembly observations"
+
+#. Default: "Assembly proxies"
+msgid "title_assembly_proxies"
+msgstr "Assembly proxies"
+
+#. Default: "Assembly staves"
+msgid "title_assembly_staves"
+msgstr "Assembly staves"
+
+#. Default: "Attendees"
+msgid "title_attendees"
+msgstr "Attendees"
+
+#. Default: "Authority notice"
+msgid "title_authority_notice"
+msgstr "Authority notice"
+
+#. Default: "Committees"
+msgid "title_committees"
+msgstr "Committees"
+
+#. Default: "Assembly"
+msgid "title_committees_assembly"
+msgstr "Assembly"
+
+#. Default: "Attendees"
+msgid "title_committees_attendees"
+msgstr "Attendees"
+
+#. Default: "Convocation date"
+msgid "title_committees_convocation_date"
+msgstr "Convocation date"
+
+#. Default: "Date"
+msgid "title_committees_date"
+msgstr "Date"
+
+#. Default: "Committees observations"
+msgid "title_committees_observations"
+msgstr "Committees observations"
+
+#. Default: "Place"
+msgid "title_committees_place"
+msgstr "Place"
+
+#. Default: "Committee"
+msgid "title_committees_row_id"
+msgstr "Committee"
+
+#. Default: "Signatories"
+msgid "title_committees_signatories"
+msgstr "Signatories"
+
+#. Default: "Signatures"
+msgid "title_committees_signatures"
+msgstr "Signatures"
+
+#. Default: "Convocation date"
+msgid "title_convocation_date"
+msgstr "Convocation date"
+
+#. Default: "Date"
+msgid "title_date"
+msgstr "Date"
+
+#. Default: "Default assembly"
+msgid "title_default_assembly"
+msgstr "Default assembly"
+
+#. Default: "Default assembly staves"
+msgid "title_default_assembly_staves"
+msgstr "Default assembly staves"
+
+#. Default: "Default signatures"
+msgid "title_default_signatures"
+msgstr "Default signatures"
+
+#. Default: "End date"
+msgid "title_end_date"
+msgstr "End date"
+
+#. Default: "Excused"
+msgid "title_excused"
+msgstr "Excused"
+
+#. Default: "Extraordinary session"
+msgid "title_extraordinary_session"
+msgstr "Extraordinary session"
+
+#. Default: "First item number (managed automatically when meeting is frozen)"
+msgid "title_first_item_number"
+msgstr "First item number (managed automatically when meeting is frozen)"
+
+#. Default: "In and out moves"
+msgid "title_in_and_out_moves"
+msgstr "In and out moves"
+
+#. Default: "Meeting number"
+msgid "title_meeting_number"
+msgstr "Meeting number"
+
+#. Default: "Meeting managers notes"
+msgid "title_meetingmanagers_notes"
+msgstr "Meeting managers notes"
+
+#. Default: "Mid date"
+msgid "title_mid_date"
+msgstr "Mid date"
+
+#. Default: "Non attendees"
+msgid "title_non_attendees"
+msgstr "Non attendees"
+
+#. Default: "Notes"
+msgid "title_notes"
+msgstr "Notes"
+
+#. Default: "Observations"
+msgid "title_observations"
+msgstr "Observations"
+
+#. Default: "Place"
+msgid "title_place"
+msgstr "Place"
+
+#. Default: "Other place"
+msgid "title_place_other"
+msgstr "Other place"
+
+#. Default: "Pre meeting date"
+msgid "title_pre_meeting_date"
+msgstr "Pre meeting date"
+
+#. Default: "Pre meeting place"
+msgid "title_pre_meeting_place"
+msgstr "Pre meeting place"
+
+#. Default: "Pre observations"
+msgid "title_pre_observations"
+msgstr "Pre observations"
+
+#. Default: "Public meeting observations"
+msgid "title_public_meeting_observations"
+msgstr "Public meeting observations"
+
+#. Default: "Replacements"
+msgid "title_replacements"
+msgstr "Replacements"
+
 #. Default: "A title is required."
 msgid "title_required"
 msgstr "A title is required."
 
+#. Default: "Secret meeting observations"
+msgid "title_secret_meeting_observations"
+msgstr "Secret meeting observations"
+
+#. Default: "Signatories"
+msgid "title_signatories"
+msgstr "Signatories"
+
+#. Default: "Signatures"
+msgid "title_signatures"
+msgstr "Signatures"
+
+#. Default: "Start date"
+msgid "title_start_date"
+msgstr "Start date"
+
+#. Default: "Votes observations"
+msgid "title_votes_observations"
+msgstr "Votes observations"
+
 #. Default: "Ask this advice again (current advice will be historized)"
 msgid "to_advice_asked_again"
 msgstr "Ask this advice again (current advice will be historized)"
 
 #. Default: "To be printed (displayed)"
 msgid "to_be_printed_display"
 msgstr "To be printed (displayed)"
@@ -5920,18 +6045,14 @@
 msgid "used_poll_types_descr"
 msgstr "Specify here which poll types you are going to use."
 
 #. Default: "Specify here what vote values are in use in this meeting configuration."
 msgid "used_vote_values_descr"
 msgstr "Specify here what vote values are in use in this meeting configuration."
 
-#. Default: "Users"
-msgid "users"
-msgstr "Users"
-
 #. Default: "If you do not select anything, every users will be displayed."
 msgid "users_hidden_in_dashboard_filter_descr"
 msgstr "If you do not select anything, every users will be displayed."
 
 #. Default: "When an advice is \"given\" and no more editable by the advisers, so when it was set in a state where advisers may not edit it anymore, it is automatically versioned. Depending on the configuration, if advice may be given when the item is still editable by the proposing group, it may be necessary to versionate advice if it was given (but still editable by advisers) and the item was edited. For example, advices are giveable when item is \"itemcreated\", a state where item may still be edited by the proposing group. If it is the case, check this box, it will ensure that the advice is versioned when the item is edited if necessary (so if it was not already versioned since last advice edition).  If you have a specific state \"waiting advice\" where proposing group is not able to edit the item, this box may be left unchecked."
 msgid "versionate_advice_if_given_and_item_modified_descr"
 msgstr "When an advice is \"given\" and no more editable by the advisers, so when it was set in a state where advisers may not edit it anymore, it is automatically versioned. Depending on the configuration, if advice may be given when the item is still editable by the proposing group, it may be necessary to versionate advice if it was given (but still editable by advisers) and the item was edited. For example, advices are giveable when item is \"itemcreated\", a state where item may still be edited by the proposing group. If it is the case, check this box, it will ensure that the advice is versioned when the item is edited if necessary (so if it was not already versioned since last advice edition).  If you have a specific state \"waiting advice\" where proposing group is not able to edit the item, this box may be left unchecked."
@@ -6209,17 +6330,16 @@
 msgstr "Return to proposing group for corrections with one validation (the last)"
 
 #. Default: "Reviewers may take back validated item"
 msgid "wa_reviewers_take_back_validated_item"
 msgstr "Reviewers may take back validated item"
 
 #. Default: "Wait advices (base: from custom configuration, from itemcreated/proposed/prevalidated, select who may send back)"
-#, fuzzy
 msgid "wa_waiting_advices"
-msgstr "Wait advices (base: from custom configuration, from itemcreated/proposed, select who may send back)"
+msgstr "Wait advices (base: from custom configuration, from itemcreated/proposed/prevalidated, select who may send back)"
 
 #. Default: "Wait advices (complementary: when item in state \"Waiting advices\", item may be validated by advisers)"
 msgid "wa_waiting_advices_adviser_may_validate"
 msgstr "Wait advices (complementary: when item in state \"Waiting advices\", item may be validated by advisers)"
 
 #. Default: "Wait advices (complementary: when item in state \"Waiting advices\", item may be sent back by advisers)"
 msgid "wa_waiting_advices_adviser_send_back"
@@ -6249,14 +6369,23 @@
 msgid "wait_msg"
 msgstr "Please wait..."
 
 #. Default: "You are currently adding an organization outside \"My organization\", please make sure this is correct.  If you want to create a new group that will be able the create items, give advices, you need to add it directly under \"My organization\"."
 msgid "warning_adding_org_outside_own_org"
 msgstr "You are currently adding an organization outside \"My organization\", please make sure this is correct.  If you want to create a new group that will be able the create items, give advices, you need to add it directly under \"My organization\"."
 
+#. Default: "Advice is currently \"Asked again\" do not forget to change value of field \"Advice type\" to another value than \"Asked again\""
+msgid "warning_advice_asked_again_need_to_change_advice_type"
+msgstr "Advice is currently \"Asked again\" do not forget to change value of field \"Advice type\" to another value than \"Asked again\""
+
+#. Default: "Warning, there is a problem with encoded data for assembly and signatures, please check especially that signatories are correctly defined"
+#, fuzzy
+msgid "warning_assembly_and_signatures"
+msgstr "Warning, there is a problem with encoded data for assembly and signatures, please check especially that at least 2 signatories are defined"
+
 #. Default: "Warning: if you modify the title or description and save this form, all given advices will be invalidated."
 msgid "warning_invalidate_advices"
 msgstr "Warning: if you modify the title or description and save this form, all given advices will be invalidated."
 
 #. Default: "If you modify this field, all given advices will be invalidated."
 msgid "warning_invalidate_advices_fastedit"
 msgstr "If you modify this field, all given advices will be invalidated."
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/collective.contact.core.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/de/LC_MESSAGES/collective.contact.core.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.history.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/plone.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/plone.po`

 * *Files 0% similar despite different names*

```diff
@@ -543,14 +543,18 @@
 msgid "close"
 msgstr "Close"
 
 #. Default: "Closed"
 msgid "closed"
 msgstr "Closed"
 
+#. Default: "Committees"
+msgid "committees"
+msgstr ""
+
 #. Default: "Confirm"
 msgid "confirm"
 msgstr "Confirm"
 
 #. Default: "Confirmed"
 msgid "confirmed"
 msgstr "Confirmed"
@@ -977,14 +981,15 @@
 msgstr "Validate"
 
 #. Default: "Validated"
 msgid "validated"
 msgstr "Validated"
 
 #. Default: "Votes"
+#, fuzzy
 msgid "votes"
 msgstr "Votes"
 
 #. Default: "Ask advices"
 msgid "wait_advices_from"
 msgstr "Ask advices"
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.actionspanel.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.annex.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/en/LC_MESSAGES/imio.annex.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/PloneMeeting.pot` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/PloneMeeting.pot`

 * *Files 1% similar despite different names*

```diff
@@ -140,26 +140,18 @@
 msgid "PloneMeeting_label_itemTitle"
 msgstr ""
 
 #. Default: "Description"
 msgid "PloneMeeting_label_description"
 msgstr ""
 
-#. Default: "Description in the second language"
-msgid "PloneMeeting_label_description2"
-msgstr ""
-
 #. Default: "Detailed description"
 msgid "PloneMeeting_label_detailedDescription"
 msgstr ""
 
-#. Default: "Detailed description"
-msgid "PloneMeeting_label_detailedDescription2"
-msgstr ""
-
 #. Default: "Assembly that is specific to this meeting item"
 msgid "PloneMeeting_label_itemAssembly"
 msgstr ""
 
 #. Default: "Attendees for this item"
 msgid "attendees_for_item"
 msgstr ""
@@ -173,23 +165,15 @@
 msgstr ""
 
 #. Default: "Assembly guests that is specific to this meeting item"
 msgid "PloneMeeting_label_itemAssemblyGuests"
 msgstr ""
 
 #. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
-msgid "assembly_meeting_descr"
-msgstr ""
-
-#. Default: "Define here people that were excused for the meeting"
-msgid "assembly_excused_meeting_descr"
-msgstr ""
-
-#. Default: "Define here people that were absents (not excused) for the meeting"
-msgid "assembly_absents_meeting_descr"
+msgid "descr_assembly"
 msgstr ""
 
 #. Default: "If you don't fill this field, meeting assembly will be used for this item.  Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use excused and absent fields"
 msgid "item_assembly_descr"
 msgstr ""
 
 #. Default: "If you don't fill this field, meeting assembly excused will be used for this item"
@@ -356,18 +340,14 @@
 msgid "PloneMeeting_inAndOutMoves"
 msgstr ""
 
 #. Default: "Observations"
 msgid "PloneMeeting_itemObservations"
 msgstr ""
 
-#. Default: "Observations"
-msgid "PloneMeeting_itemObservations2"
-msgstr ""
-
 #. Default: "Annexes"
 msgid "label_related_items"
 msgstr ""
 
 #. Default: "Number"
 msgid "PloneMeeting_label_itemNumber"
 msgstr ""
@@ -396,14 +376,18 @@
 msgid "PloneMeeting_label_takenOverBy"
 msgstr ""
 
 #. Default: "(Nobody)"
 msgid "(Nobody)"
 msgstr ""
 
+#. Default: "(None)"
+msgid "(None)"
+msgstr ""
+
 #. Default: "Taken over by ${fullname}"
 msgid "Taken over by ${fullname}"
 msgstr ""
 
 #. Default: "Copy groups"
 msgid "PloneMeeting_label_copyGroups"
 msgstr ""
@@ -652,15 +636,15 @@
 msgid "and_decision"
 msgstr ""
 
 #. Default: "State"
 msgid "item_state"
 msgstr ""
 
-#. Default: "No visible item for now."
+#. Default: "You do not have access to these items."
 msgid "no_shown_items"
 msgstr ""
 
 #. Default: "Go to the meeting containing this item."
 msgid "pm_goto_meeting"
 msgstr ""
 
@@ -760,95 +744,14 @@
 msgid "switch_votes_why_cannot"
 msgstr ""
 
 #. Default: "Votes"
 msgid "existing_votes"
 msgstr ""
 
-# Meeting
-#. Default: "Title"
-msgid "PloneMeeting_label_title"
-msgstr ""
-
-#. Default: "Title in the second language"
-msgid "PloneMeeting_label_title2"
-msgstr ""
-
-#. Default: "Date"
-msgid "PloneMeeting_label_date"
-msgstr ""
-
-#. Default: "Effective start date and hour"
-msgid "PloneMeeting_label_startDate"
-msgstr ""
-
-#. Default: "End date for meeting first part"
-msgid "PloneMeeting_label_midDate"
-msgstr ""
-
-#. Default: "Effective end date and hour"
-msgid "PloneMeeting_label_endDate"
-msgstr ""
-
-#. Default: "Meeting approval date"
-msgid "PloneMeeting_label_approvalDate"
-msgstr ""
-
-#. Default: "Meeting convocation date"
-msgid "PloneMeeting_label_convocationDate"
-msgstr ""
-
-#. Default: "Signatures"
-msgid "meeting_signatures"
-msgstr ""
-
-#. Default: "Signatories"
-msgid "meeting_signatories"
-msgstr ""
-
-#. Default: "Assembly"
-msgid "meeting_assembly"
-msgstr ""
-
-#. Default: "Excused"
-msgid "meeting_assemblyExcused"
-msgstr ""
-
-#. Default: "Absents"
-msgid "meeting_assemblyAbsents"
-msgstr ""
-
-#. Default: "Guests"
-msgid "meeting_assemblyGuests"
-msgstr ""
-
-#. Default: "Proxies"
-msgid "meeting_assemblyProxies"
-msgstr ""
-
-#. Default: "Staves"
-msgid "meeting_assemblyStaves"
-msgstr ""
-
-#. Default: "Attendees"
-msgid "PloneMeeting_label_attendees"
-msgstr ""
-
-#. Default: "Absents"
-msgid "PloneMeeting_label_absents"
-msgstr ""
-
-#. Default: "Excused"
-msgid "PloneMeeting_label_excused"
-msgstr ""
-
-#. Default: "Non attendees"
-msgid "PloneMeeting_label_nonAttendees"
-msgstr ""
-
 #. Default: "Attendee?"
 msgid "is_attendee"
 msgstr ""
 
 #. Default: "Late attendee?"
 msgid "is_late_attendee"
 msgstr ""
@@ -861,14 +764,22 @@
 msgid "person_byebye"
 msgstr ""
 
 #. Default: "Remove this person from non attendees for this item"
 msgid "nonattendee_welcome"
 msgstr ""
 
+#. Default: "Redefine position for attendee for this item"
+msgid "person_redefine_attendee_position"
+msgstr ""
+
+#. Default: "Remove redefined position for attendee for this item"
+msgid "person_remove_redefined_attendee_position"
+msgstr ""
+
 #. Default: "Mark this person as non attendee for this item"
 msgid "nonattendee_byebye"
 msgstr ""
 
 #. Default: "This person was absent during discussion on this item"
 msgid "item_attendee_absent"
 msgstr ""
@@ -901,170 +812,82 @@
 msgid "default_for_all_items"
 msgstr ""
 
 #. Default: "Replaced by"
 msgid "is_replaced"
 msgstr ""
 
-#. Default: "Place"
-msgid "PloneMeeting_label_place"
-msgstr ""
-
-#. Default: "Please encode this other place."
-msgid "place_other_required"
-msgstr ""
-
-#. Default: "Extraordinary session?"
-msgid "PloneMeeting_label_extraordinarySession"
-msgstr ""
-
 #. Default: "Extraordinary session"
-msgid "this_meeting_is_extraodrinary_session"
-msgstr ""
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations"
-msgstr ""
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations2"
-msgstr ""
-
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations"
-msgstr ""
-
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations2"
-msgstr ""
-
-#. Default: "Preparatory meeting"
-msgid "pre_meeting"
-msgstr ""
-
-#. Default: "Date"
-msgid "PloneMeeting_label_preMeetingDate"
+msgid "this_meeting_is_extraordinary_session"
 msgstr ""
 
 #. Default: "The preparatory meeting must occur before the meeting."
 msgid "pre_date_after_meeting_date"
 msgstr ""
 
-#. Default: "Place"
-msgid "PloneMeeting_label_preMeetingPlace"
+#. Default: "The meeting start date must occur after the meeting date."
+msgid "start_date_before_meeting_date"
 msgstr ""
 
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations"
+#. Default: "The meeting end date must occur after the start date and meeting date."
+msgid "end_date_before_meeting_date"
 msgstr ""
 
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations2"
+#. Default: "The meeting start date must occur before the end date."
+msgid "start_date_after_end_date"
 msgstr ""
 
 #. Default: "Observations for the committee"
 msgid "PloneMeeting_label_committeeObservations"
 msgstr ""
 
 #. Default: "Observations for the votes"
 msgid "PloneMeeting_label_votesObservations"
 msgstr ""
 
-#. Default: "Observations for public meeting"
-msgid "PloneMeeting_label_publicMeetingObservations"
-msgstr ""
-
-#. Default: "Observations for the secret meeting"
-msgid "PloneMeeting_label_secretMeetingObservations"
-msgstr ""
-
 #. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
-msgid "field_vieawable_by_everyone_descr"
+msgid "descr_field_vieawable_by_everyone"
 msgstr ""
 
 #. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
-msgid "field_vieawable_by_everyone_once_meeting_decided_descr"
+msgid "descr_field_vieawable_by_everyone_once_meeting_decided"
 msgstr ""
 
 #. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once item is decided</span>"
 msgid "field_vieawable_by_everyone_once_item_decided_descr"
 msgstr ""
 
 #. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
-msgid "field_reserved_to_meeting_managers_descr"
+msgid "descr_field_reserved_to_meeting_managers"
 msgstr ""
 
-#. Default: "Authority notice"
-msgid "PloneMeeting_label_authorityNotice"
-msgstr ""
-
-#. Default: "Meeting number (sequence number automatically attributed)"
-msgid "PloneMeeting_label_meetingNumber"
-msgstr ""
-
-#. Default: "Number of the first item contained in this meeting"
-msgid "PloneMeeting_label_firstItemNumber"
-msgstr ""
-
-#. Default: "Items"
-msgid "PloneMeeting_label_body"
-msgstr ""
-
-#. Default: "Items"
-msgid "PloneMeeting_label_items"
-msgstr ""
-
-#. Default: "Identifier of the configuration's version that is linked to this meeting"
-msgid "PloneMeeting_label_meetingConfigVersion"
-msgstr ""
-
-#. Default: "Deadline for validating items"
-msgid "PloneMeeting_label_deadlinePublish"
-msgstr ""
-
-#. Default: "Deadline for validating late items"
-msgid "PloneMeeting_label_deadlineFreeze"
+#. Default: "<span style='color: red;'>WARNING, this field is managed by the application and it's value will be \"-1\" until the meeting is frozen, then it will be computed automatically. Do only change it manually when necessary (in general this should never happen). This field is only editable and viewable by meeting managers</span>"
+msgid "descr_config_field_reserved_to_meeting_managers"
 msgstr ""
 
 #. Default: "Agenda"
 msgid "agenda"
 msgstr ""
 
 #. Default: "Decisions"
 msgid "decisions"
 msgstr ""
 
 #. Default: "Meeting of"
 msgid "meeting_of"
 msgstr ""
 
-#. Default: "Signatures"
-msgid "signatures"
-msgstr ""
-
-#. Default: "For the administrator only"
-msgid "for_admin_only"
-msgstr ""
-
 #. Default: "Available items for this meeting"
 msgid "available_items"
 msgstr ""
 
 #. Default: "Items presented to this meeting"
 msgid "presented_items"
 msgstr ""
 
-#. Default: "Items presented tardily"
-msgid "late_presented_items"
-msgstr ""
-
-#. Default: "No items."
-msgid "no_meetingitems"
-msgstr ""
-
 #. Default: "The item is signed."
 msgid "item_is_signed_yes"
 msgstr ""
 
 #. Default: "The item is not signed."
 msgid "item_is_signed_no"
 msgstr ""
@@ -1089,50 +912,14 @@
 msgid "taken_over_by_yes_edit"
 msgstr ""
 
 #. Default: "The item is still not taken over. Click on the image to take it over."
 msgid "taken_over_by_no_edit"
 msgstr ""
 
-#. Default: "The annex is not printable because it can not be converted (unsupported format or error during conversion).  Please use common office formats."
-msgid "annex_to_print_disabled"
-msgstr ""
-
-#. Default: "The annex will be printed."
-msgid "annex_to_print_yes"
-msgstr ""
-
-#. Default: "The annex will not be printed."
-msgid "annex_to_print_no"
-msgstr ""
-
-#. Default: "The annex will be printed. Click on the image not to print it."
-msgid "annex_to_print_yes_edit"
-msgstr ""
-
-#. Default: "The annex will not be printed. Click on the image to print it."
-msgid "annex_to_print_no_edit"
-msgstr ""
-
-#. Default: "The annex is confidential."
-msgid "annex_is_confidential_yes"
-msgstr ""
-
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item."
-msgid "annex_is_confidential_no"
-msgstr ""
-
-#. Default: "The annex is confidential.  Click on the image to set it as not confidential."
-msgid "annex_is_confidential_yes_edit"
-msgstr ""
-
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item.  Click on the image to set it as confidential."
-msgid "annex_is_confidential_no_edit"
-msgstr ""
-
 #. Default: "The advice is confidential."
 msgid "advice_is_confidential_yes"
 msgstr ""
 
 #. Default: "The advice is not confidential and will be visible by everybody who has access to this item."
 msgid "advice_is_confidential_no"
 msgstr ""
@@ -1193,22 +980,14 @@
 msgid "budget_related_no_view"
 msgstr ""
 
 #. Default: "This item is budget related, check \"Budgetary informations\" here under."
 msgid "budget_related_yes_view"
 msgstr ""
 
-#. Default: "Move the item down"
-msgid "move_item_down"
-msgstr ""
-
-#. Default: "Move the item up"
-msgid "move_item_up"
-msgstr ""
-
 #. Default: "Presents all selected items at once."
 msgid "present_several_items"
 msgstr ""
 
 #. Default: "remove all selected items at once."
 msgid "remove_several_items"
 msgstr ""
@@ -1720,32 +1499,24 @@
 msgid "item_templates_descr"
 msgstr ""
 
 #. Default: "No special user is currently defined."
 msgid "no_meeting_user"
 msgstr ""
 
-#. Default: "Default assembly"
-msgid "PloneMeeting_label_assembly"
-msgstr ""
-
 #. Default: "Define here the default assembly (for example you may type a list of names and first names separated by colons or new lines) that will be automatically selected on newly created meetings. If you want a more structured way to define attendees, absents and excused people on a meeting, do not fill this field, create, in the tab \"data\", special users having characteristic \"assembly member\" and select, in the same tab, \"attendees\", \"absents\" and/or \"excused\" attributes as attributes used for a meeting."
 msgid "assembly_descr"
 msgstr ""
 
-#. Default: "Default assembly staves"
-msgid "PloneMeeting_label_assemblyStaves"
-msgstr ""
-
 #. Default: "Define here the default assembly staves (for example you may type a list of names and first names separated by colons or new lines) that will be automatically selected on newly created meetings."
 msgid "assembly_staves_descr"
 msgstr ""
 
 #. Default: "Default signatures"
-msgid "PloneMeeting_label_signatures"
+msgid "title_default_signatures"
 msgstr ""
 
 #. Default: "Define here the default signatures that will be automatically selected on newly created meetings. Use 2 lines by signature, one for the function and one for the signatory name. This will be applicable only if you use attribute \"Signatures\" for meetings."
 msgid "signatures_descr"
 msgstr ""
 
 #. Default: "Group certified signatures"
@@ -1892,30 +1663,14 @@
 msgid "PloneMeeting_label_usedMeetingAttributes"
 msgstr ""
 
 #. Default: "While some meeting attributes are fixed (the title, the date, etc), other attributes (those shown below) are optional. If you select them, they will show up at various places in the user interface (in the form allowing to create meetings, in the screen that displays information about a meeting...)."
 msgid "used_meeting_attributes_descr"
 msgstr ""
 
-#. Default: "Meeting attributes for which history must be kept"
-msgid "PloneMeeting_label_historizedMeetingAttributes"
-msgstr ""
-
-#. Default: "For every field you select here, the application will keep track of any change on any meeting, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
-msgid "historized_meeting_attrs_descr"
-msgstr ""
-
-#. Default: "Meeting states into which events will be recorded in meeting's history"
-msgid "PloneMeeting_label_recordMeetingHistoryStates"
-msgstr ""
-
-#. Default: "Select here the meeting states into which some events related to the meeting will be stored in the meeting's history."
-msgid "record_meeting_history_states_descr"
-msgstr ""
-
 #. Default: "There is a problem with a date defined for group \"${groupName}\".  If the date is in the \"Rule activated for item created until\", it has to be a date in the future.  Moreover, respect following format YYYY/MM/DD, like 2013/12/31."
 msgid "custom_adviser_wrong_date_format"
 msgstr ""
 
 #. Default: "You can not change the logical values of a configuration that has already been used in the application.  Check the configuration for group \"${adviser_group}\", it is in use for example by item at ${item_url}. The old value (${column_old_data}) for column \"${column_name}\" changed. If you need to adapt it, you need to deactivate it by setting a \"For item created until\" date and create another configuration."
 msgid "custom_adviser_can_not_edit_used_row"
 msgstr ""
@@ -2069,14 +1824,18 @@
 msgid "on_all_groups"
 msgstr ""
 
 #. Default: "Follow all associated groups order"
 msgid "on_all_associated_groups"
 msgstr ""
 
+#. Default: "Follow all committees order"
+msgid "on_all_committees"
+msgstr ""
+
 #. Default: "Follow the privacy (order is defined in the field \"Selectable privacies\" here under.)"
 msgid "on_privacy"
 msgstr ""
 
 #. Default: "Follow the poll type"
 msgid "on_poll_type"
 msgstr ""
@@ -2133,38 +1892,14 @@
 msgid "rich_text_remove_blanks"
 msgstr ""
 
 #. Default: "Select here the transform types to apply on the rich text fields selected above."
 msgid "xhtml_transform_types_descr"
 msgstr ""
 
-#. Default: "Default deadline for validating items for a given meeting"
-msgid "PloneMeeting_label_publishDeadlineDefault"
-msgstr ""
-
-#. Default: "Specify here the deadline for validating items to be inserted in a given meeting. You need to express this deadline relative to the meeting date. For example, \"5.9:30\" (do not type quotes) means: \"5 days before the meeting date, at 9:30.\".  Leave the field empty not to use this functionality."
-msgid "publish_deadline_default_descr"
-msgstr ""
-
-#. Default: "Default deadline for validating late items for a given meeting"
-msgid "PloneMeeting_label_freezeDeadlineDefault"
-msgstr ""
-
-#. Default: "Specify here the deadline for validating late items to be inserted in a given meeting.  Leave the field empty not to use this functionality."
-msgid "freeze_deadline_default_descr"
-msgstr ""
-
-#. Default: "Default date for the pre-meeting"
-msgid "PloneMeeting_label_preMeetingDateDefault"
-msgstr ""
-
-#. Default: "Specify here the date of the pre-meeting, relative to its meeting, in the same format as fields above.  Leave the field empty not to use this functionality."
-msgid "pre_meeting_date_default_descr"
-msgstr ""
-
 #. Default: "No annex type is currently defined."
 msgid "no_meeting_file_type"
 msgstr ""
 
 #. Default: "No category is currently defined."
 msgid "no_category"
 msgstr ""
@@ -3181,18 +2916,14 @@
 msgid "sub_types_descr"
 msgstr ""
 
 #. Default: "No subtypes defined."
 msgid "no_sub_types_defined"
 msgstr ""
 
-#. Default: "Predefined title in the second language"
-msgid "PloneMeeting_label_predefinedTitle2"
-msgstr ""
-
 #. Default: "This annex type is specifically linked to the decision taken on this item"
 msgid "PloneMeeting_label_decisionRelated"
 msgstr ""
 
 #. Default: "You can not paste an item coming from another meeting configuration !"
 msgid "cannot_paste_item_from_other_mc"
 msgstr ""
@@ -3923,14 +3654,18 @@
 msgid "required_category_ko"
 msgstr ""
 
 #. Default: "A classifier must be selected on this item so it may evolve in the workflow"
 msgid "required_classifier_ko"
 msgstr ""
 
+#. Default: "A group in charge must be selected on this item so it may evolve in the workflow"
+msgid "required_groupsInCharge_ko"
+msgstr ""
+
 #. Default: "The emergency must be accepted in order to be able to decide the item out of meeting emergency"
 msgid "emergency_accepted_required_to_accept_out_of_meeting_emergency"
 msgstr ""
 
 #. Default: "Pre-validated"
 msgid "icon_help_prevalidated"
 msgstr ""
@@ -3967,18 +3702,14 @@
 msgid "can_not_return_to_meeting_because_of_meeting_state"
 msgstr ""
 
 #. Default: "General"
 msgid "default"
 msgstr ""
 
-#. Default: "Assembly and signatures"
-msgid "assembly_and_signatures"
-msgstr ""
-
 #. Default: "Data"
 msgid "data"
 msgstr ""
 
 #. Default: "Metadata"
 msgid "metadata"
 msgstr ""
@@ -3995,20 +3726,20 @@
 msgid "doc"
 msgstr ""
 
 #. Default: "Emails"
 msgid "mail"
 msgstr ""
 
-#. Default: "Votes"
-msgid "votes"
+#. Default: "Committees"
+msgid "committees"
 msgstr ""
 
-#. Default: "Users"
-msgid "users"
+#. Default: "Votes"
+msgid "votes"
 msgstr ""
 
 #. Default: "Criteria"
 msgid "heading_criteria"
 msgstr ""
 
 #. Default: "Subtypes"
@@ -4695,18 +4426,14 @@
 msgid "error_certified_signatures_duplicated_entries"
 msgstr ""
 
 #. Default: "You can not access this item"
 msgid "can_not_access_this_item"
 msgstr ""
 
-#. Default: "This is an extract of the comment, access full comment if necessary..."
-msgid "This is an extract of the comment, access full comment if necessary..."
-msgstr ""
-
 #. Default: "Comment"
 msgid "Advice comment"
 msgstr ""
 
 #. Default: "${meetingConfigTitle} (to send to)"
 msgid "sent_to_other_mc_term__clonable_to"
 msgstr ""
@@ -4731,50 +4458,22 @@
 msgid "to_be_send_to_authority_term"
 msgstr ""
 
 #. Default: "Not to be send to authority"
 msgid "not_to_be_send_to_authority_term"
 msgstr ""
 
-#. Default: "Annexes to print"
-msgid "annexes_to_print_term"
-msgstr ""
-
-#. Default: "No annexes to print"
-msgid "no_annexes_to_print_term"
-msgstr ""
-
-#. Default: "Annexes to sign"
-msgid "annexes_to_sign_term"
-msgstr ""
-
-#. Default: "Signed annexes"
-msgid "annexes_signed_term"
-msgstr ""
-
-#. Default: "Annexes not to sign"
-msgid "no_annexes_to_sign_term"
-msgstr ""
-
 #. Default: "Item down workflow"
 msgid "item_down_wf_term"
 msgstr ""
 
 #. Default: "Item up workflow again"
 msgid "item_up_wf_term"
 msgstr ""
 
-#. Default: "Normal"
-msgid "list_type_normal"
-msgstr ""
-
-#. Default: "Late"
-msgid "list_type_late"
-msgstr ""
-
 #. Default: "No item template."
 msgid "no_item_templates"
 msgstr ""
 
 #. Default: "Type of item"
 msgid "PloneMeeting_label_listType"
 msgstr ""
@@ -4863,15 +4562,15 @@
 msgid "holidays_wrong_date_format_error"
 msgstr ""
 
 #. Default: "Defined date must be defined by ascending order, from older date at the top to newer date at the bottom."
 msgid "holidays_date_not_ascending_error"
 msgstr ""
 
-#. Default: "You removed a date that is currently in use!"
+#. Default: "You removed a date that is currently in use! Check item at ${item_url}"
 msgid "holidays_removed_date_in_use_error"
 msgstr ""
 
 #. Default: "Keep access to item when an advice"
 msgid "PloneMeeting_label_keepAccessToItemWhenAdvice"
 msgstr ""
 
@@ -4987,15 +4686,15 @@
 msgid "advice_required_to_ask_advices"
 msgstr ""
 
 #. Default: "You are about to change emergency for this item to <span style='font-weight: bold;'>${new_emergency_value}</span>, please enter a comment."
 msgid "change_emergency_descr"
 msgstr ""
 
-#. Default: "Move item to given position"
+#. Default: "Save item number (you may also use the [Enter] key)"
 msgid "move_item_to_given_position"
 msgstr ""
 
 #. Default: "Secret?"
 msgid "Secret while presenting in other MC?"
 msgstr ""
 
@@ -5331,16 +5030,20 @@
 msgid "too_many_categories_use_folder_contents"
 msgstr ""
 
 #. Default: "You can ${force_display} of every categories (may take some time)."
 msgid "categories_force_display_descr"
 msgstr ""
 
+#. Default: "Annexes types are hidden by default, you can ${force_display} of it (may take some time)."
+msgid "annexes_types_force_display_descr"
+msgstr ""
+
 #. Default: "force display"
-msgid "categories_force_display"
+msgid "force_display"
 msgstr ""
 
 #. Default: "You may use the ${folder_contents_link} to manage elements order."
 msgid "categories_use_folder_contents"
 msgstr ""
 
 #. Default: "the \"Folder contents view\""
@@ -5475,40 +5178,48 @@
 msgid "redefinable_assembly_and_signatures"
 msgstr ""
 
 #. Default: "This attendee is marked as signatory for the ${number} following item(s)"
 msgid "This attendee is marked as signatory for the ${number} following item(s)"
 msgstr ""
 
-#. Default: "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
-msgid "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
+#. Default: "The position of this attendee was changed for the ${number} following item(s)"
+msgid "The position of this attendee was changed for the ${number} following item(s)"
 msgstr ""
 
-#. Default: "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
+#. Default: "Original position"
+msgid "Original position"
 msgstr ""
 
-#. Default: "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
+#. Default: "Redefined position"
+msgid "Redefined position"
 msgstr ""
 
-#. Default: "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
+#. Default: "Redefine position for this attendee for this item"
+msgid "Redefine position for this attendee for this item"
 msgstr ""
 
-#. Default: "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
+#. Default: "Remove redefined attendee position for this item"
+msgid "Remove redefined attendee position for this item"
 msgstr ""
 
-#. Default: "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
+#. Default: "Position type to use"
+msgid "Position type to use"
 msgstr ""
 
-#. Default: "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
+#. Default: "Position type to use for the attendee on this item."
+msgid "Position type to use for the attendee on this item."
+msgstr ""
+
+#. Default: "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
+msgid "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
+msgstr ""
+
+#. Default: "Specify a number to which this will be applied. Field default is current item number."
+msgid "Specify a number to which this will be applied. Field default is current item number."
 msgstr ""
 
 #. Default: "Selectable assembly members"
 msgid "PloneMeeting_label_orderedContacts"
 msgstr ""
 
 #. Default: "Select here contacts that will be usable to manage meeting attendees.  The contacts order defined here will be the default order when creating a new meeting."
@@ -5519,14 +5230,22 @@
 msgid "PloneMeeting_label_orderedItemInitiators"
 msgstr ""
 
 #. Default: "Select here contacts that will be usable to manage item initiators.  The contacts order defined here will be useable if relevant."
 msgid "ordered_item_initiators_descr"
 msgstr ""
 
+#. Default: "Restrict selectable redefined position types to following positions"
+msgid "PloneMeeting_label_selectableRedefinedPositionTypes"
+msgstr ""
+
+#. Default: "Select here position types that will be selectable when redefining the position of an attendee for an item.  If nothing selected (default), then any position types is selectable."
+msgid "selectable_redefined_position_types_descr"
+msgstr ""
+
 #. Default: "Signatories"
 msgid "PloneMeeting_label_signatories"
 msgstr ""
 
 #. Default: "Replacements"
 msgid "PloneMeeting_label_replacements"
 msgstr ""
@@ -6119,26 +5838,30 @@
 msgid "app_users"
 msgstr ""
 
 #. Default: "Default ${cfg_title} item template"
 msgid "Default ${cfg_title} item template"
 msgstr ""
 
-#. Default: "You cannot delete the default item template, but you can deactivate it if necessary!"
-msgid "You cannot delete the default item template, but you can deactivate it if necessary!"
+#. Default: "You cannot delete or move the default item template, but you can deactivate it if necessary!"
+msgid "You cannot delete or move the default item template, but you can deactivate it if necessary!"
 msgstr ""
 
 #. Default: "The default item template ${default_template_title} is ${default_template_review_state}."
 msgid "The default item template ${default_template_title} is ${default_template_review_state}."
 msgstr ""
 
-#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by \"${hp_url}\"!"
+#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by held position at \"${hp_url}\"!"
 msgid "removed_position_type_in_use_error"
 msgstr ""
 
+#. Default: "You can not remove a position type that was used as redefined position for an attendee on an item, you removed \"${removed_position_type}\", check attendees on item at \"${item_url}\"!"
+msgid "removed_redefined_position_type_in_use_error"
+msgstr ""
+
 #. Default: "Enabled?"
 msgid "Enabled?"
 msgstr ""
 
 #. Default: "Data that will be used on new item"
 msgid "Data that will be used on new item"
 msgstr ""
@@ -6171,26 +5894,30 @@
 msgid "Represented organizations"
 msgstr ""
 
 #. Default: "Select organizations the current held position is representative for."
 msgid "Select organizations the current held position is representative for."
 msgstr ""
 
-#. Default: "You can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
 msgid "can_not_remove_attendee_redefined_on_items"
 msgstr ""
 
-#. Default: "You can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
 msgid "can_not_remove_public_voter_voted_on_items"
 msgstr ""
 
-#. Default: "You can not unselect a voter that already voted on a secret vote item."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a secret vote item."
 msgid "can_not_remove_secret_voter_voted_on_items"
 msgstr ""
 
+#. Default: "Assembly and signatures : you can not use same signature number several times."
+msgid "can_not_define_several_same_signature_number"
+msgstr ""
+
 #. Default: "You can not remove/disable a function that is used by an item in the application.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_meetingitem"
 msgstr ""
 
 #. Default: "You can not remove/disable a function that is used by an item in the configuration.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_config_meetingitem"
 msgstr ""
@@ -6330,7 +6057,407 @@
 #. Default: "Annexes may only be added by users managing current element but are viewable by every users excepted when using confidentiality."
 msgid "annexes_descr"
 msgstr ""
 
 #. Default: "Category"
 msgid "MeetingCategory"
 msgstr ""
+
+#. Default: "Completed votes"
+msgid "Completed votes"
+msgstr ""
+
+#. Default: "Not completed votes"
+msgid "Not completed votes"
+msgstr ""
+
+#. Default: "Dates and data"
+msgid "fieldset_dates_and_data"
+msgstr ""
+
+#. Default: "Assembly and signatures"
+msgid "fieldset_assembly"
+msgstr ""
+
+#. Default: "Informations"
+msgid "fieldset_informations"
+msgstr ""
+
+#. Default: "Committees"
+msgid "fieldset_committees"
+msgstr ""
+
+#. Default: "Parameters"
+msgid "fieldset_parameters"
+msgstr ""
+
+#. Default: "Date"
+msgid "title_date"
+msgstr ""
+
+#. Default: "Start date"
+msgid "title_start_date"
+msgstr ""
+
+#. Default: "Mid date"
+msgid "title_mid_date"
+msgstr ""
+
+#. Default: "End date"
+msgid "title_end_date"
+msgstr ""
+
+#. Default: "Approval date"
+msgid "title_approval_date"
+msgstr ""
+
+#. Default: "Convocation date"
+msgid "title_convocation_date"
+msgstr ""
+
+#. Default: "Assembly"
+msgid "title_assembly"
+msgstr ""
+
+#. Default: "Assembly excused"
+msgid "title_assembly_excused"
+msgstr ""
+
+#. Default: "Assembly absents"
+msgid "title_assembly_absents"
+msgstr ""
+
+#. Default: "Assembly guests"
+msgid "title_assembly_guests"
+msgstr ""
+
+#. Default: "Assembly proxies"
+msgid "title_assembly_proxies"
+msgstr ""
+
+#. Default: "Assembly staves"
+msgid "title_assembly_staves"
+msgstr ""
+
+#. Default: "Signatures"
+msgid "title_signatures"
+msgstr ""
+
+#. Default: "Assembly observations"
+msgid "title_assembly_observations"
+msgstr ""
+
+#. Default: "Place"
+msgid "title_place"
+msgstr ""
+
+#. Default: "Other place"
+msgid "title_place_other"
+msgstr ""
+
+#. Default: "Pre meeting date"
+msgid "title_pre_meeting_date"
+msgstr ""
+
+#. Default: "Pre meeting place"
+msgid "title_pre_meeting_place"
+msgstr ""
+
+#. Default: "Extraordinary session"
+msgid "title_extraordinary_session"
+msgstr ""
+
+#. Default: "In and out moves"
+msgid "title_in_and_out_moves"
+msgstr ""
+
+#. Default: "Notes"
+msgid "title_notes"
+msgstr ""
+
+#. Default: "Observations"
+msgid "title_observations"
+msgstr ""
+
+#. Default: "Pre observations"
+msgid "title_pre_observations"
+msgstr ""
+
+#. Default: "Committees observations"
+msgid "title_committees_observations"
+msgstr ""
+
+#. Default: "Votes observations"
+msgid "title_votes_observations"
+msgstr ""
+
+#. Default: "Public meeting observations"
+msgid "title_public_meeting_observations"
+msgstr ""
+
+#. Default: "Secret meeting observations"
+msgid "title_secret_meeting_observations"
+msgstr ""
+
+#. Default: "Authority notice"
+msgid "title_authority_notice"
+msgstr ""
+
+#. Default: "Meeting managers notes"
+msgid "title_meetingmanagers_notes"
+msgstr ""
+
+#. Default: "Meeting number"
+msgid "title_meeting_number"
+msgstr ""
+
+#. Default: "First item number (managed automatically when meeting is frozen)"
+msgid "title_first_item_number"
+msgstr ""
+
+#. Default: "Assembly and signatures"
+msgid "assembly_and_signatures"
+msgstr ""
+
+#. Default: "Attendees"
+msgid "title_attendees"
+msgstr ""
+
+#. Default: "Excused"
+msgid "title_excused"
+msgstr ""
+
+#. Default: "Absents"
+msgid "title_absents"
+msgstr ""
+
+#. Default: "Non attendees"
+msgid "title_non_attendees"
+msgstr ""
+
+#. Default: "Signatories"
+msgid "title_signatories"
+msgstr ""
+
+#. Default: "Replacements"
+msgid "title_replacements"
+msgstr ""
+
+#. Default: "Default assembly"
+msgid "title_default_assembly"
+msgstr ""
+
+#. Default: "Default assembly staves"
+msgid "title_default_assembly_staves"
+msgstr ""
+
+#. Default: "Nothing selected in the configuration to be displayed."
+msgid "Nothing selected in the configuration to be displayed."
+msgstr ""
+
+#. Default: "Meeting assembly (${number_of_attendees}) and signatories (${number_of_signatories})"
+msgid "meeting_attendees_and_signatories"
+msgstr ""
+
+#. Default: "These groups will have read access to the item in following states: ${states}.\nWhen icon is green, this means that copy groups have access to the item.\nWhen the label \"[auto]\" is displayed next to the group title, it means that the group was set as copy group automatically by the application."
+msgid "copy_groups_help_msg"
+msgstr ""
+
+#. Default: "${title} (${number}&nbsp;supplement)"
+msgid "committee_title_with_suppl"
+msgstr ""
+
+#. Default: "${title} (${number}&nbsp;s.)"
+msgid "committee_title_with_abbr_suppl"
+msgstr ""
+
+#. Default: "${number}st"
+msgid "num_part_st"
+msgstr ""
+
+#. Default: "${number}th"
+msgid "num_part_th"
+msgstr ""
+
+#. Default: "Committee"
+msgid "title_committees_row_id"
+msgstr ""
+
+#. Default: "Date"
+msgid "title_committees_date"
+msgstr ""
+
+#. Default: "Convocation date"
+msgid "title_committees_convocation_date"
+msgstr ""
+
+#. Default: "Place"
+msgid "title_committees_place"
+msgstr ""
+
+#. Default: "Assembly"
+msgid "title_committees_assembly"
+msgstr ""
+
+#. Default: "Attendees"
+msgid "title_committees_attendees"
+msgstr ""
+
+#. Default: "Signatures"
+msgid "title_committees_signatures"
+msgstr ""
+
+#. Default: "Committees"
+msgid "title_committees"
+msgstr ""
+
+#. Default: "Signatories"
+msgid "title_committees_signatories"
+msgstr ""
+
+#. Default: "You can not remove a configuration that was already used, removed configuration \"${committee_label}\" is used for example by item at ${url}.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committee_row_id_removed_already_used"
+msgstr ""
+
+#. Default: "You can not define values for the \"auto_from\" and \"using_groups\" columns, their use is multually exclusive.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committees_mutually_exclusive_auto_from_and_using_groups"
+msgstr ""
+
+#. Default: "Attendees selectable for committees"
+msgid "PloneMeeting_label_orderedCommitteeContacts"
+msgstr ""
+
+#. Default: "Select here attendees that will be selectable in the \"Attendees\" column of defined committees here under.  <span style='color: red;'>If you select/unselect values, you need to save first then edit again for these values to appear/disappear if field \"Committees\" here under.</span>"
+msgid "ordered_committee_contacts_descr"
+msgstr ""
+
+#. Default: "Committees"
+msgid "PloneMeeting_label_committees"
+msgstr ""
+
+#. Default: "Define committees that will be useable on meetings and items (you also need to enable \"Committees\" on the meeting in the [Data] tab). This will show a \"Committees\" table on the meeting and will be also managed on the item. <br />There are 2 ways to manage committees on the item, either manually or automatically:<ul><li>Manually: just define committees, this will create a multiselection box on the item and users may select it.  It is possible to use the column \"Restrict to\" to define which proposing groups will be able to select the committee;</li><li>Automatically: use the column \"Auto from\" to define which committees to associate to the item depending on proposing group, category or classifier. A MeetingManager is nevertheless able to edit the committee on the item.</li></ul>. These 2 ways are mutually exclusive, if you select values in the \"auto_from\" columb here under, the \"Automatic\" mode will be used."
+msgid "committees_descr"
+msgstr ""
+
+#. Default: "Using a \"Committees\" field requires the use of attribute \"Committees (committees)\"."
+msgid "committees_required"
+msgstr ""
+
+#. Default: "Attributes \"committees_assembly\" and \"committees_attendees\" can't be used together."
+msgid "no_committees_assembly_and_committees_attendees"
+msgstr ""
+
+#. Default: "Attributes \"committees_sigantures\" and \"committees_signatories\" can't be used together."
+msgid "no_committees_signatures_and_committees_signatories"
+msgstr ""
+
+#. Default: "No committee"
+msgid "no_committee_term_title_label"
+msgstr ""
+
+#. Default: "NC"
+msgid "no_committee_term_title_acronym"
+msgstr ""
+
+#. Default: "You can not select \"No committee\" and a committee."
+msgid "can_not_select_no_committee_and_committee"
+msgstr ""
+
+#. Default: "Some selected values are no more selectable (no more selected in the \"Ordered committees contacts\" field), please check value \"${hp_title}\".  You can not select \"No committee\" and a committee.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_value_removed_used_in_committees_field"
+msgstr ""
+
+#. Default: "Signed"
+msgid "annex_term_signed"
+msgstr ""
+
+#. Default: "Confidential"
+msgid "annex_term_confidential"
+msgstr ""
+
+#. Default: "Not confidential"
+msgid "annex_term_not_confidential"
+msgstr ""
+
+#. Default: "Publishable"
+msgid "annex_term_publishable"
+msgstr ""
+
+#. Default: "Not publishable"
+msgid "annex_term_not_publishable"
+msgstr ""
+
+#. Default: "To sign"
+msgid "annex_term_to_sign"
+msgstr ""
+
+#. Default: "Not to sign"
+msgid "annex_term_not_to_sign"
+msgstr ""
+
+#. Default: "To print"
+msgid "annex_term_to_print"
+msgstr ""
+
+#. Default: "Not to print"
+msgid "annex_term_not_to_print"
+msgstr ""
+
+#. Default: "Advice is currently \"Asked again\" do not forget to change value of field \"Advice type\" to another value than \"Asked again\""
+msgid "warning_advice_asked_again_need_to_change_advice_type"
+msgstr ""
+
+#. Default: "This is the date the advice was originally given, this will change when the advice will be considered \"Given\" in a state where it is no more editable"
+msgid "help_given_on_before_started_on"
+msgstr ""
+
+#. Default: "Attendee position has been redefined."
+msgid "Attendee position has been redefined."
+msgstr ""
+
+#. Default: "Redefined attendee position was removed."
+msgid "Redefined attendee position was removed."
+msgstr ""
+
+#. Default: "Warning, there is a problem with encoded data for assembly and signatures, please check especially that signatories are correctly defined"
+msgid "warning_assembly_and_signatures"
+msgstr ""
+
+#. Default: "Not confidential annexes"
+msgid "not_confidential_annexes"
+msgstr ""
+
+#. Default: "Read more"
+msgid "read_more"
+msgstr ""
+
+#. Default: "Read less"
+msgid "read_less"
+msgstr ""
+
+#. Default: "Not able to find a meeting to present this item into.  Only meetings in the future are taken into account, check configuration if necessary"
+msgid "not_able_to_find_meeting_to_present_item_into"
+msgstr ""
+
+#. Default: "Default poll type must be among used poll types"
+msgid "error_default_poll_type_must_be_among_used_poll_types"
+msgstr ""
+
+#. Default: "First linked vote used votes values must be among used vote values"
+msgid "error_first_linked_vote_used_vote_values_must_be_among_used_vote_values"
+msgstr ""
+
+#. Default: "Next linked votes used vote values must be among used vote values"
+msgid "error_next_linked_votes_used_vote_values_must_be_among_used_vote_values"
+msgstr ""
+
+#. Default: "Enabled annexes batch actions"
+msgid "PloneMeeting_label_enabledAnnexesBatchActions"
+msgstr ""
+
+#. Default: "Select the batch actions that will be displayed on the table listing annexes"
+msgid "enabled_annexes_batch_actions_descr"
+msgstr ""
+
+#. Default: "iA.Delib documentation"
+msgid "iA.Delib documentation"
+msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/eea.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/eea.po`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 
 msgid "Category"
 msgstr ""
 
 msgid "Classifier"
 msgstr ""
 
+#. Default: "Committee"
+msgid "Committee"
+msgstr ""
+
 #. Default: "Copy groups"
 msgid "Copy groups"
 msgstr ""
 
 msgid "Created"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.documentgenerator.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.documentgenerator.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.behavior.talcondition.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.behavior.talcondition.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.eeafaceted.batchactions.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.eeafaceted.batchactions.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.iconifiedcategory.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.iconifiedcategory.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/datagridfield.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/datagridfield.po`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,62 @@
 "Language: es\n"
 "X-Is-Fallback-For: es-ar es-bo es-cl es-co es-cr es-do es-ec es-es es-sv es-gt es-hn es-mx es-ni es-pa es-py es-pe es-pr es-us es-uy es-ve\n"
 
 #. Default: "Available on"
 msgid "Available on"
 msgstr ""
 
+#. Default: "Committee acronym"
+msgid "Committee acronym"
+msgstr ""
+
+#. Default: "Committee auto from"
+msgid "Committee auto from"
+msgstr ""
+
+#. Default: "Committee default assembly"
+msgid "Committee default assembly"
+msgstr ""
+
+#. Default: "Committee default attendees"
+msgid "Committee default attendees"
+msgstr ""
+
+#. Default: "Committee default place"
+msgid "Committee default place"
+msgstr ""
+
+#. Default: "Committee default signatories"
+msgid "Committee default signatories"
+msgstr ""
+
+#. Default: "Committee default signatures"
+msgid "Committee default signatures"
+msgstr ""
+
+#. Default: "Committee enabled?"
+msgid "Committee enabled?"
+msgstr ""
+
+#. Default: "Committee label"
+msgid "Committee label"
+msgstr ""
+
+#. Default: "Committee row id"
+msgid "Committee row id"
+msgstr ""
+
+#. Default: "Committee supplements"
+msgid "Committee supplements"
+msgstr ""
+
+#. Default: "Committee using groups"
+msgid "Committee using groups"
+msgstr ""
+
 #. Default: "Full label"
 msgid "Config group full label"
 msgstr ""
 
 #. Default: "Label"
 msgid "Config group label"
 msgstr ""
@@ -313,14 +361,46 @@
 msgid "While sent, the new item is in the workflow initial state, if it was sent automatically (depending on states selected in field 'States in which an item will be automatically sent to selected other meeting configurations' here under), some transitions can be automatically triggered for the new item, select until which transition it will be done (selected transition will also be triggered).  This relies on the 'Transitions for presenting an item' you defined in the 'Workflows' tab of the meeting configuration the item will be sent to."
 msgstr ""
 
 #. Default: "Specify here a TAL expression that will restrict or allow the use of this advice to some condition.  We receive \"item\" as the meeting item to give an advice on and \"mayEdit\", a boolean to know if current user may edit the item.  A special expression is available to protect a row that should only be available thru the \"Change delay\" action, it is : \"python: item.REQUEST.get('managing_available_delays', False)\".  This can not be used if something is defined in the \"Advice will be automatically asked if\" column of this advice, but for optional delay-aware advice or for delay-aware advices linked to an automatic advice (using the \"Is linked to previous row?\" column)"
 msgid "available_on_col_description"
 msgstr ""
 
+#. Default: "Used to automatically determinate the committee for the item, the field \"Committees\" will not appear on the item when editing it (except for MeetingManagers).  This may only be used when column \"using_groups\" is not used."
+msgid "committees_auto_from_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Assembly\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_assembly_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Attendees\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_attendees_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Place\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_place_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Signatories\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatories_col_description"
+msgstr ""
+
+#. Default: "Used when creating a new meeting if field \"Signatures\" is enabled for committees, does not impact already created meetings."
+msgid "committees_default_signatures_col_description"
+msgstr ""
+
+#. Default: "Will generate new values on item \"Committees\" field when necessary to manage supplements (items added to meeting after committees convocation were sent).  This will only be useable by MeetingManagers."
+msgid "committees_supplements_col_description"
+msgstr ""
+
+#. Default: "Used to restrict availability of a committee on the item committees selection box.  This may only be used when column \"auto_from\" is not used."
+msgid "committees_using_groups_col_description"
+msgstr ""
+
 #. Default: "Enter the delay the adviser will have to give his advice. If it is not considered as an automatically asked advice (nothing defined in the \"Advice will be automatically asked if\" column), the advice will be selectable in the \"Ask advice to\" list on the item edit form. A delay is a single digit (like \"5\" or \"10\"). If no delay is relevant for this advice, leave this field blank. If several delays are possible for the same advice, you have to define several rows with exactly the same content excepted the delay."
 #, fuzzy
 msgid "delay_col_description"
 msgstr "Introduzca el retraso en que el asesor tendrá que dar su consejo. Si no se considera como un consejo pedido automáticamente (no hay nada definido en columna la 'Si el Consejo se le pedirá automáticamente'), el consejo se podrá seleccionar en la lista 'Pida consejo a' en el formulario de elemento de edición. El retraso es de un solo dígito (como '5' o '10'). Si hay retraso es relevante para este consejo, deje este campo en blanco. Si varios retrasos son posibles para el mismo consejo, usted tiene que definir varias filas con exactamente el mismo contenido exceptúa la demora."
 
 #. Default: "If you want a specific label to be displayed on the label displayed in the \"Advice to give\" list on the item edit form and on the \"?\" displayed next to the advice title in the user interface, you can enter it here.  The label will appear between brackets after the message \"Name of the group - delay of X days\"."
 #, fuzzy
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/PloneMeeting.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/PloneMeeting.po`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 msgid "${term_title} (Not selected in plonegroup)"
 msgstr ""
 
 #. Default: "(Nobody)"
 msgid "(Nobody)"
 msgstr ""
 
+#. Default: "(None)"
+msgid "(None)"
+msgstr ""
+
 #. Default: "Add PloneMeeting Portlet"
 msgid "Add PloneMeeting Portlet"
 msgstr "Agregar Portlet PloneMeeting"
 
 #. Default: "Add Todo Portlet"
 msgid "Add Todo Portlet"
 msgstr "Agregar Portlet Todo"
@@ -160,14 +164,18 @@
 msgid "Attendee has been set signatory."
 msgstr ""
 
 #. Default: "Attendee is no more defined as item signatory."
 msgid "Attendee is no more defined as item signatory."
 msgstr ""
 
+#. Default: "Attendee position has been redefined."
+msgid "Attendee position has been redefined."
+msgstr ""
+
 #. Default: "Back to the MeetingConfig"
 msgid "Back to the MeetingConfig"
 msgstr ""
 
 #. Default: "Back to the item"
 msgid "Back to the item"
 msgstr ""
@@ -244,14 +252,18 @@
 msgid "Close"
 msgstr "Cerrar"
 
 #. Default: "Comment"
 msgid "Comment"
 msgstr ""
 
+#. Default: "Completed votes"
+msgid "Completed votes"
+msgstr ""
+
 #. Default: "Contacts fields"
 msgid "Contacts fields"
 msgstr ""
 
 #. Default: "Copy PloneMeeting"
 msgid "Copy PloneMeeting"
 msgstr "Copiar PloneMeeting"
@@ -472,38 +484,14 @@
 msgid "If you need to use this person data in the application like for example scanned signature or telephone number, select it here."
 msgstr ""
 
 #. Default: "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 msgid "If you specify a number, the values entered here above will be applied from current item to the item number entered. Leave empty to only apply for current item."
 msgstr ""
 
-#. Default: "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as absent from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as attendee for the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as back into the meeting from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as non attendee from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will be defined as signatory from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
-#. Default: "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgid "If you specify a number, this attendee will no longer be considered item signatory from current item to entered item number. Leave empty to only apply for current item."
-msgstr ""
-
 # plone.app.querystring
 #. Default: "Informations about advices on an item"
 msgid "Informations about advices on an item"
 msgstr ""
 
 #. Default: "Inherited advice action"
 msgid "Inherited advice action"
@@ -743,22 +731,30 @@
 msgid "None"
 msgstr ""
 
 #. Default: "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 msgid "Not able to add new linked votes because incompatible vote vales have been encoded on current vote"
 msgstr ""
 
+#. Default: "Not completed votes"
+msgid "Not completed votes"
+msgstr ""
+
 #. Default: "Not present type"
 msgid "Not present type"
 msgstr ""
 
 #. Default: "Not voter"
 msgid "Not voter"
 msgstr ""
 
+#. Default: "Nothing selected in the configuration to be displayed."
+msgid "Nothing selected in the configuration to be displayed."
+msgstr ""
+
 #. Default: "Nothing to display when item is not presented into a meeting."
 msgid "Nothing to display when item is not presented into a meeting."
 msgstr ""
 
 #. Default: "Nothing to display."
 msgid "Nothing to display."
 msgstr ""
@@ -787,14 +783,18 @@
 msgid "Ordered groups"
 msgstr ""
 
 #. Default: "Original meeting signatory"
 msgid "Original meeting signatory"
 msgstr ""
 
+#. Default: "Original position"
+msgid "Original position"
+msgstr ""
+
 #. Default: "POD template to annex"
 msgid "POD template to annex"
 msgstr ""
 
 #. Default: "Please check item number ${item_number} at ${item_url}."
 msgid "Please check item number ${item_number} at ${item_url}."
 msgstr ""
@@ -828,22 +828,14 @@
 msgid "PloneMeeting_inAndOutMoves"
 msgstr ""
 
 #. Default: "Observations"
 msgid "PloneMeeting_itemObservations"
 msgstr "Observaciones"
 
-#. Default: "Observations"
-msgid "PloneMeeting_itemObservations2"
-msgstr "Observaciones"
-
-#. Default: "Absents"
-msgid "PloneMeeting_label_absents"
-msgstr "Ausentes"
-
 # MeetingGroup
 #. Default: "Acronym"
 msgid "PloneMeeting_label_acronym"
 msgstr "Acrónimo"
 
 #. Default: "Confidential advice annexes are visible for"
 msgid "PloneMeeting_label_adviceAnnexConfidentialVisibleFor"
@@ -881,50 +873,26 @@
 msgid "PloneMeeting_label_annexToPrintMode"
 msgstr ""
 
 #. Default: "Answers"
 msgid "PloneMeeting_label_answerers"
 msgstr "Respuestas"
 
-#. Default: "Meeting approval date"
-msgid "PloneMeeting_label_approvalDate"
-msgstr ""
-
 #. Default: "As copy group on"
 msgid "PloneMeeting_label_asCopyGroupOn"
 msgstr "Como grupo de copia"
 
-#. Default: "Default assembly"
-msgid "PloneMeeting_label_assembly"
-msgstr "Asamblea por defecto"
-
-#. Default: "Default assembly staves"
-msgid "PloneMeeting_label_assemblyStaves"
-msgstr ""
-
 #. Default: "Associated group(s)"
 msgid "PloneMeeting_label_associatedGroups"
 msgstr "Grupo(s) asociados"
 
-#. Default: "Attendees"
-msgid "PloneMeeting_label_attendees"
-msgstr "Asistentes"
-
-#. Default: "Authority notice"
-msgid "PloneMeeting_label_authorityNotice"
-msgstr ""
-
 #. Default: "Columns to display for items available for a meeting"
 msgid "PloneMeeting_label_availableItemsListVisibleColumns"
 msgstr ""
 
-#. Default: "Items"
-msgid "PloneMeeting_label_body"
-msgstr "Temas"
-
 #. Default: "Default value for the \"budget information\" field"
 #, fuzzy
 msgid "PloneMeeting_label_budgetDefault"
 msgstr "Valor por defecto para el campo de 'Información presupuestaria'"
 
 #. Default: "Budgetary informations"
 msgid "PloneMeeting_label_budgetInfos"
@@ -954,14 +922,18 @@
 msgid "PloneMeeting_label_classifier"
 msgstr ""
 
 #. Default: "Observations for the committee"
 msgid "PloneMeeting_label_committeeObservations"
 msgstr ""
 
+#. Default: "Committees"
+msgid "PloneMeeting_label_committees"
+msgstr ""
+
 #. Default: "Completeness"
 msgid "PloneMeeting_label_completeness"
 msgstr ""
 
 #. Default: "Group of meeting configurations"
 msgid "PloneMeeting_label_configGroup"
 msgstr ""
@@ -978,18 +950,14 @@
 msgid "PloneMeeting_label_configVersion"
 msgstr "Identidad de esta configuración de reunión"
 
 #. Default: "Contents to keep when item sent to another configuration"
 msgid "PloneMeeting_label_contentsKeptOnSentToOtherMC"
 msgstr ""
 
-#. Default: "Meeting convocation date"
-msgid "PloneMeeting_label_convocationDate"
-msgstr ""
-
 #. Default: "Copy groups"
 msgid "PloneMeeting_label_copyGroups"
 msgstr "Copia de grupos"
 
 #. Default: "Css classes to hide"
 msgid "PloneMeeting_label_cssClassesToHide"
 msgstr ""
@@ -1006,26 +974,14 @@
 msgid "PloneMeeting_label_dashboardMeetingAvailableItemsFilters"
 msgstr ""
 
 #. Default: "Advanced filters to show on \"Items of a meeting\""
 msgid "PloneMeeting_label_dashboardMeetingLinkedItemsFilters"
 msgstr ""
 
-#. Default: "Date"
-msgid "PloneMeeting_label_date"
-msgstr "Fecha"
-
-#. Default: "Deadline for validating late items"
-msgid "PloneMeeting_label_deadlineFreeze"
-msgstr "Limite para la validación de temas retardados"
-
-#. Default: "Deadline for validating items"
-msgid "PloneMeeting_label_deadlinePublish"
-msgstr "Limites para la validación de temas"
-
 #. Default: "Decision"
 msgid "PloneMeeting_label_decision"
 msgstr "Decisión"
 
 #. Default: "Decision (end)"
 msgid "PloneMeeting_label_decisionEnd"
 msgstr ""
@@ -1062,26 +1018,18 @@
 msgid "PloneMeeting_label_delayUnavailableEndDays"
 msgstr ""
 
 #. Default: "Description"
 msgid "PloneMeeting_label_description"
 msgstr "Descripción"
 
-#. Default: "Description in the second language"
-msgid "PloneMeeting_label_description2"
-msgstr "Descripción en el segundo idioma"
-
 #. Default: "Detailed description"
 msgid "PloneMeeting_label_detailedDescription"
 msgstr "Descripción detallada"
 
-#. Default: "Detailed description"
-msgid "PloneMeeting_label_detailedDescription2"
-msgstr "Descripción detallada"
-
 #. Default: "Display available items to"
 msgid "PloneMeeting_label_displayAvailableItemsTo"
 msgstr ""
 
 #. Default: "Emergency"
 msgid "PloneMeeting_label_emergency"
 msgstr ""
@@ -1106,46 +1054,30 @@
 msgid "PloneMeeting_label_enableScanDocs"
 msgstr ""
 
 #. Default: "Enable user preferences"
 msgid "PloneMeeting_label_enableUserPreferences"
 msgstr "Habilitar preferencias de usuario"
 
-#. Default: "Effective end date and hour"
-msgid "PloneMeeting_label_endDate"
-msgstr "Fecha y hora de culminación vigente"
+#. Default: "Enabled annexes batch actions"
+msgid "PloneMeeting_label_enabledAnnexesBatchActions"
+msgstr ""
 
 #. Default: "Enforce advice mandatoriness"
 msgid "PloneMeeting_label_enforceAdviceMandatoriness"
 msgstr "Hacer cumplir consejos obligatorios"
 
-#. Default: "Excused"
-msgid "PloneMeeting_label_excused"
-msgstr "Excusado"
-
-#. Default: "Extraordinary session?"
-msgid "PloneMeeting_label_extraordinarySession"
-msgstr ""
-
-#. Default: "Number of the first item contained in this meeting"
-msgid "PloneMeeting_label_firstItemNumber"
-msgstr "Número del primer tema contenido en esta reunión"
-
 #. Default: "First linked vote values"
 msgid "PloneMeeting_label_firstLinkedVoteUsedVoteValues"
 msgstr ""
 
 #. Default: "Name of the folder linked to this configuration"
 msgid "PloneMeeting_label_folderTitle"
 msgstr "Nombre de la carpeta enlazada a esta configuración"
 
-#. Default: "Default deadline for validating late items for a given meeting"
-msgid "PloneMeeting_label_freezeDeadlineDefault"
-msgstr "Limite por defecto para la validación de temas retardados para una reunión dada"
-
 #. Default: "Email of the functional administrator"
 msgid "PloneMeeting_label_functionalAdminEmail"
 msgstr "Correo electrónico del administrador funcional"
 
 #. Default: "Name of the functional administrator"
 msgid "PloneMeeting_label_functionalAdminName"
 msgstr "Nombre del administrador funcional"
@@ -1186,18 +1118,14 @@
 msgid "PloneMeeting_label_historizeItemDataWhenAdviceIsGiven"
 msgstr ""
 
 #. Default: "Item attributes for which history must be kept"
 msgid "PloneMeeting_label_historizedItemAttributes"
 msgstr "Atributos del tema para los cuales se debe mantener el histórico"
 
-#. Default: "Meeting attributes for which history must be kept"
-msgid "PloneMeeting_label_historizedMeetingAttributes"
-msgstr "Atributos para los cuales se debe mantener el histórico de las reuniones"
-
 #. Default: "Holidays"
 msgid "PloneMeeting_label_holidays"
 msgstr ""
 
 #. Default: "Include groups in charge defined on category"
 msgid "PloneMeeting_label_includeGroupsInChargeDefinedOnCategory"
 msgstr ""
@@ -1376,18 +1304,14 @@
 msgid "PloneMeeting_label_itemWithGivenAdviceIsNotDeletable"
 msgstr ""
 
 #. Default: "Workflow that dictates the life cycle of every item into this configuration"
 msgid "PloneMeeting_label_itemWorkflow"
 msgstr "Flujo de trabajo que dicta el ciclo de vida de cada tema dentro de esta configuración"
 
-#. Default: "Items"
-msgid "PloneMeeting_label_items"
-msgstr "Temas"
-
 #. Default: "Columns to display for items within a meeting"
 #, fuzzy
 msgid "PloneMeeting_label_itemsListVisibleColumns"
 msgstr "Las columnas a mostrar en los temas dentro de las reuniones"
 
 #. Default: "Fields of the items to show/hide in the dashboards"
 msgid "PloneMeeting_label_itemsListVisibleFields"
@@ -1478,18 +1402,14 @@
 msgid "PloneMeeting_label_meetingColumns"
 msgstr "Las columnas a mostrar en las listas de reuniones"
 
 #. Default: "Interface allowing to use a specific Zope3 adapter for modifying the conditions defined on the transitions of the meeting workflow"
 msgid "PloneMeeting_label_meetingConditionsInterface"
 msgstr "La interfaz siguiente es usada para un especifico adaptador de Zope3 para modificar las acciones definidas en las transiciones del flujo de trabajo de reunión"
 
-#. Default: "Identifier of the configuration's version that is linked to this meeting"
-msgid "PloneMeeting_label_meetingConfigVersion"
-msgstr "Identificación de la versión de configuración que esta enlazada con esta reunión"
-
 #. Default: "Meeting configs to clone items to"
 msgid "PloneMeeting_label_meetingConfigsToCloneTo"
 msgstr "Configuraciones de reuniones para clonar los temas hacia"
 
 #. Default: "Title of the folder created in each user folder"
 #, fuzzy
 msgid "PloneMeeting_label_meetingFolderTitle"
@@ -1507,58 +1427,38 @@
 msgid "PloneMeeting_label_meetingManagersNotesEnd"
 msgstr ""
 
 #. Default: "MeetingManagers notes (suite)"
 msgid "PloneMeeting_label_meetingManagersNotesSuite"
 msgstr ""
 
-#. Default: "Meeting number (sequence number automatically attributed)"
-msgid "PloneMeeting_label_meetingNumber"
-msgstr "Número de reuniones (secuencia de números atribuidos automáticamente)"
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations"
-msgstr "Observaciones"
-
-#. Default: "Observations"
-msgid "PloneMeeting_label_meetingObservations2"
-msgstr "Observaciones"
-
 #. Default: "States of the meeting to insert an item into from everywhere"
 msgid "PloneMeeting_label_meetingPresentItemWhenNoCurrentMeetingStates"
 msgstr ""
 
 #. Default: "Meeting transition that triggers the insertion of this item as a recurring item"
 msgid "PloneMeeting_label_meetingTransitionInsertingMe"
 msgstr "Transición de reunión de activa la inserción de este tema como un tema recurrente"
 
 #. Default: "Workflow that dictates the life cycle of every meeting into this configuration"
 msgid "PloneMeeting_label_meetingWorkflow"
 msgstr "Flujo de trabajo que dicta el ciclo de vida de cada reunión dentro de esta configuración"
 
-#. Default: "End date for meeting first part"
-msgid "PloneMeeting_label_midDate"
-msgstr "Fecha de culminación para la primera parte de la reunión"
-
 #. Default: "Model adaptations"
 msgid "PloneMeeting_label_modelAdaptations"
 msgstr "Adaptaciones del Modelo"
 
 #. Default: "Motivation"
 msgid "PloneMeeting_label_motivation"
 msgstr "Motivación"
 
 #. Default: "Next linked votes values"
 msgid "PloneMeeting_label_nextLinkedVotesUsedVoteValues"
 msgstr ""
 
-#. Default: "Non attendees"
-msgid "PloneMeeting_label_nonAttendees"
-msgstr ""
-
 #. Default: "Actions to execute on items of a meeting when a transition is triggered on that meeting"
 msgid "PloneMeeting_label_onMeetingTransitionItemActionToExecute"
 msgstr ""
 
 #. Default: "Transforms to apply to rich text fields of an item after a workflow transition"
 msgid "PloneMeeting_label_onTransitionFieldTransforms"
 msgstr ""
@@ -1575,14 +1475,18 @@
 msgid "PloneMeeting_label_oralQuestion"
 msgstr "¿Pregunta Oral?"
 
 #. Default: "Associated organizations order"
 msgid "PloneMeeting_label_orderedAssociatedOrganizations"
 msgstr ""
 
+#. Default: "Attendees selectable for committees"
+msgid "PloneMeeting_label_orderedCommitteeContacts"
+msgstr ""
+
 #. Default: "Selectable assembly members"
 msgid "PloneMeeting_label_orderedContacts"
 msgstr ""
 
 #. Default: "Ordered groups in charge"
 msgid "PloneMeeting_label_orderedGroupsInCharge"
 msgstr ""
@@ -1607,18 +1511,14 @@
 msgid "PloneMeeting_label_otherMeetingConfigsClonableToPrivacy"
 msgstr ""
 
 #. Default: "Owner of a annex decision may delete it when item is no more editable?"
 msgid "PloneMeeting_label_ownerMayDeleteAnnexDecision"
 msgstr ""
 
-#. Default: "Place"
-msgid "PloneMeeting_label_place"
-msgstr "Lugar"
-
 #. Default: "Meeting places"
 msgid "PloneMeeting_label_places"
 msgstr "Lugares de reunión"
 
 #. Default: "Poll type"
 msgid "PloneMeeting_label_pollType"
 msgstr ""
@@ -1632,42 +1532,18 @@
 msgid "PloneMeeting_label_powerAdvisersGroups"
 msgstr "Grupos a considerar como 'asesores potenciales'"
 
 #. Default: "Manage power observers"
 msgid "PloneMeeting_label_powerObservers"
 msgstr ""
 
-#. Default: "Date"
-msgid "PloneMeeting_label_preMeetingDate"
-msgstr "Fecha"
-
-#. Default: "Default date for the pre-meeting"
-msgid "PloneMeeting_label_preMeetingDateDefault"
-msgstr "Fecha por defecto para la reunión previa"
-
-#. Default: "Place"
-msgid "PloneMeeting_label_preMeetingPlace"
-msgstr "Lugar"
-
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations"
-msgstr "Observaciones para la reunión preparatoria"
-
-#. Default: "Observations for the preparatory meeting"
-msgid "PloneMeeting_label_preObservations2"
-msgstr "Observaciones para la reunión preparatoria"
-
 #. Default: "Previous item"
 msgid "PloneMeeting_label_predecessor"
 msgstr "Temas vinculados"
 
-#. Default: "Predefined title in the second language"
-msgid "PloneMeeting_label_predefinedTitle2"
-msgstr "Título predefinido en el segundo idioma"
-
 #. Default: "Preferred meeting"
 msgid "PloneMeeting_label_preferredMeeting"
 msgstr "Reunión preferida"
 
 #. Default: "Privacy"
 msgid "PloneMeeting_label_privacy"
 msgstr "Privacidad"
@@ -1676,38 +1552,26 @@
 msgid "PloneMeeting_label_proposingGroup"
 msgstr "Grupo propuesto"
 
 #. Default: "Proposing group (Group in charge)"
 msgid "PloneMeeting_label_proposingGroupWithGroupInCharge"
 msgstr ""
 
-#. Default: "Observations for public meeting"
-msgid "PloneMeeting_label_publicMeetingObservations"
-msgstr ""
-
 #. Default: "Public URL"
 msgid "PloneMeeting_label_publicUrl"
 msgstr "Dirección URL Pública"
 
-#. Default: "Default deadline for validating items for a given meeting"
-msgid "PloneMeeting_label_publishDeadlineDefault"
-msgstr "Limite por defecto para la validación de temas para una reunión dada"
-
 #. Default: "Questions"
 msgid "PloneMeeting_label_questioners"
 msgstr "Preguntas"
 
 #. Default: "Item states into which events will be recorded in item's history"
 msgid "PloneMeeting_label_recordItemHistoryStates"
 msgstr "Los estados de temas en los que los eventos serán registrados en el historial del tema"
 
-#. Default: "Meeting states into which events will be recorded in meeting's history"
-msgid "PloneMeeting_label_recordMeetingHistoryStates"
-msgstr "Los estados de reunión en los cuales los eventos serán registrados en el historial de la reunión"
-
 #. Default: "Redirect to the next meeting"
 msgid "PloneMeeting_label_redirectToNextMeeting"
 msgstr ""
 
 #. Default: "Remove annexes previews on meeting closure"
 msgid "PloneMeeting_label_removeAnnexesPreviewsOnMeetingClosure"
 msgstr ""
@@ -1725,30 +1589,30 @@
 msgstr ""
 
 #. Default: "\"Restrict users\" mode"
 #, fuzzy
 msgid "PloneMeeting_label_restrictUsers"
 msgstr "Modo 'usuarios restringidos'"
 
-#. Default: "Observations for the secret meeting"
-msgid "PloneMeeting_label_secretMeetingObservations"
-msgstr ""
-
 #. Default: "Selectable advisers"
 msgid "PloneMeeting_label_selectableAdvisers"
 msgstr ""
 
 #. Default: "Groups that can be in copy for an item"
 msgid "PloneMeeting_label_selectableCopyGroups"
 msgstr "Grupos que pueden copiar este tema"
 
 #. Default: "Selectable privacies"
 msgid "PloneMeeting_label_selectablePrivacies"
 msgstr ""
 
+#. Default: "Restrict selectable redefined position types to following positions"
+msgid "PloneMeeting_label_selectableRedefinedPositionTypes"
+msgstr ""
+
 #. Default: "Is group selectable in the plonegroup configuration panel?"
 msgid "PloneMeeting_label_selectable_for_plonegroup"
 msgstr ""
 
 #. Default: "Send to authority?"
 msgid "PloneMeeting_label_sendToAuthority"
 msgstr ""
@@ -1761,26 +1625,18 @@
 msgid "PloneMeeting_label_showItemKeywordsTargets"
 msgstr "Mostrar los posibles objetivos para palabras clave del tema"
 
 #. Default: "Signatories"
 msgid "PloneMeeting_label_signatories"
 msgstr ""
 
-#. Default: "Default signatures"
-msgid "PloneMeeting_label_signatures"
-msgstr "Firmas por defecto"
-
 #. Default: "Sort the tags alphabetically"
 msgid "PloneMeeting_label_sortAllItemTags"
 msgstr "Soportar la etiquetas alfabéticamente "
 
-#. Default: "Effective start date and hour"
-msgid "PloneMeeting_label_startDate"
-msgstr "Fecha y hora de inicio vigente"
-
 #. Default: "Meeting file sub types"
 msgid "PloneMeeting_label_subTypes"
 msgstr ""
 
 #. Default: "Taken over by"
 msgid "PloneMeeting_label_takenOverBy"
 msgstr ""
@@ -1789,23 +1645,14 @@
 msgid "PloneMeeting_label_templateUsingGroups"
 msgstr "Restringir el uso de esta plantilla para los grupos siguientes"
 
 #. Default: "Checklist"
 msgid "PloneMeeting_label_textCheckList"
 msgstr ""
 
-# Meeting
-#. Default: "Title"
-msgid "PloneMeeting_label_title"
-msgstr "Título"
-
-#. Default: "Title in the second language"
-msgid "PloneMeeting_label_title2"
-msgstr "Titulo en el segundo idioma"
-
 #. Default: "To discuss ?"
 msgid "PloneMeeting_label_toDiscuss"
 msgstr "¿A discutir?"
 
 #. Default: "Default value of the \"toDiscuss\" attribute for normal items"
 #, fuzzy
 msgid "PloneMeeting_label_toDiscussDefault"
@@ -1930,38 +1777,38 @@
 msgid "PloneMeeting_label_xhtmlTransformTypes"
 msgstr "Tipos de transformaciones de texto enriquecido"
 
 #. Default: "Reinitialise meeting number every year?"
 msgid "PloneMeeting_label_yearlyInitMeetingNumber"
 msgstr "¿Reinicializar número de reunión cada año?"
 
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations"
-msgstr "Observaciones"
-
-#. Default: "Observations"
-msgid "PloneMeeting_meetingObservations2"
-msgstr "Observaciones"
-
 #. Default: "Notes"
 msgid "PloneMeeting_notes"
 msgstr ""
 
 #. Default: "Document templates"
 msgid "PodTemplates"
 msgstr "Plantillas de documento"
 
 #. Default: "Position type"
 msgid "Position type"
 msgstr ""
 
+#. Default: "Position type to use"
+msgid "Position type to use"
+msgstr ""
+
 #. Default: "Position type to use as label for the signature."
 msgid "Position type to use as label for the signature."
 msgstr ""
 
+#. Default: "Position type to use for the attendee on this item."
+msgid "Position type to use for the attendee on this item."
+msgstr ""
+
 #. Default: "Preview detailed advice"
 msgid "Preview detailed advice"
 msgstr ""
 
 #. Default: "Preview of annexes were deleted upon meeting closure."
 msgid "Preview of annexes were deleted upon meeting closure."
 msgstr ""
@@ -1971,14 +1818,26 @@
 msgid "Previous review state"
 msgstr ""
 
 #. Default: "Recurring items"
 msgid "RecurringItems"
 msgstr "Temas predefinidos"
 
+#. Default: "Redefine position for this attendee for this item"
+msgid "Redefine position for this attendee for this item"
+msgstr ""
+
+#. Default: "Redefined attendee position was removed."
+msgid "Redefined attendee position was removed."
+msgstr ""
+
+#. Default: "Redefined position"
+msgid "Redefined position"
+msgstr ""
+
 #. Default: "References of contained items have been updated."
 msgid "References of contained items have been updated."
 msgstr ""
 
 #. Default: "Reinitiatlize delay"
 msgid "Reinitiatlize delay"
 msgstr ""
@@ -1995,14 +1854,18 @@
 msgid "Remove inherited advice"
 msgstr ""
 
 #. Default: "Remove inherited advice and ask advice locally"
 msgid "Remove inherited advice and ask advice locally"
 msgstr ""
 
+#. Default: "Remove redefined attendee position for this item"
+msgid "Remove redefined attendee position for this item"
+msgstr ""
+
 #. Default: "Represented organizations"
 msgid "Represented organizations"
 msgstr ""
 
 #. Default: "Searches"
 msgid "Searches"
 msgstr ""
@@ -2055,14 +1918,18 @@
 msgid "Signature number"
 msgstr ""
 
 #. Default: "Signature position type"
 msgid "Signature position type"
 msgstr ""
 
+#. Default: "Specify a number to which this will be applied. Field default is current item number."
+msgid "Specify a number to which this will be applied. Field default is current item number."
+msgstr ""
+
 #. Default: "state"
 msgid "State"
 msgstr "Estado"
 
 #. Default: "Style templates"
 msgid "Style templates"
 msgstr ""
@@ -2106,14 +1973,18 @@
 msgstr ""
 
 # plone.app.querystring
 #. Default: "The item, advice or meeting previous review state"
 msgid "The item, advice or meeting previous review state"
 msgstr ""
 
+#. Default: "The position of this attendee was changed for the ${number} following item(s)"
+msgid "The position of this attendee was changed for the ${number} following item(s)"
+msgstr ""
+
 #. Default: "There was an error during annex conversion, please contact system administrator."
 msgid "There was an error during annex conversion, please contact system administrator."
 msgstr "Se produjo un error durante la conversión del anexo, por favor, póngase en contacto con el administrador del sistema."
 
 #. Default: "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
 msgid "There was an error while trying to set this annex to printable. The error message was : ${error}. Please contact system administrator."
 msgstr "Se produjo un error al intentar configurar este anexo como imprimible. El mensaje de error fue: ${error}. Por favor, póngase en contacto con el administrador del sistema."
@@ -2154,18 +2025,14 @@
 msgid "This automatic advice has been asked by the application (shown by his title not being between brackets)"
 msgstr "Este consejo automático ha sido preguntado por la aplicación (que se muestra por su título no está entre paréntesis)"
 
 #. Default: "This copy group was set automatically by the application"
 msgid "This copy group was set automatically by the application"
 msgstr ""
 
-#. Default: "This is an extract of the comment, access full comment if necessary..."
-msgid "This is an extract of the comment, access full comment if necessary..."
-msgstr ""
-
 #. Default: "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 msgid "This item is not viewable by the advisers of this group in the current review state (${item_review_state})."
 msgstr ""
 
 #. Default: "This label can not be removed as it is used by some items, for example ${item_url}"
 msgid "This label can not be removed as it is used by some items, for example ${item_url}"
 msgstr ""
@@ -2247,16 +2114,16 @@
 msgid "Votes are not completed for following ${number} ${polltype} item(s)"
 msgstr ""
 
 #. Default: "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 msgid "You are about to change delay for this advice to ${new_advice_delay} days, you can enter a comment if necessary."
 msgstr ""
 
-#. Default: "You cannot delete the default item template, but you can deactivate it if necessary!"
-msgid "You cannot delete the default item template, but you can deactivate it if necessary!"
+#. Default: "You cannot delete or move the default item template, but you can deactivate it if necessary!"
+msgid "You cannot delete or move the default item template, but you can deactivate it if necessary!"
 msgstr ""
 
 #. Default: "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 msgid "You cannot delete the held position \"${held_position_title}\", because it is used by element at \"${obj_url}\" !"
 msgstr ""
 
 #. Default: "Not grouped meeting configurations"
@@ -2494,78 +2361,78 @@
 msgid "annexAdded_mail_subject"
 msgstr "${portalTitle} - ${meetingTitle} - Un anexo se acaba de agregar a un tema."
 
 #. Default: "If an annex is marked as \"Confidential\" by a meeting manager, following selected profiles will not be able to see it."
 msgid "annex_confidential_for_descr"
 msgstr ""
 
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item."
-msgid "annex_is_confidential_no"
+#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" could not be kept because it was not possible to find a corresponding annex type in the destination meeting configuration, please contact system administrator."
+msgid "annex_not_kept_because_no_available_annex_type_warning"
 msgstr ""
 
-#. Default: "The annex is not confidential and will be visible by everybody who has access to this item.  Click on the image to set it as confidential."
-msgid "annex_is_confidential_no_edit"
+#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" was not kept because using a scan_id, please contact system administrator."
+msgid "annex_not_kept_because_using_scan_id"
 msgstr ""
 
-#. Default: "The annex is confidential."
-msgid "annex_is_confidential_yes"
+#. Default: "Select for each optional annexes attributes which are only displayed or editable by MeetingManagers.  If an attribute is only displayed to MeetingManagers it will be automatically considered as only editable by MeetingManagers as well."
+msgid "annex_restrict_shown_and_editable_attributes_descr"
 msgstr ""
 
-#. Default: "The annex is confidential.  Click on the image to set it as not confidential."
-msgid "annex_is_confidential_yes_edit"
+#. Default: "Confidential"
+msgid "annex_term_confidential"
 msgstr ""
 
-#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" could not be kept because it was not possible to find a corresponding annex type in the destination meeting configuration, please contact system administrator."
-msgid "annex_not_kept_because_no_available_annex_type_warning"
+#. Default: "Not confidential"
+msgid "annex_term_not_confidential"
 msgstr ""
 
-#. Default: "The item was duplicated but the annex with title \"${annexTitle}\" was not kept because using a scan_id, please contact system administrator."
-msgid "annex_not_kept_because_using_scan_id"
+#. Default: "Not publishable"
+msgid "annex_term_not_publishable"
 msgstr ""
 
-#. Default: "Select for each optional annexes attributes which are only displayed or editable by MeetingManagers.  If an attribute is only displayed to MeetingManagers it will be automatically considered as only editable by MeetingManagers as well."
-msgid "annex_restrict_shown_and_editable_attributes_descr"
+#. Default: "Not to print"
+msgid "annex_term_not_to_print"
+msgstr ""
+
+#. Default: "Not to sign"
+msgid "annex_term_not_to_sign"
+msgstr ""
+
+#. Default: "Publishable"
+msgid "annex_term_publishable"
+msgstr ""
+
+#. Default: "Signed"
+msgid "annex_term_signed"
+msgstr ""
+
+#. Default: "To print"
+msgid "annex_term_to_print"
+msgstr ""
+
+#. Default: "To sign"
+msgid "annex_term_to_sign"
 msgstr ""
 
 #. Default: "Title"
 msgid "annex_title"
 msgstr "Título"
 
-#. Default: "The annex is not printable because it can not be converted (unsupported format or error during conversion).  Please use common office formats."
-msgid "annex_to_print_disabled"
-msgstr "El anexo no puede ser impreso, ya que no se puede convertir (formato no admitido o error durante la conversión). Utilice los formatos ofimaticos comunes."
-
 #. Default: "Automated (annexes are printed by the application)"
 msgid "annex_to_print_mode_automated"
 msgstr ""
 
 #. Default: "If print functionnality is enabled for annexes and an annex is set \"to print\", select here the to print mode that will be used : \"Manual\", means that the to print is just defined for information and that the printing process will be handled manually or \"Automated\", in this case, the application will generate a printable format for the annex (converted to images) so it can be inserted in a generated document."
 msgid "annex_to_print_mode_descr"
 msgstr ""
 
 #. Default: "For information (annexes are printed manually)"
 msgid "annex_to_print_mode_info"
 msgstr ""
 
-#. Default: "The annex will not be printed."
-msgid "annex_to_print_no"
-msgstr "El anexo no sera impreso."
-
-#. Default: "The annex will not be printed. Click on the image to print it."
-msgid "annex_to_print_no_edit"
-msgstr "El anexo no se imprimirá. Haga clic en la imagen a imprimir."
-
-#. Default: "The annex will be printed."
-msgid "annex_to_print_yes"
-msgstr "El anexo sera impreso."
-
-#. Default: "The annex will be printed. Click on the image not to print it."
-msgid "annex_to_print_yes_edit"
-msgstr "El anexo sera impreso. Haga clic en la imagen no se imprime."
-
 #. Default: "Annex type"
 msgid "annex_type"
 msgstr "Tipo de anexo"
 
 #. Default: "Every item may be associated with a series of annexes. Some annexes may be specifically tied to the decision taken on the item. You can consult and modify here the annex types that are defined within this meeting configuration. An annex type is defined by a title, an icon (preferably of 16x16 pixels) and a predefined title. When users want to associate an annex to an item, they may choose, in a dropdown list, an annex type among those defined here and upload a file."
 msgid "annex_types_descr"
 msgstr ""
@@ -2590,24 +2457,16 @@
 msgid "annexes_preview_disabled"
 msgstr ""
 
 #. Default: "<span style='color: green;'>Annexes preview is enabled in the ${documentviewer_url}.</span>"
 msgid "annexes_preview_enabled"
 msgstr ""
 
-#. Default: "Signed annexes"
-msgid "annexes_signed_term"
-msgstr ""
-
-#. Default: "Annexes to print"
-msgid "annexes_to_print_term"
-msgstr ""
-
-#. Default: "Annexes to sign"
-msgid "annexes_to_sign_term"
+#. Default: "Annexes types are hidden by default, you can ${force_display} of it (may take some time)."
+msgid "annexes_types_force_display_descr"
 msgstr ""
 
 #. Default: "Application users"
 msgid "app_users"
 msgstr ""
 
 #. Default: "Are you sure?"
@@ -2644,18 +2503,14 @@
 msgid "assemblyMember"
 msgstr ""
 
 #. Default: "Absents as defined on the linked meeting"
 msgid "assembly_absents_defined_on_meeting"
 msgstr ""
 
-#. Default: "Define here people that were absents (not excused) for the meeting"
-msgid "assembly_absents_meeting_descr"
-msgstr ""
-
 #. Default: "Assembly and signatures"
 msgid "assembly_and_signatures"
 msgstr ""
 
 #. Default: "Assembly as defined on the linked meeting"
 msgid "assembly_defined_on_meeting"
 msgstr "Asamblea ha sido definida en la reunión vinculada"
@@ -2665,27 +2520,18 @@
 msgid "assembly_descr"
 msgstr "Defina aquí la asamblea por defecto (por ejemplo, puede escribir una lista de nombres y apellidos separados por dos puntos o líneas nuevas) que se seleccionará automáticamente en la creación de nuevas reuniones. Si desea una forma más estructurada para definir a los asistentes, ausentes y personas excusadas en una reunión, no llene este campo, crear, en la pestaña \"datos\", los usuarios especial que tienen la característica de 'miembro de la asamblea' y seleccione, en la misma pestaña, los atributos  'asistentes', 'ausentes' y / o 'excusado' como atributos que se utilizan para una reunión."
 
 #. Default: "Excused as defined on the linked meeting"
 msgid "assembly_excused_defined_on_meeting"
 msgstr ""
 
-#. Default: "Define here people that were excused for the meeting"
-msgid "assembly_excused_meeting_descr"
-msgstr ""
-
 #. Default: "Guests as defined on the linked meeting"
 msgid "assembly_guests_defined_on_meeting"
 msgstr ""
 
-#. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
-#, fuzzy
-msgid "assembly_meeting_descr"
-msgstr "Agregue los corchetes [[ ]] alrededor de las personas ausentes (como [[Señor Pedro Perez]])"
-
 #. Default: "Using attribute(s) \"itemExcused\" and/or \"itemAbsents\" requires the use of attribute \"assembly\"."
 msgid "assembly_required"
 msgstr ""
 
 #. Default: "Define here the default assembly staves (for example you may type a list of names and first names separated by colons or new lines) that will be automatically selected on newly created meetings."
 msgid "assembly_staves_descr"
 msgstr ""
@@ -2776,14 +2622,18 @@
 msgid "budgetimpacteditors"
 msgstr "Editores de impacto del presupuestario"
 
 #. Default: "You can not access this item"
 msgid "can_not_access_this_item"
 msgstr ""
 
+#. Default: "Assembly and signatures : you can not use same signature number several times."
+msgid "can_not_define_several_same_signature_number"
+msgstr ""
+
 #. Default: "You can not define two rows for the same meeting configuration!"
 msgid "can_not_define_two_rows_for_same_meeting_config"
 msgstr ""
 
 #. Default: "You can not remove/disable a function that is used by an item in the configuration.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_config_meetingitem"
 msgstr ""
@@ -2792,30 +2642,34 @@
 msgid "can_not_delete_plone_group_meetingconfig"
 msgstr ""
 
 #. Default: "You can not remove/disable a function that is used by an item in the application.  Please check ${item_url}."
 msgid "can_not_delete_plone_group_meetingitem"
 msgstr ""
 
-#. Default: "You can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect an attendee that has been redefined on items.  Please check ${attendee_title}."
 msgid "can_not_remove_attendee_redefined_on_items"
 msgstr ""
 
-#. Default: "You can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a public vote item.  Please check ${attendee_title}."
 msgid "can_not_remove_public_voter_voted_on_items"
 msgstr ""
 
-#. Default: "You can not unselect a voter that already voted on a secret vote item."
+#. Default: "Assembly and signatures : you can not unselect a voter that already voted on a secret vote item."
 msgid "can_not_remove_secret_voter_voted_on_items"
 msgstr ""
 
 #. Default: "This item can no more be returned to the meeting managers because the meeting is in a state not authorizing it (${meetingState})."
 msgid "can_not_return_to_meeting_because_of_meeting_state"
 msgstr "Este tema ya no puede ser devuelto a los administrador de reunión porque la reunión se encuentra en un estado no se autoriza (${meetingState})."
 
+#. Default: "You can not select \"No committee\" and a committee."
+msgid "can_not_select_no_committee_and_committee"
+msgstr ""
+
 #. Default: "You can not select an adviser that is already displayed on the item as an inherited advice.  If you need to ask this advice again, you need to remove the inherited advice (as a MeetingManager or a Manager) then select advice again."
 msgid "can_not_select_optional_adviser_same_group_as_inherited"
 msgstr ""
 
 #. Default: "You can not select several values for the same group.  Please select a single value for the same group among available ones."
 msgid "can_not_select_several_optional_advisers_same_group"
 msgstr "No puede seleccionar varios valores para el mismo grupo. Por favor, seleccione un valor único para el mismo grupo de entre los disponibles."
@@ -2850,18 +2704,14 @@
 msgid "categories_descr"
 msgstr "Cada tema, con este configuración de reunión, puede solamente seguir una categoría. Esas categorías son definidas aquí (por un título y una descripción). El orden como ellas aparecerán en esta carpeta es importante. En verdad, si nosotros hacemos la suposición que usted desea eso (eso depende de un parámetro que usted tal ves modificará en la sección 'Datos'), cuando un tema es agregado a una reunión, ese puede ser insertado al fin de los temas siguientes a la misma categoría, esos temas inician entonces insertando en un lugar que correspondan la posición de sus categorías en medio de la lista de categorías definidas aquí. Dicho esto, si usted le dice a PloneMeeting que quiere usar los grupos de PloneMeeting como categorías (otros parámetros de la sección 'Datos'), las categorías definidas aquí será ignoradas."
 
 #. Default: "the \"Folder contents view\""
 msgid "categories_folder_contents_view"
 msgstr ""
 
-#. Default: "force display"
-msgid "categories_force_display"
-msgstr ""
-
 #. Default: "You can ${force_display} of every categories (may take some time)."
 msgid "categories_force_display_descr"
 msgstr ""
 
 #. Default: "You may use the ${folder_contents_link} to manage elements order."
 msgid "categories_use_folder_contents"
 msgstr ""
@@ -3013,14 +2863,34 @@
 msgid "clone_to"
 msgstr "Clonar a"
 
 #. Default: "Your configuration says can not correct this closed meeting, contact your system administrator if you want to change this."
 msgid "closed_meeting_not_correctable_by_config"
 msgstr ""
 
+#. Default: "${title} (${number}&nbsp;s.)"
+msgid "committee_title_with_abbr_suppl"
+msgstr ""
+
+#. Default: "${title} (${number}&nbsp;supplement)"
+msgid "committee_title_with_suppl"
+msgstr ""
+
+#. Default: "Committees"
+msgid "committees"
+msgstr ""
+
+#. Default: "Define committees that will be useable on meetings and items (you also need to enable \"Committees\" on the meeting in the [Data] tab). This will show a \"Committees\" table on the meeting and will be also managed on the item. <br />There are 2 ways to manage committees on the item, either manually or automatically:<ul><li>Manually: just define committees, this will create a multiselection box on the item and users may select it.  It is possible to use the column \"Restrict to\" to define which proposing groups will be able to select the committee;</li><li>Automatically: use the column \"Auto from\" to define which committees to associate to the item depending on proposing group, category or classifier. A MeetingManager is nevertheless able to edit the committee on the item.</li></ul>. These 2 ways are mutually exclusive, if you select values in the \"auto_from\" columb here under, the \"Automatic\" mode will be used."
+msgid "committees_descr"
+msgstr ""
+
+#. Default: "Using a \"Committees\" field requires the use of attribute \"Committees (committees)\"."
+msgid "committees_required"
+msgstr ""
+
 #. Default: "Complete"
 msgid "completeness_complete"
 msgstr ""
 
 #. Default: "Evaluation asked again"
 msgid "completeness_evaluation_asked_again"
 msgstr ""
@@ -3107,14 +2977,18 @@
 msgid "copyGroups_mail_body"
 msgstr ""
 
 #. Default: "${meetingConfigTitle} - You have been carbon copied - ${itemTitle}"
 msgid "copyGroups_mail_subject"
 msgstr ""
 
+#. Default: "These groups will have read access to the item in following states: ${states}.\nWhen icon is green, this means that copy groups have access to the item.\nWhen the label \"[auto]\" is displayed next to the group title, it means that the group was set as copy group automatically by the application."
+msgid "copy_groups_help_msg"
+msgstr ""
+
 #. Default: " "
 msgid "copy_groups_item_descr"
 msgstr "Seleccione aquí los grupos que podrán ver este tema"
 
 #. Default: "The cloned item could not be presented to a meeting in the \"${destMeetingConfigTitle}\" configuration, no suitable meeting could be found."
 msgid "could_not_present_item_no_meeting_accepting_items"
 msgstr ""
@@ -3302,14 +3176,34 @@
 msgid "delay_of_x_days"
 msgstr "Retraso de ${delay} día(s) claro"
 
 #. Default: "Select here the days a computed delay can not ends with.  If a computed delay is ending on one of selected week day, the delay will be extend to next available day.  <span style='color: red;'>If you change this parameter, do not forget to run \"Update items and meetings\"!</span>"
 msgid "delay_unavailable_end_days_descr"
 msgstr ""
 
+#. Default: "Add [[ ]] around absent people (like [[Mister Sample Peter]]) if you do not use \"Excused\" and \"Absents\" fields"
+msgid "descr_assembly"
+msgstr ""
+
+#. Default: "<span style='color: red;'>WARNING, this field is managed by the application and it's value will be \"-1\" until the meeting is frozen, then it will be computed automatically. Do only change it manually when necessary (in general this should never happen). This field is only editable and viewable by meeting managers</span>"
+msgid "descr_config_field_reserved_to_meeting_managers"
+msgstr ""
+
+#. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
+msgid "descr_field_reserved_to_meeting_managers"
+msgstr ""
+
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
+msgid "descr_field_vieawable_by_everyone"
+msgstr ""
+
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
+msgid "descr_field_vieawable_by_everyone_once_meeting_decided"
+msgstr ""
+
 #. Default: "You are just able to see visible elements here. Please consult the \"manage\" box here opposite."
 #, fuzzy
 msgid "description_only_see_visible_items"
 msgstr "Usted es capaz de ver sólo temas visibles aquí. Por favor, consulte la caja 'administrar' aquí contrario."
 
 #. Default: "By default only MeetingManagers will see the available items panel on a meeting as long as the meeting is accepting items.  This let's you show this panel to selected profiles.  Note that if you enable this, the meeting view will be displayed slower."
 msgid "display_available_items_to_descr"
@@ -3408,14 +3302,22 @@
 msgid "enable_scan_docs_descr"
 msgstr ""
 
 #. Default: "If you check this box, users will be able to access a screen for modifying their preferences. While powerful, some may think it exposes too much complexity to users."
 msgid "enable_user_preferences_descr"
 msgstr "Si marca esta casilla, los usuarios podrán acceder a una pantalla para modificar sus preferencias. Mientras que usted piensa que esta potenciando a sus usuarios, para algunos otros pueden pensar que esta característica expone mucha complejidad para los usuarios."
 
+#. Default: "Select the batch actions that will be displayed on the table listing annexes"
+msgid "enabled_annexes_batch_actions_descr"
+msgstr ""
+
+#. Default: "The meeting end date must occur after the start date and meeting date."
+msgid "end_date_before_meeting_date"
+msgstr ""
+
 #. Default: "When advice mandatoriness is enforced, an item can't be inserted into a meeting unless all mandatory advices are given and positive."
 msgid "enforce_advice_mandatoriness_descr"
 msgstr "Cuando el consejo obligatorio es forzado, un tema no puede ser insertado dentro de una reunión a menos que todos los consejos obligatorios son dados y son positivos."
 
 #. Default: "You can not encode more than ${max_voters} voters."
 msgid "error_can_not_encode_more_than_max_voters"
 msgstr ""
@@ -3436,14 +3338,30 @@
 msgid "error_certified_signatures_invalid_dates"
 msgstr ""
 
 #. Default: "Signatures must be ordered by signature number, please check and order signature using the arrows on the right of the table."
 msgid "error_certified_signatures_order"
 msgstr ""
 
+#. Default: "You can not remove a configuration that was already used, removed configuration \"${committee_label}\" is used for example by item at ${url}.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committee_row_id_removed_already_used"
+msgstr ""
+
+#. Default: "You can not define values for the \"auto_from\" and \"using_groups\" columns, their use is multually exclusive.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_committees_mutually_exclusive_auto_from_and_using_groups"
+msgstr ""
+
+#. Default: "Default poll type must be among used poll types"
+msgid "error_default_poll_type_must_be_among_used_poll_types"
+msgstr ""
+
+#. Default: "First linked vote used votes values must be among used vote values"
+msgid "error_first_linked_vote_used_vote_values_must_be_among_used_vote_values"
+msgstr ""
+
 #. Default: "You may not remove a list type that is currently used by an item, check for example : ${url}."
 msgid "error_list_types_identifier_removed_already_used"
 msgstr ""
 
 #. Default: "You may not remove the default list types (\"normal\" and \"late\")."
 msgid "error_list_types_missing_default"
 msgstr ""
@@ -3452,14 +3370,22 @@
 msgid "error_list_types_same_identifier"
 msgstr ""
 
 #. Default: "You may only use lowercase letters for identifier."
 msgid "error_list_types_wrong_identifier_format"
 msgstr ""
 
+#. Default: "Next linked votes used vote values must be among used vote values"
+msgid "error_next_linked_votes_used_vote_values_must_be_among_used_vote_values"
+msgstr ""
+
+#. Default: "Some selected values are no more selectable (no more selected in the \"Ordered committees contacts\" field), please check value \"${hp_title}\".  You can not select \"No committee\" and a committee.  If you lost encoded values, just cancel edition and edit again correctly."
+msgid "error_value_removed_used_in_committees_field"
+msgstr ""
+
 #. Default: "An advice was added or updated on an item (notify the \"Creators\")"
 #, fuzzy
 msgid "event_add_advice"
 msgstr "Un consejo fue agregado o actualizado en un tema"
 
 #. Default: "An advice was added or updated on an item (notify the \"Owner\")"
 msgid "event_add_advice_owner"
@@ -3582,28 +3508,36 @@
 msgid "fastedit_save_changes"
 msgstr "Guardar cambios."
 
 #. Default: "Please fill this field."
 msgid "field_required"
 msgstr "Por favor, rellene este campo"
 
-#. Default: "<span style='color: red;'>This field is only editable and viewable by meeting managers</span>"
-msgid "field_reserved_to_meeting_managers_descr"
+#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once item is decided</span>"
+msgid "field_vieawable_by_everyone_once_item_decided_descr"
 msgstr ""
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone</span>"
-msgid "field_vieawable_by_everyone_descr"
+#. Default: "Assembly and signatures"
+msgid "fieldset_assembly"
 msgstr ""
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once item is decided</span>"
-msgid "field_vieawable_by_everyone_once_item_decided_descr"
+#. Default: "Committees"
+msgid "fieldset_committees"
 msgstr ""
 
-#. Default: "<span style='color: green;'>This field is only editable by meeting managers but viewable by everyone once meeting is decided</span>"
-msgid "field_vieawable_by_everyone_once_meeting_decided_descr"
+#. Default: "Dates and data"
+msgid "fieldset_dates_and_data"
+msgstr ""
+
+#. Default: "Informations"
+msgid "fieldset_informations"
+msgstr ""
+
+#. Default: "Parameters"
+msgid "fieldset_parameters"
 msgstr ""
 
 #. Default: "Please choose a file by clicking on the \"Browse\" button."
 #, fuzzy
 msgid "file_required"
 msgstr "Por favor elija un archivo haciendo clic en el botón 'Navegar'."
 
@@ -3616,21 +3550,17 @@
 msgstr ""
 
 #. Default: "In the application folder of every member, a sub-folder is created for each meeting configuration. The name of this sub-folder is defined here."
 #, fuzzy
 msgid "folder_title_descr"
 msgstr "En la carpeta PloneMeeting de cada miembro, una subcarpeta es creada para cada configuración de reunión. El nombre de esta subcarpeta es definida aquí."
 
-#. Default: "For the administrator only"
-msgid "for_admin_only"
-msgstr "Para la administración solamente"
-
-#. Default: "Specify here the deadline for validating late items to be inserted in a given meeting.  Leave the field empty not to use this functionality."
-msgid "freeze_deadline_default_descr"
-msgstr "Especifique aquí el limite para la validación de temas retardados a ser insertados en un reunión dada."
+#. Default: "force display"
+msgid "force_display"
+msgstr ""
 
 #. Default: "<p>PloneMeeting body in HTML format.</p>"
 msgid "front_page_body"
 msgstr "<p>Cuerpo de PloneMeeting en formato HTML.</p>"
 
 #. Default: "Manage here your official meetings."
 msgid "front_page_description"
@@ -3736,14 +3666,18 @@
 msgstr ""
 
 # Other
 #. Default: "Check/uncheck items"
 msgid "helpSelectItemsIcon"
 msgstr "Marcar / Desmarcar temas"
 
+#. Default: "This is the date the advice was originally given, this will change when the advice will be considered \"Given\" in a state where it is no more editable"
+msgid "help_given_on_before_started_on"
+msgstr ""
+
 #. Default: "No preview available because this type of file can not be converted.  Please use common office formats.  You can download the file, look in the \"actions\" column."
 msgid "help_no_preview_available"
 msgstr ""
 
 #. Default: "No preview available because there was an error during conversion to a previewable format.  Please contact system administrator that will have access to more debugging informations."
 msgid "help_no_preview_available_conversion_error"
 msgstr ""
@@ -3785,19 +3719,14 @@
 msgstr ""
 
 #. Default: "For every field you select here, the application will keep track of any change on any item, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
 #, fuzzy
 msgid "historized_item_attrs_descr"
 msgstr "Por cada campo que seleccione aquí, PloneMeeting realizará un seguimiento de cualquier cambio en cualquier elemento, si encuentra en uno de los estados trazables, según se define a continuación."
 
-#. Default: "For every field you select here, the application will keep track of any change on any meeting, if it is in one of the \"historizable\" states as defined below.  <span style='color: red;'>This functionnality is still in beta status, you may use it but encounter some weirdness, this will be entirely reworked in a forthcoming version.</span>"
-#, fuzzy
-msgid "historized_meeting_attrs_descr"
-msgstr "Por cada campo que seleccione aquí, PloneMeeting realizará un seguimiento de cualquier cambio en cualquier reunión, si encuentra en uno de los estados trazables, según se define a continuación."
-
 #. Default: "See changes"
 msgid "history_changes"
 msgstr "Ver cambios"
 
 #. Default: "Deleted by ${userName}"
 msgid "history_delete"
 msgstr "Eliminado por ${userName}"
@@ -3814,15 +3743,15 @@
 msgid "holidays_date_not_ascending_error"
 msgstr ""
 
 #. Default: "These dates will be used to compute advices delays.  <span style='color: red;'>If you change this parameter and modified dates are interacting with some existing advice delays, do not forget to run \"Update items and meetings\"!</span>"
 msgid "holidays_descr"
 msgstr ""
 
-#. Default: "You removed a date that is currently in use!"
+#. Default: "You removed a date that is currently in use! Check item at ${item_url}"
 msgid "holidays_removed_date_in_use_error"
 msgstr ""
 
 #. Default: "There are not enough holidays defined in the configuration.  These days are used for advice delay computation.  This warning appear when last holiday defined in the configuration is in less than 60 days. Contact you system administrator if necessary."
 msgid "holidays_warning_message"
 msgstr ""
 
@@ -3843,14 +3772,18 @@
 msgstr "Nombre"
 
 #. Default: "This application allows you to manage your official meetings."
 #, fuzzy
 msgid "hs_welcome_body"
 msgstr "Este sitio le permite administrar sus reuniones oficiales."
 
+#. Default: "iA.Delib documentation"
+msgid "iA.Delib documentation"
+msgstr ""
+
 #. Default: "Azur"
 msgid "icon_color_azur"
 msgstr ""
 
 #. Default: "Black"
 msgid "icon_color_black"
 msgstr ""
@@ -4479,38 +4412,26 @@
 
 # Mails (item-related)
 #. Default: "${meetingConfigTitle} - A \"late\" item has been validated."
 #, fuzzy
 msgid "lateItem_mail_subject"
 msgstr "${meetingConfigTitle} - Un tema 'tardío' ha sido validado."
 
-#. Default: "Items presented tardily"
-msgid "late_presented_items"
-msgstr "Temas presentados después de la reunión que fue publicada."
-
 #. Default: "--- Do nothing, let the item in the workflow initial state ---"
 msgid "let_item_in_initial_state"
 msgstr ""
 
 #. Default: "Linked items (${auto_linked_items})"
 msgid "linked_items"
 msgstr ""
 
 #. Default: "Linked items, ${auto_linked_items} automatically and ${manually_linked_items} manually"
 msgid "linked_items_with_manually_linked_items"
 msgstr ""
 
-#. Default: "Late"
-msgid "list_type_late"
-msgstr ""
-
-#. Default: "Normal"
-msgid "list_type_normal"
-msgstr ""
-
 #. Default: "Types of list of items that will be available when an item is linked to a meeting."
 msgid "list_types_descr"
 msgstr ""
 
 #. Default: "Size"
 msgid "listingheader_size"
 msgstr "Tamaño"
@@ -4609,36 +4530,16 @@
 msgid "meeting_annex_confidential_visible_for_descr"
 msgstr ""
 
 #. Default: "Choose here which page will be shown after logon."
 msgid "meeting_app_default_view_descr"
 msgstr "Selecciona aquí con qué página se mostrará después del inicio de sesión."
 
-#. Default: "Assembly"
-msgid "meeting_assembly"
-msgstr "Asamblea"
-
-#. Default: "Absents"
-msgid "meeting_assemblyAbsents"
-msgstr ""
-
-#. Default: "Excused"
-msgid "meeting_assemblyExcused"
-msgstr ""
-
-#. Default: "Guests"
-msgid "meeting_assemblyGuests"
-msgstr ""
-
-#. Default: "Proxies"
-msgid "meeting_assemblyProxies"
-msgstr ""
-
-#. Default: "Staves"
-msgid "meeting_assemblyStaves"
+#. Default: "Meeting assembly (${number_of_attendees}) and signatories (${number_of_signatories})"
+msgid "meeting_attendees_and_signatories"
 msgstr ""
 
 #. Default: "Choose here which columns to display when listing meetings (ie, when displaying the list of available meetings or decisions, or when performing custom searches)."
 msgid "meeting_columns_descr"
 msgstr "Seleccione aquí cuales columnas se mostrarán en la lista de reuniones (es decir, cuando muestra la lista de reuniones disponibles o decisiones, o cuando ejecutaba búsqueda personalizadas)."
 
 #. Default: "Similarly to interfaces defined for items, the conditions expressed on the transitions of the meeting workflow may be configured through the development of another Plone product into which you must:<ul><li>create a Python interface that inherits from interface Products.PloneMeeting.interfaces.IMeetingWorkflowConditions (you must enter the full package name of this interface in the field below);</li><li>create and declare in ZCML an adapter that adapts the interface  Products.PloneMeeting.interfaces.IMeeting to the interface you have defined in the previous step.</li></ul>Your adapter may inherit from the default adapter Products.PloneMeeting.Meeting.MeetingWorkflowConditions: it will allow you to override only methods for which you want an altered behaviour. All the methods proposed by the interface Products.PloneMeeting.interfaces.IMeetingWorkflowConditions are documented."
@@ -4684,22 +4585,14 @@
 msgid "meeting_organizations"
 msgstr ""
 
 #. Default: "When an item is inserted in a meeting from everywhere (so not when on a meeting view), this will take the very next meeting still accepting items.  Define here states to take into account to get this very next meeting."
 msgid "meeting_present_item_when_no_current_meeting_states_descr"
 msgstr ""
 
-#. Default: "Signatories"
-msgid "meeting_signatories"
-msgstr "Firmantes"
-
-#. Default: "Signatures"
-msgid "meeting_signatures"
-msgstr "Firmas"
-
 #. Default: "You can consult this meeting at ${objectUrl}."
 msgid "meeting_state_changed_default_mail_body"
 msgstr "Usted puede consultar esta reunión en ${objectUrl}."
 
 # Mails (meeting-related)
 # Default translation for mails sent upon meeting transition
 # This default is used if no accurate translation can be found. We will try for example to translate
@@ -4792,26 +4685,18 @@
 msgid "metadata"
 msgstr "Metadata"
 
 #. Default: "Select here some standard adaptations that can be applied to data structures."
 msgid "model_adaptations_descr"
 msgstr "Seleccione aquí algunas adaptaciones estándar que puede ser aplicada a la estructuras de los datos."
 
-#. Default: "Move the item down"
-msgid "move_item_down"
-msgstr "Mover el tema abajo"
-
-#. Default: "Move item to given position"
+#. Default: "Save item number (you may also use the [Enter] key)"
 msgid "move_item_to_given_position"
 msgstr ""
 
-#. Default: "Move the item up"
-msgid "move_item_up"
-msgstr "Mover el tema arriba"
-
 #. Default: "Moves this item to the position that precedes the number you have introduced besides. If you want to move the item at the end of the list, specify the number of the last item plus one."
 msgid "move_several"
 msgstr "Mover este tema a la posición que precede al número que ha introducido. Además, si usted desea mover este tema al final de la lista, especifique le número del último temas mas uno (por ejemplo 3 + 1  = 4)."
 
 #. Default: "Negative"
 msgid "negative"
 msgstr "Negativo"
@@ -4828,35 +4713,43 @@
 msgid "nil"
 msgstr "Nulo"
 
 #. Default: "No annex is currently defined for this element."
 msgid "no_annexes"
 msgstr "Actualmente sin anexos definidos para este tema."
 
-#. Default: "No annexes to print"
-msgid "no_annexes_to_print_term"
-msgstr ""
-
-#. Default: "Annexes not to sign"
-msgid "no_annexes_to_sign_term"
-msgstr ""
-
 #. Default: "Attributes \"assembly\" and \"attendees\" can't be used together."
 #, fuzzy
 msgid "no_assembly_and_attendees"
 msgstr "Los atributos 'asamblea' y 'asistentes' no puede ser usado juntos."
 
 #. Default: "No category is currently defined."
 msgid "no_category"
 msgstr "Actualmente sin categorías definida."
 
 #. Default: "No classifier is currently defined."
 msgid "no_classifier"
 msgstr ""
 
+#. Default: "NC"
+msgid "no_committee_term_title_acronym"
+msgstr ""
+
+#. Default: "No committee"
+msgid "no_committee_term_title_label"
+msgstr ""
+
+#. Default: "Attributes \"committees_assembly\" and \"committees_attendees\" can't be used together."
+msgid "no_committees_assembly_and_committees_attendees"
+msgstr ""
+
+#. Default: "Attributes \"committees_sigantures\" and \"committees_signatories\" can't be used together."
+msgid "no_committees_signatures_and_committees_signatories"
+msgstr ""
+
 #. Default: "None"
 msgid "no_config_group"
 msgstr ""
 
 #. Default: "No emergency"
 msgid "no_emergency"
 msgstr ""
@@ -4881,31 +4774,28 @@
 msgid "no_meeting_file_type"
 msgstr "Actualmente sin tipo de anexo definido."
 
 #. Default: "No special user is currently defined."
 msgid "no_meeting_user"
 msgstr "Sin usuario especial aun definido."
 
-#. Default: "No items."
-msgid "no_meetingitems"
-msgstr "Sin temas."
-
 #. Default: "No POD template is currently defined."
 msgid "no_pod_folder"
 msgstr "Actualmente sin plantilla POD definido."
 
 #. Default: "Attributes \"proposingGroupWithGroupInCharge\" and \"groupsInCharge\" can't be used together."
 msgid "no_proposingGroupWithGroupInCharge_and_groupsInCharge"
 msgstr ""
 
 #. Default: "No recurring item is currently defined."
 msgid "no_recurring_item"
 msgstr "Actualmente sin tema recurrente definido."
 
-#. Default: "No visible item for now."
+#. Default: "You do not have access to these items."
+#, fuzzy
 msgid "no_shown_items"
 msgstr "Sin tema visible por ahora."
 
 #. Default: "Attributes \"signatures\" and \"signatories\" can't be used together."
 #, fuzzy
 msgid "no_signatories_and_signatures"
 msgstr "Los atributos 'firmas' y 'firmantes' no puede ser usado juntos."
@@ -4934,14 +4824,22 @@
 msgid "normal"
 msgstr ""
 
 #. Default: "You are a registered user but your account has not been activated yet. Please contact the system administrator."
 msgid "notPloneMeetingUser"
 msgstr "Usted es un usuario registrado pero su cuenta no ha sido activada aun. Por favor, contacte al administrador de sistema."
 
+#. Default: "Not able to find a meeting to present this item into.  Only meetings in the future are taken into account, check configuration if necessary"
+msgid "not_able_to_find_meeting_to_present_item_into"
+msgstr ""
+
+#. Default: "Not confidential annexes"
+msgid "not_confidential_annexes"
+msgstr ""
+
 #. Default: "Not given yet"
 msgid "not_given"
 msgstr "Sin dar un consejo aun"
 
 #. Default: "Not to be cloned to anywhere"
 msgid "not_to_be_cloned_to_term"
 msgstr ""
@@ -4958,14 +4856,22 @@
 msgid "nothing_to_do"
 msgstr "Nada por hacer"
 
 #. Default: "notify users able to view the element"
 msgid "notify_users_able_to_view_element"
 msgstr ""
 
+#. Default: "${number}st"
+msgid "num_part_st"
+msgstr ""
+
+#. Default: "${number}th"
+msgid "num_part_th"
+msgstr ""
+
 #. Default: "Total number of voters"
 msgid "number_of_voters"
 msgstr ""
 
 #. Default: "Observer"
 msgid "observer"
 msgstr "Observador"
@@ -4974,14 +4880,18 @@
 msgid "observers"
 msgstr "Observadores"
 
 #. Default: "Follow all associated groups order"
 msgid "on_all_associated_groups"
 msgstr ""
 
+#. Default: "Follow all committees order"
+msgid "on_all_committees"
+msgstr ""
+
 #. Default: "Follow all groups order"
 msgid "on_all_groups"
 msgstr "Seguir orden de todos los grupos"
 
 #. Default: "Follow categories order"
 msgid "on_categories"
 msgstr "Seguir orden de categorías"
@@ -5063,14 +4973,18 @@
 msgid "oral_question_item_descr"
 msgstr ""
 
 #. Default: "If this field is left empty, selectable associated organizations are every organizations selected in the plonegroup configuration panel.  Here you may select associated organizations in a particular order including organizations that are not selected in the plonegroup configuration panel.  This is only relevant if the 'Associated groups' field is enabled on items."
 msgid "ordered_associated_organizations_descr"
 msgstr ""
 
+#. Default: "Select here attendees that will be selectable in the \"Attendees\" column of defined committees here under.  <span style='color: red;'>If you select/unselect values, you need to save first then edit again for these values to appear/disappear if field \"Committees\" here under.</span>"
+msgid "ordered_committee_contacts_descr"
+msgstr ""
+
 #. Default: "Select here contacts that will be usable to manage meeting attendees.  The contacts order defined here will be the default order when creating a new meeting."
 msgid "ordered_contacts_descr"
 msgstr ""
 
 #. Default: "If this field is left empty, selectable groups in charge are every organizations selected in the plonegroup configuration panel.  Here you may select groups in charge in a particular order.  This is only relevant if the 'Groups in charge' field is enabled on items."
 msgid "ordered_groups_in_charge_descr"
 msgstr ""
@@ -5104,23 +5018,27 @@
 msgstr ""
 
 #. Default: "Mark this person absent for this item"
 #, fuzzy
 msgid "person_byebye"
 msgstr "Dar la bienvenida después de este tema"
 
+#. Default: "Redefine position for attendee for this item"
+msgid "person_redefine_attendee_position"
+msgstr ""
+
+#. Default: "Remove redefined position for attendee for this item"
+msgid "person_remove_redefined_attendee_position"
+msgstr ""
+
 #. Default: "Remove this person from absents for this item"
 #, fuzzy
 msgid "person_welcome"
 msgstr "Bienvenido a este tema"
 
-#. Default: "Please encode this other place."
-msgid "place_other_required"
-msgstr "Por favor, escriba este otro lugar."
-
 #. Default: "Enter here some default places where meetings occur. There must be one place per line. The first one will be the default one."
 msgid "places_descr"
 msgstr "Ingrese aquí algunos lugares por defecto donde ocurren las reuniones. Allí debe haber un lugar por linea. El primero será el lugar por defecto."
 
 #. Default: "You are about to delete this meeting and all included items. Are you sure?"
 msgid "plonemeeting_delete_meeting_confirm_message"
 msgstr "Usted está a punto de eliminar esta reunión y todos los temas incluidos. ¿Estás seguro?"
@@ -5317,22 +5235,14 @@
 msgid "powerobservers"
 msgstr "Observadores potenciales"
 
 #. Default: "The preparatory meeting must occur before the meeting."
 msgid "pre_date_after_meeting_date"
 msgstr "La reunión preparatoria debe ocurrir antes de la reunión."
 
-#. Default: "Preparatory meeting"
-msgid "pre_meeting"
-msgstr "Reunión preparatoria"
-
-#. Default: "Specify here the date of the pre-meeting, relative to its meeting, in the same format as fields above.  Leave the field empty not to use this functionality."
-msgid "pre_meeting_date_default_descr"
-msgstr "Especifique aquí la fecha de la reunión preparatoria, relativa a esta reunión, en el mismo formato como en los campos de arriba."
-
 #. Default: "If this is a normal item and you want it to be inserted in any availale meeting, just select \"No preference\" value.  Selecting a date is for 2 usecases : this will make the item not presentable to the meetings before selected one, or if the selected meeting is \"frozen\", this will make current item considered as \"late\" item presentable in the selected frozen meeting.  Indeed, the only way to insert an item in a frozen meeting is to select this meeting as preferred meeting."
 msgid "preferred_meeting_descr"
 msgstr ""
 
 #. Default: "Pre-validator"
 msgid "prereviewer"
 msgstr "Pre-validador"
@@ -5377,35 +5287,34 @@
 msgid "public"
 msgstr ""
 
 #. Default: "Public meeting (heading)"
 msgid "public_heading"
 msgstr ""
 
-#. Default: "Specify here the deadline for validating items to be inserted in a given meeting. You need to express this deadline relative to the meeting date. For example, \"5.9:30\" (do not type quotes) means: \"5 days before the meeting date, at 9:30.\".  Leave the field empty not to use this functionality."
-#, fuzzy
-msgid "publish_deadline_default_descr"
-msgstr "Especifique aquí la fecha límite para la validación de los temas que se insertan en una reunión dada. Usted tiene la necesidad de expresar este plazo en relación con la fecha de la reunión. Por ejemplo, '5 .9:30' (no escriba las comillas) eso significa: '5 días antes de la fecha de la reunión, a las 9:30'."
-
 #. Default: "Publishable (displayed)"
 msgid "publishable_display"
 msgstr ""
 
 #. Default: "Publishable (editable)"
 msgid "publishable_edit"
 msgstr ""
 
+#. Default: "Read less"
+msgid "read_less"
+msgstr ""
+
+#. Default: "Read more"
+msgid "read_more"
+msgstr ""
+
 #. Default: "Select here the item states into which some events related to the item (like annex creations or deletions) will be stored in the item's history."
 msgid "record_item_history_states_descr"
 msgstr "Seleccione aquí los estados del tema en los cuales algunos eventos relacionados al tema (como creaciones o eliminaciones de anexo) será almacenada en el histórico del tema."
 
-#. Default: "Select here the meeting states into which some events related to the meeting will be stored in the meeting's history."
-msgid "record_meeting_history_states_descr"
-msgstr "Seleccione aquí los estados de la reunión en los cuales algunos eventos relacionados a la reunión será almacenada en el histórico de la reunión."
-
 #. Default: "The recurring item specified in the subject of this email could not be inserted in a meeting. Maybe does it lack some important information (a text for the decision, for example) while the meeting is in an \"advanced\" state (it is already \"decided\", for instance). More information can be found in the log file of your Zope instance."
 #, fuzzy
 msgid "recurringItemWorkflowError_mail_body"
 msgstr "El tema recurrente especificado en sujeto de este mensaje de correo electrónico no puede insertarse en una reunión. Tal vez lo hace falta alguna información importante (un texto de la decisión, por ejemplo), mientras que en la reunión este en un estado 'avanzado' (que ya está \"decidido\", por ejemplo). Más información puede ser encontrada en archivo de registro de su instancia Zope."
 
 #. Default: "${portalTitle} - A problem occurred while inserting a recurring into a meeting - ${itemTitle}"
 #, fuzzy
@@ -5452,26 +5361,34 @@
 msgid "remove_several_items"
 msgstr ""
 
 #. Default: "Selected items have been removed from the meeting."
 msgid "remove_several_items_done"
 msgstr ""
 
-#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by \"${hp_url}\"!"
+#. Default: "You can not remove a position type that is in use, you removed \"${removed_position_type}\" used by held position at \"${hp_url}\"!"
 msgid "removed_position_type_in_use_error"
 msgstr ""
 
+#. Default: "You can not remove a position type that was used as redefined position for an attendee on an item, you removed \"${removed_position_type}\", check attendees on item at \"${item_url}\"!"
+msgid "removed_redefined_position_type_in_use_error"
+msgstr ""
+
 #. Default: "A category must be selected on this item so it may evolve in the workflow"
 msgid "required_category_ko"
 msgstr ""
 
 #. Default: "A classifier must be selected on this item so it may evolve in the workflow"
 msgid "required_classifier_ko"
 msgstr ""
 
+#. Default: "A group in charge must be selected on this item so it may evolve in the workflow"
+msgid "required_groupsInCharge_ko"
+msgstr ""
+
 #. Default: "Check the box if access to secret items must be restricted.  This will let only users for which an explicit access to the item has been given, access the item.  It will be the case so for members of the proposing groups, power users (Managers, MeetingManagers, power observers), copy groups and advisers.  Only activate this if necessary, it could be the case if you have a state where everything is accessible by everyone (like a \"published\" state for items) but where you want \"secret\" items not to be accessible by everyone."
 msgid "restrict_access_to_secret_items_descr"
 msgstr ""
 
 #. Default: "Restrict access to secret items to description"
 msgid "restrict_access_to_secret_items_to_descr"
 msgstr ""
@@ -5659,14 +5576,18 @@
 msgid "selectable_for_plonegroup_descr"
 msgstr ""
 
 #. Default: "Select here privacies that will be selectable by users editing items of this configuration.  If \"on privacy\" is used in the \"Sort order(s) to apply when adding an item to a meeting\" field, it is the order of values selected here that will be used."
 msgid "selectable_privacies_descr"
 msgstr ""
 
+#. Default: "Select here position types that will be selectable when redefining the position of an attendee for an item.  If nothing selected (default), then any position types is selectable."
+msgid "selectable_redefined_position_types_descr"
+msgstr ""
+
 #. Default: "Check the box if item needs to be send to authority, if so, a line will be automatically printed in the item deliberation document."
 msgid "send_to_authority_descr"
 msgstr ""
 
 #. Default: "Unable to send this item to the ${meetingConfigTitle} meetingConfig because the user to create the item to does not have a personal folder in this meetingConfig.  If necessary, the concerned user can connect for this folder to be created automatically."
 msgid "sendto_inexistent_destfolder_error"
 msgstr "No se puede enviar este tema a la configuración de reunión ${meetingConfigTitle} debido a que el usuario pueda crear el tema por que no tiene una carpeta personal en esta configuración de reunión. Si es necesario, el usuario en cuestión puede conectarse a esta carpeta que se creará automáticamente."
@@ -5714,18 +5635,14 @@
 msgid "show_or_hide_details"
 msgstr "Mostrar / ocultar detalles"
 
 #. Default: "Show / hide poll type observations"
 msgid "show_or_hide_pollTypeObservations"
 msgstr ""
 
-#. Default: "Signatures"
-msgid "signatures"
-msgstr "Firmas"
-
 #. Default: "Signatures as defined on the linked meeting"
 msgid "signatures_defined_on_meeting"
 msgstr "Firmas como se definen en la reunión vinculada"
 
 #. Default: "Define here the default signatures that will be automatically selected on newly created meetings. Use 2 lines by signature, one for the function and one for the signatory name. This will be applicable only if you use attribute \"Signatures\" for meetings."
 #, fuzzy
 msgid "signatures_descr"
@@ -5739,14 +5656,22 @@
 msgid "signed_edit"
 msgstr ""
 
 #. Default: "Check this box if you want to sort the tags in alphabetic order."
 msgid "sort_all_item_tags_descr"
 msgstr "Verifique esta casilla si usted quiere ordenar las etiquetas en orden alfabético."
 
+#. Default: "The meeting start date must occur before the end date."
+msgid "start_date_after_end_date"
+msgstr ""
+
+#. Default: "The meeting start date must occur after the meeting date."
+msgid "start_date_before_meeting_date"
+msgstr ""
+
 #. Default: "Store as annex of type ${annex_type_title}"
 msgid "store_as_annex_type_title"
 msgstr ""
 
 #. Default: "Not allowed to add annex in this element."
 msgid "store_podtemplate_as_annex_can_not_add_annex"
 msgstr ""
@@ -5840,21 +5765,217 @@
 msgstr "Este tema es una pregunta oral"
 
 #. Default: "This item is NOT an oral question"
 msgid "this_item_is_not_an_oral_question"
 msgstr "Este tema NO es una pregunta oral"
 
 #. Default: "Extraordinary session"
-msgid "this_meeting_is_extraodrinary_session"
+msgid "this_meeting_is_extraordinary_session"
+msgstr ""
+
+#. Default: "Absents"
+msgid "title_absents"
+msgstr ""
+
+#. Default: "Approval date"
+msgid "title_approval_date"
+msgstr ""
+
+#. Default: "Assembly"
+msgid "title_assembly"
+msgstr ""
+
+#. Default: "Assembly absents"
+msgid "title_assembly_absents"
+msgstr ""
+
+#. Default: "Assembly excused"
+msgid "title_assembly_excused"
+msgstr ""
+
+#. Default: "Assembly guests"
+msgid "title_assembly_guests"
+msgstr ""
+
+#. Default: "Assembly observations"
+msgid "title_assembly_observations"
+msgstr ""
+
+#. Default: "Assembly proxies"
+msgid "title_assembly_proxies"
+msgstr ""
+
+#. Default: "Assembly staves"
+msgid "title_assembly_staves"
+msgstr ""
+
+#. Default: "Attendees"
+msgid "title_attendees"
+msgstr ""
+
+#. Default: "Authority notice"
+msgid "title_authority_notice"
+msgstr ""
+
+#. Default: "Committees"
+msgid "title_committees"
+msgstr ""
+
+#. Default: "Assembly"
+msgid "title_committees_assembly"
+msgstr ""
+
+#. Default: "Attendees"
+msgid "title_committees_attendees"
+msgstr ""
+
+#. Default: "Convocation date"
+msgid "title_committees_convocation_date"
+msgstr ""
+
+#. Default: "Date"
+msgid "title_committees_date"
+msgstr ""
+
+#. Default: "Committees observations"
+msgid "title_committees_observations"
+msgstr ""
+
+#. Default: "Place"
+msgid "title_committees_place"
+msgstr ""
+
+#. Default: "Committee"
+msgid "title_committees_row_id"
+msgstr ""
+
+#. Default: "Signatories"
+msgid "title_committees_signatories"
+msgstr ""
+
+#. Default: "Signatures"
+msgid "title_committees_signatures"
+msgstr ""
+
+#. Default: "Convocation date"
+msgid "title_convocation_date"
+msgstr ""
+
+#. Default: "Date"
+msgid "title_date"
+msgstr ""
+
+#. Default: "Default assembly"
+msgid "title_default_assembly"
+msgstr ""
+
+#. Default: "Default assembly staves"
+msgid "title_default_assembly_staves"
+msgstr ""
+
+#. Default: "Default signatures"
+msgid "title_default_signatures"
+msgstr ""
+
+#. Default: "End date"
+msgid "title_end_date"
+msgstr ""
+
+#. Default: "Excused"
+msgid "title_excused"
+msgstr ""
+
+#. Default: "Extraordinary session"
+msgid "title_extraordinary_session"
+msgstr ""
+
+#. Default: "First item number (managed automatically when meeting is frozen)"
+msgid "title_first_item_number"
+msgstr ""
+
+#. Default: "In and out moves"
+msgid "title_in_and_out_moves"
+msgstr ""
+
+#. Default: "Meeting number"
+msgid "title_meeting_number"
+msgstr ""
+
+#. Default: "Meeting managers notes"
+msgid "title_meetingmanagers_notes"
+msgstr ""
+
+#. Default: "Mid date"
+msgid "title_mid_date"
+msgstr ""
+
+#. Default: "Non attendees"
+msgid "title_non_attendees"
+msgstr ""
+
+#. Default: "Notes"
+msgid "title_notes"
+msgstr ""
+
+#. Default: "Observations"
+msgid "title_observations"
+msgstr ""
+
+#. Default: "Place"
+msgid "title_place"
+msgstr ""
+
+#. Default: "Other place"
+msgid "title_place_other"
+msgstr ""
+
+#. Default: "Pre meeting date"
+msgid "title_pre_meeting_date"
+msgstr ""
+
+#. Default: "Pre meeting place"
+msgid "title_pre_meeting_place"
+msgstr ""
+
+#. Default: "Pre observations"
+msgid "title_pre_observations"
+msgstr ""
+
+#. Default: "Public meeting observations"
+msgid "title_public_meeting_observations"
+msgstr ""
+
+#. Default: "Replacements"
+msgid "title_replacements"
 msgstr ""
 
 #. Default: "A title is required."
 msgid "title_required"
 msgstr "Un título es requerido"
 
+#. Default: "Secret meeting observations"
+msgid "title_secret_meeting_observations"
+msgstr ""
+
+#. Default: "Signatories"
+msgid "title_signatories"
+msgstr ""
+
+#. Default: "Signatures"
+msgid "title_signatures"
+msgstr ""
+
+#. Default: "Start date"
+msgid "title_start_date"
+msgstr ""
+
+#. Default: "Votes observations"
+msgid "title_votes_observations"
+msgstr ""
+
 #. Default: "Ask this advice again (current advice will be historized)"
 msgid "to_advice_asked_again"
 msgstr ""
 
 #. Default: "To be printed (displayed)"
 msgid "to_be_printed_display"
 msgstr ""
@@ -6046,18 +6167,14 @@
 msgid "used_poll_types_descr"
 msgstr ""
 
 #. Default: "Specify here what vote values are in use in this meeting configuration."
 msgid "used_vote_values_descr"
 msgstr "Especifique aquí que valores de la votación están en uso en esta configuración de reunión."
 
-#. Default: "Users"
-msgid "users"
-msgstr "Usuarios"
-
 #. Default: "If you do not select anything, every users will be displayed."
 msgid "users_hidden_in_dashboard_filter_descr"
 msgstr ""
 
 #. Default: "When an advice is \"given\" and no more editable by the advisers, so when it was set in a state where advisers may not edit it anymore, it is automatically versioned. Depending on the configuration, if advice may be given when the item is still editable by the proposing group, it may be necessary to versionate advice if it was given (but still editable by advisers) and the item was edited. For example, advices are giveable when item is \"itemcreated\", a state where item may still be edited by the proposing group. If it is the case, check this box, it will ensure that the advice is versioned when the item is edited if necessary (so if it was not already versioned since last advice edition).  If you have a specific state \"waiting advice\" where proposing group is not able to edit the item, this box may be left unchecked."
 msgid "versionate_advice_if_given_and_item_modified_descr"
 msgstr ""
@@ -6164,14 +6281,15 @@
 msgstr ""
 
 #. Default: "There are ${numberOfVoters} voters for this item."
 msgid "voter_count"
 msgstr "Aquí son ${numberOfVoters} los votantes para este tema."
 
 #. Default: "Votes"
+#, fuzzy
 msgid "votes"
 msgstr "Votos"
 
 #. Default: "You can choose here who will effectively encode the votes. Several choices are possible."
 msgid "votes_encoder_descr"
 msgstr "Usted puede elegir aquí quien efectivamente escribe los votos. Varias opciones son posibles."
 
@@ -6375,14 +6493,22 @@
 msgid "wait_msg"
 msgstr ""
 
 #. Default: "You are currently adding an organization outside \"My organization\", please make sure this is correct.  If you want to create a new group that will be able the create items, give advices, you need to add it directly under \"My organization\"."
 msgid "warning_adding_org_outside_own_org"
 msgstr ""
 
+#. Default: "Advice is currently \"Asked again\" do not forget to change value of field \"Advice type\" to another value than \"Asked again\""
+msgid "warning_advice_asked_again_need_to_change_advice_type"
+msgstr ""
+
+#. Default: "Warning, there is a problem with encoded data for assembly and signatures, please check especially that signatories are correctly defined"
+msgid "warning_assembly_and_signatures"
+msgstr ""
+
 #. Default: "Warning: if you modify the title or description and save this form, all given advices will be invalidated."
 msgid "warning_invalidate_advices"
 msgstr "Advertencia: si modifica el título o descripción y guardar este formulario, todos los consejos dados serán invalidados."
 
 #. Default: "If you modify this field, all given advices will be invalidated."
 msgid "warning_invalidate_advices_fastedit"
 msgstr "Si modifica este campo, todos los consejos dados serán invalidados."
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/collective.contact.core.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/collective.contact.core.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.history.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/plone.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/plone.po`

 * *Files 0% similar despite different names*

```diff
@@ -550,14 +550,18 @@
 msgid "close"
 msgstr "Cerrar"
 
 #. Default: "Closed"
 msgid "closed"
 msgstr "Cerrado"
 
+#. Default: "Committees"
+msgid "committees"
+msgstr ""
+
 #. Default: "Confirm"
 msgid "confirm"
 msgstr "Confirmar"
 
 #. Default: "Confirmed"
 msgid "confirmed"
 msgstr "Confirmado"
@@ -987,14 +991,15 @@
 msgstr "Validar"
 
 #. Default: "Validated"
 msgid "validated"
 msgstr "Validado"
 
 #. Default: "Votes"
+#, fuzzy
 msgid "votes"
 msgstr "Votos"
 
 #. Default: "Ask advices"
 msgid "wait_advices_from"
 msgstr ""
```

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.actionspanel.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/es/LC_MESSAGES/imio.annex.po` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/nl/LC_MESSAGES/imio.annex.po`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/src/imio/pm/locales/locales/sync_pos.sh` & `imio.pm.locales-4.2b9/src/imio/pm/locales/locales/sync_pos.sh`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/ez_setup.py` & `imio.pm.locales-4.2b9/ez_setup.py`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/base.cfg` & `imio.pm.locales-4.2b9/base.cfg`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/setup.py` & `imio.pm.locales-4.2b9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup, find_packages
 import os
 
-version = '4.2b8'
+version = '4.2b9'
 
 setup(name='imio.pm.locales',
       version=version,
       description="Locales for PloneMeeting",
       long_description=open("README.rst", encoding='utf-8').read() + "\n" + open("CHANGES.rst", encoding='utf-8').read(),
       # Get more strings from
       # http://pypi.python.org/pypi?:action=list_classifiers
```

### Comparing `imio.pm.locales-4.2b8/bootstrap.py` & `imio.pm.locales-4.2b9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `imio.pm.locales-4.2b8/CHANGES.rst` & `imio.pm.locales-4.2b9/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,80 @@
 Changelog
 =========
 
 
+4.2b9 (2021-07-16)
+------------------
+
+- Added translations for `Not completed votes` and `Completed votes`.
+  [gbastien]
+- Removed single quotes for `meeting_state_changed_default_mail_body`.
+  [aduchene]
+- Added translations now that `Preferred meeting date` column is abbreviated.
+  [gbastien]
+- Renamed msgid `You cannot delete the default item template, but you can deactivate it if necessary!` to
+  `You cannot delete or move the default item template, but you can deactivate it if necessary!`.
+  [gbastien]
+- Added translations for `copy_groups_help_msg`.
+  [gbastien]
+- Adapted translations now that Meeting was moved from AT to DX.
+  [gbastien]
+- Added translations regarding the `Committees` management.
+  [gbastien]
+- Changed default translation for `move_item_to_given_position`.
+  [gbastien]
+- Added translations for annexes faceted filter vocabulary.
+  [gbastien]
+- Added translation for `required_groupsInCharge_ko`.
+  [gbastien]
+- Include `item_url` in `holidays_removed_date_in_use_error` translation.
+  [gbastien]
+- Added translation related to advice behavior that changed (delay no more reinitialized for a given advice).
+  [gbastien]
+- Removed msgids beginning with `list_type_` in the `PloneMeeting` domain, seem no more used.
+  [gbastien]
+- Added translations related to `Redefine attendee position on item`.
+  [gbastien]
+- Changed translation for `no_shown_items` from `No visible item for now.`
+  to `You do not have access to these items.`.
+  [gbastien]
+- Added translation for warning displayed on the meeting view when `assembly/signatures` are not correct.
+  [gbastien]
+- More accurate translation for `Meeting.meeting_number` and `Meeting.first_item_number`
+  description, explaining it is managed by the application.
+  [gbastien]
+- Added translations for new static columns selectable in `MeetingConfig.meetingColumns`.
+  [gbastien]
+- Added translations for `not_confidential_annexes`.
+  [gbastien]
+- Added translations for `Read more/Read less`, removed useless translation
+  `This is an extract of the comment, access full comment if necessary...`.
+  [gbastien]
+- Added translation for `marginal_notes_column`.
+  [gbastien]
+- Added translation for `not_able_to_find_meeting_to_present_item_into`.
+  [gbastien]
+- Added translations for `error_default_poll_type_must_be_among_used_poll_types`,
+  `error_first_linked_vote_used_vote_values_must_be_among_used_vote_values` and
+  `error_next_linked_votes_used_vote_values_must_be_among_used_vote_values`.
+  [gbastien]
+- Added translation for `title_meetingmanagers_notes`.
+  [gbastien]
+- Added translation for `MeetingConfig.enabledAnnexesBatchActions`.
+  [gbastien]
+- Adapted translations for `MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup`
+  and `MeetingConfig.includeGroupsInChargeDefinedOnCategory` fields description
+  now that, when enabled, selected `groupsInCharge` will be stored on the item.
+  [gbastien]
+- Completed french translation for the help message about copy groups on the item view.
+  [gbastien]
+- Added translations for `MeetingConfig.selectableRedefinedPositionTypes` and
+  `directory.position_types` invariant `removed_redefined_position_type_in_use_error` error message.
+  [gbastien]
+
 4.2b8 (2021-01-14)
 ------------------
 
 - Accurate french translation for `Position type to use as label for the signature.`.
   [gbastien]
 
 4.2b7 (2021-01-06)
```

