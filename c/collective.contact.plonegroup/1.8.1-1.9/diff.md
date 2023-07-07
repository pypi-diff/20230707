# Comparing `tmp/collective.contact.plonegroup-1.8.1.tar.gz` & `tmp/collective.contact.plonegroup-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.contact.plonegroup-1.8.1.tar", last modified: Mon Jul 30 10:20:52 2018, max compression
+gzip compressed data, was "dist/collective.contact.plonegroup-1.9.tar", last modified: Tue Sep  4 12:30:10 2018, max compression
```

## Comparing `collective.contact.plonegroup-1.8.1.tar` & `collective.contact.plonegroup-1.9.tar`

### file list

```diff
@@ -1,85 +1,90 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     6322 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     1716 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6158 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/bootstrap.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1865 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      431 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)      138 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)     2354 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      402 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/.travis.yml
--rw-rw-r--   0 sge       (1000) sge       (1000)      354 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/.coveragerc
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/
--rw-rw-r--   0 sge       (1000) sge       (1000)       71 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/.gitignore
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/top_level.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      165 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)       30 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       53 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)     3127 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)     6322 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/PKG-INFO
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/
--rw-rw-r--   0 sge       (1000) sge       (1000)       56 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/
--rw-rw-r--   0 sge       (1000) sge       (1000)       56 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2338 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      549 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/testing.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2165 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/testing.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1769 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/subscribers.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     8543 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/subscribers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      621 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/setuphandlers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      528 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/interfaces.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1004 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)      277 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/config.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      234 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/upgrades/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2216 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/upgrades/upgrades.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      713 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/upgrades/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/upgrades/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)     4393 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/test_utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1419 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/test_upgrades.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     8091 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/test_subscribers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1327 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/test_setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    10792 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/test_settings.py
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/testing/
--rw-rw-r--   0 sge       (1000) sge       (1000)      230 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/testing/types.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      177 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/testing/metadata.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/testing/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2721 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/testing/types/acontent.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)      138 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/default/registry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      172 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/default/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      366 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/default/jsregistry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      403 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/default/import_steps.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      567 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/default/controlpanel.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/default/collective.contactplonegroup_marker.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      186 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/default/browserlayer.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/
--rwxrwxr-x   0 sge       (1000) sge       (1000)      272 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/update.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)      819 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/plone.pot
--rw-rw-r--   0 sge       (1000) sge       (1000)     2783 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/collective.contact.plonegroup.pot
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)      764 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     3832 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/collective.contact.plonegroup.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/content/
--rw-rw-r--   0 sge       (1000) sge       (1000)      166 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/content/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/content/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/browser/
--rw-rw-r--   0 sge       (1000) sge       (1000)    16400 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/browser/settings.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      806 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/browser/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/browser/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/browser/static/
--rw-rw-r--   0 sge       (1000) sge       (1000)      245 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/browser/static/plonegroup.js
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/browser/static/.gitkeep
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/browser/overrides/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/browser/overrides/.gitkeep
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)      732 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/docs/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2018-07-30 10:20:52.000000 collective.contact.plonegroup-1.8.1/docs/LICENSE.GPL
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1865 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6935 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/PKG-INFO
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      234 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1769 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/subscribers.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/testing/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      230 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/testing/types.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/testing/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2721 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/testing/types/acontent.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/default/collective.contactplonegroup_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      172 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/default/jsregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      567 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/default/controlpanel.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      138 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/default/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      371 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      186 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      403 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/default/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2503 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8543 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/subscribers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      549 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/content/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/content/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      166 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/content/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2165 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      528 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/interfaces.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/upgrades/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/upgrades/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2216 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/upgrades/upgrades.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1084 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/upgrades/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1327 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8091 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/test_subscribers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1419 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/test_upgrades.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10792 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/test_settings.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4393 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/test_utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      621 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/setuphandlers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      277 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1004 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/overrides/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/overrides/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16871 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/settings.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1195 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/templates/suborganizations.pt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      245 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/static/plonegroup.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/static/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/static/plonegroup.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4322 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/tables.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2617 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3136 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/collective.contact.plonegroup.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      819 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/plone.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4388 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/collective.contact.plonegroup.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      764 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/plone.po
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      272 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/update.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6935 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3382 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       30 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      196 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/requires.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       71 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/src/.gitignore
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      454 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      354 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/.coveragerc
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1756 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6158 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/bootstrap.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2865 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      402 2018-09-04 12:30:10.000000 collective.contact.plonegroup-1.9/.travis.yml
```

### Comparing `collective.contact.plonegroup-1.8.1/PKG-INFO` & `collective.contact.plonegroup-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.contact.plonegroup
-Version: 1.8.1
+Version: 1.9
 Summary: Organizations and functions combinations to create plone groups
 Home-page: http://pypi.python.org/pypi/collective.contact.plonegroup
 Author: Ecreall, Entrouvert, IMIO
 Author-email: s.geulette@imio.be
 License: GPL
 Description: .. contents::
         
@@ -65,14 +65,27 @@
         - Cédric Messiant, Ecreall
         - Frédéric Peters, Entr'ouvert
         
         Changelog
         =========
         
         
+        1.9 (2018-09-04)
+        ----------------
+        
+        - Added utils.get_plone_group_id to get Plone group id for given organization and suffix.
+          [gbastien]
+        - Overrided "@@suborganizations" view to display the entire hierarchy of contained
+          organizations and sub-organizations and more informations in a table.
+          [gbastien]
+        - When the plonegroup-organization is displayed in a tooltip, use original way
+          to display sub organizations because the new rendering using the table takes
+          too much place in the tooltip.
+          [gbastien]
+        
         1.8.1 (2018-07-30)
         ------------------
         
         - Sort user vocabulary by fullname
           [sgeulette]
         - Added cache on travis.
           [sgeulette]
```

### Comparing `collective.contact.plonegroup-1.8.1/setup.py` & `collective.contact.plonegroup-1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     + '\n' +
     open('CHANGES.rst').read()
     + '\n')
 
 
 setup(
     name='collective.contact.plonegroup',
-    version='1.8.1',
+    version='1.9',
     description="Organizations and functions combinations to create plone groups",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.2",
@@ -42,14 +42,15 @@
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'five.grok',
         'plone.api',
         'setuptools',
         'collective.contact.core',
+        'collective.eeafaceted.z3ctable',
         'collective.elephantvocabulary',
         'imio.helpers > 0.4.13'
     ],
     extras_require={
         'test': [
             'ecreall.helpers.testing',
             'plone.app.testing',
```

### Comparing `collective.contact.plonegroup-1.8.1/bootstrap.py` & `collective.contact.plonegroup-1.9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/README.rst` & `collective.contact.plonegroup-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/CHANGES.rst` & `collective.contact.plonegroup-1.9/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 Changelog
 =========
 
 
+1.9 (2018-09-04)
+----------------
+
+- Added utils.get_plone_group_id to get Plone group id for given organization and suffix.
+  [gbastien]
+- Overrided "@@suborganizations" view to display the entire hierarchy of contained
+  organizations and sub-organizations and more informations in a table.
+  [gbastien]
+- When the plonegroup-organization is displayed in a tooltip, use original way
+  to display sub organizations because the new rendering using the table takes
+  too much place in the tooltip.
+  [gbastien]
+
 1.8.1 (2018-07-30)
 ------------------
 
 - Sort user vocabulary by fullname
   [sgeulette]
 - Added cache on travis.
   [sgeulette]
```

### Comparing `collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/SOURCES.txt` & `collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,31 @@
 src/collective/contact/plonegroup/subscribers.zcml
 src/collective/contact/plonegroup/testing.py
 src/collective/contact/plonegroup/testing.zcml
 src/collective/contact/plonegroup/utils.py
 src/collective/contact/plonegroup/browser/__init__.py
 src/collective/contact/plonegroup/browser/configure.zcml
 src/collective/contact/plonegroup/browser/settings.py
+src/collective/contact/plonegroup/browser/tables.py
 src/collective/contact/plonegroup/browser/overrides/.gitkeep
 src/collective/contact/plonegroup/browser/static/.gitkeep
+src/collective/contact/plonegroup/browser/static/plonegroup.css
 src/collective/contact/plonegroup/browser/static/plonegroup.js
+src/collective/contact/plonegroup/browser/templates/suborganizations.pt
 src/collective/contact/plonegroup/content/__init__.py
 src/collective/contact/plonegroup/content/configure.zcml
 src/collective/contact/plonegroup/locales/collective.contact.plonegroup.pot
 src/collective/contact/plonegroup/locales/plone.pot
 src/collective/contact/plonegroup/locales/update.sh
 src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/collective.contact.plonegroup.po
 src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/plone.po
 src/collective/contact/plonegroup/profiles/default/browserlayer.xml
 src/collective/contact/plonegroup/profiles/default/collective.contactplonegroup_marker.txt
 src/collective/contact/plonegroup/profiles/default/controlpanel.xml
+src/collective/contact/plonegroup/profiles/default/cssregistry.xml
 src/collective/contact/plonegroup/profiles/default/import_steps.xml
 src/collective/contact/plonegroup/profiles/default/jsregistry.xml
 src/collective/contact/plonegroup/profiles/default/metadata.xml
 src/collective/contact/plonegroup/profiles/default/registry.xml
 src/collective/contact/plonegroup/profiles/testing/metadata.xml
 src/collective/contact/plonegroup/profiles/testing/types.xml
 src/collective/contact/plonegroup/profiles/testing/types/acontent.xml
```

### Comparing `collective.contact.plonegroup-1.8.1/src/collective.contact.plonegroup.egg-info/PKG-INFO` & `collective.contact.plonegroup-1.9/src/collective.contact.plonegroup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.contact.plonegroup
-Version: 1.8.1
+Version: 1.9
 Summary: Organizations and functions combinations to create plone groups
 Home-page: http://pypi.python.org/pypi/collective.contact.plonegroup
 Author: Ecreall, Entrouvert, IMIO
 Author-email: s.geulette@imio.be
 License: GPL
 Description: .. contents::
         
@@ -65,14 +65,27 @@
         - Cédric Messiant, Ecreall
         - Frédéric Peters, Entr'ouvert
         
         Changelog
         =========
         
         
+        1.9 (2018-09-04)
+        ----------------
+        
+        - Added utils.get_plone_group_id to get Plone group id for given organization and suffix.
+          [gbastien]
+        - Overrided "@@suborganizations" view to display the entire hierarchy of contained
+          organizations and sub-organizations and more informations in a table.
+          [gbastien]
+        - When the plonegroup-organization is displayed in a tooltip, use original way
+          to display sub organizations because the new rendering using the table takes
+          too much place in the tooltip.
+          [gbastien]
+        
         1.8.1 (2018-07-30)
         ------------------
         
         - Sort user vocabulary by fullname
           [sgeulette]
         - Added cache on travis.
           [sgeulette]
```

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/utils.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,21 @@
             continue
         group_suffix = '_'.join(parts[1:])
         if group_suffix in suffixes and parts[0] not in orgs:
             orgs.append(parts[0])
     return orgs
 
 
+def get_plone_group_id(org, suffix):
+    """
+        Return Plone group id corresponding to org_uid/suffix.
+    """
+    return '{0}_{1}'.format(org.UID(), suffix)
+
+
 def get_selected_org_suffix_users(org_uid, suffixes):
     """
         Get users that belongs to suffixed groups related to selected organization.
     """
     org_members = []
     # only add to vocabulary users with these functions in the organization
     for function_id in suffixes:
```

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/testing.zcml` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/testing.zcml`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/testing.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/testing.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/subscribers.zcml` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/subscribers.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/subscribers.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/setuphandlers.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/interfaces.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/configure.zcml` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/upgrades/upgrades.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/upgrades/configure.zcml` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/upgrades/configure.zcml`

 * *Files 11% similar despite different names*

```diff
@@ -15,8 +15,18 @@
       title="Migration profile for collective.contact.plonegroup to 3"
       description="Upgrade from 2 to 3"
       source="2"
       destination="3"
       handler=".upgrades.v3"
       profile="collective.contact.plonegroup:default" />
 
+  <genericsetup:upgradeSteps
+      source="3"
+      destination="4"
+      profile="collective.contact.plonegroup:default">
+      <genericsetup:upgradeDepends
+          title="Migration profile for collective.contact.plonegroup to 4"
+          description="Register new plonegroup.css in portal_css"
+          import_steps="cssregistry" />
+  </genericsetup:upgradeSteps>
+
 </configure>
```

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/test_utils.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/test_upgrades.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/test_upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/test_subscribers.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/test_setup.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/tests/test_settings.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/testing/types/acontent.xml` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/testing/types/acontent.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/profiles/default/controlpanel.xml` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/plone.pot` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/plone.po`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-# --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
-# SOME DESCRIPTIVE TITLE.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2017-02-27 08:54+0000\n"
+"POT-Creation-Date: 2018-08-28 14:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
-"Domain: plone\n"
+"Domain: DOMAIN\n"
 
 #: ../profiles/testing/types/acontent.xml
 msgid "A content"
-msgstr ""
+msgstr "A content"
 
 #: ../profiles/default/controlpanel.xml
 msgid "Contact Plone Group settings"
-msgstr ""
+msgstr "Configuration des groupes plone via contact"
 
 #: ../profiles/testing/types/acontent.xml
 msgid "None"
-msgstr ""
+msgstr "None"
```

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/collective.contact.plonegroup.pot` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/collective.contact.plonegroup.pot`

 * *Files 9% similar despite different names*

```diff
@@ -1,114 +1,127 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2017-02-27 08:54+0000\n"
+"POT-Creation-Date: 2018-08-28 14:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: collective.contact.plonegroup\n"
 
-#: ../browser/settings.py:109
+#: ../browser/tables.py:126
+msgid "Actions"
+msgstr ""
+
+#: ../browser/settings.py:117
 msgid "Choose multiple organization levels for which you want to create a plone group."
 msgstr ""
 
-#: ../browser/settings.py:116
+#: ../browser/settings.py:124
 msgid "Each defined function will suffix each organization plone group."
 msgstr ""
 
-#: ../browser/settings.py:118
+#: ../browser/settings.py:126
 msgid "Function"
 msgstr ""
 
-#: ../browser/settings.py:115
+#: ../browser/settings.py:123
 msgid "Function list"
 msgstr ""
 
 #: ../configure.zcml:29
 msgid "Installs the collective.contact.plonegroup add-on."
 msgstr ""
 
-#: ../browser/settings.py:37
+#: ../browser/settings.py:45
 msgid "Organization id"
 msgstr ""
 
-#: ../browser/settings.py:38
+#: ../browser/settings.py:46
 msgid "Organization title"
 msgstr ""
 
-#: ../browser/settings.py:45
+#: ../browser/settings.py:53
 msgid "Plone group suffix id"
 msgstr ""
 
-#: ../browser/settings.py:46
+#: ../browser/settings.py:54
 msgid "Plone group suffix title"
 msgstr ""
 
-#: ../browser/settings.py:108
+#: ../browser/tables.py:110
+msgid "Selected in plonegroup"
+msgstr ""
+
+#: ../browser/settings.py:116
 msgid "Selected organizations"
 msgstr ""
 
 #: ../testing.zcml:16
 msgid "Steps to ease tests of collective.contact.plonegroup"
 msgstr ""
 
-#: ../subscribers.py:136
+#: ../subscribers.py:147
 msgid "This contact is selected in configuration"
 msgstr ""
 
-#: ../subscribers.py:142
+#: ../subscribers.py:153
 msgid "This contact is used in following content: ${items}"
 msgstr ""
 
-#: ../browser/settings.py:289
+#: ../browser/settings.py:300
 msgid "This organization or a contained organization is used in plonegroup configuration ! Remove it first from the configuration !"
 msgstr ""
 
-#: ../subscribers.py:148
+#: ../subscribers.py:159
 msgid "You cannot deactivate this item !"
 msgstr ""
 
-#: ../subscribers.py:189
+#: ../subscribers.py:200
 msgid "You cannot delete the group '${group}', linked to used organization '${orga}'."
 msgstr ""
 
-#: ../browser/settings.py:288
+#: ../browser/settings.py:299
 msgid "You cannot delete this item !"
 msgstr ""
 
-#: ../browser/settings.py:126
+#: ../browser/settings.py:134
 msgid "You must choose at least one organization !"
 msgstr ""
 
-#: ../browser/settings.py:128
+#: ../browser/settings.py:136
 msgid "You must correct the organization error first !"
 msgstr ""
 
-#: ../browser/settings.py:86
+#: ../browser/settings.py:94
 msgid "You must define an organization with id '${pgo}' !"
 msgstr ""
 
-#: ../browser/settings.py:130
+#: ../browser/settings.py:138
 msgid "You must define at least one function !"
 msgstr ""
 
-#: ../browser/settings.py:90
+#: ../browser/settings.py:98
 msgid "You must have only one organization with id '${pgo}' !"
 msgstr ""
 
 #: ../configure.zcml:29
 msgid "collective.contact.plonegroup"
 msgstr ""
 
 #: ../testing.zcml:16
 msgid "collective.contact.plonegroup tests"
 msgstr ""
+
+#. Default: "For convenience, organizations are listed alphabetically. Order is defined in the ${plonegroup_config_url}."
+#: ../browser/templates/suborganizations.pt:5
+msgid "help_organizations_sorted_alphabetically"
+msgstr ""
```

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/plone.po` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/plone.pot`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+# --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
+# SOME DESCRIPTIVE TITLE.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2017-02-27 08:54+0000\n"
+"POT-Creation-Date: 2018-08-28 14:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
-"Domain: DOMAIN\n"
+"Domain: plone\n"
 
 #: ../profiles/testing/types/acontent.xml
 msgid "A content"
-msgstr "A content"
+msgstr ""
 
 #: ../profiles/default/controlpanel.xml
 msgid "Contact Plone Group settings"
-msgstr "Configuration des groupes plone via contact"
+msgstr ""
 
 #: ../profiles/testing/types/acontent.xml
 msgid "None"
-msgstr "None"
+msgstr ""
```

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/collective.contact.plonegroup.po` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/locales/fr/LC_MESSAGES/collective.contact.plonegroup.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,112 +1,125 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2017-02-27 08:54+0000\n"
+"POT-Creation-Date: 2018-08-28 14:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: fr\n"
 "Language-Name: French\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: collective.contact.plonegroup\n"
 "X-is-fallback-for: fr-fr fr-be fr-ca\n"
 
-#: ../browser/settings.py:109
+#: ../browser/tables.py:126
+msgid "Actions"
+msgstr "Actions"
+
+#: ../browser/settings.py:117
 msgid "Choose multiple organization levels for which you want to create a plone group."
 msgstr "Choisir des niveaux d'organisation pour lesquels un groupe plone sera créé."
 
-#: ../browser/settings.py:116
+#: ../browser/settings.py:124
 msgid "Each defined function will suffix each organization plone group."
 msgstr "Chaque fonction définie suffixera les groupes plone créés."
 
-#: ../browser/settings.py:118
+#: ../browser/settings.py:126
 msgid "Function"
 msgstr "Fonction"
 
-#: ../browser/settings.py:115
+#: ../browser/settings.py:123
 msgid "Function list"
 msgstr "Liste de fonctions"
 
 #: ../configure.zcml:29
 msgid "Installs the collective.contact.plonegroup add-on."
 msgstr "Installs the collective.contact.plonegroup add-on."
 
-#: ../browser/settings.py:37
+#: ../browser/settings.py:45
 msgid "Organization id"
 msgstr "Id de l'organisation"
 
-#: ../browser/settings.py:38
+#: ../browser/settings.py:46
 msgid "Organization title"
 msgstr "Titre de l'organisation"
 
-#: ../browser/settings.py:45
+#: ../browser/settings.py:53
 msgid "Plone group suffix id"
 msgstr "Id du suffixe"
 
-#: ../browser/settings.py:46
+#: ../browser/settings.py:54
 msgid "Plone group suffix title"
 msgstr "Titre du suffixe"
 
-#: ../browser/settings.py:108
+#: ../browser/tables.py:110
+msgid "Selected in plonegroup"
+msgstr "Sélectionné dans \"Configuration des groupes plone via contact\""
+
+#: ../browser/settings.py:116
 msgid "Selected organizations"
 msgstr "Organisations"
 
 #: ../testing.zcml:16
 msgid "Steps to ease tests of collective.contact.plonegroup"
 msgstr "Steps to ease tests of collective.contact.plonegroup"
 
-#: ../subscribers.py:136
+#: ../subscribers.py:147
 msgid "This contact is selected in configuration"
 msgstr "Ce contact est sélectionné dans la configuration"
 
-#: ../subscribers.py:142
+#: ../subscribers.py:153
 msgid "This contact is used in following content: ${items}"
 msgstr "Ce contact est utilisé dans le contenu suivant: ${items}"
 
-#: ../browser/settings.py:289
+#: ../browser/settings.py:300
 msgid "This organization or a contained organization is used in plonegroup configuration ! Remove it first from the configuration !"
 msgstr "Cette organisation ou une organisation contenue est utilisée dans la configuration de groupe plone via contact ! Il faut d'abord l'enlever de la configuration !"
 
-#: ../subscribers.py:148
+#: ../subscribers.py:159
 msgid "You cannot deactivate this item !"
 msgstr "Vous ne pouvez pas désactiver cet élément !"
 
-#: ../subscribers.py:189
+#: ../subscribers.py:200
 msgid "You cannot delete the group '${group}', linked to used organization '${orga}'."
 msgstr "Vous ne pouvez pas effacer le groupe '${group}', lié à l'organisation utilisée '${orga}'."
 
-#: ../browser/settings.py:288
+#: ../browser/settings.py:299
 msgid "You cannot delete this item !"
 msgstr "Vous ne pouvez pas effacer cet élément !"
 
-#: ../browser/settings.py:126
+#: ../browser/settings.py:134
 msgid "You must choose at least one organization !"
 msgstr "Vous devez au moins choisir une organisation !"
 
-#: ../browser/settings.py:128
+#: ../browser/settings.py:136
 msgid "You must correct the organization error first !"
 msgstr "Vous devez corriger l'erreur sur l'organisation !"
 
-#: ../browser/settings.py:86
+#: ../browser/settings.py:94
 msgid "You must define an organization with id '${pgo}' !"
 msgstr "Vous devez définir une organisation dont l'id est '${pgo}' !"
 
-#: ../browser/settings.py:130
+#: ../browser/settings.py:138
 msgid "You must define at least one function !"
 msgstr "Vous devez au moins choisir une fonction !"
 
-#: ../browser/settings.py:90
+#: ../browser/settings.py:98
 msgid "You must have only one organization with id '${pgo}' !"
 msgstr "Vous devez avoir une seule organisation avec l'id '${pgo}' !"
 
 #: ../configure.zcml:29
 msgid "collective.contact.plonegroup"
 msgstr "collective.contact.plonegroup"
 
 #: ../testing.zcml:16
 msgid "collective.contact.plonegroup tests"
 msgstr "collective.contact.plonegroup tests"
+
+#. Default: "For convenience, organizations are listed alphabetically. Order is defined in the ${plonegroup_config_url}."
+#: ../browser/templates/suborganizations.pt:5
+msgid "help_organizations_sorted_alphabetically"
+msgstr "Par facilité, les organisations sont listées ici par ordre alphabétique.  L'ordre est défini dans la ${plonegroup_config_url}."
```

### Comparing `collective.contact.plonegroup-1.8.1/src/collective/contact/plonegroup/browser/settings.py` & `collective.contact.plonegroup-1.9/src/collective/contact/plonegroup/browser/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import re
 
 from collective.contact.plonegroup import _
 from collective.contact.plonegroup.config import FUNCTIONS_REGISTRY
 from collective.contact.plonegroup.config import ORGANIZATIONS_REGISTRY
 from collective.contact.plonegroup.config import PLONEGROUP_ORG
 from collective.elephantvocabulary import wrap_vocabulary
 from collective.z3cform.datagridfield import DataGridFieldFactory
@@ -379,14 +380,25 @@
     """
         Returns a vocabulary of selected organizations
     """
     terms = [SimpleTerm(t[0], title=t[1]) for t in getSelectedOrganizations()]
     return SimpleVocabulary(terms)
 
 
+class SearchableSimpleVocabulary(SimpleVocabulary):
+
+    def search(self, query, limit=50):
+        # transform query in a regexp
+        regexp = u' '.join([u'{}.*'.format(p) for p in query.split(' ')])
+        regexp = re.compile(regexp, re.I)
+        return [
+            term for term in self._terms if re.search(regexp, term.title)
+        ]
+
+
 class SelectedOrganizationsElephantVocabulary(object):
     """ Vocabulary of selected plonegroup-organizations services. """
     implements(IVocabularyFactory)
 
     @ram.cache(voc_cache_key)
     def __call__(self, context):
         factory = getUtility(IVocabularyFactory, 'collective.contact.plonegroup.organization_services')
@@ -396,10 +408,11 @@
         ordered_terms = []
         for uid in registry[ORGANIZATIONS_REGISTRY]:
             if uid in terms:
                 ordered_terms.append(terms[uid])
                 del terms[uid]
         extra_uids = terms.keys()
         extra_terms = terms.values()
+        # ordered_vocab = SearchableSimpleVocabulary(ordered_terms + extra_terms)  # bug in widget, trac #15186
         ordered_vocab = SimpleVocabulary(ordered_terms + extra_terms)
         wrapped_vocab = wrap_vocabulary(ordered_vocab, hidden_terms=extra_uids)(context)
         return wrapped_vocab
```

### Comparing `collective.contact.plonegroup-1.8.1/docs/LICENSE.rst` & `collective.contact.plonegroup-1.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.contact.plonegroup-1.8.1/docs/LICENSE.GPL` & `collective.contact.plonegroup-1.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

