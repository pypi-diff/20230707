# Comparing `tmp/imio.helpers-0.8.tar.gz` & `tmp/imio.helpers-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.helpers-0.8.tar", last modified: Wed Oct  4 13:44:36 2017, max compression
+gzip compressed data, was "dist/imio.helpers-0.9.tar", last modified: Mon Nov 27 10:01:14 2017, max compression
```

## Comparing `imio.helpers-0.8.tar` & `imio.helpers-0.9.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2017-10-04 13:44:36.000000 imio.helpers-0.8/docs/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2017-10-04 13:44:36.000000 imio.helpers-0.8/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      527 2017-10-04 13:44:36.000000 imio.helpers-0.8/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       86 2017-10-04 13:44:36.000000 imio.helpers-0.8/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15304 2017-10-04 13:44:36.000000 imio.helpers-0.8/PKG-INFO
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/buildout.d/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      767 2017-10-04 13:44:36.000000 imio.helpers-0.8/buildout.d/jenkins.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       95 2017-10-04 13:44:36.000000 imio.helpers-0.8/buildout.d/checkouts.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      745 2017-10-04 13:44:36.000000 imio.helpers-0.8/buildout.d/sources.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      284 2017-10-04 13:44:36.000000 imio.helpers-0.8/buildout.d/base.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      450 2017-10-04 13:44:36.000000 imio.helpers-0.8/buildout.d/versions.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      745 2017-10-04 13:44:36.000000 imio.helpers-0.8/buildout.d/development.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      320 2017-10-04 13:44:36.000000 imio.helpers-0.8/jenkins.cfg
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio.helpers.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio.helpers.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15304 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio.helpers.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio.helpers.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2822 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio.helpers.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio.helpers.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio.helpers.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      122 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio.helpers.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio.helpers.egg-info/not-zip-safe
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      129 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1895 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/security.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      668 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/barcode.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      168 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/profiles/testing/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      232 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/profiles/testing/types.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/profiles/testing/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2770 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/profiles/testing/types/testingtype.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      103 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/profiles/default/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6690 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/date.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      898 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/test_helpers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1743 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/appy_pod.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      235 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/path.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   110704 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/appy_pod.html
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      872 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/testing.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2367 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      319 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2184 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/adapters.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/vocabularies.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      584 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_barcode.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    31315 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_xhtml.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      278 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/barcode.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1502 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_security.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1823 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_appy_pod.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2828 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_date.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      299 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/indexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      497 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_path.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      464 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2928 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_fancytree.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      873 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/dot.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7263 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_content.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9959 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_cache.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8691 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/tests/test_catalog.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3311 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/pdf.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4766 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/catalog.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18727 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/xhtml.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/fancytree/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/fancytree/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2377 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/fancytree/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1206 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/fancytree/fancytree.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      546 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/fancytree/fancytree.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      307 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/fancytree/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7834 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/content.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1066 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1690 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/folder_listing_table.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2037 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1772 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/container.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      656 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/folder_listing.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1403 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/content.pt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1220 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/static/listings.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      681 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/static/helpers.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1370 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4153 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/cache.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      602 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/locales/manual.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/locales/fr/LC_MESSAGES/imio.helpers.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4093 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      969 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/locales/imio.helpers.pot
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      777 2017-10-04 13:44:36.000000 imio.helpers-0.8/src/imio/helpers/locales/update.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      266 2017-10-04 13:44:36.000000 imio.helpers-0.8/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      111 2017-10-04 13:44:36.000000 imio.helpers-0.8/.coveragerc
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      225 2017-10-04 13:44:36.000000 imio.helpers-0.8/travis.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2017-10-04 13:44:36.000000 imio.helpers-0.8/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1565 2017-10-04 13:44:36.000000 imio.helpers-0.8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6159 2017-10-04 13:44:36.000000 imio.helpers-0.8/bootstrap.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10973 2017-10-04 13:44:36.000000 imio.helpers-0.8/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       74 2017-10-04 13:44:36.000000 imio.helpers-0.8/buildout.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      854 2017-10-04 13:44:36.000000 imio.helpers-0.8/.travis.yml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      477 2017-10-04 13:44:36.000000 imio.helpers-0.8/Makefile
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2017-11-27 10:01:14.000000 imio.helpers-0.9/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2017-11-27 10:01:14.000000 imio.helpers-0.9/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      527 2017-11-27 10:01:14.000000 imio.helpers-0.9/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       86 2017-11-27 10:01:14.000000 imio.helpers-0.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15763 2017-11-27 10:01:14.000000 imio.helpers-0.9/PKG-INFO
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/buildout.d/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      767 2017-11-27 10:01:14.000000 imio.helpers-0.9/buildout.d/jenkins.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       62 2017-11-27 10:01:14.000000 imio.helpers-0.9/buildout.d/checkouts.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      587 2017-11-27 10:01:14.000000 imio.helpers-0.9/buildout.d/sources.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      250 2017-11-27 10:01:14.000000 imio.helpers-0.9/buildout.d/base.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      470 2017-11-27 10:01:14.000000 imio.helpers-0.9/buildout.d/versions.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      745 2017-11-27 10:01:14.000000 imio.helpers-0.9/buildout.d/development.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      320 2017-11-27 10:01:14.000000 imio.helpers-0.9/jenkins.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio.helpers.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio.helpers.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15763 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio.helpers.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio.helpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2822 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio.helpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio.helpers.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio.helpers.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      122 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio.helpers.egg-info/requires.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio.helpers.egg-info/not-zip-safe
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      129 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1895 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/security.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      668 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/barcode.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      168 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/profiles/testing/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      232 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/profiles/testing/types.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/profiles/testing/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2770 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/profiles/testing/types/testingtype.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      103 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/profiles/default/jsregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6690 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/date.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      898 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/test_helpers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1743 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/appy_pod.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      235 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/path.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   110944 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/appy_pod.html
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      872 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/testing.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2367 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      319 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2184 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/vocabularies.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      584 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_barcode.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    31600 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_xhtml.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      278 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/barcode.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1502 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_security.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1823 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_appy_pod.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2828 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_date.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      299 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/indexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      497 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_path.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      464 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2928 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_fancytree.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      873 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/dot.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9883 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_content.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9959 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_cache.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8691 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/tests/test_catalog.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3311 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/pdf.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4766 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/catalog.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18728 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/xhtml.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/fancytree/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/fancytree/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2377 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/fancytree/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1206 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/fancytree/fancytree.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      546 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/fancytree/fancytree.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      307 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/fancytree/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9248 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/content.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1066 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1690 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/folder_listing_table.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2037 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1772 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/container.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      656 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/folder_listing.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1403 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/content.pt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1220 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/static/listings.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      681 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/static/helpers.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1370 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4153 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/cache.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      602 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/locales/manual.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/locales/fr/LC_MESSAGES/imio.helpers.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4093 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      969 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/locales/imio.helpers.pot
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      777 2017-11-27 10:01:14.000000 imio.helpers-0.9/src/imio/helpers/locales/update.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      266 2017-11-27 10:01:14.000000 imio.helpers-0.9/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      111 2017-11-27 10:01:14.000000 imio.helpers-0.9/.coveragerc
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      225 2017-11-27 10:01:14.000000 imio.helpers-0.9/travis.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2017-11-27 10:01:14.000000 imio.helpers-0.9/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1565 2017-11-27 10:01:14.000000 imio.helpers-0.9/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6159 2017-11-27 10:01:14.000000 imio.helpers-0.9/bootstrap.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11302 2017-11-27 10:01:14.000000 imio.helpers-0.9/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       74 2017-11-27 10:01:14.000000 imio.helpers-0.9/buildout.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      854 2017-11-27 10:01:14.000000 imio.helpers-0.9/.travis.yml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      493 2017-11-27 10:01:14.000000 imio.helpers-0.9/Makefile
```

### Comparing `imio.helpers-0.8/docs/LICENSE.rst` & `imio.helpers-0.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/docs/LICENSE.GPL` & `imio.helpers-0.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/README.rst` & `imio.helpers-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/PKG-INFO` & `imio.helpers-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: imio.helpers
-Version: 0.8
+Version: 0.9
 Summary: Various helper methods for development.
 Home-page: http://pypi.python.org/pypi/imio.helpers
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL
+Description-Content-Type: UNKNOWN
 Description: .. image:: https://travis-ci.org/IMIO/imio.helpers.svg?branch=master
            :target: https://travis-ci.org/IMIO/imio.helpers
         
         .. image:: https://coveralls.io/repos/IMIO/imio.helpers/badge.png?branch=master
            :target: https://coveralls.io/r/IMIO/imio.helpers?branch=master
         
         
@@ -32,14 +33,26 @@
         
         - Simon Delcourt, simon.delcourt@imio.be
         - Gauthier Bastien, gauthier.bastien@imio.be
         
         Changelog
         =========
         
+        0.9 (2017-11-27)
+        ----------------
+        
+        - Added appy.pod usecase for complex styles start/end on same paragraph.
+          [gbastien]
+        - Do not break in `xhtml.storeImagesLocally` when no `<img> src` found.
+          [gbastien]
+        - Add methods to manage annotations (Add and Remove).
+          [anuyens, odelaere]
+        - Added method to get annotation
+          [sgeulette]
+        
         0.8 (2017-10-04)
         ----------------
         
         - In `xhtml.storeImagesLocally`, take into account `<img> src`
           that uses `resolveuid`.  This is the case when using `collective.ckeditor` and
           option `allow_link_byuid` is enabled.
           [gbastien]
@@ -74,15 +87,15 @@
           validation for `Choice` field that is `required=False` and for which given
           value is None. Validation fails because None not in vocabulary but it is
           nevertheless a correct value as it is managed by the widget while added thru
           the UI.
           [gbastien]
         - Added JS fix to be able to print `<fieldset>` on several pages in Firefox,
           see https://bugzilla.mozilla.org/show_bug.cgi?id=471015.
-          This makes it necessary to add a default profile to add the JS resource 
+          This makes it necessary to add a default profile to add the JS resource
           `++resource++imio.helpers/helpers.js`.
           [gbastien]
         
         0.4.29 (2017-07-25)
         -------------------
         
         - Get intid value or create it if not found.
```

### Comparing `imio.helpers-0.8/buildout.d/jenkins.cfg` & `imio.helpers-0.9/buildout.d/jenkins.cfg`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/buildout.d/development.cfg` & `imio.helpers-0.9/buildout.d/development.cfg`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio.helpers.egg-info/PKG-INFO` & `imio.helpers-0.9/src/imio.helpers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: imio.helpers
-Version: 0.8
+Version: 0.9
 Summary: Various helper methods for development.
 Home-page: http://pypi.python.org/pypi/imio.helpers
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL
+Description-Content-Type: UNKNOWN
 Description: .. image:: https://travis-ci.org/IMIO/imio.helpers.svg?branch=master
            :target: https://travis-ci.org/IMIO/imio.helpers
         
         .. image:: https://coveralls.io/repos/IMIO/imio.helpers/badge.png?branch=master
            :target: https://coveralls.io/r/IMIO/imio.helpers?branch=master
         
         
@@ -32,14 +33,26 @@
         
         - Simon Delcourt, simon.delcourt@imio.be
         - Gauthier Bastien, gauthier.bastien@imio.be
         
         Changelog
         =========
         
+        0.9 (2017-11-27)
+        ----------------
+        
+        - Added appy.pod usecase for complex styles start/end on same paragraph.
+          [gbastien]
+        - Do not break in `xhtml.storeImagesLocally` when no `<img> src` found.
+          [gbastien]
+        - Add methods to manage annotations (Add and Remove).
+          [anuyens, odelaere]
+        - Added method to get annotation
+          [sgeulette]
+        
         0.8 (2017-10-04)
         ----------------
         
         - In `xhtml.storeImagesLocally`, take into account `<img> src`
           that uses `resolveuid`.  This is the case when using `collective.ckeditor` and
           option `allow_link_byuid` is enabled.
           [gbastien]
@@ -74,15 +87,15 @@
           validation for `Choice` field that is `required=False` and for which given
           value is None. Validation fails because None not in vocabulary but it is
           nevertheless a correct value as it is managed by the widget while added thru
           the UI.
           [gbastien]
         - Added JS fix to be able to print `<fieldset>` on several pages in Firefox,
           see https://bugzilla.mozilla.org/show_bug.cgi?id=471015.
-          This makes it necessary to add a default profile to add the JS resource 
+          This makes it necessary to add a default profile to add the JS resource
           `++resource++imio.helpers/helpers.js`.
           [gbastien]
         
         0.4.29 (2017-07-25)
         -------------------
         
         - Get intid value or create it if not found.
```

### Comparing `imio.helpers-0.8/src/imio.helpers.egg-info/SOURCES.txt` & `imio.helpers-0.9/src/imio.helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/security.py` & `imio.helpers-0.9/src/imio/helpers/security.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/barcode.py` & `imio.helpers-0.9/src/imio/helpers/barcode.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/profiles/testing/types/testingtype.xml` & `imio.helpers-0.9/src/imio/helpers/profiles/testing/types/testingtype.xml`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/date.py` & `imio.helpers-0.9/src/imio/helpers/date.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/test_helpers.py` & `imio.helpers-0.9/src/imio/helpers/test_helpers.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/appy_pod.py` & `imio.helpers-0.9/src/imio/helpers/appy_pod.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/appy_pod.html` & `imio.helpers-0.9/src/imio/helpers/appy_pod.html`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,21 @@
 <p><s><em><strong>gras italique barré</strong></em></s>;</p>
 <p><u><em><strong>gras italique souligné</strong></em></u>;</p>
 <p><u><s><strong>gras barré souligné</strong></s></u>;</p>
 <p><s><u><em><strong>gras italique barré souligné</strong></em></u></s>.</p>
 
 <p>&nbsp;</p>
 
+<p style="color: #0000FF;"><u><strong>Styles qui ne se finissent pas en même temps :</strong></u></p>
+
+<p><s><u>test </u><u>test</u> test test <u>test</u></s></p>
+<p><s><u>test </u><u>test</u> test test</s> <u>test</u></p>
+
+<p>&nbsp;</p>
+
 <p style="color: #0000FF;"><u><strong>Utilisation de CSS pour la mise en forme :</strong></u></p>
 
 <p>&nbsp;</p>
 style directement sur &lt;li style=...&gt;
 <ul>
     <li style="font-style: italic; text-decoration: line-through;">italique barré;</li>
     <li style="font-style: italic; font-weight: bold;">italique gras;</li>
```

### Comparing `imio.helpers-0.8/src/imio/helpers/testing.zcml` & `imio.helpers-0.9/src/imio/helpers/testing.zcml`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/testing.py` & `imio.helpers-0.9/src/imio/helpers/testing.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/adapters.py` & `imio.helpers-0.9/src/imio/helpers/adapters.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/tests/vocabularies.py` & `imio.helpers-0.9/src/imio/helpers/tests/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/tests/test_barcode.py` & `imio.helpers-0.9/src/imio/helpers/tests/test_barcode.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/tests/test_xhtml.py` & `imio.helpers-0.9/src/imio/helpers/tests/test_xhtml.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,7 +558,13 @@
         self.assertEqual(self.portal.folder.objectIds(), ['dot.gif', 'dot2.gif'])
         new_img = self.portal.folder.get('dot.gif')
         new_img2 = self.portal.folder.get('dot2.gif')
         expected = '<p>Internal image full url <img src="resolveuid/{0}"/>.</p>' \
             '<p>Internal image resolveuid <img src="resolveuid/{1}"/>.</p>'.format(
                 new_img.UID(), new_img2.UID())
         self.assertEqual(result, expected)
+
+    def test_storeImagesLocallyWithoutSrc(self):
+        """Do not fail when no src in the <img> tag."""
+        text = '<p>Text <img style="width: 50px; height: 50px;"/>.</p>'
+        # nothing was changed
+        self.assertEqual(storeImagesLocally(self.portal.folder, text), text)
```

### Comparing `imio.helpers-0.8/src/imio/helpers/tests/test_security.py` & `imio.helpers-0.9/src/imio/helpers/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/tests/test_appy_pod.py` & `imio.helpers-0.9/src/imio/helpers/tests/test_appy_pod.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/tests/test_date.py` & `imio.helpers-0.9/src/imio/helpers/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/tests/test_fancytree.py` & `imio.helpers-0.9/src/imio/helpers/tests/test_fancytree.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/tests/dot.gif` & `imio.helpers-0.9/src/imio/helpers/tests/dot.gif`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/tests/test_cache.py` & `imio.helpers-0.9/src/imio/helpers/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/tests/test_catalog.py` & `imio.helpers-0.9/src/imio/helpers/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/pdf.py` & `imio.helpers-0.9/src/imio/helpers/pdf.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/catalog.py` & `imio.helpers-0.9/src/imio/helpers/catalog.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/xhtml.py` & `imio.helpers-0.9/src/imio/helpers/xhtml.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
         name_chooser = INameChooser(context)
     except TypeError:
         parent = context.getParentNode()
         name_chooser = INameChooser(parent)
     # return received xhtmlContent if nothing was changed
     changed = False
     for img in imgs:
-        img_src = img.attrib['src']
+        img_src = img.get('src', '')
         # we only handle http stored images
         if not img_src.startswith('http') and not img_src.startswith('resolveuid'):
             continue
         filename = data = None
         # external images
         if store_external_images and not img_src.startswith(portal_url):
             filename, data = _handle_external_image(img_src)
```

### Comparing `imio.helpers-0.8/src/imio/helpers/fancytree/views.py` & `imio.helpers-0.9/src/imio/helpers/fancytree/views.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/fancytree/fancytree.pt` & `imio.helpers-0.9/src/imio/helpers/fancytree/fancytree.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/fancytree/fancytree.js` & `imio.helpers-0.9/src/imio/helpers/fancytree/fancytree.js`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/content.py` & `imio.helpers-0.9/src/imio/helpers/content.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 
+import logging
 import os
-from zope.schema._field import Choice
 
+from Products.CMFCore.WorkflowCore import WorkflowException
+from Products.CMFPlone.utils import safe_unicode
 from plone import api
+from plone.api.validation import mutually_exclusive_parameters
 from plone.app.textfield.value import RichTextValue
 from plone.namedfile.file import NamedBlobFile, NamedBlobImage
+from zope.annotation import IAnnotations
+from zope.schema._field import Choice
 
-from Products.CMFCore.WorkflowCore import WorkflowException
-from Products.CMFPlone.utils import safe_unicode
-
-import logging
 logger = logging.getLogger('imo.helpers.content')
 
 
 def get_object(parent='', id='', title='', type='', obj_path=''):
     """
     Find an object following parameters
     :param id: searched id.
@@ -222,7 +223,52 @@
 def safe_encode(value, encoding='utf-8'):
     """
         Converts a value to encoding, only when it is not already encoded.
     """
     if isinstance(value, unicode):
         return value.encode(encoding)
     return value
+
+
+@mutually_exclusive_parameters('obj', 'uid')
+def add_to_annotation(annotation_key, value, obj=None, uid=None):
+    """ Add annotation related to obj or uid """
+    if not obj:
+        obj = api.content.get(UID=uid)
+
+    # api.content.get may return None
+    if obj:
+        annot = IAnnotations(obj)
+        if annotation_key not in annot:
+            annot[annotation_key] = set([])
+        annot[annotation_key].add(value)
+
+
+@mutually_exclusive_parameters('obj', 'uid')
+def del_from_annotation(annotation_key, value, obj=None, uid=None):
+    """ Delete annotation related to obj or uid """
+    if not obj:
+        obj = api.content.get(UID=uid)
+
+    # api.content.get may return None
+    if obj:
+        annot = IAnnotations(obj)
+        if annotation_key not in annot:
+            return
+        if value in annot[annotation_key]:
+            annot[annotation_key].remove(value)
+
+
+@mutually_exclusive_parameters('obj', 'uid')
+def get_from_annotation(annotation_key, obj=None, uid=None, default=None):
+    """ Get annotation related to obj or uid """
+    if not obj:
+        obj = api.content.get(UID=uid)
+
+    # api.content.get may return None
+    if not obj:
+        return default
+
+    annot = IAnnotations(obj)
+    if annotation_key not in annot:
+        return default
+    return annot[annotation_key]
```

### Comparing `imio.helpers-0.8/src/imio/helpers/configure.zcml` & `imio.helpers-0.9/src/imio/helpers/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/browser/folder_listing_table.pt` & `imio.helpers-0.9/src/imio/helpers/browser/folder_listing_table.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/browser/views.py` & `imio.helpers-0.9/src/imio/helpers/browser/views.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/browser/container.pt` & `imio.helpers-0.9/src/imio/helpers/browser/container.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/browser/folder_listing.pt` & `imio.helpers-0.9/src/imio/helpers/browser/folder_listing.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/browser/content.pt` & `imio.helpers-0.9/src/imio/helpers/browser/content.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/browser/static/listings.js` & `imio.helpers-0.9/src/imio/helpers/browser/static/listings.js`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/browser/static/helpers.js` & `imio.helpers-0.9/src/imio/helpers/browser/static/helpers.js`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/browser/configure.zcml` & `imio.helpers-0.9/src/imio/helpers/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/cache.py` & `imio.helpers-0.9/src/imio/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/locales/manual.pot` & `imio.helpers-0.9/src/imio/helpers/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/locales/fr/LC_MESSAGES/imio.helpers.po` & `imio.helpers-0.9/src/imio/helpers/locales/fr/LC_MESSAGES/imio.helpers.po`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po` & `imio.helpers-0.9/src/imio/helpers/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/locales/imio.helpers.pot` & `imio.helpers-0.9/src/imio/helpers/locales/imio.helpers.pot`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/src/imio/helpers/locales/update.sh` & `imio.helpers-0.9/src/imio/helpers/locales/update.sh`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/setup.py` & `imio.helpers-0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     + '\n' +
     open('CHANGES.rst').read()
     + '\n')
 
 
 setup(
     name='imio.helpers',
-    version='0.8',
+    version='0.9',
     description="Various helper methods for development.",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `imio.helpers-0.8/bootstrap.py` & `imio.helpers-0.9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-0.8/CHANGES.rst` & `imio.helpers-0.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Changelog
 =========
 
+0.9 (2017-11-27)
+----------------
+
+- Added appy.pod usecase for complex styles start/end on same paragraph.
+  [gbastien]
+- Do not break in `xhtml.storeImagesLocally` when no `<img> src` found.
+  [gbastien]
+- Add methods to manage annotations (Add and Remove).
+  [anuyens, odelaere]
+- Added method to get annotation
+  [sgeulette]
+
 0.8 (2017-10-04)
 ----------------
 
 - In `xhtml.storeImagesLocally`, take into account `<img> src`
   that uses `resolveuid`.  This is the case when using `collective.ckeditor` and
   option `allow_link_byuid` is enabled.
   [gbastien]
@@ -39,15 +51,15 @@
   validation for `Choice` field that is `required=False` and for which given
   value is None. Validation fails because None not in vocabulary but it is
   nevertheless a correct value as it is managed by the widget while added thru
   the UI.
   [gbastien]
 - Added JS fix to be able to print `<fieldset>` on several pages in Firefox,
   see https://bugzilla.mozilla.org/show_bug.cgi?id=471015.
-  This makes it necessary to add a default profile to add the JS resource 
+  This makes it necessary to add a default profile to add the JS resource
   `++resource++imio.helpers/helpers.js`.
   [gbastien]
 
 0.4.29 (2017-07-25)
 -------------------
 
 - Get intid value or create it if not found.
```

### Comparing `imio.helpers-0.8/.travis.yml` & `imio.helpers-0.9/.travis.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 before_install:
   - sudo apt-get install libpng12-dev cmake libqt4-dev libqt5widgets5 qttools5-dev
   - sudo wget https://10gbps-io.dl.sourceforge.net/project/zint/zint/2.6.0/zint_2.6.0_amd64.deb
   - sudo dpkg -i zint_2.6.0_amd64.deb
 
 install:
   - mkdir -p buildout-cache/{eggs,downloads}
-  - python bootstrap.py --version=2.5.3 -c travis.cfg
+  - python bootstrap.py --version=2.9.5 -c travis.cfg
   - bin/buildout -c travis.cfg -N annotate
   - bin/buildout -c travis.cfg -Nqt 5
 
 script:
   - bin/test
 
 after_success:
```

