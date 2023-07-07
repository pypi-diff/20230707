# Comparing `tmp/cubicweb-bootstrap-1.9.0.tar.gz` & `tmp/cubicweb-bootstrap-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-bootstrap-1.9.0.tar", last modified: Thu Nov 24 02:18:45 2022, max compression
+gzip compressed data, was "cubicweb-bootstrap-2.0.0.tar", last modified: Fri Jul  7 12:54:11 2023, max compression
```

## Comparing `cubicweb-bootstrap-1.9.0.tar` & `cubicweb-bootstrap-2.0.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.452827 cubicweb-bootstrap-1.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      974 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      505 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      556 2022-11-24 02:18:45.448827 cubicweb-bootstrap-1.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       17 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.436827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/
--rw-rw-rw-   0 root         (0) root         (0)      974 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.436827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/ajax-loader.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/
--rw-rw-rw-   0 root         (0) root         (0)    26133 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap-theme.css
--rw-rw-rw-   0 root         (0) root         (0)    23358 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap-theme.min.css
--rw-rw-rw-   0 root         (0) root         (0)   122932 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap.min.css
--rw-rw-rw-   0 root         (0) root         (0)     8972 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.css
--rw-rw-rw-   0 root         (0) root         (0)     1364 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.cw_compat.css
--rw-rw-rw-   0 root         (0) root         (0)     2979 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.edition.js
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.js
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubicweb.form.css
--rw-rw-rw-   0 root         (0) root         (0)      109 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubicweb.tableview.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    20127 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0 root         (0) root         (0)   108738 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0 root         (0) root         (0)    45404 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)    23424 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0 root         (0) root         (0)    18028 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff2
--rw-rw-rw-   0 root         (0) root         (0)      308 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/go_next.png
--rw-rw-rw-   0 root         (0) root         (0)      265 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/go_prev.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/facet_selected.png
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/facet_unselected.png
--rw-rw-rw-   0 root         (0) root         (0)      243 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/table_down.png
--rw-rw-rw-   0 root         (0) root         (0)      254 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/table_sortable.png
--rw-rw-rw-   0 root         (0) root         (0)      247 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/table_up.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/js/
--rw-rw-rw-   0 root         (0) root         (0)    36817 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/js/bootstrap.min.js
--rw-rw-rw-   0 root         (0) root         (0)     9202 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/logo-cubicweb.svg
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/pen_icon.png
--rw-rw-rw-   0 root         (0) root         (0)       86 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/required.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1095 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     3070 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/uiprops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.448827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/
--rw-rw-rw-   0 root         (0) root         (0)     1515 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5687 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/basecomponents.py
--rw-rw-rw-   0 root         (0) root         (0)     2495 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/basetemplates.py
--rw-rw-rw-   0 root         (0) root         (0)     3391 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/baseviews.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)      450 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/component.py
--rw-rw-rw-   0 root         (0) root         (0)     1666 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/cwproperties.py
--rw-rw-rw-   0 root         (0) root         (0)     4705 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/editforms.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/facets.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formfields.py
--rw-rw-rw-   0 root         (0) root         (0)    11353 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formrenderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/htmlwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)     1623 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/ibreadcrumbs.py
--rw-rw-rw-   0 root         (0) root         (0)     7406 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/navigation.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/primary.py
--rw-rw-rw-   0 root         (0) root         (0)      962 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/reledit.py
--rw-rw-rw-   0 root         (0) root         (0)     2891 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/startup.py
--rw-rw-rw-   0 root         (0) root         (0)      678 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/tableview.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/tag.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.436827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/
--rw-r--r--   0 root         (0) root         (0)      556 2022-11-24 02:18:44.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2977 2022-11-24 02:18:45.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 02:18:44.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2022-11-24 02:18:45.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 02:18:44.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       37 2022-11-24 02:18:45.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-11-24 02:18:45.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.448827 cubicweb-bootstrap-1.9.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     4605 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      779 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     7382 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/dependencies.rst
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/header.rst
--rw-rw-rw-   0 root         (0) root         (0)      396 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      141 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/primary.rst
--rw-rw-rw-   0 root         (0) root         (0)      983 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/release_0.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      257 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/release_0.6.0.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-24 02:18:45.452827 cubicweb-bootstrap-1.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2557 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.448827 cubicweb-bootstrap-1.9.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.448827 cubicweb-bootstrap-1.9.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     2324 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/test/test_bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/test/unittest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.326726 cubicweb-bootstrap-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-07 12:54:11.322726 cubicweb-bootstrap-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.294725 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/
+-rw-rw-rw-   0 root         (0) root         (0)      890 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.302725 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/ajax-loader.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.302725 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/css/
+-rw-rw-rw-   0 root         (0) root         (0)    26133 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/css/bootstrap-theme.css
+-rw-rw-rw-   0 root         (0) root         (0)    23358 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/css/bootstrap-theme.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   122932 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/css/bootstrap.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     8972 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/cubes.bootstrap.css
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/cubes.bootstrap.cw_compat.css
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/cubes.bootstrap.edition.js
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/cubes.bootstrap.js
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/cubicweb.form.css
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/cubicweb.tableview.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.306725 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0 root         (0) root         (0)   108738 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45404 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    23424 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)    18028 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff2
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/go_next.png
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/go_prev.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.306725 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/img/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/img/facet_selected.png
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/img/facet_unselected.png
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/img/table_down.png
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/img/table_sortable.png
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/img/table_up.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.306725 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/js/
+-rw-rw-rw-   0 root         (0) root         (0)    36817 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/js/bootstrap.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/logo-cubicweb.svg
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/pen_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/required.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.310725 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.310725 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3096 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/uiprops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.318725 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5604 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/basecomponents.py
+-rw-rw-rw-   0 root         (0) root         (0)     2474 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/basetemplates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3343 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/baseviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     1660 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/cwproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)     4807 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/editforms.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/facets.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/formfields.py
+-rw-rw-rw-   0 root         (0) root         (0)    11614 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/formrenderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1517 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/formwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/htmlwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/ibreadcrumbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7472 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/navigation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4708 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/primary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/reledit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/startup.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/tableview.py
+-rw-rw-rw-   0 root         (0) root         (0)     2302 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.298725 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-07 12:54:11.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-07-07 12:54:11.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 12:54:11.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-07 12:54:11.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 12:54:11.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-07 12:54:11.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-07 12:54:11.000000 cubicweb-bootstrap-2.0.0/cubicweb_bootstrap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.322726 cubicweb-bootstrap-2.0.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     4605 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/doc/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/doc/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7387 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/doc/dependencies.rst
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/doc/header.rst
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/doc/primary.rst
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/doc/release_0.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/doc/release_0.6.0.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 12:54:11.326726 cubicweb-bootstrap-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.322726 cubicweb-bootstrap-2.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:54:11.322726 cubicweb-bootstrap-2.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     2319 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/test/test_bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/test/unittest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-07-07 12:53:42.000000 cubicweb-bootstrap-2.0.0/tox.ini
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/__init__.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 """cubicweb-bootstrap application package
 
 
 """
 import inspect
 
-import six
-
 from cubicweb.__pkginfo__ import numversion as cubicweb_version
 
 CW_323 = cubicweb_version[:2] >= (3, 23)
 CW_325 = cubicweb_version[:2] >= (3, 25)
 
 
 def monkeypatch_default_value(func, arg, value):
     # work on the underlying function object if func is a method, that's
     # where '__defaults__' is actually stored.
     if inspect.ismethod(func):
         func = func.__func__
-    if six.PY2:
-        getfullargspec = inspect.getargspec
-    else:
-        getfullargspec = inspect.getfullargspec
+    getfullargspec = inspect.getfullargspec
     argspec = getfullargspec(func)
     # ArgSpec.args contains regular and named parameters, only keep the latter
-    named_args = argspec.args[-len(argspec.defaults):]
+    named_args = argspec.args[-len(argspec.defaults) :]
     idx = named_args.index(arg)
     # generate and inject a new '__defaults__' tuple with the new default value
-    new_defaults = func.__defaults__[:idx] + (value,) + func.__defaults__[idx + 1:]
+    new_defaults = func.__defaults__[:idx] + (value,) + func.__defaults__[idx + 1 :]
     func.__defaults__ = new_defaults
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/__pkginfo__.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/__pkginfo__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # pylint: disable=W0622
 """cubicweb-bootstrap application packaging information"""
 
-modname = 'bootstrap'
-distname = 'cubicweb-bootstrap'
+modname = "bootstrap"
+distname = "cubicweb-bootstrap"
 
-numversion = (1, 9, 0)
-version = '.'.join(str(num) for num in numversion)
+numversion = (2, 0, 0)
+version = ".".join(str(num) for num in numversion)
 
-license = 'LGPL'
-author = 'LOGILAB S.A. (Paris, FRANCE)'
-author_email = 'contact@logilab.fr'
-description = ''
-web = 'https://forge.extranet.logilab.fr/cubicweb/cubes/%s' % distname
+license = "LGPL"
+author = "LOGILAB S.A. (Paris, FRANCE)"
+author_email = "contact@logilab.fr"
+description = ""
+web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
 
 __depends__ = {
-    'cubicweb': ">= 3.38.0, < 3.39.0",
-    'six': '>= 1.12.0',
+    "cubicweb": ">= 4.0.0, < 5.0.0",
+    "cubicweb-web": ">= 1.0.0, < 2.0.0",
 }
 __recommends__ = {}
 
 classifiers = [
-    'Environment :: Web Environment',
-    'Framework :: CubicWeb',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 2',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: JavaScript',
+    "Environment :: Web Environment",
+    "Framework :: CubicWeb",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 2",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: JavaScript",
 ]
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/ajax-loader.gif` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap-theme.css` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap-theme.min.css` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap.min.css` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.css` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/cubes.bootstrap.css`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.cw_compat.css` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/cubes.bootstrap.cw_compat.css`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.edition.js` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/cubes.bootstrap.edition.js`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.eot` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.svg` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.ttf` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff2` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/js/bootstrap.min.js` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/logo-cubicweb.svg` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/data/logo-cubicweb.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/migration/postcreate.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/migration/postcreate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# copyright 2013-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2013-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact https://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -18,9 +17,8 @@
 """cubicweb-bootstrap postcreate script, executed at instance creation time or when
 the cube is added to an existing instance.
 
 You could setup site properties or a workflow here for example.
 """
 
 # Example of site property change
-#set_property('ui.site-title', "<sitename>")
-
+# set_property('ui.site-title', "<sitename>")
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/site_cubicweb.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/site_cubicweb.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2013-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2013-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact https://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -25,57 +25,64 @@
 # put there monkeypatches of things that aren't reloaded automatically
 
 # monkeypatches #############################################################
 
 # keep the original `formwidgets.FieldWidget.attributes`
 orig_attributes = formwidgets.FieldWidget.attributes
 
-formwidgets.FieldWidget.css_class = 'form-control'
+formwidgets.FieldWidget.css_class = "form-control"
 
 # Keep the `validateButton` as it is used in js (e.g `unfreezeFormButtons`)
-formwidgets.ButtonInput.css_class = 'btn btn-default'
-formwidgets.Button.css_class = 'btn btn-default validateButton'
-formwidgets.SubmitButton.css_class = 'btn btn-primary validateButton'
+formwidgets.ButtonInput.css_class = "btn btn-default"
+formwidgets.Button.css_class = "btn btn-default validateButton"
+formwidgets.SubmitButton.css_class = "btn btn-primary validateButton"
 
 
 @monkeypatch(formwidgets.FieldWidget)
 def attributes(self, form, field):
-    """ add the bootstrap `form-control` class to formwidgets.FieldWidget.attributes method
-    """
+    """add the bootstrap `form-control` class to formwidgets.FieldWidget.attributes method"""
     attrs = orig_attributes(self, form, field)
     if self.css_class:
-        attrs['class'] = ' '.join((attrs.get('class', ''),
-                                   self.css_class)).strip()
+        attrs["class"] = " ".join((attrs.get("class", ""), self.css_class)).strip()
     return attrs
 
+
 # in bootstrap 3.0.0 CheckBox, RadioBox and FileInput must not have
 # form-control class
 
 
 formwidgets.CheckBox.attributes = orig_attributes
 formwidgets.FileInput.attributes = orig_attributes
 
 
 # Buttons
-stdmsgs.BUTTON_OK = (stdmsgs.BUTTON_OK[0], 'glyphicon glyphicon-ok')
-stdmsgs.BUTTON_APPLY = (stdmsgs.BUTTON_APPLY[0], 'glyphicon glyphicon-cog')
-stdmsgs.BUTTON_CANCEL = (stdmsgs.BUTTON_CANCEL[0], 'glyphicon glyphicon-remove')
-stdmsgs.BUTTON_DELETE = (stdmsgs.BUTTON_DELETE[0], 'glyphicon glyphicon-trash')
+stdmsgs.BUTTON_OK = (stdmsgs.BUTTON_OK[0], "glyphicon glyphicon-ok")
+stdmsgs.BUTTON_APPLY = (stdmsgs.BUTTON_APPLY[0], "glyphicon glyphicon-cog")
+stdmsgs.BUTTON_CANCEL = (stdmsgs.BUTTON_CANCEL[0], "glyphicon glyphicon-remove")
+stdmsgs.BUTTON_DELETE = (stdmsgs.BUTTON_DELETE[0], "glyphicon glyphicon-trash")
 
 
 # Override default form buttons to 'btn-class' and use bootstrap glyphicons.
 
 
-monkeypatch_default_value(formwidgets.Button.__init__, 'label',
-                          (stdmsgs.BUTTON_OK[0], 'glyphicon glyphicon-ok'))
+monkeypatch_default_value(
+    formwidgets.Button.__init__,
+    "label",
+    (stdmsgs.BUTTON_OK[0], "glyphicon glyphicon-ok"),
+)
 
 
 # options #############################################################
 
 options = (
-    ('cw_compatibility',
-     {'type': 'yn',
-      'default': False,
-      'help': 'use compat css rules (enable if your application uses views '
-      'that have not been ported to bootstrap)',
-      'group': 'bootstrap', 'level': 2}),
+    (
+        "cw_compatibility",
+        {
+            "type": "yn",
+            "default": False,
+            "help": "use compat css rules (enable if your application uses views "
+            "that have not been ported to bootstrap)",
+            "group": "bootstrap",
+            "level": 2,
+        },
+    ),
 )
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/uiprops.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/uiprops.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 :organization: Logilab
 :copyright: 2013-2022 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 # flake8: noqa
 
-STYLESHEETS = [data('css/bootstrap.min.css'),
-               data('cubes.bootstrap.css'),
-               data('cubicweb.pictograms.css'),
-               ]
-CW_COMPAT_STYLESHEETS = [data('cubes.bootstrap.cw_compat.css'),
-                         ]
+STYLESHEETS = [
+    data("css/bootstrap.min.css"),
+    data("cubes.bootstrap.css"),
+    data("cubicweb.pictograms.css"),
+]
+CW_COMPAT_STYLESHEETS = [
+    data("cubes.bootstrap.cw_compat.css"),
+]
 
-JAVASCRIPTS.extend((data('js/bootstrap.min.js'),
-                   data('cubes.bootstrap.js')))
+JAVASCRIPTS.extend((data("js/bootstrap.min.js"), data("cubes.bootstrap.js")))
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/__init__.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,52 +2,47 @@
 :organization: Logilab
 :copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 from logilab.common.decorators import monkeypatch
 
-from cubicweb import view as cwview
 from cubicweb.schema import display_name
+from cubicweb_web import view as cwview
 from cubicweb_web.views.basetemplates import HTMLHeader
 
 # do not wrap cell_calls with <div class="section">
 
 cwview.View.add_div_section = False
 
 
 @monkeypatch(cwview.View)
-def field(self, label, value, row=True, show_label=True, w=None, tr=True,
-          table=False):
+def field(self, label, value, row=True, show_label=True, w=None, tr=True, table=False):
     """read-only field"""
     if w is None:
         w = self.w
-    w(u'<tr>')
+    w("<tr>")
     if show_label and label:
         if tr:
             label = display_name(self._cw, label)
-        w(u'<th>%s</th>' % label)
+        w("<th>%s</th>" % label)
     if not (show_label and label):
-        w(u'<td colspan="2">%s</td>' % value)
+        w('<td colspan="2">%s</td>' % value)
     else:
-        w(u'<td>%s</td>' % value)
-    w(u'</tr>')
+        w("<td>%s</td>" % value)
+    w("</tr>")
 
 
 class BSHTMLHeader(HTMLHeader):
-
     def stylesheets(self):
-        super(BSHTMLHeader, self).stylesheets()
+        super().stylesheets()
         # add cw compatibility stylesheets
-        if self._cw.vreg.config['cw_compatibility']:
-            for css in self._cw.uiprops['CW_COMPAT_STYLESHEETS']:
+        if self._cw.vreg.config["cw_compatibility"]:
+            for css in self._cw.uiprops["CW_COMPAT_STYLESHEETS"]:
                 self._cw.add_css(css, localfile=False)
 
 
 def registration_callback(vreg):
-    components = (
-        (BSHTMLHeader, HTMLHeader),
-    )
-    vreg.register_all(globals().values(), __name__,
-                      [new for (new, old) in components])
+    components = ((BSHTMLHeader, HTMLHeader),)
+    vreg.register_all(globals().values(), __name__, [new for (new, old) in components])
     for new, old in components:
         vreg.register_and_replace(new, old)
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/basecomponents.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/basecomponents.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """bootstrap implementation of base components
 
 :organization: Logilab
 :copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
@@ -11,133 +10,162 @@
 from logilab.common.decorators import monkeypatch
 from logilab.mtconverter import xml_escape
 
 from cubicweb_web.views import basecomponents
 from cubicweb.uilib import js
 
 from cubicweb_bootstrap.views import utils
-from cubicweb_bootstrap import CW_325
 
 
 basecomponents.CookieLoginComponent._html = (
-    u'<a class="icon-login" data-toggle="modal" href="#loginModal">%s</a>')
+    '<a class="icon-login" data-toggle="modal" href="#loginModal">%s</a>'
+)
 
 
 @monkeypatch(basecomponents.CookieLoginComponent)
 def call(self):
-    self.w(self._html % self._cw._('i18n_login_popup'))
-    self._cw.add_onload(js.jQuery("body").append(
-        self._cw.view('logform', rset=self.cw_rset, id=self.loginboxid,
-                      klass='%s' % self.loginboxid, title=True,
-                      showmessage=False, showonload=False)))
-    self._cw.add_onload('''
+    self.w(self._html % self._cw._("i18n_login_popup"))
+    self._cw.add_onload(
+        js.jQuery("body").append(
+            self._cw.view(
+                "logform",
+                rset=self.cw_rset,
+                id=self.loginboxid,
+                klass=self.loginboxid,
+                title=True,
+                showmessage=False,
+                showonload=False,
+            )
+        )
+    )
+    self._cw.add_onload(
+        """
        $('#loginModal').on('shown.bs.modal', function () {
            $('#__login:visible').focus();
-       });''')
+       });"""
+    )
 
 
 # NOTE: CW 3.18 may introduce render_messages(). This would be the
 #       the only method to override
 @monkeypatch(basecomponents.ApplicationMessage)
 def call(self, msg=None):  # noqa: F811
     if msg is None:
         msg = self._cw.message  # XXX don't call self._cw.message twice
     if msg:
-        self.w(u'<div class="alert alert-info" id="%s">'
-               u'<button class="close" data-dismiss="alert" type="button">x</button>'
-               u' %s</div>' % (self.domid, msg))
+        self.w(
+            '<div class="alert alert-info" id="%s">'
+            '<button class="close" data-dismiss="alert" type="button">x</button>'
+            " %s</div>",
+            self.domid,
+            msg,
+            escape=False,
+        )
 
 
 @monkeypatch(basecomponents.ApplLogo)
 def render(self, w):
-    w(u'<a id="logo" href="%s"></a>' % self._cw.base_url())
+    w('<a id="logo" href="%s"></a>' % self._cw.base_url())
 
 
 @monkeypatch(basecomponents.ApplicationName)
 def render(self, w, **kwargs):  # noqa: F811
-    title = self._cw.property_value('ui.site-title')
+    title = self._cw.property_value("ui.site-title")
     if title:
-        w(u'<a class="cw-site-title" href="%s">%s</a>'
-          % (self._cw.base_url(), xml_escape(title)))
+        w(
+            '<a class="cw-site-title" href="%s">%s</a>'
+            % (self._cw.base_url(), xml_escape(title))
+        )
 
 
 class BSAuthenticatedUserStatus(basecomponents.AuthenticatedUserStatus):
-    divider_html = u'<li class="divider"></li>'
+    divider_html = '<li class="divider"></li>'
 
     def render(self, w):
         # display useractions and siteactions
-        actions = self._cw.vreg['actions'].possible_actions(
-            self._cw, rset=self.cw_rset, view=self.cw_extra_kwargs['view'])
+        actions = self._cw.vreg["actions"].possible_actions(
+            self._cw, rset=self.cw_rset, view=self.cw_extra_kwargs["view"]
+        )
         html = []
-        for action in actions.get('useractions', ()):
+        for action in actions.get("useractions", ()):
             self.render_actions(html.append, action)
-        if actions.get('useractions') and actions.get('siteactions'):
+        if actions.get("useractions") and actions.get("siteactions"):
             html.append(self.divider_html)
-        for action in actions.get('siteactions', ()):
+        for action in actions.get("siteactions", ()):
             self.render_actions(html.append, action)
-        ddb = AUSDropDownBox(self._cw.user.login, u'\n'.join(html), klass='icon-user')
+        ddb = AUSDropDownBox(self._cw.user.login, "\n".join(html), klass="icon-user")
         ddb.render(w=w)
 
     def render_actions(self, w, action):
-        w(u'<li>')
+        w("<li>")
         self.action_link(action).render(w=w)
-        w(u'</li>')
+        w("</li>")
 
 
 class AUSDropDownBox(utils.DropDownBox):
     def render(self, w):
         if not len(self.actions):
-            return u''
-        w(self.ul_template % {'title': self.title,
-                              'actions': self.actions,
-                              'klass': self.klass})
+            return ""
+        w(
+            self.ul_template
+            % {"title": self.title, "actions": self.actions, "klass": self.klass}
+        )
 
 
 class BSRQLInputForm(basecomponents.RQLInputForm):
     """build the rql input form, usually displayed in the header"""
-    __regid__ = 'rqlinput'
+
+    __regid__ = "rqlinput"
     cw_property_defs = basecomponents.VISIBLE_PROP_DEF
     visible = False
-    formdef = u"""<form id="rqlinput" action="%(action)s" class="%(css_class)s" role="search">
-    <input type="text" id="rql" name="rql" value="%(rql)s" placeholder="%(title)s" class="form-control"
-       title="%(title)s" tabindex="%(ind)s" accesskey="q" />
-    %(hidden)s</form>"""
+    formdef = """<form id="rqlinput" action="%s" class="%s" role="search">
+    <input type="text" id="rql" name="rql" value="%s" placeholder="%s" class="form-control"
+       title="%s" tabindex="%s" accesskey="q" />
+    %s</form>"""
 
     def call(self, view=None):
         req = self._cw
-        if hasattr(view, 'filter_box_context_info'):
+        if hasattr(view, "filter_box_context_info"):
             rset = view.filter_box_context_info()[0]
         else:
             rset = self.cw_rset
         # display multilines query as one line
-        rql = rset is not None and rset.printable_rql() or req.form.get('rql', '')
-        rql = rql.replace(u"\n", u" ")
-        rql_suggestion_comp = self._cw.vreg['components'].select_or_none('rql.suggestions', self._cw)
+        rql = rset is not None and rset.printable_rql() or req.form.get("rql", "")
+        rql = rql.replace("\n", " ")
+        rql_suggestion_comp = self._cw.vreg["components"].select_or_none(
+            "rql.suggestions", self._cw
+        )
         if rql_suggestion_comp is not None:
             # enable autocomplete feature only if the rql
             # suggestions builder is available
-            self._cw.add_css('jquery.ui.css')
-            self._cw.add_js(('cubicweb.ajax.js', 'jquery.ui.js'))
-            self._cw.add_onload('$("#rql").autocomplete({source: "%s"});'
-                                % (req.build_url('ajax', fname='rql_suggest')))
-        hidden = u''
-        if req.search_state[0] != 'normal':
-            hidden = u'<input type="hidden" name="__mode" value="%s"/>' % \
-                           ':'.join(req.search_state[1])
-        self.w(self.formdef % {'css_class': not self.cw_propval('visible') and 'hidden' or '',
-                               'action': req.build_url('view'),
-                               'rql': xml_escape(rql),
-                               'title': req._('full text or RQL query'),
-                               'ind': req.next_tabindex() if not CW_325 else u'',
-                               'hidden': hidden})
+            self._cw.add_css("jquery.ui.css")
+            self._cw.add_js(("cubicweb.ajax.js", "jquery.ui.js"))
+            self._cw.add_onload(
+                '$("#rql").autocomplete({source: "%s"});'
+                % (req.build_url("ajax", fname="rql_suggest"))
+            )
+        hidden = ""
+        if req.search_state[0] != "normal":
+            hidden = '<input type="hidden" name="__mode" value="%s"/>' % ":".join(
+                req.search_state[1]
+            )
+        self.w(
+            self.formdef,
+            req.build_url("view"),
+            not self.cw_propval("visible") and "hidden" or "",
+            rql,
+            req._("full text or RQL query"),
+            "",
+            "",
+            hidden,
+        )
 
 
 def registration_callback(vreg):
     components = (
         (BSAuthenticatedUserStatus, basecomponents.AuthenticatedUserStatus),
         (BSRQLInputForm, basecomponents.RQLInputForm),
-        )
-    vreg.register_all(globals().values(), __name__,
-                      [new for (new, old) in components])
+    )
+    vreg.register_all(globals().values(), __name__, [new for (new, old) in components])
     for new, old in components:
         vreg.register_and_replace(new, old)
     vreg.unregister(basecomponents.AnonUserStatusLink)
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/baseviews.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/baseviews.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,88 +4,91 @@
 :copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
-from six.moves import range
 
 from cubicweb_web.views import baseviews
 
-baseviews.ListView.listtag = 'ul'
+baseviews.ListView.listtag = "ul"
 
 
 @monkeypatch(baseviews.ListView)
-def call(self, klass='list-striped', title=None, subvid=None, listid=None, **kwargs):
+def call(self, klass="list-striped", title=None, subvid=None, listid=None, **kwargs):
     """display a list of entities by calling their <item_vid> view
 
     :param listid: the DOM id to use for the root element
     """
-    if subvid is None and 'subvid' in self._cw.form:
-        subvid = self._cw.form.pop('subvid')  # consume it
+    if subvid is None and "subvid" in self._cw.form:
+        subvid = self._cw.form.pop("subvid")  # consume it
     if listid:
-        listid = u' id="%s"' % listid
+        listid = ' id="%s"' % listid
     else:
-        listid = u''
+        listid = ""
     if title:
-        self.w(u'<div%s class="%s"><h4>%s</h4>\n' % (listid, klass or u'', title))
-        self.w(u'<%s class="%s">\n' % (self.listtag, klass or u''))
+        self.w('<div%s class="%s"><h4>%s</h4>\n', listid, klass or "", title)
+        self.w('<%s class="%s">\n', self.listtag, klass or "")
     else:
-        self.w(u'<%s%s class="%s">\n' % (self.listtag, listid, klass or u''))
+        self.w('<%s%s class="%s">\n', self.listtag, listid, klass or "")
     for i in range(self.cw_rset.rowcount):
         self.cell_call(row=i, col=0, vid=subvid, klass=klass, **kwargs)
-    self.w(u'</%s>\n' % self.listtag)
+    self.w("</%s>\n", self.listtag)
     if title:
-        self.w(u'</div>\n')
+        self.w("</div>\n")
 
 
 @monkeypatch(baseviews.ListView)
 def cell_call(self, row, col=0, vid=None, klass=None, **kwargs):
-    self.w(u'<li class="%s">' % (u'odd' if row % 2 else u'even'))
+    self.w('<li class="%s">', "odd" if row % 2 else "even")
     self.wview(self.item_vid, self.cw_rset, row=row, col=col, vid=vid, **kwargs)
-    self.w(u'</li>\n')
+    self.w("</li>\n")
 
 
 @monkeypatch(baseviews.SameETypeListView)
-def call(self, klass='list-striped', **kwargs):  # noqa: F811
-    w = self.w
-    showtitle = kwargs.pop('showtitle', 'vtitle' not in self._cw.form)
+def call(self, klass="list-striped", **kwargs):  # noqa: F811
+    showtitle = kwargs.pop("showtitle", "vtitle" not in self._cw.form)
     if showtitle:
-        w(u'<h1>%s</h1>' % self.title)
-    klass = u'' if klass is None else u' class="%s"' % klass
-    w(u'<ul%s>\n' % klass)
+        self.w("<h1>%s</h1>", self.title)
+    if klass:
+        self.w('<ul class="%s">\n', klass)
+    else:
+        self.w("<ul>\n")
     for i in range(len(self.cw_rset)):
-        w(u'<li class="%s">' % (u'odd' if i % 2 else u'even'))
-        self._cw.view(self.item_vid, self.cw_rset, row=i, col=0, w=w)
-        w(u'</li>')
-    w(u'</ul>\n')
+        self.w('<li class="%s">', "odd" if i % 2 else "even")
+        self._cw.view(self.item_vid, self.cw_rset, row=i, col=0, w=self.w)
+        self.w("</li>")
+    self.w("</ul>\n")
 
 
 @monkeypatch(baseviews.MetaDataView)
 def cell_call(self, row, col):  # noqa: F811
     _ = self._cw._
     entity = self.cw_rset.get_entity(row, col)
-    self.w(u'<p class="text-right"><small>')
+    self.w('<p class="text-right"><small>')
     if self.show_eid:
-        self.w(u'%s #%s - ' % (entity.dc_type(), entity.eid))
+        self.w("%s #%s - ", entity.dc_type(), entity.eid)
     if entity.modification_date != entity.creation_date:
-        self.w(u'<span>%s</span> ' % _('latest update on'))
-        self.w(u'<span class="value">%s</span>, '
-               % self._cw.format_date(entity.modification_date))
+        self.w("<span>%s</span> ", _("latest update on"))
+        self.w(
+            '<span class="value">%s</span>, ',
+            self._cw.format_date(entity.modification_date),
+        )
     # entities from external source may not have a creation date (eg ldap)
     if entity.creation_date:
-        self.w(u'<span>%s</span> ' % _('created on'))
-        self.w(u'<span class="value">%s</span>'
-               % self._cw.format_date(entity.creation_date))
+        self.w("<span>%s</span> ", _("created on"))
+        self.w(
+            '<span class="value">%s</span>', self._cw.format_date(entity.creation_date)
+        )
     if entity.creator:
         if entity.creation_date:
-            self.w(u' <span>%s</span> ' % _('by'))
+            self.w(" <span>%s</span> ", _("by"))
         else:
-            self.w(u' <span>%s</span> ' % _('created_by'))
-        self.w(u'<span class="value">%s</span>' % entity.creator.name())
+            self.w(" <span>%s</span> ", _("created_by"))
+        self.w('<span class="value">%s</span>', entity.creator.name())
     if entity.cw_source:
         source = entity.cw_source[0]
-        if source.name != 'system':
-            self.w(u' (<span>%s</span>' % _('cw_source'))
-            self.w(u' <span class="value">%s</span>)' % source.name)
-    self.w(u'</small></p>')
+        if source.name != "system":
+            self.w(" (<span>%s</span>", _("cw_source"))
+            self.w(' <span class="value">%s</span>)', source.name)
+    self.w("</small></p>")
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/boxes.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/boxes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """bootstrap implementation of boxes
 
 :organization: Logilab
 :copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
@@ -13,44 +12,52 @@
 
 from cubicweb.utils import wrap_on_write
 from cubicweb_web.views import boxes
 
 from cubicweb_bootstrap import CW_325
 
 boxes.SearchBox.formdef = (
-    u'<form action="%(action)s" id="search_box" class="navbar-form" role="search">\n'
-    u'  <input id="norql" type="text" accesskey="q" tabindex="%(tabindex1)s"'
-    u'    title="search text" value="%(value)s" name="rql"'
-    u'    class="search-query form-control" placeholder="%(searchlabel)s"/>\n'
-    u'  <input type="hidden" name="__fromsearchbox" value="1" />\n'
-    u'  <input type="hidden" name="subvid" value="tsearch" />\n'
-    u'</form>\n')
+    '<form action="%(action)s" id="search_box" class="navbar-form" role="search">\n'
+    '  <input id="norql" type="text" accesskey="q" tabindex="%(tabindex1)s"'
+    '    title="search text" value="%(value)s" name="rql"'
+    '    class="search-query form-control" placeholder="%(searchlabel)s"/>\n'
+    '  <input type="hidden" name="__fromsearchbox" value="1" />\n'
+    '  <input type="hidden" name="subvid" value="tsearch" />\n'
+    "</form>\n"
+)
 
 
 @monkeypatch(boxes.SearchBox)
 def render_body(self, w):
     # Don't display search box title, just display the search box body
-    if self._cw.form.pop('__fromsearchbox', None):
-        rql = self._cw.form.get('rql', '')
+    if self._cw.form.pop("__fromsearchbox", None):
+        rql = self._cw.form.get("rql", "")
     else:
-        rql = ''
-    w(self.formdef % {'action': self._cw.build_url('view'),
-                      'tabindex1': self._cw.next_tabindex() if not CW_325 else u'',
-                      'value': xml_escape(rql),
-                      'searchlabel': self._cw._('Search')})
+        rql = ""
+    w(
+        self.formdef
+        % {
+            "action": self._cw.build_url("view"),
+            "tabindex1": self._cw.next_tabindex() if not CW_325 else "",
+            "value": xml_escape(rql),
+            "searchlabel": self._cw._("Search"),
+        }
+    )
 
 
 @monkeypatch(boxes.ContextualBoxLayout)
 def render(self, w):
     if self.init_rendering():
-        view = self.cw_extra_kwargs['view']
-        w(u'<div class="panel panel-default %s %s" id="%s">' % (self.cssclass, view.cssclass,
-                                                                view.domid))
-        with wrap_on_write(w,
-                           u'<div class="panel-heading"><div class="panel-title">',
-                           u'</div></div>') as wow:
+        view = self.cw_extra_kwargs["view"]
+        w(
+            '<div class="panel panel-default %s %s" id="%s">'
+            % (self.cssclass, view.cssclass, view.domid)
+        )
+        with wrap_on_write(
+            w, '<div class="panel-heading"><div class="panel-title">', "</div></div>"
+        ) as wow:
             view.render_title(wow)
-        w(u'<div class="panel-body">')
+        w('<div class="panel-body">')
         view.render_body(w)
         # We dissapear the boxFooter CSS place holder, as shadows
         # or effect will be made with CSS
-        w(u'</div></div>\n')
+        w("</div></div>\n")
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/cwproperties.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/cwproperties.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,42 +4,45 @@
 :copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
-from cubicweb_web.views.cwproperties import (
-    SystemCWPropertiesForm, make_togglable_link
-)
+from cubicweb_web.views.cwproperties import SystemCWPropertiesForm, make_togglable_link
 
 
 @monkeypatch(SystemCWPropertiesForm)
 def wrap_main_form(self, group, label, form):
-    label += u' <span class="caret"></span>'
+    label += ' <span class="caret"></span>'
     status = self._group_status(group)
-    cssclass = 'panel-body %s' % status if status else 'panel-body'
-    self.w(u'<div class="panel panel-default">'
-           u'<div class="panel-heading">%s</div>\n' %
-           (make_togglable_link('fieldset_' + group, label)))
-    self.w(u'<div class="%s" id="fieldset_%s">' % (cssclass, group))
+    cssclass = "panel-body %s" % status if status else "panel-body"
+    self.w(
+        '<div class="panel panel-default">' '<div class="panel-heading">%s</div>\n',
+        make_togglable_link("fieldset_" + group, label),
+        escape=False,
+    )
+    self.w('<div class="%s" id="fieldset_%s">', cssclass, group)
     self.w(form)
-    self.w(u'</div>')
-    self.w(u'</div>')
+    self.w("</div>")
+    self.w("</div>")
 
 
 @monkeypatch(SystemCWPropertiesForm)
 def wrap_grouped_form(self, group, label, objects):
-    label += u' <span class="caret"></span>'
+    label += ' <span class="caret"></span>'
     status = self._group_status(group)
-    cssclass = 'panel-body %s' % status if status else 'panel-body'
-    self.w(u'<div class="panel panel-default">'
-           u'<div class="panel-heading">%s</div>\n' %
-           (make_togglable_link('fieldset_' + group, label)))
-    self.w(u'<div class="%s" id="fieldset_%s">' % (cssclass, group))
-
-    sorted_objects = sorted((self._cw.__('%s_%s' % (group, o)), o, f)
-                            for o, f in objects.items())
+    cssclass = "panel-body %s" % status if status else "panel-body"
+    self.w(
+        '<div class="panel panel-default">' '<div class="panel-heading">%s</div>\n',
+        make_togglable_link("fieldset_" + group, label),
+        escape=False,
+    )
+    self.w('<div class="%s" id="fieldset_%s">', cssclass, group)
+
+    sorted_objects = sorted(
+        (self._cw.__(f"{group}_{o}"), o, f) for o, f in objects.items()
+    )
     for label, oid, form in sorted_objects:
         self.wrap_object_form(group, oid, label, form)
-    self.w(u'</div>')
-    self.w(u'</div>')
+    self.w("</div>")
+    self.w("</div>")
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/editforms.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/editforms.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,35 +11,44 @@
 from cubicweb_web.views import editforms
 
 
 @monkeypatch(editforms.EditionFormView)
 def form_title(self, entity):
     """the form view title"""
     ptitle = self._cw._(self.title)
-    self.w(u'<div class="formTitle"><h1>%s %s</h1></div>' % (
-        entity.dc_type(), ptitle and '(%s)' % ptitle))
+    self.w(
+        '<div class="formTitle"><h1>%s %s</h1></div>',
+        entity.dc_type(),
+        ptitle and "(%s)" % ptitle,
+    )
 
 
 @monkeypatch(editforms.CreationFormView)
 def form_title(self, entity):  # noqa: F811
     """the form view title"""
-    if '__linkto' in self._cw.form:
-        if isinstance(self._cw.form['__linkto'], list):
+    if "__linkto" in self._cw.form:
+        if isinstance(self._cw.form["__linkto"], list):
             # XXX which one should be considered (case: add a ticket to a
             # version in jpl)
-            rtype, linkto_eid, role = self._cw.form['__linkto'][0].split(':')
+            rtype, linkto_eid, role = self._cw.form["__linkto"][0].split(":")
         else:
-            rtype, linkto_eid, role = self._cw.form['__linkto'].split(':')
+            rtype, linkto_eid, role = self._cw.form["__linkto"].split(":")
         linkto_rset = self._cw.eid_rset(linkto_eid)
         linkto_type = linkto_rset.description[0][0]
-        if role == 'subject':
-            title = self._cw.__('creating %s (%s %s %s %%(linkto)s)' % (
-                entity.e_schema, entity.e_schema, rtype, linkto_type))
+        if role == "subject":
+            title = self._cw.__(
+                "creating %s (%s %s %s %%(linkto)s)"
+                % (entity.e_schema, entity.e_schema, rtype, linkto_type)
+            )
         else:
-            title = self._cw.__('creating %s (%s %%(linkto)s %s %s)' % (
-                entity.e_schema, linkto_type, rtype, entity.e_schema))
-        msg = title % {'linkto': self._cw.view('incontext', linkto_rset)}
+            title = self._cw.__(
+                "creating %s (%s %%(linkto)s %s %s)"
+                % (entity.e_schema, linkto_type, rtype, entity.e_schema)
+            )
+        msg = title % {"linkto": self._cw.view("incontext", linkto_rset)}
         # bs customization begins
-        self.w(u'<div class="formTitle notransform"><h1>%s</h1></div>' % msg)
+        self.w(
+            '<div class="formTitle notransform"><h1>%s</h1></div>', msg, escape=False
+        )
         # bs customization ends
     else:
         super(editforms.CreationFormView, self).form_title(entity)
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formfields.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/formfields.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from cubicweb_web import formfields
 
 
 @monkeypatch(formfields.FileField)
 def render_subfield(self, form, field, renderer):
     data = UStringIO()  # XXX add support for tracewrites
     w = data.write
-    w(u'<div class="row">')
+    w('<div class="row">')
     w(renderer.render_label(form, field))
-    w(u'<div class="col-md-9">')
+    w('<div class="col-md-9">')
     w(field.render(form, renderer))
-    w(u'</div>')
-    w(u'</div>')
-    w(u'<div class="row">')
-    w(u'<div class="col-md-offset-3 col-md-9">')
+    w("</div>")
+    w("</div>")
+    w('<div class="row">')
+    w('<div class="col-md-offset-3 col-md-9">')
     w(renderer.render_help(form, field))
-    w(u'</div>')
-    w(u'</div>')
+    w("</div>")
+    w("</div>")
     return data.getvalue()
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formrenderers.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/formrenderers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2013-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2013-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact https://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -16,239 +16,265 @@
 """bootstrap implementation of formrenderers"""
 
 __docformat__ = "restructuredtext en"
 
 from warnings import warn
 
 from logilab.common.decorators import monkeypatch
+from logilab.mtconverter import xml_escape
 
 from cubicweb import tags
 from cubicweb.utils import support_args
 from cubicweb_web.views import formrenderers
 
 
 @monkeypatch(formrenderers.EntityCompositeFormRenderer)
 def render_fields(self, w, form, values):
     if form.parent_form is None:
         # We should probably take those CSS classes to uiprops.py
-        w(u'<table class="table table-striped table-bordered table-condensed">')
+        w('<table class="table table-striped table-bordered table-condensed">')
         # get fields from the first subform with something to display (we
         # may have subforms with nothing editable that will simply be
         # skipped later)
         for subform in form.forms:
-            subfields = [field for field in subform.fields
-                         if field.is_visible()]
+            subfields = [field for field in subform.fields if field.is_visible()]
             if subfields:
                 break
         if subfields:
             # main form, display table headers HTML5
-            w(u'<thead>')
-            w(u'<tr>')
-            w(u'<th>%s</th>' %
-              tags.input(type='checkbox',
-                         title=self._cw._('toggle check boxes'),
-                         onclick="setCheckboxesState('eid', null, this.checked)"))
+            w("<thead>")
+            w("<tr>")
+            w(
+                "<th>%s</th>"
+                % tags.input(
+                    type="checkbox",
+                    title=self._cw._("toggle check boxes"),
+                    onclick="setCheckboxesState('eid', null, this.checked)",
+                )
+            )
             for field in subfields:
-                w(u'<th>%s</th>' % formrenderers.field_label(form, field))
-            w(u'</tr>')
-            w(u'</thead>')
-    super(formrenderers.EntityCompositeFormRenderer, self).render_fields(w, form, values)
+                w("<th>%s</th>" % formrenderers.field_label(form, field))
+            w("</tr>")
+            w("</thead>")
+    super(formrenderers.EntityCompositeFormRenderer, self).render_fields(
+        w, form, values
+    )
     if form.parent_form is None:
-        w(u'</table>')
+        w("</table>")
         if self._main_display_fields:
             super(formrenderers.EntityCompositeFormRenderer, self)._render_fields(
-                self._main_display_fields, w, form)
+                self._main_display_fields, w, form
+            )
 
 
-formrenderers.FormRenderer.button_bar_class = u'form-group'
+formrenderers.FormRenderer.button_bar_class = "form-group"
 
 
 class ModalFormRenderer(formrenderers.FormRenderer):
-    __regid__ = 'modal-form-renderer'
-    button_bar_class = 'modal-footer'
+    __regid__ = "modal-form-renderer"
+    button_bar_class = "modal-footer"
 
     def open_form(self, form, values, **attrs):
-        showmessage = values.get('showmessage')
-        showonload = values.get('showonload', False)
+        showmessage = values.get("showmessage")
+        showonload = values.get("showonload", False)
         if showonload:
             # show the `modal` dialog : initialized in
             # basecomponents.CookieLoginComponent by showonload=True
-            self._cw.add_onload("$('#%s').modal('show')" % values['modal_id'])
-            data_backdrop, data_keyboard = u'static', u'false'
+            self._cw.add_onload("$('#%s').modal('show')" % values["modal_id"])
+            data_backdrop, data_keyboard = "static", "false"
         else:
-            data_backdrop, data_keyboard = u'true', u'true'
+            data_backdrop, data_keyboard = "true", "true"
 
-        html = [u'<div class="%(class)s" id="%(id)s" tabindex="-1" role="dialog" '
-                u'data-backdrop="%(backdrop)s" data-keyboard="%(keyboard)s">\n'
-                u'<div class="modal-dialog">'
-                u'<div class="modal-content">' % {
-                    'id': values['modal_id'],
-                    'class': u'modal fade in' if showmessage else u'modal',
-                    'backdrop': data_backdrop, 'keyboard': data_keyboard}]
-        html.append(super(ModalFormRenderer, self).open_form(form, values, **attrs))
-        html.append(u'<div class="modal-header">')
+        html = [
+            '<div class="%(class)s" id="%(id)s" tabindex="-1" role="dialog" '
+            'data-backdrop="%(backdrop)s" data-keyboard="%(keyboard)s">\n'
+            '<div class="modal-dialog">'
+            '<div class="modal-content">'
+            % {
+                "id": values["modal_id"],
+                "class": "modal fade in" if showmessage else "modal",
+                "backdrop": data_backdrop,
+                "keyboard": data_keyboard,
+            }
+        ]
+        html.append(super().open_form(form, values, **attrs))
+        html.append('<div class="modal-header">')
         if not showonload:
             # add cancel button when modal triggered by CookieLoginComponent
-            html.append(u'<button type="button" class="close" data-dismiss="modal" '
-                        'aria-hidden="true">&#215;</button>')
+            html.append(
+                '<button type="button" class="close" data-dismiss="modal" '
+                'aria-hidden="true">&#215;</button>'
+            )
         html.append(
-            u'<div class="modal-title">%s</div>\n</div>\n' % values.get('title', u''))
-        return u'\n'.join(html)
+            '<div class="modal-title">%s</div>\n</div>\n'
+            % xml_escape(values.get("title", ""))
+        )
+        return "\n".join(html)
 
     def render_content(self, w, form, values):
-        self._cw.add_onload("$('.close').click(function () {$(this).parent().removeClass('in');});")
-        w(u'<div class="modal-body">')
-        if values.get('showmessage'):
+        self._cw.add_onload(
+            "$('.close').click(function () {$(this).parent().removeClass('in');});"
+        )
+        w('<div class="modal-body">')
+        if values.get("showmessage"):
             message = self._cw.message
             if message:
-                w(u'<div class="alert alert-danger in">%s'
-                  u'<button class="close" data-dismiss="alert">x</button></div>' % message)
+                w(
+                    '<div class="alert alert-danger in">%s'
+                    '<button class="close" data-dismiss="alert">x</button></div>'
+                    % xml_escape(message)
+                )
         if self.display_progress_div:
-            w(u'<div id="progress">%s</div>' % self._cw._('validating...'))
-        w(u'\n<fieldset>\n')
+            w('<div id="progress">%s</div>' % self._cw._("validating..."))
+        w("\n<fieldset>\n")
         self.render_fields(w, form, values)
-        w(u'\n</fieldset>\n')
-        w(u'</div>')
+        w("\n</fieldset>\n")
+        w("</div>")
         self.render_buttons(w, form)
 
     def close_form(self, form, values):
-        html = [super(ModalFormRenderer, self).close_form(form, values)]
-        html.append('</div></div></div>')  # close modal-content, modal-dialog, ...
-        return u'\n'.join(html)
+        html = [super().close_form(form, values)]
+        html.append("</div></div></div>")  # close modal-content, modal-dialog, ...
+        return "\n".join(html)
 
 
 @monkeypatch(formrenderers.FormRenderer)
 def render_help(self, form, field):
-    """display help in the form
-    """
+    """display help in the form"""
     help = []
     descr = field.help
     if callable(descr):
-        if support_args(descr, 'form', 'field'):
+        if support_args(descr, "form", "field"):
             descr = descr(form, field)
         else:
-            warn("[3.10] field's help callback must now take form "
-                 "and field as argument (%s)" % field, DeprecationWarning)
+            warn(
+                "[3.10] field's help callback must now take form "
+                "and field as argument (%s)" % field,
+                DeprecationWarning,
+            )
             descr = descr(form)
     if descr:
         help.append('<p class="help-block">%s</p>' % self._cw._(descr))
     example = field.example_format(self._cw)
     if example:
-        help.append('<p class="form-control-static">(%s: %s)</p>'
-                    % (self._cw._('sample format'), example))
-    return u'&#160;'.join(help)
+        help.append(
+            '<p class="form-control-static">(%s: %s)</p>'
+            % (self._cw._("sample format"), example)
+        )
+    return "&#160;".join(help)
 
 
 @monkeypatch(formrenderers.FormRenderer)
 def error_message(self, form):
     """return formatted error message
 
     This method should be called once inlined field errors has been consumed
     """
     req = self._cw
     errex = form.form_valerror
     # get extra errors
     if errex is not None:
-        errormsg = req._('please correct the following errors:')
+        errormsg = req._("please correct the following errors:")
         errors = form.remaining_errors()
         if errors:
             if len(errors) > 1:
-                templstr = u'<li>%s</li>'
+                templstr = "<li>%s</li>"
             else:
-                templstr = u'&#160;%s'
+                templstr = "&#160;%s"
             for field, err in errors:
                 if field is None:
                     errormsg += templstr % err
                 else:
-                    errormsg += templstr % '%s: %s' % (req._(field), err)
+                    errormsg += templstr % "%s: %s" % (req._(field), err)
             if len(errors) > 1:
-                errormsg = '<ul>%s</ul>' % errormsg
-        return u'<div class="alert alert-danger">%s</div>' % errormsg
-    return u''
+                errormsg = "<ul>%s</ul>" % errormsg
+        return '<div class="alert alert-danger">%s</div>' % errormsg
+    return ""
 
 
 @monkeypatch(formrenderers.FormRenderer)
 def _render_fields(self, fields, w, form):
-    """render form fields
-    """
+    """render form fields"""
     byfieldset = {}
     for field in fields:
         byfieldset.setdefault(field.fieldset, []).append(field)
     if form.fieldsets_in_order:
         fieldsets = form.fieldsets_in_order
     else:
         fieldsets = byfieldset
     for fieldset in list(fieldsets):
         try:
             fields = byfieldset.pop(fieldset)
         except KeyError:
-            self.warning('no such fieldset: %s (%s)', fieldset, form)
+            self.warning("no such fieldset: %s (%s)", fieldset, form)
             continue
-        w(u'<fieldset>\n')
+        w("<fieldset>\n")
         if fieldset:
-            w(u'<legend>%s</legend>' % self._cw.__(fieldset))
+            w("<legend>%s</legend>" % self._cw.__(fieldset))
         for field in fields:
             error = form.field_error(field)
-            control = not hasattr(field, 'control_field') or field.control_field
-            w(u'<div id="%s-%s_row" class="form-group %s">' % (
-                field.name, field.role, 'error' if error else ''))
+            control = not hasattr(field, "control_field") or field.control_field
+            w(
+                '<div id="%s-%s_row" class="form-group %s">'
+                % (field.name, field.role, "error" if error else "")
+            )
             if self.display_label and field.label is not None:
-                w(u'%s' % self.render_label(form, field))
+                w("%s" % self.render_label(form, field))
             # Use full width for inlined forms, 9/12 for normal fields
-            base_css = 'col-md-12' if hasattr(field, 'view') else 'col-md-9'
+            base_css = "col-md-12" if hasattr(field, "view") else "col-md-9"
             if not control:
                 # katia : 'control' class no longer exists in bootstrap 3.0.0
                 # but is used here because of
                 # 'form-horizontal' bootstrap 2.0.4 css
                 # backport
-                base_css += ' nomargin'
-            w(u'<div class="%s">' % base_css)
+                base_css += " nomargin"
+            w('<div class="%s">' % base_css)
             w(field.render(form, self))
             if error:
                 self.render_error(w, error)
             if self.display_help:
                 w(self.render_help(form, field))
-            w(u'</div>')
-            w(u'</div>')
-        w(u'</fieldset>')
+            w("</div>")
+            w("</div>")
+        w("</fieldset>")
     if byfieldset:
-        self.warning('unused fieldsets: %s', ', '.join(byfieldset))
+        self.warning("unused fieldsets: %s", ", ".join(byfieldset))
 
 
 @monkeypatch(formrenderers.FormRenderer)
 def render_label(self, form, field):
     if field.label is None:
-        return u''
+        return ""
     label = formrenderers.field_label(form, field)
-    attrs = {'for': field.dom_id(form)}
-    attrs['class'] = 'col-md-3 control-label'
+    attrs = {"for": field.dom_id(form)}
+    attrs["class"] = "col-md-3 control-label"
     if field.required:
-        attrs['class'] += ' required'
+        attrs["class"] += " required"
     return tags.label(label, **attrs)
 
 
 @monkeypatch(formrenderers.FormRenderer)
 def render_buttons(self, w, form):
-    """render form's buttons
-    """
+    """render form's buttons"""
     if not form.form_buttons:
         return
-    w(u'<div class="%s">' % self.button_bar_class)
+    w('<div class="%s">' % self.button_bar_class)
     for button in form.form_buttons:
         w(button.render(form))
-    w(u'</div>')
+    w("</div>")
 
 
 @monkeypatch(formrenderers.EntityFormRenderer)
 def open_form(self, form, values):
-    attrs_fs_label = u''
+    attrs_fs_label = ""
     if self.main_form_title:
-        attrs_fs_label = u'<h3>%s</h3>' % self._cw._(self.main_form_title)
-    open_form = attrs_fs_label + super(formrenderers.EntityFormRenderer,
-                                       self).open_form(form, values)
+        attrs_fs_label = "<h3>%s</h3>" % self._cw._(self.main_form_title)
+    open_form = attrs_fs_label + super(
+        formrenderers.EntityFormRenderer, self
+    ).open_form(form, values)
     return open_form
 
 
 @monkeypatch(formrenderers.EntityFormRenderer)
 def close_form(self, form, values):
     # needed to remove the '</div>' from the original method
     return super(formrenderers.EntityFormRenderer, self).close_form(form, values)
@@ -260,30 +286,32 @@
     # doesn't need to add a special case when there are 3 buttons to render
     super(formrenderers.EntityFormRenderer, self).render_buttons(w, form)
 
 
 @monkeypatch(formrenderers.EntityInlinedFormRenderer)
 def open_form(self, w, form, values):  # noqa: F811
     try:
-        w(u'<div id="div-%(divid)s" onclick="%(divonclick)s">' % values)
+        w('<div id="div-%(divid)s" onclick="%(divonclick)s">' % values)
     except KeyError:
-        w(u'<div id="div-%(divid)s">' % values)
+        w('<div id="div-%(divid)s">' % values)
     else:
-        w(u'<div id="notice-%s" class="notice text-info">'
-          u'<span class="glyphicon glyphicon-info-sign"></span> %s</div>' % (
-              values['divid'], self._cw._('click on the box to cancel the deletion')))
-    w(u'<div class="iformBody">')
+        w(
+            '<div id="notice-%s" class="notice text-info">'
+            '<span class="glyphicon glyphicon-info-sign"></span> %s</div>'
+            % (values["divid"], self._cw._("click on the box to cancel the deletion"))
+        )
+    w('<div class="iformBody">')
 
 
 @monkeypatch(formrenderers.EntityInlinedFormRenderer)
 def close_form(self, w, form, values):  # noqa: F811
-    w(u'</div></div>')
+    w("</div></div>")
 
 
 @monkeypatch(formrenderers.EntityInlinedFormRenderer)
 def render_fields(self, w, form, values):  # noqa: F811
-    w(u'<fieldset id="fs-%(divid)s">' % values)
+    w('<fieldset id="fs-%(divid)s">' % values)
     fields = self._render_hidden_fields(w, form)
-    w(u'</fieldset>')
+    w("</fieldset>")
     if fields:
         self._render_fields(fields, w, form)
     self.render_child_forms(w, form, values)
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/forms.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2013-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2013-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact https://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -18,10 +18,10 @@
 __docformat__ = "restructuredtext en"
 
 
 from cubicweb_web.views.forms import FieldsForm
 from cubicweb_web.views.autoform import AutomaticEntityForm
 
 # Forms
-FieldsForm.needs_js += ('cubes.bootstrap.edition.js',)
+FieldsForm.needs_js += ("cubes.bootstrap.edition.js",)
 FieldsForm.needs_css = ()
-FieldsForm.cssclass = AutomaticEntityForm.cssclass = 'form-horizontal'
+FieldsForm.cssclass = AutomaticEntityForm.cssclass = "form-horizontal"
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formwidgets.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/formwidgets.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,29 +17,37 @@
 
 
 # Buttons
 @monkeypatch(formwidgets.Button)
 def render(self, form, field=None, renderer=None):
     label = form._cw._(self.label)
     attrs = self.attrs.copy()
-    if not cwver.startswith('3.20'):
+    if not cwver.startswith("3.20"):
         # 3.21 commit b0417cacecd9
-        attrs.setdefault('class', self.css_class)
+        attrs.setdefault("class", self.css_class)
     if self.cwaction:
         assert self.onclick is None
-        attrs['onclick'] = "postForm('__action_%s', \'%s\', \'%s\')" % (
-            self.cwaction, self.label, form.domid)
+        attrs["onclick"] = "postForm('__action_{}', '{}', '{}')".format(
+            self.cwaction,
+            self.label,
+            form.domid,
+        )
     elif self.onclick:
-        attrs['onclick'] = self.onclick
+        attrs["onclick"] = self.onclick
     if self.name:
-        attrs['name'] = self.name
+        attrs["name"] = self.name
         if self.setdomid:
-            attrs['id'] = self.name
+            attrs["id"] = self.name
     if not CW_325:
-        if self.settabindex and 'tabindex' not in attrs:
-            attrs['tabindex'] = form._cw.next_tabindex()
+        if self.settabindex and "tabindex" not in attrs:
+            attrs["tabindex"] = form._cw.next_tabindex()
     if self.icon:
-        img = u'<i class="%s"> </i>' % self.icon
+        img = '<i class="%s"> </i>' % self.icon
     else:
-        img = u''
-    return tags.button(img + xml_escape(label), escapecontent=False,
-                       value=label, type=self.type, **attrs)
+        img = ""
+    return tags.button(
+        img + xml_escape(label),
+        escapecontent=False,
+        value=label,
+        type=self.type,
+        **attrs,
+    )
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/htmlwidgets.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,41 @@
-"""bootstrap implementation of htmlwidgets
+"""bootstrap html helpers
 
 :organization: Logilab
-:copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
+:copyright: 2013-2022 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 __docformat__ = "restructuredtext en"
 
-from logilab.common.decorators import monkeypatch
 
-from cubicweb_web import htmlwidgets
-from cubicweb_web.component import Separator
+class DropDownBox:
+    ul_template = """
+    <a class="dropdown-toggle %(klass)s" data-toggle="dropdown" href="#">
+    %(title)s<span class="caret"></span></a>
+    <ul class="dropdown-menu" role="menu">%(actions)s</ul>"""
+
+    li_template = "<li>%(link)s<li>"
+
+    def __init__(self, title, actions, klass=""):
+        self.title = title
+        self.actions = actions
+        self.klass = klass
+
+    def render(self, w):
+        if not len(self.actions):
+            return ""
+        w(
+            self.ul_template
+            % {
+                "title": self.title,
+                "klass": self.klass,
+                "actions": "".join(self.render_items()),
+            }
+        )
+
+    def render_items(self):
+        for item in self.actions:
+            yield self.li_template % {"link": self._item_value(item)}
 
-
-@monkeypatch(Separator)
-def render(self, w):
-    w(u'<li class="divider"></li>')
-
-
-def bwcompatible_render_item(w, item):
-    if hasattr(item, 'render'):
-        if getattr(item, 'newstyle', False):
-            if isinstance(item, Separator):
-                item.render(w)
-            else:
-                w(u'<li>')
-                item.render(w)
-                w(u'</li>')
-        else:
-            item.render(w)  # XXX displays <li> by itself
-    else:
-        w(u'<li>%s</li>' % item)
-
-
-@monkeypatch(htmlwidgets.BoxMenu)
-def _render(self):
-    tag = u'li' if self.isitem else u'div'
-    self.w(u'<%s class="dropdown">' % tag)
-    self.w(u'<a class="dropdown-toggle" data-toggle="dropdown" href="#">'
-           u'%s&nbsp;'
-           u'<span class="caret"></span>'
-           u'</a>' % self.label)
-    self.w(u'<ul class="dropdown-menu">')
-    for item in self.items:
-        bwcompatible_render_item(self.w, item)
-    self.w(u'</ul>')
-    self.w(u'</%s>' % tag)
+    def _item_value(self, item):
+        return item
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/ibreadcrumbs.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/ibreadcrumbs.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,47 +9,49 @@
 
 from logilab.common.decorators import monkeypatch
 
 from cubicweb.entity import Entity
 from cubicweb_web.views import ibreadcrumbs
 
 
-ibreadcrumbs.BreadCrumbEntityVComponent.css_class = u'breadcrumb'
+ibreadcrumbs.BreadCrumbEntityVComponent.css_class = "breadcrumb"
 
 
 @monkeypatch(ibreadcrumbs.BreadCrumbEntityVComponent)
 def open_breadcrumbs(self, w):
-    w(u'<ul id="breadcrumbs" class="%s">' % self.css_class)
+    w('<ul id="breadcrumbs" class="%s">' % self.css_class)
 
 
 @monkeypatch(ibreadcrumbs.BreadCrumbEntityVComponent)
 def close_breadcrumbs(self, w):
-    w(u'</ul>')
+    w("</ul>")
 
 
 @monkeypatch(ibreadcrumbs.BreadCrumbEntityVComponent)
 def render_breadcrumbs(self, w, contextentity, path):
     root = path.pop(0)
     if isinstance(root, Entity):
-        w(u'<li>')
-        w(self.link_template % (self._cw.build_url(root.__regid__),
-                                root.dc_type('plural')))
-        w(u'</li>')
-    liclass = u' class="active"' if not path else u''
-    w(u'<li%s>' % liclass)
+        w("<li>")
+        w(
+            self.link_template
+            % (self._cw.build_url(root.__regid__), root.dc_type("plural"))
+        )
+        w("</li>")
+    liclass = ' class="active"' if not path else ""
+    w("<li%s>" % liclass)
     self.wpath_part(w, root, contextentity, not path)
-    w(u'</li>')
+    w("</li>")
     for i, parent in enumerate(path):
         last = i == len(path) - 1
-        liclass = u' class="active"' if last else u''
-        w(u'<li%s>' % liclass)
+        liclass = ' class="active"' if last else ""
+        w("<li%s>" % liclass)
         self.wpath_part(w, parent, contextentity, last)
-        w(u'</li>')
+        w("</li>")
 
 
 @monkeypatch(ibreadcrumbs.BreadCrumbAnyRSetVComponent)
 def render(self, w, **kwargs):
     self.open_breadcrumbs(w)
-    w(u'<li class="active">')
-    w(self._cw._('search'))
-    w(u'</li>')
+    w('<li class="active">')
+    w(self._cw._("search"))
+    w("</li>")
     self.close_breadcrumbs(w)
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/navigation.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/navigation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,172 +1,187 @@
-# -*- coding: utf-8 -*-
 """bootstrap implementation of navigation components
 
 :organization: Logilab
 :copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 from logilab.common.decorators import monkeypatch
 
 from logilab.mtconverter import xml_escape
 
 from cubicweb_web.view import View
 from cubicweb_web.component import NavigationComponent
 
-from cubicweb_web.views.navigation import (NextPrevNavigationComponent,
-                                           SortedNavigation,
-                                           PageNavigation,
-                                           PageNavigationSelect)
+from cubicweb_web.views.navigation import (
+    NextPrevNavigationComponent,
+    SortedNavigation,
+    PageNavigation,
+    PageNavigationSelect,
+)
 from cubicweb_bootstrap import CW_323
 
 __docformat__ = "restructuredtext en"
 
-NavigationComponent.page_link_templ = u'<li><a href="%s" title="%s">%s</a></li>'
-NavigationComponent.selected_page_link_templ = u'<li class="active"><a href="%s" title="%s">%s</a></li>'
+NavigationComponent.page_link_templ = '<li><a href="%s" title="%s">%s</a></li>'
+NavigationComponent.selected_page_link_templ = (
+    '<li class="active"><a href="%s" title="%s">%s</a></li>'
+)
 NavigationComponent.previous_page_link_templ = NavigationComponent.page_link_templ
 NavigationComponent.next_page_link_templ = NavigationComponent.page_link_templ
-NavigationComponent.no_previous_page_link = u'<li class="disabled"><a href="#">«</a></li>'
-NavigationComponent.no_next_page_link = u'<li class="disabled"><a href="#">»</a></li>'
-NavigationComponent.no_content_prev_link = u'«'
-NavigationComponent.no_content_next_link = u'»'
+NavigationComponent.no_previous_page_link = (
+    '<li class="disabled"><a href="#">«</a></li>'
+)
+NavigationComponent.no_next_page_link = '<li class="disabled"><a href="#">»</a></li>'
+NavigationComponent.no_content_prev_link = "«"
+NavigationComponent.no_content_next_link = "»"
 
 
 @monkeypatch(NavigationComponent)
 def render_link_back_to_pagination(self, w):
     "allow to come back to the paginated view"
     req = self._cw
     params = dict(req.form)
     basepath = req.relative_path(includeparams=False)
-    del params['__force_display']
+    del params["__force_display"]
     url = self.page_url(basepath, params)
-    w(u'<ul class="pagination"><li>'
-      u'<span><a href="%s">%s</a></span>'
-      u'</li></ul>'
-      % (xml_escape(url),
-         req._('back to pagination (%s results)') % self.page_size))
+    w(
+        '<ul class="pagination"><li>'
+        '<span><a href="%s">%s</a></span>'
+        "</li></ul>"
+        % (xml_escape(url), req._("back to pagination (%s results)") % self.page_size)
+    )
 
 
 @monkeypatch(NavigationComponent)
 def render_link_display_all(self, w):
     "make a link to see them all"
     req = self._cw
     params = dict(req.form)
     self.clean_params(params)
     basepath = req.relative_path(includeparams=False)
-    params['__force_display'] = 1
-    params['__fromnavigation'] = 1
+    params["__force_display"] = 1
+    params["__fromnavigation"] = 1
     url = self.page_url(basepath, params)
-    w(u'<ul class="pagination pull-right"><li>'
-      u'<span><a href="%s">%s</a></span>'
-      u'</li></ul>'
-      % (xml_escape(url), req._('show %s results') % len(self.cw_rset)))
+    w(
+        '<ul class="pagination pull-right"><li>'
+        '<span><a href="%s">%s</a></span>'
+        "</li></ul>" % (xml_escape(url), req._("show %s results") % len(self.cw_rset))
+    )
 
 
 @monkeypatch(SortedNavigation)
 def write_links(self, basepath, params, blocklist):
     """Return HTML for the whole navigation: `blocklist` is a list of HTML
     snippets for each page, `basepath` and `params` will be necessary to
     build previous/next links.
     """
-    self.w(u'<ul class="pagination">')
-    self.w(u'%s&#160;' % self.previous_link(basepath, params))
-    self.w(u'%s' % u''.join(blocklist))
-    self.w(u'&#160;%s' % self.next_link(basepath, params))
-    self.w(u'</ul>')
+    self.w('<ul class="pagination">')
+    self.w("%s&#160;", self.previous_link(basepath, params), escape=False)
+    self.w("%s", "".join(blocklist), escape=False)
+    self.w("&#160;%s", self.next_link(basepath, params), escape=False)
+    self.w("</ul>")
 
 
 @monkeypatch(PageNavigation)
 def call(self):
     """displays a resultset by page"""
     params = dict(self._cw.form)
     self.clean_params(params)
     basepath = self._cw.relative_path(includeparams=False)
-    self.w(u'<ul class="pagination">')
-    self.w(u'%s&#160;' % self.previous_link(basepath, params))
-    self.w(u'&#160;'.join(self.iter_page_links(basepath, params)))
-    self.w(u'&#160;%s' % self.next_link(basepath, params))
-    self.w(u'</ul>')
+    self.w('<ul class="pagination">')
+    self.w("%s&#160;", self.previous_link(basepath, params), escape=False)
+    self.w("&#160;".join(self.iter_page_links(basepath, params)), escape=False)
+    self.w("&#160;%s", self.next_link(basepath, params), escape=False)
+    self.w("</ul>")
 
 
-NextPrevNavigationComponent.prev_icon = u'&#8592;'
-NextPrevNavigationComponent.next_icon = u'&#8594;'
+NextPrevNavigationComponent.prev_icon = "&#8592;"
+NextPrevNavigationComponent.next_icon = "&#8594;"
 
 
 @monkeypatch(NextPrevNavigationComponent)
 # Should be better done, but this works
 def render_body(self, w):
-    w(u'<div class="prevnext row">')
-    w(u'<ul class="pager">')
+    w('<div class="prevnext row">')
+    w('<ul class="pager">')
     self.prevnext(w)
-    w(u'</ul>')
-    w(u'</div>')
+    w("</ul>")
+    w("</div>")
     # w(u'<div class="clear"></div>')
 
 
 @monkeypatch(NextPrevNavigationComponent)
 def prevnext_div(self, w, type, cssclass, url, title, content):
-    csscls = {'prev': 'previous', 'next': 'next'}
-    w(u'<li class="%s">' % csscls[type])
-    w(u'<a href="%s" title="%s">%s</a>' % (xml_escape(url),
-                                           xml_escape(title),
-                                           content))
-    w(u'</li>')
-    self._cw.html_headers.add_raw(
-        '<link rel="%s" href="%s" />' % (type, xml_escape(url)))
+    csscls = {"prev": "previous", "next": "next"}
+    w('<li class="%s">' % csscls[type])
+    w(
+        '<a href="{}" title="{}">{}</a>'.format(
+            xml_escape(url), xml_escape(title), content
+        )
+    )
+    w("</li>")
+    self._cw.html_headers.add_raw(f'<link rel="{type}" href="{xml_escape(url)}" />')
 
 
 def do_paginate(view, rset=None, w=None, show_all_option=True, page_size=None):
     """write pages index in w stream (default to view.w) and then limit the
     result set (default to view.rset) to the currently displayed page if we're
     not explicitly told to display everything (by setting __force_display in
     req.form)
     """
     req = view._cw
     if rset is None:
         rset = view.cw_rset
     if w is None:
         w = view.w
-    nav = req.vreg['components'].select_or_none(
-        'navigation', req, rset=rset, page_size=page_size, view=view)
+    nav = req.vreg["components"].select_or_none(
+        "navigation", req, rset=rset, page_size=page_size, view=view
+    )
     if nav:
         if w is None:
             w = view.w
-        if req.form.get('__force_display'):
+        if req.form.get("__force_display"):
             # allow to come back to the paginated view
             params = dict(req.form)
             basepath = req.relative_path(includeparams=False)
-            del params['__force_display']
+            del params["__force_display"]
             url = nav.page_url(basepath, params)
-            w(u'<span><a href="%s">%s</a></span>\n'
-              % (xml_escape(url),
-                 req._('back to pagination (%s results)') % nav.page_size))
+            w(
+                '<span><a href="%s">%s</a></span>\n'
+                % (
+                    xml_escape(url),
+                    req._("back to pagination (%s results)") % nav.page_size,
+                )
+            )
         else:
             # get boundaries before component rendering
             start, stop = nav.page_boundaries()
             nav.render(w=w)
             params = dict(req.form)
             nav.clean_params(params)
             # make a link to see them all
             if show_all_option:
                 basepath = req.relative_path(includeparams=False)
-                params['__force_display'] = 1
-                params['__fromnavigation'] = 1
+                params["__force_display"] = 1
+                params["__fromnavigation"] = 1
                 url = nav.page_url(basepath, params)
-                w(u'<span><a href="%s">%s</a></span>\n'
-                  % (xml_escape(url), req._('show %s results') % len(rset)))
-            rset.limit(offset=start, limit=stop-start, inplace=True)  # noqa
+                w(
+                    '<span><a href="%s">%s</a></span>\n'
+                    % (xml_escape(url), req._("show %s results") % len(rset))
+                )
+            rset.limit(offset=start, limit=stop - start, inplace=True)  # noqa
 
 
 def paginate(view, show_all_option=True, w=None, page_size=None, rset=None):
-    """paginate results if the view is paginable
-    """
+    """paginate results if the view is paginable"""
     if view.paginable:
         do_paginate(view, rset, w, show_all_option, page_size)
 
+
 # monkey patch base View class to add a .paginate([...])
 # method to be called to write pages index in the view and then limit the result
 # set to the current page
 
 
 if not CW_323:
     View.do_paginate = do_paginate
@@ -175,23 +190,27 @@
 
 
 @monkeypatch(PageNavigationSelect)
 def call(self):  # noqa: F811
     params = dict(self._cw.form)
     self.clean_params(params)
     basepath = self._cw.relative_path(includeparams=False)
-    w = self.w
-    w(u'<ul class="pagination">')
-    w(self.previous_link(basepath, params))
+    self.w('<ul class="pagination">')
+    self.w(self.previous_link(basepath, params))
     start, stop = self.page_boundaries()
-    w(u'<li><span><a class="dropdown-toggle" data-toggle="dropdown" href="#">'
-        '%s<span class="caret"></span></a>' % self.index_display(start, stop - 1))
-    w(u'<ul class="dropdown-menu" role="menu">')
+    self.w(
+        '<li><span><a class="dropdown-toggle" data-toggle="dropdown" href="#">'
+        '%s<span class="caret"></span></a>',
+        self.index_display(start, stop - 1),
+    )
+    self.w('<ul class="dropdown-menu" role="menu">')
     for option in self.iter_page_links(basepath, params):
-        w(option)
-    w(u'</ul></span></li>')
-    w(u'&#160;%s' % self.next_link(basepath, params))
-    w(u'</ul>')
+        self.w(option)
+    self.w("</ul></span></li>")
+    self.w("&#160;%s", self.next_link(basepath, params), escape=False)
+    self.w("</ul>")
 
 
-PageNavigationSelect.page_link_templ = u'<li><a href="%s" title="%s">%s</a></li>'
-PageNavigationSelect.selected_page_link_templ = u'<li class="disabled"><a href="%s" title="%s">%s</a></li>'
+PageNavigationSelect.page_link_templ = '<li><a href="%s" title="%s">%s</a></li>'
+PageNavigationSelect.selected_page_link_templ = (
+    '<li class="disabled"><a href="%s" title="%s">%s</a></li>'
+)
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/primary.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/primary.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,117 +4,119 @@
 :copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
-from logilab.mtconverter import xml_escape
 
 from cubicweb_web.views import primary
 
 
 @monkeypatch(primary.PrimaryView)
 def render_entity(self, entity):
     self.render_entity_toolbox(entity)
     self.render_entity_title(entity)
     # entity's attributes and relations, excluding meta data
     # if the entity isn't meta itself
     if self.is_primary():
         boxes = self._prepare_side_boxes(entity)
     else:
         boxes = None
-    if boxes or hasattr(self, 'render_side_related'):
-        self.w(u'<div class="row">'
-               u'<div class="col-md-8">')
-    self.content_navigation_components('navcontenttop')
+    if boxes or hasattr(self, "render_side_related"):
+        self.w('<div class="row">' '<div class="col-md-8">')
+    self.content_navigation_components("navcontenttop")
     self.render_entity_attributes(entity)
     if self.main_related_section:
         self.render_entity_relations(entity)
-    self.content_navigation_components('navcontentbottom')
+    self.content_navigation_components("navcontentbottom")
     # side boxes
-    if boxes or hasattr(self, 'render_side_related'):
-        self.w(u'</div>'  # </col-md-8>
-               u'<div class="col-md-4">')
+    if boxes or hasattr(self, "render_side_related"):
+        self.w("</div>" '<div class="col-md-4">')  # </col-md-8>
         self.render_side_boxes(boxes)
-        self.w(u'</div>'  # </col-md-4>
-               u'</div>')  # </row>
+        self.w("</div>" "</div>")  # </col-md-4>  # </row>
 
 
 @monkeypatch(primary.PrimaryView)
 def render_entity_attributes(self, entity):
-    """Renders all attributes and relations in the 'attributes' section.
-    """
+    """Renders all attributes and relations in the 'attributes' section."""
     display_attributes = []
-    for rschema, _, role, dispctrl in self._section_def(entity, 'attributes'):
-        vid = dispctrl.get('vid', 'reledit')
-        if rschema.final or vid == 'reledit' or dispctrl.get('rtypevid'):
-            value = entity.view(vid, rtype=rschema.type, role=role,
-                                initargs={'dispctrl': dispctrl})
+    for rschema, _, role, dispctrl in self._section_def(entity, "attributes"):
+        vid = dispctrl.get("vid", "reledit")
+        if rschema.final or vid == "reledit" or dispctrl.get("rtypevid"):
+            value = entity.view(
+                vid, rtype=rschema.type, role=role, initargs={"dispctrl": dispctrl}
+            )
         else:
             rset = self._relation_rset(entity, rschema, role, dispctrl)
             if rset:
                 value = self._cw.view(vid, rset)
             else:
                 value = None
-        if value is not None and value != '':
+        if value is not None and value != "":
             display_attributes.append((rschema, role, dispctrl, value))
     if display_attributes:
         # bs customization begins
-        self.w(u'<table class="table cw-table-primary-entity">')
+        self.w('<table class="table cw-table-primary-entity">')
         # bs customization ends
         for rschema, role, dispctrl, value in display_attributes:
             label = self._rel_label(entity, rschema, role, dispctrl)
             self.render_attribute(label, value, table=True)
-        self.w(u'</table>')
+        self.w("</table>")
 
 
 @monkeypatch(primary.PrimaryView)
 def render_relation(self, label, value):
-    self.w(u'<div class="panel panel-default relations">')
+    self.w('<div class="panel panel-default relations">')
     if label:
-        self.w(u'<div class="panel-heading"><div class="panel-title">%s</div></div>' % label)
-    self.w(u'<div class="panel-body">')
+        self.w(
+            '<div class="panel-heading"><div class="panel-title">%s</div></div>', label
+        )
+    self.w('<div class="panel-body">')
     self.w(value)
-    self.w(u'</div>')
-    self.w(u'</div>')
+    self.w("</div>")
+    self.w("</div>")
 
 
 @monkeypatch(primary.RelatedView)
 def call(self, **kwargs):
-    if 'dispctrl' in self.cw_extra_kwargs:
-        if 'limit' in self.cw_extra_kwargs['dispctrl']:
-            limit = self.cw_extra_kwargs['dispctrl']['limit']
+    if "dispctrl" in self.cw_extra_kwargs:
+        if "limit" in self.cw_extra_kwargs["dispctrl"]:
+            limit = self.cw_extra_kwargs["dispctrl"]["limit"]
         else:
-            limit = self._cw.property_value('navigation.related-limit')
-        list_limit = self.cw_extra_kwargs['dispctrl'].get('use_list_limit', 5)
-        subvid = self.cw_extra_kwargs['dispctrl'].get('subvid', 'incontext')
+            limit = self._cw.property_value("navigation.related-limit")
+        list_limit = self.cw_extra_kwargs["dispctrl"].get("use_list_limit", 5)
+        subvid = self.cw_extra_kwargs["dispctrl"].get("subvid", "incontext")
     else:
         limit = list_limit = None
-        subvid = 'incontext'
+        subvid = "incontext"
     if limit is None or self.cw_rset.rowcount <= limit:
         if self.cw_rset.rowcount == 1:
             self.wview(subvid, self.cw_rset, row=0)
         elif list_limit is None or 1 < self.cw_rset.rowcount <= list_limit:
-            self.wview('csv', self.cw_rset, subvid=subvid)
+            self.wview("csv", self.cw_rset, subvid=subvid)
         else:
             # bs customization begins
-            self.wview('list', self.cw_rset, subvid=subvid, klass='list-unstyled')
+            self.wview("list", self.cw_rset, subvid=subvid, klass="list-unstyled")
             # bs customization ends
     # else show links to display related entities
     else:
         rql = self.cw_rset.printable_rql()
         rset = self.cw_rset.limit(limit)  # remove extra entity
         if list_limit is None:
-            self.wview('csv', rset, subvid=subvid)
-            self.w(u'<a href="%s" class="see-all">%s</a>' % (
-                xml_escape(self._cw.build_url(rql=rql, vid='list', subvid=subvid)),
-                self._cw._('see them all')))
+            self.wview("csv", rset, subvid=subvid)
+            self.w(
+                '<a href="%s" class="see-all">%s</a>',
+                self._cw.build_url(rql=rql, vid="list", subvid=subvid),
+                self._cw._("see them all"),
+            )
         else:
-            self.w(u'<div>')
+            self.w("<div>")
             # bs customization begins
-            self.wview('list', rset, subvid=subvid, klass='list-unstyled')
+            self.wview("list", rset, subvid=subvid, klass="list-unstyled")
             # bs customization ends
-            self.w(u'<a href="%s" class="see-all">%s</a>' % (
-                xml_escape(self._cw.build_url(rql=rql, vid='list', subvid=subvid)),
-                self._cw._('see them all')))
-            self.w(u'</div>')
+            self.w(
+                '<a href="%s" class="see-all">%s</a>',
+                self._cw.build_url(rql=rql, vid="list", subvid=subvid),
+                self._cw._("see them all"),
+            )
+            self.w("</div>")
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/reledit.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/reledit.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,28 @@
 :organization: Logilab
 :copyright: 2013-2022 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 from cubicweb_web.views.reledit import AutoClickAndEditFormView
-AutoClickAndEditFormView._addzone = u' <span class="glyphicon glyphicon-plus"></span>'
-AutoClickAndEditFormView._deletezone = u' <span class="glyphicon glyphicon-remove"></span>'
-AutoClickAndEditFormView._editzone = u' <span class="glyphicon glyphicon-pencil"></span>'
+
+AutoClickAndEditFormView._addzone = ' <span class="glyphicon glyphicon-plus"></span>'
+AutoClickAndEditFormView._deletezone = (
+    ' <span class="glyphicon glyphicon-remove"></span>'
+)
+AutoClickAndEditFormView._editzone = ' <span class="glyphicon glyphicon-pencil"></span>'
 
 try:
     from cubicweb_inlinedit.views import reledit
 except ImportError:
     pass
 else:
-    reledit.ReleditRelationFormHandler._addzone = u' <span class="glyphicon glyphicon-plus"></span>'
-    reledit.ReleditFormHandler._editzone = u' <span class="glyphicon glyphicon-pencil"></span>'
-    reledit.ReleditEntityFormHandler._deletezone = u' <span class="glyphicon glyphicon-remove"></span>'
+    reledit.ReleditRelationFormHandler._addzone = (
+        ' <span class="glyphicon glyphicon-plus"></span>'
+    )
+    reledit.ReleditFormHandler._editzone = (
+        ' <span class="glyphicon glyphicon-pencil"></span>'
+    )
+    reledit.ReleditEntityFormHandler._deletezone = (
+        ' <span class="glyphicon glyphicon-remove"></span>'
+    )
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/startup.py` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap/views/startup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """bootstrap implementation of startup views
 
 :organization: Logilab
 :copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
@@ -10,77 +9,98 @@
 
 from logilab.common.decorators import monkeypatch
 from logilab.common.textutils import unormalize
 from logilab.mtconverter import xml_escape
 
 from cubicweb_web.views import startup, uicfg
 
-startup.ManageView.box_html = u'''<div class="panel panel-default">
+startup.ManageView.box_html = """<div class="panel panel-default">
     <div class="panel-heading">
-        <div class="panel-title">%(title)s</div>
+        <div class="panel-title">%s</div>
     </div>
-    <div class="panel-body">%(content)s</div>
-    </div>'''
+    <div class="panel-body">%s</div>
+    </div>"""
 
 
 @monkeypatch(startup.ManageView)
 def manage_actions(self):
-    allactions = self._cw.vreg['actions'].possible_actions(self._cw)
-    if allactions.get('manage'):
+    allactions = self._cw.vreg["actions"].possible_actions(self._cw)
+    if allactions.get("manage"):
         html = []
         w = html.append
-        w(u'<ul>')
-        for action in allactions['manage']:
-            w(u'<li><a href="%s">%s</a></li>' % (
-                action.url(), self._cw._(action.title)))
-        w(u'</ul>')
-        self.w(self.box_html % {'title': self._cw._('Manage'),
-                                'content': u'\n'.join(html)})
+        w("<ul>")
+        for action in allactions["manage"]:
+            w(
+                '<li><a href="{}">{}</a></li>'.format(
+                    action.url(), self._cw._(action.title)
+                )
+            )
+        w("</ul>")
+        self.w(
+            self.box_html,
+            self._cw._("Manage"),
+            "\n".join(html),
+            escape=False,
+        )
 
 
 @monkeypatch(startup.ManageView)
 def startup_views(self):
-    views = [v for v in self._cw.vreg['views'].possible_views(self._cw, None)
-             if v.category == 'startupview'
-             and v.__regid__ not in self.skip_startup_views]
+    views = [
+        v
+        for v in self._cw.vreg["views"].possible_views(self._cw, None)
+        if v.category == "startupview" and v.__regid__ not in self.skip_startup_views
+    ]
     if not views:
         return
     html = []
     w = html.append
-    w(u'<ul>')
+    w("<ul>")
     for v in sorted(views, key=lambda x: self._cw._(x.title)):
-        w('<li><a href="%s">%s</a></li>' % (
-            xml_escape(v.url()), xml_escape(self._cw._(v.title).capitalize())))
-    w(u'</ul>')
-    self.w(self.box_html % {'title': self._cw._('Startup views'),
-                            'content': u'\n'.join(html)})
+        w(
+            '<li><a href="%s">%s</a></li>'
+            % (xml_escape(v.url()), xml_escape(self._cw._(v.title).capitalize()))
+        )
+    w("</ul>")
+    self.w(
+        self.box_html,
+        self._cw._("Startup views"),
+        "\n".join(html),
+        escape=False,
+    )
 
 
 @monkeypatch(startup.ManageView)
 def entities(self):
     schema = self._cw.vreg.schema
-    eschemas = [eschema for eschema in schema.entities()
-                if uicfg.indexview_etype_section.get(eschema) == 'application']
+    eschemas = [
+        eschema
+        for eschema in schema.entities()
+        if uicfg.indexview_etype_section.get(eschema) == "application"
+    ]
     if eschemas:
         html = self.entity_types_table(eschemas)
-        self.w(self.box_html % {'title': self._cw._('Browse by entity type'),
-                                'content': u'\n'.join(html)})
+        self.w(
+            self.box_html,
+            self._cw._("Browse by entity type"),
+            "\n".join(html),
+            escape=False,
+        )
 
 
 @monkeypatch(startup.ManageView)
 def entity_types_table(self, eschemas):
-    infos = sorted(self.entity_types(eschemas),
-                   key=lambda t: unormalize(t[0]))
+    infos = sorted(self.entity_types(eschemas), key=lambda t: unormalize(t[0]))
     q, r = divmod(len(infos), 2)
     html = []
     w = html.append
-    w(u'<div class="row">')
-    for links in (infos[:q + r], infos[q + r:]):
+    w('<div class="row">')
+    for links in (infos[: q + r], infos[q + r :]):
         if links:
-            w(u'<div class="col-md-6">')
-            w(u'<ul class="list-unstyled">')
-            for (_, etypelink, addlink) in links:
-                w('<li>%s %s</li>' % (addlink, etypelink))
-            w(u'</ul>')
-            w(u'</div>')
-    w(u'</div>')
+            w('<div class="col-md-6">')
+            w('<ul class="list-unstyled">')
+            for _, etypelink, addlink in links:
+                w(f"<li>{addlink} {etypelink}</li>")
+            w("</ul>")
+            w("</div>")
+    w("</div>")
     return html
```

### Comparing `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/SOURCES.txt` & `cubicweb-bootstrap-2.0.0/cubicweb_bootstrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/doc/Makefile` & `cubicweb-bootstrap-2.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/doc/README.rst` & `cubicweb-bootstrap-2.0.0/doc/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/doc/conf.py` & `cubicweb-bootstrap-2.0.0/doc/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Bootstrap documentation build configuration file, created by
 # sphinx-quickstart on Wed Jun 15 10:14:35 2011.
 #
 # This file is execfile()d with the current directory set to its containing dir.
 #
 # Note that not all possible configuration values are present in this
@@ -12,216 +11,213 @@
 # serve to show the default.
 
 import sys, os
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest', 'sphinx.ext.intersphinx']
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.doctest", "sphinx.ext.intersphinx"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'bootstrap'
-copyright = u'2013-2022, Logilab'
+project = "bootstrap"
+copyright = "2013-2022, Logilab"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 from cubicweb_bootstrap.__pkginfo__ import version
+
 ##version = '0.8.4'
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build"]
 
 # The reST default role (used for this markup: `text`) to use for all documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = "default"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'bootstrapdoc'
+htmlhelp_basename = "bootstrapdoc"
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 # The paper size ('letter' or 'a4').
-#latex_paper_size = 'letter'
+# latex_paper_size = 'letter'
 
 # The font size ('10pt', '11pt' or '12pt').
-#latex_font_size = '10pt'
+# latex_font_size = '10pt'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'bootstrap.tex', u'Bootstrap documentation',
-   u'Logilab', 'manual'),
+    ("index", "bootstrap.tex", "Bootstrap documentation", "Logilab", "manual"),
 ]
 
 latex_elements = {
-  'papersize':'a4paper',
-  'babel': '\\usepackage[english,french]{babel}',
-  'fncychap': '\\usepackage[Sonny]{fncychap}'
+    "papersize": "a4paper",
+    "babel": "\\usepackage[english,french]{babel}",
+    "fncychap": "\\usepackage[Sonny]{fncychap}",
 }
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Additional stuff for the LaTeX preamble.
-#latex_preamble = ''
+# latex_preamble = ''
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    ('index', 'bootstrap', u'Bootstrap documentation',
-     [u'Logilab'], 1)
-]
+man_pages = [("index", "bootstrap", "Bootstrap documentation", ["Logilab"], 1)]
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'http://docs.python.org/': None}
+intersphinx_mapping = {"http://docs.python.org/": None}
```

### Comparing `cubicweb-bootstrap-1.9.0/doc/release_0.5.0.rst` & `cubicweb-bootstrap-2.0.0/doc/release_0.5.0.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.9.0/setup.py` & `cubicweb-bootstrap-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact https://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of a cubicweb-bootstrap.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -27,53 +27,57 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_bootstrap', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_bootstrap", "__pkginfo__.py")
 __pkginfo__ = {}
 with open(pkginfo) as f:
     exec(f.read(), __pkginfo__)
 
 # get required metadatas
-distname = __pkginfo__['distname']
-version = __pkginfo__['version']
-license = __pkginfo__['license']
-description = __pkginfo__['description']
-web = __pkginfo__['web']
-author = __pkginfo__['author']
-author_email = __pkginfo__['author_email']
-classifiers = __pkginfo__['classifiers']
+distname = __pkginfo__["distname"]
+version = __pkginfo__["version"]
+license = __pkginfo__["license"]
+description = __pkginfo__["description"]
+web = __pkginfo__["web"]
+author = __pkginfo__["author"]
+author_email = __pkginfo__["author_email"]
+classifiers = __pkginfo__["classifiers"]
 
 # get optional metadatas
-data_files = __pkginfo__.get('data_files', None)
-dependency_links = __pkginfo__.get('dependency_links', ())
+data_files = __pkginfo__.get("data_files", None)
+dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = ["{0} {1}".format(d, v and v or "").strip()
-                    for d, v in requires.items()]
+install_requires = [
+    "{} {}".format(d, v and v or "").strip() for d, v in requires.items()
+]
 
+with open(join(here, "README.rst")) as f:
+    long_description = f.read()
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
+    long_description=long_description,
     author=author,
     author_email=author_email,
     url=web,
     classifiers=classifiers,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
-        'cubicweb.cubes': [
-            'bootstrap=cubicweb_bootstrap',
+        "cubicweb.cubes": [
+            "bootstrap=cubicweb_bootstrap",
         ],
     },
     zip_safe=False,
     python_requires=">=2.7",
 )
```

### Comparing `cubicweb-bootstrap-1.9.0/test/test_bootstrap.py` & `cubicweb-bootstrap-2.0.0/test/test_bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2013-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2013-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact https://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -45,24 +45,27 @@
 from cubicweb_bootstrap import monkeypatch_default_value
 
 
 class MonkeypatchDefaultValueTC(TestCase):
     def test_function(self):
         def func(a, b, c=0, d=None, e=False, f=()):
             return c
+
         self.assertEqual(func(1, 2), 0)
-        monkeypatch_default_value(func, 'c', 42)
+        monkeypatch_default_value(func, "c", 42)
         self.assertEqual(func(1, 2), 42)
 
     def test_method(self):
-        class Class(object):
+        class Class:
             def meth(self, a, b, c=0, d=None, e=False, f=()):
                 return c
+
         obj = Class()
         self.assertEqual(obj.meth(1, 2), 0)
-        monkeypatch_default_value(Class.meth, 'c', 42)
+        monkeypatch_default_value(Class.meth, "c", 42)
         self.assertEqual(obj.meth(1, 2), 42)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import unittest
+
     unittest.main()
```

### Comparing `cubicweb-bootstrap-1.9.0/test/unittest_views.py` & `cubicweb-bootstrap-2.0.0/test/unittest_views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import unittest
 
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb.devtools.htmlparser import XMLValidator
 
 
-class BoostrapLogFormTemplateTC(CubicWebTC):
-
+class BoostrapLogFormTemplateTC(WebCWTC):
     def _login_labels(self):
-        valid = self.content_type_validators.get('text/html', XMLValidator)()
-        with self.new_access(u'anon').web_request() as req:
-            page = valid.parse_string(self.vreg['views'].main_template(req, 'login'))
-        return page.find_tag('label')
+        valid = self.content_type_validators.get("text/html", XMLValidator)()
+        with self.new_access("anon").web_request() as req:
+            page = valid.parse_string(self.vreg["views"].main_template(req, "login"))
+        return page.find_tag("label")
 
     def test_label(self):
-        self.set_option('allow-email-login', 'yes')
-        self.assertEqual(self._login_labels(), ['login or email', 'password'])
-        self.set_option('allow-email-login', 'no')
-        self.assertEqual(self._login_labels(), ['login', 'password'])
+        self.set_option("allow-email-login", "yes")
+        self.assertEqual(self._login_labels(), ["login or email", "password"])
+        self.set_option("allow-email-login", "no")
+        self.assertEqual(self._login_labels(), ["login", "password"])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `cubicweb-bootstrap-1.9.0/tox.ini` & `cubicweb-bootstrap-2.0.0/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tox]
-envlist =  py3, flake8, check-manifest, yamllint
+envlist =  py3, flake8, check-manifest, yamllint, black
 
 [testenv]
 deps =
   pytest
+  webtest
   git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
   {envpython} -m pytest {posargs}
 
 [pytest]
 python_files = *test_*.py
 testpaths = test
@@ -24,21 +25,23 @@
 skip_install = true
 deps =
   check-manifest
 commands =
   {envpython} -m check_manifest {toxinidir}
 
 [flake8]
+basepython = python3
+ignore = W503, E203, E731, E231
 max-line-length = 120
 exclude = cubicweb_bootstrap/migration/*,.tox/*,doc/*
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -48,7 +51,21 @@
 
 [testenv:yamllint]
 skip_install = true
 deps = yamllint
 commands =
   yamllint .
 
+
+[testenv:black]
+basepython = python3
+skip_install = true
+deps =
+  black >= 22.12
+commands = black --check .
+
+[testenv:black-run]
+basepython = python3
+skip_install = true
+deps =
+  black >= 22.12
+commands = black .
```

