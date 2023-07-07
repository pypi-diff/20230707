# Comparing `tmp/design.plone.policy-5.0.3.tar.gz` & `tmp/design.plone.policy-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.policy-5.0.3.tar", last modified: Tue Jun 13 12:52:49 2023, max compression
+gzip compressed data, was "design.plone.policy-5.0.4.tar", last modified: Tue Jul  4 14:00:54 2023, max compression
```

## Comparing `design.plone.policy-5.0.3.tar` & `design.plone.policy-5.0.4.tar`

### file list

```diff
@@ -1,90 +1,83 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.886366 design.plone.policy-5.0.3/
--rw-r--r--   0 cekk       (501) staff       (20)     5447 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       73 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      585 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      670 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      139 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)    20651 2023-06-13 12:52:49.886753 design.plone.policy-5.0.3/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     9030 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/README.rst
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.868979 design.plone.policy-5.0.3/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7993 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)       31 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      367 2023-06-13 12:52:49.887373 design.plone.policy-5.0.3/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2887 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.863187 design.plone.policy-5.0.3/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.869273 design.plone.policy-5.0.3/src/design/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.871845 design.plone.policy-5.0.3/src/design/plone/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.875266 design.plone.policy-5.0.3/src/design/plone/policy/
--rw-r--r--   0 cekk       (501) staff       (20)      173 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.876644 design.plone.policy-5.0.3/src/design/plone/policy/browser/
--rw-r--r--   0 cekk       (501) staff       (20)      119 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)    19901 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/browser/config.py
--rw-r--r--   0 cekk       (501) staff       (20)      540 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     5622 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/browser/trasparenza.py
--rw-r--r--   0 cekk       (501) staff       (20)     1623 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      441 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.877985 design.plone.policy-5.0.3/src/design/plone/policy/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/design.plone.policy.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.864024 design.plone.policy-5.0.3/src/design/plone/policy/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.878687 design.plone.policy-5.0.3/src/design/plone/policy/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)       28 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.mo
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
--rw-r--r--   0 cekk       (501) staff       (20)     1748 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      494 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      273 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.864558 design.plone.policy-5.0.3/src/design/plone/policy/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.880369 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      584 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/actions.xml
--rw-r--r--   0 cekk       (501) staff       (20)      175 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      122 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)     1027 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)     1473 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      341 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.880654 design.plone.policy-5.0.3/src/design/plone/policy/profiles/to_1400/
--rw-r--r--   0 cekk       (501) staff       (20)      237 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/to_1400/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.881407 design.plone.policy-5.0.3/src/design/plone/policy/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      122 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      268 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/uninstall/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      311 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/rejectanonymous.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.881947 design.plone.policy-5.0.3/src/design/plone/policy/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.882840 design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      534 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      996 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/get.py
--rw-r--r--   0 cekk       (501) staff       (20)      288 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.883655 design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      519 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     3831 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/get.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.884602 design.plone.policy-5.0.3/src/design/plone/policy/restapi/twitter_feed/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/twitter_feed/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      513 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/twitter_feed/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     6581 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/twitter_feed/get.py
--rw-r--r--   0 cekk       (501) staff       (20)     2342 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/sensitive.py
--rw-r--r--   0 cekk       (501) staff       (20)     3306 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     5214 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.886142 design.plone.policy-5.0.3/src/design/plone/policy/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     4286 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/tests/test_bandi_search_filters_api.py
--rw-r--r--   0 cekk       (501) staff       (20)     4625 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/tests/test_initial_structure.py
--rw-r--r--   0 cekk       (501) staff       (20)     3864 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/tests/test_search_filters_api.py
--rw-r--r--   0 cekk       (501) staff       (20)     3720 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)    12447 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/upgrades.py
--rw-r--r--   0 cekk       (501) staff       (20)     5069 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/upgrades.zcml
--rw-r--r--   0 cekk       (501) staff       (20)    13290 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/utils.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.871405 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)    20651 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2938 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)       53 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       20 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      504 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)        7 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/top_level.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.275555 design.plone.policy-5.0.4/
+-rw-r--r--   0 lucabel    (501) staff       (20)     5589 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       73 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      585 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      670 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      139 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)    14258 2023-07-04 14:00:54.275680 design.plone.policy-5.0.4/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)     7466 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/README.rst
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.260834 design.plone.policy-5.0.4/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     7993 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       31 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/requirements.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      367 2023-07-04 14:00:54.276132 design.plone.policy-5.0.4/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2887 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.254667 design.plone.policy-5.0.4/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.261053 design.plone.policy-5.0.4/src/design/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.263870 design.plone.policy-5.0.4/src/design/plone/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.266863 design.plone.policy-5.0.4/src/design/plone/policy/
+-rw-r--r--   0 lucabel    (501) staff       (20)      173 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.268367 design.plone.policy-5.0.4/src/design/plone/policy/browser/
+-rw-r--r--   0 lucabel    (501) staff       (20)      119 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/browser/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    19901 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/browser/config.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      540 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/browser/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5622 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/browser/trasparenza.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1623 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      398 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/interfaces.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.269606 design.plone.policy-5.0.4/src/design/plone/policy/locales/
+-rw-r--r--   0 lucabel    (501) staff       (20)      611 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/locales/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/locales/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/locales/design.plone.policy.pot
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.255844 design.plone.policy-5.0.4/src/design/plone/policy/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.269892 design.plone.policy-5.0.4/src/design/plone/policy/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     1748 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      494 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/locales/update.sh
+-rw-r--r--   0 lucabel    (501) staff       (20)      273 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/permissions.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.256585 design.plone.policy-5.0.4/src/design/plone/policy/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.271376 design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)      584 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/actions.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      175 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      122 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/catalog.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1027 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/metadata.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1473 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/registry.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      341 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.271894 design.plone.policy-5.0.4/src/design/plone/policy/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      122 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      268 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/profiles/uninstall/registry.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      311 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/rejectanonymous.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.272333 design.plone.policy-5.0.4/src/design/plone/policy/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/restapi/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.273276 design.plone.policy-5.0.4/src/design/plone/policy/restapi/bandi_search_filters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      534 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      996 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/restapi/bandi_search_filters/get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      250 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/restapi/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.274050 design.plone.policy-5.0.4/src/design/plone/policy/restapi/search_filters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/restapi/search_filters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      519 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/restapi/search_filters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3831 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/restapi/search_filters/get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2342 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/sensitive.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3306 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/setuphandlers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5214 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.275373 design.plone.policy-5.0.4/src/design/plone/policy/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/tests/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4286 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/tests/test_bandi_search_filters_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4625 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/tests/test_initial_structure.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3864 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/tests/test_search_filters_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3720 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/tests/test_setup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    13543 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/upgrades.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5341 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/upgrades.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    13481 2023-07-04 14:00:53.000000 design.plone.policy-5.0.4/src/design/plone/policy/utils.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-07-04 14:00:54.263640 design.plone.policy-5.0.4/src/design.plone.policy.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)    14258 2023-07-04 14:00:54.000000 design.plone.policy-5.0.4/src/design.plone.policy.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)     2645 2023-07-04 14:00:54.000000 design.plone.policy-5.0.4/src/design.plone.policy.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-07-04 14:00:54.000000 design.plone.policy-5.0.4/src/design.plone.policy.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       40 2023-07-04 14:00:54.000000 design.plone.policy-5.0.4/src/design.plone.policy.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       20 2023-07-04 14:00:54.000000 design.plone.policy-5.0.4/src/design.plone.policy.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-07-04 14:00:54.000000 design.plone.policy-5.0.4/src/design.plone.policy.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      504 2023-07-04 14:00:54.000000 design.plone.policy-5.0.4/src/design.plone.policy.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        7 2023-07-04 14:00:54.000000 design.plone.policy-5.0.4/src/design.plone.policy.egg-info/top_level.txt
```

### Comparing `design.plone.policy-5.0.3/CHANGES.rst` & `design.plone.policy-5.0.4/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+5.0.4 (2023-07-04)
+------------------
+
+- Add "Credits" with href https://www.io-comune.it.
+  [lucabel]
+- Remove twitter feeds.
+  [folix-01]
+
+
 5.0.3 (2023-06-13)
 ------------------
 
 - Fix creation script: now set default blocks and blocks_layout.
   [cekk]
 - Upgrade-step to fix all contents with broken blocks_layout.
   [cekk]
```

### Comparing `design.plone.policy-5.0.3/DEVELOP.rst` & `design.plone.policy-5.0.4/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/LICENSE.GPL` & `design.plone.policy-5.0.4/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/LICENSE.rst` & `design.plone.policy-5.0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/README.rst` & `design.plone.policy-5.0.4/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     :target: https://pypi.org/project/design.plone.policy/
     :alt: Number of PyPI downloads
 
 .. image:: https://img.shields.io/pypi/l/design.plone.policy.svg
     :target: https://pypi.org/project/design.plone.policy/
     :alt: License
 
-.. image:: https://github.com/RedTurtle/design.plone.policy/actions/workflows/test.yml/badge.svg
+.. image:: https://github.com/RedTurtle/design.plone.policy/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/RedTurtle/design.plone.policy/actions
     :alt: Tests
 
 .. image:: https://coveralls.io/repos/github/RedTurtle/design.plone.policy/badge.svg?branch=main
     :target: https://coveralls.io/github/RedTurtle/design.plone.policy?branch=main
     :alt: Coverage
 
@@ -160,59 +160,14 @@
                 "filename": "example.pdf"
             }
         }
     }
 
 Se l'invio va a buon fine, viene tornata una risposta con `204`.
 
-@twitter-feed
--------------
-
-Endpoint per poter visualizzare una serie di tweet.
-
-Per poterla utilizzare, bisogna creare un'app su Twitter e impostare il token Bearer dentro al registry Plone nella entry *design.plone.policy.twitter_token*.
-
-Per fare la ricerca, utilizza l'endpoint `recent`_ che permette di visualizzare solo i tweet dell'ultima settimana.
-
-.. _recent: https://developer.twitter.com/en/docs/twitter-api/tweets/search/introduction
-
-Come parametri accetta i seguenti:
-
-- **authors**: una lista di username tra cui ricercare gli ultimi Tweet.
-- **max_results**: un numero tra 10 e 100.
-
-Esempio di chiamata::
-
-    > curl -i -X GET http://localhost:8080/Plone/@twitter-feed?authors=foo&authors=bar -H 'Accept: application/json' -H 'Content-Type: application/json'
-
-La risposta è una lista di tweet con le informazioni necessarie per essere renderizzati::
-
-    [
-        {
-            "author": {
-            "id": "12345678",
-            "name": "John Doe",
-            "profile_image_url": "https://pbs.twimg.com/profile_images/xxx/xxx_normal.jpg",
-            "username": "jdoe"
-            },
-            "id": "xxxxx",
-            "like_count": 1,
-            "reply_count": 0,
-            "retweet_count": 0,
-            "text": "stringa html"
-        },
-        ...
-    ]
-
-Il campo `text` contiene già eventuali link ad hashtag, menzioni e link esterni dentro ad un tag <a/>.
-
-**Per evitare troppe chiamate al servizio (c'è un limite di 500000 tweet al mese), c'è della cache: per ogni query
-i risultati rimangono in cache per mezz'ora.**
-
-
 Amministrazione trasparente
 ===========================
 
 La vista "crea_area_trasparenza" crea la struttura per l'area "Amministrazione Trasparente".
 Si può lanciare dalla root del sito.
```

### Comparing `design.plone.policy-5.0.3/docs/conf.py` & `design.plone.policy-5.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/setup.py` & `design.plone.policy-5.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.policy",
-    version="5.0.3",
+    version="5.0.4",
     description="Pacchetto per creare un sito Agid su Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/browser/config.py` & `design.plone.policy-5.0.4/src/design/plone/policy/browser/config.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/browser/configure.zcml` & `design.plone.policy-5.0.4/src/design/plone/policy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/browser/trasparenza.py` & `design.plone.policy-5.0.4/src/design/plone/policy/browser/trasparenza.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/configure.zcml` & `design.plone.policy-5.0.4/src/design/plone/policy/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/locales/README.rst` & `design.plone.policy-5.0.4/src/design/plone/policy/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/locales/update.py` & `design.plone.policy-5.0.4/src/design/plone/policy/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/actions.xml` & `design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/metadata.xml`

 * *Files 8% similar despite different names*

#### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>3100</version>
+  <version>3101</version>
   <dependencies>
     <dependency>profile-plone.restapi:default</dependency>
     <dependency>profile-design.plone.contenttypes:default</dependency>
     <dependency>profile-redturtle.volto:default</dependency>
     <dependency>profile-collective.volto.dropdownmenu:default</dependency>
     <dependency>profile-collective.volto.socialsettings:default</dependency>
     <dependency>profile-collective.volto.secondarymenu:default</dependency>
```

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/registry.xml` & `design.plone.policy-5.0.4/src/design/plone/policy/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml` & `design.plone.policy-5.0.4/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/get.py` & `design.plone.policy-5.0.4/src/design/plone/policy/restapi/bandi_search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/configure.zcml` & `design.plone.policy-5.0.4/src/design/plone/policy/restapi/search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/get.py` & `design.plone.policy-5.0.4/src/design/plone/policy/restapi/search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/sensitive.py` & `design.plone.policy-5.0.4/src/design/plone/policy/sensitive.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/setuphandlers.py` & `design.plone.policy-5.0.4/src/design/plone/policy/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/testing.py` & `design.plone.policy-5.0.4/src/design/plone/policy/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/tests/test_bandi_search_filters_api.py` & `design.plone.policy-5.0.4/src/design/plone/policy/tests/test_bandi_search_filters_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/tests/test_initial_structure.py` & `design.plone.policy-5.0.4/src/design/plone/policy/tests/test_initial_structure.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/tests/test_search_filters_api.py` & `design.plone.policy-5.0.4/src/design/plone/policy/tests/test_search_filters_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/tests/test_setup.py` & `design.plone.policy-5.0.4/src/design/plone/policy/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/upgrades.py` & `design.plone.policy-5.0.4/src/design/plone/policy/upgrades.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from collective.volto.blocksfield.field import BlocksField
 from copy import deepcopy
-from design.plone.policy.interfaces import IDesignPlonePolicySettings
 from design.plone.policy.setuphandlers import disable_searchable_types
 from design.plone.policy.setuphandlers import set_default_subsite_colors
 from design.plone.policy.utils import create_default_blocks
+from design.plone.policy.interfaces import IDesignPlonePolicySettings
 from plone import api
 from plone.app.upgrade.utils import installOrReinstallProduct
 from plone.dexterity.utils import iterSchemata
 from plone.registry.interfaces import IRegistry
 from plone.restapi.behaviors import IBlocks
 from Products.CMFPlone.interfaces import IFilterSchema
 from Products.CMFPlone.interfaces import ISelectableConstrainTypes
 from zope.component import getUtility
 from zope.schema import getFields
 
+
 import json
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_PROFILE = "profile-design.plone.policy:default"
@@ -360,7 +361,37 @@
         for i, path in enumerate(already_modified):
             logger.info(f"[{i+1}/{len(already_modified)}] - {path}")
 
     if not_modified:
         logger.info("### Items that were not modified ###")
         for i, path in enumerate(not_modified):
             logger.info(f"[{i+1}/{len(not_modified)}] - {path}")
+
+
+def to_3101(context):
+    def remove_twitter(blocks_orig):
+        blocks = deepcopy(blocks_orig)
+        for key, block in blocks.items():
+            if block.get("@type", "") == "twitter_posts":
+                del blocks[key]
+
+        return blocks
+
+    for brain in api.portal.get_tool("portal_catalog")():
+        item = aq_base(brain.getObject())
+        for schema in iterSchemata(item):
+            for name, field in getFields(schema).items():
+                if name == "blocks":
+                    item.blocks = remove_twitter(item.blocks)
+
+                elif isinstance(field, BlocksField):
+                    value = deepcopy(field.get(item))
+                    if not value:
+                        continue
+                    try:
+                        blocks = value.get("blocks", {})
+                    except AttributeError:
+                        logger.warning(
+                            "[BLOCK] - {} (not converted)".format(brain.getURL())
+                        )
+                    if blocks:
+                        item.blocks = remove_twitter(blocks)
```

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/upgrades.zcml` & `design.plone.policy-5.0.4/src/design/plone/policy/upgrades.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -177,8 +177,18 @@
       destination="3100"
       >
     <genericsetup:upgradeStep
         title="Fix default blocks on pages created with script"
         handler=".upgrades.to_3100"
         />
   </genericsetup:upgradeSteps>
+  <genericsetup:upgradeSteps
+      profile="design.plone.policy:default"
+      source="3100"
+      destination="3101"
+      >
+    <genericsetup:upgradeStep
+        title="Remove twitter blocks"
+        handler=".upgrades.to_3101"
+        />
+  </genericsetup:upgradeSteps>
 </configure>
```

### Comparing `design.plone.policy-5.0.3/src/design/plone/policy/utils.py` & `design.plone.policy-5.0.4/src/design/plone/policy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,14 +348,19 @@
                 "items": [
                     {
                         "title": "Media Policy",
                         "visible": True,
                         "href": f"/{obj.getId()}",
                     },
                     {"title": "Sitemap", "visible": True, "href": "/sitemap"},
+                    {
+                        "title": "Credits",
+                        "visible": True,
+                        "href": "https://www.io-comune.it/",
+                    },
                 ],
             }
         ]
     )
     api.portal.set_registry_record(
         "subfooter_configuration", payload, interface=ISubfooter
     )
```

### Comparing `design.plone.policy-5.0.3/src/design.plone.policy.egg-info/SOURCES.txt` & `design.plone.policy-5.0.4/src/design.plone.policy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -36,34 +36,29 @@
 src/design/plone/policy/browser/configure.zcml
 src/design/plone/policy/browser/trasparenza.py
 src/design/plone/policy/locales/README.rst
 src/design/plone/policy/locales/__init__.py
 src/design/plone/policy/locales/design.plone.policy.pot
 src/design/plone/policy/locales/update.py
 src/design/plone/policy/locales/update.sh
-src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.mo
 src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
 src/design/plone/policy/profiles/default/actions.xml
 src/design/plone/policy/profiles/default/browserlayer.xml
 src/design/plone/policy/profiles/default/catalog.xml
 src/design/plone/policy/profiles/default/metadata.xml
 src/design/plone/policy/profiles/default/registry.xml
 src/design/plone/policy/profiles/default/rolemap.xml
-src/design/plone/policy/profiles/to_1400/registry.xml
 src/design/plone/policy/profiles/uninstall/browserlayer.xml
 src/design/plone/policy/profiles/uninstall/registry.xml
 src/design/plone/policy/restapi/__init__.py
 src/design/plone/policy/restapi/configure.zcml
 src/design/plone/policy/restapi/bandi_search_filters/__init__.py
 src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
 src/design/plone/policy/restapi/bandi_search_filters/get.py
 src/design/plone/policy/restapi/search_filters/__init__.py
 src/design/plone/policy/restapi/search_filters/configure.zcml
 src/design/plone/policy/restapi/search_filters/get.py
-src/design/plone/policy/restapi/twitter_feed/__init__.py
-src/design/plone/policy/restapi/twitter_feed/configure.zcml
-src/design/plone/policy/restapi/twitter_feed/get.py
 src/design/plone/policy/tests/__init__.py
 src/design/plone/policy/tests/test_bandi_search_filters_api.py
 src/design/plone/policy/tests/test_initial_structure.py
 src/design/plone/policy/tests/test_search_filters_api.py
 src/design/plone/policy/tests/test_setup.py
```

