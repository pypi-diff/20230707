# Comparing `tmp/pyams_skin-1.8.4.tar.gz` & `tmp/pyams_skin-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_skin-1.8.4.tar", last modified: Mon Feb  6 13:32:00 2023, max compression
+gzip compressed data, was "dist/pyams_skin-1.9.0.tar", last modified: Sun Feb 19 13:33:49 2023, max compression
```

## Comparing `pyams_skin-1.8.4.tar` & `pyams_skin-1.9.0.tar`

### file list

```diff
@@ -1,128 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4626 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/docs/
--rwxrwxrwx   0 root         (0) root         (0)     3064 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2398 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    20789 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2445 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/doctests/metas.rst
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     1408 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1651 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/form.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/metas.py
--rw-rw-rw-   0 root         (0) root         (0)     3018 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/bootstrap-devices-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/bootstrap-devices-input.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/bootstrap-selection-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/bootstrap-selection-input.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/button-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1289 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/button-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/checkbox-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/checkbox-input.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/close-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      902 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/close-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/date-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/date-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/dates-range-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/dates-range-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1474 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/datetime-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     2018 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/datetime-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/form-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1673 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/form-group.pt
--rw-rw-rw-   0 root         (0) root         (0)     1393 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/form-tabform.pt
--rw-rw-rw-   0 root         (0) root         (0)     2918 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/form.pt
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/fullpage-modal-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/html-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/html-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/http-method-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/http-method-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/inner-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/modal-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1035 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/object-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/object-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/object-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/ordered-list-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      754 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/ordered-list-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/ordered-select-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      918 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/password-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/password-input.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/reset-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      878 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/reset-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1209 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/select-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1395 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/select-input.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/submit-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1005 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/submit-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/text-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/text-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/textarea-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/textarea-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/textlines-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/textlines-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1500 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/time-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     2041 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/time-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      787 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/widget-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1695 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/view.py
--rw-rw-rw-   0 root         (0) root         (0)     4891 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/viewlet.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/interfaces/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1137 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.mo
--rw-rw-rw-   0 root         (0) root         (0)     4121 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.po
--rw-rw-rw-   0 root         (0) root         (0)     2101 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/locales/pyams_skin.pot
--rw-rw-rw-   0 root         (0) root         (0)     3620 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/metas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/schema/
--rw-rw-rw-   0 root         (0) root         (0)     3450 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/schema/button.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/tests/
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     2621 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/breadcrumb.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/footer.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/header.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/help.py
--rw-rw-rw-   0 root         (0) root         (0)     2278 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/menu.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/metas.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/prefix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/action.pt
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/actions-menu.pt
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/actions.pt
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/alert.pt
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/breadcrumbs.pt
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/menu-divider.pt
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/menu-dropdown.pt
--rw-rw-rw-   0 root         (0) root         (0)      452 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/menu-item.pt
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/widget.pt
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/viewlet/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin/widget/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1146 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/widget/bool.py
--rw-rw-rw-   0 root         (0) root         (0)     5420 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/widget/bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/widget/button.py
--rw-rw-rw-   0 root         (0) root         (0)     4543 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/widget/datetime.py
--rw-rw-rw-   0 root         (0) root         (0)     2586 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/widget/html.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/widget/http.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/widget/list.py
--rw-rw-rw-   0 root         (0) root         (0)     3106 2023-02-06 13:31:38.000000 pyams_skin-1.8.4/src/pyams_skin/widget/select.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4626 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4819 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      173 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-06 13:32:00.000000 pyams_skin-1.8.4/src/pyams_skin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4714 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     3152 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2398 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    21998 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2445 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/doctests/metas.rst
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1651 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/metas.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/bootstrap-devices-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/bootstrap-devices-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/bootstrap-selection-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/bootstrap-selection-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/button-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/button-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/checkbox-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/checkbox-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/close-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      902 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/close-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/date-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/date-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/dates-range-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/dates-range-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/datetime-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/datetime-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/form-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/form-group.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/form-tabform.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2918 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/form.pt
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/fullpage-modal-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/html-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/html-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/http-method-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/http-method-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/inner-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/modal-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/object-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/object-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/object-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/ordered-list-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      754 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/ordered-list-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/ordered-select-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      918 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/password-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/password-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/reset-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/reset-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/select-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1395 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/select-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/submit-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/submit-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/text-copy-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/text-copy-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/text-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/text-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/textarea-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/textarea-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/textlines-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/textlines-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/time-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/time-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      787 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/widget-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1695 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/view.py
+-rw-rw-rw-   0 root         (0) root         (0)     4891 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/viewlet.py
+-rw-rw-rw-   0 root         (0) root         (0)    10695 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/interfaces/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.mo
+-rw-rw-rw-   0 root         (0) root         (0)     4317 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.po
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/locales/pyams_skin.pot
+-rw-rw-rw-   0 root         (0) root         (0)     3620 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/metas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/schema/button.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2621 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/breadcrumb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/footer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/help.py
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/menu.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/metas.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/prefix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/action.pt
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/actions-menu.pt
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/actions.pt
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/alert.pt
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/breadcrumbs.pt
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/menu-divider.pt
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/menu-dropdown.pt
+-rw-rw-rw-   0 root         (0) root         (0)      452 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/menu-item.pt
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/widget.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/viewlet/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/widget/bool.py
+-rw-rw-rw-   0 root         (0) root         (0)     5420 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/widget/bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/widget/button.py
+-rw-rw-rw-   0 root         (0) root         (0)     4543 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/widget/datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/widget/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/widget/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/widget/list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/widget/select.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-02-19 13:33:25.000000 pyams_skin-1.9.0/src/pyams_skin/widget/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4714 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4961 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      173 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-02-19 13:33:49.000000 pyams_skin-1.9.0/src/pyams_skin.egg-info/top_level.txt
```

### Comparing `pyams_skin-1.8.4/LICENSE` & `pyams_skin-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/PKG-INFO` & `pyams_skin-1.9.0/src/pyams_skin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_skin
-Version: 1.8.4
+Name: pyams-skin
+Version: 1.9.0
 Summary: PyAMS base skin management features
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -47,14 +47,18 @@
 It also provides a small set of custom form widgets and buttons, and overrides default templates
 of many widgets provided by PyAMS_form package.
 
 
 Changelog
 =========
 
+1.9.0
+-----
+ - added new textline widgets with button to copy input value to clipboard
+
 1.8.4
 -----
  - updated default field management of Bootstrap thumbnails selection field to be able to
    set default column width for each device
 
 1.8.3
 -----
```

### Comparing `pyams_skin-1.8.4/docs/HISTORY.rst` & `pyams_skin-1.9.0/docs/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+1.9.0
+-----
+ - added new textline widgets with button to copy input value to clipboard
+
 1.8.4
 -----
  - updated default field management of Bootstrap thumbnails selection field to be able to
    set default column width for each device
 
 1.8.3
 -----
```

### Comparing `pyams_skin-1.8.4/docs/README.rst` & `pyams_skin-1.9.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/setup.py` & `pyams_skin-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.8.4'
+version = '1.9.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_skin-1.8.4/src/pyams_skin/__init__.py` & `pyams_skin-1.9.0/src/pyams_skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/doctests/README.rst` & `pyams_skin-1.9.0/src/pyams_skin/doctests/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -143,14 +143,15 @@
 
     >>> from zope.schema import Tuple, TextLine, Date, Time, Datetime, Choice
     >>> from zope.schema.vocabulary import SimpleVocabulary
     >>> from pyams_utils.schema import HTTPMethodField, HTMLField
     >>> from pyams_skin.schema import BootstrapThumbnailsSelectionField, BootstrapDevicesBooleanField
 
     >>> class IMyContent(Interface):
+    ...     textline_field = TextLine(title="Textline field")
     ...     list_field = Tuple(title="List field",
     ...                        value_type=TextLine())
     ...     http_method = HTTPMethodField(title="HTTP method")
     ...     html_field = HTMLField(title="HTML field")
     ...     date_field = Date(title="Date field")
     ...     time_field = Time(title="Time field")
     ...     datetime_field = Datetime(title="Datetime field")
@@ -164,14 +165,15 @@
     >>> from zope.interface import implementer
     >>> from zope.schema.fieldproperty import FieldProperty
 
     >>> @implementer(IMyContent)
     ... class MyContent:
     ...     __name__ = None
     ...     __parent__ = None
+    ...     textline_field = FieldProperty(IMyContent['textline_field'])
     ...     list_field = FieldProperty(IMyContent['list_field'])
     ...     http_method = FieldProperty(IMyContent['http_method'])
     ...     html_field = FieldProperty(IMyContent['html_field'])
     ...     date_field = FieldProperty(IMyContent['date_field'])
     ...     time_field = FieldProperty(IMyContent['time_field'])
     ...     datetime_field = FieldProperty(IMyContent['datetime_field'])
     ...     select_field = FieldProperty(IMyContent['select_field'])
@@ -212,14 +214,42 @@
     >>> from zope.interface import alsoProvides
     >>> from pyams_layer.interfaces import IPyAMSLayer
 
     >>> request = TestRequest(context=content)
     >>> alsoProvides(request, IPyAMSLayer)
 
 
+Text widget with clipboard copy
+-------------------------------
+
+This widget can be used to copy input value to clipboard:
+
+    >>> from pyams_skin.widget.text import TextCopyFieldWidget
+    >>> text_widget = TextCopyFieldWidget(IMyContent['textline_field'], request)
+    >>> text_widget.update()
+    >>> print(text_widget.render())
+    <div class="input-group"
+         data-ams-modules="clipboard"
+         data-target-input="nearest">
+        <input type="text"
+                   id="textline_field"
+                   name="textline_field"
+                   class="form-control text-widget required textline-field"
+                   value="" />
+        <div class="input-group-append">
+                <div class="input-group-text hint"
+                           data-original-title="Copy value to clipboard"
+                           data-ams-click-handler="MyAMS.clipboard.copyText"
+                           data-ams-clipboard-target="#textline_field">
+                        <i class="far fa-clipboard"></i>
+                </div>
+        </div>
+    </div>
+
+
 Ordered list widget
 ...................
 
     >>> from pyams_skin.widget.list import OrderedListFieldWidget
     >>> list_widget = OrderedListFieldWidget(IMyContent['list_field'], request)
     >>> list_widget.extract()
     <NO_VALUE>
```

### Comparing `pyams_skin-1.8.4/src/pyams_skin/doctests/metas.rst` & `pyams_skin-1.9.0/src/pyams_skin/doctests/metas.rst`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/include.py` & `pyams_skin-1.9.0/src/pyams_skin/include.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/__init__.py` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/form.py` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/form.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/metas.py` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/metas.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/schema.py` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/bootstrap-devices-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/bootstrap-devices-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/bootstrap-devices-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/bootstrap-devices-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/bootstrap-selection-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/bootstrap-selection-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/button-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/button-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/close-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/close-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/date-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/date-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/date-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/date-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/dates-range-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/dates-range-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/datetime-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/datetime-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/datetime-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/datetime-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/form-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/form-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/form-group.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/form-group.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/form-tabform.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/form-tabform.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/form.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/form.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/html-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/html-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/http-method-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/http-method-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/http-method-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/http-method-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/modal-layout.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/modal-layout.pt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <div class="modal-dialog ${view.modal_class | ''}">
 	<div class="modal-content">
 		<div class="modal-header">
 			<div tal:define="header provider:pyams.header"
 				 tal:condition="header">
-				<i tal:omit-tag="">${structure:provider:pyams.header}</i>
+				<i tal:omit-tag="">${structure:header}</i>
 			</div>
 			<button type="button" class="close"
 					data-dismiss="modal" aria-label="Close">
 				<i class="far fa-times-circle" aria-hidden="true"></i>
 			</button>
 		</div>
 		<div class="modal-body p-0">
```

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/object-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/object-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/object-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/object-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/ordered-list-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/ordered-list-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/ordered-select-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/ordered-select-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/password-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/password-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/password-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/password-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/reset-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/reset-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/select-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/select-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/select-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/select-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/submit-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/submit-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/text-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/text-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/text-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/text-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/textarea-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/textarea-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/textlines-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/textlines-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/textlines-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/textlines-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/time-display.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/time-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/time-input.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/time-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/templates/widget-layout.pt` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/templates/widget-layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/view.py` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/view.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/viewlet.py` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/interfaces/widget.py` & `pyams_skin-1.9.0/src/pyams_skin/interfaces/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,22 @@
                          mode=INPUT_MODE,
                          template='templates/text-input.pt', layer=IPyAMSLayer)
 override_widget_template(ITextWidget,
                          mode=DISPLAY_MODE,
                          template='templates/text-display.pt', layer=IPyAMSLayer)
 
 
+@widget_template_config(mode=INPUT_MODE,
+                        template='templates/text-copy-input.pt', layer=IPyAMSLayer)
+@widget_template_config(mode=DISPLAY_MODE,
+                        template='templates/text-copy-display.pt', layer=IPyAMSLayer)
+class ITextCopyWidget(ITextWidget):
+    """Text widget with copy button"""
+
+
 override_widget_template(ITextAreaWidget,
                          mode=INPUT_MODE,
                          template='templates/textarea-input.pt', layer=IPyAMSLayer)
 override_widget_template(ITextAreaWidget,
                          mode=DISPLAY_MODE,
                          template='templates/textarea-display.pt', layer=IPyAMSLayer)
```

### Comparing `pyams_skin-1.8.4/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.mo` & `pyams_skin-1.9.0/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -15,14 +15,17 @@
 
 msgid "Back to previous page"
 msgstr "Revenir à la page précédente"
 
 msgid "Cols width"
 msgstr "Largeur des colonnes"
 
+msgid "Copy value to clipboard"
+msgstr "Copier dans le presse-papiers"
+
 msgid "Extra large screens"
 msgstr "Sur très grands écrans"
 
 msgid "Large screens"
 msgstr "Sur grands écrans"
 
 msgid "Medium screens"
```

### Comparing `pyams_skin-1.8.4/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.po` & `pyams_skin-1.9.0/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.po`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2022-09-09 18:13+0200\n"
+"POT-Creation-Date: 2023-02-19 01:41+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -65,14 +65,19 @@
 msgid "(no selection)"
 msgstr "(pas de sélection)"
 
 #: src/pyams_skin/interfaces/templates/form.pt:10
 msgid "Back to previous page"
 msgstr "Revenir à la page précédente"
 
+#: src/pyams_skin/interfaces/templates/text-copy-input.pt:39
+#: src/pyams_skin/interfaces/templates/text-copy-display.pt:39
+msgid "Copy value to clipboard"
+msgstr "Copier dans le presse-papiers"
+
 #: src/pyams_skin/interfaces/templates/dates-range-input.pt:7
 msgid "from"
 msgstr "à partir du"
 
 #: src/pyams_skin/interfaces/templates/dates-range-input.pt:9
 msgid "to"
 msgstr "et avant le"
```

### Comparing `pyams_skin-1.8.4/src/pyams_skin/locales/pyams_skin.pot` & `pyams_skin-1.9.0/src/pyams_skin/locales/pyams_skin.pot`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2022-09-09 18:13+0200\n"
+"POT-Creation-Date: 2023-02-19 01:41+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -65,14 +65,19 @@
 msgid "(no selection)"
 msgstr ""
 
 #: ./src/pyams_skin/interfaces/templates/form.pt:10
 msgid "Back to previous page"
 msgstr ""
 
+#: ./src/pyams_skin/interfaces/templates/text-copy-input.pt:39
+#: ./src/pyams_skin/interfaces/templates/text-copy-display.pt:39
+msgid "Copy value to clipboard"
+msgstr ""
+
 #: ./src/pyams_skin/interfaces/templates/dates-range-input.pt:7
 msgid "from"
 msgstr ""
 
 #: ./src/pyams_skin/interfaces/templates/dates-range-input.pt:9
 msgid "to"
 msgstr ""
```

### Comparing `pyams_skin-1.8.4/src/pyams_skin/metas.py` & `pyams_skin-1.9.0/src/pyams_skin/metas.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/schema/__init__.py` & `pyams_skin-1.9.0/src/pyams_skin/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/schema/button.py` & `pyams_skin-1.9.0/src/pyams_skin/schema/button.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/tests/__init__.py` & `pyams_skin-1.9.0/src/pyams_skin/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/tests/test_utilsdocs.py` & `pyams_skin-1.9.0/src/pyams_skin/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/tests/test_utilsdocstrings.py` & `pyams_skin-1.9.0/src/pyams_skin/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/__init__.py` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/actions.py` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/actions.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/breadcrumb.py` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/footer.py` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/footer.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/header.py` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/header.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/help.py` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/help.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/menu.py` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/menu.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/metas.py` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/metas.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/prefix.py` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/prefix.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/templates/action.pt` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/templates/action.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/viewlet/widget.py` & `pyams_skin-1.9.0/src/pyams_skin/viewlet/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/widget/__init__.py` & `pyams_skin-1.9.0/src/pyams_skin/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/widget/bool.py` & `pyams_skin-1.9.0/src/pyams_skin/widget/bool.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/widget/bootstrap.py` & `pyams_skin-1.9.0/src/pyams_skin/widget/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/widget/button.py` & `pyams_skin-1.9.0/src/pyams_skin/widget/button.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/widget/datetime.py` & `pyams_skin-1.9.0/src/pyams_skin/widget/datetime.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/widget/html.py` & `pyams_skin-1.9.0/src/pyams_skin/widget/html.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/widget/http.py` & `pyams_skin-1.9.0/src/pyams_skin/widget/http.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/widget/list.py` & `pyams_skin-1.9.0/src/pyams_skin/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin/widget/select.py` & `pyams_skin-1.9.0/src/pyams_skin/widget/select.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-1.8.4/src/pyams_skin.egg-info/PKG-INFO` & `pyams_skin-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams-skin
-Version: 1.8.4
+Name: pyams_skin
+Version: 1.9.0
 Summary: PyAMS base skin management features
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -47,14 +47,18 @@
 It also provides a small set of custom form widgets and buttons, and overrides default templates
 of many widgets provided by PyAMS_form package.
 
 
 Changelog
 =========
 
+1.9.0
+-----
+ - added new textline widgets with button to copy input value to clipboard
+
 1.8.4
 -----
  - updated default field management of Bootstrap thumbnails selection field to be able to
    set default column width for each device
 
 1.8.3
 -----
```

### Comparing `pyams_skin-1.8.4/src/pyams_skin.egg-info/SOURCES.txt` & `pyams_skin-1.9.0/src/pyams_skin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 src/pyams_skin/interfaces/templates/password-input.pt
 src/pyams_skin/interfaces/templates/reset-display.pt
 src/pyams_skin/interfaces/templates/reset-input.pt
 src/pyams_skin/interfaces/templates/select-display.pt
 src/pyams_skin/interfaces/templates/select-input.pt
 src/pyams_skin/interfaces/templates/submit-display.pt
 src/pyams_skin/interfaces/templates/submit-input.pt
+src/pyams_skin/interfaces/templates/text-copy-display.pt
+src/pyams_skin/interfaces/templates/text-copy-input.pt
 src/pyams_skin/interfaces/templates/text-display.pt
 src/pyams_skin/interfaces/templates/text-input.pt
 src/pyams_skin/interfaces/templates/textarea-display.pt
 src/pyams_skin/interfaces/templates/textarea-input.pt
 src/pyams_skin/interfaces/templates/textlines-display.pt
 src/pyams_skin/interfaces/templates/textlines-input.pt
 src/pyams_skin/interfaces/templates/time-display.pt
@@ -103,8 +105,9 @@
 src/pyams_skin/widget/bool.py
 src/pyams_skin/widget/bootstrap.py
 src/pyams_skin/widget/button.py
 src/pyams_skin/widget/datetime.py
 src/pyams_skin/widget/html.py
 src/pyams_skin/widget/http.py
 src/pyams_skin/widget/list.py
-src/pyams_skin/widget/select.py
+src/pyams_skin/widget/select.py
+src/pyams_skin/widget/text.py
```

