# Comparing `tmp/pyams_zmi-1.9.0.tar.gz` & `tmp/pyams_zmi-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_zmi-1.9.0.tar", last modified: Thu Nov 25 22:20:50 2021, max compression
+gzip compressed data, was "dist/pyams_zmi-1.9.2.tar", last modified: Fri Nov 26 15:55:07 2021, max compression
```

## Comparing `pyams_zmi-1.9.0.tar` & `pyams_zmi-1.9.2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      104 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6757 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)     3829 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/docs/HISTORY.txt
--rw-rw-rw-   0 root         (0) root         (0)     1088 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/docs/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2857 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/
--rw-rw-rw-   0 root         (0) root         (0)      855 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6232 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/doctests/
--rw-rw-rw-   0 root         (0) root         (0)      721 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     7237 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/form.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/generations/
--rw-rw-rw-   0 root         (0) root         (0)      567 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      771 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/generations/zodbupdate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/helper/
--rw-rw-rw-   0 root         (0) root         (0)      562 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/helper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5819 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/helper/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/helper/event.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     1431 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8186 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4360 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/form.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/
--rw-rw-rw-   0 root         (0) root         (0)      744 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/admin-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1883 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form-checker.pt
--rw-rw-rw-   0 root         (0) root         (0)     2587 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1676 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form-group.pt
--rw-rw-rw-   0 root         (0) root         (0)     1606 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form-switcher.pt
--rw-rw-rw-   0 root         (0) root         (0)     1393 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form-tabform.pt
--rw-rw-rw-   0 root         (0) root         (0)     3257 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form.pt
--rw-rw-rw-   0 root         (0) root         (0)      454 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/inner-table-empty.pt
--rw-rw-rw-   0 root         (0) root         (0)      770 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/inner-table.pt
--rw-rw-rw-   0 root         (0) root         (0)      130 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/search-view.pt
--rw-rw-rw-   0 root         (0) root         (0)      738 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/table-empty.pt
--rw-rw-rw-   0 root         (0) root         (0)      763 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/table-multiple.pt
--rw-rw-rw-   0 root         (0) root         (0)     1026 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/table.pt
--rw-rw-rw-   0 root         (0) root         (0)     3398 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/interfaces/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11091 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.mo
--rw-rw-rw-   0 root         (0) root         (0)    17825 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.po
--rw-rw-rw-   0 root         (0) root         (0)    12825 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/locales/pyams_zmi.pot
--rw-rw-rw-   0 root         (0) root         (0)     4064 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     2502 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/skin.py
--rw-rw-rw-   0 root         (0) root         (0)    15303 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/tests/
--rw-rw-rw-   0 root         (0) root         (0)      798 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1821 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     1208 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2269 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1218 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/breadcrumb.py
--rw-rw-rw-   0 root         (0) root         (0)     7366 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4380 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/controlpanel.py
--rw-rw-rw-   0 root         (0) root         (0)     7844 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3258 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/metas.py
--rw-rw-rw-   0 root         (0) root         (0)     2442 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     6604 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     4778 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/skin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)       81 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/templates/admin-index.pt
--rw-rw-rw-   0 root         (0) root         (0)      324 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/templates/breadcrumbs.pt
--rw-rw-rw-   0 root         (0) root         (0)     1768 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/timezone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      567 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1757 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/aside.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/breadcrumb.py
--rw-rw-rw-   0 root         (0) root         (0)     3182 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/logo.py
--rw-rw-rw-   0 root         (0) root         (0)     4020 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/menu.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/nav.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/ribbon.py
--rw-rw-rw-   0 root         (0) root         (0)     1522 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/
--rw-rw-rw-   0 root         (0) root         (0)       68 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/ajax-gear.pt
--rw-rw-rw-   0 root         (0) root         (0)       50 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/header.pt
--rw-rw-rw-   0 root         (0) root         (0)      332 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/hide-nav.pt
--rw-rw-rw-   0 root         (0) root         (0)      225 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/logo.pt
--rw-rw-rw-   0 root         (0) root         (0)       70 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/modal-header.pt
--rw-rw-rw-   0 root         (0) root         (0)       25 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/nav-divider.pt
--rw-rw-rw-   0 root         (0) root         (0)       24 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/nav-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      692 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/nav-item.pt
--rw-rw-rw-   0 root         (0) root         (0)      211 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/nav-menu.pt
--rw-rw-rw-   0 root         (0) root         (0)      120 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/page-aside.pt
--rw-rw-rw-   0 root         (0) root         (0)      172 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/page-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      554 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/page-nav.pt
--rw-rw-rw-   0 root         (0) root         (0)       62 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/page-ribbon.pt
--rw-rw-rw-   0 root         (0) root         (0)     1001 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/site-search.pt
--rw-rw-rw-   0 root         (0) root         (0)      154 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/toolbar.pt
--rw-rw-rw-   0 root         (0) root         (0)      154 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/top-links.pt
--rw-rw-rw-   0 root         (0) root         (0)      136 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/top-menu-item.pt
--rw-rw-rw-   0 root         (0) root         (0)      519 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/top-menu.pt
--rw-rw-rw-   0 root         (0) root         (0)      613 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/top-menus-group.pt
--rw-rw-rw-   0 root         (0) root         (0)      185 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/top-tab.pt
--rw-rw-rw-   0 root         (0) root         (0)      397 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/top-tabs.pt
--rw-rw-rw-   0 root         (0) root         (0)      162 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/user-links.pt
--rw-rw-rw-   0 root         (0) root         (0)      454 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/user-menu.pt
--rw-rw-rw-   0 root         (0) root         (0)      206 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/version.pt
--rw-rw-rw-   0 root         (0) root         (0)     2499 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/toolbar.py
--rw-rw-rw-   0 root         (0) root         (0)     3113 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/toplinks.py
--rw-rw-rw-   0 root         (0) root         (0)     3642 2021-11-25 22:20:35.000000 pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/userlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6757 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4001 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      351 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2021-11-25 22:20:50.000000 pyams_zmi-1.9.0/src/pyams_zmi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6948 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     3956 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/docs/HISTORY.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/docs/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2857 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      855 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7237 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/form.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/generations/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      771 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/generations/zodbupdate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/helper/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/helper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5819 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/helper/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/helper/event.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8186 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4360 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      744 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/admin-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form-checker.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1676 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form-group.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form-switcher.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form-tabform.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3257 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form.pt
+-rw-rw-rw-   0 root         (0) root         (0)      454 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/inner-table-empty.pt
+-rw-rw-rw-   0 root         (0) root         (0)      770 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/inner-table.pt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/search-view.pt
+-rw-rw-rw-   0 root         (0) root         (0)      738 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/table-empty.pt
+-rw-rw-rw-   0 root         (0) root         (0)      763 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/table-multiple.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/table.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3398 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/interfaces/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11091 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.mo
+-rw-rw-rw-   0 root         (0) root         (0)    17825 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.po
+-rw-rw-rw-   0 root         (0) root         (0)    12825 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/locales/pyams_zmi.pot
+-rw-rw-rw-   0 root         (0) root         (0)     4064 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2502 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/skin.py
+-rw-rw-rw-   0 root         (0) root         (0)    15303 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      798 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/breadcrumb.py
+-rw-rw-rw-   0 root         (0) root         (0)     7366 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4380 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/controlpanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     7844 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3258 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/metas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2442 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6604 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/skin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/templates/admin-index.pt
+-rw-rw-rw-   0 root         (0) root         (0)      324 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/templates/breadcrumbs.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1768 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/timezone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/aside.py
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/breadcrumb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3182 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/logo.py
+-rw-rw-rw-   0 root         (0) root         (0)     4020 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/menu.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/nav.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/ribbon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1522 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/ajax-gear.pt
+-rw-rw-rw-   0 root         (0) root         (0)       50 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      332 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/hide-nav.pt
+-rw-rw-rw-   0 root         (0) root         (0)      225 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/logo.pt
+-rw-rw-rw-   0 root         (0) root         (0)       70 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/modal-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/nav-divider.pt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/nav-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      692 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/nav-item.pt
+-rw-rw-rw-   0 root         (0) root         (0)      211 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/nav-menu.pt
+-rw-rw-rw-   0 root         (0) root         (0)      120 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/page-aside.pt
+-rw-rw-rw-   0 root         (0) root         (0)      172 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/page-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      554 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/page-nav.pt
+-rw-rw-rw-   0 root         (0) root         (0)       62 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/page-ribbon.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/site-search.pt
+-rw-rw-rw-   0 root         (0) root         (0)      154 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/toolbar.pt
+-rw-rw-rw-   0 root         (0) root         (0)      154 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/top-links.pt
+-rw-rw-rw-   0 root         (0) root         (0)      136 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/top-menu-item.pt
+-rw-rw-rw-   0 root         (0) root         (0)      519 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/top-menu.pt
+-rw-rw-rw-   0 root         (0) root         (0)      613 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/top-menus-group.pt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/top-tab.pt
+-rw-rw-rw-   0 root         (0) root         (0)      397 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/top-tabs.pt
+-rw-rw-rw-   0 root         (0) root         (0)      162 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/user-links.pt
+-rw-rw-rw-   0 root         (0) root         (0)      454 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/user-menu.pt
+-rw-rw-rw-   0 root         (0) root         (0)      206 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/version.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/toolbar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3113 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/toplinks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3642 2021-11-26 15:54:51.000000 pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/userlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6948 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4001 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      351 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2021-11-26 15:55:07.000000 pyams_zmi-1.9.2/src/pyams_zmi.egg-info/top_level.txt
```

### Comparing `pyams_zmi-1.9.0/PKG-INFO` & `pyams_zmi-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_zmi
-Version: 1.9.0
+Version: 1.9.2
 Summary: PyAMS management interface package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Description: =================
         PyAMS_zmi package
@@ -38,14 +38,22 @@
         This package is using many content providers and viewlet managers (including in forms), so it can
         be extended easily by extensions packages without having to modify existing code.
         
         
         Changelog
         =========
         
+        1.9.2
+        -----
+         - package version mismatch
+        
+        1.9.1
+        -----
+         - updated user profile theme selection checker to handle empty profiles
+        
         1.9.0
         -----
          - added MyAMS dark theme support
          - added custom breadcrumbs viewlet template
          - added user profile management
          - added support for user selection of graphical theme
          - updated default toolbar add menu status
```

### Comparing `pyams_zmi-1.9.0/docs/HISTORY.txt` & `pyams_zmi-1.9.2/docs/HISTORY.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.9.2
+-----
+ - package version mismatch
+
+1.9.1
+-----
+ - updated user profile theme selection checker to handle empty profiles
+
 1.9.0
 -----
  - added MyAMS dark theme support
  - added custom breadcrumbs viewlet template
  - added user profile management
  - added support for user selection of graphical theme
  - updated default toolbar add menu status
```

### Comparing `pyams_zmi-1.9.0/docs/README.txt` & `pyams_zmi-1.9.2/docs/README.txt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/setup.py` & `pyams_zmi-1.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.txt')
 HISTORY = os.path.join(DOCS, 'HISTORY.txt')
 
-version = '1.9.0'
+version = '1.9.2'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_file',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/__init__.py` & `pyams_zmi-1.9.2/src/pyams_zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/configuration.py` & `pyams_zmi-1.9.2/src/pyams_zmi/configuration.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/doctests/README.rst` & `pyams_zmi-1.9.2/src/pyams_zmi/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/form.py` & `pyams_zmi-1.9.2/src/pyams_zmi/form.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/generations/__init__.py` & `pyams_zmi-1.9.2/src/pyams_zmi/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/generations/zodbupdate.py` & `pyams_zmi-1.9.2/src/pyams_zmi/generations/zodbupdate.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/helper/__init__.py` & `pyams_zmi-1.9.2/src/pyams_zmi/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/helper/container.py` & `pyams_zmi-1.9.2/src/pyams_zmi/helper/container.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/helper/event.py` & `pyams_zmi-1.9.2/src/pyams_zmi/helper/event.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/include.py` & `pyams_zmi-1.9.2/src/pyams_zmi/include.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/__init__.py` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/configuration.py` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/configuration.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/form.py` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/form.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/profile.py` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/table.py` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/table.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/admin-layout.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/admin-layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form-checker.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form-checker.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form-display.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form-group.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form-group.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form-switcher.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form-switcher.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form-tabform.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form-tabform.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/form.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/form.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/inner-table.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/inner-table.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/table-empty.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/table-empty.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/table-multiple.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/table-multiple.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/templates/table.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/templates/table.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/interfaces/viewlet.py` & `pyams_zmi-1.9.2/src/pyams_zmi/interfaces/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.mo` & `pyams_zmi-1.9.2/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.mo`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.po` & `pyams_zmi-1.9.2/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.po`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/locales/pyams_zmi.pot` & `pyams_zmi-1.9.2/src/pyams_zmi/locales/pyams_zmi.pot`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/profile.py` & `pyams_zmi-1.9.2/src/pyams_zmi/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/search.py` & `pyams_zmi-1.9.2/src/pyams_zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/skin.py` & `pyams_zmi-1.9.2/src/pyams_zmi/skin.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/table.py` & `pyams_zmi-1.9.2/src/pyams_zmi/table.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/tests/__init__.py` & `pyams_zmi-1.9.2/src/pyams_zmi/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/tests/test_utilsdocs.py` & `pyams_zmi-1.9.2/src/pyams_zmi/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/tests/test_utilsdocstrings.py` & `pyams_zmi-1.9.2/src/pyams_zmi/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/utils.py` & `pyams_zmi-1.9.2/src/pyams_zmi/utils.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/view.py` & `pyams_zmi-1.9.2/src/pyams_zmi/view.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/__init__.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/breadcrumb.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/configuration.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/configuration.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/controlpanel.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/controlpanel.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/environment.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/environment.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/interfaces.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/metas.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/metas.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/profile.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/registry.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/registry.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/resources.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         configuration = IZMIConfiguration(request.root, None)
         if configuration is not None:
             # yield main bundle
             bundle = None
             if configuration.user_bundle_selection:
                 profile = IUserProfile(self.request.principal, None)
                 if profile is not None:
-                    bundle, _label = MYAMS_BUNDLES.get(profile.zmi_bundle)
+                    bundle, _label = MYAMS_BUNDLES.get(profile.zmi_bundle, (None, None))
             if bundle is None:
                 bundle, _label = MYAMS_BUNDLES.get(configuration.myams_bundle)
             yield bundle
             # yield stylesheet
             stylesheet = configuration.custom_stylesheet
             if stylesheet:
                 modified = IZopeDublinCore(stylesheet).modified
```

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/skin.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/skin.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/timezone.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/timezone.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/__init__.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/aside.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/aside.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/breadcrumb.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/header.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/header.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/logo.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/logo.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/menu.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/menu.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/nav.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/nav.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/ribbon.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/ribbon.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/search.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/search.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/nav-item.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/nav-item.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/page-nav.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/page-nav.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/site-search.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/site-search.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/top-menu.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/top-menu.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/templates/top-menus-group.pt` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/templates/top-menus-group.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/toolbar.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/toplinks.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/toplinks.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi/zmi/viewlet/userlinks.py` & `pyams_zmi-1.9.2/src/pyams_zmi/zmi/viewlet/userlinks.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi.egg-info/PKG-INFO` & `pyams_zmi-1.9.2/src/pyams_zmi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-zmi
-Version: 1.9.0
+Version: 1.9.2
 Summary: PyAMS management interface package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Description: =================
         PyAMS_zmi package
@@ -38,14 +38,22 @@
         This package is using many content providers and viewlet managers (including in forms), so it can
         be extended easily by extensions packages without having to modify existing code.
         
         
         Changelog
         =========
         
+        1.9.2
+        -----
+         - package version mismatch
+        
+        1.9.1
+        -----
+         - updated user profile theme selection checker to handle empty profiles
+        
         1.9.0
         -----
          - added MyAMS dark theme support
          - added custom breadcrumbs viewlet template
          - added user profile management
          - added support for user selection of graphical theme
          - updated default toolbar add menu status
```

### Comparing `pyams_zmi-1.9.0/src/pyams_zmi.egg-info/SOURCES.txt` & `pyams_zmi-1.9.2/src/pyams_zmi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

