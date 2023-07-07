# Comparing `tmp/pyams_form-1.8.0.tar.gz` & `tmp/pyams_form-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_form-1.8.0.tar", last modified: Sun Feb 19 13:16:54 2023, max compression
+gzip compressed data, was "dist/pyams_form-1.8.1.tar", last modified: Fri Jul  7 15:06:17 2023, max compression
```

## Comparing `pyams_form-1.8.0.tar` & `pyams_form-1.8.1.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2021-05-31 01:04:48.000000 pyams_form-1.8.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2021-05-31 01:04:48.000000 pyams_form-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4600 2023-02-19 13:16:54.000000 pyams_form-1.8.0/PKG-INFO
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)     2841 2023-02-19 13:10:00.000000 pyams_form-1.8.0/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1215 2022-12-26 16:39:11.000000 pyams_form-1.8.0/docs/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1589 2021-05-31 01:04:48.000000 pyams_form-1.8.0/docs/form-graph.dot
--rw-rw-rw-   0 root         (0) root         (0)    11877 2021-05-31 01:04:48.000000 pyams_form-1.8.0/docs/form-graph.png
--rw-rw-rw-   0 root         (0) root         (0)     1510 2021-05-31 01:04:48.000000 pyams_form-1.8.0/docs/widget-graph.dot
--rw-rw-rw-   0 root         (0) root         (0)    13789 2021-05-31 01:04:48.000000 pyams_form-1.8.0/docs/widget-graph.png
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-19 13:16:54.000000 pyams_form-1.8.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2837 2023-02-19 13:10:00.000000 pyams_form-1.8.0/setup.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/
--rw-rw-rw-   0 root         (0) root         (0)      854 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/action.py
--rw-rw-rw-   0 root         (0) root         (0)    16892 2022-02-18 15:58:05.000000 pyams_form-1.8.0/src/pyams_form/ajax.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/browser/
--rw-rw-rw-   0 root         (0) root         (0)      892 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/button.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/checkbox.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/file.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/image.py
--rw-rw-rw-   0 root         (0) root         (0)    13085 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3801 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/multi.py
--rw-rw-rw-   0 root         (0) root         (0)     1421 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/object.py
--rw-rw-rw-   0 root         (0) root         (0)     3729 2022-04-16 16:43:17.000000 pyams_form-1.8.0/src/pyams_form/browser/orderedselect.py
--rw-rw-rw-   0 root         (0) root         (0)     1375 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/password.py
--rw-rw-rw-   0 root         (0) root         (0)     3745 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/radio.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/browser/resources/
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/browser/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)     3364 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/resources/js/orderedselect-input.js
--rw-rw-rw-   0 root         (0) root         (0)     1503 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/resources/js/orderedselect-input.min.js
--rw-rw-rw-   0 root         (0) root         (0)     5163 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/select.py
--rw-rw-rw-   0 root         (0) root         (0)     1518 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/submit.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/text.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/textarea.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/textlines.py
--rw-rw-rw-   0 root         (0) root         (0)     8027 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/browser/widget.py
--rw-rw-rw-   0 root         (0) root         (0)    11593 2023-02-19 13:10:00.000000 pyams_form-1.8.0/src/pyams_form/button.py
--rw-rw-rw-   0 root         (0) root         (0)     5383 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/contentprovider.py
--rw-rw-rw-   0 root         (0) root         (0)    16755 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/converter.py
--rw-rw-rw-   0 root         (0) root         (0)     5480 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/datamanager.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     3471 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     9810 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/action.rst
--rw-rw-rw-   0 root         (0) root         (0)    19164 2022-10-20 15:24:15.000000 pyams_form-1.8.0/src/pyams_form/doctests/ajax.rst
--rw-rw-rw-   0 root         (0) root         (0)   113044 2021-10-17 00:19:28.000000 pyams_form-1.8.0/src/pyams_form/doctests/browser.rst
--rw-rw-rw-   0 root         (0) root         (0)    19674 2021-07-13 11:35:55.000000 pyams_form-1.8.0/src/pyams_form/doctests/button.rst
--rw-rw-rw-   0 root         (0) root         (0)    10584 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/contentprovider.rst
--rw-rw-rw-   0 root         (0) root         (0)    32780 2021-07-13 11:35:55.000000 pyams_form-1.8.0/src/pyams_form/doctests/converter.rst
--rw-rw-rw-   0 root         (0) root         (0)    10500 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/datamanager.rst
--rw-rw-rw-   0 root         (0) root         (0)     8281 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/error.rst
--rw-rw-rw-   0 root         (0) root         (0)    30830 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/field.rst
--rw-rw-rw-   0 root         (0) root         (0)    65455 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/form.rst
--rw-rw-rw-   0 root         (0) root         (0)    33058 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/group.rst
--rw-rw-rw-   0 root         (0) root         (0)    26338 2021-10-17 00:19:28.000000 pyams_form-1.8.0/src/pyams_form/doctests/hint.rst
--rw-rw-rw-   0 root         (0) root         (0)      522 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/index-browser.rst
--rw-rw-rw-   0 root         (0) root         (0)      445 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2589 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/object-caveat.rst
--rw-rw-rw-   0 root         (0) root         (0)     6197 2022-02-18 15:58:05.000000 pyams_form-1.8.0/src/pyams_form/doctests/security.rst
--rw-rw-rw-   0 root         (0) root         (0)    38934 2022-10-20 15:24:15.000000 pyams_form-1.8.0/src/pyams_form/doctests/subform.rst
--rw-rw-rw-   0 root         (0) root         (0)    20861 2022-12-26 16:44:22.000000 pyams_form-1.8.0/src/pyams_form/doctests/term.rst
--rw-rw-rw-   0 root         (0) root         (0)     1466 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/testing.rst
--rw-rw-rw-   0 root         (0) root         (0)    15386 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/util.rst
--rw-rw-rw-   0 root         (0) root         (0)    20915 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/validator.rst
--rw-rw-rw-   0 root         (0) root         (0)     8357 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/value.rst
--rw-rw-rw-   0 root         (0) root         (0)     2257 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-button.rst
--rw-rw-rw-   0 root         (0) root         (0)    12744 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-checkbox.rst
--rw-rw-rw-   0 root         (0) root         (0)     4496 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-file-testing.rst
--rw-rw-rw-   0 root         (0) root         (0)     3221 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-file.rst
--rw-rw-rw-   0 root         (0) root         (0)     2669 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-image.rst
--rw-rw-rw-   0 root         (0) root         (0)    21423 2022-04-16 16:43:17.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-multi-dict-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)    14042 2022-04-16 16:43:17.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-multi-list-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)    52089 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-multi.rst
--rw-rw-rw-   0 root         (0) root         (0)    20939 2022-04-16 16:43:17.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-object-multi-dict-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)    17704 2022-04-16 16:43:17.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-object-multi-list-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)     7548 2022-04-16 16:43:17.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-object-single-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)    39941 2021-09-12 09:17:30.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-object.rst
--rw-rw-rw-   0 root         (0) root         (0)    63174 2021-09-12 09:17:30.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-objectmulti.rst
--rw-rw-rw-   0 root         (0) root         (0)     8679 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-orderedselect.rst
--rw-rw-rw-   0 root         (0) root         (0)     2669 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-password.rst
--rw-rw-rw-   0 root         (0) root         (0)     9424 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-radio.rst
--rw-rw-rw-   0 root         (0) root         (0)     8172 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-select-missing-terms.rst
--rw-rw-rw-   0 root         (0) root         (0)     2997 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-select-source.rst
--rw-rw-rw-   0 root         (0) root         (0)    12593 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-select.rst
--rw-rw-rw-   0 root         (0) root         (0)     2482 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-submit.rst
--rw-rw-rw-   0 root         (0) root         (0)     2345 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-text.rst
--rw-rw-rw-   0 root         (0) root         (0)     2299 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-textarea.rst
--rw-rw-rw-   0 root         (0) root         (0)     2787 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget-textlines.rst
--rw-rw-rw-   0 root         (0) root         (0)    31086 2021-07-13 11:35:55.000000 pyams_form-1.8.0/src/pyams_form/doctests/widget.rst
--rw-rw-rw-   0 root         (0) root         (0)     4433 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/error.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2022-04-16 16:43:17.000000 pyams_form-1.8.0/src/pyams_form/events.py
--rw-rw-rw-   0 root         (0) root         (0)    13295 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/field.py
--rw-rw-rw-   0 root         (0) root         (0)    20194 2023-02-19 13:10:00.000000 pyams_form-1.8.0/src/pyams_form/form.py
--rw-rw-rw-   0 root         (0) root         (0)     4385 2023-02-19 13:10:00.000000 pyams_form-1.8.0/src/pyams_form/group.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/hint.py
--rw-rw-rw-   0 root         (0) root         (0)     1028 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/include.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     9914 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4651 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/button.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/error.py
--rw-rw-rw-   0 root         (0) root         (0)    13619 2023-02-19 13:10:00.000000 pyams_form-1.8.0/src/pyams_form/interfaces/form.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/
--rw-rw-rw-   0 root         (0) root         (0)      185 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/button-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      868 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/button-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      680 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/checkbox-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1183 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/checkbox-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)     2725 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/checkbox-input.pt
--rw-rw-rw-   0 root         (0) root         (0)       40 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/error.pt
--rw-rw-rw-   0 root         (0) root         (0)      563 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/file-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      931 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/file-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      205 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/image-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      892 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/image-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1701 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/multi-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      301 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/multi-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)     1849 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/multi-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      371 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/object-display.pt
--rw-rw-rw-   0 root         (0) root         (0)       93 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/object-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)      515 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/object-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      678 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/orderedselect-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     3266 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/orderedselect-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      563 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/password-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      975 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/password-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      674 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/radio-display-single.pt
--rw-rw-rw-   0 root         (0) root         (0)      680 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/radio-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      214 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/radio-hidden-single.pt
--rw-rw-rw-   0 root         (0) root         (0)       95 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/radio-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)      952 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/radio-input-single.pt
--rw-rw-rw-   0 root         (0) root         (0)      265 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/radio-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      680 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/select-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      283 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/select-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)     1087 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/select-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      185 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/submit-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      868 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/submit-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      480 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/text-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      211 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/text-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)     1008 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/text-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      480 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/textarea-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      185 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/textarea-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)      826 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/textarea-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      563 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/textlines-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      229 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/textlines-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)      986 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/textlines-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      243 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/widget-layout-display.pt
--rw-rw-rw-   0 root         (0) root         (0)       26 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/widget-layout-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)      408 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/templates/widget-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)    19108 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/interfaces/widget.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/locales/
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/locales/fr/
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    14287 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.mo
--rw-rw-rw-   0 root         (0) root         (0)    20915 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.po
--rw-rw-rw-   0 root         (0) root         (0)    15253 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/locales/pyams_form.pot
--rw-rw-rw-   0 root         (0) root         (0)    14307 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/object.py
--rw-rw-rw-   0 root         (0) root         (0)     4226 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/outputchecker.py
--rw-rw-rw-   0 root         (0) root         (0)     2969 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/subform.py
--rw-rw-rw-   0 root         (0) root         (0)     6836 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/template.py
--rw-rw-rw-   0 root         (0) root         (0)    11899 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/term.py
--rw-rw-rw-   0 root         (0) root         (0)    20278 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/testing.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/tests/
--rw-rw-rw-   0 root         (0) root         (0)      799 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/__init__.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/
--rw-rw-rw-   0 root         (0) root         (0)       95 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/custom-error.pt
--rw-rw-rw-   0 root         (0) root         (0)     1100 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/file-testing-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      651 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/integration-edit.pt
--rw-rw-rw-   0 root         (0) root         (0)      744 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-caredit-subforms.pt
--rw-rw-rw-   0 root         (0) root         (0)      709 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-caredit.pt
--rw-rw-rw-   0 root         (0) root         (0)       97 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1243 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-edit-with-providers.pt
--rw-rw-rw-   0 root         (0) root         (0)      744 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-edit-with-subforms.pt
--rw-rw-rw-   0 root         (0) root         (0)      628 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-edit.pt
--rw-rw-rw-   0 root         (0) root         (0)     1052 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-groupedit.pt
--rw-rw-rw-   0 root         (0) root         (0)      268 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1341 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-nested-groupedit.pt
--rw-rw-rw-   0 root         (0) root         (0)      584 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-owneredit.pt
--rw-rw-rw-   0 root         (0) root         (0)      482 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/templates/simple-subedit.pt
--rw-rw-rw-   0 root         (0) root         (0)     1836 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     8555 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/util.py
--rw-rw-rw-   0 root         (0) root         (0)     8061 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/validator.py
--rw-rw-rw-   0 root         (0) root         (0)     3006 2021-05-31 01:04:48.000000 pyams_form-1.8.0/src/pyams_form/value.py
--rw-rw-rw-   0 root         (0) root         (0)    24848 2021-07-13 11:35:55.000000 pyams_form-1.8.0/src/pyams_form/widget.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4600 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7239 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      344 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-19 13:16:54.000000 pyams_form-1.8.0/src/pyams_form.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 15:06:03.000000 pyams_form-1.8.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 15:06:03.000000 pyams_form-1.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-07-07 15:06:17.000000 pyams_form-1.8.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     2881 2023-07-07 15:06:03.000000 pyams_form-1.8.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2023-07-07 15:06:03.000000 pyams_form-1.8.1/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-07-07 15:06:03.000000 pyams_form-1.8.1/docs/form-graph.dot
+-rw-rw-rw-   0 root         (0) root         (0)    11877 2023-07-07 15:06:03.000000 pyams_form-1.8.1/docs/form-graph.png
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-07-07 15:06:03.000000 pyams_form-1.8.1/docs/widget-graph.dot
+-rw-rw-rw-   0 root         (0) root         (0)    13789 2023-07-07 15:06:03.000000 pyams_form-1.8.1/docs/widget-graph.png
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 15:06:17.000000 pyams_form-1.8.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2837 2023-07-07 15:06:03.000000 pyams_form-1.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/action.py
+-rw-rw-rw-   0 root         (0) root         (0)    16892 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/ajax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/browser/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/button.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/checkbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/image.py
+-rw-rw-rw-   0 root         (0) root         (0)    13085 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3801 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/multi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/object.py
+-rw-rw-rw-   0 root         (0) root         (0)     3729 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/orderedselect.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/password.py
+-rw-rw-rw-   0 root         (0) root         (0)     3745 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/radio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/browser/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/browser/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)     3364 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/resources/js/orderedselect-input.js
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/resources/js/orderedselect-input.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     5163 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/select.py
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/submit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/textarea.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/textlines.py
+-rw-rw-rw-   0 root         (0) root         (0)     8027 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/browser/widget.py
+-rw-rw-rw-   0 root         (0) root         (0)    11593 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/button.py
+-rw-rw-rw-   0 root         (0) root         (0)     5383 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/contentprovider.py
+-rw-rw-rw-   0 root         (0) root         (0)    16755 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/datamanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     3471 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9810 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/action.rst
+-rw-rw-rw-   0 root         (0) root         (0)    19164 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/ajax.rst
+-rw-rw-rw-   0 root         (0) root         (0)   113044 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/browser.rst
+-rw-rw-rw-   0 root         (0) root         (0)    19674 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/button.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10584 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/contentprovider.rst
+-rw-rw-rw-   0 root         (0) root         (0)    32780 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/converter.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10500 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/datamanager.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8281 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/error.rst
+-rw-rw-rw-   0 root         (0) root         (0)    30830 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/field.rst
+-rw-rw-rw-   0 root         (0) root         (0)    65455 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/form.rst
+-rw-rw-rw-   0 root         (0) root         (0)    33058 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/group.rst
+-rw-rw-rw-   0 root         (0) root         (0)    26338 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/hint.rst
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/index-browser.rst
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/object-caveat.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6197 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/security.rst
+-rw-rw-rw-   0 root         (0) root         (0)    38934 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/subform.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20861 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/term.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/testing.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15386 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/util.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20915 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/validator.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8357 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/value.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-button.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12744 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-checkbox.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-file-testing.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-file.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-image.rst
+-rw-rw-rw-   0 root         (0) root         (0)    21423 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-multi-dict-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14042 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-multi-list-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)    52089 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-multi.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20939 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-object-multi-dict-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17704 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-object-multi-list-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-object-single-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)    39953 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-object.rst
+-rw-rw-rw-   0 root         (0) root         (0)    63193 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-objectmulti.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-orderedselect.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-password.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9424 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-radio.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8172 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-select-missing-terms.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-select-source.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12593 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-select.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2482 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-submit.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-text.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-textarea.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget-textlines.rst
+-rw-rw-rw-   0 root         (0) root         (0)    31086 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/doctests/widget.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/events.py
+-rw-rw-rw-   0 root         (0) root         (0)    13295 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/field.py
+-rw-rw-rw-   0 root         (0) root         (0)    20194 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     4385 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/hint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     9914 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4651 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/button.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/error.py
+-rw-rw-rw-   0 root         (0) root         (0)    13619 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/form.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/button-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/button-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      680 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/checkbox-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/checkbox-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/checkbox-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/error.pt
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/file-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/file-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/image-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/image-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/multi-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/multi-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/multi-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      371 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/object-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/object-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/object-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/orderedselect-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3266 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/orderedselect-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/password-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/password-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/radio-display-single.pt
+-rw-rw-rw-   0 root         (0) root         (0)      680 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/radio-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/radio-hidden-single.pt
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/radio-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/radio-input-single.pt
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/radio-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      680 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/select-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/select-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/select-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/submit-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/submit-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/text-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/text-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/text-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/textarea-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/textarea-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/textarea-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/textlines-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/textlines-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/textlines-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/widget-layout-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/widget-layout-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/templates/widget-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)    19108 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/interfaces/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    14287 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.mo
+-rw-rw-rw-   0 root         (0) root         (0)    20915 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.po
+-rw-rw-rw-   0 root         (0) root         (0)    15253 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/locales/pyams_form.pot
+-rw-rw-rw-   0 root         (0) root         (0)    14307 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/object.py
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/outputchecker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/subform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6836 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/template.py
+-rw-rw-rw-   0 root         (0) root         (0)    11899 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/term.py
+-rw-rw-rw-   0 root         (0) root         (0)    20278 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/custom-error.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/file-testing-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/integration-edit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-caredit-subforms.pt
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-caredit.pt
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-edit-with-providers.pt
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-edit-with-subforms.pt
+-rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-edit.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-groupedit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-nested-groupedit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-owneredit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/templates/simple-subedit.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     8555 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     8061 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3006 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/value.py
+-rw-rw-rw-   0 root         (0) root         (0)    24867 2023-07-07 15:06:03.000000 pyams_form-1.8.1/src/pyams_form/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7239 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-07 15:06:17.000000 pyams_form-1.8.1/src/pyams_form.egg-info/top_level.txt
```

### Comparing `pyams_form-1.8.0/LICENSE` & `pyams_form-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/PKG-INFO` & `pyams_form-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_form
-Version: 1.8.0
+Version: 1.8.1
 Summary: PyAMS forms management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -50,14 +50,18 @@
 ** Package API is also converted to common Python standards, using snake_case for variables and
 methods.
 
 
 Changelog
 =========
 
+1.8.1
+-----
+ - small templates updates
+
 1.8.0
 -----
  - added support for optional *factory* argument when using *form_and_handler* decorator
  - added optional *notify* argument to form *extract_data* method; you can set this argument
    to *False* when you don't want to generate extra events on a manual data extraction
 
 1.7.4
```

### Comparing `pyams_form-1.8.0/docs/HISTORY.rst` & `pyams_form-1.8.1/docs/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+1.8.1
+-----
+ - small templates updates
+
 1.8.0
 -----
  - added support for optional *factory* argument when using *form_and_handler* decorator
  - added optional *notify* argument to form *extract_data* method; you can set this argument
    to *False* when you don't want to generate extra events on a manual data extraction
 
 1.7.4
```

### Comparing `pyams_form-1.8.0/docs/README.rst` & `pyams_form-1.8.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/docs/form-graph.dot` & `pyams_form-1.8.1/docs/form-graph.dot`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/docs/form-graph.png` & `pyams_form-1.8.1/docs/form-graph.png`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/docs/widget-graph.dot` & `pyams_form-1.8.1/docs/widget-graph.dot`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/docs/widget-graph.png` & `pyams_form-1.8.1/docs/widget-graph.png`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/setup.py` & `pyams_form-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.8.0'
+version = '1.8.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_i18n',
     'zc.sourcefactory',
     'zope.testing'
 ]
```

### Comparing `pyams_form-1.8.0/src/pyams_form/__init__.py` & `pyams_form-1.8.1/src/pyams_form/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/action.py` & `pyams_form-1.8.1/src/pyams_form/action.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/ajax.py` & `pyams_form-1.8.1/src/pyams_form/ajax.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/__init__.py` & `pyams_form-1.8.1/src/pyams_form/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/button.py` & `pyams_form-1.8.1/src/pyams_form/browser/button.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/checkbox.py` & `pyams_form-1.8.1/src/pyams_form/browser/checkbox.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/file.py` & `pyams_form-1.8.1/src/pyams_form/browser/file.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/image.py` & `pyams_form-1.8.1/src/pyams_form/browser/image.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/interfaces.py` & `pyams_form-1.8.1/src/pyams_form/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/multi.py` & `pyams_form-1.8.1/src/pyams_form/browser/multi.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/object.py` & `pyams_form-1.8.1/src/pyams_form/browser/object.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/orderedselect.py` & `pyams_form-1.8.1/src/pyams_form/browser/orderedselect.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/password.py` & `pyams_form-1.8.1/src/pyams_form/browser/password.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/radio.py` & `pyams_form-1.8.1/src/pyams_form/browser/radio.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/resources/js/orderedselect-input.js` & `pyams_form-1.8.1/src/pyams_form/browser/resources/js/orderedselect-input.js`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/resources/js/orderedselect-input.min.js` & `pyams_form-1.8.1/src/pyams_form/browser/resources/js/orderedselect-input.min.js`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/select.py` & `pyams_form-1.8.1/src/pyams_form/browser/select.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/submit.py` & `pyams_form-1.8.1/src/pyams_form/browser/submit.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/text.py` & `pyams_form-1.8.1/src/pyams_form/browser/text.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/textarea.py` & `pyams_form-1.8.1/src/pyams_form/browser/textarea.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/textlines.py` & `pyams_form-1.8.1/src/pyams_form/browser/textlines.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/browser/widget.py` & `pyams_form-1.8.1/src/pyams_form/browser/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/button.py` & `pyams_form-1.8.1/src/pyams_form/button.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/contentprovider.py` & `pyams_form-1.8.1/src/pyams_form/contentprovider.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/converter.py` & `pyams_form-1.8.1/src/pyams_form/converter.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/datamanager.py` & `pyams_form-1.8.1/src/pyams_form/datamanager.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/README.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/action.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/action.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/ajax.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/ajax.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/browser.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/browser.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/button.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/button.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/contentprovider.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/contentprovider.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/converter.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/converter.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/datamanager.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/datamanager.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/error.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/error.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/field.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/field.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/form.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/form.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/group.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/group.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/hint.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/hint.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/index-browser.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/index-browser.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/object-caveat.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/object-caveat.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/security.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/security.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/subform.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/subform.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/term.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/term.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/testing.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/testing.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/util.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/util.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/validator.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/validator.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/value.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/value.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-button.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-button.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-checkbox.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-checkbox.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-file-testing.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-file-testing.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-file.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-file.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-image.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-image.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-multi-dict-integration.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-multi-dict-integration.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-multi-list-integration.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-multi-list-integration.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-multi.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-multi.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-object-multi-dict-integration.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-object-multi-dict-integration.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-object-multi-list-integration.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-object-multi-list-integration.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-object-single-integration.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-object-single-integration.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-object.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-object.rst`

 * *Files 0% similar despite different names*

```diff
@@ -227,2271 +227,2272 @@
 00000e20: 742d 6669 656c 6422 0a20 2020 2020 2020  t-field".       
 00000e30: 2020 7661 6c75 653d 2232 2c32 3232 2220    value="2,222" 
 00000e40: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
 00000e50: 203c 2f64 6976 3e0a 2020 2020 2020 3c69   </div>.      <i
 00000e60: 6e70 7574 206e 616d 653d 2273 7562 6f62  nput name="subob
 00000e70: 6a65 6374 2d65 6d70 7479 2d6d 6172 6b65  ject-empty-marke
 00000e80: 7222 2074 7970 653d 2268 6964 6465 6e22  r" type="hidden"
-00000e90: 2076 616c 7565 3d22 3122 2f3e 0a20 203c   value="1"/>.  <
-00000ea0: 2f64 6976 3e0a 0a0a 4173 2079 6f75 2073  /div>...As you s
-00000eb0: 6565 2061 6c6c 2073 6f72 7420 6f66 2064  ee all sort of d
-00000ec0: 6566 6175 6c74 2076 616c 7565 7320 6172  efault values ar
-00000ed0: 6520 7265 6e64 6572 6564 2e0a 0a4c 6574  e rendered...Let
-00000ee0: 2773 2070 726f 7669 6465 2061 206d 6f72  's provide a mor
-00000ef0: 6520 6d65 616e 696e 6766 756c 2076 616c  e meaningful val
-00000f00: 7565 3a0a 0a20 203e 3e3e 2066 726f 6d20  ue:..  >>> from 
-00000f10: 7079 616d 735f 666f 726d 2e74 6573 7469  pyams_form.testi
-00000f20: 6e67 2069 6d70 6f72 7420 4d79 5375 624f  ng import MySubO
-00000f30: 626a 6563 740a 2020 3e3e 3e20 7620 3d20  bject.  >>> v = 
-00000f40: 4d79 5375 624f 626a 6563 7428 290a 2020  MySubObject().  
-00000f50: 3e3e 3e20 762e 666f 6f66 6965 6c64 203d  >>> v.foofield =
-00000f60: 2034 320a 2020 3e3e 3e20 762e 6261 7266   42.  >>> v.barf
-00000f70: 6965 6c64 203d 2036 3636 0a20 203e 3e3e  ield = 666.  >>>
-00000f80: 2076 2e5f 5f6d 6172 6b65 725f 5f20 3d20   v.__marker__ = 
-00000f90: 2254 6869 734d 7573 7453 7461 7954 6865  "ThisMustStayThe
-00000fa0: 5361 6d65 220a 0a0a 2020 3e3e 3e20 7769  Same"...  >>> wi
-00000fb0: 6467 6574 2e69 676e 6f72 655f 636f 6e74  dget.ignore_cont
-00000fc0: 6578 7420 3d20 4661 6c73 650a 2020 3e3e  ext = False.  >>
-00000fd0: 3e20 7769 6467 6574 2e76 616c 7565 203d  > widget.value =
-00000fe0: 2064 6963 7428 666f 6f66 6965 6c64 3d27   dict(foofield='
-00000ff0: 3432 272c 2062 6172 6669 656c 643d 2736  42', barfield='6
-00001000: 3636 2729 0a0a 2020 3e3e 3e20 7769 6467  66')..  >>> widg
-00001010: 6574 2e75 7064 6174 6528 290a 0a20 203e  et.update()..  >
-00001020: 3e3e 2070 7269 6e74 2866 6f72 6d61 745f  >> print(format_
-00001030: 6874 6d6c 2877 6964 6765 742e 7265 6e64  html(widget.rend
-00001040: 6572 2829 2929 0a20 203c 6469 7620 636c  er())).  <div cl
-00001050: 6173 733d 226f 626a 6563 742d 7769 6467  ass="object-widg
-00001060: 6574 2072 6571 7569 7265 6422 3e0a 2020  et required">.  
-00001070: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00001080: 2063 6c61 7373 3d22 6c61 6265 6c22 3e0a   class="label">.
-00001090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010a0: 2020 2020 2020 3c6c 6162 656c 2066 6f72        <label for
-000010b0: 3d22 7375 626f 626a 6563 742d 7769 6467  ="subobject-widg
-000010c0: 6574 732d 666f 6f66 6965 6c64 223e 0a20  ets-foofield">. 
+00000e90: 2076 616c 7565 3d22 3122 202f 3e0a 2020   value="1" />.  
+00000ea0: 3c2f 6469 763e 0a0a 0a41 7320 796f 7520  </div>...As you 
+00000eb0: 7365 6520 616c 6c20 736f 7274 206f 6620  see all sort of 
+00000ec0: 6465 6661 756c 7420 7661 6c75 6573 2061  default values a
+00000ed0: 7265 2072 656e 6465 7265 642e 0a0a 4c65  re rendered...Le
+00000ee0: 7427 7320 7072 6f76 6964 6520 6120 6d6f  t's provide a mo
+00000ef0: 7265 206d 6561 6e69 6e67 6675 6c20 7661  re meaningful va
+00000f00: 6c75 653a 0a0a 2020 3e3e 3e20 6672 6f6d  lue:..  >>> from
+00000f10: 2070 7961 6d73 5f66 6f72 6d2e 7465 7374   pyams_form.test
+00000f20: 696e 6720 696d 706f 7274 204d 7953 7562  ing import MySub
+00000f30: 4f62 6a65 6374 0a20 203e 3e3e 2076 203d  Object.  >>> v =
+00000f40: 204d 7953 7562 4f62 6a65 6374 2829 0a20   MySubObject(). 
+00000f50: 203e 3e3e 2076 2e66 6f6f 6669 656c 6420   >>> v.foofield 
+00000f60: 3d20 3432 0a20 203e 3e3e 2076 2e62 6172  = 42.  >>> v.bar
+00000f70: 6669 656c 6420 3d20 3636 360a 2020 3e3e  field = 666.  >>
+00000f80: 3e20 762e 5f5f 6d61 726b 6572 5f5f 203d  > v.__marker__ =
+00000f90: 2022 5468 6973 4d75 7374 5374 6179 5468   "ThisMustStayTh
+00000fa0: 6553 616d 6522 0a0a 0a20 203e 3e3e 2077  eSame"...  >>> w
+00000fb0: 6964 6765 742e 6967 6e6f 7265 5f63 6f6e  idget.ignore_con
+00000fc0: 7465 7874 203d 2046 616c 7365 0a20 203e  text = False.  >
+00000fd0: 3e3e 2077 6964 6765 742e 7661 6c75 6520  >> widget.value 
+00000fe0: 3d20 6469 6374 2866 6f6f 6669 656c 643d  = dict(foofield=
+00000ff0: 2734 3227 2c20 6261 7266 6965 6c64 3d27  '42', barfield='
+00001000: 3636 3627 290a 0a20 203e 3e3e 2077 6964  666')..  >>> wid
+00001010: 6765 742e 7570 6461 7465 2829 0a0a 2020  get.update()..  
+00001020: 3e3e 3e20 7072 696e 7428 666f 726d 6174  >>> print(format
+00001030: 5f68 746d 6c28 7769 6467 6574 2e72 656e  _html(widget.ren
+00001040: 6465 7228 2929 290a 2020 3c64 6976 2063  der())).  <div c
+00001050: 6c61 7373 3d22 6f62 6a65 6374 2d77 6964  lass="object-wid
+00001060: 6765 7420 7265 7175 6972 6564 223e 0a20  get required">. 
+00001070: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00001080: 7620 636c 6173 733d 226c 6162 656c 223e  v class="label">
+00001090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000010a0: 2020 2020 2020 203c 6c61 6265 6c20 666f         <label fo
+000010b0: 723d 2273 7562 6f62 6a65 6374 2d77 6964  r="subobject-wid
+000010c0: 6765 7473 2d66 6f6f 6669 656c 6422 3e0a  gets-foofield">.
 000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010e0: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
-000010f0: 616e 3e4d 7920 666f 6f20 6669 656c 643c  an>My foo field<
-00001100: 2f73 7061 6e3e 0a20 2020 2020 2020 2020  /span>.         
+000010e0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+000010f0: 7061 6e3e 4d79 2066 6f6f 2066 6965 6c64  pan>My foo field
+00001100: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
 00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001120: 2020 2020 203c 7370 616e 2063 6c61 7373       <span class
-00001130: 3d22 7265 7175 6972 6564 223e 2a3c 2f73  ="required">*</s
-00001140: 7061 6e3e 0a20 2020 2020 2020 2020 2020  pan>.           
-00001150: 2020 2020 2020 2020 2020 203c 2f6c 6162             </lab
-00001160: 656c 3e0a 2020 2020 2020 2020 2020 2020  el>.            
-00001170: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00001180: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00001190: 733d 2277 6964 6765 7422 3e0a 2020 2020  s="widget">.    
+00001120: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
+00001130: 733d 2272 6571 7569 7265 6422 3e2a 3c2f  s="required">*</
+00001140: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
+00001150: 2020 2020 2020 2020 2020 2020 3c2f 6c61              </la
+00001160: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
+00001170: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00001180: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00001190: 7373 3d22 7769 6467 6574 223e 0a20 2020  ss="widget">.   
 000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011b0: 2020 3c69 6e70 7574 2074 7970 653d 2274    <input type="t
-000011c0: 6578 7422 0a20 2020 2020 2020 2020 6964  ext".         id
-000011d0: 3d22 7375 626f 626a 6563 742d 7769 6467  ="subobject-widg
-000011e0: 6574 732d 666f 6f66 6965 6c64 220a 2020  ets-foofield".  
-000011f0: 2020 2020 2020 206e 616d 653d 2273 7562         name="sub
-00001200: 6f62 6a65 6374 2e77 6964 6765 7473 2e66  object.widgets.f
-00001210: 6f6f 6669 656c 6422 0a20 2020 2020 2020  oofield".       
-00001220: 2020 636c 6173 733d 2274 6578 742d 7769    class="text-wi
-00001230: 6467 6574 2072 6571 7569 7265 6420 696e  dget required in
-00001240: 742d 6669 656c 6422 0a20 2020 2020 2020  t-field".       
-00001250: 2020 7661 6c75 653d 2234 3222 202f 3e0a    value="42" />.
-00001260: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001270: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00001280: 2020 203c 6469 7620 636c 6173 733d 226c     <div class="l
-00001290: 6162 656c 223e 0a20 2020 2020 2020 2020  abel">.         
-000012a0: 2020 2020 2020 2020 2020 2020 203c 6c61               <la
-000012b0: 6265 6c20 666f 723d 2273 7562 6f62 6a65  bel for="subobje
-000012c0: 6374 2d77 6964 6765 7473 2d62 6172 6669  ct-widgets-barfi
-000012d0: 656c 6422 3e0a 2020 2020 2020 2020 2020  eld">.          
+000011b0: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
+000011c0: 7465 7874 220a 2020 2020 2020 2020 2069  text".         i
+000011d0: 643d 2273 7562 6f62 6a65 6374 2d77 6964  d="subobject-wid
+000011e0: 6765 7473 2d66 6f6f 6669 656c 6422 0a20  gets-foofield". 
+000011f0: 2020 2020 2020 2020 6e61 6d65 3d22 7375          name="su
+00001200: 626f 626a 6563 742e 7769 6467 6574 732e  bobject.widgets.
+00001210: 666f 6f66 6965 6c64 220a 2020 2020 2020  foofield".      
+00001220: 2020 2063 6c61 7373 3d22 7465 7874 2d77     class="text-w
+00001230: 6964 6765 7420 7265 7175 6972 6564 2069  idget required i
+00001240: 6e74 2d66 6965 6c64 220a 2020 2020 2020  nt-field".      
+00001250: 2020 2076 616c 7565 3d22 3432 2220 2f3e     value="42" />
+00001260: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00001270: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00001280: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00001290: 6c61 6265 6c22 3e0a 2020 2020 2020 2020  label">.        
+000012a0: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
+000012b0: 6162 656c 2066 6f72 3d22 7375 626f 626a  abel for="subobj
+000012c0: 6563 742d 7769 6467 6574 732d 6261 7266  ect-widgets-barf
+000012d0: 6965 6c64 223e 0a20 2020 2020 2020 2020  ield">.         
 000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2020 2020 3c73 7061 6e3e 4d79 2064 6561      <span>My dea
-00001300: 7220 6261 723c 2f73 7061 6e3e 0a20 2020  r bar</span>.   
+000012f0: 2020 2020 203c 7370 616e 3e4d 7920 6465       <span>My de
+00001300: 6172 2062 6172 3c2f 7370 616e 3e0a 2020  ar bar</span>.  
 00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001320: 2020 203c 2f6c 6162 656c 3e0a 2020 2020     </label>.    
-00001330: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00001340: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00001350: 6469 7620 636c 6173 733d 2277 6964 6765  div class="widge
-00001360: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-00001370: 2020 2020 2020 2020 2020 3c69 6e70 7574            <input
-00001380: 2074 7970 653d 2274 6578 7422 0a20 2020   type="text".   
-00001390: 2020 2020 2020 6964 3d22 7375 626f 626a        id="subobj
-000013a0: 6563 742d 7769 6467 6574 732d 6261 7266  ect-widgets-barf
-000013b0: 6965 6c64 220a 2020 2020 2020 2020 206e  ield".         n
-000013c0: 616d 653d 2273 7562 6f62 6a65 6374 2e77  ame="subobject.w
-000013d0: 6964 6765 7473 2e62 6172 6669 656c 6422  idgets.barfield"
-000013e0: 0a20 2020 2020 2020 2020 636c 6173 733d  .         class=
-000013f0: 2274 6578 742d 7769 6467 6574 2069 6e74  "text-widget int
-00001400: 2d66 6965 6c64 220a 2020 2020 2020 2020  -field".        
-00001410: 2076 616c 7565 3d22 3636 3622 202f 3e0a   value="666" />.
-00001420: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001430: 6469 763e 0a20 2020 2020 203c 696e 7075  div>.      <inpu
-00001440: 7420 6e61 6d65 3d22 7375 626f 626a 6563  t name="subobjec
-00001450: 742d 656d 7074 792d 6d61 726b 6572 2220  t-empty-marker" 
-00001460: 7479 7065 3d22 6869 6464 656e 2220 7661  type="hidden" va
-00001470: 6c75 653d 2231 222f 3e0a 2020 3c2f 6469  lue="1"/>.  </di
-00001480: 763e 0a0a 0a54 6865 2077 6964 6765 7427  v>...The widget'
-00001490: 7320 7661 6c75 6520 6973 204e 4f5f 5641  s value is NO_VA
-000014a0: 4c55 4520 756e 7469 6c20 6974 2067 6574  LUE until it get
-000014b0: 7320 6120 7265 7175 6573 743a 0a0a 2020  s a request:..  
-000014c0: 3e3e 3e20 7769 6467 6574 2e76 616c 7565  >>> widget.value
-000014d0: 0a20 203c 4e4f 5f56 414c 5545 3e0a 0a4c  .  <NO_VALUE>..L
-000014e0: 6574 2773 2066 696c 6c20 696e 2073 6f6d  et's fill in som
-000014f0: 6520 7661 6c75 6573 2076 6961 2074 6865  e values via the
-00001500: 2072 6571 7565 7374 3a0a 0a20 203e 3e3e   request:..  >>>
-00001510: 2077 6964 6765 742e 7265 7175 6573 7420   widget.request 
-00001520: 3d20 5465 7374 5265 7175 6573 7428 7061  = TestRequest(pa
-00001530: 7261 6d73 3d7b 2773 7562 6f62 6a65 6374  rams={'subobject
-00001540: 2e77 6964 6765 7473 2e66 6f6f 6669 656c  .widgets.foofiel
-00001550: 6427 3a27 3227 2c0a 2020 2e2e 2e20 2020  d':'2',.  ...   
+00001320: 2020 2020 3c2f 6c61 6265 6c3e 0a20 2020      </label>.   
+00001330: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00001340: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001350: 3c64 6976 2063 6c61 7373 3d22 7769 6467  <div class="widg
+00001360: 6574 223e 0a20 2020 2020 2020 2020 2020  et">.           
+00001370: 2020 2020 2020 2020 2020 203c 696e 7075             <inpu
+00001380: 7420 7479 7065 3d22 7465 7874 220a 2020  t type="text".  
+00001390: 2020 2020 2020 2069 643d 2273 7562 6f62         id="subob
+000013a0: 6a65 6374 2d77 6964 6765 7473 2d62 6172  ject-widgets-bar
+000013b0: 6669 656c 6422 0a20 2020 2020 2020 2020  field".         
+000013c0: 6e61 6d65 3d22 7375 626f 626a 6563 742e  name="subobject.
+000013d0: 7769 6467 6574 732e 6261 7266 6965 6c64  widgets.barfield
+000013e0: 220a 2020 2020 2020 2020 2063 6c61 7373  ".         class
+000013f0: 3d22 7465 7874 2d77 6964 6765 7420 696e  ="text-widget in
+00001400: 742d 6669 656c 6422 0a20 2020 2020 2020  t-field".       
+00001410: 2020 7661 6c75 653d 2236 3636 2220 2f3e    value="666" />
+00001420: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00001430: 2f64 6976 3e0a 2020 2020 2020 3c69 6e70  /div>.      <inp
+00001440: 7574 206e 616d 653d 2273 7562 6f62 6a65  ut name="subobje
+00001450: 6374 2d65 6d70 7479 2d6d 6172 6b65 7222  ct-empty-marker"
+00001460: 2074 7970 653d 2268 6964 6465 6e22 2076   type="hidden" v
+00001470: 616c 7565 3d22 3122 202f 3e0a 2020 3c2f  alue="1" />.  </
+00001480: 6469 763e 0a0a 0a54 6865 2077 6964 6765  div>...The widge
+00001490: 7427 7320 7661 6c75 6520 6973 204e 4f5f  t's value is NO_
+000014a0: 5641 4c55 4520 756e 7469 6c20 6974 2067  VALUE until it g
+000014b0: 6574 7320 6120 7265 7175 6573 743a 0a0a  ets a request:..
+000014c0: 2020 3e3e 3e20 7769 6467 6574 2e76 616c    >>> widget.val
+000014d0: 7565 0a20 203c 4e4f 5f56 414c 5545 3e0a  ue.  <NO_VALUE>.
+000014e0: 0a4c 6574 2773 2066 696c 6c20 696e 2073  .Let's fill in s
+000014f0: 6f6d 6520 7661 6c75 6573 2076 6961 2074  ome values via t
+00001500: 6865 2072 6571 7565 7374 3a0a 0a20 203e  he request:..  >
+00001510: 3e3e 2077 6964 6765 742e 7265 7175 6573  >> widget.reques
+00001520: 7420 3d20 5465 7374 5265 7175 6573 7428  t = TestRequest(
+00001530: 7061 7261 6d73 3d7b 2773 7562 6f62 6a65  params={'subobje
+00001540: 6374 2e77 6964 6765 7473 2e66 6f6f 6669  ct.widgets.foofi
+00001550: 656c 6427 3a27 3227 2c0a 2020 2e2e 2e20  eld':'2',.  ... 
 00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 2020 2027 7375 626f 626a 6563 742e 7769     'subobject.wi
-00001590: 6467 6574 732e 6261 7266 6965 6c64 273a  dgets.barfield':
-000015a0: 2739 3939 272c 0a20 202e 2e2e 2020 2020  '999',.  ...    
+00001580: 2020 2020 2027 7375 626f 626a 6563 742e       'subobject.
+00001590: 7769 6467 6574 732e 6261 7266 6965 6c64  widgets.barfield
+000015a0: 273a 2739 3939 272c 0a20 202e 2e2e 2020  ':'999',.  ...  
 000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015d0: 2020 2773 7562 6f62 6a65 6374 2d65 6d70    'subobject-emp
-000015e0: 7479 2d6d 6172 6b65 7227 3a27 3127 7d29  ty-marker':'1'})
-000015f0: 0a20 203e 3e3e 2077 6964 6765 742e 7570  .  >>> widget.up
-00001600: 6461 7465 2829 0a20 203e 3e3e 2070 7269  date().  >>> pri
-00001610: 6e74 2866 6f72 6d61 745f 6874 6d6c 2877  nt(format_html(w
-00001620: 6964 6765 742e 7265 6e64 6572 2829 2929  idget.render()))
-00001630: 0a20 203c 6469 7620 636c 6173 733d 226f  .  <div class="o
-00001640: 626a 6563 742d 7769 6467 6574 2072 6571  bject-widget req
-00001650: 7569 7265 6422 3e0a 2020 2020 2020 2020  uired">.        
-00001660: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00001670: 3d22 6c61 6265 6c22 3e0a 2020 2020 2020  ="label">.      
+000015d0: 2020 2020 2773 7562 6f62 6a65 6374 2d65      'subobject-e
+000015e0: 6d70 7479 2d6d 6172 6b65 7227 3a27 3127  mpty-marker':'1'
+000015f0: 7d29 0a20 203e 3e3e 2077 6964 6765 742e  }).  >>> widget.
+00001600: 7570 6461 7465 2829 0a20 203e 3e3e 2070  update().  >>> p
+00001610: 7269 6e74 2866 6f72 6d61 745f 6874 6d6c  rint(format_html
+00001620: 2877 6964 6765 742e 7265 6e64 6572 2829  (widget.render()
+00001630: 2929 0a20 203c 6469 7620 636c 6173 733d  )).  <div class=
+00001640: 226f 626a 6563 742d 7769 6467 6574 2072  "object-widget r
+00001650: 6571 7569 7265 6422 3e0a 2020 2020 2020  equired">.      
+00001660: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00001670: 7373 3d22 6c61 6265 6c22 3e0a 2020 2020  ss="label">.    
 00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 3c6c 6162 656c 2066 6f72 3d22 7375 626f  <label for="subo
-000016a0: 626a 6563 742d 7769 6467 6574 732d 666f  bject-widgets-fo
-000016b0: 6f66 6965 6c64 223e 0a20 2020 2020 2020  ofield">.       
+00001690: 2020 3c6c 6162 656c 2066 6f72 3d22 7375    <label for="su
+000016a0: 626f 626a 6563 742d 7769 6467 6574 732d  bobject-widgets-
+000016b0: 666f 6f66 6965 6c64 223e 0a20 2020 2020  foofield">.     
 000016c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016d0: 2020 2020 2020 203c 7370 616e 3e4d 7920         <span>My 
-000016e0: 666f 6f20 6669 656c 643c 2f73 7061 6e3e  foo field</span>
-000016f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001700: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001710: 7370 616e 2063 6c61 7373 3d22 7265 7175  span class="requ
-00001720: 6972 6564 223e 2a3c 2f73 7061 6e3e 0a20  ired">*</span>. 
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2020 2020 203c 2f6c 6162 656c 3e0a 2020       </label>.  
-00001750: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00001760: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00001770: 203c 6469 7620 636c 6173 733d 2277 6964   <div class="wid
-00001780: 6765 7422 3e0a 2020 2020 2020 2020 2020  get">.          
-00001790: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
-000017a0: 7574 2074 7970 653d 2274 6578 7422 0a20  ut type="text". 
-000017b0: 2020 2020 2020 2020 6964 3d22 7375 626f          id="subo
-000017c0: 626a 6563 742d 7769 6467 6574 732d 666f  bject-widgets-fo
-000017d0: 6f66 6965 6c64 220a 2020 2020 2020 2020  ofield".        
-000017e0: 206e 616d 653d 2273 7562 6f62 6a65 6374   name="subobject
-000017f0: 2e77 6964 6765 7473 2e66 6f6f 6669 656c  .widgets.foofiel
-00001800: 6422 0a20 2020 2020 2020 2020 636c 6173  d".         clas
-00001810: 733d 2274 6578 742d 7769 6467 6574 2072  s="text-widget r
-00001820: 6571 7569 7265 6420 696e 742d 6669 656c  equired int-fiel
-00001830: 6422 0a20 2020 2020 2020 2020 7661 6c75  d".         valu
-00001840: 653d 2232 2220 2f3e 0a20 2020 2020 2020  e="2" />.       
-00001850: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00001860: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00001870: 2063 6c61 7373 3d22 6c61 6265 6c22 3e0a   class="label">.
-00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001890: 2020 2020 2020 3c6c 6162 656c 2066 6f72        <label for
-000018a0: 3d22 7375 626f 626a 6563 742d 7769 6467  ="subobject-widg
-000018b0: 6574 732d 6261 7266 6965 6c64 223e 0a20  ets-barfield">. 
-000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018d0: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
-000018e0: 616e 3e4d 7920 6465 6172 2062 6172 3c2f  an>My dear bar</
-000018f0: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
-00001900: 2020 2020 2020 2020 2020 2020 3c2f 6c61              </la
-00001910: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
-00001920: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00001930: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00001940: 7373 3d22 7769 6467 6574 223e 0a20 2020  ss="widget">.   
+000016d0: 2020 2020 2020 2020 203c 7370 616e 3e4d           <span>M
+000016e0: 7920 666f 6f20 6669 656c 643c 2f73 7061  y foo field</spa
+000016f0: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 203c 7370 616e 2063 6c61 7373 3d22 7265   <span class="re
+00001720: 7175 6972 6564 223e 2a3c 2f73 7061 6e3e  quired">*</span>
+00001730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001740: 2020 2020 2020 203c 2f6c 6162 656c 3e0a         </label>.
+00001750: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001760: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00001770: 2020 203c 6469 7620 636c 6173 733d 2277     <div class="w
+00001780: 6964 6765 7422 3e0a 2020 2020 2020 2020  idget">.        
+00001790: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+000017a0: 6e70 7574 2074 7970 653d 2274 6578 7422  nput type="text"
+000017b0: 0a20 2020 2020 2020 2020 6964 3d22 7375  .         id="su
+000017c0: 626f 626a 6563 742d 7769 6467 6574 732d  bobject-widgets-
+000017d0: 666f 6f66 6965 6c64 220a 2020 2020 2020  foofield".      
+000017e0: 2020 206e 616d 653d 2273 7562 6f62 6a65     name="subobje
+000017f0: 6374 2e77 6964 6765 7473 2e66 6f6f 6669  ct.widgets.foofi
+00001800: 656c 6422 0a20 2020 2020 2020 2020 636c  eld".         cl
+00001810: 6173 733d 2274 6578 742d 7769 6467 6574  ass="text-widget
+00001820: 2072 6571 7569 7265 6420 696e 742d 6669   required int-fi
+00001830: 656c 6422 0a20 2020 2020 2020 2020 7661  eld".         va
+00001840: 6c75 653d 2232 2220 2f3e 0a20 2020 2020  lue="2" />.     
+00001850: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00001860: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00001870: 6976 2063 6c61 7373 3d22 6c61 6265 6c22  iv class="label"
+00001880: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001890: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
+000018a0: 6f72 3d22 7375 626f 626a 6563 742d 7769  or="subobject-wi
+000018b0: 6467 6574 732d 6261 7266 6965 6c64 223e  dgets-barfield">
+000018c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000018d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000018e0: 7370 616e 3e4d 7920 6465 6172 2062 6172  span>My dear bar
+000018f0: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
+00001900: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001910: 6c61 6265 6c3e 0a20 2020 2020 2020 2020  label>.         
+00001920: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00001930: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00001940: 6c61 7373 3d22 7769 6467 6574 223e 0a20  lass="widget">. 
 00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001960: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
-00001970: 7465 7874 220a 2020 2020 2020 2020 2069  text".         i
-00001980: 643d 2273 7562 6f62 6a65 6374 2d77 6964  d="subobject-wid
-00001990: 6765 7473 2d62 6172 6669 656c 6422 0a20  gets-barfield". 
-000019a0: 2020 2020 2020 2020 6e61 6d65 3d22 7375          name="su
-000019b0: 626f 626a 6563 742e 7769 6467 6574 732e  bobject.widgets.
-000019c0: 6261 7266 6965 6c64 220a 2020 2020 2020  barfield".      
-000019d0: 2020 2063 6c61 7373 3d22 7465 7874 2d77     class="text-w
-000019e0: 6964 6765 7420 696e 742d 6669 656c 6422  idget int-field"
-000019f0: 0a20 2020 2020 2020 2020 7661 6c75 653d  .         value=
-00001a00: 2239 3939 2220 2f3e 0a20 2020 2020 2020  "999" />.       
-00001a10: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00001a20: 2020 2020 3c69 6e70 7574 206e 616d 653d      <input name=
-00001a30: 2273 7562 6f62 6a65 6374 2d65 6d70 7479  "subobject-empty
-00001a40: 2d6d 6172 6b65 7222 2074 7970 653d 2268  -marker" type="h
-00001a50: 6964 6465 6e22 2076 616c 7565 3d22 3122  idden" value="1"
-00001a60: 2f3e 0a20 203c 2f64 6976 3e0a 0a57 6964  />.  </div>..Wid
-00001a70: 6765 7420 7661 6c75 6520 636f 6d65 7320  get value comes 
-00001a80: 6672 6f6d 2074 6865 2072 6571 7565 7374  from the request
-00001a90: 3a0a 0a20 203e 3e3e 2066 726f 6d20 7070  :..  >>> from pp
-00001aa0: 7269 6e74 2069 6d70 6f72 7420 7070 7269  rint import ppri
-00001ab0: 6e74 0a20 203e 3e3e 2077 7620 3d20 7769  nt.  >>> wv = wi
-00001ac0: 6467 6574 2e76 616c 7565 0a20 203e 3e3e  dget.value.  >>>
-00001ad0: 2070 7072 696e 7428 7776 290a 2020 7b27   pprint(wv).  {'
-00001ae0: 6261 7266 6965 6c64 273a 2027 3939 3927  barfield': '999'
-00001af0: 2c20 2766 6f6f 6669 656c 6427 3a20 2732  , 'foofield': '2
-00001b00: 277d 0a0a 4275 7420 6f75 7220 6f62 6a65  '}..But our obje
-00001b10: 6374 2077 696c 6c20 6e6f 7420 6265 206d  ct will not be m
-00001b20: 6f64 6966 6965 642c 2073 696e 6365 2074  odified, since t
-00001b30: 6865 7265 2077 6173 206e 6f20 2261 7070  here was no "app
-00001b40: 6c79 222d 6c69 6b65 2063 6f6e 7472 6f6c  ly"-like control
-00001b50: 2e0a 0a20 203e 3e3e 2076 0a20 203c 7079  ...  >>> v.  <py
-00001b60: 616d 735f 666f 726d 2e74 6573 7469 6e67  ams_form.testing
-00001b70: 2e4d 7953 7562 4f62 6a65 6374 206f 626a  .MySubObject obj
-00001b80: 6563 7420 6174 202e 2e2e 3e0a 2020 3e3e  ect at ...>.  >>
-00001b90: 3e20 762e 666f 6f66 6965 6c64 0a20 2034  > v.foofield.  4
-00001ba0: 320a 2020 3e3e 3e20 762e 6261 7266 6965  2.  >>> v.barfie
-00001bb0: 6c64 0a20 2036 3636 0a0a 5468 6520 6d61  ld.  666..The ma
-00001bc0: 726b 6572 206d 7573 7420 7374 6179 2028  rker must stay (
-00001bd0: 7765 2068 6176 6520 746f 206d 6f64 6966  we have to modif
-00001be0: 7920 7468 6520 7361 6d65 206f 626a 6563  y the same objec
-00001bf0: 7429 3a0a 0a20 203e 3e3e 2076 2e5f 5f6d  t):..  >>> v.__m
-00001c00: 6172 6b65 725f 5f0a 2020 2754 6869 734d  arker__.  'ThisM
-00001c10: 7573 7453 7461 7954 6865 5361 6d65 270a  ustStayTheSame'.
-00001c20: 0a0a 2020 3e3e 3e20 636f 6e76 6572 7465  ..  >>> converte
-00001c30: 7220 3d20 696e 7465 7266 6163 6573 2e49  r = interfaces.I
-00001c40: 4461 7461 436f 6e76 6572 7465 7228 7769  DataConverter(wi
-00001c50: 6467 6574 290a 0a20 203e 3e3e 2076 616c  dget)..  >>> val
-00001c60: 7565 203d 2063 6f6e 7665 7274 6572 2e74  ue = converter.t
-00001c70: 6f5f 6669 656c 645f 7661 6c75 6528 7776  o_field_value(wv
-00001c80: 290a 2020 5472 6163 6562 6163 6b20 286d  ).  Traceback (m
-00001c90: 6f73 7420 7265 6365 6e74 2063 616c 6c20  ost recent call 
-00001ca0: 6c61 7374 293a 0a20 202e 2e2e 0a20 2052  last):.  ....  R
-00001cb0: 756e 7469 6d65 4572 726f 723a 204e 6f20  untimeError: No 
-00001cc0: 494f 626a 6563 7446 6163 746f 7279 2061  IObjectFactory a
-00001cd0: 6461 7074 6572 2072 6567 6973 7465 7265  dapter registere
-00001ce0: 6420 666f 7220 7079 616d 735f 666f 726d  d for pyams_form
-00001cf0: 2e74 6573 7469 6e67 2e49 4d79 5375 624f  .testing.IMySubO
-00001d00: 626a 6563 740a 0a57 6520 6861 7665 2074  bject..We have t
-00001d10: 6f20 7265 6769 7374 6572 206f 626a 6563  o register objec
-00001d20: 7420 6661 6374 6f72 7920 6164 6170 7465  t factory adapte
-00001d30: 7273 2074 6f20 616c 6c6f 7720 7468 6520  rs to allow the 
-00001d40: 6f62 6a65 6374 7769 6467 6574 2074 6f0a  objectwidget to.
-00001d50: 6372 6561 7465 206f 626a 6563 7473 3a0a  create objects:.
-00001d60: 0a20 203e 3e3e 2066 726f 6d20 7079 616d  .  >>> from pyam
-00001d70: 735f 666f 726d 2e6f 626a 6563 7420 696d  s_form.object im
-00001d80: 706f 7274 2072 6567 6973 7465 725f 6661  port register_fa
-00001d90: 6374 6f72 795f 6164 6170 7465 720a 2020  ctory_adapter.  
-00001da0: 3e3e 3e20 7265 6769 7374 6572 5f66 6163  >>> register_fac
-00001db0: 746f 7279 5f61 6461 7074 6572 2849 4d79  tory_adapter(IMy
-00001dc0: 5375 624f 626a 6563 742c 204d 7953 7562  SubObject, MySub
-00001dd0: 4f62 6a65 6374 2c20 636f 6e66 6967 2e72  Object, config.r
-00001de0: 6567 6973 7472 7929 0a20 203e 3e3e 2072  egistry).  >>> r
-00001df0: 6567 6973 7465 725f 6661 6374 6f72 795f  egister_factory_
-00001e00: 6164 6170 7465 7228 494d 7953 6563 6f6e  adapter(IMySecon
-00001e10: 642c 204d 7953 6563 6f6e 642c 2063 6f6e  d, MySecond, con
-00001e20: 6669 672e 7265 6769 7374 7279 290a 0a20  fig.registry).. 
-00001e30: 203e 3e3e 2076 616c 7565 203d 2063 6f6e   >>> value = con
-00001e40: 7665 7274 6572 2e74 6f5f 6669 656c 645f  verter.to_field_
-00001e50: 7661 6c75 6528 7776 290a 2020 3e3e 3e20  value(wv).  >>> 
-00001e60: 7661 6c75 650a 2020 3c70 7961 6d73 5f66  value.  <pyams_f
-00001e70: 6f72 6d2e 7465 7374 696e 672e 4d79 5375  orm.testing.MySu
-00001e80: 624f 626a 6563 7420 6f62 6a65 6374 2061  bObject object a
-00001e90: 7420 2e2e 2e3e 0a20 203e 3e3e 2076 616c  t ...>.  >>> val
-00001ea0: 7565 2e66 6f6f 6669 656c 640a 2020 320a  ue.foofield.  2.
-00001eb0: 2020 3e3e 3e20 7661 6c75 652e 6261 7266    >>> value.barf
-00001ec0: 6965 6c64 0a20 2039 3939 0a0a 5468 6973  ield.  999..This
-00001ed0: 2069 7320 6120 6469 6666 6572 656e 7420   is a different 
-00001ee0: 6f62 6a65 6374 3a0a 0a20 203e 3e3e 2076  object:..  >>> v
-00001ef0: 616c 7565 2e5f 5f6d 6172 6b65 725f 5f0a  alue.__marker__.
-00001f00: 2020 5472 6163 6562 6163 6b20 286d 6f73    Traceback (mos
-00001f10: 7420 7265 6365 6e74 2063 616c 6c20 6c61  t recent call la
-00001f20: 7374 293a 0a20 202e 2e2e 0a20 2041 7474  st):.  ....  Att
-00001f30: 7269 6275 7465 4572 726f 723a 2027 4d79  ributeError: 'My
-00001f40: 5375 624f 626a 6563 7427 206f 626a 6563  SubObject' objec
-00001f50: 7420 6861 7320 6e6f 2061 7474 7269 6275  t has no attribu
-00001f60: 7465 2027 5f5f 6d61 726b 6572 5f5f 270a  te '__marker__'.
-00001f70: 0a0a 5365 7474 696e 6720 6d69 7373 696e  ..Setting missin
-00001f80: 6720 7661 6c75 6573 206f 6e20 7468 6520  g values on the 
-00001f90: 7769 6467 6574 2077 6f72 6b73 2074 6f6f  widget works too
-00001fa0: 3a0a 0a20 203e 3e3e 2077 6964 6765 742e  :..  >>> widget.
-00001fb0: 7661 6c75 6520 3d20 636f 6e76 6572 7465  value = converte
-00001fc0: 722e 746f 5f77 6964 6765 745f 7661 6c75  r.to_widget_valu
-00001fd0: 6528 6669 656c 642e 6d69 7373 696e 675f  e(field.missing_
-00001fe0: 7661 6c75 6529 0a0a 2020 3e3e 3e20 7769  value)..  >>> wi
-00001ff0: 6467 6574 2e75 7064 6174 6528 290a 0a44  dget.update()..D
-00002000: 6566 6175 6c74 2076 616c 7565 7320 6765  efault values ge
-00002010: 7420 7265 6e64 6572 6564 3a0a 0a20 203e  t rendered:..  >
-00002020: 3e3e 2070 7269 6e74 2866 6f72 6d61 745f  >> print(format_
-00002030: 6874 6d6c 2877 6964 6765 742e 7265 6e64  html(widget.rend
-00002040: 6572 2829 2929 0a20 203c 6469 7620 636c  er())).  <div cl
-00002050: 6173 733d 226f 626a 6563 742d 7769 6467  ass="object-widg
-00002060: 6574 2072 6571 7569 7265 6422 3e0a 2020  et required">.  
-00002070: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00002080: 2063 6c61 7373 3d22 6c61 6265 6c22 3e0a   class="label">.
-00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020a0: 2020 2020 2020 3c6c 6162 656c 2066 6f72        <label for
-000020b0: 3d22 7375 626f 626a 6563 742d 7769 6467  ="subobject-widg
-000020c0: 6574 732d 666f 6f66 6965 6c64 223e 0a20  ets-foofield">. 
-000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020e0: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
-000020f0: 616e 3e4d 7920 666f 6f20 6669 656c 643c  an>My foo field<
-00002100: 2f73 7061 6e3e 0a20 2020 2020 2020 2020  /span>.         
+00001960: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
+00001970: 3d22 7465 7874 220a 2020 2020 2020 2020  ="text".        
+00001980: 2069 643d 2273 7562 6f62 6a65 6374 2d77   id="subobject-w
+00001990: 6964 6765 7473 2d62 6172 6669 656c 6422  idgets-barfield"
+000019a0: 0a20 2020 2020 2020 2020 6e61 6d65 3d22  .         name="
+000019b0: 7375 626f 626a 6563 742e 7769 6467 6574  subobject.widget
+000019c0: 732e 6261 7266 6965 6c64 220a 2020 2020  s.barfield".    
+000019d0: 2020 2020 2063 6c61 7373 3d22 7465 7874       class="text
+000019e0: 2d77 6964 6765 7420 696e 742d 6669 656c  -widget int-fiel
+000019f0: 6422 0a20 2020 2020 2020 2020 7661 6c75  d".         valu
+00001a00: 653d 2239 3939 2220 2f3e 0a20 2020 2020  e="999" />.     
+00001a10: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00001a20: 2020 2020 2020 3c69 6e70 7574 206e 616d        <input nam
+00001a30: 653d 2273 7562 6f62 6a65 6374 2d65 6d70  e="subobject-emp
+00001a40: 7479 2d6d 6172 6b65 7222 2074 7970 653d  ty-marker" type=
+00001a50: 2268 6964 6465 6e22 2076 616c 7565 3d22  "hidden" value="
+00001a60: 3122 202f 3e0a 2020 3c2f 6469 763e 0a0a  1" />.  </div>..
+00001a70: 5769 6467 6574 2076 616c 7565 2063 6f6d  Widget value com
+00001a80: 6573 2066 726f 6d20 7468 6520 7265 7175  es from the requ
+00001a90: 6573 743a 0a0a 2020 3e3e 3e20 6672 6f6d  est:..  >>> from
+00001aa0: 2070 7072 696e 7420 696d 706f 7274 2070   pprint import p
+00001ab0: 7072 696e 740a 2020 3e3e 3e20 7776 203d  print.  >>> wv =
+00001ac0: 2077 6964 6765 742e 7661 6c75 650a 2020   widget.value.  
+00001ad0: 3e3e 3e20 7070 7269 6e74 2877 7629 0a20  >>> pprint(wv). 
+00001ae0: 207b 2762 6172 6669 656c 6427 3a20 2739   {'barfield': '9
+00001af0: 3939 272c 2027 666f 6f66 6965 6c64 273a  99', 'foofield':
+00001b00: 2027 3227 7d0a 0a42 7574 206f 7572 206f   '2'}..But our o
+00001b10: 626a 6563 7420 7769 6c6c 206e 6f74 2062  bject will not b
+00001b20: 6520 6d6f 6469 6669 6564 2c20 7369 6e63  e modified, sinc
+00001b30: 6520 7468 6572 6520 7761 7320 6e6f 2022  e there was no "
+00001b40: 6170 706c 7922 2d6c 696b 6520 636f 6e74  apply"-like cont
+00001b50: 726f 6c2e 0a0a 2020 3e3e 3e20 760a 2020  rol...  >>> v.  
+00001b60: 3c70 7961 6d73 5f66 6f72 6d2e 7465 7374  <pyams_form.test
+00001b70: 696e 672e 4d79 5375 624f 626a 6563 7420  ing.MySubObject 
+00001b80: 6f62 6a65 6374 2061 7420 2e2e 2e3e 0a20  object at ...>. 
+00001b90: 203e 3e3e 2076 2e66 6f6f 6669 656c 640a   >>> v.foofield.
+00001ba0: 2020 3432 0a20 203e 3e3e 2076 2e62 6172    42.  >>> v.bar
+00001bb0: 6669 656c 640a 2020 3636 360a 0a54 6865  field.  666..The
+00001bc0: 206d 6172 6b65 7220 6d75 7374 2073 7461   marker must sta
+00001bd0: 7920 2877 6520 6861 7665 2074 6f20 6d6f  y (we have to mo
+00001be0: 6469 6679 2074 6865 2073 616d 6520 6f62  dify the same ob
+00001bf0: 6a65 6374 293a 0a0a 2020 3e3e 3e20 762e  ject):..  >>> v.
+00001c00: 5f5f 6d61 726b 6572 5f5f 0a20 2027 5468  __marker__.  'Th
+00001c10: 6973 4d75 7374 5374 6179 5468 6553 616d  isMustStayTheSam
+00001c20: 6527 0a0a 0a20 203e 3e3e 2063 6f6e 7665  e'...  >>> conve
+00001c30: 7274 6572 203d 2069 6e74 6572 6661 6365  rter = interface
+00001c40: 732e 4944 6174 6143 6f6e 7665 7274 6572  s.IDataConverter
+00001c50: 2877 6964 6765 7429 0a0a 2020 3e3e 3e20  (widget)..  >>> 
+00001c60: 7661 6c75 6520 3d20 636f 6e76 6572 7465  value = converte
+00001c70: 722e 746f 5f66 6965 6c64 5f76 616c 7565  r.to_field_value
+00001c80: 2877 7629 0a20 2054 7261 6365 6261 636b  (wv).  Traceback
+00001c90: 2028 6d6f 7374 2072 6563 656e 7420 6361   (most recent ca
+00001ca0: 6c6c 206c 6173 7429 3a0a 2020 2e2e 2e0a  ll last):.  ....
+00001cb0: 2020 5275 6e74 696d 6545 7272 6f72 3a20    RuntimeError: 
+00001cc0: 4e6f 2049 4f62 6a65 6374 4661 6374 6f72  No IObjectFactor
+00001cd0: 7920 6164 6170 7465 7220 7265 6769 7374  y adapter regist
+00001ce0: 6572 6564 2066 6f72 2070 7961 6d73 5f66  ered for pyams_f
+00001cf0: 6f72 6d2e 7465 7374 696e 672e 494d 7953  orm.testing.IMyS
+00001d00: 7562 4f62 6a65 6374 0a0a 5765 2068 6176  ubObject..We hav
+00001d10: 6520 746f 2072 6567 6973 7465 7220 6f62  e to register ob
+00001d20: 6a65 6374 2066 6163 746f 7279 2061 6461  ject factory ada
+00001d30: 7074 6572 7320 746f 2061 6c6c 6f77 2074  pters to allow t
+00001d40: 6865 206f 626a 6563 7477 6964 6765 7420  he objectwidget 
+00001d50: 746f 0a63 7265 6174 6520 6f62 6a65 6374  to.create object
+00001d60: 733a 0a0a 2020 3e3e 3e20 6672 6f6d 2070  s:..  >>> from p
+00001d70: 7961 6d73 5f66 6f72 6d2e 6f62 6a65 6374  yams_form.object
+00001d80: 2069 6d70 6f72 7420 7265 6769 7374 6572   import register
+00001d90: 5f66 6163 746f 7279 5f61 6461 7074 6572  _factory_adapter
+00001da0: 0a20 203e 3e3e 2072 6567 6973 7465 725f  .  >>> register_
+00001db0: 6661 6374 6f72 795f 6164 6170 7465 7228  factory_adapter(
+00001dc0: 494d 7953 7562 4f62 6a65 6374 2c20 4d79  IMySubObject, My
+00001dd0: 5375 624f 626a 6563 742c 2063 6f6e 6669  SubObject, confi
+00001de0: 672e 7265 6769 7374 7279 290a 2020 3e3e  g.registry).  >>
+00001df0: 3e20 7265 6769 7374 6572 5f66 6163 746f  > register_facto
+00001e00: 7279 5f61 6461 7074 6572 2849 4d79 5365  ry_adapter(IMySe
+00001e10: 636f 6e64 2c20 4d79 5365 636f 6e64 2c20  cond, MySecond, 
+00001e20: 636f 6e66 6967 2e72 6567 6973 7472 7929  config.registry)
+00001e30: 0a0a 2020 3e3e 3e20 7661 6c75 6520 3d20  ..  >>> value = 
+00001e40: 636f 6e76 6572 7465 722e 746f 5f66 6965  converter.to_fie
+00001e50: 6c64 5f76 616c 7565 2877 7629 0a20 203e  ld_value(wv).  >
+00001e60: 3e3e 2076 616c 7565 0a20 203c 7079 616d  >> value.  <pyam
+00001e70: 735f 666f 726d 2e74 6573 7469 6e67 2e4d  s_form.testing.M
+00001e80: 7953 7562 4f62 6a65 6374 206f 626a 6563  ySubObject objec
+00001e90: 7420 6174 202e 2e2e 3e0a 2020 3e3e 3e20  t at ...>.  >>> 
+00001ea0: 7661 6c75 652e 666f 6f66 6965 6c64 0a20  value.foofield. 
+00001eb0: 2032 0a20 203e 3e3e 2076 616c 7565 2e62   2.  >>> value.b
+00001ec0: 6172 6669 656c 640a 2020 3939 390a 0a54  arfield.  999..T
+00001ed0: 6869 7320 6973 2061 2064 6966 6665 7265  his is a differe
+00001ee0: 6e74 206f 626a 6563 743a 0a0a 2020 3e3e  nt object:..  >>
+00001ef0: 3e20 7661 6c75 652e 5f5f 6d61 726b 6572  > value.__marker
+00001f00: 5f5f 0a20 2054 7261 6365 6261 636b 2028  __.  Traceback (
+00001f10: 6d6f 7374 2072 6563 656e 7420 6361 6c6c  most recent call
+00001f20: 206c 6173 7429 3a0a 2020 2e2e 2e0a 2020   last):.  ....  
+00001f30: 4174 7472 6962 7574 6545 7272 6f72 3a20  AttributeError: 
+00001f40: 274d 7953 7562 4f62 6a65 6374 2720 6f62  'MySubObject' ob
+00001f50: 6a65 6374 2068 6173 206e 6f20 6174 7472  ject has no attr
+00001f60: 6962 7574 6520 275f 5f6d 6172 6b65 725f  ibute '__marker_
+00001f70: 5f27 0a0a 0a53 6574 7469 6e67 206d 6973  _'...Setting mis
+00001f80: 7369 6e67 2076 616c 7565 7320 6f6e 2074  sing values on t
+00001f90: 6865 2077 6964 6765 7420 776f 726b 7320  he widget works 
+00001fa0: 746f 6f3a 0a0a 2020 3e3e 3e20 7769 6467  too:..  >>> widg
+00001fb0: 6574 2e76 616c 7565 203d 2063 6f6e 7665  et.value = conve
+00001fc0: 7274 6572 2e74 6f5f 7769 6467 6574 5f76  rter.to_widget_v
+00001fd0: 616c 7565 2866 6965 6c64 2e6d 6973 7369  alue(field.missi
+00001fe0: 6e67 5f76 616c 7565 290a 0a20 203e 3e3e  ng_value)..  >>>
+00001ff0: 2077 6964 6765 742e 7570 6461 7465 2829   widget.update()
+00002000: 0a0a 4465 6661 756c 7420 7661 6c75 6573  ..Default values
+00002010: 2067 6574 2072 656e 6465 7265 643a 0a0a   get rendered:..
+00002020: 2020 3e3e 3e20 7072 696e 7428 666f 726d    >>> print(form
+00002030: 6174 5f68 746d 6c28 7769 6467 6574 2e72  at_html(widget.r
+00002040: 656e 6465 7228 2929 290a 2020 3c64 6976  ender())).  <div
+00002050: 2063 6c61 7373 3d22 6f62 6a65 6374 2d77   class="object-w
+00002060: 6964 6765 7420 7265 7175 6972 6564 223e  idget required">
+00002070: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00002080: 6469 7620 636c 6173 733d 226c 6162 656c  div class="label
+00002090: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000020a0: 2020 2020 2020 2020 203c 6c61 6265 6c20           <label 
+000020b0: 666f 723d 2273 7562 6f62 6a65 6374 2d77  for="subobject-w
+000020c0: 6964 6765 7473 2d66 6f6f 6669 656c 6422  idgets-foofield"
+000020d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000020e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020f0: 3c73 7061 6e3e 4d79 2066 6f6f 2066 6965  <span>My foo fie
+00002100: 6c64 3c2f 7370 616e 3e0a 2020 2020 2020  ld</span>.      
 00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002120: 2020 2020 203c 7370 616e 2063 6c61 7373       <span class
-00002130: 3d22 7265 7175 6972 6564 223e 2a3c 2f73  ="required">*</s
-00002140: 7061 6e3e 0a20 2020 2020 2020 2020 2020  pan>.           
-00002150: 2020 2020 2020 2020 2020 203c 2f6c 6162             </lab
-00002160: 656c 3e0a 2020 2020 2020 2020 2020 2020  el>.            
-00002170: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00002180: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00002190: 733d 2277 6964 6765 7422 3e0a 2020 2020  s="widget">.    
+00002120: 2020 2020 2020 2020 3c73 7061 6e20 636c          <span cl
+00002130: 6173 733d 2272 6571 7569 7265 6422 3e2a  ass="required">*
+00002140: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
+00002150: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00002160: 6c61 6265 6c3e 0a20 2020 2020 2020 2020  label>.         
+00002170: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00002180: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00002190: 6c61 7373 3d22 7769 6467 6574 223e 0a20  lass="widget">. 
 000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 2020 3c69 6e70 7574 2074 7970 653d 2274    <input type="t
-000021c0: 6578 7422 0a20 2020 2020 2020 2020 6964  ext".         id
-000021d0: 3d22 7375 626f 626a 6563 742d 7769 6467  ="subobject-widg
-000021e0: 6574 732d 666f 6f66 6965 6c64 220a 2020  ets-foofield".  
-000021f0: 2020 2020 2020 206e 616d 653d 2273 7562         name="sub
-00002200: 6f62 6a65 6374 2e77 6964 6765 7473 2e66  object.widgets.f
-00002210: 6f6f 6669 656c 6422 0a20 2020 2020 2020  oofield".       
-00002220: 2020 636c 6173 733d 2274 6578 742d 7769    class="text-wi
-00002230: 6467 6574 2072 6571 7569 7265 6420 696e  dget required in
-00002240: 742d 6669 656c 6422 0a20 2020 2020 2020  t-field".       
-00002250: 2020 7661 6c75 653d 2232 2220 2f3e 0a20    value="2" />. 
-00002260: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00002270: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00002280: 2020 3c64 6976 2063 6c61 7373 3d22 6c61    <div class="la
-00002290: 6265 6c22 3e0a 2020 2020 2020 2020 2020  bel">.          
-000022a0: 2020 2020 2020 2020 2020 2020 3c6c 6162              <lab
-000022b0: 656c 2066 6f72 3d22 7375 626f 626a 6563  el for="subobjec
-000022c0: 742d 7769 6467 6574 732d 6261 7266 6965  t-widgets-barfie
-000022d0: 6c64 223e 0a20 2020 2020 2020 2020 2020  ld">.           
+000021b0: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
+000021c0: 3d22 7465 7874 220a 2020 2020 2020 2020  ="text".        
+000021d0: 2069 643d 2273 7562 6f62 6a65 6374 2d77   id="subobject-w
+000021e0: 6964 6765 7473 2d66 6f6f 6669 656c 6422  idgets-foofield"
+000021f0: 0a20 2020 2020 2020 2020 6e61 6d65 3d22  .         name="
+00002200: 7375 626f 626a 6563 742e 7769 6467 6574  subobject.widget
+00002210: 732e 666f 6f66 6965 6c64 220a 2020 2020  s.foofield".    
+00002220: 2020 2020 2063 6c61 7373 3d22 7465 7874       class="text
+00002230: 2d77 6964 6765 7420 7265 7175 6972 6564  -widget required
+00002240: 2069 6e74 2d66 6965 6c64 220a 2020 2020   int-field".    
+00002250: 2020 2020 2076 616c 7565 3d22 3222 202f       value="2" /
+00002260: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002270: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00002280: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00002290: 226c 6162 656c 223e 0a20 2020 2020 2020  "label">.       
+000022a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000022b0: 6c61 6265 6c20 666f 723d 2273 7562 6f62  label for="subob
+000022c0: 6a65 6374 2d77 6964 6765 7473 2d62 6172  ject-widgets-bar
+000022d0: 6669 656c 6422 3e0a 2020 2020 2020 2020  field">.        
 000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022f0: 2020 203c 7370 616e 3e4d 7920 6465 6172     <span>My dear
-00002300: 2062 6172 3c2f 7370 616e 3e0a 2020 2020   bar</span>.    
+000022f0: 2020 2020 2020 3c73 7061 6e3e 4d79 2064        <span>My d
+00002300: 6561 7220 6261 723c 2f73 7061 6e3e 0a20  ear bar</span>. 
 00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 2020 3c2f 6c61 6265 6c3e 0a20 2020 2020    </label>.     
-00002330: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00002340: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00002350: 6976 2063 6c61 7373 3d22 7769 6467 6574  iv class="widget
-00002360: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00002370: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-00002380: 7479 7065 3d22 7465 7874 220a 2020 2020  type="text".    
-00002390: 2020 2020 2069 643d 2273 7562 6f62 6a65       id="subobje
-000023a0: 6374 2d77 6964 6765 7473 2d62 6172 6669  ct-widgets-barfi
-000023b0: 656c 6422 0a20 2020 2020 2020 2020 6e61  eld".         na
-000023c0: 6d65 3d22 7375 626f 626a 6563 742e 7769  me="subobject.wi
-000023d0: 6467 6574 732e 6261 7266 6965 6c64 220a  dgets.barfield".
-000023e0: 2020 2020 2020 2020 2063 6c61 7373 3d22           class="
-000023f0: 7465 7874 2d77 6964 6765 7420 696e 742d  text-widget int-
-00002400: 6669 656c 6422 0a20 2020 2020 2020 2020  field".         
-00002410: 7661 6c75 653d 2239 3939 2220 2f3e 0a20  value="999" />. 
-00002420: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00002430: 6976 3e0a 2020 2020 2020 3c69 6e70 7574  iv>.      <input
-00002440: 206e 616d 653d 2273 7562 6f62 6a65 6374   name="subobject
-00002450: 2d65 6d70 7479 2d6d 6172 6b65 7222 2074  -empty-marker" t
-00002460: 7970 653d 2268 6964 6465 6e22 2076 616c  ype="hidden" val
-00002470: 7565 3d22 3122 2f3e 0a20 203c 2f64 6976  ue="1"/>.  </div
-00002480: 3e0a 0a42 7574 206f 6e20 7468 6520 7265  >..But on the re
-00002490: 7475 726e 2077 6520 6765 7420 6465 6661  turn we get defa
-000024a0: 756c 7420 7661 6c75 6573 2062 6163 6b3a  ult values back:
-000024b0: 0a0a 2020 3e3e 3e20 7070 7269 6e74 2877  ..  >>> pprint(w
-000024c0: 6964 6765 742e 7661 6c75 6529 0a20 207b  idget.value).  {
-000024d0: 2762 6172 6669 656c 6427 3a20 2739 3939  'barfield': '999
-000024e0: 272c 2027 666f 6f66 6965 6c64 273a 2027  ', 'foofield': '
-000024f0: 3227 7d0a 0a20 203e 3e3e 2076 616c 7565  2'}..  >>> value
-00002500: 203d 2063 6f6e 7665 7274 6572 2e74 6f5f   = converter.to_
-00002510: 6669 656c 645f 7661 6c75 6528 7769 6467  field_value(widg
-00002520: 6574 2e76 616c 7565 290a 2020 3e3e 3e20  et.value).  >>> 
-00002530: 7661 6c75 650a 2020 3c70 7961 6d73 5f66  value.  <pyams_f
-00002540: 6f72 6d2e 7465 7374 696e 672e 4d79 5375  orm.testing.MySu
-00002550: 624f 626a 6563 7420 6f62 6a65 6374 2061  bObject object a
-00002560: 7420 2e2e 2e3e 0a0a 484d 4d4d 4d2e 2e2e  t ...>..HMMMM...
-00002570: 2e20 646f 2077 6520 6861 7665 2074 6f20  . do we have to 
-00002580: 7465 7374 2065 7272 6f72 2068 616e 646c  test error handl
-00002590: 696e 6720 6865 7265 3f0a 4927 6d20 7465  ing here?.I'm te
-000025a0: 6d70 7465 6420 746f 206c 6561 7665 2069  mpted to leave i
-000025b0: 7420 6f75 7420 6173 206e 6f20 7769 6467  t out as no widg
-000025c0: 6574 7320 7365 656d 2074 6f20 646f 2074  ets seem to do t
-000025d0: 6869 732e 0a0a 0a49 6e20 666f 726d 730a  his....In forms.
-000025e0: 3d3d 3d3d 3d3d 3d3d 0a0a 446f 2061 6c6c  ========..Do all
-000025f0: 2074 6861 7420 6675 6e20 696e 2061 6464   that fun in add
-00002600: 2061 6e64 2065 6469 7420 666f 726d 7320   and edit forms 
-00002610: 746f 6f2e 0a0a 466f 726d 7320 616e 6420  too...Forms and 
-00002620: 6f75 7220 6f62 6a65 6374 7769 6467 6574  our objectwidget
-00002630: 2066 6972 6520 6576 656e 7473 206f 6e20   fire events on 
-00002640: 6164 6420 616e 6420 6564 6974 2c20 7365  add and edit, se
-00002650: 7475 7020 6120 7375 6273 6372 6962 6572  tup a subscriber
-00002660: 0a66 6f72 2074 686f 7365 3a0a 0a20 203e  .for those:..  >
-00002670: 3e3e 2065 7665 6e74 6c6f 6720 3d20 5b5d  >> eventlog = []
-00002680: 0a20 203e 3e3e 2069 6d70 6f72 7420 7a6f  .  >>> import zo
-00002690: 7065 2e6c 6966 6563 7963 6c65 6576 656e  pe.lifecycleeven
-000026a0: 740a 0a20 203e 3e3e 2064 6566 206c 6f67  t..  >>> def log
-000026b0: 4576 656e 7428 6576 656e 7429 3a0a 2020  Event(event):.  
-000026c0: 2e2e 2e20 2020 2020 6576 656e 746c 6f67  ...     eventlog
-000026d0: 2e61 7070 656e 6428 6576 656e 7429 0a20  .append(event). 
-000026e0: 203e 3e3e 205f 203d 2063 6f6e 6669 672e   >>> _ = config.
-000026f0: 6164 645f 7375 6273 6372 6962 6572 286c  add_subscriber(l
-00002700: 6f67 4576 656e 742c 207a 6f70 652e 6c69  ogEvent, zope.li
-00002710: 6665 6379 636c 6565 7665 6e74 2e69 6e74  fecycleevent.int
-00002720: 6572 6661 6365 732e 494f 626a 6563 744d  erfaces.IObjectM
-00002730: 6f64 6966 6965 6445 7665 6e74 290a 2020  odifiedEvent).  
-00002740: 3e3e 3e20 5f20 3d20 636f 6e66 6967 2e61  >>> _ = config.a
-00002750: 6464 5f73 7562 7363 7269 6265 7228 6c6f  dd_subscriber(lo
-00002760: 6745 7665 6e74 2c20 7a6f 7065 2e6c 6966  gEvent, zope.lif
-00002770: 6563 7963 6c65 6576 656e 742e 696e 7465  ecycleevent.inte
-00002780: 7266 6163 6573 2e49 4f62 6a65 6374 4372  rfaces.IObjectCr
-00002790: 6561 7465 6445 7665 6e74 290a 2020 3e3e  eatedEvent).  >>
-000027a0: 3e20 5f20 3d20 636f 6e66 6967 2e61 6464  > _ = config.add
-000027b0: 5f73 7562 7363 7269 6265 7228 6c6f 6745  _subscriber(logE
-000027c0: 7665 6e74 2c20 7a6f 7065 2e6c 6966 6563  vent, zope.lifec
-000027d0: 7963 6c65 6576 656e 742e 696e 7465 7266  ycleevent.interf
-000027e0: 6163 6573 2e49 4f62 6a65 6374 4164 6465  aces.IObjectAdde
-000027f0: 6445 7665 6e74 290a 0a20 203e 3e3e 2064  dEvent)..  >>> d
-00002800: 6566 206c 6f67 4576 656e 7432 2865 7665  ef logEvent2(eve
-00002810: 6e74 293a 0a20 202e 2e2e 2020 2020 2065  nt):.  ...     e
-00002820: 7665 6e74 6c6f 672e 6170 7065 6e64 2865  ventlog.append(e
-00002830: 7665 6e74 290a 0a20 2023 203e 3e3e 205f  vent)..  # >>> _
-00002840: 203d 2063 6f6e 6669 672e 6164 645f 7375   = config.add_su
-00002850: 6273 6372 6962 6572 286c 6f67 4576 656e  bscriber(logEven
-00002860: 7432 2c20 7a6f 7065 2e6c 6966 6563 7963  t2, zope.lifecyc
-00002870: 6c65 6576 656e 742e 696e 7465 7266 6163  leevent.interfac
-00002880: 6573 2e49 4f62 6a65 6374 4372 6561 7465  es.IObjectCreate
-00002890: 6445 7665 6e74 290a 0a20 203e 3e3e 2064  dEvent)..  >>> d
-000028a0: 6566 2070 7269 6e74 4576 656e 7473 2829  ef printEvents()
-000028b0: 3a0a 2020 2e2e 2e20 2020 2020 666f 7220  :.  ...     for 
-000028c0: 6576 656e 7420 696e 2065 7665 6e74 6c6f  event in eventlo
-000028d0: 673a 0a20 202e 2e2e 2020 2020 2020 2020  g:.  ...        
-000028e0: 2070 7269 6e74 2873 7472 2865 7665 6e74   print(str(event
-000028f0: 2929 0a20 202e 2e2e 2020 2020 2020 2020  )).  ...        
-00002900: 2069 6620 6973 696e 7374 616e 6365 2865   if isinstance(e
-00002910: 7665 6e74 2c20 7a6f 7065 2e6c 6966 6563  vent, zope.lifec
-00002920: 7963 6c65 6576 656e 742e 4f62 6a65 6374  ycleevent.Object
-00002930: 4d6f 6469 6669 6564 4576 656e 7429 3a0a  ModifiedEvent):.
-00002940: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
-00002950: 2020 666f 7220 6174 7472 2069 6e20 6576    for attr in ev
-00002960: 656e 742e 6465 7363 7269 7074 696f 6e73  ent.descriptions
-00002970: 3a0a 2020 2e2e 2e20 2020 2020 2020 2020  :.  ...         
-00002980: 2020 2020 2020 2020 7072 696e 7428 6174          print(at
-00002990: 7472 2e69 6e74 6572 6661 6365 290a 2020  tr.interface).  
-000029a0: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
-000029b0: 2020 2020 7072 696e 7428 736f 7274 6564      print(sorted
-000029c0: 2861 7474 722e 6174 7472 6962 7574 6573  (attr.attributes
-000029d0: 2929 0a0a 5765 2064 6566 696e 6520 616e  ))..We define an
-000029e0: 2069 6e74 6572 6661 6365 2063 6f6e 7461   interface conta
-000029f0: 696e 696e 6720 6120 7375 626f 626a 6563  ining a subobjec
-00002a00: 742c 2061 6e64 2061 6e20 6164 6466 6f72  t, and an addfor
-00002a10: 6d20 666f 7220 6974 3a0a 0a20 203e 3e3e  m for it:..  >>>
-00002a20: 2066 726f 6d20 7079 616d 735f 666f 726d   from pyams_form
-00002a30: 2069 6d70 6f72 7420 666f 726d 2c20 6669   import form, fi
-00002a40: 656c 640a 2020 3e3e 3e20 6672 6f6d 2070  eld.  >>> from p
-00002a50: 7961 6d73 5f66 6f72 6d2e 7465 7374 696e  yams_form.testin
-00002a60: 6720 696d 706f 7274 204d 794f 626a 6563  g import MyObjec
-00002a70: 742c 2049 4d79 4f62 6a65 6374 0a0a 4e6f  t, IMyObject..No
-00002a80: 7465 2c20 7468 6174 2063 7265 6174 696e  te, that creatin
-00002a90: 6720 616e 206f 626a 6563 7420 7769 6c6c  g an object will
-00002aa0: 2070 7269 6e74 2073 6f6d 6520 696e 666f   print some info
-00002ab0: 726d 6174 696f 6e20 6162 6f75 7420 6974  rmation about it
-00002ac0: 3a0a 0a20 203e 3e3e 2063 6c61 7373 204d  :..  >>> class M
-00002ad0: 7941 6464 466f 726d 2866 6f72 6d2e 4164  yAddForm(form.Ad
-00002ae0: 6446 6f72 6d29 3a0a 2020 2e2e 2e20 2020  dForm):.  ...   
-00002af0: 2020 6669 656c 6473 203d 2066 6965 6c64    fields = field
-00002b00: 2e46 6965 6c64 7328 494d 794f 626a 6563  .Fields(IMyObjec
-00002b10: 7429 0a20 202e 2e2e 2020 2020 2064 6566  t).  ...     def
-00002b20: 2063 7265 6174 6528 7365 6c66 2c20 6461   create(self, da
-00002b30: 7461 293a 0a20 202e 2e2e 2020 2020 2020  ta):.  ...      
-00002b40: 2020 2070 7269 6e74 2822 4d79 4164 6446     print("MyAddF
-00002b50: 6f72 6d2e 6372 6561 7465 2229 0a20 202e  orm.create").  .
-00002b60: 2e2e 2020 2020 2020 2020 2070 7072 696e  ..         pprin
-00002b70: 7428 6461 7461 290a 2020 2e2e 2e20 2020  t(data).  ...   
-00002b80: 2020 2020 2020 7265 7475 726e 204d 794f        return MyO
-00002b90: 626a 6563 7428 2a2a 6461 7461 290a 2020  bject(**data).  
-00002ba0: 2e2e 2e20 2020 2020 6465 6620 6164 6428  ...     def add(
-00002bb0: 7365 6c66 2c20 6f62 6a29 3a0a 2020 2e2e  self, obj):.  ..
-00002bc0: 2e20 2020 2020 2020 2020 7365 6c66 2e63  .         self.c
-00002bd0: 6f6e 7465 7874 5b6f 626a 2e6e 616d 655d  ontext[obj.name]
-00002be0: 203d 206f 626a 0a20 202e 2e2e 2020 2020   = obj.  ...    
-00002bf0: 2064 6566 206e 6578 745f 7572 6c28 7365   def next_url(se
-00002c00: 6c66 293a 0a20 202e 2e2e 2020 2020 2020  lf):.  ...      
-00002c10: 2020 2070 6173 730a 0a57 6520 6372 6561     pass..We crea
-00002c20: 7465 2074 6865 2066 6f72 6d20 616e 6420  te the form and 
-00002c30: 7472 7920 746f 2075 7064 6174 6520 6974  try to update it
-00002c40: 3a0a 0a20 203e 3e3e 2066 726f 6d20 7a6f  :..  >>> from zo
-00002c50: 7065 2e63 6f6e 7461 696e 6572 2e66 6f6c  pe.container.fol
-00002c60: 6465 7220 696d 706f 7274 2046 6f6c 6465  der import Folde
-00002c70: 720a 2020 3e3e 3e20 726f 6f74 203d 2046  r.  >>> root = F
-00002c80: 6f6c 6465 7228 290a 2020 3e3e 3e20 7265  older().  >>> re
-00002c90: 7175 6573 7420 3d20 5465 7374 5265 7175  quest = TestRequ
-00002ca0: 6573 7428 290a 2020 3e3e 3e20 6d79 6164  est().  >>> myad
-00002cb0: 6466 6f72 6d20 3d20 204d 7941 6464 466f  dform =  MyAddFo
-00002cc0: 726d 2872 6f6f 742c 2072 6571 7565 7374  rm(root, request
-00002cd0: 290a 0a20 203e 3e3e 206d 7961 6464 666f  )..  >>> myaddfo
-00002ce0: 726d 2e75 7064 6174 6528 290a 0a41 7320  rm.update()..As 
-00002cf0: 7573 7561 6c2c 2074 6865 2066 6f72 6d20  usual, the form 
-00002d00: 636f 6e74 6169 6e73 2061 2077 6964 6765  contains a widge
-00002d10: 7420 6d61 6e61 6765 7220 7769 7468 2074  t manager with t
-00002d20: 6865 2065 7870 6563 7465 6420 7769 6467  he expected widg
-00002d30: 6574 0a0a 2020 3e3e 3e20 6c69 7374 286d  et..  >>> list(m
-00002d40: 7961 6464 666f 726d 2e77 6964 6765 7473  yaddform.widgets
-00002d50: 2e6b 6579 7328 2929 0a20 205b 2773 7562  .keys()).  ['sub
-00002d60: 6f62 6a65 6374 272c 2027 6e61 6d65 275d  object', 'name']
-00002d70: 0a20 203e 3e3e 206c 6973 7428 6d79 6164  .  >>> list(myad
-00002d80: 6466 6f72 6d2e 7769 6467 6574 732e 7661  dform.widgets.va
-00002d90: 6c75 6573 2829 290a 2020 5b3c 4f62 6a65  lues()).  [<Obje
-00002da0: 6374 5769 6467 6574 2027 666f 726d 2e77  ctWidget 'form.w
-00002db0: 6964 6765 7473 2e73 7562 6f62 6a65 6374  idgets.subobject
-00002dc0: 273e 2c20 3c54 6578 7457 6964 6765 7420  '>, <TextWidget 
-00002dd0: 2766 6f72 6d2e 7769 6467 6574 732e 6e61  'form.widgets.na
-00002de0: 6d65 273e 5d0a 0a54 6865 2077 6964 6765  me'>]..The widge
-00002df0: 7420 6861 7320 7375 622d 7769 6467 6574  t has sub-widget
-00002e00: 733a 0a0a 2020 3e3e 3e20 6c69 7374 286d  s:..  >>> list(m
-00002e10: 7961 6464 666f 726d 2e77 6964 6765 7473  yaddform.widgets
-00002e20: 5b27 7375 626f 626a 6563 7427 5d2e 7769  ['subobject'].wi
-00002e30: 6467 6574 732e 6b65 7973 2829 290a 2020  dgets.keys()).  
-00002e40: 5b27 666f 6f66 6965 6c64 272c 2027 6261  ['foofield', 'ba
-00002e50: 7266 6965 6c64 275d 0a0a 4966 2077 6520  rfield']..If we 
-00002e60: 7761 6e74 2074 6f20 7265 6e64 6572 2074  want to render t
-00002e70: 6865 2061 6464 666f 726d 2c20 7765 206d  he addform, we m
-00002e80: 7573 7420 6769 7665 2069 7420 6120 7465  ust give it a te
-00002e90: 6d70 6c61 7465 3a0a 0a20 203e 3e3e 2069  mplate:..  >>> i
-00002ea0: 6d70 6f72 7420 6f73 0a20 203e 3e3e 2066  mport os.  >>> f
-00002eb0: 726f 6d20 7079 616d 735f 7465 6d70 6c61  rom pyams_templa
-00002ec0: 7465 2e69 6e74 6572 6661 6365 7320 696d  te.interfaces im
-00002ed0: 706f 7274 2049 436f 6e74 656e 7454 656d  port IContentTem
-00002ee0: 706c 6174 650a 2020 3e3e 3e20 6672 6f6d  plate.  >>> from
-00002ef0: 2070 7961 6d73 5f74 656d 706c 6174 652e   pyams_template.
-00002f00: 7465 6d70 6c61 7465 2069 6d70 6f72 7420  template import 
-00002f10: 5465 6d70 6c61 7465 4661 6374 6f72 790a  TemplateFactory.
-00002f20: 2020 3e3e 3e20 6672 6f6d 2070 7961 6d73    >>> from pyams
-00002f30: 5f6c 6179 6572 2e69 6e74 6572 6661 6365  _layer.interface
-00002f40: 7320 696d 706f 7274 2049 466f 726d 4c61  s import IFormLa
-00002f50: 7965 720a 2020 3e3e 3e20 6672 6f6d 2070  yer.  >>> from p
-00002f60: 7961 6d73 5f66 6f72 6d20 696d 706f 7274  yams_form import
-00002f70: 2069 6e74 6572 6661 6365 732c 2074 6573   interfaces, tes
-00002f80: 7473 0a20 203e 3e3e 2064 6566 2061 6464  ts.  >>> def add
-00002f90: 5465 6d70 6c61 7465 2866 6f72 6d29 3a0a  Template(form):.
-00002fa0: 2020 2e2e 2e20 2020 2020 6661 6374 6f72    ...     factor
-00002fb0: 7920 3d20 5465 6d70 6c61 7465 4661 6374  y = TemplateFact
-00002fc0: 6f72 7928 6f73 2e70 6174 682e 6a6f 696e  ory(os.path.join
-00002fd0: 286f 732e 7061 7468 2e64 6972 6e61 6d65  (os.path.dirname
-00002fe0: 2874 6573 7473 2e5f 5f66 696c 655f 5f29  (tests.__file__)
-00002ff0: 2c0a 2020 2e2e 2e20 2020 2020 2020 2020  ,.  ...         
+00002320: 2020 2020 203c 2f6c 6162 656c 3e0a 2020       </label>.  
+00002330: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00002340: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00002350: 203c 6469 7620 636c 6173 733d 2277 6964   <div class="wid
+00002360: 6765 7422 3e0a 2020 2020 2020 2020 2020  get">.          
+00002370: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
+00002380: 7574 2074 7970 653d 2274 6578 7422 0a20  ut type="text". 
+00002390: 2020 2020 2020 2020 6964 3d22 7375 626f          id="subo
+000023a0: 626a 6563 742d 7769 6467 6574 732d 6261  bject-widgets-ba
+000023b0: 7266 6965 6c64 220a 2020 2020 2020 2020  rfield".        
+000023c0: 206e 616d 653d 2273 7562 6f62 6a65 6374   name="subobject
+000023d0: 2e77 6964 6765 7473 2e62 6172 6669 656c  .widgets.barfiel
+000023e0: 6422 0a20 2020 2020 2020 2020 636c 6173  d".         clas
+000023f0: 733d 2274 6578 742d 7769 6467 6574 2069  s="text-widget i
+00002400: 6e74 2d66 6965 6c64 220a 2020 2020 2020  nt-field".      
+00002410: 2020 2076 616c 7565 3d22 3939 3922 202f     value="999" /
+00002420: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002430: 3c2f 6469 763e 0a20 2020 2020 203c 696e  </div>.      <in
+00002440: 7075 7420 6e61 6d65 3d22 7375 626f 626a  put name="subobj
+00002450: 6563 742d 656d 7074 792d 6d61 726b 6572  ect-empty-marker
+00002460: 2220 7479 7065 3d22 6869 6464 656e 2220  " type="hidden" 
+00002470: 7661 6c75 653d 2231 2220 2f3e 0a20 203c  value="1" />.  <
+00002480: 2f64 6976 3e0a 0a42 7574 206f 6e20 7468  /div>..But on th
+00002490: 6520 7265 7475 726e 2077 6520 6765 7420  e return we get 
+000024a0: 6465 6661 756c 7420 7661 6c75 6573 2062  default values b
+000024b0: 6163 6b3a 0a0a 2020 3e3e 3e20 7070 7269  ack:..  >>> ppri
+000024c0: 6e74 2877 6964 6765 742e 7661 6c75 6529  nt(widget.value)
+000024d0: 0a20 207b 2762 6172 6669 656c 6427 3a20  .  {'barfield': 
+000024e0: 2739 3939 272c 2027 666f 6f66 6965 6c64  '999', 'foofield
+000024f0: 273a 2027 3227 7d0a 0a20 203e 3e3e 2076  ': '2'}..  >>> v
+00002500: 616c 7565 203d 2063 6f6e 7665 7274 6572  alue = converter
+00002510: 2e74 6f5f 6669 656c 645f 7661 6c75 6528  .to_field_value(
+00002520: 7769 6467 6574 2e76 616c 7565 290a 2020  widget.value).  
+00002530: 3e3e 3e20 7661 6c75 650a 2020 3c70 7961  >>> value.  <pya
+00002540: 6d73 5f66 6f72 6d2e 7465 7374 696e 672e  ms_form.testing.
+00002550: 4d79 5375 624f 626a 6563 7420 6f62 6a65  MySubObject obje
+00002560: 6374 2061 7420 2e2e 2e3e 0a0a 484d 4d4d  ct at ...>..HMMM
+00002570: 4d2e 2e2e 2e20 646f 2077 6520 6861 7665  M.... do we have
+00002580: 2074 6f20 7465 7374 2065 7272 6f72 2068   to test error h
+00002590: 616e 646c 696e 6720 6865 7265 3f0a 4927  andling here?.I'
+000025a0: 6d20 7465 6d70 7465 6420 746f 206c 6561  m tempted to lea
+000025b0: 7665 2069 7420 6f75 7420 6173 206e 6f20  ve it out as no 
+000025c0: 7769 6467 6574 7320 7365 656d 2074 6f20  widgets seem to 
+000025d0: 646f 2074 6869 732e 0a0a 0a49 6e20 666f  do this....In fo
+000025e0: 726d 730a 3d3d 3d3d 3d3d 3d3d 0a0a 446f  rms.========..Do
+000025f0: 2061 6c6c 2074 6861 7420 6675 6e20 696e   all that fun in
+00002600: 2061 6464 2061 6e64 2065 6469 7420 666f   add and edit fo
+00002610: 726d 7320 746f 6f2e 0a0a 466f 726d 7320  rms too...Forms 
+00002620: 616e 6420 6f75 7220 6f62 6a65 6374 7769  and our objectwi
+00002630: 6467 6574 2066 6972 6520 6576 656e 7473  dget fire events
+00002640: 206f 6e20 6164 6420 616e 6420 6564 6974   on add and edit
+00002650: 2c20 7365 7475 7020 6120 7375 6273 6372  , setup a subscr
+00002660: 6962 6572 0a66 6f72 2074 686f 7365 3a0a  iber.for those:.
+00002670: 0a20 203e 3e3e 2065 7665 6e74 6c6f 6720  .  >>> eventlog 
+00002680: 3d20 5b5d 0a20 203e 3e3e 2069 6d70 6f72  = [].  >>> impor
+00002690: 7420 7a6f 7065 2e6c 6966 6563 7963 6c65  t zope.lifecycle
+000026a0: 6576 656e 740a 0a20 203e 3e3e 2064 6566  event..  >>> def
+000026b0: 206c 6f67 4576 656e 7428 6576 656e 7429   logEvent(event)
+000026c0: 3a0a 2020 2e2e 2e20 2020 2020 6576 656e  :.  ...     even
+000026d0: 746c 6f67 2e61 7070 656e 6428 6576 656e  tlog.append(even
+000026e0: 7429 0a20 203e 3e3e 205f 203d 2063 6f6e  t).  >>> _ = con
+000026f0: 6669 672e 6164 645f 7375 6273 6372 6962  fig.add_subscrib
+00002700: 6572 286c 6f67 4576 656e 742c 207a 6f70  er(logEvent, zop
+00002710: 652e 6c69 6665 6379 636c 6565 7665 6e74  e.lifecycleevent
+00002720: 2e69 6e74 6572 6661 6365 732e 494f 626a  .interfaces.IObj
+00002730: 6563 744d 6f64 6966 6965 6445 7665 6e74  ectModifiedEvent
+00002740: 290a 2020 3e3e 3e20 5f20 3d20 636f 6e66  ).  >>> _ = conf
+00002750: 6967 2e61 6464 5f73 7562 7363 7269 6265  ig.add_subscribe
+00002760: 7228 6c6f 6745 7665 6e74 2c20 7a6f 7065  r(logEvent, zope
+00002770: 2e6c 6966 6563 7963 6c65 6576 656e 742e  .lifecycleevent.
+00002780: 696e 7465 7266 6163 6573 2e49 4f62 6a65  interfaces.IObje
+00002790: 6374 4372 6561 7465 6445 7665 6e74 290a  ctCreatedEvent).
+000027a0: 2020 3e3e 3e20 5f20 3d20 636f 6e66 6967    >>> _ = config
+000027b0: 2e61 6464 5f73 7562 7363 7269 6265 7228  .add_subscriber(
+000027c0: 6c6f 6745 7665 6e74 2c20 7a6f 7065 2e6c  logEvent, zope.l
+000027d0: 6966 6563 7963 6c65 6576 656e 742e 696e  ifecycleevent.in
+000027e0: 7465 7266 6163 6573 2e49 4f62 6a65 6374  terfaces.IObject
+000027f0: 4164 6465 6445 7665 6e74 290a 0a20 203e  AddedEvent)..  >
+00002800: 3e3e 2064 6566 206c 6f67 4576 656e 7432  >> def logEvent2
+00002810: 2865 7665 6e74 293a 0a20 202e 2e2e 2020  (event):.  ...  
+00002820: 2020 2065 7665 6e74 6c6f 672e 6170 7065     eventlog.appe
+00002830: 6e64 2865 7665 6e74 290a 0a20 2023 203e  nd(event)..  # >
+00002840: 3e3e 205f 203d 2063 6f6e 6669 672e 6164  >> _ = config.ad
+00002850: 645f 7375 6273 6372 6962 6572 286c 6f67  d_subscriber(log
+00002860: 4576 656e 7432 2c20 7a6f 7065 2e6c 6966  Event2, zope.lif
+00002870: 6563 7963 6c65 6576 656e 742e 696e 7465  ecycleevent.inte
+00002880: 7266 6163 6573 2e49 4f62 6a65 6374 4372  rfaces.IObjectCr
+00002890: 6561 7465 6445 7665 6e74 290a 0a20 203e  eatedEvent)..  >
+000028a0: 3e3e 2064 6566 2070 7269 6e74 4576 656e  >> def printEven
+000028b0: 7473 2829 3a0a 2020 2e2e 2e20 2020 2020  ts():.  ...     
+000028c0: 666f 7220 6576 656e 7420 696e 2065 7665  for event in eve
+000028d0: 6e74 6c6f 673a 0a20 202e 2e2e 2020 2020  ntlog:.  ...    
+000028e0: 2020 2020 2070 7269 6e74 2873 7472 2865       print(str(e
+000028f0: 7665 6e74 2929 0a20 202e 2e2e 2020 2020  vent)).  ...    
+00002900: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00002910: 6365 2865 7665 6e74 2c20 7a6f 7065 2e6c  ce(event, zope.l
+00002920: 6966 6563 7963 6c65 6576 656e 742e 4f62  ifecycleevent.Ob
+00002930: 6a65 6374 4d6f 6469 6669 6564 4576 656e  jectModifiedEven
+00002940: 7429 3a0a 2020 2e2e 2e20 2020 2020 2020  t):.  ...       
+00002950: 2020 2020 2020 666f 7220 6174 7472 2069        for attr i
+00002960: 6e20 6576 656e 742e 6465 7363 7269 7074  n event.descript
+00002970: 696f 6e73 3a0a 2020 2e2e 2e20 2020 2020  ions:.  ...     
+00002980: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00002990: 7428 6174 7472 2e69 6e74 6572 6661 6365  t(attr.interface
+000029a0: 290a 2020 2e2e 2e20 2020 2020 2020 2020  ).  ...         
+000029b0: 2020 2020 2020 2020 7072 696e 7428 736f          print(so
+000029c0: 7274 6564 2861 7474 722e 6174 7472 6962  rted(attr.attrib
+000029d0: 7574 6573 2929 0a0a 5765 2064 6566 696e  utes))..We defin
+000029e0: 6520 616e 2069 6e74 6572 6661 6365 2063  e an interface c
+000029f0: 6f6e 7461 696e 696e 6720 6120 7375 626f  ontaining a subo
+00002a00: 626a 6563 742c 2061 6e64 2061 6e20 6164  bject, and an ad
+00002a10: 6466 6f72 6d20 666f 7220 6974 3a0a 0a20  dform for it:.. 
+00002a20: 203e 3e3e 2066 726f 6d20 7079 616d 735f   >>> from pyams_
+00002a30: 666f 726d 2069 6d70 6f72 7420 666f 726d  form import form
+00002a40: 2c20 6669 656c 640a 2020 3e3e 3e20 6672  , field.  >>> fr
+00002a50: 6f6d 2070 7961 6d73 5f66 6f72 6d2e 7465  om pyams_form.te
+00002a60: 7374 696e 6720 696d 706f 7274 204d 794f  sting import MyO
+00002a70: 626a 6563 742c 2049 4d79 4f62 6a65 6374  bject, IMyObject
+00002a80: 0a0a 4e6f 7465 2c20 7468 6174 2063 7265  ..Note, that cre
+00002a90: 6174 696e 6720 616e 206f 626a 6563 7420  ating an object 
+00002aa0: 7769 6c6c 2070 7269 6e74 2073 6f6d 6520  will print some 
+00002ab0: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00002ac0: 7420 6974 3a0a 0a20 203e 3e3e 2063 6c61  t it:..  >>> cla
+00002ad0: 7373 204d 7941 6464 466f 726d 2866 6f72  ss MyAddForm(for
+00002ae0: 6d2e 4164 6446 6f72 6d29 3a0a 2020 2e2e  m.AddForm):.  ..
+00002af0: 2e20 2020 2020 6669 656c 6473 203d 2066  .     fields = f
+00002b00: 6965 6c64 2e46 6965 6c64 7328 494d 794f  ield.Fields(IMyO
+00002b10: 626a 6563 7429 0a20 202e 2e2e 2020 2020  bject).  ...    
+00002b20: 2064 6566 2063 7265 6174 6528 7365 6c66   def create(self
+00002b30: 2c20 6461 7461 293a 0a20 202e 2e2e 2020  , data):.  ...  
+00002b40: 2020 2020 2020 2070 7269 6e74 2822 4d79         print("My
+00002b50: 4164 6446 6f72 6d2e 6372 6561 7465 2229  AddForm.create")
+00002b60: 0a20 202e 2e2e 2020 2020 2020 2020 2070  .  ...         p
+00002b70: 7072 696e 7428 6461 7461 290a 2020 2e2e  print(data).  ..
+00002b80: 2e20 2020 2020 2020 2020 7265 7475 726e  .         return
+00002b90: 204d 794f 626a 6563 7428 2a2a 6461 7461   MyObject(**data
+00002ba0: 290a 2020 2e2e 2e20 2020 2020 6465 6620  ).  ...     def 
+00002bb0: 6164 6428 7365 6c66 2c20 6f62 6a29 3a0a  add(self, obj):.
+00002bc0: 2020 2e2e 2e20 2020 2020 2020 2020 7365    ...         se
+00002bd0: 6c66 2e63 6f6e 7465 7874 5b6f 626a 2e6e  lf.context[obj.n
+00002be0: 616d 655d 203d 206f 626a 0a20 202e 2e2e  ame] = obj.  ...
+00002bf0: 2020 2020 2064 6566 206e 6578 745f 7572       def next_ur
+00002c00: 6c28 7365 6c66 293a 0a20 202e 2e2e 2020  l(self):.  ...  
+00002c10: 2020 2020 2020 2070 6173 730a 0a57 6520         pass..We 
+00002c20: 6372 6561 7465 2074 6865 2066 6f72 6d20  create the form 
+00002c30: 616e 6420 7472 7920 746f 2075 7064 6174  and try to updat
+00002c40: 6520 6974 3a0a 0a20 203e 3e3e 2066 726f  e it:..  >>> fro
+00002c50: 6d20 7a6f 7065 2e63 6f6e 7461 696e 6572  m zope.container
+00002c60: 2e66 6f6c 6465 7220 696d 706f 7274 2046  .folder import F
+00002c70: 6f6c 6465 720a 2020 3e3e 3e20 726f 6f74  older.  >>> root
+00002c80: 203d 2046 6f6c 6465 7228 290a 2020 3e3e   = Folder().  >>
+00002c90: 3e20 7265 7175 6573 7420 3d20 5465 7374  > request = Test
+00002ca0: 5265 7175 6573 7428 290a 2020 3e3e 3e20  Request().  >>> 
+00002cb0: 6d79 6164 6466 6f72 6d20 3d20 204d 7941  myaddform =  MyA
+00002cc0: 6464 466f 726d 2872 6f6f 742c 2072 6571  ddForm(root, req
+00002cd0: 7565 7374 290a 0a20 203e 3e3e 206d 7961  uest)..  >>> mya
+00002ce0: 6464 666f 726d 2e75 7064 6174 6528 290a  ddform.update().
+00002cf0: 0a41 7320 7573 7561 6c2c 2074 6865 2066  .As usual, the f
+00002d00: 6f72 6d20 636f 6e74 6169 6e73 2061 2077  orm contains a w
+00002d10: 6964 6765 7420 6d61 6e61 6765 7220 7769  idget manager wi
+00002d20: 7468 2074 6865 2065 7870 6563 7465 6420  th the expected 
+00002d30: 7769 6467 6574 0a0a 2020 3e3e 3e20 6c69  widget..  >>> li
+00002d40: 7374 286d 7961 6464 666f 726d 2e77 6964  st(myaddform.wid
+00002d50: 6765 7473 2e6b 6579 7328 2929 0a20 205b  gets.keys()).  [
+00002d60: 2773 7562 6f62 6a65 6374 272c 2027 6e61  'subobject', 'na
+00002d70: 6d65 275d 0a20 203e 3e3e 206c 6973 7428  me'].  >>> list(
+00002d80: 6d79 6164 6466 6f72 6d2e 7769 6467 6574  myaddform.widget
+00002d90: 732e 7661 6c75 6573 2829 290a 2020 5b3c  s.values()).  [<
+00002da0: 4f62 6a65 6374 5769 6467 6574 2027 666f  ObjectWidget 'fo
+00002db0: 726d 2e77 6964 6765 7473 2e73 7562 6f62  rm.widgets.subob
+00002dc0: 6a65 6374 273e 2c20 3c54 6578 7457 6964  ject'>, <TextWid
+00002dd0: 6765 7420 2766 6f72 6d2e 7769 6467 6574  get 'form.widget
+00002de0: 732e 6e61 6d65 273e 5d0a 0a54 6865 2077  s.name'>]..The w
+00002df0: 6964 6765 7420 6861 7320 7375 622d 7769  idget has sub-wi
+00002e00: 6467 6574 733a 0a0a 2020 3e3e 3e20 6c69  dgets:..  >>> li
+00002e10: 7374 286d 7961 6464 666f 726d 2e77 6964  st(myaddform.wid
+00002e20: 6765 7473 5b27 7375 626f 626a 6563 7427  gets['subobject'
+00002e30: 5d2e 7769 6467 6574 732e 6b65 7973 2829  ].widgets.keys()
+00002e40: 290a 2020 5b27 666f 6f66 6965 6c64 272c  ).  ['foofield',
+00002e50: 2027 6261 7266 6965 6c64 275d 0a0a 4966   'barfield']..If
+00002e60: 2077 6520 7761 6e74 2074 6f20 7265 6e64   we want to rend
+00002e70: 6572 2074 6865 2061 6464 666f 726d 2c20  er the addform, 
+00002e80: 7765 206d 7573 7420 6769 7665 2069 7420  we must give it 
+00002e90: 6120 7465 6d70 6c61 7465 3a0a 0a20 203e  a template:..  >
+00002ea0: 3e3e 2069 6d70 6f72 7420 6f73 0a20 203e  >> import os.  >
+00002eb0: 3e3e 2066 726f 6d20 7079 616d 735f 7465  >> from pyams_te
+00002ec0: 6d70 6c61 7465 2e69 6e74 6572 6661 6365  mplate.interface
+00002ed0: 7320 696d 706f 7274 2049 436f 6e74 656e  s import IConten
+00002ee0: 7454 656d 706c 6174 650a 2020 3e3e 3e20  tTemplate.  >>> 
+00002ef0: 6672 6f6d 2070 7961 6d73 5f74 656d 706c  from pyams_templ
+00002f00: 6174 652e 7465 6d70 6c61 7465 2069 6d70  ate.template imp
+00002f10: 6f72 7420 5465 6d70 6c61 7465 4661 6374  ort TemplateFact
+00002f20: 6f72 790a 2020 3e3e 3e20 6672 6f6d 2070  ory.  >>> from p
+00002f30: 7961 6d73 5f6c 6179 6572 2e69 6e74 6572  yams_layer.inter
+00002f40: 6661 6365 7320 696d 706f 7274 2049 466f  faces import IFo
+00002f50: 726d 4c61 7965 720a 2020 3e3e 3e20 6672  rmLayer.  >>> fr
+00002f60: 6f6d 2070 7961 6d73 5f66 6f72 6d20 696d  om pyams_form im
+00002f70: 706f 7274 2069 6e74 6572 6661 6365 732c  port interfaces,
+00002f80: 2074 6573 7473 0a20 203e 3e3e 2064 6566   tests.  >>> def
+00002f90: 2061 6464 5465 6d70 6c61 7465 2866 6f72   addTemplate(for
+00002fa0: 6d29 3a0a 2020 2e2e 2e20 2020 2020 6661  m):.  ...     fa
+00002fb0: 6374 6f72 7920 3d20 5465 6d70 6c61 7465  ctory = Template
+00002fc0: 4661 6374 6f72 7928 6f73 2e70 6174 682e  Factory(os.path.
+00002fd0: 6a6f 696e 286f 732e 7061 7468 2e64 6972  join(os.path.dir
+00002fe0: 6e61 6d65 2874 6573 7473 2e5f 5f66 696c  name(tests.__fil
+00002ff0: 655f 5f29 2c0a 2020 2e2e 2e20 2020 2020  e__),.  ...     
 00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 2020 2020 2020 2774 656d 706c 6174 6573        'templates
-00003020: 272c 2027 7369 6d70 6c65 2d65 6469 742e  ', 'simple-edit.
-00003030: 7074 2729 2c20 2774 6578 742f 6874 6d6c  pt'), 'text/html
-00003040: 2729 0a20 202e 2e2e 2020 2020 2063 6f6e  ').  ...     con
-00003050: 6669 672e 7265 6769 7374 7279 2e72 6567  fig.registry.reg
-00003060: 6973 7465 7241 6461 7074 6572 2866 6163  isterAdapter(fac
-00003070: 746f 7279 2c20 284e 6f6e 652c 2049 466f  tory, (None, IFo
-00003080: 726d 4c61 7965 722c 2066 6f72 6d2e 5f5f  rmLayer, form.__
-00003090: 636c 6173 735f 5f29 2c0a 2020 2e2e 2e20  class__),.  ... 
-000030a0: 2020 2020 2020 2020 2020 4943 6f6e 7465            IConte
-000030b0: 6e74 5465 6d70 6c61 7465 290a 2020 3e3e  ntTemplate).  >>
-000030c0: 3e20 6164 6454 656d 706c 6174 6528 6d79  > addTemplate(my
-000030d0: 6164 6466 6f72 6d29 0a0a 4e6f 7720 7265  addform)..Now re
-000030e0: 6e64 6572 696e 6720 7468 6520 6164 6466  ndering the addf
-000030f0: 6f72 6d20 7265 6e64 6572 7320 7468 6520  orm renders the 
-00003100: 7375 6266 6f72 6d20 6173 2077 656c 6c3a  subform as well:
-00003110: 0a0a 2020 3e3e 3e20 7072 696e 7428 666f  ..  >>> print(fo
-00003120: 726d 6174 5f68 746d 6c28 6d79 6164 6466  rmat_html(myaddf
-00003130: 6f72 6d2e 7265 6e64 6572 2829 2929 0a20  orm.render())). 
-00003140: 203c 666f 726d 2061 6374 696f 6e3d 222e   <form action=".
-00003150: 223e 0a20 2020 203c 6469 7620 636c 6173  ">.    <div clas
-00003160: 733d 2272 6f77 223e 0a20 2020 2020 203c  s="row">.      <
-00003170: 6c61 6265 6c20 666f 723d 2266 6f72 6d2d  label for="form-
-00003180: 7769 6467 6574 732d 7375 626f 626a 6563  widgets-subobjec
-00003190: 7422 3e6d 7920 6f62 6a65 6374 3c2f 6c61  t">my object</la
-000031a0: 6265 6c3e 0a20 2020 2020 203c 6469 7620  bel>.      <div 
-000031b0: 636c 6173 733d 226f 626a 6563 742d 7769  class="object-wi
-000031c0: 6467 6574 2072 6571 7569 7265 6422 3e0a  dget required">.
-000031d0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000031e0: 6976 2063 6c61 7373 3d22 6c61 6265 6c22  iv class="label"
-000031f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00003200: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
-00003210: 6f72 3d22 666f 726d 2d77 6964 6765 7473  or="form-widgets
-00003220: 2d73 7562 6f62 6a65 6374 2d77 6964 6765  -subobject-widge
-00003230: 7473 2d66 6f6f 6669 656c 6422 3e0a 2020  ts-foofield">.  
-00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003250: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
-00003260: 6e3e 4d79 2066 6f6f 2066 6965 6c64 3c2f  n>My foo field</
-00003270: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
+00003010: 2020 2020 2020 2020 2020 2774 656d 706c            'templ
+00003020: 6174 6573 272c 2027 7369 6d70 6c65 2d65  ates', 'simple-e
+00003030: 6469 742e 7074 2729 2c20 2774 6578 742f  dit.pt'), 'text/
+00003040: 6874 6d6c 2729 0a20 202e 2e2e 2020 2020  html').  ...    
+00003050: 2063 6f6e 6669 672e 7265 6769 7374 7279   config.registry
+00003060: 2e72 6567 6973 7465 7241 6461 7074 6572  .registerAdapter
+00003070: 2866 6163 746f 7279 2c20 284e 6f6e 652c  (factory, (None,
+00003080: 2049 466f 726d 4c61 7965 722c 2066 6f72   IFormLayer, for
+00003090: 6d2e 5f5f 636c 6173 735f 5f29 2c0a 2020  m.__class__),.  
+000030a0: 2e2e 2e20 2020 2020 2020 2020 2020 4943  ...           IC
+000030b0: 6f6e 7465 6e74 5465 6d70 6c61 7465 290a  ontentTemplate).
+000030c0: 2020 3e3e 3e20 6164 6454 656d 706c 6174    >>> addTemplat
+000030d0: 6528 6d79 6164 6466 6f72 6d29 0a0a 4e6f  e(myaddform)..No
+000030e0: 7720 7265 6e64 6572 696e 6720 7468 6520  w rendering the 
+000030f0: 6164 6466 6f72 6d20 7265 6e64 6572 7320  addform renders 
+00003100: 7468 6520 7375 6266 6f72 6d20 6173 2077  the subform as w
+00003110: 656c 6c3a 0a0a 2020 3e3e 3e20 7072 696e  ell:..  >>> prin
+00003120: 7428 666f 726d 6174 5f68 746d 6c28 6d79  t(format_html(my
+00003130: 6164 6466 6f72 6d2e 7265 6e64 6572 2829  addform.render()
+00003140: 2929 0a20 203c 666f 726d 2061 6374 696f  )).  <form actio
+00003150: 6e3d 222e 223e 0a20 2020 203c 6469 7620  n=".">.    <div 
+00003160: 636c 6173 733d 2272 6f77 223e 0a20 2020  class="row">.   
+00003170: 2020 203c 6c61 6265 6c20 666f 723d 2266     <label for="f
+00003180: 6f72 6d2d 7769 6467 6574 732d 7375 626f  orm-widgets-subo
+00003190: 626a 6563 7422 3e6d 7920 6f62 6a65 6374  bject">my object
+000031a0: 3c2f 6c61 6265 6c3e 0a20 2020 2020 203c  </label>.      <
+000031b0: 6469 7620 636c 6173 733d 226f 626a 6563  div class="objec
+000031c0: 742d 7769 6467 6574 2072 6571 7569 7265  t-widget require
+000031d0: 6422 3e0a 2020 2020 2020 2020 2020 2020  d">.            
+000031e0: 2020 3c64 6976 2063 6c61 7373 3d22 6c61    <div class="la
+000031f0: 6265 6c22 3e0a 2020 2020 2020 2020 2020  bel">.          
+00003200: 2020 2020 2020 2020 2020 2020 3c6c 6162              <lab
+00003210: 656c 2066 6f72 3d22 666f 726d 2d77 6964  el for="form-wid
+00003220: 6765 7473 2d73 7562 6f62 6a65 6374 2d77  gets-subobject-w
+00003230: 6964 6765 7473 2d66 6f6f 6669 656c 6422  idgets-foofield"
+00003240: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003260: 3c73 7061 6e3e 4d79 2066 6f6f 2066 6965  <span>My foo fie
+00003270: 6c64 3c2f 7370 616e 3e0a 2020 2020 2020  ld</span>.      
 00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003290: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
-000032a0: 2272 6571 7569 7265 6422 3e2a 3c2f 7370  "required">*</sp
-000032b0: 616e 3e0a 2020 2020 2020 2020 2020 2020  an>.            
-000032c0: 2020 2020 2020 2020 2020 3c2f 6c61 6265            </labe
-000032d0: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
-000032e0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-000032f0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00003300: 3d22 7769 6467 6574 223e 0a20 2020 2020  ="widget">.     
+00003290: 2020 2020 2020 2020 3c73 7061 6e20 636c          <span cl
+000032a0: 6173 733d 2272 6571 7569 7265 6422 3e2a  ass="required">*
+000032b0: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
+000032c0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000032d0: 6c61 6265 6c3e 0a20 2020 2020 2020 2020  label>.         
+000032e0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+000032f0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00003300: 6c61 7373 3d22 7769 6467 6574 223e 0a20  lass="widget">. 
 00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003320: 203c 696e 7075 7420 7479 7065 3d22 7465   <input type="te
-00003330: 7874 220a 2020 2020 2020 2020 2069 643d  xt".         id=
-00003340: 2266 6f72 6d2d 7769 6467 6574 732d 7375  "form-widgets-su
-00003350: 626f 626a 6563 742d 7769 6467 6574 732d  bobject-widgets-
-00003360: 666f 6f66 6965 6c64 220a 2020 2020 2020  foofield".      
-00003370: 2020 206e 616d 653d 2266 6f72 6d2e 7769     name="form.wi
-00003380: 6467 6574 732e 7375 626f 626a 6563 742e  dgets.subobject.
-00003390: 7769 6467 6574 732e 666f 6f66 6965 6c64  widgets.foofield
-000033a0: 220a 2020 2020 2020 2020 2063 6c61 7373  ".         class
-000033b0: 3d22 7465 7874 2d77 6964 6765 7420 7265  ="text-widget re
-000033c0: 7175 6972 6564 2069 6e74 2d66 6965 6c64  quired int-field
-000033d0: 220a 2020 2020 2020 2020 2076 616c 7565  ".         value
-000033e0: 3d22 312c 3131 3122 202f 3e0a 2020 2020  ="1,111" />.    
-000033f0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00003400: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00003410: 6469 7620 636c 6173 733d 226c 6162 656c  div class="label
-00003420: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00003430: 2020 2020 2020 2020 203c 6c61 6265 6c20           <label 
-00003440: 666f 723d 2266 6f72 6d2d 7769 6467 6574  for="form-widget
-00003450: 732d 7375 626f 626a 6563 742d 7769 6467  s-subobject-widg
-00003460: 6574 732d 6261 7266 6965 6c64 223e 0a20  ets-barfield">. 
-00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003480: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
-00003490: 616e 3e4d 7920 6465 6172 2062 6172 3c2f  an>My dear bar</
-000034a0: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
-000034b0: 2020 2020 2020 2020 2020 2020 3c2f 6c61              </la
-000034c0: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
-000034d0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-000034e0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000034f0: 7373 3d22 7769 6467 6574 223e 0a20 2020  ss="widget">.   
-00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003510: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
-00003520: 7465 7874 220a 2020 2020 2020 2020 2069  text".         i
-00003530: 643d 2266 6f72 6d2d 7769 6467 6574 732d  d="form-widgets-
-00003540: 7375 626f 626a 6563 742d 7769 6467 6574  subobject-widget
-00003550: 732d 6261 7266 6965 6c64 220a 2020 2020  s-barfield".    
-00003560: 2020 2020 206e 616d 653d 2266 6f72 6d2e       name="form.
-00003570: 7769 6467 6574 732e 7375 626f 626a 6563  widgets.subobjec
-00003580: 742e 7769 6467 6574 732e 6261 7266 6965  t.widgets.barfie
-00003590: 6c64 220a 2020 2020 2020 2020 2063 6c61  ld".         cla
-000035a0: 7373 3d22 7465 7874 2d77 6964 6765 7420  ss="text-widget 
-000035b0: 696e 742d 6669 656c 6422 0a20 2020 2020  int-field".     
-000035c0: 2020 2020 7661 6c75 653d 2232 2c32 3232      value="2,222
-000035d0: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
-000035e0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-000035f0: 3c69 6e70 7574 206e 616d 653d 2266 6f72  <input name="for
-00003600: 6d2e 7769 6467 6574 732e 7375 626f 626a  m.widgets.subobj
-00003610: 6563 742d 656d 7074 792d 6d61 726b 6572  ect-empty-marker
-00003620: 2220 7479 7065 3d22 6869 6464 656e 2220  " type="hidden" 
-00003630: 7661 6c75 653d 2231 222f 3e0a 2020 3c2f  value="1"/>.  </
-00003640: 6469 763e 0a20 2020 203c 2f64 6976 3e0a  div>.    </div>.
-00003650: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00003660: 726f 7722 3e0a 2020 2020 2020 3c6c 6162  row">.      <lab
-00003670: 656c 2066 6f72 3d22 666f 726d 2d77 6964  el for="form-wid
-00003680: 6765 7473 2d6e 616d 6522 3e6e 616d 653c  gets-name">name<
-00003690: 2f6c 6162 656c 3e0a 2020 2020 2020 3c69  /label>.      <i
-000036a0: 6e70 7574 2074 7970 653d 2274 6578 7422  nput type="text"
-000036b0: 0a20 2020 2020 2020 2020 6964 3d22 666f  .         id="fo
-000036c0: 726d 2d77 6964 6765 7473 2d6e 616d 6522  rm-widgets-name"
-000036d0: 0a20 2020 2020 2020 2020 6e61 6d65 3d22  .         name="
-000036e0: 666f 726d 2e77 6964 6765 7473 2e6e 616d  form.widgets.nam
-000036f0: 6522 0a20 2020 2020 2020 2020 636c 6173  e".         clas
-00003700: 733d 2274 6578 742d 7769 6467 6574 2072  s="text-widget r
-00003710: 6571 7569 7265 6420 7465 7874 6c69 6e65  equired textline
-00003720: 2d66 6965 6c64 220a 2020 2020 2020 2020  -field".        
-00003730: 2076 616c 7565 3d22 2220 2f3e 0a20 2020   value="" />.   
-00003740: 203c 2f64 6976 3e0a 2020 2020 3c64 6976   </div>.    <div
-00003750: 2063 6c61 7373 3d22 6163 7469 6f6e 223e   class="action">
-00003760: 0a20 2020 2020 203c 696e 7075 7420 7479  .      <input ty
-00003770: 7065 3d22 7375 626d 6974 220a 2020 2020  pe="submit".    
-00003780: 2020 2020 2069 643d 2266 6f72 6d2d 6275       id="form-bu
-00003790: 7474 6f6e 732d 6164 6422 0a20 2020 2020  ttons-add".     
-000037a0: 2020 2020 6e61 6d65 3d22 666f 726d 2e62      name="form.b
-000037b0: 7574 746f 6e73 2e61 6464 220a 2020 2020  uttons.add".    
-000037c0: 2020 2020 2063 6c61 7373 3d22 7375 626d       class="subm
-000037d0: 6974 2d77 6964 6765 7420 6275 7474 6f6e  it-widget button
-000037e0: 2d66 6965 6c64 220a 2020 2020 2020 2020  -field".        
-000037f0: 2076 616c 7565 3d22 4164 6422 202f 3e0a   value="Add" />.
-00003800: 2020 2020 3c2f 6469 763e 0a20 203c 2f66      </div>.  </f
-00003810: 6f72 6d3e 0a0a 0a57 6520 646f 6e27 7420  orm>...We don't 
-00003820: 6861 7665 2074 6865 206f 626a 6563 7420  have the object 
-00003830: 2879 6574 2920 696e 2074 6865 2072 6f6f  (yet) in the roo
-00003840: 743a 0a0a 2020 3e3e 3e20 726f 6f74 5b27  t:..  >>> root['
-00003850: 6669 7273 7427 5d0a 2020 5472 6163 6562  first'].  Traceb
-00003860: 6163 6b20 286d 6f73 7420 7265 6365 6e74  ack (most recent
-00003870: 2063 616c 6c20 6c61 7374 293a 0a20 202e   call last):.  .
-00003880: 2e2e 0a20 204b 6579 4572 726f 723a 2027  ...  KeyError: '
-00003890: 6669 7273 7427 0a0a 4c65 7427 7320 7472  first'..Let's tr
-000038a0: 7920 746f 2061 6464 2061 6e20 6f62 6a65  y to add an obje
-000038b0: 6374 3a0a 0a20 203e 3e3e 2072 6571 7565  ct:..  >>> reque
-000038c0: 7374 203d 2054 6573 7452 6571 7565 7374  st = TestRequest
-000038d0: 2870 6172 616d 733d 7b0a 2020 2e2e 2e20  (params={.  ... 
-000038e0: 2020 2020 2766 6f72 6d2e 7769 6467 6574      'form.widget
-000038f0: 732e 7375 626f 626a 6563 742e 7769 6467  s.subobject.widg
-00003900: 6574 732e 666f 6f66 6965 6c64 273a 2736  ets.foofield':'6
-00003910: 3627 2c0a 2020 2e2e 2e20 2020 2020 2766  6',.  ...     'f
-00003920: 6f72 6d2e 7769 6467 6574 732e 7375 626f  orm.widgets.subo
-00003930: 626a 6563 742e 7769 6467 6574 732e 6261  bject.widgets.ba
-00003940: 7266 6965 6c64 273a 2739 3927 2c0a 2020  rfield':'99',.  
-00003950: 2e2e 2e20 2020 2020 2766 6f72 6d2e 7769  ...     'form.wi
-00003960: 6467 6574 732e 6e61 6d65 273a 2766 6972  dgets.name':'fir
-00003970: 7374 272c 0a20 202e 2e2e 2020 2020 2027  st',.  ...     '
-00003980: 666f 726d 2e77 6964 6765 7473 2e73 7562  form.widgets.sub
-00003990: 6f62 6a65 6374 2d65 6d70 7479 2d6d 6172  object-empty-mar
-000039a0: 6b65 7227 3a27 3127 2c0a 2020 2e2e 2e20  ker':'1',.  ... 
-000039b0: 2020 2020 2766 6f72 6d2e 6275 7474 6f6e      'form.button
-000039c0: 732e 6164 6427 3a27 4164 6427 7d29 0a20  s.add':'Add'}). 
-000039d0: 203e 3e3e 206d 7961 6464 666f 726d 2e72   >>> myaddform.r
-000039e0: 6571 7565 7374 203d 2072 6571 7565 7374  equest = request
-000039f0: 0a0a 2020 3e3e 3e20 6d79 6164 6466 6f72  ..  >>> myaddfor
-00003a00: 6d2e 7570 6461 7465 2829 0a20 204d 7941  m.update().  MyA
-00003a10: 6464 466f 726d 2e63 7265 6174 650a 2020  ddForm.create.  
-00003a20: 7b27 6e61 6d65 273a 2027 6669 7273 7427  {'name': 'first'
-00003a30: 2c0a 2020 2027 7375 626f 626a 6563 7427  ,.   'subobject'
-00003a40: 3a20 3c70 7961 6d73 5f66 6f72 6d2e 7465  : <pyams_form.te
-00003a50: 7374 696e 672e 4d79 5375 624f 626a 6563  sting.MySubObjec
-00003a60: 7420 6f62 6a65 6374 2061 7420 2e2e 2e3e  t object at ...>
-00003a70: 7d0a 0a57 6f77 2c20 6974 2067 6f74 2061  }..Wow, it got a
-00003a80: 6464 6564 3a0a 0a20 203e 3e3e 2072 6f6f  dded:..  >>> roo
-00003a90: 745b 2766 6972 7374 275d 0a20 203c 7079  t['first'].  <py
-00003aa0: 616d 735f 666f 726d 2e74 6573 7469 6e67  ams_form.testing
-00003ab0: 2e4d 794f 626a 6563 7420 6f62 6a65 6374  .MyObject object
-00003ac0: 2061 7420 2e2e 2e3e 0a0a 2020 3e3e 3e20   at ...>..  >>> 
-00003ad0: 726f 6f74 5b27 6669 7273 7427 5d2e 7375  root['first'].su
-00003ae0: 626f 626a 6563 740a 2020 3c70 7961 6d73  bobject.  <pyams
-00003af0: 5f66 6f72 6d2e 7465 7374 696e 672e 4d79  _form.testing.My
-00003b00: 5375 624f 626a 6563 7420 6f62 6a65 6374  SubObject object
-00003b10: 2061 7420 2e2e 2e3e 0a0a 4669 656c 6420   at ...>..Field 
-00003b20: 7661 6c75 6573 206e 6565 6420 746f 2062  values need to b
-00003b30: 6520 7269 6768 743a 0a0a 2020 3e3e 3e20  e right:..  >>> 
-00003b40: 726f 6f74 5b27 6669 7273 7427 5d2e 7375  root['first'].su
-00003b50: 626f 626a 6563 742e 666f 6f66 6965 6c64  bobject.foofield
-00003b60: 0a20 2036 360a 2020 3e3e 3e20 726f 6f74  .  66.  >>> root
-00003b70: 5b27 6669 7273 7427 5d2e 7375 626f 626a  ['first'].subobj
-00003b80: 6563 742e 6261 7266 6965 6c64 0a20 2039  ect.barfield.  9
-00003b90: 390a 0a4c 6574 2773 2073 6565 206f 7572  9..Let's see our
-00003ba0: 2065 7665 6e74 206c 6f67 3a0a 0a20 203e   event log:..  >
-00003bb0: 3e3e 206c 656e 2865 7665 6e74 6c6f 6729  >> len(eventlog)
-00003bc0: 0a20 2033 0a0a 2020 3e3e 3e20 7072 696e  .  3..  >>> prin
-00003bd0: 7445 7665 6e74 7328 290a 2020 3c7a 6f70  tEvents().  <zop
-00003be0: 652e 2e2e 4f62 6a65 6374 4372 6561 7465  e...ObjectCreate
-00003bf0: 6445 7665 6e74 206f 626a 6563 7420 6174  dEvent object at
-00003c00: 202e 2e2e 3e0a 2020 3c7a 6f70 652e 2e2e   ...>.  <zope...
-00003c10: 4f62 6a65 6374 4d6f 6469 6669 6564 4576  ObjectModifiedEv
-00003c20: 656e 7420 6f62 6a65 6374 2061 7420 2e2e  ent object at ..
-00003c30: 2e3e 0a20 2070 7961 6d73 5f66 6f72 6d2e  .>.  pyams_form.
-00003c40: 7465 7374 696e 672e 494d 7953 7562 4f62  testing.IMySubOb
-00003c50: 6a65 6374 0a20 205b 2762 6172 6669 656c  ject.  ['barfiel
-00003c60: 6427 2c20 2766 6f6f 6669 656c 6427 5d0a  d', 'foofield'].
-00003c70: 2020 3c7a 6f70 652e 2e2e 4f62 6a65 6374    <zope...Object
-00003c80: 4372 6561 7465 6445 7665 6e74 206f 626a  CreatedEvent obj
-00003c90: 6563 7420 6174 202e 2e2e 3e0a 0a23 2046  ect at ...>..# F
-00003ca0: 4958 4d45 3a20 6c6f 6f6b 2066 6f72 206d  IXME: look for m
-00003cb0: 6973 7369 6e67 2065 7874 7261 2043 6f6e  issing extra Con
-00003cc0: 7461 696e 6572 4d6f 6469 6669 6564 4576  tainerModifiedEv
-00003cd0: 656e 7420 2121 210a 0a20 203e 3e3e 2065  ent !!!..  >>> e
-00003ce0: 7665 6e74 6c6f 6720 3d20 5b5d 0a0a 4c65  ventlog = []..Le
-00003cf0: 7427 7320 7472 7920 746f 2065 6469 7420  t's try to edit 
-00003d00: 7468 6174 206e 6577 6c79 2061 6464 6564  that newly added
-00003d10: 206f 626a 6563 743a 0a0a 2020 3e3e 3e20   object:..  >>> 
-00003d20: 636c 6173 7320 4d79 4564 6974 466f 726d  class MyEditForm
-00003d30: 2866 6f72 6d2e 4564 6974 466f 726d 293a  (form.EditForm):
-00003d40: 0a20 202e 2e2e 2020 2020 2066 6965 6c64  .  ...     field
-00003d50: 7320 3d20 6669 656c 642e 4669 656c 6473  s = field.Fields
-00003d60: 2849 4d79 4f62 6a65 6374 290a 0a20 203e  (IMyObject)..  >
-00003d70: 3e3e 2065 6469 7466 6f72 6d20 3d20 4d79  >> editform = My
-00003d80: 4564 6974 466f 726d 2872 6f6f 745b 2766  EditForm(root['f
-00003d90: 6972 7374 275d 2c20 5465 7374 5265 7175  irst'], TestRequ
-00003da0: 6573 7428 2929 0a20 203e 3e3e 2061 6464  est()).  >>> add
-00003db0: 5465 6d70 6c61 7465 2865 6469 7466 6f72  Template(editfor
-00003dc0: 6d29 0a20 203e 3e3e 2065 6469 7466 6f72  m).  >>> editfor
-00003dd0: 6d2e 7570 6461 7465 2829 0a0a 5761 7463  m.update()..Watc
-00003de0: 6820 666f 7220 7468 6520 7769 6467 6574  h for the widget
-00003df0: 2076 616c 7565 7320 696e 2074 6865 2048   values in the H
-00003e00: 544d 4c3a 0a0a 2020 3e3e 3e20 7072 696e  TML:..  >>> prin
-00003e10: 7428 666f 726d 6174 5f68 746d 6c28 6564  t(format_html(ed
-00003e20: 6974 666f 726d 2e72 656e 6465 7228 2929  itform.render())
-00003e30: 290a 2020 3c66 6f72 6d20 6163 7469 6f6e  ).  <form action
-00003e40: 3d22 2e22 3e0a 2020 2020 3c64 6976 2063  =".">.    <div c
-00003e50: 6c61 7373 3d22 726f 7722 3e0a 2020 2020  lass="row">.    
-00003e60: 2020 3c6c 6162 656c 2066 6f72 3d22 666f    <label for="fo
-00003e70: 726d 2d77 6964 6765 7473 2d73 7562 6f62  rm-widgets-subob
-00003e80: 6a65 6374 223e 6d79 206f 626a 6563 743c  ject">my object<
-00003e90: 2f6c 6162 656c 3e0a 2020 2020 2020 3c64  /label>.      <d
-00003ea0: 6976 2063 6c61 7373 3d22 6f62 6a65 6374  iv class="object
-00003eb0: 2d77 6964 6765 7420 7265 7175 6972 6564  -widget required
-00003ec0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00003ed0: 203c 6469 7620 636c 6173 733d 226c 6162   <div class="lab
-00003ee0: 656c 223e 0a20 2020 2020 2020 2020 2020  el">.           
-00003ef0: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
-00003f00: 6c20 666f 723d 2266 6f72 6d2d 7769 6467  l for="form-widg
-00003f10: 6574 732d 7375 626f 626a 6563 742d 7769  ets-subobject-wi
-00003f20: 6467 6574 732d 666f 6f66 6965 6c64 223e  dgets-foofield">
-00003f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003f40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00003f50: 7370 616e 3e4d 7920 666f 6f20 6669 656c  span>My foo fiel
-00003f60: 643c 2f73 7061 6e3e 0a20 2020 2020 2020  d</span>.       
+00003320: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
+00003330: 3d22 7465 7874 220a 2020 2020 2020 2020  ="text".        
+00003340: 2069 643d 2266 6f72 6d2d 7769 6467 6574   id="form-widget
+00003350: 732d 7375 626f 626a 6563 742d 7769 6467  s-subobject-widg
+00003360: 6574 732d 666f 6f66 6965 6c64 220a 2020  ets-foofield".  
+00003370: 2020 2020 2020 206e 616d 653d 2266 6f72         name="for
+00003380: 6d2e 7769 6467 6574 732e 7375 626f 626a  m.widgets.subobj
+00003390: 6563 742e 7769 6467 6574 732e 666f 6f66  ect.widgets.foof
+000033a0: 6965 6c64 220a 2020 2020 2020 2020 2063  ield".         c
+000033b0: 6c61 7373 3d22 7465 7874 2d77 6964 6765  lass="text-widge
+000033c0: 7420 7265 7175 6972 6564 2069 6e74 2d66  t required int-f
+000033d0: 6965 6c64 220a 2020 2020 2020 2020 2076  ield".         v
+000033e0: 616c 7565 3d22 312c 3131 3122 202f 3e0a  alue="1,111" />.
+000033f0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00003400: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00003410: 2020 203c 6469 7620 636c 6173 733d 226c     <div class="l
+00003420: 6162 656c 223e 0a20 2020 2020 2020 2020  abel">.         
+00003430: 2020 2020 2020 2020 2020 2020 203c 6c61               <la
+00003440: 6265 6c20 666f 723d 2266 6f72 6d2d 7769  bel for="form-wi
+00003450: 6467 6574 732d 7375 626f 626a 6563 742d  dgets-subobject-
+00003460: 7769 6467 6574 732d 6261 7266 6965 6c64  widgets-barfield
+00003470: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003490: 203c 7370 616e 3e4d 7920 6465 6172 2062   <span>My dear b
+000034a0: 6172 3c2f 7370 616e 3e0a 2020 2020 2020  ar</span>.      
+000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034c0: 3c2f 6c61 6265 6c3e 0a20 2020 2020 2020  </label>.       
+000034d0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000034e0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000034f0: 2063 6c61 7373 3d22 7769 6467 6574 223e   class="widget">
+00003500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003510: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
+00003520: 7065 3d22 7465 7874 220a 2020 2020 2020  pe="text".      
+00003530: 2020 2069 643d 2266 6f72 6d2d 7769 6467     id="form-widg
+00003540: 6574 732d 7375 626f 626a 6563 742d 7769  ets-subobject-wi
+00003550: 6467 6574 732d 6261 7266 6965 6c64 220a  dgets-barfield".
+00003560: 2020 2020 2020 2020 206e 616d 653d 2266           name="f
+00003570: 6f72 6d2e 7769 6467 6574 732e 7375 626f  orm.widgets.subo
+00003580: 626a 6563 742e 7769 6467 6574 732e 6261  bject.widgets.ba
+00003590: 7266 6965 6c64 220a 2020 2020 2020 2020  rfield".        
+000035a0: 2063 6c61 7373 3d22 7465 7874 2d77 6964   class="text-wid
+000035b0: 6765 7420 696e 742d 6669 656c 6422 0a20  get int-field". 
+000035c0: 2020 2020 2020 2020 7661 6c75 653d 2232          value="2
+000035d0: 2c32 3232 2220 2f3e 0a20 2020 2020 2020  ,222" />.       
+000035e0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000035f0: 2020 2020 3c69 6e70 7574 206e 616d 653d      <input name=
+00003600: 2266 6f72 6d2e 7769 6467 6574 732e 7375  "form.widgets.su
+00003610: 626f 626a 6563 742d 656d 7074 792d 6d61  bobject-empty-ma
+00003620: 726b 6572 2220 7479 7065 3d22 6869 6464  rker" type="hidd
+00003630: 656e 2220 7661 6c75 653d 2231 2220 2f3e  en" value="1" />
+00003640: 0a20 203c 2f64 6976 3e0a 2020 2020 3c2f  .  </div>.    </
+00003650: 6469 763e 0a20 2020 203c 6469 7620 636c  div>.    <div cl
+00003660: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
+00003670: 203c 6c61 6265 6c20 666f 723d 2266 6f72   <label for="for
+00003680: 6d2d 7769 6467 6574 732d 6e61 6d65 223e  m-widgets-name">
+00003690: 6e61 6d65 3c2f 6c61 6265 6c3e 0a20 2020  name</label>.   
+000036a0: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
+000036b0: 7465 7874 220a 2020 2020 2020 2020 2069  text".         i
+000036c0: 643d 2266 6f72 6d2d 7769 6467 6574 732d  d="form-widgets-
+000036d0: 6e61 6d65 220a 2020 2020 2020 2020 206e  name".         n
+000036e0: 616d 653d 2266 6f72 6d2e 7769 6467 6574  ame="form.widget
+000036f0: 732e 6e61 6d65 220a 2020 2020 2020 2020  s.name".        
+00003700: 2063 6c61 7373 3d22 7465 7874 2d77 6964   class="text-wid
+00003710: 6765 7420 7265 7175 6972 6564 2074 6578  get required tex
+00003720: 746c 696e 652d 6669 656c 6422 0a20 2020  tline-field".   
+00003730: 2020 2020 2020 7661 6c75 653d 2222 202f        value="" /
+00003740: 3e0a 2020 2020 3c2f 6469 763e 0a20 2020  >.    </div>.   
+00003750: 203c 6469 7620 636c 6173 733d 2261 6374   <div class="act
+00003760: 696f 6e22 3e0a 2020 2020 2020 3c69 6e70  ion">.      <inp
+00003770: 7574 2074 7970 653d 2273 7562 6d69 7422  ut type="submit"
+00003780: 0a20 2020 2020 2020 2020 6964 3d22 666f  .         id="fo
+00003790: 726d 2d62 7574 746f 6e73 2d61 6464 220a  rm-buttons-add".
+000037a0: 2020 2020 2020 2020 206e 616d 653d 2266           name="f
+000037b0: 6f72 6d2e 6275 7474 6f6e 732e 6164 6422  orm.buttons.add"
+000037c0: 0a20 2020 2020 2020 2020 636c 6173 733d  .         class=
+000037d0: 2273 7562 6d69 742d 7769 6467 6574 2062  "submit-widget b
+000037e0: 7574 746f 6e2d 6669 656c 6422 0a20 2020  utton-field".   
+000037f0: 2020 2020 2020 7661 6c75 653d 2241 6464        value="Add
+00003800: 2220 2f3e 0a20 2020 203c 2f64 6976 3e0a  " />.    </div>.
+00003810: 2020 3c2f 666f 726d 3e0a 0a0a 5765 2064    </form>...We d
+00003820: 6f6e 2774 2068 6176 6520 7468 6520 6f62  on't have the ob
+00003830: 6a65 6374 2028 7965 7429 2069 6e20 7468  ject (yet) in th
+00003840: 6520 726f 6f74 3a0a 0a20 203e 3e3e 2072  e root:..  >>> r
+00003850: 6f6f 745b 2766 6972 7374 275d 0a20 2054  oot['first'].  T
+00003860: 7261 6365 6261 636b 2028 6d6f 7374 2072  raceback (most r
+00003870: 6563 656e 7420 6361 6c6c 206c 6173 7429  ecent call last)
+00003880: 3a0a 2020 2e2e 2e0a 2020 4b65 7945 7272  :.  ....  KeyErr
+00003890: 6f72 3a20 2766 6972 7374 270a 0a4c 6574  or: 'first'..Let
+000038a0: 2773 2074 7279 2074 6f20 6164 6420 616e  's try to add an
+000038b0: 206f 626a 6563 743a 0a0a 2020 3e3e 3e20   object:..  >>> 
+000038c0: 7265 7175 6573 7420 3d20 5465 7374 5265  request = TestRe
+000038d0: 7175 6573 7428 7061 7261 6d73 3d7b 0a20  quest(params={. 
+000038e0: 202e 2e2e 2020 2020 2027 666f 726d 2e77   ...     'form.w
+000038f0: 6964 6765 7473 2e73 7562 6f62 6a65 6374  idgets.subobject
+00003900: 2e77 6964 6765 7473 2e66 6f6f 6669 656c  .widgets.foofiel
+00003910: 6427 3a27 3636 272c 0a20 202e 2e2e 2020  d':'66',.  ...  
+00003920: 2020 2027 666f 726d 2e77 6964 6765 7473     'form.widgets
+00003930: 2e73 7562 6f62 6a65 6374 2e77 6964 6765  .subobject.widge
+00003940: 7473 2e62 6172 6669 656c 6427 3a27 3939  ts.barfield':'99
+00003950: 272c 0a20 202e 2e2e 2020 2020 2027 666f  ',.  ...     'fo
+00003960: 726d 2e77 6964 6765 7473 2e6e 616d 6527  rm.widgets.name'
+00003970: 3a27 6669 7273 7427 2c0a 2020 2e2e 2e20  :'first',.  ... 
+00003980: 2020 2020 2766 6f72 6d2e 7769 6467 6574      'form.widget
+00003990: 732e 7375 626f 626a 6563 742d 656d 7074  s.subobject-empt
+000039a0: 792d 6d61 726b 6572 273a 2731 272c 0a20  y-marker':'1',. 
+000039b0: 202e 2e2e 2020 2020 2027 666f 726d 2e62   ...     'form.b
+000039c0: 7574 746f 6e73 2e61 6464 273a 2741 6464  uttons.add':'Add
+000039d0: 277d 290a 2020 3e3e 3e20 6d79 6164 6466  '}).  >>> myaddf
+000039e0: 6f72 6d2e 7265 7175 6573 7420 3d20 7265  orm.request = re
+000039f0: 7175 6573 740a 0a20 203e 3e3e 206d 7961  quest..  >>> mya
+00003a00: 6464 666f 726d 2e75 7064 6174 6528 290a  ddform.update().
+00003a10: 2020 4d79 4164 6446 6f72 6d2e 6372 6561    MyAddForm.crea
+00003a20: 7465 0a20 207b 276e 616d 6527 3a20 2766  te.  {'name': 'f
+00003a30: 6972 7374 272c 0a20 2020 2773 7562 6f62  irst',.   'subob
+00003a40: 6a65 6374 273a 203c 7079 616d 735f 666f  ject': <pyams_fo
+00003a50: 726d 2e74 6573 7469 6e67 2e4d 7953 7562  rm.testing.MySub
+00003a60: 4f62 6a65 6374 206f 626a 6563 7420 6174  Object object at
+00003a70: 202e 2e2e 3e7d 0a0a 576f 772c 2069 7420   ...>}..Wow, it 
+00003a80: 676f 7420 6164 6465 643a 0a0a 2020 3e3e  got added:..  >>
+00003a90: 3e20 726f 6f74 5b27 6669 7273 7427 5d0a  > root['first'].
+00003aa0: 2020 3c70 7961 6d73 5f66 6f72 6d2e 7465    <pyams_form.te
+00003ab0: 7374 696e 672e 4d79 4f62 6a65 6374 206f  sting.MyObject o
+00003ac0: 626a 6563 7420 6174 202e 2e2e 3e0a 0a20  bject at ...>.. 
+00003ad0: 203e 3e3e 2072 6f6f 745b 2766 6972 7374   >>> root['first
+00003ae0: 275d 2e73 7562 6f62 6a65 6374 0a20 203c  '].subobject.  <
+00003af0: 7079 616d 735f 666f 726d 2e74 6573 7469  pyams_form.testi
+00003b00: 6e67 2e4d 7953 7562 4f62 6a65 6374 206f  ng.MySubObject o
+00003b10: 626a 6563 7420 6174 202e 2e2e 3e0a 0a46  bject at ...>..F
+00003b20: 6965 6c64 2076 616c 7565 7320 6e65 6564  ield values need
+00003b30: 2074 6f20 6265 2072 6967 6874 3a0a 0a20   to be right:.. 
+00003b40: 203e 3e3e 2072 6f6f 745b 2766 6972 7374   >>> root['first
+00003b50: 275d 2e73 7562 6f62 6a65 6374 2e66 6f6f  '].subobject.foo
+00003b60: 6669 656c 640a 2020 3636 0a20 203e 3e3e  field.  66.  >>>
+00003b70: 2072 6f6f 745b 2766 6972 7374 275d 2e73   root['first'].s
+00003b80: 7562 6f62 6a65 6374 2e62 6172 6669 656c  ubobject.barfiel
+00003b90: 640a 2020 3939 0a0a 4c65 7427 7320 7365  d.  99..Let's se
+00003ba0: 6520 6f75 7220 6576 656e 7420 6c6f 673a  e our event log:
+00003bb0: 0a0a 2020 3e3e 3e20 6c65 6e28 6576 656e  ..  >>> len(even
+00003bc0: 746c 6f67 290a 2020 330a 0a20 203e 3e3e  tlog).  3..  >>>
+00003bd0: 2070 7269 6e74 4576 656e 7473 2829 0a20   printEvents(). 
+00003be0: 203c 7a6f 7065 2e2e 2e4f 626a 6563 7443   <zope...ObjectC
+00003bf0: 7265 6174 6564 4576 656e 7420 6f62 6a65  reatedEvent obje
+00003c00: 6374 2061 7420 2e2e 2e3e 0a20 203c 7a6f  ct at ...>.  <zo
+00003c10: 7065 2e2e 2e4f 626a 6563 744d 6f64 6966  pe...ObjectModif
+00003c20: 6965 6445 7665 6e74 206f 626a 6563 7420  iedEvent object 
+00003c30: 6174 202e 2e2e 3e0a 2020 7079 616d 735f  at ...>.  pyams_
+00003c40: 666f 726d 2e74 6573 7469 6e67 2e49 4d79  form.testing.IMy
+00003c50: 5375 624f 626a 6563 740a 2020 5b27 6261  SubObject.  ['ba
+00003c60: 7266 6965 6c64 272c 2027 666f 6f66 6965  rfield', 'foofie
+00003c70: 6c64 275d 0a20 203c 7a6f 7065 2e2e 2e4f  ld'].  <zope...O
+00003c80: 626a 6563 7443 7265 6174 6564 4576 656e  bjectCreatedEven
+00003c90: 7420 6f62 6a65 6374 2061 7420 2e2e 2e3e  t object at ...>
+00003ca0: 0a0a 2320 4649 584d 453a 206c 6f6f 6b20  ..# FIXME: look 
+00003cb0: 666f 7220 6d69 7373 696e 6720 6578 7472  for missing extr
+00003cc0: 6120 436f 6e74 6169 6e65 724d 6f64 6966  a ContainerModif
+00003cd0: 6965 6445 7665 6e74 2021 2121 0a0a 2020  iedEvent !!!..  
+00003ce0: 3e3e 3e20 6576 656e 746c 6f67 203d 205b  >>> eventlog = [
+00003cf0: 5d0a 0a4c 6574 2773 2074 7279 2074 6f20  ]..Let's try to 
+00003d00: 6564 6974 2074 6861 7420 6e65 776c 7920  edit that newly 
+00003d10: 6164 6465 6420 6f62 6a65 6374 3a0a 0a20  added object:.. 
+00003d20: 203e 3e3e 2063 6c61 7373 204d 7945 6469   >>> class MyEdi
+00003d30: 7446 6f72 6d28 666f 726d 2e45 6469 7446  tForm(form.EditF
+00003d40: 6f72 6d29 3a0a 2020 2e2e 2e20 2020 2020  orm):.  ...     
+00003d50: 6669 656c 6473 203d 2066 6965 6c64 2e46  fields = field.F
+00003d60: 6965 6c64 7328 494d 794f 626a 6563 7429  ields(IMyObject)
+00003d70: 0a0a 2020 3e3e 3e20 6564 6974 666f 726d  ..  >>> editform
+00003d80: 203d 204d 7945 6469 7446 6f72 6d28 726f   = MyEditForm(ro
+00003d90: 6f74 5b27 6669 7273 7427 5d2c 2054 6573  ot['first'], Tes
+00003da0: 7452 6571 7565 7374 2829 290a 2020 3e3e  tRequest()).  >>
+00003db0: 3e20 6164 6454 656d 706c 6174 6528 6564  > addTemplate(ed
+00003dc0: 6974 666f 726d 290a 2020 3e3e 3e20 6564  itform).  >>> ed
+00003dd0: 6974 666f 726d 2e75 7064 6174 6528 290a  itform.update().
+00003de0: 0a57 6174 6368 2066 6f72 2074 6865 2077  .Watch for the w
+00003df0: 6964 6765 7420 7661 6c75 6573 2069 6e20  idget values in 
+00003e00: 7468 6520 4854 4d4c 3a0a 0a20 203e 3e3e  the HTML:..  >>>
+00003e10: 2070 7269 6e74 2866 6f72 6d61 745f 6874   print(format_ht
+00003e20: 6d6c 2865 6469 7466 6f72 6d2e 7265 6e64  ml(editform.rend
+00003e30: 6572 2829 2929 0a20 203c 666f 726d 2061  er())).  <form a
+00003e40: 6374 696f 6e3d 222e 223e 0a20 2020 203c  ction=".">.    <
+00003e50: 6469 7620 636c 6173 733d 2272 6f77 223e  div class="row">
+00003e60: 0a20 2020 2020 203c 6c61 6265 6c20 666f  .      <label fo
+00003e70: 723d 2266 6f72 6d2d 7769 6467 6574 732d  r="form-widgets-
+00003e80: 7375 626f 626a 6563 7422 3e6d 7920 6f62  subobject">my ob
+00003e90: 6a65 6374 3c2f 6c61 6265 6c3e 0a20 2020  ject</label>.   
+00003ea0: 2020 203c 6469 7620 636c 6173 733d 226f     <div class="o
+00003eb0: 626a 6563 742d 7769 6467 6574 2072 6571  bject-widget req
+00003ec0: 7569 7265 6422 3e0a 2020 2020 2020 2020  uired">.        
+00003ed0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00003ee0: 3d22 6c61 6265 6c22 3e0a 2020 2020 2020  ="label">.      
+00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f00: 3c6c 6162 656c 2066 6f72 3d22 666f 726d  <label for="form
+00003f10: 2d77 6964 6765 7473 2d73 7562 6f62 6a65  -widgets-subobje
+00003f20: 6374 2d77 6964 6765 7473 2d66 6f6f 6669  ct-widgets-foofi
+00003f30: 656c 6422 3e0a 2020 2020 2020 2020 2020  eld">.          
+00003f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f50: 2020 2020 3c73 7061 6e3e 4d79 2066 6f6f      <span>My foo
+00003f60: 2066 6965 6c64 3c2f 7370 616e 3e0a 2020   field</span>.  
 00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f80: 2020 2020 2020 203c 7370 616e 2063 6c61         <span cla
-00003f90: 7373 3d22 7265 7175 6972 6564 223e 2a3c  ss="required">*<
-00003fa0: 2f73 7061 6e3e 0a20 2020 2020 2020 2020  /span>.         
-00003fb0: 2020 2020 2020 2020 2020 2020 203c 2f6c               </l
-00003fc0: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
-00003fd0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00003fe0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00003ff0: 6173 733d 2277 6964 6765 7422 3e0a 2020  ass="widget">.  
-00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004010: 2020 2020 3c69 6e70 7574 2074 7970 653d      <input type=
-00004020: 2274 6578 7422 0a20 2020 2020 2020 2020  "text".         
-00004030: 6964 3d22 666f 726d 2d77 6964 6765 7473  id="form-widgets
-00004040: 2d73 7562 6f62 6a65 6374 2d77 6964 6765  -subobject-widge
-00004050: 7473 2d66 6f6f 6669 656c 6422 0a20 2020  ts-foofield".   
-00004060: 2020 2020 2020 6e61 6d65 3d22 666f 726d        name="form
-00004070: 2e77 6964 6765 7473 2e73 7562 6f62 6a65  .widgets.subobje
-00004080: 6374 2e77 6964 6765 7473 2e66 6f6f 6669  ct.widgets.foofi
-00004090: 656c 6422 0a20 2020 2020 2020 2020 636c  eld".         cl
-000040a0: 6173 733d 2274 6578 742d 7769 6467 6574  ass="text-widget
-000040b0: 2072 6571 7569 7265 6420 696e 742d 6669   required int-fi
-000040c0: 656c 6422 0a20 2020 2020 2020 2020 7661  eld".         va
-000040d0: 6c75 653d 2236 3622 202f 3e0a 2020 2020  lue="66" />.    
-000040e0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-000040f0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00004100: 6469 7620 636c 6173 733d 226c 6162 656c  div class="label
-00004110: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00004120: 2020 2020 2020 2020 203c 6c61 6265 6c20           <label 
-00004130: 666f 723d 2266 6f72 6d2d 7769 6467 6574  for="form-widget
-00004140: 732d 7375 626f 626a 6563 742d 7769 6467  s-subobject-widg
-00004150: 6574 732d 6261 7266 6965 6c64 223e 0a20  ets-barfield">. 
-00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004170: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
-00004180: 616e 3e4d 7920 6465 6172 2062 6172 3c2f  an>My dear bar</
-00004190: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
-000041a0: 2020 2020 2020 2020 2020 2020 3c2f 6c61              </la
-000041b0: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
-000041c0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-000041d0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000041e0: 7373 3d22 7769 6467 6574 223e 0a20 2020  ss="widget">.   
-000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004200: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
-00004210: 7465 7874 220a 2020 2020 2020 2020 2069  text".         i
-00004220: 643d 2266 6f72 6d2d 7769 6467 6574 732d  d="form-widgets-
-00004230: 7375 626f 626a 6563 742d 7769 6467 6574  subobject-widget
-00004240: 732d 6261 7266 6965 6c64 220a 2020 2020  s-barfield".    
-00004250: 2020 2020 206e 616d 653d 2266 6f72 6d2e       name="form.
-00004260: 7769 6467 6574 732e 7375 626f 626a 6563  widgets.subobjec
-00004270: 742e 7769 6467 6574 732e 6261 7266 6965  t.widgets.barfie
-00004280: 6c64 220a 2020 2020 2020 2020 2063 6c61  ld".         cla
-00004290: 7373 3d22 7465 7874 2d77 6964 6765 7420  ss="text-widget 
-000042a0: 696e 742d 6669 656c 6422 0a20 2020 2020  int-field".     
-000042b0: 2020 2020 7661 6c75 653d 2239 3922 202f      value="99" /
-000042c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000042d0: 3c2f 6469 763e 0a20 2020 2020 203c 696e  </div>.      <in
-000042e0: 7075 7420 6e61 6d65 3d22 666f 726d 2e77  put name="form.w
-000042f0: 6964 6765 7473 2e73 7562 6f62 6a65 6374  idgets.subobject
-00004300: 2d65 6d70 7479 2d6d 6172 6b65 7222 2074  -empty-marker" t
-00004310: 7970 653d 2268 6964 6465 6e22 2076 616c  ype="hidden" val
-00004320: 7565 3d22 3122 2f3e 0a20 203c 2f64 6976  ue="1"/>.  </div
-00004330: 3e0a 2020 2020 3c2f 6469 763e 0a20 2020  >.    </div>.   
-00004340: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
-00004350: 223e 0a20 2020 2020 203c 6c61 6265 6c20  ">.      <label 
-00004360: 666f 723d 2266 6f72 6d2d 7769 6467 6574  for="form-widget
-00004370: 732d 6e61 6d65 223e 6e61 6d65 3c2f 6c61  s-name">name</la
-00004380: 6265 6c3e 0a20 2020 2020 203c 696e 7075  bel>.      <inpu
-00004390: 7420 7479 7065 3d22 7465 7874 220a 2020  t type="text".  
-000043a0: 2020 2020 2020 2069 643d 2266 6f72 6d2d         id="form-
-000043b0: 7769 6467 6574 732d 6e61 6d65 220a 2020  widgets-name".  
-000043c0: 2020 2020 2020 206e 616d 653d 2266 6f72         name="for
-000043d0: 6d2e 7769 6467 6574 732e 6e61 6d65 220a  m.widgets.name".
-000043e0: 2020 2020 2020 2020 2063 6c61 7373 3d22           class="
-000043f0: 7465 7874 2d77 6964 6765 7420 7265 7175  text-widget requ
-00004400: 6972 6564 2074 6578 746c 696e 652d 6669  ired textline-fi
-00004410: 656c 6422 0a20 2020 2020 2020 2020 7661  eld".         va
-00004420: 6c75 653d 2266 6972 7374 2220 2f3e 0a20  lue="first" />. 
-00004430: 2020 203c 2f64 6976 3e0a 2020 2020 3c64     </div>.    <d
-00004440: 6976 2063 6c61 7373 3d22 6163 7469 6f6e  iv class="action
-00004450: 223e 0a20 2020 2020 203c 696e 7075 7420  ">.      <input 
-00004460: 7479 7065 3d22 7375 626d 6974 220a 2020  type="submit".  
-00004470: 2020 2020 2020 2069 643d 2266 6f72 6d2d         id="form-
-00004480: 6275 7474 6f6e 732d 6170 706c 7922 0a20  buttons-apply". 
-00004490: 2020 2020 2020 2020 6e61 6d65 3d22 666f          name="fo
-000044a0: 726d 2e62 7574 746f 6e73 2e61 7070 6c79  rm.buttons.apply
-000044b0: 220a 2020 2020 2020 2020 2063 6c61 7373  ".         class
-000044c0: 3d22 7375 626d 6974 2d77 6964 6765 7420  ="submit-widget 
-000044d0: 6275 7474 6f6e 2d66 6965 6c64 220a 2020  button-field".  
-000044e0: 2020 2020 2020 2076 616c 7565 3d22 4170         value="Ap
-000044f0: 706c 7922 202f 3e0a 2020 2020 3c2f 6469  ply" />.    </di
-00004500: 763e 0a20 203c 2f66 6f72 6d3e 0a0a 4c65  v>.  </form>..Le
-00004510: 7427 7320 6d6f 6469 6679 2074 6865 2076  t's modify the v
-00004520: 616c 7565 733a 0a0a 2020 3e3e 3e20 7265  alues:..  >>> re
-00004530: 7175 6573 7420 3d20 5465 7374 5265 7175  quest = TestRequ
-00004540: 6573 7428 7061 7261 6d73 3d7b 0a20 202e  est(params={.  .
-00004550: 2e2e 2020 2020 2027 666f 726d 2e77 6964  ..     'form.wid
-00004560: 6765 7473 2e73 7562 6f62 6a65 6374 2e77  gets.subobject.w
-00004570: 6964 6765 7473 2e66 6f6f 6669 656c 6427  idgets.foofield'
-00004580: 3a27 3433 272c 0a20 202e 2e2e 2020 2020  :'43',.  ...    
-00004590: 2027 666f 726d 2e77 6964 6765 7473 2e73   'form.widgets.s
-000045a0: 7562 6f62 6a65 6374 2e77 6964 6765 7473  ubobject.widgets
-000045b0: 2e62 6172 6669 656c 6427 3a27 3535 272c  .barfield':'55',
-000045c0: 0a20 202e 2e2e 2020 2020 2027 666f 726d  .  ...     'form
-000045d0: 2e77 6964 6765 7473 2e6e 616d 6527 3a27  .widgets.name':'
-000045e0: 6669 7273 7427 2c0a 2020 2e2e 2e20 2020  first',.  ...   
-000045f0: 2020 2766 6f72 6d2e 7769 6467 6574 732e    'form.widgets.
-00004600: 7375 626f 626a 6563 742d 656d 7074 792d  subobject-empty-
-00004610: 6d61 726b 6572 273a 2731 272c 0a20 202e  marker':'1',.  .
-00004620: 2e2e 2020 2020 2027 666f 726d 2e62 7574  ..     'form.but
-00004630: 746f 6e73 2e61 7070 6c79 273a 2741 7070  tons.apply':'App
-00004640: 6c79 277d 290a 0a54 6865 7920 6172 6520  ly'})..They are 
-00004650: 7374 696c 6c20 7468 6520 7361 6d65 3a0a  still the same:.
-00004660: 0a20 203e 3e3e 2072 6f6f 745b 2766 6972  .  >>> root['fir
-00004670: 7374 275d 2e73 7562 6f62 6a65 6374 2e66  st'].subobject.f
-00004680: 6f6f 6669 656c 640a 2020 3636 0a20 203e  oofield.  66.  >
-00004690: 3e3e 2072 6f6f 745b 2766 6972 7374 275d  >> root['first']
-000046a0: 2e73 7562 6f62 6a65 6374 2e62 6172 6669  .subobject.barfi
-000046b0: 656c 640a 2020 3939 0a0a 2020 3e3e 3e20  eld.  99..  >>> 
-000046c0: 6564 6974 666f 726d 2e72 6571 7565 7374  editform.request
-000046d0: 203d 2072 6571 7565 7374 0a20 203e 3e3e   = request.  >>>
-000046e0: 2065 6469 7466 6f72 6d2e 7570 6461 7465   editform.update
-000046f0: 2829 0a0a 556e 7469 6c20 7765 2068 6176  ()..Until we hav
-00004700: 6520 7570 6461 7465 6420 7468 6520 666f  e updated the fo
-00004710: 726d 3a0a 0a20 203e 3e3e 2072 6f6f 745b  rm:..  >>> root[
-00004720: 2766 6972 7374 275d 2e73 7562 6f62 6a65  'first'].subobje
-00004730: 6374 2e66 6f6f 6669 656c 640a 2020 3433  ct.foofield.  43
-00004740: 0a20 203e 3e3e 2072 6f6f 745b 2766 6972  .  >>> root['fir
-00004750: 7374 275d 2e73 7562 6f62 6a65 6374 2e62  st'].subobject.b
-00004760: 6172 6669 656c 640a 2020 3535 0a0a 4c65  arfield.  55..Le
-00004770: 7427 7320 7365 6520 6f75 7220 6576 656e  t's see our even
-00004780: 7420 6c6f 673a 0a0a 2020 3e3e 3e20 6c65  t log:..  >>> le
-00004790: 6e28 6576 656e 746c 6f67 290a 2020 320a  n(eventlog).  2.
-000047a0: 0a20 203e 3e3e 2070 7269 6e74 4576 656e  .  >>> printEven
-000047b0: 7473 2829 0a20 203c 7a6f 7065 2e2e 2e4f  ts().  <zope...O
-000047c0: 626a 6563 744d 6f64 6966 6965 6445 7665  bjectModifiedEve
-000047d0: 6e74 206f 626a 6563 7420 6174 202e 2e2e  nt object at ...
-000047e0: 3e0a 2020 7079 616d 735f 666f 726d 2e74  >.  pyams_form.t
-000047f0: 6573 7469 6e67 2e49 4d79 5375 624f 626a  esting.IMySubObj
-00004800: 6563 740a 2020 5b27 6261 7266 6965 6c64  ect.  ['barfield
-00004810: 272c 2027 666f 6f66 6965 6c64 275d 0a20  ', 'foofield']. 
-00004820: 203c 7a6f 7065 2e2e 2e4f 626a 6563 744d   <zope...ObjectM
-00004830: 6f64 6966 6965 6445 7665 6e74 206f 626a  odifiedEvent obj
-00004840: 6563 7420 6174 202e 2e2e 3e0a 2020 7079  ect at ...>.  py
-00004850: 616d 735f 666f 726d 2e74 6573 7469 6e67  ams_form.testing
-00004860: 2e49 4d79 4f62 6a65 6374 0a20 205b 2773  .IMyObject.  ['s
-00004870: 7562 6f62 6a65 6374 275d 0a0a 0a20 203e  ubobject']...  >
-00004880: 3e3e 2065 7665 6e74 6c6f 673d 5b5d 0a0a  >> eventlog=[]..
-00004890: 0a41 6674 6572 2074 6865 2075 7064 6174  .After the updat
-000048a0: 6520 7468 6520 666f 726d 2073 6179 7320  e the form says 
-000048b0: 7468 6174 2074 6865 2076 616c 7565 7320  that the values 
-000048c0: 676f 7420 7570 6461 7465 6420 616e 6420  got updated and 
-000048d0: 7265 6e64 6572 7320 7468 6520 6e65 770a  renders the new.
-000048e0: 7661 6c75 6573 3a0a 0a20 203e 3e3e 2070  values:..  >>> p
-000048f0: 7269 6e74 2866 6f72 6d61 745f 6874 6d6c  rint(format_html
-00004900: 2865 6469 7466 6f72 6d2e 7265 6e64 6572  (editform.render
-00004910: 2829 2929 0a20 203c 693e 4461 7461 2073  ())).  <i>Data s
-00004920: 7563 6365 7373 6675 6c6c 7920 7570 6461  uccessfully upda
-00004930: 7465 642e 3c2f 693e 0a20 203c 666f 726d  ted.</i>.  <form
-00004940: 2061 6374 696f 6e3d 222e 223e 0a20 2020   action=".">.   
-00004950: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
-00004960: 223e 0a20 2020 2020 203c 6c61 6265 6c20  ">.      <label 
-00004970: 666f 723d 2266 6f72 6d2d 7769 6467 6574  for="form-widget
-00004980: 732d 7375 626f 626a 6563 7422 3e6d 7920  s-subobject">my 
-00004990: 6f62 6a65 6374 3c2f 6c61 6265 6c3e 0a20  object</label>. 
-000049a0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-000049b0: 226f 626a 6563 742d 7769 6467 6574 2072  "object-widget r
-000049c0: 6571 7569 7265 6422 3e0a 2020 2020 2020  equired">.      
-000049d0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000049e0: 7373 3d22 6c61 6265 6c22 3e0a 2020 2020  ss="label">.    
-000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a00: 2020 3c6c 6162 656c 2066 6f72 3d22 666f    <label for="fo
-00004a10: 726d 2d77 6964 6765 7473 2d73 7562 6f62  rm-widgets-subob
-00004a20: 6a65 6374 2d77 6964 6765 7473 2d66 6f6f  ject-widgets-foo
-00004a30: 6669 656c 6422 3e0a 2020 2020 2020 2020  field">.        
+00003f80: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
+00003f90: 6e20 636c 6173 733d 2272 6571 7569 7265  n class="require
+00003fa0: 6422 3e2a 3c2f 7370 616e 3e0a 2020 2020  d">*</span>.    
+00003fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fc0: 2020 3c2f 6c61 6265 6c3e 0a20 2020 2020    </label>.     
+00003fd0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00003fe0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00003ff0: 6976 2063 6c61 7373 3d22 7769 6467 6574  iv class="widget
+00004000: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00004010: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
+00004020: 7479 7065 3d22 7465 7874 220a 2020 2020  type="text".    
+00004030: 2020 2020 2069 643d 2266 6f72 6d2d 7769       id="form-wi
+00004040: 6467 6574 732d 7375 626f 626a 6563 742d  dgets-subobject-
+00004050: 7769 6467 6574 732d 666f 6f66 6965 6c64  widgets-foofield
+00004060: 220a 2020 2020 2020 2020 206e 616d 653d  ".         name=
+00004070: 2266 6f72 6d2e 7769 6467 6574 732e 7375  "form.widgets.su
+00004080: 626f 626a 6563 742e 7769 6467 6574 732e  bobject.widgets.
+00004090: 666f 6f66 6965 6c64 220a 2020 2020 2020  foofield".      
+000040a0: 2020 2063 6c61 7373 3d22 7465 7874 2d77     class="text-w
+000040b0: 6964 6765 7420 7265 7175 6972 6564 2069  idget required i
+000040c0: 6e74 2d66 6965 6c64 220a 2020 2020 2020  nt-field".      
+000040d0: 2020 2076 616c 7565 3d22 3636 2220 2f3e     value="66" />
+000040e0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+000040f0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00004100: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00004110: 6c61 6265 6c22 3e0a 2020 2020 2020 2020  label">.        
+00004120: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
+00004130: 6162 656c 2066 6f72 3d22 666f 726d 2d77  abel for="form-w
+00004140: 6964 6765 7473 2d73 7562 6f62 6a65 6374  idgets-subobject
+00004150: 2d77 6964 6765 7473 2d62 6172 6669 656c  -widgets-barfiel
+00004160: 6422 3e0a 2020 2020 2020 2020 2020 2020  d">.            
+00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004180: 2020 3c73 7061 6e3e 4d79 2064 6561 7220    <span>My dear 
+00004190: 6261 723c 2f73 7061 6e3e 0a20 2020 2020  bar</span>.     
+000041a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041b0: 203c 2f6c 6162 656c 3e0a 2020 2020 2020   </label>.      
+000041c0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+000041d0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+000041e0: 7620 636c 6173 733d 2277 6964 6765 7422  v class="widget"
+000041f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004200: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
+00004210: 7970 653d 2274 6578 7422 0a20 2020 2020  ype="text".     
+00004220: 2020 2020 6964 3d22 666f 726d 2d77 6964      id="form-wid
+00004230: 6765 7473 2d73 7562 6f62 6a65 6374 2d77  gets-subobject-w
+00004240: 6964 6765 7473 2d62 6172 6669 656c 6422  idgets-barfield"
+00004250: 0a20 2020 2020 2020 2020 6e61 6d65 3d22  .         name="
+00004260: 666f 726d 2e77 6964 6765 7473 2e73 7562  form.widgets.sub
+00004270: 6f62 6a65 6374 2e77 6964 6765 7473 2e62  object.widgets.b
+00004280: 6172 6669 656c 6422 0a20 2020 2020 2020  arfield".       
+00004290: 2020 636c 6173 733d 2274 6578 742d 7769    class="text-wi
+000042a0: 6467 6574 2069 6e74 2d66 6965 6c64 220a  dget int-field".
+000042b0: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
+000042c0: 3939 2220 2f3e 0a20 2020 2020 2020 2020  99" />.         
+000042d0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+000042e0: 2020 3c69 6e70 7574 206e 616d 653d 2266    <input name="f
+000042f0: 6f72 6d2e 7769 6467 6574 732e 7375 626f  orm.widgets.subo
+00004300: 626a 6563 742d 656d 7074 792d 6d61 726b  bject-empty-mark
+00004310: 6572 2220 7479 7065 3d22 6869 6464 656e  er" type="hidden
+00004320: 2220 7661 6c75 653d 2231 2220 2f3e 0a20  " value="1" />. 
+00004330: 203c 2f64 6976 3e0a 2020 2020 3c2f 6469   </div>.    </di
+00004340: 763e 0a20 2020 203c 6469 7620 636c 6173  v>.    <div clas
+00004350: 733d 2272 6f77 223e 0a20 2020 2020 203c  s="row">.      <
+00004360: 6c61 6265 6c20 666f 723d 2266 6f72 6d2d  label for="form-
+00004370: 7769 6467 6574 732d 6e61 6d65 223e 6e61  widgets-name">na
+00004380: 6d65 3c2f 6c61 6265 6c3e 0a20 2020 2020  me</label>.     
+00004390: 203c 696e 7075 7420 7479 7065 3d22 7465   <input type="te
+000043a0: 7874 220a 2020 2020 2020 2020 2069 643d  xt".         id=
+000043b0: 2266 6f72 6d2d 7769 6467 6574 732d 6e61  "form-widgets-na
+000043c0: 6d65 220a 2020 2020 2020 2020 206e 616d  me".         nam
+000043d0: 653d 2266 6f72 6d2e 7769 6467 6574 732e  e="form.widgets.
+000043e0: 6e61 6d65 220a 2020 2020 2020 2020 2063  name".         c
+000043f0: 6c61 7373 3d22 7465 7874 2d77 6964 6765  lass="text-widge
+00004400: 7420 7265 7175 6972 6564 2074 6578 746c  t required textl
+00004410: 696e 652d 6669 656c 6422 0a20 2020 2020  ine-field".     
+00004420: 2020 2020 7661 6c75 653d 2266 6972 7374      value="first
+00004430: 2220 2f3e 0a20 2020 203c 2f64 6976 3e0a  " />.    </div>.
+00004440: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00004450: 6163 7469 6f6e 223e 0a20 2020 2020 203c  action">.      <
+00004460: 696e 7075 7420 7479 7065 3d22 7375 626d  input type="subm
+00004470: 6974 220a 2020 2020 2020 2020 2069 643d  it".         id=
+00004480: 2266 6f72 6d2d 6275 7474 6f6e 732d 6170  "form-buttons-ap
+00004490: 706c 7922 0a20 2020 2020 2020 2020 6e61  ply".         na
+000044a0: 6d65 3d22 666f 726d 2e62 7574 746f 6e73  me="form.buttons
+000044b0: 2e61 7070 6c79 220a 2020 2020 2020 2020  .apply".        
+000044c0: 2063 6c61 7373 3d22 7375 626d 6974 2d77   class="submit-w
+000044d0: 6964 6765 7420 6275 7474 6f6e 2d66 6965  idget button-fie
+000044e0: 6c64 220a 2020 2020 2020 2020 2076 616c  ld".         val
+000044f0: 7565 3d22 4170 706c 7922 202f 3e0a 2020  ue="Apply" />.  
+00004500: 2020 3c2f 6469 763e 0a20 203c 2f66 6f72    </div>.  </for
+00004510: 6d3e 0a0a 4c65 7427 7320 6d6f 6469 6679  m>..Let's modify
+00004520: 2074 6865 2076 616c 7565 733a 0a0a 2020   the values:..  
+00004530: 3e3e 3e20 7265 7175 6573 7420 3d20 5465  >>> request = Te
+00004540: 7374 5265 7175 6573 7428 7061 7261 6d73  stRequest(params
+00004550: 3d7b 0a20 202e 2e2e 2020 2020 2027 666f  ={.  ...     'fo
+00004560: 726d 2e77 6964 6765 7473 2e73 7562 6f62  rm.widgets.subob
+00004570: 6a65 6374 2e77 6964 6765 7473 2e66 6f6f  ject.widgets.foo
+00004580: 6669 656c 6427 3a27 3433 272c 0a20 202e  field':'43',.  .
+00004590: 2e2e 2020 2020 2027 666f 726d 2e77 6964  ..     'form.wid
+000045a0: 6765 7473 2e73 7562 6f62 6a65 6374 2e77  gets.subobject.w
+000045b0: 6964 6765 7473 2e62 6172 6669 656c 6427  idgets.barfield'
+000045c0: 3a27 3535 272c 0a20 202e 2e2e 2020 2020  :'55',.  ...    
+000045d0: 2027 666f 726d 2e77 6964 6765 7473 2e6e   'form.widgets.n
+000045e0: 616d 6527 3a27 6669 7273 7427 2c0a 2020  ame':'first',.  
+000045f0: 2e2e 2e20 2020 2020 2766 6f72 6d2e 7769  ...     'form.wi
+00004600: 6467 6574 732e 7375 626f 626a 6563 742d  dgets.subobject-
+00004610: 656d 7074 792d 6d61 726b 6572 273a 2731  empty-marker':'1
+00004620: 272c 0a20 202e 2e2e 2020 2020 2027 666f  ',.  ...     'fo
+00004630: 726d 2e62 7574 746f 6e73 2e61 7070 6c79  rm.buttons.apply
+00004640: 273a 2741 7070 6c79 277d 290a 0a54 6865  ':'Apply'})..The
+00004650: 7920 6172 6520 7374 696c 6c20 7468 6520  y are still the 
+00004660: 7361 6d65 3a0a 0a20 203e 3e3e 2072 6f6f  same:..  >>> roo
+00004670: 745b 2766 6972 7374 275d 2e73 7562 6f62  t['first'].subob
+00004680: 6a65 6374 2e66 6f6f 6669 656c 640a 2020  ject.foofield.  
+00004690: 3636 0a20 203e 3e3e 2072 6f6f 745b 2766  66.  >>> root['f
+000046a0: 6972 7374 275d 2e73 7562 6f62 6a65 6374  irst'].subobject
+000046b0: 2e62 6172 6669 656c 640a 2020 3939 0a0a  .barfield.  99..
+000046c0: 2020 3e3e 3e20 6564 6974 666f 726d 2e72    >>> editform.r
+000046d0: 6571 7565 7374 203d 2072 6571 7565 7374  equest = request
+000046e0: 0a20 203e 3e3e 2065 6469 7466 6f72 6d2e  .  >>> editform.
+000046f0: 7570 6461 7465 2829 0a0a 556e 7469 6c20  update()..Until 
+00004700: 7765 2068 6176 6520 7570 6461 7465 6420  we have updated 
+00004710: 7468 6520 666f 726d 3a0a 0a20 203e 3e3e  the form:..  >>>
+00004720: 2072 6f6f 745b 2766 6972 7374 275d 2e73   root['first'].s
+00004730: 7562 6f62 6a65 6374 2e66 6f6f 6669 656c  ubobject.foofiel
+00004740: 640a 2020 3433 0a20 203e 3e3e 2072 6f6f  d.  43.  >>> roo
+00004750: 745b 2766 6972 7374 275d 2e73 7562 6f62  t['first'].subob
+00004760: 6a65 6374 2e62 6172 6669 656c 640a 2020  ject.barfield.  
+00004770: 3535 0a0a 4c65 7427 7320 7365 6520 6f75  55..Let's see ou
+00004780: 7220 6576 656e 7420 6c6f 673a 0a0a 2020  r event log:..  
+00004790: 3e3e 3e20 6c65 6e28 6576 656e 746c 6f67  >>> len(eventlog
+000047a0: 290a 2020 320a 0a20 203e 3e3e 2070 7269  ).  2..  >>> pri
+000047b0: 6e74 4576 656e 7473 2829 0a20 203c 7a6f  ntEvents().  <zo
+000047c0: 7065 2e2e 2e4f 626a 6563 744d 6f64 6966  pe...ObjectModif
+000047d0: 6965 6445 7665 6e74 206f 626a 6563 7420  iedEvent object 
+000047e0: 6174 202e 2e2e 3e0a 2020 7079 616d 735f  at ...>.  pyams_
+000047f0: 666f 726d 2e74 6573 7469 6e67 2e49 4d79  form.testing.IMy
+00004800: 5375 624f 626a 6563 740a 2020 5b27 6261  SubObject.  ['ba
+00004810: 7266 6965 6c64 272c 2027 666f 6f66 6965  rfield', 'foofie
+00004820: 6c64 275d 0a20 203c 7a6f 7065 2e2e 2e4f  ld'].  <zope...O
+00004830: 626a 6563 744d 6f64 6966 6965 6445 7665  bjectModifiedEve
+00004840: 6e74 206f 626a 6563 7420 6174 202e 2e2e  nt object at ...
+00004850: 3e0a 2020 7079 616d 735f 666f 726d 2e74  >.  pyams_form.t
+00004860: 6573 7469 6e67 2e49 4d79 4f62 6a65 6374  esting.IMyObject
+00004870: 0a20 205b 2773 7562 6f62 6a65 6374 275d  .  ['subobject']
+00004880: 0a0a 0a20 203e 3e3e 2065 7665 6e74 6c6f  ...  >>> eventlo
+00004890: 673d 5b5d 0a0a 0a41 6674 6572 2074 6865  g=[]...After the
+000048a0: 2075 7064 6174 6520 7468 6520 666f 726d   update the form
+000048b0: 2073 6179 7320 7468 6174 2074 6865 2076   says that the v
+000048c0: 616c 7565 7320 676f 7420 7570 6461 7465  alues got update
+000048d0: 6420 616e 6420 7265 6e64 6572 7320 7468  d and renders th
+000048e0: 6520 6e65 770a 7661 6c75 6573 3a0a 0a20  e new.values:.. 
+000048f0: 203e 3e3e 2070 7269 6e74 2866 6f72 6d61   >>> print(forma
+00004900: 745f 6874 6d6c 2865 6469 7466 6f72 6d2e  t_html(editform.
+00004910: 7265 6e64 6572 2829 2929 0a20 203c 693e  render())).  <i>
+00004920: 4461 7461 2073 7563 6365 7373 6675 6c6c  Data successfull
+00004930: 7920 7570 6461 7465 642e 3c2f 693e 0a20  y updated.</i>. 
+00004940: 203c 666f 726d 2061 6374 696f 6e3d 222e   <form action=".
+00004950: 223e 0a20 2020 203c 6469 7620 636c 6173  ">.    <div clas
+00004960: 733d 2272 6f77 223e 0a20 2020 2020 203c  s="row">.      <
+00004970: 6c61 6265 6c20 666f 723d 2266 6f72 6d2d  label for="form-
+00004980: 7769 6467 6574 732d 7375 626f 626a 6563  widgets-subobjec
+00004990: 7422 3e6d 7920 6f62 6a65 6374 3c2f 6c61  t">my object</la
+000049a0: 6265 6c3e 0a20 2020 2020 203c 6469 7620  bel>.      <div 
+000049b0: 636c 6173 733d 226f 626a 6563 742d 7769  class="object-wi
+000049c0: 6467 6574 2072 6571 7569 7265 6422 3e0a  dget required">.
+000049d0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+000049e0: 6976 2063 6c61 7373 3d22 6c61 6265 6c22  iv class="label"
+000049f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004a00: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
+00004a10: 6f72 3d22 666f 726d 2d77 6964 6765 7473  or="form-widgets
+00004a20: 2d73 7562 6f62 6a65 6374 2d77 6964 6765  -subobject-widge
+00004a30: 7473 2d66 6f6f 6669 656c 6422 3e0a 2020  ts-foofield">.  
 00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a50: 2020 2020 2020 3c73 7061 6e3e 4d79 2066        <span>My f
-00004a60: 6f6f 2066 6965 6c64 3c2f 7370 616e 3e0a  oo field</span>.
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a80: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00004a90: 7061 6e20 636c 6173 733d 2272 6571 7569  pan class="requi
-00004aa0: 7265 6422 3e2a 3c2f 7370 616e 3e0a 2020  red">*</span>.  
-00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ac0: 2020 2020 3c2f 6c61 6265 6c3e 0a20 2020      </label>.   
-00004ad0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00004ae0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00004af0: 3c64 6976 2063 6c61 7373 3d22 7769 6467  <div class="widg
-00004b00: 6574 223e 0a20 2020 2020 2020 2020 2020  et">.           
-00004b10: 2020 2020 2020 2020 2020 203c 696e 7075             <inpu
-00004b20: 7420 7479 7065 3d22 7465 7874 220a 2020  t type="text".  
-00004b30: 2020 2020 2020 2069 643d 2266 6f72 6d2d         id="form-
-00004b40: 7769 6467 6574 732d 7375 626f 626a 6563  widgets-subobjec
-00004b50: 742d 7769 6467 6574 732d 666f 6f66 6965  t-widgets-foofie
-00004b60: 6c64 220a 2020 2020 2020 2020 206e 616d  ld".         nam
-00004b70: 653d 2266 6f72 6d2e 7769 6467 6574 732e  e="form.widgets.
-00004b80: 7375 626f 626a 6563 742e 7769 6467 6574  subobject.widget
-00004b90: 732e 666f 6f66 6965 6c64 220a 2020 2020  s.foofield".    
-00004ba0: 2020 2020 2063 6c61 7373 3d22 7465 7874       class="text
-00004bb0: 2d77 6964 6765 7420 7265 7175 6972 6564  -widget required
-00004bc0: 2069 6e74 2d66 6965 6c64 220a 2020 2020   int-field".    
-00004bd0: 2020 2020 2076 616c 7565 3d22 3433 2220       value="43" 
-00004be0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00004bf0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00004c00: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00004c10: 3d22 6c61 6265 6c22 3e0a 2020 2020 2020  ="label">.      
+00004a50: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
+00004a60: 6e3e 4d79 2066 6f6f 2066 6965 6c64 3c2f  n>My foo field</
+00004a70: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
+00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a90: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+00004aa0: 2272 6571 7569 7265 6422 3e2a 3c2f 7370  "required">*</sp
+00004ab0: 616e 3e0a 2020 2020 2020 2020 2020 2020  an>.            
+00004ac0: 2020 2020 2020 2020 2020 3c2f 6c61 6265            </labe
+00004ad0: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
+00004ae0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00004af0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00004b00: 3d22 7769 6467 6574 223e 0a20 2020 2020  ="widget">.     
+00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b20: 203c 696e 7075 7420 7479 7065 3d22 7465   <input type="te
+00004b30: 7874 220a 2020 2020 2020 2020 2069 643d  xt".         id=
+00004b40: 2266 6f72 6d2d 7769 6467 6574 732d 7375  "form-widgets-su
+00004b50: 626f 626a 6563 742d 7769 6467 6574 732d  bobject-widgets-
+00004b60: 666f 6f66 6965 6c64 220a 2020 2020 2020  foofield".      
+00004b70: 2020 206e 616d 653d 2266 6f72 6d2e 7769     name="form.wi
+00004b80: 6467 6574 732e 7375 626f 626a 6563 742e  dgets.subobject.
+00004b90: 7769 6467 6574 732e 666f 6f66 6965 6c64  widgets.foofield
+00004ba0: 220a 2020 2020 2020 2020 2063 6c61 7373  ".         class
+00004bb0: 3d22 7465 7874 2d77 6964 6765 7420 7265  ="text-widget re
+00004bc0: 7175 6972 6564 2069 6e74 2d66 6965 6c64  quired int-field
+00004bd0: 220a 2020 2020 2020 2020 2076 616c 7565  ".         value
+00004be0: 3d22 3433 2220 2f3e 0a20 2020 2020 2020  ="43" />.       
+00004bf0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00004c00: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00004c10: 2063 6c61 7373 3d22 6c61 6265 6c22 3e0a   class="label">.
 00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 3c6c 6162 656c 2066 6f72 3d22 666f 726d  <label for="form
-00004c40: 2d77 6964 6765 7473 2d73 7562 6f62 6a65  -widgets-subobje
-00004c50: 6374 2d77 6964 6765 7473 2d62 6172 6669  ct-widgets-barfi
-00004c60: 656c 6422 3e0a 2020 2020 2020 2020 2020  eld">.          
+00004c30: 2020 2020 2020 3c6c 6162 656c 2066 6f72        <label for
+00004c40: 3d22 666f 726d 2d77 6964 6765 7473 2d73  ="form-widgets-s
+00004c50: 7562 6f62 6a65 6374 2d77 6964 6765 7473  ubobject-widgets
+00004c60: 2d62 6172 6669 656c 6422 3e0a 2020 2020  -barfield">.    
 00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c80: 2020 2020 3c73 7061 6e3e 4d79 2064 6561      <span>My dea
-00004c90: 7220 6261 723c 2f73 7061 6e3e 0a20 2020  r bar</span>.   
-00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cb0: 2020 203c 2f6c 6162 656c 3e0a 2020 2020     </label>.    
-00004cc0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00004cd0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00004ce0: 6469 7620 636c 6173 733d 2277 6964 6765  div class="widge
-00004cf0: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-00004d00: 2020 2020 2020 2020 2020 3c69 6e70 7574            <input
-00004d10: 2074 7970 653d 2274 6578 7422 0a20 2020   type="text".   
-00004d20: 2020 2020 2020 6964 3d22 666f 726d 2d77        id="form-w
-00004d30: 6964 6765 7473 2d73 7562 6f62 6a65 6374  idgets-subobject
-00004d40: 2d77 6964 6765 7473 2d62 6172 6669 656c  -widgets-barfiel
-00004d50: 6422 0a20 2020 2020 2020 2020 6e61 6d65  d".         name
-00004d60: 3d22 666f 726d 2e77 6964 6765 7473 2e73  ="form.widgets.s
-00004d70: 7562 6f62 6a65 6374 2e77 6964 6765 7473  ubobject.widgets
-00004d80: 2e62 6172 6669 656c 6422 0a20 2020 2020  .barfield".     
-00004d90: 2020 2020 636c 6173 733d 2274 6578 742d      class="text-
-00004da0: 7769 6467 6574 2069 6e74 2d66 6965 6c64  widget int-field
-00004db0: 220a 2020 2020 2020 2020 2076 616c 7565  ".         value
-00004dc0: 3d22 3535 2220 2f3e 0a20 2020 2020 2020  ="55" />.       
-00004dd0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00004de0: 2020 2020 3c69 6e70 7574 206e 616d 653d      <input name=
-00004df0: 2266 6f72 6d2e 7769 6467 6574 732e 7375  "form.widgets.su
-00004e00: 626f 626a 6563 742d 656d 7074 792d 6d61  bobject-empty-ma
-00004e10: 726b 6572 2220 7479 7065 3d22 6869 6464  rker" type="hidd
-00004e20: 656e 2220 7661 6c75 653d 2231 222f 3e0a  en" value="1"/>.
-00004e30: 2020 3c2f 6469 763e 0a20 2020 203c 2f64    </div>.    </d
-00004e40: 6976 3e0a 2020 2020 3c64 6976 2063 6c61  iv>.    <div cla
-00004e50: 7373 3d22 726f 7722 3e0a 2020 2020 2020  ss="row">.      
-00004e60: 3c6c 6162 656c 2066 6f72 3d22 666f 726d  <label for="form
-00004e70: 2d77 6964 6765 7473 2d6e 616d 6522 3e6e  -widgets-name">n
-00004e80: 616d 653c 2f6c 6162 656c 3e0a 2020 2020  ame</label>.    
-00004e90: 2020 3c69 6e70 7574 2074 7970 653d 2274    <input type="t
-00004ea0: 6578 7422 0a20 2020 2020 2020 2020 6964  ext".         id
-00004eb0: 3d22 666f 726d 2d77 6964 6765 7473 2d6e  ="form-widgets-n
-00004ec0: 616d 6522 0a20 2020 2020 2020 2020 6e61  ame".         na
-00004ed0: 6d65 3d22 666f 726d 2e77 6964 6765 7473  me="form.widgets
-00004ee0: 2e6e 616d 6522 0a20 2020 2020 2020 2020  .name".         
-00004ef0: 636c 6173 733d 2274 6578 742d 7769 6467  class="text-widg
-00004f00: 6574 2072 6571 7569 7265 6420 7465 7874  et required text
-00004f10: 6c69 6e65 2d66 6965 6c64 220a 2020 2020  line-field".    
-00004f20: 2020 2020 2076 616c 7565 3d22 6669 7273       value="firs
-00004f30: 7422 202f 3e0a 2020 2020 3c2f 6469 763e  t" />.    </div>
-00004f40: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
-00004f50: 2261 6374 696f 6e22 3e0a 2020 2020 2020  "action">.      
-00004f60: 3c69 6e70 7574 2074 7970 653d 2273 7562  <input type="sub
-00004f70: 6d69 7422 0a20 2020 2020 2020 2020 6964  mit".         id
-00004f80: 3d22 666f 726d 2d62 7574 746f 6e73 2d61  ="form-buttons-a
-00004f90: 7070 6c79 220a 2020 2020 2020 2020 206e  pply".         n
-00004fa0: 616d 653d 2266 6f72 6d2e 6275 7474 6f6e  ame="form.button
-00004fb0: 732e 6170 706c 7922 0a20 2020 2020 2020  s.apply".       
-00004fc0: 2020 636c 6173 733d 2273 7562 6d69 742d    class="submit-
-00004fd0: 7769 6467 6574 2062 7574 746f 6e2d 6669  widget button-fi
-00004fe0: 656c 6422 0a20 2020 2020 2020 2020 7661  eld".         va
-00004ff0: 6c75 653d 2241 7070 6c79 2220 2f3e 0a20  lue="Apply" />. 
-00005000: 2020 203c 2f64 6976 3e0a 2020 3c2f 666f     </div>.  </fo
-00005010: 726d 3e0a 0a4c 6574 2773 2073 6565 2069  rm>..Let's see i
-00005020: 6620 7468 6520 7769 6467 6574 206b 6565  f the widget kee
-00005030: 7073 2074 6865 206f 6c64 206f 626a 6563  ps the old objec
-00005040: 7420 6f6e 2065 6469 7469 6e67 3a0a 0a57  t on editing:..W
-00005050: 6520 6164 6420 6120 7370 6563 6961 6c20  e add a special 
-00005060: 7072 6f70 6572 7479 2074 6f20 6b65 6570  property to keep
-00005070: 2074 7261 636b 206f 6620 7468 6520 6f62   track of the ob
-00005080: 6a65 6374 3a0a 0a20 203e 3e3e 2072 6f6f  ject:..  >>> roo
-00005090: 745b 2766 6972 7374 275d 2e5f 5f6d 6172  t['first'].__mar
-000050a0: 6b65 725f 5f20 3d20 2254 6869 734d 7573  ker__ = "ThisMus
-000050b0: 7453 7461 7954 6865 5361 6d65 220a 0a20  tStayTheSame".. 
-000050c0: 203e 3e3e 2072 6f6f 745b 2766 6972 7374   >>> root['first
-000050d0: 275d 2e73 7562 6f62 6a65 6374 2e66 6f6f  '].subobject.foo
-000050e0: 6669 656c 640a 2020 3433 0a20 203e 3e3e  field.  43.  >>>
-000050f0: 2072 6f6f 745b 2766 6972 7374 275d 2e73   root['first'].s
-00005100: 7562 6f62 6a65 6374 2e62 6172 6669 656c  ubobject.barfiel
-00005110: 640a 2020 3535 0a0a 4c65 7427 7320 6d6f  d.  55..Let's mo
-00005120: 6469 6679 2074 6865 2076 616c 7565 733a  dify the values:
-00005130: 0a0a 2020 3e3e 3e20 7265 7175 6573 7420  ..  >>> request 
-00005140: 3d20 5465 7374 5265 7175 6573 7428 7061  = TestRequest(pa
-00005150: 7261 6d73 3d7b 0a20 202e 2e2e 2020 2020  rams={.  ...    
-00005160: 2027 666f 726d 2e77 6964 6765 7473 2e73   'form.widgets.s
-00005170: 7562 6f62 6a65 6374 2e77 6964 6765 7473  ubobject.widgets
-00005180: 2e66 6f6f 6669 656c 6427 3a27 3636 3627  .foofield':'666'
-00005190: 2c0a 2020 2e2e 2e20 2020 2020 2766 6f72  ,.  ...     'for
-000051a0: 6d2e 7769 6467 6574 732e 7375 626f 626a  m.widgets.subobj
-000051b0: 6563 742e 7769 6467 6574 732e 6261 7266  ect.widgets.barf
-000051c0: 6965 6c64 273a 2739 3939 272c 0a20 202e  ield':'999',.  .
-000051d0: 2e2e 2020 2020 2027 666f 726d 2e77 6964  ..     'form.wid
-000051e0: 6765 7473 2e6e 616d 6527 3a27 6669 7273  gets.name':'firs
-000051f0: 7427 2c0a 2020 2e2e 2e20 2020 2020 2766  t',.  ...     'f
-00005200: 6f72 6d2e 7769 6467 6574 732e 7375 626f  orm.widgets.subo
-00005210: 626a 6563 742d 656d 7074 792d 6d61 726b  bject-empty-mark
-00005220: 6572 273a 2731 272c 0a20 202e 2e2e 2020  er':'1',.  ...  
-00005230: 2020 2027 666f 726d 2e62 7574 746f 6e73     'form.buttons
-00005240: 2e61 7070 6c79 273a 2741 7070 6c79 277d  .apply':'Apply'}
-00005250: 290a 0a20 203e 3e3e 2065 6469 7466 6f72  )..  >>> editfor
-00005260: 6d2e 7265 7175 6573 7420 3d20 7265 7175  m.request = requ
-00005270: 6573 740a 0a20 203e 3e3e 2065 6469 7466  est..  >>> editf
-00005280: 6f72 6d2e 7570 6461 7465 2829 0a0a 4c65  orm.update()..Le
-00005290: 7427 7320 6368 6563 6b20 7768 6174 2061  t's check what a
-000052a0: 7265 2074 6865 7220 6573 756c 7473 206f  re ther esults o
-000052b0: 6620 7468 6520 7570 6461 7465 3a0a 0a20  f the update:.. 
-000052c0: 203e 3e3e 2072 6f6f 745b 2766 6972 7374   >>> root['first
-000052d0: 275d 2e73 7562 6f62 6a65 6374 2e66 6f6f  '].subobject.foo
-000052e0: 6669 656c 640a 2020 3636 360a 2020 3e3e  field.  666.  >>
-000052f0: 3e20 726f 6f74 5b27 6669 7273 7427 5d2e  > root['first'].
-00005300: 7375 626f 626a 6563 742e 6261 7266 6965  subobject.barfie
-00005310: 6c64 0a20 2039 3939 0a20 203e 3e3e 2072  ld.  999.  >>> r
-00005320: 6f6f 745b 2766 6972 7374 275d 2e5f 5f6d  oot['first'].__m
-00005330: 6172 6b65 725f 5f0a 2020 2754 6869 734d  arker__.  'ThisM
-00005340: 7573 7453 7461 7954 6865 5361 6d65 270a  ustStayTheSame'.
-00005350: 0a0a 4c65 7427 7320 6d61 6b65 2061 206e  ..Let's make a n
-00005360: 6173 7479 2065 7272 6f72 2c20 6279 2074  asty error, by t
-00005370: 7970 696e 6720 2762 6164 2720 696e 7374  yping 'bad' inst
-00005380: 6561 6420 6f66 2061 6e20 696e 7465 6765  ead of an intege
-00005390: 723a 0a0a 2020 3e3e 3e20 7265 7175 6573  r:..  >>> reques
-000053a0: 7420 3d20 5465 7374 5265 7175 6573 7428  t = TestRequest(
-000053b0: 7061 7261 6d73 3d7b 0a20 202e 2e2e 2020  params={.  ...  
-000053c0: 2020 2027 666f 726d 2e77 6964 6765 7473     'form.widgets
-000053d0: 2e73 7562 6f62 6a65 6374 2e77 6964 6765  .subobject.widge
-000053e0: 7473 2e66 6f6f 6669 656c 6427 3a27 3939  ts.foofield':'99
-000053f0: 272c 0a20 202e 2e2e 2020 2020 2027 666f  ',.  ...     'fo
-00005400: 726d 2e77 6964 6765 7473 2e73 7562 6f62  rm.widgets.subob
-00005410: 6a65 6374 2e77 6964 6765 7473 2e62 6172  ject.widgets.bar
-00005420: 6669 656c 6427 3a27 6261 6427 2c0a 2020  field':'bad',.  
-00005430: 2e2e 2e20 2020 2020 2766 6f72 6d2e 7769  ...     'form.wi
-00005440: 6467 6574 732e 6e61 6d65 273a 2766 6972  dgets.name':'fir
-00005450: 7374 272c 0a20 202e 2e2e 2020 2020 2027  st',.  ...     '
-00005460: 666f 726d 2e77 6964 6765 7473 2e73 7562  form.widgets.sub
-00005470: 6f62 6a65 6374 2d65 6d70 7479 2d6d 6172  object-empty-mar
-00005480: 6b65 7227 3a27 3127 2c0a 2020 2e2e 2e20  ker':'1',.  ... 
-00005490: 2020 2020 2766 6f72 6d2e 6275 7474 6f6e      'form.button
-000054a0: 732e 6170 706c 7927 3a27 4170 706c 7927  s.apply':'Apply'
-000054b0: 7d29 0a0a 2020 3e3e 3e20 6564 6974 666f  })..  >>> editfo
-000054c0: 726d 2e72 6571 7565 7374 203d 2072 6571  rm.request = req
-000054d0: 7565 7374 0a20 203e 3e3e 2065 7665 6e74  uest.  >>> event
-000054e0: 6c6f 673d 5b5d 0a20 203e 3e3e 2065 6469  log=[].  >>> edi
-000054f0: 7466 6f72 6d2e 7570 6461 7465 2829 0a0a  tform.update()..
-00005500: 4576 656e 746c 6f67 206d 7573 7420 6265  Eventlog must be
-00005510: 2063 6c65 616e 3a0a 0a20 203e 3e3e 206c   clean:..  >>> l
-00005520: 656e 2865 7665 6e74 6c6f 6729 0a20 2030  en(eventlog).  0
-00005530: 0a0a 5761 7463 6820 666f 7220 7468 6520  ..Watch for the 
-00005540: 6572 726f 7220 6d65 7373 6167 6520 696e  error message in
-00005550: 2074 6865 2048 544d 4c3a 0a69 7420 6861   the HTML:.it ha
-00005560: 7320 746f 2061 7070 6561 7220 6174 2074  s to appear at t
-00005570: 6865 2066 6965 6c64 2069 7473 656c 6620  he field itself 
-00005580: 616e 6420 6174 2074 6865 2074 6f70 206f  and at the top o
-00005590: 6620 7468 6520 666f 726d 3a0a 0a20 203e  f the form:..  >
-000055a0: 3e3e 2070 7269 6e74 2866 6f72 6d61 745f  >> print(format_
-000055b0: 6874 6d6c 2865 6469 7466 6f72 6d2e 7265  html(editform.re
-000055c0: 6e64 6572 2829 2929 0a20 203c 693e 5468  nder())).  <i>Th
-000055d0: 6572 6520 7765 7265 2073 6f6d 6520 6572  ere were some er
-000055e0: 726f 7273 2e3c 2f69 3e0a 2020 3c75 6c3e  rors.</i>.  <ul>
-000055f0: 0a20 2020 203c 6c69 3e0a 2020 2020 2020  .    <li>.      
-00005600: 2020 6d79 206f 626a 6563 740a 2020 2020    my object.    
-00005610: 2020 3c64 6976 2063 6c61 7373 3d22 6572    <div class="er
-00005620: 726f 7222 3e54 6865 2065 6e74 6572 6564  ror">The entered
-00005630: 2076 616c 7565 2069 7320 6e6f 7420 6120   value is not a 
-00005640: 7661 6c69 6420 696e 7465 6765 7220 6c69  valid integer li
-00005650: 7465 7261 6c2e 3c2f 6469 763e 0a20 2020  teral.</div>.   
-00005660: 203c 2f6c 693e 0a20 203c 2f75 6c3e 0a20   </li>.  </ul>. 
-00005670: 203c 666f 726d 2061 6374 696f 6e3d 222e   <form action=".
-00005680: 223e 0a20 2020 203c 6469 7620 636c 6173  ">.    <div clas
-00005690: 733d 2272 6f77 223e 0a20 2020 2020 203c  s="row">.      <
-000056a0: 623e 3c64 6976 2063 6c61 7373 3d22 6572  b><div class="er
-000056b0: 726f 7222 3e54 6865 2065 6e74 6572 6564  ror">The entered
-000056c0: 2076 616c 7565 2069 7320 6e6f 7420 6120   value is not a 
-000056d0: 7661 6c69 6420 696e 7465 6765 7220 6c69  valid integer li
-000056e0: 7465 7261 6c2e 3c2f 6469 763e 3c2f 623e  teral.</div></b>
-000056f0: 0a20 2020 2020 203c 6c61 6265 6c20 666f  .      <label fo
-00005700: 723d 2266 6f72 6d2d 7769 6467 6574 732d  r="form-widgets-
-00005710: 7375 626f 626a 6563 7422 3e6d 7920 6f62  subobject">my ob
-00005720: 6a65 6374 3c2f 6c61 6265 6c3e 0a20 2020  ject</label>.   
-00005730: 2020 203c 6469 7620 636c 6173 733d 226f     <div class="o
-00005740: 626a 6563 742d 7769 6467 6574 2072 6571  bject-widget req
-00005750: 7569 7265 6422 3e0a 2020 2020 2020 2020  uired">.        
-00005760: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00005770: 3d22 6c61 6265 6c22 3e0a 2020 2020 2020  ="label">.      
-00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005790: 3c6c 6162 656c 2066 6f72 3d22 666f 726d  <label for="form
-000057a0: 2d77 6964 6765 7473 2d73 7562 6f62 6a65  -widgets-subobje
-000057b0: 6374 2d77 6964 6765 7473 2d66 6f6f 6669  ct-widgets-foofi
-000057c0: 656c 6422 3e0a 2020 2020 2020 2020 2020  eld">.          
+00004c80: 2020 2020 2020 2020 2020 3c73 7061 6e3e            <span>
+00004c90: 4d79 2064 6561 7220 6261 723c 2f73 7061  My dear bar</spa
+00004ca0: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00004cb0: 2020 2020 2020 2020 203c 2f6c 6162 656c           </label
+00004cc0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004cd0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00004ce0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00004cf0: 2277 6964 6765 7422 3e0a 2020 2020 2020  "widget">.      
+00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d10: 3c69 6e70 7574 2074 7970 653d 2274 6578  <input type="tex
+00004d20: 7422 0a20 2020 2020 2020 2020 6964 3d22  t".         id="
+00004d30: 666f 726d 2d77 6964 6765 7473 2d73 7562  form-widgets-sub
+00004d40: 6f62 6a65 6374 2d77 6964 6765 7473 2d62  object-widgets-b
+00004d50: 6172 6669 656c 6422 0a20 2020 2020 2020  arfield".       
+00004d60: 2020 6e61 6d65 3d22 666f 726d 2e77 6964    name="form.wid
+00004d70: 6765 7473 2e73 7562 6f62 6a65 6374 2e77  gets.subobject.w
+00004d80: 6964 6765 7473 2e62 6172 6669 656c 6422  idgets.barfield"
+00004d90: 0a20 2020 2020 2020 2020 636c 6173 733d  .         class=
+00004da0: 2274 6578 742d 7769 6467 6574 2069 6e74  "text-widget int
+00004db0: 2d66 6965 6c64 220a 2020 2020 2020 2020  -field".        
+00004dc0: 2076 616c 7565 3d22 3535 2220 2f3e 0a20   value="55" />. 
+00004dd0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00004de0: 6976 3e0a 2020 2020 2020 3c69 6e70 7574  iv>.      <input
+00004df0: 206e 616d 653d 2266 6f72 6d2e 7769 6467   name="form.widg
+00004e00: 6574 732e 7375 626f 626a 6563 742d 656d  ets.subobject-em
+00004e10: 7074 792d 6d61 726b 6572 2220 7479 7065  pty-marker" type
+00004e20: 3d22 6869 6464 656e 2220 7661 6c75 653d  ="hidden" value=
+00004e30: 2231 2220 2f3e 0a20 203c 2f64 6976 3e0a  "1" />.  </div>.
+00004e40: 2020 2020 3c2f 6469 763e 0a20 2020 203c      </div>.    <
+00004e50: 6469 7620 636c 6173 733d 2272 6f77 223e  div class="row">
+00004e60: 0a20 2020 2020 203c 6c61 6265 6c20 666f  .      <label fo
+00004e70: 723d 2266 6f72 6d2d 7769 6467 6574 732d  r="form-widgets-
+00004e80: 6e61 6d65 223e 6e61 6d65 3c2f 6c61 6265  name">name</labe
+00004e90: 6c3e 0a20 2020 2020 203c 696e 7075 7420  l>.      <input 
+00004ea0: 7479 7065 3d22 7465 7874 220a 2020 2020  type="text".    
+00004eb0: 2020 2020 2069 643d 2266 6f72 6d2d 7769       id="form-wi
+00004ec0: 6467 6574 732d 6e61 6d65 220a 2020 2020  dgets-name".    
+00004ed0: 2020 2020 206e 616d 653d 2266 6f72 6d2e       name="form.
+00004ee0: 7769 6467 6574 732e 6e61 6d65 220a 2020  widgets.name".  
+00004ef0: 2020 2020 2020 2063 6c61 7373 3d22 7465         class="te
+00004f00: 7874 2d77 6964 6765 7420 7265 7175 6972  xt-widget requir
+00004f10: 6564 2074 6578 746c 696e 652d 6669 656c  ed textline-fiel
+00004f20: 6422 0a20 2020 2020 2020 2020 7661 6c75  d".         valu
+00004f30: 653d 2266 6972 7374 2220 2f3e 0a20 2020  e="first" />.   
+00004f40: 203c 2f64 6976 3e0a 2020 2020 3c64 6976   </div>.    <div
+00004f50: 2063 6c61 7373 3d22 6163 7469 6f6e 223e   class="action">
+00004f60: 0a20 2020 2020 203c 696e 7075 7420 7479  .      <input ty
+00004f70: 7065 3d22 7375 626d 6974 220a 2020 2020  pe="submit".    
+00004f80: 2020 2020 2069 643d 2266 6f72 6d2d 6275       id="form-bu
+00004f90: 7474 6f6e 732d 6170 706c 7922 0a20 2020  ttons-apply".   
+00004fa0: 2020 2020 2020 6e61 6d65 3d22 666f 726d        name="form
+00004fb0: 2e62 7574 746f 6e73 2e61 7070 6c79 220a  .buttons.apply".
+00004fc0: 2020 2020 2020 2020 2063 6c61 7373 3d22           class="
+00004fd0: 7375 626d 6974 2d77 6964 6765 7420 6275  submit-widget bu
+00004fe0: 7474 6f6e 2d66 6965 6c64 220a 2020 2020  tton-field".    
+00004ff0: 2020 2020 2076 616c 7565 3d22 4170 706c       value="Appl
+00005000: 7922 202f 3e0a 2020 2020 3c2f 6469 763e  y" />.    </div>
+00005010: 0a20 203c 2f66 6f72 6d3e 0a0a 4c65 7427  .  </form>..Let'
+00005020: 7320 7365 6520 6966 2074 6865 2077 6964  s see if the wid
+00005030: 6765 7420 6b65 6570 7320 7468 6520 6f6c  get keeps the ol
+00005040: 6420 6f62 6a65 6374 206f 6e20 6564 6974  d object on edit
+00005050: 696e 673a 0a0a 5765 2061 6464 2061 2073  ing:..We add a s
+00005060: 7065 6369 616c 2070 726f 7065 7274 7920  pecial property 
+00005070: 746f 206b 6565 7020 7472 6163 6b20 6f66  to keep track of
+00005080: 2074 6865 206f 626a 6563 743a 0a0a 2020   the object:..  
+00005090: 3e3e 3e20 726f 6f74 5b27 6669 7273 7427  >>> root['first'
+000050a0: 5d2e 5f5f 6d61 726b 6572 5f5f 203d 2022  ].__marker__ = "
+000050b0: 5468 6973 4d75 7374 5374 6179 5468 6553  ThisMustStayTheS
+000050c0: 616d 6522 0a0a 2020 3e3e 3e20 726f 6f74  ame"..  >>> root
+000050d0: 5b27 6669 7273 7427 5d2e 7375 626f 626a  ['first'].subobj
+000050e0: 6563 742e 666f 6f66 6965 6c64 0a20 2034  ect.foofield.  4
+000050f0: 330a 2020 3e3e 3e20 726f 6f74 5b27 6669  3.  >>> root['fi
+00005100: 7273 7427 5d2e 7375 626f 626a 6563 742e  rst'].subobject.
+00005110: 6261 7266 6965 6c64 0a20 2035 350a 0a4c  barfield.  55..L
+00005120: 6574 2773 206d 6f64 6966 7920 7468 6520  et's modify the 
+00005130: 7661 6c75 6573 3a0a 0a20 203e 3e3e 2072  values:..  >>> r
+00005140: 6571 7565 7374 203d 2054 6573 7452 6571  equest = TestReq
+00005150: 7565 7374 2870 6172 616d 733d 7b0a 2020  uest(params={.  
+00005160: 2e2e 2e20 2020 2020 2766 6f72 6d2e 7769  ...     'form.wi
+00005170: 6467 6574 732e 7375 626f 626a 6563 742e  dgets.subobject.
+00005180: 7769 6467 6574 732e 666f 6f66 6965 6c64  widgets.foofield
+00005190: 273a 2736 3636 272c 0a20 202e 2e2e 2020  ':'666',.  ...  
+000051a0: 2020 2027 666f 726d 2e77 6964 6765 7473     'form.widgets
+000051b0: 2e73 7562 6f62 6a65 6374 2e77 6964 6765  .subobject.widge
+000051c0: 7473 2e62 6172 6669 656c 6427 3a27 3939  ts.barfield':'99
+000051d0: 3927 2c0a 2020 2e2e 2e20 2020 2020 2766  9',.  ...     'f
+000051e0: 6f72 6d2e 7769 6467 6574 732e 6e61 6d65  orm.widgets.name
+000051f0: 273a 2766 6972 7374 272c 0a20 202e 2e2e  ':'first',.  ...
+00005200: 2020 2020 2027 666f 726d 2e77 6964 6765       'form.widge
+00005210: 7473 2e73 7562 6f62 6a65 6374 2d65 6d70  ts.subobject-emp
+00005220: 7479 2d6d 6172 6b65 7227 3a27 3127 2c0a  ty-marker':'1',.
+00005230: 2020 2e2e 2e20 2020 2020 2766 6f72 6d2e    ...     'form.
+00005240: 6275 7474 6f6e 732e 6170 706c 7927 3a27  buttons.apply':'
+00005250: 4170 706c 7927 7d29 0a0a 2020 3e3e 3e20  Apply'})..  >>> 
+00005260: 6564 6974 666f 726d 2e72 6571 7565 7374  editform.request
+00005270: 203d 2072 6571 7565 7374 0a0a 2020 3e3e   = request..  >>
+00005280: 3e20 6564 6974 666f 726d 2e75 7064 6174  > editform.updat
+00005290: 6528 290a 0a4c 6574 2773 2063 6865 636b  e()..Let's check
+000052a0: 2077 6861 7420 6172 6520 7468 6572 2065   what are ther e
+000052b0: 7375 6c74 7320 6f66 2074 6865 2075 7064  sults of the upd
+000052c0: 6174 653a 0a0a 2020 3e3e 3e20 726f 6f74  ate:..  >>> root
+000052d0: 5b27 6669 7273 7427 5d2e 7375 626f 626a  ['first'].subobj
+000052e0: 6563 742e 666f 6f66 6965 6c64 0a20 2036  ect.foofield.  6
+000052f0: 3636 0a20 203e 3e3e 2072 6f6f 745b 2766  66.  >>> root['f
+00005300: 6972 7374 275d 2e73 7562 6f62 6a65 6374  irst'].subobject
+00005310: 2e62 6172 6669 656c 640a 2020 3939 390a  .barfield.  999.
+00005320: 2020 3e3e 3e20 726f 6f74 5b27 6669 7273    >>> root['firs
+00005330: 7427 5d2e 5f5f 6d61 726b 6572 5f5f 0a20  t'].__marker__. 
+00005340: 2027 5468 6973 4d75 7374 5374 6179 5468   'ThisMustStayTh
+00005350: 6553 616d 6527 0a0a 0a4c 6574 2773 206d  eSame'...Let's m
+00005360: 616b 6520 6120 6e61 7374 7920 6572 726f  ake a nasty erro
+00005370: 722c 2062 7920 7479 7069 6e67 2027 6261  r, by typing 'ba
+00005380: 6427 2069 6e73 7465 6164 206f 6620 616e  d' instead of an
+00005390: 2069 6e74 6567 6572 3a0a 0a20 203e 3e3e   integer:..  >>>
+000053a0: 2072 6571 7565 7374 203d 2054 6573 7452   request = TestR
+000053b0: 6571 7565 7374 2870 6172 616d 733d 7b0a  equest(params={.
+000053c0: 2020 2e2e 2e20 2020 2020 2766 6f72 6d2e    ...     'form.
+000053d0: 7769 6467 6574 732e 7375 626f 626a 6563  widgets.subobjec
+000053e0: 742e 7769 6467 6574 732e 666f 6f66 6965  t.widgets.foofie
+000053f0: 6c64 273a 2739 3927 2c0a 2020 2e2e 2e20  ld':'99',.  ... 
+00005400: 2020 2020 2766 6f72 6d2e 7769 6467 6574      'form.widget
+00005410: 732e 7375 626f 626a 6563 742e 7769 6467  s.subobject.widg
+00005420: 6574 732e 6261 7266 6965 6c64 273a 2762  ets.barfield':'b
+00005430: 6164 272c 0a20 202e 2e2e 2020 2020 2027  ad',.  ...     '
+00005440: 666f 726d 2e77 6964 6765 7473 2e6e 616d  form.widgets.nam
+00005450: 6527 3a27 6669 7273 7427 2c0a 2020 2e2e  e':'first',.  ..
+00005460: 2e20 2020 2020 2766 6f72 6d2e 7769 6467  .     'form.widg
+00005470: 6574 732e 7375 626f 626a 6563 742d 656d  ets.subobject-em
+00005480: 7074 792d 6d61 726b 6572 273a 2731 272c  pty-marker':'1',
+00005490: 0a20 202e 2e2e 2020 2020 2027 666f 726d  .  ...     'form
+000054a0: 2e62 7574 746f 6e73 2e61 7070 6c79 273a  .buttons.apply':
+000054b0: 2741 7070 6c79 277d 290a 0a20 203e 3e3e  'Apply'})..  >>>
+000054c0: 2065 6469 7466 6f72 6d2e 7265 7175 6573   editform.reques
+000054d0: 7420 3d20 7265 7175 6573 740a 2020 3e3e  t = request.  >>
+000054e0: 3e20 6576 656e 746c 6f67 3d5b 5d0a 2020  > eventlog=[].  
+000054f0: 3e3e 3e20 6564 6974 666f 726d 2e75 7064  >>> editform.upd
+00005500: 6174 6528 290a 0a45 7665 6e74 6c6f 6720  ate()..Eventlog 
+00005510: 6d75 7374 2062 6520 636c 6561 6e3a 0a0a  must be clean:..
+00005520: 2020 3e3e 3e20 6c65 6e28 6576 656e 746c    >>> len(eventl
+00005530: 6f67 290a 2020 300a 0a57 6174 6368 2066  og).  0..Watch f
+00005540: 6f72 2074 6865 2065 7272 6f72 206d 6573  or the error mes
+00005550: 7361 6765 2069 6e20 7468 6520 4854 4d4c  sage in the HTML
+00005560: 3a0a 6974 2068 6173 2074 6f20 6170 7065  :.it has to appe
+00005570: 6172 2061 7420 7468 6520 6669 656c 6420  ar at the field 
+00005580: 6974 7365 6c66 2061 6e64 2061 7420 7468  itself and at th
+00005590: 6520 746f 7020 6f66 2074 6865 2066 6f72  e top of the for
+000055a0: 6d3a 0a0a 2020 3e3e 3e20 7072 696e 7428  m:..  >>> print(
+000055b0: 666f 726d 6174 5f68 746d 6c28 6564 6974  format_html(edit
+000055c0: 666f 726d 2e72 656e 6465 7228 2929 290a  form.render())).
+000055d0: 2020 3c69 3e54 6865 7265 2077 6572 6520    <i>There were 
+000055e0: 736f 6d65 2065 7272 6f72 732e 3c2f 693e  some errors.</i>
+000055f0: 0a20 203c 756c 3e0a 2020 2020 3c6c 693e  .  <ul>.    <li>
+00005600: 0a20 2020 2020 2020 206d 7920 6f62 6a65  .        my obje
+00005610: 6374 0a20 2020 2020 203c 6469 7620 636c  ct.      <div cl
+00005620: 6173 733d 2265 7272 6f72 223e 5468 6520  ass="error">The 
+00005630: 656e 7465 7265 6420 7661 6c75 6520 6973  entered value is
+00005640: 206e 6f74 2061 2076 616c 6964 2069 6e74   not a valid int
+00005650: 6567 6572 206c 6974 6572 616c 2e3c 2f64  eger literal.</d
+00005660: 6976 3e0a 2020 2020 3c2f 6c69 3e0a 2020  iv>.    </li>.  
+00005670: 3c2f 756c 3e0a 2020 3c66 6f72 6d20 6163  </ul>.  <form ac
+00005680: 7469 6f6e 3d22 2e22 3e0a 2020 2020 3c64  tion=".">.    <d
+00005690: 6976 2063 6c61 7373 3d22 726f 7722 3e0a  iv class="row">.
+000056a0: 2020 2020 2020 3c62 3e3c 6469 7620 636c        <b><div cl
+000056b0: 6173 733d 2265 7272 6f72 223e 5468 6520  ass="error">The 
+000056c0: 656e 7465 7265 6420 7661 6c75 6520 6973  entered value is
+000056d0: 206e 6f74 2061 2076 616c 6964 2069 6e74   not a valid int
+000056e0: 6567 6572 206c 6974 6572 616c 2e3c 2f64  eger literal.</d
+000056f0: 6976 3e3c 2f62 3e0a 2020 2020 2020 3c6c  iv></b>.      <l
+00005700: 6162 656c 2066 6f72 3d22 666f 726d 2d77  abel for="form-w
+00005710: 6964 6765 7473 2d73 7562 6f62 6a65 6374  idgets-subobject
+00005720: 223e 6d79 206f 626a 6563 743c 2f6c 6162  ">my object</lab
+00005730: 656c 3e0a 2020 2020 2020 3c64 6976 2063  el>.      <div c
+00005740: 6c61 7373 3d22 6f62 6a65 6374 2d77 6964  lass="object-wid
+00005750: 6765 7420 7265 7175 6972 6564 223e 0a20  get required">. 
+00005760: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00005770: 7620 636c 6173 733d 226c 6162 656c 223e  v class="label">
+00005780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005790: 2020 2020 2020 203c 6c61 6265 6c20 666f         <label fo
+000057a0: 723d 2266 6f72 6d2d 7769 6467 6574 732d  r="form-widgets-
+000057b0: 7375 626f 626a 6563 742d 7769 6467 6574  subobject-widget
+000057c0: 732d 666f 6f66 6965 6c64 223e 0a20 2020  s-foofield">.   
 000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057e0: 2020 2020 3c73 7061 6e3e 4d79 2066 6f6f      <span>My foo
-000057f0: 2066 6965 6c64 3c2f 7370 616e 3e0a 2020   field</span>.  
-00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005810: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
-00005820: 6e20 636c 6173 733d 2272 6571 7569 7265  n class="require
-00005830: 6422 3e2a 3c2f 7370 616e 3e0a 2020 2020  d">*</span>.    
-00005840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005850: 2020 3c2f 6c61 6265 6c3e 0a20 2020 2020    </label>.     
-00005860: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00005870: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00005880: 6976 2063 6c61 7373 3d22 7769 6467 6574  iv class="widget
-00005890: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000058a0: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-000058b0: 7479 7065 3d22 7465 7874 220a 2020 2020  type="text".    
-000058c0: 2020 2020 2069 643d 2266 6f72 6d2d 7769       id="form-wi
-000058d0: 6467 6574 732d 7375 626f 626a 6563 742d  dgets-subobject-
-000058e0: 7769 6467 6574 732d 666f 6f66 6965 6c64  widgets-foofield
-000058f0: 220a 2020 2020 2020 2020 206e 616d 653d  ".         name=
-00005900: 2266 6f72 6d2e 7769 6467 6574 732e 7375  "form.widgets.su
-00005910: 626f 626a 6563 742e 7769 6467 6574 732e  bobject.widgets.
-00005920: 666f 6f66 6965 6c64 220a 2020 2020 2020  foofield".      
-00005930: 2020 2063 6c61 7373 3d22 7465 7874 2d77     class="text-w
-00005940: 6964 6765 7420 7265 7175 6972 6564 2069  idget required i
-00005950: 6e74 2d66 6965 6c64 220a 2020 2020 2020  nt-field".      
-00005960: 2020 2076 616c 7565 3d22 3939 2220 2f3e     value="99" />
-00005970: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00005980: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00005990: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000059a0: 6c61 6265 6c22 3e0a 2020 2020 2020 2020  label">.        
-000059b0: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
-000059c0: 6162 656c 2066 6f72 3d22 666f 726d 2d77  abel for="form-w
-000059d0: 6964 6765 7473 2d73 7562 6f62 6a65 6374  idgets-subobject
-000059e0: 2d77 6964 6765 7473 2d62 6172 6669 656c  -widgets-barfiel
-000059f0: 6422 3e0a 2020 2020 2020 2020 2020 2020  d">.            
+000057e0: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+000057f0: 3e4d 7920 666f 6f20 6669 656c 643c 2f73  >My foo field</s
+00005800: 7061 6e3e 0a20 2020 2020 2020 2020 2020  pan>.           
+00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005820: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
+00005830: 7265 7175 6972 6564 223e 2a3c 2f73 7061  required">*</spa
+00005840: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00005850: 2020 2020 2020 2020 203c 2f6c 6162 656c           </label
+00005860: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005870: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00005880: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00005890: 2277 6964 6765 7422 3e0a 2020 2020 2020  "widget">.      
+000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058b0: 3c69 6e70 7574 2074 7970 653d 2274 6578  <input type="tex
+000058c0: 7422 0a20 2020 2020 2020 2020 6964 3d22  t".         id="
+000058d0: 666f 726d 2d77 6964 6765 7473 2d73 7562  form-widgets-sub
+000058e0: 6f62 6a65 6374 2d77 6964 6765 7473 2d66  object-widgets-f
+000058f0: 6f6f 6669 656c 6422 0a20 2020 2020 2020  oofield".       
+00005900: 2020 6e61 6d65 3d22 666f 726d 2e77 6964    name="form.wid
+00005910: 6765 7473 2e73 7562 6f62 6a65 6374 2e77  gets.subobject.w
+00005920: 6964 6765 7473 2e66 6f6f 6669 656c 6422  idgets.foofield"
+00005930: 0a20 2020 2020 2020 2020 636c 6173 733d  .         class=
+00005940: 2274 6578 742d 7769 6467 6574 2072 6571  "text-widget req
+00005950: 7569 7265 6420 696e 742d 6669 656c 6422  uired int-field"
+00005960: 0a20 2020 2020 2020 2020 7661 6c75 653d  .         value=
+00005970: 2239 3922 202f 3e0a 2020 2020 2020 2020  "99" />.        
+00005980: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00005990: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000059a0: 636c 6173 733d 226c 6162 656c 223e 0a20  class="label">. 
+000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059c0: 2020 2020 203c 6c61 6265 6c20 666f 723d       <label for=
+000059d0: 2266 6f72 6d2d 7769 6467 6574 732d 7375  "form-widgets-su
+000059e0: 626f 626a 6563 742d 7769 6467 6574 732d  bobject-widgets-
+000059f0: 6261 7266 6965 6c64 223e 0a20 2020 2020  barfield">.     
 00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 2020 3c73 7061 6e3e 4d79 2064 6561 7220    <span>My dear 
-00005a20: 6261 723c 2f73 7061 6e3e 0a20 2020 2020  bar</span>.     
-00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a40: 203c 2f6c 6162 656c 3e0a 2020 2020 2020   </label>.      
-00005a50: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00005a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a70: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00005a80: 2265 7272 6f72 223e 5468 6520 656e 7465  "error">The ente
-00005a90: 7265 6420 7661 6c75 6520 6973 206e 6f74  red value is not
-00005aa0: 2061 2076 616c 6964 2069 6e74 6567 6572   a valid integer
-00005ab0: 206c 6974 6572 616c 2e3c 2f64 6976 3e0a   literal.</div>.
-00005ac0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00005ad0: 6976 2063 6c61 7373 3d22 7769 6467 6574  iv class="widget
-00005ae0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00005af0: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-00005b00: 7479 7065 3d22 7465 7874 220a 2020 2020  type="text".    
-00005b10: 2020 2020 2069 643d 2266 6f72 6d2d 7769       id="form-wi
-00005b20: 6467 6574 732d 7375 626f 626a 6563 742d  dgets-subobject-
-00005b30: 7769 6467 6574 732d 6261 7266 6965 6c64  widgets-barfield
-00005b40: 220a 2020 2020 2020 2020 206e 616d 653d  ".         name=
-00005b50: 2266 6f72 6d2e 7769 6467 6574 732e 7375  "form.widgets.su
-00005b60: 626f 626a 6563 742e 7769 6467 6574 732e  bobject.widgets.
-00005b70: 6261 7266 6965 6c64 220a 2020 2020 2020  barfield".      
-00005b80: 2020 2063 6c61 7373 3d22 7465 7874 2d77     class="text-w
-00005b90: 6964 6765 7420 696e 742d 6669 656c 6422  idget int-field"
-00005ba0: 0a20 2020 2020 2020 2020 7661 6c75 653d  .         value=
-00005bb0: 2262 6164 2220 2f3e 0a20 2020 2020 2020  "bad" />.       
-00005bc0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00005bd0: 2020 2020 3c69 6e70 7574 206e 616d 653d      <input name=
-00005be0: 2266 6f72 6d2e 7769 6467 6574 732e 7375  "form.widgets.su
-00005bf0: 626f 626a 6563 742d 656d 7074 792d 6d61  bobject-empty-ma
-00005c00: 726b 6572 2220 7479 7065 3d22 6869 6464  rker" type="hidd
-00005c10: 656e 2220 7661 6c75 653d 2231 222f 3e0a  en" value="1"/>.
-00005c20: 2020 3c2f 6469 763e 0a20 2020 203c 2f64    </div>.    </d
-00005c30: 6976 3e0a 2020 2020 3c64 6976 2063 6c61  iv>.    <div cla
-00005c40: 7373 3d22 726f 7722 3e0a 2020 2020 2020  ss="row">.      
-00005c50: 3c6c 6162 656c 2066 6f72 3d22 666f 726d  <label for="form
-00005c60: 2d77 6964 6765 7473 2d6e 616d 6522 3e6e  -widgets-name">n
-00005c70: 616d 653c 2f6c 6162 656c 3e0a 2020 2020  ame</label>.    
-00005c80: 2020 3c69 6e70 7574 2074 7970 653d 2274    <input type="t
-00005c90: 6578 7422 0a20 2020 2020 2020 2020 6964  ext".         id
-00005ca0: 3d22 666f 726d 2d77 6964 6765 7473 2d6e  ="form-widgets-n
-00005cb0: 616d 6522 0a20 2020 2020 2020 2020 6e61  ame".         na
-00005cc0: 6d65 3d22 666f 726d 2e77 6964 6765 7473  me="form.widgets
-00005cd0: 2e6e 616d 6522 0a20 2020 2020 2020 2020  .name".         
-00005ce0: 636c 6173 733d 2274 6578 742d 7769 6467  class="text-widg
-00005cf0: 6574 2072 6571 7569 7265 6420 7465 7874  et required text
-00005d00: 6c69 6e65 2d66 6965 6c64 220a 2020 2020  line-field".    
-00005d10: 2020 2020 2076 616c 7565 3d22 6669 7273       value="firs
-00005d20: 7422 202f 3e0a 2020 2020 3c2f 6469 763e  t" />.    </div>
-00005d30: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
-00005d40: 2261 6374 696f 6e22 3e0a 2020 2020 2020  "action">.      
-00005d50: 3c69 6e70 7574 2074 7970 653d 2273 7562  <input type="sub
-00005d60: 6d69 7422 0a20 2020 2020 2020 2020 6964  mit".         id
-00005d70: 3d22 666f 726d 2d62 7574 746f 6e73 2d61  ="form-buttons-a
-00005d80: 7070 6c79 220a 2020 2020 2020 2020 206e  pply".         n
-00005d90: 616d 653d 2266 6f72 6d2e 6275 7474 6f6e  ame="form.button
-00005da0: 732e 6170 706c 7922 0a20 2020 2020 2020  s.apply".       
-00005db0: 2020 636c 6173 733d 2273 7562 6d69 742d    class="submit-
-00005dc0: 7769 6467 6574 2062 7574 746f 6e2d 6669  widget button-fi
-00005dd0: 656c 6422 0a20 2020 2020 2020 2020 7661  eld".         va
-00005de0: 6c75 653d 2241 7070 6c79 2220 2f3e 0a20  lue="Apply" />. 
-00005df0: 2020 203c 2f64 6976 3e0a 2020 3c2f 666f     </div>.  </fo
-00005e00: 726d 3e0a 0a54 6865 206f 626a 6563 7420  rm>..The object 
-00005e10: 7661 6c75 6573 206d 7573 7420 7374 6179  values must stay
-00005e20: 2061 7420 7468 6520 6f6c 6420 6f6e 6573   at the old ones
-00005e30: 3a0a 0a20 203e 3e3e 2072 6f6f 745b 2766  :..  >>> root['f
-00005e40: 6972 7374 275d 2e73 7562 6f62 6a65 6374  irst'].subobject
-00005e50: 2e66 6f6f 6669 656c 640a 2020 3636 360a  .foofield.  666.
-00005e60: 2020 3e3e 3e20 726f 6f74 5b27 6669 7273    >>> root['firs
-00005e70: 7427 5d2e 7375 626f 626a 6563 742e 6261  t'].subobject.ba
-00005e80: 7266 6965 6c64 0a20 2039 3939 0a0a 4c65  rfield.  999..Le
-00005e90: 7427 7320 6d61 6b65 206d 6f72 6520 6572  t's make more er
-00005ea0: 726f 7273 3a0a 4e6f 7720 7765 2065 6e74  rors:.Now we ent
-00005eb0: 6572 2027 6261 6427 2061 6e64 2027 3939  er 'bad' and '99
-00005ec0: 3939 3939 272c 2077 6865 7265 2027 3939  9999', where '99
-00005ed0: 3939 3939 2720 6869 7473 2074 6865 2075  9999' hits the u
-00005ee0: 7070 6572 206c 696d 6974 206f 6620 7468  pper limit of th
-00005ef0: 6520 6669 656c 642e 0a0a 2020 3e3e 3e20  e field...  >>> 
-00005f00: 7265 7175 6573 7420 3d20 5465 7374 5265  request = TestRe
-00005f10: 7175 6573 7428 7061 7261 6d73 3d7b 0a20  quest(params={. 
-00005f20: 202e 2e2e 2020 2020 2027 666f 726d 2e77   ...     'form.w
-00005f30: 6964 6765 7473 2e73 7562 6f62 6a65 6374  idgets.subobject
-00005f40: 2e77 6964 6765 7473 2e66 6f6f 6669 656c  .widgets.foofiel
-00005f50: 6427 3a27 3939 3939 3939 272c 0a20 202e  d':'999999',.  .
-00005f60: 2e2e 2020 2020 2027 666f 726d 2e77 6964  ..     'form.wid
-00005f70: 6765 7473 2e73 7562 6f62 6a65 6374 2e77  gets.subobject.w
-00005f80: 6964 6765 7473 2e62 6172 6669 656c 6427  idgets.barfield'
-00005f90: 3a27 6261 6427 2c0a 2020 2e2e 2e20 2020  :'bad',.  ...   
-00005fa0: 2020 2766 6f72 6d2e 7769 6467 6574 732e    'form.widgets.
-00005fb0: 6e61 6d65 273a 2766 6972 7374 272c 0a20  name':'first',. 
-00005fc0: 202e 2e2e 2020 2020 2027 666f 726d 2e77   ...     'form.w
-00005fd0: 6964 6765 7473 2e73 7562 6f62 6a65 6374  idgets.subobject
-00005fe0: 2d65 6d70 7479 2d6d 6172 6b65 7227 3a27  -empty-marker':'
-00005ff0: 3127 2c0a 2020 2e2e 2e20 2020 2020 2766  1',.  ...     'f
-00006000: 6f72 6d2e 6275 7474 6f6e 732e 6170 706c  orm.buttons.appl
-00006010: 7927 3a27 4170 706c 7927 7d29 0a0a 2020  y':'Apply'})..  
-00006020: 3e3e 3e20 6564 6974 666f 726d 2e72 6571  >>> editform.req
-00006030: 7565 7374 203d 2072 6571 7565 7374 0a20  uest = request. 
-00006040: 203e 3e3e 2065 6469 7466 6f72 6d2e 7570   >>> editform.up
-00006050: 6461 7465 2829 0a0a 426f 7468 2065 7272  date()..Both err
-00006060: 6f72 7320 6d75 7374 2061 7070 6561 7220  ors must appear 
-00006070: 6174 2074 6865 2074 6f70 206f 6620 7468  at the top of th
-00006080: 6520 666f 726d 3a0a 0a20 203e 3e3e 2070  e form:..  >>> p
-00006090: 7269 6e74 2866 6f72 6d61 745f 6874 6d6c  rint(format_html
-000060a0: 2865 6469 7466 6f72 6d2e 7265 6e64 6572  (editform.render
-000060b0: 2829 2929 0a20 203c 693e 5468 6572 6520  ())).  <i>There 
-000060c0: 7765 7265 2073 6f6d 6520 6572 726f 7273  were some errors
-000060d0: 2e3c 2f69 3e0a 2020 3c75 6c3e 0a20 2020  .</i>.  <ul>.   
-000060e0: 203c 6c69 3e0a 2020 2020 2020 2020 6d79   <li>.        my
-000060f0: 206f 626a 6563 740a 2020 2020 2020 3c64   object.      <d
-00006100: 6976 2063 6c61 7373 3d22 6572 726f 7222  iv class="error"
-00006110: 3e56 616c 7565 2069 7320 746f 6f20 6269  >Value is too bi
-00006120: 673c 2f64 6976 3e3c 6469 7620 636c 6173  g</div><div clas
-00006130: 733d 2265 7272 6f72 223e 5468 6520 656e  s="error">The en
-00006140: 7465 7265 6420 7661 6c75 6520 6973 206e  tered value is n
-00006150: 6f74 2061 2076 616c 6964 2069 6e74 6567  ot a valid integ
-00006160: 6572 206c 6974 6572 616c 2e3c 2f64 6976  er literal.</div
-00006170: 3e0a 2020 2020 3c2f 6c69 3e0a 2020 3c2f  >.    </li>.  </
-00006180: 756c 3e0a 2020 3c66 6f72 6d20 6163 7469  ul>.  <form acti
-00006190: 6f6e 3d22 2e22 3e0a 2020 2020 3c64 6976  on=".">.    <div
-000061a0: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
-000061b0: 2020 2020 3c62 3e3c 6469 7620 636c 6173      <b><div clas
-000061c0: 733d 2265 7272 6f72 223e 5661 6c75 6520  s="error">Value 
-000061d0: 6973 2074 6f6f 2062 6967 3c2f 6469 763e  is too big</div>
-000061e0: 3c64 6976 2063 6c61 7373 3d22 6572 726f  <div class="erro
-000061f0: 7222 3e54 6865 2065 6e74 6572 6564 2076  r">The entered v
-00006200: 616c 7565 2069 7320 6e6f 7420 6120 7661  alue is not a va
-00006210: 6c69 6420 696e 7465 6765 7220 6c69 7465  lid integer lite
-00006220: 7261 6c2e 3c2f 6469 763e 3c2f 623e 0a20  ral.</div></b>. 
-00006230: 2020 2020 203c 6c61 6265 6c20 666f 723d       <label for=
-00006240: 2266 6f72 6d2d 7769 6467 6574 732d 7375  "form-widgets-su
-00006250: 626f 626a 6563 7422 3e6d 7920 6f62 6a65  bobject">my obje
-00006260: 6374 3c2f 6c61 6265 6c3e 0a20 2020 2020  ct</label>.     
-00006270: 203c 6469 7620 636c 6173 733d 226f 626a   <div class="obj
-00006280: 6563 742d 7769 6467 6574 2072 6571 7569  ect-widget requi
-00006290: 7265 6422 3e0a 2020 2020 2020 2020 2020  red">.          
-000062a0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000062b0: 6c61 6265 6c22 3e0a 2020 2020 2020 2020  label">.        
-000062c0: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
-000062d0: 6162 656c 2066 6f72 3d22 666f 726d 2d77  abel for="form-w
-000062e0: 6964 6765 7473 2d73 7562 6f62 6a65 6374  idgets-subobject
-000062f0: 2d77 6964 6765 7473 2d66 6f6f 6669 656c  -widgets-foofiel
-00006300: 6422 3e0a 2020 2020 2020 2020 2020 2020  d">.            
+00005a10: 2020 2020 2020 2020 203c 7370 616e 3e4d           <span>M
+00005a20: 7920 6465 6172 2062 6172 3c2f 7370 616e  y dear bar</span
+00005a30: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005a40: 2020 2020 2020 2020 3c2f 6c61 6265 6c3e          </label>
+00005a50: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00005a60: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00005a70: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00005a80: 2063 6c61 7373 3d22 6572 726f 7222 3e54   class="error">T
+00005a90: 6865 2065 6e74 6572 6564 2076 616c 7565  he entered value
+00005aa0: 2069 7320 6e6f 7420 6120 7661 6c69 6420   is not a valid 
+00005ab0: 696e 7465 6765 7220 6c69 7465 7261 6c2e  integer literal.
+00005ac0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00005ad0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00005ae0: 2277 6964 6765 7422 3e0a 2020 2020 2020  "widget">.      
+00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b00: 3c69 6e70 7574 2074 7970 653d 2274 6578  <input type="tex
+00005b10: 7422 0a20 2020 2020 2020 2020 6964 3d22  t".         id="
+00005b20: 666f 726d 2d77 6964 6765 7473 2d73 7562  form-widgets-sub
+00005b30: 6f62 6a65 6374 2d77 6964 6765 7473 2d62  object-widgets-b
+00005b40: 6172 6669 656c 6422 0a20 2020 2020 2020  arfield".       
+00005b50: 2020 6e61 6d65 3d22 666f 726d 2e77 6964    name="form.wid
+00005b60: 6765 7473 2e73 7562 6f62 6a65 6374 2e77  gets.subobject.w
+00005b70: 6964 6765 7473 2e62 6172 6669 656c 6422  idgets.barfield"
+00005b80: 0a20 2020 2020 2020 2020 636c 6173 733d  .         class=
+00005b90: 2274 6578 742d 7769 6467 6574 2069 6e74  "text-widget int
+00005ba0: 2d66 6965 6c64 220a 2020 2020 2020 2020  -field".        
+00005bb0: 2076 616c 7565 3d22 6261 6422 202f 3e0a   value="bad" />.
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00005bd0: 6469 763e 0a20 2020 2020 203c 696e 7075  div>.      <inpu
+00005be0: 7420 6e61 6d65 3d22 666f 726d 2e77 6964  t name="form.wid
+00005bf0: 6765 7473 2e73 7562 6f62 6a65 6374 2d65  gets.subobject-e
+00005c00: 6d70 7479 2d6d 6172 6b65 7222 2074 7970  mpty-marker" typ
+00005c10: 653d 2268 6964 6465 6e22 2076 616c 7565  e="hidden" value
+00005c20: 3d22 3122 202f 3e0a 2020 3c2f 6469 763e  ="1" />.  </div>
+00005c30: 0a20 2020 203c 2f64 6976 3e0a 2020 2020  .    </div>.    
+00005c40: 3c64 6976 2063 6c61 7373 3d22 726f 7722  <div class="row"
+00005c50: 3e0a 2020 2020 2020 3c6c 6162 656c 2066  >.      <label f
+00005c60: 6f72 3d22 666f 726d 2d77 6964 6765 7473  or="form-widgets
+00005c70: 2d6e 616d 6522 3e6e 616d 653c 2f6c 6162  -name">name</lab
+00005c80: 656c 3e0a 2020 2020 2020 3c69 6e70 7574  el>.      <input
+00005c90: 2074 7970 653d 2274 6578 7422 0a20 2020   type="text".   
+00005ca0: 2020 2020 2020 6964 3d22 666f 726d 2d77        id="form-w
+00005cb0: 6964 6765 7473 2d6e 616d 6522 0a20 2020  idgets-name".   
+00005cc0: 2020 2020 2020 6e61 6d65 3d22 666f 726d        name="form
+00005cd0: 2e77 6964 6765 7473 2e6e 616d 6522 0a20  .widgets.name". 
+00005ce0: 2020 2020 2020 2020 636c 6173 733d 2274          class="t
+00005cf0: 6578 742d 7769 6467 6574 2072 6571 7569  ext-widget requi
+00005d00: 7265 6420 7465 7874 6c69 6e65 2d66 6965  red textline-fie
+00005d10: 6c64 220a 2020 2020 2020 2020 2076 616c  ld".         val
+00005d20: 7565 3d22 6669 7273 7422 202f 3e0a 2020  ue="first" />.  
+00005d30: 2020 3c2f 6469 763e 0a20 2020 203c 6469    </div>.    <di
+00005d40: 7620 636c 6173 733d 2261 6374 696f 6e22  v class="action"
+00005d50: 3e0a 2020 2020 2020 3c69 6e70 7574 2074  >.      <input t
+00005d60: 7970 653d 2273 7562 6d69 7422 0a20 2020  ype="submit".   
+00005d70: 2020 2020 2020 6964 3d22 666f 726d 2d62        id="form-b
+00005d80: 7574 746f 6e73 2d61 7070 6c79 220a 2020  uttons-apply".  
+00005d90: 2020 2020 2020 206e 616d 653d 2266 6f72         name="for
+00005da0: 6d2e 6275 7474 6f6e 732e 6170 706c 7922  m.buttons.apply"
+00005db0: 0a20 2020 2020 2020 2020 636c 6173 733d  .         class=
+00005dc0: 2273 7562 6d69 742d 7769 6467 6574 2062  "submit-widget b
+00005dd0: 7574 746f 6e2d 6669 656c 6422 0a20 2020  utton-field".   
+00005de0: 2020 2020 2020 7661 6c75 653d 2241 7070        value="App
+00005df0: 6c79 2220 2f3e 0a20 2020 203c 2f64 6976  ly" />.    </div
+00005e00: 3e0a 2020 3c2f 666f 726d 3e0a 0a54 6865  >.  </form>..The
+00005e10: 206f 626a 6563 7420 7661 6c75 6573 206d   object values m
+00005e20: 7573 7420 7374 6179 2061 7420 7468 6520  ust stay at the 
+00005e30: 6f6c 6420 6f6e 6573 3a0a 0a20 203e 3e3e  old ones:..  >>>
+00005e40: 2072 6f6f 745b 2766 6972 7374 275d 2e73   root['first'].s
+00005e50: 7562 6f62 6a65 6374 2e66 6f6f 6669 656c  ubobject.foofiel
+00005e60: 640a 2020 3636 360a 2020 3e3e 3e20 726f  d.  666.  >>> ro
+00005e70: 6f74 5b27 6669 7273 7427 5d2e 7375 626f  ot['first'].subo
+00005e80: 626a 6563 742e 6261 7266 6965 6c64 0a20  bject.barfield. 
+00005e90: 2039 3939 0a0a 4c65 7427 7320 6d61 6b65   999..Let's make
+00005ea0: 206d 6f72 6520 6572 726f 7273 3a0a 4e6f   more errors:.No
+00005eb0: 7720 7765 2065 6e74 6572 2027 6261 6427  w we enter 'bad'
+00005ec0: 2061 6e64 2027 3939 3939 3939 272c 2077   and '999999', w
+00005ed0: 6865 7265 2027 3939 3939 3939 2720 6869  here '999999' hi
+00005ee0: 7473 2074 6865 2075 7070 6572 206c 696d  ts the upper lim
+00005ef0: 6974 206f 6620 7468 6520 6669 656c 642e  it of the field.
+00005f00: 0a0a 2020 3e3e 3e20 7265 7175 6573 7420  ..  >>> request 
+00005f10: 3d20 5465 7374 5265 7175 6573 7428 7061  = TestRequest(pa
+00005f20: 7261 6d73 3d7b 0a20 202e 2e2e 2020 2020  rams={.  ...    
+00005f30: 2027 666f 726d 2e77 6964 6765 7473 2e73   'form.widgets.s
+00005f40: 7562 6f62 6a65 6374 2e77 6964 6765 7473  ubobject.widgets
+00005f50: 2e66 6f6f 6669 656c 6427 3a27 3939 3939  .foofield':'9999
+00005f60: 3939 272c 0a20 202e 2e2e 2020 2020 2027  99',.  ...     '
+00005f70: 666f 726d 2e77 6964 6765 7473 2e73 7562  form.widgets.sub
+00005f80: 6f62 6a65 6374 2e77 6964 6765 7473 2e62  object.widgets.b
+00005f90: 6172 6669 656c 6427 3a27 6261 6427 2c0a  arfield':'bad',.
+00005fa0: 2020 2e2e 2e20 2020 2020 2766 6f72 6d2e    ...     'form.
+00005fb0: 7769 6467 6574 732e 6e61 6d65 273a 2766  widgets.name':'f
+00005fc0: 6972 7374 272c 0a20 202e 2e2e 2020 2020  irst',.  ...    
+00005fd0: 2027 666f 726d 2e77 6964 6765 7473 2e73   'form.widgets.s
+00005fe0: 7562 6f62 6a65 6374 2d65 6d70 7479 2d6d  ubobject-empty-m
+00005ff0: 6172 6b65 7227 3a27 3127 2c0a 2020 2e2e  arker':'1',.  ..
+00006000: 2e20 2020 2020 2766 6f72 6d2e 6275 7474  .     'form.butt
+00006010: 6f6e 732e 6170 706c 7927 3a27 4170 706c  ons.apply':'Appl
+00006020: 7927 7d29 0a0a 2020 3e3e 3e20 6564 6974  y'})..  >>> edit
+00006030: 666f 726d 2e72 6571 7565 7374 203d 2072  form.request = r
+00006040: 6571 7565 7374 0a20 203e 3e3e 2065 6469  equest.  >>> edi
+00006050: 7466 6f72 6d2e 7570 6461 7465 2829 0a0a  tform.update()..
+00006060: 426f 7468 2065 7272 6f72 7320 6d75 7374  Both errors must
+00006070: 2061 7070 6561 7220 6174 2074 6865 2074   appear at the t
+00006080: 6f70 206f 6620 7468 6520 666f 726d 3a0a  op of the form:.
+00006090: 0a20 203e 3e3e 2070 7269 6e74 2866 6f72  .  >>> print(for
+000060a0: 6d61 745f 6874 6d6c 2865 6469 7466 6f72  mat_html(editfor
+000060b0: 6d2e 7265 6e64 6572 2829 2929 0a20 203c  m.render())).  <
+000060c0: 693e 5468 6572 6520 7765 7265 2073 6f6d  i>There were som
+000060d0: 6520 6572 726f 7273 2e3c 2f69 3e0a 2020  e errors.</i>.  
+000060e0: 3c75 6c3e 0a20 2020 203c 6c69 3e0a 2020  <ul>.    <li>.  
+000060f0: 2020 2020 2020 6d79 206f 626a 6563 740a        my object.
+00006100: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00006110: 3d22 6572 726f 7222 3e56 616c 7565 2069  ="error">Value i
+00006120: 7320 746f 6f20 6269 673c 2f64 6976 3e3c  s too big</div><
+00006130: 6469 7620 636c 6173 733d 2265 7272 6f72  div class="error
+00006140: 223e 5468 6520 656e 7465 7265 6420 7661  ">The entered va
+00006150: 6c75 6520 6973 206e 6f74 2061 2076 616c  lue is not a val
+00006160: 6964 2069 6e74 6567 6572 206c 6974 6572  id integer liter
+00006170: 616c 2e3c 2f64 6976 3e0a 2020 2020 3c2f  al.</div>.    </
+00006180: 6c69 3e0a 2020 3c2f 756c 3e0a 2020 3c66  li>.  </ul>.  <f
+00006190: 6f72 6d20 6163 7469 6f6e 3d22 2e22 3e0a  orm action=".">.
+000061a0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000061b0: 726f 7722 3e0a 2020 2020 2020 3c62 3e3c  row">.      <b><
+000061c0: 6469 7620 636c 6173 733d 2265 7272 6f72  div class="error
+000061d0: 223e 5661 6c75 6520 6973 2074 6f6f 2062  ">Value is too b
+000061e0: 6967 3c2f 6469 763e 3c64 6976 2063 6c61  ig</div><div cla
+000061f0: 7373 3d22 6572 726f 7222 3e54 6865 2065  ss="error">The e
+00006200: 6e74 6572 6564 2076 616c 7565 2069 7320  ntered value is 
+00006210: 6e6f 7420 6120 7661 6c69 6420 696e 7465  not a valid inte
+00006220: 6765 7220 6c69 7465 7261 6c2e 3c2f 6469  ger literal.</di
+00006230: 763e 3c2f 623e 0a20 2020 2020 203c 6c61  v></b>.      <la
+00006240: 6265 6c20 666f 723d 2266 6f72 6d2d 7769  bel for="form-wi
+00006250: 6467 6574 732d 7375 626f 626a 6563 7422  dgets-subobject"
+00006260: 3e6d 7920 6f62 6a65 6374 3c2f 6c61 6265  >my object</labe
+00006270: 6c3e 0a20 2020 2020 203c 6469 7620 636c  l>.      <div cl
+00006280: 6173 733d 226f 626a 6563 742d 7769 6467  ass="object-widg
+00006290: 6574 2072 6571 7569 7265 6422 3e0a 2020  et required">.  
+000062a0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000062b0: 2063 6c61 7373 3d22 6c61 6265 6c22 3e0a   class="label">.
+000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062d0: 2020 2020 2020 3c6c 6162 656c 2066 6f72        <label for
+000062e0: 3d22 666f 726d 2d77 6964 6765 7473 2d73  ="form-widgets-s
+000062f0: 7562 6f62 6a65 6374 2d77 6964 6765 7473  ubobject-widgets
+00006300: 2d66 6f6f 6669 656c 6422 3e0a 2020 2020  -foofield">.    
 00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006320: 2020 3c73 7061 6e3e 4d79 2066 6f6f 2066    <span>My foo f
-00006330: 6965 6c64 3c2f 7370 616e 3e0a 2020 2020  ield</span>.    
-00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006350: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
-00006360: 636c 6173 733d 2272 6571 7569 7265 6422  class="required"
-00006370: 3e2a 3c2f 7370 616e 3e0a 2020 2020 2020  >*</span>.      
-00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006390: 3c2f 6c61 6265 6c3e 0a20 2020 2020 2020  </label>.       
-000063a0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063c0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000063d0: 6572 726f 7222 3e56 616c 7565 2069 7320  error">Value is 
-000063e0: 746f 6f20 6269 673c 2f64 6976 3e0a 2020  too big</div>.  
-000063f0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00006400: 2063 6c61 7373 3d22 7769 6467 6574 223e   class="widget">
-00006410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006420: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
-00006430: 7065 3d22 7465 7874 220a 2020 2020 2020  pe="text".      
-00006440: 2020 2069 643d 2266 6f72 6d2d 7769 6467     id="form-widg
-00006450: 6574 732d 7375 626f 626a 6563 742d 7769  ets-subobject-wi
-00006460: 6467 6574 732d 666f 6f66 6965 6c64 220a  dgets-foofield".
-00006470: 2020 2020 2020 2020 206e 616d 653d 2266           name="f
-00006480: 6f72 6d2e 7769 6467 6574 732e 7375 626f  orm.widgets.subo
-00006490: 626a 6563 742e 7769 6467 6574 732e 666f  bject.widgets.fo
-000064a0: 6f66 6965 6c64 220a 2020 2020 2020 2020  ofield".        
-000064b0: 2063 6c61 7373 3d22 7465 7874 2d77 6964   class="text-wid
-000064c0: 6765 7420 7265 7175 6972 6564 2069 6e74  get required int
-000064d0: 2d66 6965 6c64 220a 2020 2020 2020 2020  -field".        
-000064e0: 2076 616c 7565 3d22 3939 3939 3939 2220   value="999999" 
-000064f0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00006500: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00006510: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00006520: 3d22 6c61 6265 6c22 3e0a 2020 2020 2020  ="label">.      
-00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006540: 3c6c 6162 656c 2066 6f72 3d22 666f 726d  <label for="form
-00006550: 2d77 6964 6765 7473 2d73 7562 6f62 6a65  -widgets-subobje
-00006560: 6374 2d77 6964 6765 7473 2d62 6172 6669  ct-widgets-barfi
-00006570: 656c 6422 3e0a 2020 2020 2020 2020 2020  eld">.          
+00006320: 2020 2020 2020 2020 2020 3c73 7061 6e3e            <span>
+00006330: 4d79 2066 6f6f 2066 6965 6c64 3c2f 7370  My foo field</sp
+00006340: 616e 3e0a 2020 2020 2020 2020 2020 2020  an>.            
+00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006360: 2020 3c73 7061 6e20 636c 6173 733d 2272    <span class="r
+00006370: 6571 7569 7265 6422 3e2a 3c2f 7370 616e  equired">*</span
+00006380: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006390: 2020 2020 2020 2020 3c2f 6c61 6265 6c3e          </label>
+000063a0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+000063b0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+000063c0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000063d0: 2063 6c61 7373 3d22 6572 726f 7222 3e56   class="error">V
+000063e0: 616c 7565 2069 7320 746f 6f20 6269 673c  alue is too big<
+000063f0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00006400: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00006410: 7769 6467 6574 223e 0a20 2020 2020 2020  widget">.       
+00006420: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006430: 696e 7075 7420 7479 7065 3d22 7465 7874  input type="text
+00006440: 220a 2020 2020 2020 2020 2069 643d 2266  ".         id="f
+00006450: 6f72 6d2d 7769 6467 6574 732d 7375 626f  orm-widgets-subo
+00006460: 626a 6563 742d 7769 6467 6574 732d 666f  bject-widgets-fo
+00006470: 6f66 6965 6c64 220a 2020 2020 2020 2020  ofield".        
+00006480: 206e 616d 653d 2266 6f72 6d2e 7769 6467   name="form.widg
+00006490: 6574 732e 7375 626f 626a 6563 742e 7769  ets.subobject.wi
+000064a0: 6467 6574 732e 666f 6f66 6965 6c64 220a  dgets.foofield".
+000064b0: 2020 2020 2020 2020 2063 6c61 7373 3d22           class="
+000064c0: 7465 7874 2d77 6964 6765 7420 7265 7175  text-widget requ
+000064d0: 6972 6564 2069 6e74 2d66 6965 6c64 220a  ired int-field".
+000064e0: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
+000064f0: 3939 3939 3939 2220 2f3e 0a20 2020 2020  999999" />.     
+00006500: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00006510: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00006520: 6976 2063 6c61 7373 3d22 6c61 6265 6c22  iv class="label"
+00006530: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006540: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
+00006550: 6f72 3d22 666f 726d 2d77 6964 6765 7473  or="form-widgets
+00006560: 2d73 7562 6f62 6a65 6374 2d77 6964 6765  -subobject-widge
+00006570: 7473 2d62 6172 6669 656c 6422 3e0a 2020  ts-barfield">.  
 00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006590: 2020 2020 3c73 7061 6e3e 4d79 2064 6561      <span>My dea
-000065a0: 7220 6261 723c 2f73 7061 6e3e 0a20 2020  r bar</span>.   
-000065b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065c0: 2020 203c 2f6c 6162 656c 3e0a 2020 2020     </label>.    
-000065d0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-000065e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000065f0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00006600: 733d 2265 7272 6f72 223e 5468 6520 656e  s="error">The en
-00006610: 7465 7265 6420 7661 6c75 6520 6973 206e  tered value is n
-00006620: 6f74 2061 2076 616c 6964 2069 6e74 6567  ot a valid integ
-00006630: 6572 206c 6974 6572 616c 2e3c 2f64 6976  er literal.</div
-00006640: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00006650: 3c64 6976 2063 6c61 7373 3d22 7769 6467  <div class="widg
-00006660: 6574 223e 0a20 2020 2020 2020 2020 2020  et">.           
-00006670: 2020 2020 2020 2020 2020 203c 696e 7075             <inpu
-00006680: 7420 7479 7065 3d22 7465 7874 220a 2020  t type="text".  
-00006690: 2020 2020 2020 2069 643d 2266 6f72 6d2d         id="form-
-000066a0: 7769 6467 6574 732d 7375 626f 626a 6563  widgets-subobjec
-000066b0: 742d 7769 6467 6574 732d 6261 7266 6965  t-widgets-barfie
-000066c0: 6c64 220a 2020 2020 2020 2020 206e 616d  ld".         nam
-000066d0: 653d 2266 6f72 6d2e 7769 6467 6574 732e  e="form.widgets.
-000066e0: 7375 626f 626a 6563 742e 7769 6467 6574  subobject.widget
-000066f0: 732e 6261 7266 6965 6c64 220a 2020 2020  s.barfield".    
-00006700: 2020 2020 2063 6c61 7373 3d22 7465 7874       class="text
-00006710: 2d77 6964 6765 7420 696e 742d 6669 656c  -widget int-fiel
-00006720: 6422 0a20 2020 2020 2020 2020 7661 6c75  d".         valu
-00006730: 653d 2262 6164 2220 2f3e 0a20 2020 2020  e="bad" />.     
-00006740: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00006750: 2020 2020 2020 3c69 6e70 7574 206e 616d        <input nam
-00006760: 653d 2266 6f72 6d2e 7769 6467 6574 732e  e="form.widgets.
-00006770: 7375 626f 626a 6563 742d 656d 7074 792d  subobject-empty-
-00006780: 6d61 726b 6572 2220 7479 7065 3d22 6869  marker" type="hi
-00006790: 6464 656e 2220 7661 6c75 653d 2231 222f  dden" value="1"/
-000067a0: 3e0a 2020 3c2f 6469 763e 0a20 2020 203c  >.  </div>.    <
-000067b0: 2f64 6976 3e0a 2020 2020 3c64 6976 2063  /div>.    <div c
-000067c0: 6c61 7373 3d22 726f 7722 3e0a 2020 2020  lass="row">.    
-000067d0: 2020 3c6c 6162 656c 2066 6f72 3d22 666f    <label for="fo
-000067e0: 726d 2d77 6964 6765 7473 2d6e 616d 6522  rm-widgets-name"
-000067f0: 3e6e 616d 653c 2f6c 6162 656c 3e0a 2020  >name</label>.  
-00006800: 2020 2020 3c69 6e70 7574 2074 7970 653d      <input type=
-00006810: 2274 6578 7422 0a20 2020 2020 2020 2020  "text".         
-00006820: 6964 3d22 666f 726d 2d77 6964 6765 7473  id="form-widgets
-00006830: 2d6e 616d 6522 0a20 2020 2020 2020 2020  -name".         
-00006840: 6e61 6d65 3d22 666f 726d 2e77 6964 6765  name="form.widge
-00006850: 7473 2e6e 616d 6522 0a20 2020 2020 2020  ts.name".       
-00006860: 2020 636c 6173 733d 2274 6578 742d 7769    class="text-wi
-00006870: 6467 6574 2072 6571 7569 7265 6420 7465  dget required te
-00006880: 7874 6c69 6e65 2d66 6965 6c64 220a 2020  xtline-field".  
-00006890: 2020 2020 2020 2076 616c 7565 3d22 6669         value="fi
-000068a0: 7273 7422 202f 3e0a 2020 2020 3c2f 6469  rst" />.    </di
-000068b0: 763e 0a20 2020 203c 6469 7620 636c 6173  v>.    <div clas
-000068c0: 733d 2261 6374 696f 6e22 3e0a 2020 2020  s="action">.    
-000068d0: 2020 3c69 6e70 7574 2074 7970 653d 2273    <input type="s
-000068e0: 7562 6d69 7422 0a20 2020 2020 2020 2020  ubmit".         
-000068f0: 6964 3d22 666f 726d 2d62 7574 746f 6e73  id="form-buttons
-00006900: 2d61 7070 6c79 220a 2020 2020 2020 2020  -apply".        
-00006910: 206e 616d 653d 2266 6f72 6d2e 6275 7474   name="form.butt
-00006920: 6f6e 732e 6170 706c 7922 0a20 2020 2020  ons.apply".     
-00006930: 2020 2020 636c 6173 733d 2273 7562 6d69      class="submi
-00006940: 742d 7769 6467 6574 2062 7574 746f 6e2d  t-widget button-
-00006950: 6669 656c 6422 0a20 2020 2020 2020 2020  field".         
-00006960: 7661 6c75 653d 2241 7070 6c79 2220 2f3e  value="Apply" />
-00006970: 0a20 2020 203c 2f64 6976 3e0a 2020 3c2f  .    </div>.  </
-00006980: 666f 726d 3e0a 0a41 6e64 206f 6620 636f  form>..And of co
-00006990: 7572 7365 2c20 7468 6520 6f62 6a65 6374  urse, the object
-000069a0: 2076 616c 7565 7320 646f 206e 6f74 2067   values do not g
-000069b0: 6574 206d 6f64 6966 6965 643a 0a0a 2020  et modified:..  
-000069c0: 3e3e 3e20 726f 6f74 5b27 6669 7273 7427  >>> root['first'
-000069d0: 5d2e 7375 626f 626a 6563 742e 666f 6f66  ].subobject.foof
-000069e0: 6965 6c64 0a20 2036 3636 0a20 203e 3e3e  ield.  666.  >>>
-000069f0: 2072 6f6f 745b 2766 6972 7374 275d 2e73   root['first'].s
-00006a00: 7562 6f62 6a65 6374 2e62 6172 6669 656c  ubobject.barfiel
-00006a10: 640a 2020 3939 390a 0a53 696d 706c 6520  d.  999..Simple 
-00006a20: 6275 7420 6f66 7465 6e20 7573 6564 2075  but often used u
-00006a30: 7365 2d63 6173 6520 6973 2074 6865 2064  se-case is the d
-00006a40: 6973 706c 6179 2066 6f72 6d3a 0a0a 2020  isplay form:..  
-00006a50: 3e3e 3e20 6564 6974 666f 726d 203d 204d  >>> editform = M
-00006a60: 7945 6469 7446 6f72 6d28 726f 6f74 5b27  yEditForm(root['
-00006a70: 6669 7273 7427 5d2c 2054 6573 7452 6571  first'], TestReq
-00006a80: 7565 7374 2829 290a 2020 3e3e 3e20 6164  uest()).  >>> ad
-00006a90: 6454 656d 706c 6174 6528 6564 6974 666f  dTemplate(editfo
-00006aa0: 726d 290a 2020 3e3e 3e20 6564 6974 666f  rm).  >>> editfo
-00006ab0: 726d 2e6d 6f64 6520 3d20 696e 7465 7266  rm.mode = interf
-00006ac0: 6163 6573 2e44 4953 504c 4159 5f4d 4f44  aces.DISPLAY_MOD
-00006ad0: 450a 2020 3e3e 3e20 6564 6974 666f 726d  E.  >>> editform
-00006ae0: 2e75 7064 6174 6528 290a 2020 3e3e 3e20  .update().  >>> 
-00006af0: 7072 696e 7428 666f 726d 6174 5f68 746d  print(format_htm
-00006b00: 6c28 6564 6974 666f 726d 2e72 656e 6465  l(editform.rende
-00006b10: 7228 2929 290a 2020 3c66 6f72 6d20 6163  r())).  <form ac
-00006b20: 7469 6f6e 3d22 2e22 3e0a 2020 2020 3c64  tion=".">.    <d
-00006b30: 6976 2063 6c61 7373 3d22 726f 7722 3e0a  iv class="row">.
-00006b40: 2020 2020 2020 3c6c 6162 656c 2066 6f72        <label for
-00006b50: 3d22 666f 726d 2d77 6964 6765 7473 2d73  ="form-widgets-s
-00006b60: 7562 6f62 6a65 6374 223e 6d79 206f 626a  ubobject">my obj
-00006b70: 6563 743c 2f6c 6162 656c 3e0a 2020 2020  ect</label>.    
-00006b80: 2020 3c64 6976 2063 6c61 7373 3d22 6f62    <div class="ob
-00006b90: 6a65 6374 2d77 6964 6765 7422 3e0a 2020  ject-widget">.  
-00006ba0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00006bb0: 2063 6c61 7373 3d22 6c61 6265 6c22 3e0a   class="label">.
-00006bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bd0: 2020 2020 2020 3c6c 6162 656c 2066 6f72        <label for
-00006be0: 3d22 666f 726d 2d77 6964 6765 7473 2d73  ="form-widgets-s
-00006bf0: 7562 6f62 6a65 6374 2d77 6964 6765 7473  ubobject-widgets
-00006c00: 2d66 6f6f 6669 656c 6422 3e0a 2020 2020  -foofield">.    
-00006c10: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00006c20: 7061 6e3e 4d79 2066 6f6f 2066 6965 6c64  pan>My foo field
-00006c30: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
-00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c50: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
-00006c60: 733d 2272 6571 7569 7265 6422 3e2a 3c2f  s="required">*</
-00006c70: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
-00006c80: 2020 2020 2020 2020 2020 2020 3c2f 6c61              </la
-00006c90: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
-00006ca0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00006cb0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00006cc0: 7373 3d22 7769 6467 6574 223e 0a20 2020  ss="widget">.   
-00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2020 203c 7370 616e 2069 643d 2266 6f72     <span id="for
-00006cf0: 6d2d 7769 6467 6574 732d 7375 626f 626a  m-widgets-subobj
-00006d00: 6563 742d 7769 6467 6574 732d 666f 6f66  ect-widgets-foof
-00006d10: 6965 6c64 220a 2020 2020 2020 2020 636c  ield".        cl
-00006d20: 6173 733d 2274 6578 742d 7769 6467 6574  ass="text-widget
-00006d30: 2069 6e74 2d66 6965 6c64 223e 3636 363c   int-field">666<
-00006d40: 2f73 7061 6e3e 0a20 2020 2020 2020 2020  /span>.         
-00006d50: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00006d60: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00006d70: 6c61 7373 3d22 6c61 6265 6c22 3e0a 2020  lass="label">.  
-00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d90: 2020 2020 3c6c 6162 656c 2066 6f72 3d22      <label for="
-00006da0: 666f 726d 2d77 6964 6765 7473 2d73 7562  form-widgets-sub
-00006db0: 6f62 6a65 6374 2d77 6964 6765 7473 2d62  object-widgets-b
-00006dc0: 6172 6669 656c 6422 3e0a 2020 2020 2020  arfield">.      
-00006dd0: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
-00006de0: 6e3e 4d79 2064 6561 7220 6261 723c 2f73  n>My dear bar</s
-00006df0: 7061 6e3e 0a20 2020 2020 2020 2020 2020  pan>.           
-00006e00: 2020 2020 2020 2020 2020 203c 2f6c 6162             </lab
-00006e10: 656c 3e0a 2020 2020 2020 2020 2020 2020  el>.            
-00006e20: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00006e30: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00006e40: 733d 2277 6964 6765 7422 3e0a 2020 2020  s="widget">.    
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2020 3c73 7061 6e20 6964 3d22 666f 726d    <span id="form
-00006e70: 2d77 6964 6765 7473 2d73 7562 6f62 6a65  -widgets-subobje
-00006e80: 6374 2d77 6964 6765 7473 2d62 6172 6669  ct-widgets-barfi
-00006e90: 656c 6422 0a20 2020 2020 2020 2063 6c61  eld".        cla
-00006ea0: 7373 3d22 7465 7874 2d77 6964 6765 7420  ss="text-widget 
-00006eb0: 696e 742d 6669 656c 6422 3e39 3939 3c2f  int-field">999</
-00006ec0: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
-00006ed0: 2020 2020 3c2f 6469 763e 0a20 203c 2f64      </div>.  </d
-00006ee0: 6976 3e0a 2020 2020 3c2f 6469 763e 0a20  iv>.    </div>. 
-00006ef0: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
-00006f00: 6f77 223e 0a20 2020 2020 203c 6c61 6265  ow">.      <labe
-00006f10: 6c20 666f 723d 2266 6f72 6d2d 7769 6467  l for="form-widg
-00006f20: 6574 732d 6e61 6d65 223e 6e61 6d65 3c2f  ets-name">name</
-00006f30: 6c61 6265 6c3e 0a20 2020 2020 203c 7370  label>.      <sp
-00006f40: 616e 2069 643d 2266 6f72 6d2d 7769 6467  an id="form-widg
-00006f50: 6574 732d 6e61 6d65 220a 2020 2020 2020  ets-name".      
-00006f60: 2020 636c 6173 733d 2274 6578 742d 7769    class="text-wi
-00006f70: 6467 6574 2074 6578 746c 696e 652d 6669  dget textline-fi
-00006f80: 656c 6422 3e66 6972 7374 3c2f 7370 616e  eld">first</span
-00006f90: 3e0a 2020 2020 3c2f 6469 763e 0a20 2020  >.    </div>.   
-00006fa0: 203c 6469 7620 636c 6173 733d 2261 6374   <div class="act
-00006fb0: 696f 6e22 3e0a 2020 2020 2020 3c69 6e70  ion">.      <inp
-00006fc0: 7574 2074 7970 653d 2273 7562 6d69 7422  ut type="submit"
-00006fd0: 0a20 2020 2020 2020 2020 6964 3d22 666f  .         id="fo
-00006fe0: 726d 2d62 7574 746f 6e73 2d61 7070 6c79  rm-buttons-apply
-00006ff0: 220a 2020 2020 2020 2020 206e 616d 653d  ".         name=
-00007000: 2266 6f72 6d2e 6275 7474 6f6e 732e 6170  "form.buttons.ap
-00007010: 706c 7922 0a20 2020 2020 2020 2020 636c  ply".         cl
-00007020: 6173 733d 2273 7562 6d69 742d 7769 6467  ass="submit-widg
-00007030: 6574 2062 7574 746f 6e2d 6669 656c 6422  et button-field"
-00007040: 0a20 2020 2020 2020 2020 7661 6c75 653d  .         value=
-00007050: 2241 7070 6c79 2220 2f3e 0a20 2020 203c  "Apply" />.    <
-00007060: 2f64 6976 3e0a 2020 3c2f 666f 726d 3e0a  /div>.  </form>.
-00007070: 0a4c 6574 2773 2073 6565 2077 6861 7420  .Let's see what 
-00007080: 6861 7070 656e 7320 696e 2048 4944 4445  happens in HIDDE
-00007090: 4e5f 4d4f 4445 2028 286e 6f74 2071 7569  N_MODE ((not qui
-000070a0: 7465 2073 616e 6520 7468 696e 672c 2062  te sane thing, b
-000070b0: 7574 2077 6520 7761 6e74 2074 6f20 7365  ut we want to se
-000070c0: 6520 7468 650a 6f62 6a65 6374 7769 6467  e the.objectwidg
-000070d0: 6574 2072 656e 6465 7265 6420 696e 2068  et rendered in h
-000070e0: 6964 6465 6e20 6d6f 6465 293a 0a0a 2020  idden mode):..  
-000070f0: 3e3e 3e20 6564 6974 666f 726d 203d 204d  >>> editform = M
-00007100: 7945 6469 7446 6f72 6d28 726f 6f74 5b27  yEditForm(root['
-00007110: 6669 7273 7427 5d2c 2054 6573 7452 6571  first'], TestReq
-00007120: 7565 7374 2829 290a 2020 3e3e 3e20 6164  uest()).  >>> ad
-00007130: 6454 656d 706c 6174 6528 6564 6974 666f  dTemplate(editfo
-00007140: 726d 290a 2020 3e3e 3e20 6564 6974 666f  rm).  >>> editfo
-00007150: 726d 2e6d 6f64 6520 3d20 696e 7465 7266  rm.mode = interf
-00007160: 6163 6573 2e48 4944 4445 4e5f 4d4f 4445  aces.HIDDEN_MODE
-00007170: 0a20 203e 3e3e 2065 6469 7466 6f72 6d2e  .  >>> editform.
-00007180: 7570 6461 7465 2829 0a0a 4e6f 7465 2c20  update()..Note, 
-00007190: 7468 6174 2074 6865 206c 6162 656c 7320  that the labels 
-000071a0: 616e 6420 7468 6520 6275 7474 6f6e 2069  and the button i
-000071b0: 7320 7468 6572 6520 6265 6361 7573 6520  s there because 
-000071c0: 7468 6520 666f 726d 2074 656d 706c 6174  the form templat
-000071d0: 6520 666f 7220 7465 7374 696e 670a 646f  e for testing.do
-000071e0: 6573 2f73 686f 756c 6420 6e6f 7420 6361  es/should not ca
-000071f0: 7265 2061 626f 7574 2074 6865 2066 6f72  re about the for
-00007200: 6d20 6265 696e 6720 6869 6464 656e 2e0a  m being hidden..
-00007210: 5768 6174 206d 6174 7465 7273 2069 7320  What matters is 
-00007220: 7468 6174 2074 6865 206f 626a 6563 7477  that the objectw
-00007230: 6964 6765 7420 6973 2072 656e 6465 7265  idget is rendere
-00007240: 6420 6869 6464 656e 2e0a 0a20 203e 3e3e  d hidden...  >>>
-00007250: 2070 7269 6e74 2866 6f72 6d61 745f 6874   print(format_ht
-00007260: 6d6c 2865 6469 7466 6f72 6d2e 7265 6e64  ml(editform.rend
-00007270: 6572 2829 2929 0a20 203c 666f 726d 2061  er())).  <form a
-00007280: 6374 696f 6e3d 222e 223e 0a20 2020 203c  ction=".">.    <
-00007290: 6469 7620 636c 6173 733d 2272 6f77 223e  div class="row">
-000072a0: 0a20 2020 2020 203c 6c61 6265 6c20 666f  .      <label fo
-000072b0: 723d 2266 6f72 6d2d 7769 6467 6574 732d  r="form-widgets-
-000072c0: 7375 626f 626a 6563 7422 3e6d 7920 6f62  subobject">my ob
-000072d0: 6a65 6374 3c2f 6c61 6265 6c3e 0a20 2020  ject</label>.   
-000072e0: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
-000072f0: 6869 6464 656e 220a 2020 2020 2020 2020  hidden".        
-00007300: 2069 643d 2266 6f72 6d2d 7769 6467 6574   id="form-widget
-00007310: 732d 7375 626f 626a 6563 742d 7769 6467  s-subobject-widg
-00007320: 6574 732d 666f 6f66 6965 6c64 220a 2020  ets-foofield".  
-00007330: 2020 2020 2020 206e 616d 653d 2266 6f72         name="for
-00007340: 6d2e 7769 6467 6574 732e 7375 626f 626a  m.widgets.subobj
-00007350: 6563 742e 7769 6467 6574 732e 666f 6f66  ect.widgets.foof
-00007360: 6965 6c64 220a 2020 2020 2020 2020 2076  ield".         v
-00007370: 616c 7565 3d22 3636 3622 0a20 2020 2020  alue="666".     
-00007380: 2020 2020 636c 6173 733d 2268 6964 6465      class="hidde
-00007390: 6e2d 7769 6467 6574 2220 2f3e 0a20 2020  n-widget" />.   
-000073a0: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
-000073b0: 6869 6464 656e 220a 2020 2020 2020 2020  hidden".        
-000073c0: 2069 643d 2266 6f72 6d2d 7769 6467 6574   id="form-widget
-000073d0: 732d 7375 626f 626a 6563 742d 7769 6467  s-subobject-widg
-000073e0: 6574 732d 6261 7266 6965 6c64 220a 2020  ets-barfield".  
-000073f0: 2020 2020 2020 206e 616d 653d 2266 6f72         name="for
-00007400: 6d2e 7769 6467 6574 732e 7375 626f 626a  m.widgets.subobj
-00007410: 6563 742e 7769 6467 6574 732e 6261 7266  ect.widgets.barf
-00007420: 6965 6c64 220a 2020 2020 2020 2020 2076  ield".         v
-00007430: 616c 7565 3d22 3939 3922 0a20 2020 2020  alue="999".     
-00007440: 2020 2020 636c 6173 733d 2268 6964 6465      class="hidde
-00007450: 6e2d 7769 6467 6574 2220 2f3e 0a20 2020  n-widget" />.   
-00007460: 203c 2f64 6976 3e0a 2020 2020 3c64 6976   </div>.    <div
-00007470: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
-00007480: 2020 2020 3c6c 6162 656c 2066 6f72 3d22      <label for="
-00007490: 666f 726d 2d77 6964 6765 7473 2d6e 616d  form-widgets-nam
-000074a0: 6522 3e6e 616d 653c 2f6c 6162 656c 3e0a  e">name</label>.
-000074b0: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
-000074c0: 653d 2268 6964 6465 6e22 0a20 2020 2020  e="hidden".     
-000074d0: 2020 2020 6964 3d22 666f 726d 2d77 6964      id="form-wid
-000074e0: 6765 7473 2d6e 616d 6522 0a20 2020 2020  gets-name".     
-000074f0: 2020 2020 6e61 6d65 3d22 666f 726d 2e77      name="form.w
-00007500: 6964 6765 7473 2e6e 616d 6522 0a20 2020  idgets.name".   
-00007510: 2020 2020 2020 7661 6c75 653d 2266 6972        value="fir
-00007520: 7374 220a 2020 2020 2020 2020 2063 6c61  st".         cla
-00007530: 7373 3d22 6869 6464 656e 2d77 6964 6765  ss="hidden-widge
-00007540: 7422 202f 3e0a 2020 2020 3c2f 6469 763e  t" />.    </div>
-00007550: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
-00007560: 2261 6374 696f 6e22 3e0a 2020 2020 2020  "action">.      
-00007570: 3c69 6e70 7574 2074 7970 653d 2273 7562  <input type="sub
-00007580: 6d69 7422 0a20 2020 2020 2020 2020 6964  mit".         id
-00007590: 3d22 666f 726d 2d62 7574 746f 6e73 2d61  ="form-buttons-a
-000075a0: 7070 6c79 220a 2020 2020 2020 2020 206e  pply".         n
-000075b0: 616d 653d 2266 6f72 6d2e 6275 7474 6f6e  ame="form.button
-000075c0: 732e 6170 706c 7922 0a20 2020 2020 2020  s.apply".       
-000075d0: 2020 636c 6173 733d 2273 7562 6d69 742d    class="submit-
-000075e0: 7769 6467 6574 2062 7574 746f 6e2d 6669  widget button-fi
-000075f0: 656c 6422 0a20 2020 2020 2020 2020 7661  eld".         va
-00007600: 6c75 653d 2241 7070 6c79 2220 2f3e 0a20  lue="Apply" />. 
-00007610: 2020 203c 2f64 6976 3e0a 2020 3c2f 666f     </div>.  </fo
-00007620: 726d 3e0a 0a0a 4564 6974 666f 726d 7320  rm>...Editforms 
-00007630: 6d69 6768 7420 7573 6520 6469 6374 7320  might use dicts 
-00007640: 6173 2063 6f6e 7465 7874 3a0a 0a20 203e  as context:..  >
-00007650: 3e3e 206e 6577 7375 6220 3d20 4d79 5375  >> newsub = MySu
-00007660: 624f 626a 6563 7428 290a 2020 3e3e 3e20  bObject().  >>> 
-00007670: 6e65 7773 7562 2e66 6f6f 6669 656c 6420  newsub.foofield 
-00007680: 3d20 3738 0a20 203e 3e3e 206e 6577 7375  = 78.  >>> newsu
-00007690: 622e 6261 7266 6965 6c64 203d 2038 370a  b.barfield = 87.
-000076a0: 0a20 203e 3e3e 2063 6c61 7373 204d 7945  .  >>> class MyE
-000076b0: 6469 7446 6f72 6d44 6963 7428 666f 726d  ditFormDict(form
-000076c0: 2e45 6469 7446 6f72 6d29 3a0a 2020 2e2e  .EditForm):.  ..
-000076d0: 2e20 2020 2020 6669 656c 6473 203d 2066  .     fields = f
-000076e0: 6965 6c64 2e46 6965 6c64 7328 494d 794f  ield.Fields(IMyO
-000076f0: 626a 6563 7429 0a20 202e 2e2e 2020 2020  bject).  ...    
-00007700: 2064 6566 2067 6574 5f63 6f6e 7465 6e74   def get_content
-00007710: 2873 656c 6629 3a0a 2020 2e2e 2e20 2020  (self):.  ...   
-00007720: 2020 2020 2020 7265 7475 726e 207b 2773        return {'s
-00007730: 7562 6f62 6a65 6374 273a 206e 6577 7375  ubobject': newsu
-00007740: 622c 2027 6e61 6d65 273a 2027 626c 6f6f  b, 'name': 'bloo
-00007750: 6b69 277d 0a0a 2020 3e3e 3e20 6564 6974  ki'}..  >>> edit
-00007760: 666f 726d 203d 204d 7945 6469 7446 6f72  form = MyEditFor
-00007770: 6d44 6963 7428 4e6f 6e65 2c20 5465 7374  mDict(None, Test
-00007780: 5265 7175 6573 7428 2929 0a20 203e 3e3e  Request()).  >>>
-00007790: 2061 6464 5465 6d70 6c61 7465 2865 6469   addTemplate(edi
-000077a0: 7466 6f72 6d29 0a20 203e 3e3e 2065 6469  tform).  >>> edi
-000077b0: 7466 6f72 6d2e 7570 6461 7465 2829 0a0a  tform.update()..
-000077c0: 5761 7463 6820 666f 7220 7468 6520 7769  Watch for the wi
-000077d0: 6467 6574 2076 616c 7565 7320 696e 2074  dget values in t
-000077e0: 6865 2048 544d 4c3a 0a0a 2020 3e3e 3e20  he HTML:..  >>> 
-000077f0: 7072 696e 7428 666f 726d 6174 5f68 746d  print(format_htm
-00007800: 6c28 6564 6974 666f 726d 2e72 656e 6465  l(editform.rende
-00007810: 7228 2929 290a 2020 3c66 6f72 6d20 6163  r())).  <form ac
-00007820: 7469 6f6e 3d22 2e22 3e0a 2020 2020 3c64  tion=".">.    <d
-00007830: 6976 2063 6c61 7373 3d22 726f 7722 3e0a  iv class="row">.
-00007840: 2020 2020 2020 3c6c 6162 656c 2066 6f72        <label for
-00007850: 3d22 666f 726d 2d77 6964 6765 7473 2d73  ="form-widgets-s
-00007860: 7562 6f62 6a65 6374 223e 6d79 206f 626a  ubobject">my obj
-00007870: 6563 743c 2f6c 6162 656c 3e0a 2020 2020  ect</label>.    
-00007880: 2020 3c64 6976 2063 6c61 7373 3d22 6f62    <div class="ob
-00007890: 6a65 6374 2d77 6964 6765 7420 7265 7175  ject-widget requ
-000078a0: 6972 6564 223e 0a20 2020 2020 2020 2020  ired">.         
-000078b0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-000078c0: 226c 6162 656c 223e 0a20 2020 2020 2020  "label">.       
-000078d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000078e0: 6c61 6265 6c20 666f 723d 2266 6f72 6d2d  label for="form-
-000078f0: 7769 6467 6574 732d 7375 626f 626a 6563  widgets-subobjec
-00007900: 742d 7769 6467 6574 732d 666f 6f66 6965  t-widgets-foofie
-00007910: 6c64 223e 0a20 2020 2020 2020 2020 2020  ld">.           
+00006590: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
+000065a0: 6e3e 4d79 2064 6561 7220 6261 723c 2f73  n>My dear bar</s
+000065b0: 7061 6e3e 0a20 2020 2020 2020 2020 2020  pan>.           
+000065c0: 2020 2020 2020 2020 2020 203c 2f6c 6162             </lab
+000065d0: 656c 3e0a 2020 2020 2020 2020 2020 2020  el>.            
+000065e0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+000065f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006600: 6469 7620 636c 6173 733d 2265 7272 6f72  div class="error
+00006610: 223e 5468 6520 656e 7465 7265 6420 7661  ">The entered va
+00006620: 6c75 6520 6973 206e 6f74 2061 2076 616c  lue is not a val
+00006630: 6964 2069 6e74 6567 6572 206c 6974 6572  id integer liter
+00006640: 616c 2e3c 2f64 6976 3e0a 2020 2020 2020  al.</div>.      
+00006650: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00006660: 7373 3d22 7769 6467 6574 223e 0a20 2020  ss="widget">.   
+00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006680: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
+00006690: 7465 7874 220a 2020 2020 2020 2020 2069  text".         i
+000066a0: 643d 2266 6f72 6d2d 7769 6467 6574 732d  d="form-widgets-
+000066b0: 7375 626f 626a 6563 742d 7769 6467 6574  subobject-widget
+000066c0: 732d 6261 7266 6965 6c64 220a 2020 2020  s-barfield".    
+000066d0: 2020 2020 206e 616d 653d 2266 6f72 6d2e       name="form.
+000066e0: 7769 6467 6574 732e 7375 626f 626a 6563  widgets.subobjec
+000066f0: 742e 7769 6467 6574 732e 6261 7266 6965  t.widgets.barfie
+00006700: 6c64 220a 2020 2020 2020 2020 2063 6c61  ld".         cla
+00006710: 7373 3d22 7465 7874 2d77 6964 6765 7420  ss="text-widget 
+00006720: 696e 742d 6669 656c 6422 0a20 2020 2020  int-field".     
+00006730: 2020 2020 7661 6c75 653d 2262 6164 2220      value="bad" 
+00006740: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00006750: 203c 2f64 6976 3e0a 2020 2020 2020 3c69   </div>.      <i
+00006760: 6e70 7574 206e 616d 653d 2266 6f72 6d2e  nput name="form.
+00006770: 7769 6467 6574 732e 7375 626f 626a 6563  widgets.subobjec
+00006780: 742d 656d 7074 792d 6d61 726b 6572 2220  t-empty-marker" 
+00006790: 7479 7065 3d22 6869 6464 656e 2220 7661  type="hidden" va
+000067a0: 6c75 653d 2231 2220 2f3e 0a20 203c 2f64  lue="1" />.  </d
+000067b0: 6976 3e0a 2020 2020 3c2f 6469 763e 0a20  iv>.    </div>. 
+000067c0: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
+000067d0: 6f77 223e 0a20 2020 2020 203c 6c61 6265  ow">.      <labe
+000067e0: 6c20 666f 723d 2266 6f72 6d2d 7769 6467  l for="form-widg
+000067f0: 6574 732d 6e61 6d65 223e 6e61 6d65 3c2f  ets-name">name</
+00006800: 6c61 6265 6c3e 0a20 2020 2020 203c 696e  label>.      <in
+00006810: 7075 7420 7479 7065 3d22 7465 7874 220a  put type="text".
+00006820: 2020 2020 2020 2020 2069 643d 2266 6f72           id="for
+00006830: 6d2d 7769 6467 6574 732d 6e61 6d65 220a  m-widgets-name".
+00006840: 2020 2020 2020 2020 206e 616d 653d 2266           name="f
+00006850: 6f72 6d2e 7769 6467 6574 732e 6e61 6d65  orm.widgets.name
+00006860: 220a 2020 2020 2020 2020 2063 6c61 7373  ".         class
+00006870: 3d22 7465 7874 2d77 6964 6765 7420 7265  ="text-widget re
+00006880: 7175 6972 6564 2074 6578 746c 696e 652d  quired textline-
+00006890: 6669 656c 6422 0a20 2020 2020 2020 2020  field".         
+000068a0: 7661 6c75 653d 2266 6972 7374 2220 2f3e  value="first" />
+000068b0: 0a20 2020 203c 2f64 6976 3e0a 2020 2020  .    </div>.    
+000068c0: 3c64 6976 2063 6c61 7373 3d22 6163 7469  <div class="acti
+000068d0: 6f6e 223e 0a20 2020 2020 203c 696e 7075  on">.      <inpu
+000068e0: 7420 7479 7065 3d22 7375 626d 6974 220a  t type="submit".
+000068f0: 2020 2020 2020 2020 2069 643d 2266 6f72           id="for
+00006900: 6d2d 6275 7474 6f6e 732d 6170 706c 7922  m-buttons-apply"
+00006910: 0a20 2020 2020 2020 2020 6e61 6d65 3d22  .         name="
+00006920: 666f 726d 2e62 7574 746f 6e73 2e61 7070  form.buttons.app
+00006930: 6c79 220a 2020 2020 2020 2020 2063 6c61  ly".         cla
+00006940: 7373 3d22 7375 626d 6974 2d77 6964 6765  ss="submit-widge
+00006950: 7420 6275 7474 6f6e 2d66 6965 6c64 220a  t button-field".
+00006960: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
+00006970: 4170 706c 7922 202f 3e0a 2020 2020 3c2f  Apply" />.    </
+00006980: 6469 763e 0a20 203c 2f66 6f72 6d3e 0a0a  div>.  </form>..
+00006990: 416e 6420 6f66 2063 6f75 7273 652c 2074  And of course, t
+000069a0: 6865 206f 626a 6563 7420 7661 6c75 6573  he object values
+000069b0: 2064 6f20 6e6f 7420 6765 7420 6d6f 6469   do not get modi
+000069c0: 6669 6564 3a0a 0a20 203e 3e3e 2072 6f6f  fied:..  >>> roo
+000069d0: 745b 2766 6972 7374 275d 2e73 7562 6f62  t['first'].subob
+000069e0: 6a65 6374 2e66 6f6f 6669 656c 640a 2020  ject.foofield.  
+000069f0: 3636 360a 2020 3e3e 3e20 726f 6f74 5b27  666.  >>> root['
+00006a00: 6669 7273 7427 5d2e 7375 626f 626a 6563  first'].subobjec
+00006a10: 742e 6261 7266 6965 6c64 0a20 2039 3939  t.barfield.  999
+00006a20: 0a0a 5369 6d70 6c65 2062 7574 206f 6674  ..Simple but oft
+00006a30: 656e 2075 7365 6420 7573 652d 6361 7365  en used use-case
+00006a40: 2069 7320 7468 6520 6469 7370 6c61 7920   is the display 
+00006a50: 666f 726d 3a0a 0a20 203e 3e3e 2065 6469  form:..  >>> edi
+00006a60: 7466 6f72 6d20 3d20 4d79 4564 6974 466f  tform = MyEditFo
+00006a70: 726d 2872 6f6f 745b 2766 6972 7374 275d  rm(root['first']
+00006a80: 2c20 5465 7374 5265 7175 6573 7428 2929  , TestRequest())
+00006a90: 0a20 203e 3e3e 2061 6464 5465 6d70 6c61  .  >>> addTempla
+00006aa0: 7465 2865 6469 7466 6f72 6d29 0a20 203e  te(editform).  >
+00006ab0: 3e3e 2065 6469 7466 6f72 6d2e 6d6f 6465  >> editform.mode
+00006ac0: 203d 2069 6e74 6572 6661 6365 732e 4449   = interfaces.DI
+00006ad0: 5350 4c41 595f 4d4f 4445 0a20 203e 3e3e  SPLAY_MODE.  >>>
+00006ae0: 2065 6469 7466 6f72 6d2e 7570 6461 7465   editform.update
+00006af0: 2829 0a20 203e 3e3e 2070 7269 6e74 2866  ().  >>> print(f
+00006b00: 6f72 6d61 745f 6874 6d6c 2865 6469 7466  ormat_html(editf
+00006b10: 6f72 6d2e 7265 6e64 6572 2829 2929 0a20  orm.render())). 
+00006b20: 203c 666f 726d 2061 6374 696f 6e3d 222e   <form action=".
+00006b30: 223e 0a20 2020 203c 6469 7620 636c 6173  ">.    <div clas
+00006b40: 733d 2272 6f77 223e 0a20 2020 2020 203c  s="row">.      <
+00006b50: 6c61 6265 6c20 666f 723d 2266 6f72 6d2d  label for="form-
+00006b60: 7769 6467 6574 732d 7375 626f 626a 6563  widgets-subobjec
+00006b70: 7422 3e6d 7920 6f62 6a65 6374 3c2f 6c61  t">my object</la
+00006b80: 6265 6c3e 0a20 2020 2020 203c 6469 7620  bel>.      <div 
+00006b90: 636c 6173 733d 226f 626a 6563 742d 7769  class="object-wi
+00006ba0: 6467 6574 223e 0a20 2020 2020 2020 2020  dget">.         
+00006bb0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00006bc0: 226c 6162 656c 223e 0a20 2020 2020 2020  "label">.       
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006be0: 6c61 6265 6c20 666f 723d 2266 6f72 6d2d  label for="form-
+00006bf0: 7769 6467 6574 732d 7375 626f 626a 6563  widgets-subobjec
+00006c00: 742d 7769 6467 6574 732d 666f 6f66 6965  t-widgets-foofie
+00006c10: 6c64 223e 0a20 2020 2020 2020 2020 2020  ld">.           
+00006c20: 2020 2020 2020 203c 7370 616e 3e4d 7920         <span>My 
+00006c30: 666f 6f20 6669 656c 643c 2f73 7061 6e3e  foo field</span>
+00006c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006c60: 7370 616e 2063 6c61 7373 3d22 7265 7175  span class="requ
+00006c70: 6972 6564 223e 2a3c 2f73 7061 6e3e 0a20  ired">*</span>. 
+00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c90: 2020 2020 203c 2f6c 6162 656c 3e0a 2020       </label>.  
+00006ca0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00006cb0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00006cc0: 203c 6469 7620 636c 6173 733d 2277 6964   <div class="wid
+00006cd0: 6765 7422 3e0a 2020 2020 2020 2020 2020  get">.          
+00006ce0: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
+00006cf0: 6e20 6964 3d22 666f 726d 2d77 6964 6765  n id="form-widge
+00006d00: 7473 2d73 7562 6f62 6a65 6374 2d77 6964  ts-subobject-wid
+00006d10: 6765 7473 2d66 6f6f 6669 656c 6422 0a20  gets-foofield". 
+00006d20: 2020 2020 2020 2063 6c61 7373 3d22 7465         class="te
+00006d30: 7874 2d77 6964 6765 7420 696e 742d 6669  xt-widget int-fi
+00006d40: 656c 6422 3e36 3636 3c2f 7370 616e 3e0a  eld">666</span>.
+00006d50: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00006d60: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00006d70: 2020 203c 6469 7620 636c 6173 733d 226c     <div class="l
+00006d80: 6162 656c 223e 0a20 2020 2020 2020 2020  abel">.         
+00006d90: 2020 2020 2020 2020 2020 2020 203c 6c61               <la
+00006da0: 6265 6c20 666f 723d 2266 6f72 6d2d 7769  bel for="form-wi
+00006db0: 6467 6574 732d 7375 626f 626a 6563 742d  dgets-subobject-
+00006dc0: 7769 6467 6574 732d 6261 7266 6965 6c64  widgets-barfield
+00006dd0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00006de0: 2020 2020 203c 7370 616e 3e4d 7920 6465       <span>My de
+00006df0: 6172 2062 6172 3c2f 7370 616e 3e0a 2020  ar bar</span>.  
+00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e10: 2020 2020 3c2f 6c61 6265 6c3e 0a20 2020      </label>.   
+00006e20: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00006e30: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006e40: 3c64 6976 2063 6c61 7373 3d22 7769 6467  <div class="widg
+00006e50: 6574 223e 0a20 2020 2020 2020 2020 2020  et">.           
+00006e60: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+00006e70: 2069 643d 2266 6f72 6d2d 7769 6467 6574   id="form-widget
+00006e80: 732d 7375 626f 626a 6563 742d 7769 6467  s-subobject-widg
+00006e90: 6574 732d 6261 7266 6965 6c64 220a 2020  ets-barfield".  
+00006ea0: 2020 2020 2020 636c 6173 733d 2274 6578        class="tex
+00006eb0: 742d 7769 6467 6574 2069 6e74 2d66 6965  t-widget int-fie
+00006ec0: 6c64 223e 3939 393c 2f73 7061 6e3e 0a20  ld">999</span>. 
+00006ed0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00006ee0: 6976 3e0a 2020 3c2f 6469 763e 0a20 2020  iv>.  </div>.   
+00006ef0: 203c 2f64 6976 3e0a 2020 2020 3c64 6976   </div>.    <div
+00006f00: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
+00006f10: 2020 2020 3c6c 6162 656c 2066 6f72 3d22      <label for="
+00006f20: 666f 726d 2d77 6964 6765 7473 2d6e 616d  form-widgets-nam
+00006f30: 6522 3e6e 616d 653c 2f6c 6162 656c 3e0a  e">name</label>.
+00006f40: 2020 2020 2020 3c73 7061 6e20 6964 3d22        <span id="
+00006f50: 666f 726d 2d77 6964 6765 7473 2d6e 616d  form-widgets-nam
+00006f60: 6522 0a20 2020 2020 2020 2063 6c61 7373  e".        class
+00006f70: 3d22 7465 7874 2d77 6964 6765 7420 7465  ="text-widget te
+00006f80: 7874 6c69 6e65 2d66 6965 6c64 223e 6669  xtline-field">fi
+00006f90: 7273 743c 2f73 7061 6e3e 0a20 2020 203c  rst</span>.    <
+00006fa0: 2f64 6976 3e0a 2020 2020 3c64 6976 2063  /div>.    <div c
+00006fb0: 6c61 7373 3d22 6163 7469 6f6e 223e 0a20  lass="action">. 
+00006fc0: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
+00006fd0: 3d22 7375 626d 6974 220a 2020 2020 2020  ="submit".      
+00006fe0: 2020 2069 643d 2266 6f72 6d2d 6275 7474     id="form-butt
+00006ff0: 6f6e 732d 6170 706c 7922 0a20 2020 2020  ons-apply".     
+00007000: 2020 2020 6e61 6d65 3d22 666f 726d 2e62      name="form.b
+00007010: 7574 746f 6e73 2e61 7070 6c79 220a 2020  uttons.apply".  
+00007020: 2020 2020 2020 2063 6c61 7373 3d22 7375         class="su
+00007030: 626d 6974 2d77 6964 6765 7420 6275 7474  bmit-widget butt
+00007040: 6f6e 2d66 6965 6c64 220a 2020 2020 2020  on-field".      
+00007050: 2020 2076 616c 7565 3d22 4170 706c 7922     value="Apply"
+00007060: 202f 3e0a 2020 2020 3c2f 6469 763e 0a20   />.    </div>. 
+00007070: 203c 2f66 6f72 6d3e 0a0a 4c65 7427 7320   </form>..Let's 
+00007080: 7365 6520 7768 6174 2068 6170 7065 6e73  see what happens
+00007090: 2069 6e20 4849 4444 454e 5f4d 4f44 4520   in HIDDEN_MODE 
+000070a0: 2828 6e6f 7420 7175 6974 6520 7361 6e65  ((not quite sane
+000070b0: 2074 6869 6e67 2c20 6275 7420 7765 2077   thing, but we w
+000070c0: 616e 7420 746f 2073 6565 2074 6865 0a6f  ant to see the.o
+000070d0: 626a 6563 7477 6964 6765 7420 7265 6e64  bjectwidget rend
+000070e0: 6572 6564 2069 6e20 6869 6464 656e 206d  ered in hidden m
+000070f0: 6f64 6529 3a0a 0a20 203e 3e3e 2065 6469  ode):..  >>> edi
+00007100: 7466 6f72 6d20 3d20 4d79 4564 6974 466f  tform = MyEditFo
+00007110: 726d 2872 6f6f 745b 2766 6972 7374 275d  rm(root['first']
+00007120: 2c20 5465 7374 5265 7175 6573 7428 2929  , TestRequest())
+00007130: 0a20 203e 3e3e 2061 6464 5465 6d70 6c61  .  >>> addTempla
+00007140: 7465 2865 6469 7466 6f72 6d29 0a20 203e  te(editform).  >
+00007150: 3e3e 2065 6469 7466 6f72 6d2e 6d6f 6465  >> editform.mode
+00007160: 203d 2069 6e74 6572 6661 6365 732e 4849   = interfaces.HI
+00007170: 4444 454e 5f4d 4f44 450a 2020 3e3e 3e20  DDEN_MODE.  >>> 
+00007180: 6564 6974 666f 726d 2e75 7064 6174 6528  editform.update(
+00007190: 290a 0a4e 6f74 652c 2074 6861 7420 7468  )..Note, that th
+000071a0: 6520 6c61 6265 6c73 2061 6e64 2074 6865  e labels and the
+000071b0: 2062 7574 746f 6e20 6973 2074 6865 7265   button is there
+000071c0: 2062 6563 6175 7365 2074 6865 2066 6f72   because the for
+000071d0: 6d20 7465 6d70 6c61 7465 2066 6f72 2074  m template for t
+000071e0: 6573 7469 6e67 0a64 6f65 732f 7368 6f75  esting.does/shou
+000071f0: 6c64 206e 6f74 2063 6172 6520 6162 6f75  ld not care abou
+00007200: 7420 7468 6520 666f 726d 2062 6569 6e67  t the form being
+00007210: 2068 6964 6465 6e2e 0a57 6861 7420 6d61   hidden..What ma
+00007220: 7474 6572 7320 6973 2074 6861 7420 7468  tters is that th
+00007230: 6520 6f62 6a65 6374 7769 6467 6574 2069  e objectwidget i
+00007240: 7320 7265 6e64 6572 6564 2068 6964 6465  s rendered hidde
+00007250: 6e2e 0a0a 2020 3e3e 3e20 7072 696e 7428  n...  >>> print(
+00007260: 666f 726d 6174 5f68 746d 6c28 6564 6974  format_html(edit
+00007270: 666f 726d 2e72 656e 6465 7228 2929 290a  form.render())).
+00007280: 2020 3c66 6f72 6d20 6163 7469 6f6e 3d22    <form action="
+00007290: 2e22 3e0a 2020 2020 3c64 6976 2063 6c61  .">.    <div cla
+000072a0: 7373 3d22 726f 7722 3e0a 2020 2020 2020  ss="row">.      
+000072b0: 3c6c 6162 656c 2066 6f72 3d22 666f 726d  <label for="form
+000072c0: 2d77 6964 6765 7473 2d73 7562 6f62 6a65  -widgets-subobje
+000072d0: 6374 223e 6d79 206f 626a 6563 743c 2f6c  ct">my object</l
+000072e0: 6162 656c 3e0a 2020 2020 2020 3c69 6e70  abel>.      <inp
+000072f0: 7574 2074 7970 653d 2268 6964 6465 6e22  ut type="hidden"
+00007300: 0a20 2020 2020 2020 2020 6964 3d22 666f  .         id="fo
+00007310: 726d 2d77 6964 6765 7473 2d73 7562 6f62  rm-widgets-subob
+00007320: 6a65 6374 2d77 6964 6765 7473 2d66 6f6f  ject-widgets-foo
+00007330: 6669 656c 6422 0a20 2020 2020 2020 2020  field".         
+00007340: 6e61 6d65 3d22 666f 726d 2e77 6964 6765  name="form.widge
+00007350: 7473 2e73 7562 6f62 6a65 6374 2e77 6964  ts.subobject.wid
+00007360: 6765 7473 2e66 6f6f 6669 656c 6422 0a20  gets.foofield". 
+00007370: 2020 2020 2020 2020 7661 6c75 653d 2236          value="6
+00007380: 3636 220a 2020 2020 2020 2020 2063 6c61  66".         cla
+00007390: 7373 3d22 6869 6464 656e 2d77 6964 6765  ss="hidden-widge
+000073a0: 7422 202f 3e0a 2020 2020 2020 3c69 6e70  t" />.      <inp
+000073b0: 7574 2074 7970 653d 2268 6964 6465 6e22  ut type="hidden"
+000073c0: 0a20 2020 2020 2020 2020 6964 3d22 666f  .         id="fo
+000073d0: 726d 2d77 6964 6765 7473 2d73 7562 6f62  rm-widgets-subob
+000073e0: 6a65 6374 2d77 6964 6765 7473 2d62 6172  ject-widgets-bar
+000073f0: 6669 656c 6422 0a20 2020 2020 2020 2020  field".         
+00007400: 6e61 6d65 3d22 666f 726d 2e77 6964 6765  name="form.widge
+00007410: 7473 2e73 7562 6f62 6a65 6374 2e77 6964  ts.subobject.wid
+00007420: 6765 7473 2e62 6172 6669 656c 6422 0a20  gets.barfield". 
+00007430: 2020 2020 2020 2020 7661 6c75 653d 2239          value="9
+00007440: 3939 220a 2020 2020 2020 2020 2063 6c61  99".         cla
+00007450: 7373 3d22 6869 6464 656e 2d77 6964 6765  ss="hidden-widge
+00007460: 7422 202f 3e0a 2020 2020 3c2f 6469 763e  t" />.    </div>
+00007470: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+00007480: 2272 6f77 223e 0a20 2020 2020 203c 6c61  "row">.      <la
+00007490: 6265 6c20 666f 723d 2266 6f72 6d2d 7769  bel for="form-wi
+000074a0: 6467 6574 732d 6e61 6d65 223e 6e61 6d65  dgets-name">name
+000074b0: 3c2f 6c61 6265 6c3e 0a20 2020 2020 203c  </label>.      <
+000074c0: 696e 7075 7420 7479 7065 3d22 6869 6464  input type="hidd
+000074d0: 656e 220a 2020 2020 2020 2020 2069 643d  en".         id=
+000074e0: 2266 6f72 6d2d 7769 6467 6574 732d 6e61  "form-widgets-na
+000074f0: 6d65 220a 2020 2020 2020 2020 206e 616d  me".         nam
+00007500: 653d 2266 6f72 6d2e 7769 6467 6574 732e  e="form.widgets.
+00007510: 6e61 6d65 220a 2020 2020 2020 2020 2076  name".         v
+00007520: 616c 7565 3d22 6669 7273 7422 0a20 2020  alue="first".   
+00007530: 2020 2020 2020 636c 6173 733d 2268 6964        class="hid
+00007540: 6465 6e2d 7769 6467 6574 2220 2f3e 0a20  den-widget" />. 
+00007550: 2020 203c 2f64 6976 3e0a 2020 2020 3c64     </div>.    <d
+00007560: 6976 2063 6c61 7373 3d22 6163 7469 6f6e  iv class="action
+00007570: 223e 0a20 2020 2020 203c 696e 7075 7420  ">.      <input 
+00007580: 7479 7065 3d22 7375 626d 6974 220a 2020  type="submit".  
+00007590: 2020 2020 2020 2069 643d 2266 6f72 6d2d         id="form-
+000075a0: 6275 7474 6f6e 732d 6170 706c 7922 0a20  buttons-apply". 
+000075b0: 2020 2020 2020 2020 6e61 6d65 3d22 666f          name="fo
+000075c0: 726d 2e62 7574 746f 6e73 2e61 7070 6c79  rm.buttons.apply
+000075d0: 220a 2020 2020 2020 2020 2063 6c61 7373  ".         class
+000075e0: 3d22 7375 626d 6974 2d77 6964 6765 7420  ="submit-widget 
+000075f0: 6275 7474 6f6e 2d66 6965 6c64 220a 2020  button-field".  
+00007600: 2020 2020 2020 2076 616c 7565 3d22 4170         value="Ap
+00007610: 706c 7922 202f 3e0a 2020 2020 3c2f 6469  ply" />.    </di
+00007620: 763e 0a20 203c 2f66 6f72 6d3e 0a0a 0a45  v>.  </form>...E
+00007630: 6469 7466 6f72 6d73 206d 6967 6874 2075  ditforms might u
+00007640: 7365 2064 6963 7473 2061 7320 636f 6e74  se dicts as cont
+00007650: 6578 743a 0a0a 2020 3e3e 3e20 6e65 7773  ext:..  >>> news
+00007660: 7562 203d 204d 7953 7562 4f62 6a65 6374  ub = MySubObject
+00007670: 2829 0a20 203e 3e3e 206e 6577 7375 622e  ().  >>> newsub.
+00007680: 666f 6f66 6965 6c64 203d 2037 380a 2020  foofield = 78.  
+00007690: 3e3e 3e20 6e65 7773 7562 2e62 6172 6669  >>> newsub.barfi
+000076a0: 656c 6420 3d20 3837 0a0a 2020 3e3e 3e20  eld = 87..  >>> 
+000076b0: 636c 6173 7320 4d79 4564 6974 466f 726d  class MyEditForm
+000076c0: 4469 6374 2866 6f72 6d2e 4564 6974 466f  Dict(form.EditFo
+000076d0: 726d 293a 0a20 202e 2e2e 2020 2020 2066  rm):.  ...     f
+000076e0: 6965 6c64 7320 3d20 6669 656c 642e 4669  ields = field.Fi
+000076f0: 656c 6473 2849 4d79 4f62 6a65 6374 290a  elds(IMyObject).
+00007700: 2020 2e2e 2e20 2020 2020 6465 6620 6765    ...     def ge
+00007710: 745f 636f 6e74 656e 7428 7365 6c66 293a  t_content(self):
+00007720: 0a20 202e 2e2e 2020 2020 2020 2020 2072  .  ...         r
+00007730: 6574 7572 6e20 7b27 7375 626f 626a 6563  eturn {'subobjec
+00007740: 7427 3a20 6e65 7773 7562 2c20 276e 616d  t': newsub, 'nam
+00007750: 6527 3a20 2762 6c6f 6f6b 6927 7d0a 0a20  e': 'blooki'}.. 
+00007760: 203e 3e3e 2065 6469 7466 6f72 6d20 3d20   >>> editform = 
+00007770: 4d79 4564 6974 466f 726d 4469 6374 284e  MyEditFormDict(N
+00007780: 6f6e 652c 2054 6573 7452 6571 7565 7374  one, TestRequest
+00007790: 2829 290a 2020 3e3e 3e20 6164 6454 656d  ()).  >>> addTem
+000077a0: 706c 6174 6528 6564 6974 666f 726d 290a  plate(editform).
+000077b0: 2020 3e3e 3e20 6564 6974 666f 726d 2e75    >>> editform.u
+000077c0: 7064 6174 6528 290a 0a57 6174 6368 2066  pdate()..Watch f
+000077d0: 6f72 2074 6865 2077 6964 6765 7420 7661  or the widget va
+000077e0: 6c75 6573 2069 6e20 7468 6520 4854 4d4c  lues in the HTML
+000077f0: 3a0a 0a20 203e 3e3e 2070 7269 6e74 2866  :..  >>> print(f
+00007800: 6f72 6d61 745f 6874 6d6c 2865 6469 7466  ormat_html(editf
+00007810: 6f72 6d2e 7265 6e64 6572 2829 2929 0a20  orm.render())). 
+00007820: 203c 666f 726d 2061 6374 696f 6e3d 222e   <form action=".
+00007830: 223e 0a20 2020 203c 6469 7620 636c 6173  ">.    <div clas
+00007840: 733d 2272 6f77 223e 0a20 2020 2020 203c  s="row">.      <
+00007850: 6c61 6265 6c20 666f 723d 2266 6f72 6d2d  label for="form-
+00007860: 7769 6467 6574 732d 7375 626f 626a 6563  widgets-subobjec
+00007870: 7422 3e6d 7920 6f62 6a65 6374 3c2f 6c61  t">my object</la
+00007880: 6265 6c3e 0a20 2020 2020 203c 6469 7620  bel>.      <div 
+00007890: 636c 6173 733d 226f 626a 6563 742d 7769  class="object-wi
+000078a0: 6467 6574 2072 6571 7569 7265 6422 3e0a  dget required">.
+000078b0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+000078c0: 6976 2063 6c61 7373 3d22 6c61 6265 6c22  iv class="label"
+000078d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000078e0: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
+000078f0: 6f72 3d22 666f 726d 2d77 6964 6765 7473  or="form-widgets
+00007900: 2d73 7562 6f62 6a65 6374 2d77 6964 6765  -subobject-widge
+00007910: 7473 2d66 6f6f 6669 656c 6422 3e0a 2020  ts-foofield">.  
 00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007930: 2020 203c 7370 616e 3e4d 7920 666f 6f20     <span>My foo 
-00007940: 6669 656c 643c 2f73 7061 6e3e 0a20 2020  field</span>.   
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2020 2020 2020 2020 2020 203c 7370 616e             <span
-00007970: 2063 6c61 7373 3d22 7265 7175 6972 6564   class="required
-00007980: 223e 2a3c 2f73 7061 6e3e 0a20 2020 2020  ">*</span>.     
-00007990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079a0: 203c 2f6c 6162 656c 3e0a 2020 2020 2020   </label>.      
-000079b0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-000079c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000079d0: 7620 636c 6173 733d 2277 6964 6765 7422  v class="widget"
-000079e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000079f0: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
-00007a00: 7970 653d 2274 6578 7422 0a20 2020 2020  ype="text".     
-00007a10: 2020 2020 6964 3d22 666f 726d 2d77 6964      id="form-wid
-00007a20: 6765 7473 2d73 7562 6f62 6a65 6374 2d77  gets-subobject-w
-00007a30: 6964 6765 7473 2d66 6f6f 6669 656c 6422  idgets-foofield"
-00007a40: 0a20 2020 2020 2020 2020 6e61 6d65 3d22  .         name="
-00007a50: 666f 726d 2e77 6964 6765 7473 2e73 7562  form.widgets.sub
-00007a60: 6f62 6a65 6374 2e77 6964 6765 7473 2e66  object.widgets.f
-00007a70: 6f6f 6669 656c 6422 0a20 2020 2020 2020  oofield".       
-00007a80: 2020 636c 6173 733d 2274 6578 742d 7769    class="text-wi
-00007a90: 6467 6574 2072 6571 7569 7265 6420 696e  dget required in
-00007aa0: 742d 6669 656c 6422 0a20 2020 2020 2020  t-field".       
-00007ab0: 2020 7661 6c75 653d 2237 3822 202f 3e0a    value="78" />.
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00007ad0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00007ae0: 2020 203c 6469 7620 636c 6173 733d 226c     <div class="l
-00007af0: 6162 656c 223e 0a20 2020 2020 2020 2020  abel">.         
-00007b00: 2020 2020 2020 2020 2020 2020 203c 6c61               <la
-00007b10: 6265 6c20 666f 723d 2266 6f72 6d2d 7769  bel for="form-wi
-00007b20: 6467 6574 732d 7375 626f 626a 6563 742d  dgets-subobject-
-00007b30: 7769 6467 6574 732d 6261 7266 6965 6c64  widgets-barfield
-00007b40: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00007930: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
+00007940: 6e3e 4d79 2066 6f6f 2066 6965 6c64 3c2f  n>My foo field</
+00007950: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
+00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007970: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+00007980: 2272 6571 7569 7265 6422 3e2a 3c2f 7370  "required">*</sp
+00007990: 616e 3e0a 2020 2020 2020 2020 2020 2020  an>.            
+000079a0: 2020 2020 2020 2020 2020 3c2f 6c61 6265            </labe
+000079b0: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
+000079c0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+000079d0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000079e0: 3d22 7769 6467 6574 223e 0a20 2020 2020  ="widget">.     
+000079f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a00: 203c 696e 7075 7420 7479 7065 3d22 7465   <input type="te
+00007a10: 7874 220a 2020 2020 2020 2020 2069 643d  xt".         id=
+00007a20: 2266 6f72 6d2d 7769 6467 6574 732d 7375  "form-widgets-su
+00007a30: 626f 626a 6563 742d 7769 6467 6574 732d  bobject-widgets-
+00007a40: 666f 6f66 6965 6c64 220a 2020 2020 2020  foofield".      
+00007a50: 2020 206e 616d 653d 2266 6f72 6d2e 7769     name="form.wi
+00007a60: 6467 6574 732e 7375 626f 626a 6563 742e  dgets.subobject.
+00007a70: 7769 6467 6574 732e 666f 6f66 6965 6c64  widgets.foofield
+00007a80: 220a 2020 2020 2020 2020 2063 6c61 7373  ".         class
+00007a90: 3d22 7465 7874 2d77 6964 6765 7420 7265  ="text-widget re
+00007aa0: 7175 6972 6564 2069 6e74 2d66 6965 6c64  quired int-field
+00007ab0: 220a 2020 2020 2020 2020 2076 616c 7565  ".         value
+00007ac0: 3d22 3738 2220 2f3e 0a20 2020 2020 2020  ="78" />.       
+00007ad0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00007ae0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00007af0: 2063 6c61 7373 3d22 6c61 6265 6c22 3e0a   class="label">.
+00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b10: 2020 2020 2020 3c6c 6162 656c 2066 6f72        <label for
+00007b20: 3d22 666f 726d 2d77 6964 6765 7473 2d73  ="form-widgets-s
+00007b30: 7562 6f62 6a65 6374 2d77 6964 6765 7473  ubobject-widgets
+00007b40: 2d62 6172 6669 656c 6422 3e0a 2020 2020  -barfield">.    
 00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b60: 203c 7370 616e 3e4d 7920 6465 6172 2062   <span>My dear b
-00007b70: 6172 3c2f 7370 616e 3e0a 2020 2020 2020  ar</span>.      
-00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b90: 3c2f 6c61 6265 6c3e 0a20 2020 2020 2020  </label>.       
-00007ba0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00007bb0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00007bc0: 2063 6c61 7373 3d22 7769 6467 6574 223e   class="widget">
-00007bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007be0: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
-00007bf0: 7065 3d22 7465 7874 220a 2020 2020 2020  pe="text".      
-00007c00: 2020 2069 643d 2266 6f72 6d2d 7769 6467     id="form-widg
-00007c10: 6574 732d 7375 626f 626a 6563 742d 7769  ets-subobject-wi
-00007c20: 6467 6574 732d 6261 7266 6965 6c64 220a  dgets-barfield".
-00007c30: 2020 2020 2020 2020 206e 616d 653d 2266           name="f
-00007c40: 6f72 6d2e 7769 6467 6574 732e 7375 626f  orm.widgets.subo
-00007c50: 626a 6563 742e 7769 6467 6574 732e 6261  bject.widgets.ba
-00007c60: 7266 6965 6c64 220a 2020 2020 2020 2020  rfield".        
-00007c70: 2063 6c61 7373 3d22 7465 7874 2d77 6964   class="text-wid
-00007c80: 6765 7420 696e 742d 6669 656c 6422 0a20  get int-field". 
-00007c90: 2020 2020 2020 2020 7661 6c75 653d 2238          value="8
-00007ca0: 3722 202f 3e0a 2020 2020 2020 2020 2020  7" />.          
-00007cb0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00007cc0: 203c 696e 7075 7420 6e61 6d65 3d22 666f   <input name="fo
-00007cd0: 726d 2e77 6964 6765 7473 2e73 7562 6f62  rm.widgets.subob
-00007ce0: 6a65 6374 2d65 6d70 7479 2d6d 6172 6b65  ject-empty-marke
-00007cf0: 7222 2074 7970 653d 2268 6964 6465 6e22  r" type="hidden"
-00007d00: 2076 616c 7565 3d22 3122 2f3e 0a20 203c   value="1"/>.  <
-00007d10: 2f64 6976 3e0a 2020 2020 3c2f 6469 763e  /div>.    </div>
-00007d20: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
-00007d30: 2272 6f77 223e 0a20 2020 2020 203c 6c61  "row">.      <la
-00007d40: 6265 6c20 666f 723d 2266 6f72 6d2d 7769  bel for="form-wi
-00007d50: 6467 6574 732d 6e61 6d65 223e 6e61 6d65  dgets-name">name
-00007d60: 3c2f 6c61 6265 6c3e 0a20 2020 2020 203c  </label>.      <
-00007d70: 696e 7075 7420 7479 7065 3d22 7465 7874  input type="text
-00007d80: 220a 2020 2020 2020 2020 2069 643d 2266  ".         id="f
-00007d90: 6f72 6d2d 7769 6467 6574 732d 6e61 6d65  orm-widgets-name
-00007da0: 220a 2020 2020 2020 2020 206e 616d 653d  ".         name=
-00007db0: 2266 6f72 6d2e 7769 6467 6574 732e 6e61  "form.widgets.na
-00007dc0: 6d65 220a 2020 2020 2020 2020 2063 6c61  me".         cla
-00007dd0: 7373 3d22 7465 7874 2d77 6964 6765 7420  ss="text-widget 
-00007de0: 7265 7175 6972 6564 2074 6578 746c 696e  required textlin
-00007df0: 652d 6669 656c 6422 0a20 2020 2020 2020  e-field".       
-00007e00: 2020 7661 6c75 653d 2262 6c6f 6f6b 6922    value="blooki"
-00007e10: 202f 3e0a 2020 2020 3c2f 6469 763e 0a20   />.    </div>. 
-00007e20: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
-00007e30: 6374 696f 6e22 3e0a 2020 2020 2020 3c69  ction">.      <i
-00007e40: 6e70 7574 2074 7970 653d 2273 7562 6d69  nput type="submi
-00007e50: 7422 0a20 2020 2020 2020 2020 6964 3d22  t".         id="
-00007e60: 666f 726d 2d62 7574 746f 6e73 2d61 7070  form-buttons-app
-00007e70: 6c79 220a 2020 2020 2020 2020 206e 616d  ly".         nam
-00007e80: 653d 2266 6f72 6d2e 6275 7474 6f6e 732e  e="form.buttons.
-00007e90: 6170 706c 7922 0a20 2020 2020 2020 2020  apply".         
-00007ea0: 636c 6173 733d 2273 7562 6d69 742d 7769  class="submit-wi
-00007eb0: 6467 6574 2062 7574 746f 6e2d 6669 656c  dget button-fiel
-00007ec0: 6422 0a20 2020 2020 2020 2020 7661 6c75  d".         valu
-00007ed0: 653d 2241 7070 6c79 2220 2f3e 0a20 2020  e="Apply" />.   
-00007ee0: 203c 2f64 6976 3e0a 2020 3c2f 666f 726d   </div>.  </form
-00007ef0: 3e0a 0a4c 6574 2773 206d 6f64 6966 7920  >..Let's modify 
-00007f00: 7468 6520 7661 6c75 6573 3a0a 0a20 203e  the values:..  >
-00007f10: 3e3e 2072 6571 7565 7374 203d 2054 6573  >> request = Tes
-00007f20: 7452 6571 7565 7374 2870 6172 616d 733d  tRequest(params=
-00007f30: 7b0a 2020 2e2e 2e20 2020 2020 2766 6f72  {.  ...     'for
-00007f40: 6d2e 7769 6467 6574 732e 7375 626f 626a  m.widgets.subobj
-00007f50: 6563 742e 7769 6467 6574 732e 666f 6f66  ect.widgets.foof
-00007f60: 6965 6c64 273a 2734 3327 2c0a 2020 2e2e  ield':'43',.  ..
-00007f70: 2e20 2020 2020 2766 6f72 6d2e 7769 6467  .     'form.widg
-00007f80: 6574 732e 7375 626f 626a 6563 742e 7769  ets.subobject.wi
-00007f90: 6467 6574 732e 6261 7266 6965 6c64 273a  dgets.barfield':
-00007fa0: 2735 3527 2c0a 2020 2e2e 2e20 2020 2020  '55',.  ...     
-00007fb0: 2766 6f72 6d2e 7769 6467 6574 732e 6e61  'form.widgets.na
-00007fc0: 6d65 273a 2766 6972 7374 272c 0a20 202e  me':'first',.  .
-00007fd0: 2e2e 2020 2020 2027 666f 726d 2e77 6964  ..     'form.wid
-00007fe0: 6765 7473 2e73 7562 6f62 6a65 6374 2d65  gets.subobject-e
-00007ff0: 6d70 7479 2d6d 6172 6b65 7227 3a27 3127  mpty-marker':'1'
-00008000: 2c0a 2020 2e2e 2e20 2020 2020 2766 6f72  ,.  ...     'for
-00008010: 6d2e 6275 7474 6f6e 732e 6170 706c 7927  m.buttons.apply'
-00008020: 3a27 4170 706c 7927 7d29 0a0a 5468 6579  :'Apply'})..They
-00008030: 2061 7265 2073 7469 6c6c 2074 6865 2073   are still the s
-00008040: 616d 653a 0a0a 2020 3e3e 3e20 6e65 7773  ame:..  >>> news
-00008050: 7562 2e66 6f6f 6669 656c 640a 2020 3738  ub.foofield.  78
-00008060: 0a20 203e 3e3e 206e 6577 7375 622e 6261  .  >>> newsub.ba
-00008070: 7266 6965 6c64 0a20 2038 370a 0a55 6e74  rfield.  87..Unt
-00008080: 696c 2075 7064 6174 696e 6720 7468 6520  il updating the 
-00008090: 666f 726d 3a0a 0a20 203e 3e3e 2065 6469  form:..  >>> edi
-000080a0: 7466 6f72 6d2e 7265 7175 6573 7420 3d20  tform.request = 
-000080b0: 7265 7175 6573 740a 2020 3e3e 3e20 6576  request.  >>> ev
-000080c0: 656e 746c 6f67 3d5b 5d0a 0a20 203e 3e3e  entlog=[]..  >>>
-000080d0: 2065 6469 7466 6f72 6d2e 7570 6461 7465   editform.update
-000080e0: 2829 0a0a 2020 3e3e 3e20 6e65 7773 7562  ()..  >>> newsub
-000080f0: 2e66 6f6f 6669 656c 640a 2020 3433 0a20  .foofield.  43. 
-00008100: 203e 3e3e 206e 6577 7375 622e 6261 7266   >>> newsub.barf
-00008110: 6965 6c64 0a20 2035 350a 0a20 203e 3e3e  ield.  55..  >>>
-00008120: 206c 656e 2865 7665 6e74 6c6f 6729 0a20   len(eventlog). 
-00008130: 2032 0a20 203e 3e3e 2070 7269 6e74 4576   2.  >>> printEv
-00008140: 656e 7473 2829 0a20 203c 7a6f 7065 2e2e  ents().  <zope..
-00008150: 2e4f 626a 6563 744d 6f64 6966 6965 6445  .ObjectModifiedE
-00008160: 7665 6e74 206f 626a 6563 7420 6174 202e  vent object at .
-00008170: 2e2e 3e0a 2020 7079 616d 735f 666f 726d  ..>.  pyams_form
-00008180: 2e74 6573 7469 6e67 2e49 4d79 5375 624f  .testing.IMySubO
-00008190: 626a 6563 740a 2020 5b27 6261 7266 6965  bject.  ['barfie
-000081a0: 6c64 272c 2027 666f 6f66 6965 6c64 275d  ld', 'foofield']
-000081b0: 0a20 203c 7a6f 7065 2e2e 2e4f 626a 6563  .  <zope...Objec
-000081c0: 744d 6f64 6966 6965 6445 7665 6e74 206f  tModifiedEvent o
-000081d0: 626a 6563 7420 6174 202e 2e2e 3e0a 2020  bject at ...>.  
-000081e0: 7079 616d 735f 666f 726d 2e74 6573 7469  pyams_form.testi
-000081f0: 6e67 2e49 4d79 4f62 6a65 6374 0a20 205b  ng.IMyObject.  [
-00008200: 276e 616d 6527 2c20 2773 7562 6f62 6a65  'name', 'subobje
-00008210: 6374 275d 0a0a 0a4f 626a 6563 7420 696e  ct']...Object in
-00008220: 2061 6e20 4f62 6a65 6374 2073 6974 7561   an Object situa
-00008230: 7469 6f6e 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  tion.===========
+00007b60: 2020 2020 2020 2020 2020 3c73 7061 6e3e            <span>
+00007b70: 4d79 2064 6561 7220 6261 723c 2f73 7061  My dear bar</spa
+00007b80: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00007b90: 2020 2020 2020 2020 203c 2f6c 6162 656c           </label
+00007ba0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00007bb0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00007bc0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00007bd0: 2277 6964 6765 7422 3e0a 2020 2020 2020  "widget">.      
+00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bf0: 3c69 6e70 7574 2074 7970 653d 2274 6578  <input type="tex
+00007c00: 7422 0a20 2020 2020 2020 2020 6964 3d22  t".         id="
+00007c10: 666f 726d 2d77 6964 6765 7473 2d73 7562  form-widgets-sub
+00007c20: 6f62 6a65 6374 2d77 6964 6765 7473 2d62  object-widgets-b
+00007c30: 6172 6669 656c 6422 0a20 2020 2020 2020  arfield".       
+00007c40: 2020 6e61 6d65 3d22 666f 726d 2e77 6964    name="form.wid
+00007c50: 6765 7473 2e73 7562 6f62 6a65 6374 2e77  gets.subobject.w
+00007c60: 6964 6765 7473 2e62 6172 6669 656c 6422  idgets.barfield"
+00007c70: 0a20 2020 2020 2020 2020 636c 6173 733d  .         class=
+00007c80: 2274 6578 742d 7769 6467 6574 2069 6e74  "text-widget int
+00007c90: 2d66 6965 6c64 220a 2020 2020 2020 2020  -field".        
+00007ca0: 2076 616c 7565 3d22 3837 2220 2f3e 0a20   value="87" />. 
+00007cb0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00007cc0: 6976 3e0a 2020 2020 2020 3c69 6e70 7574  iv>.      <input
+00007cd0: 206e 616d 653d 2266 6f72 6d2e 7769 6467   name="form.widg
+00007ce0: 6574 732e 7375 626f 626a 6563 742d 656d  ets.subobject-em
+00007cf0: 7074 792d 6d61 726b 6572 2220 7479 7065  pty-marker" type
+00007d00: 3d22 6869 6464 656e 2220 7661 6c75 653d  ="hidden" value=
+00007d10: 2231 2220 2f3e 0a20 203c 2f64 6976 3e0a  "1" />.  </div>.
+00007d20: 2020 2020 3c2f 6469 763e 0a20 2020 203c      </div>.    <
+00007d30: 6469 7620 636c 6173 733d 2272 6f77 223e  div class="row">
+00007d40: 0a20 2020 2020 203c 6c61 6265 6c20 666f  .      <label fo
+00007d50: 723d 2266 6f72 6d2d 7769 6467 6574 732d  r="form-widgets-
+00007d60: 6e61 6d65 223e 6e61 6d65 3c2f 6c61 6265  name">name</labe
+00007d70: 6c3e 0a20 2020 2020 203c 696e 7075 7420  l>.      <input 
+00007d80: 7479 7065 3d22 7465 7874 220a 2020 2020  type="text".    
+00007d90: 2020 2020 2069 643d 2266 6f72 6d2d 7769       id="form-wi
+00007da0: 6467 6574 732d 6e61 6d65 220a 2020 2020  dgets-name".    
+00007db0: 2020 2020 206e 616d 653d 2266 6f72 6d2e       name="form.
+00007dc0: 7769 6467 6574 732e 6e61 6d65 220a 2020  widgets.name".  
+00007dd0: 2020 2020 2020 2063 6c61 7373 3d22 7465         class="te
+00007de0: 7874 2d77 6964 6765 7420 7265 7175 6972  xt-widget requir
+00007df0: 6564 2074 6578 746c 696e 652d 6669 656c  ed textline-fiel
+00007e00: 6422 0a20 2020 2020 2020 2020 7661 6c75  d".         valu
+00007e10: 653d 2262 6c6f 6f6b 6922 202f 3e0a 2020  e="blooki" />.  
+00007e20: 2020 3c2f 6469 763e 0a20 2020 203c 6469    </div>.    <di
+00007e30: 7620 636c 6173 733d 2261 6374 696f 6e22  v class="action"
+00007e40: 3e0a 2020 2020 2020 3c69 6e70 7574 2074  >.      <input t
+00007e50: 7970 653d 2273 7562 6d69 7422 0a20 2020  ype="submit".   
+00007e60: 2020 2020 2020 6964 3d22 666f 726d 2d62        id="form-b
+00007e70: 7574 746f 6e73 2d61 7070 6c79 220a 2020  uttons-apply".  
+00007e80: 2020 2020 2020 206e 616d 653d 2266 6f72         name="for
+00007e90: 6d2e 6275 7474 6f6e 732e 6170 706c 7922  m.buttons.apply"
+00007ea0: 0a20 2020 2020 2020 2020 636c 6173 733d  .         class=
+00007eb0: 2273 7562 6d69 742d 7769 6467 6574 2062  "submit-widget b
+00007ec0: 7574 746f 6e2d 6669 656c 6422 0a20 2020  utton-field".   
+00007ed0: 2020 2020 2020 7661 6c75 653d 2241 7070        value="App
+00007ee0: 6c79 2220 2f3e 0a20 2020 203c 2f64 6976  ly" />.    </div
+00007ef0: 3e0a 2020 3c2f 666f 726d 3e0a 0a4c 6574  >.  </form>..Let
+00007f00: 2773 206d 6f64 6966 7920 7468 6520 7661  's modify the va
+00007f10: 6c75 6573 3a0a 0a20 203e 3e3e 2072 6571  lues:..  >>> req
+00007f20: 7565 7374 203d 2054 6573 7452 6571 7565  uest = TestReque
+00007f30: 7374 2870 6172 616d 733d 7b0a 2020 2e2e  st(params={.  ..
+00007f40: 2e20 2020 2020 2766 6f72 6d2e 7769 6467  .     'form.widg
+00007f50: 6574 732e 7375 626f 626a 6563 742e 7769  ets.subobject.wi
+00007f60: 6467 6574 732e 666f 6f66 6965 6c64 273a  dgets.foofield':
+00007f70: 2734 3327 2c0a 2020 2e2e 2e20 2020 2020  '43',.  ...     
+00007f80: 2766 6f72 6d2e 7769 6467 6574 732e 7375  'form.widgets.su
+00007f90: 626f 626a 6563 742e 7769 6467 6574 732e  bobject.widgets.
+00007fa0: 6261 7266 6965 6c64 273a 2735 3527 2c0a  barfield':'55',.
+00007fb0: 2020 2e2e 2e20 2020 2020 2766 6f72 6d2e    ...     'form.
+00007fc0: 7769 6467 6574 732e 6e61 6d65 273a 2766  widgets.name':'f
+00007fd0: 6972 7374 272c 0a20 202e 2e2e 2020 2020  irst',.  ...    
+00007fe0: 2027 666f 726d 2e77 6964 6765 7473 2e73   'form.widgets.s
+00007ff0: 7562 6f62 6a65 6374 2d65 6d70 7479 2d6d  ubobject-empty-m
+00008000: 6172 6b65 7227 3a27 3127 2c0a 2020 2e2e  arker':'1',.  ..
+00008010: 2e20 2020 2020 2766 6f72 6d2e 6275 7474  .     'form.butt
+00008020: 6f6e 732e 6170 706c 7927 3a27 4170 706c  ons.apply':'Appl
+00008030: 7927 7d29 0a0a 5468 6579 2061 7265 2073  y'})..They are s
+00008040: 7469 6c6c 2074 6865 2073 616d 653a 0a0a  till the same:..
+00008050: 2020 3e3e 3e20 6e65 7773 7562 2e66 6f6f    >>> newsub.foo
+00008060: 6669 656c 640a 2020 3738 0a20 203e 3e3e  field.  78.  >>>
+00008070: 206e 6577 7375 622e 6261 7266 6965 6c64   newsub.barfield
+00008080: 0a20 2038 370a 0a55 6e74 696c 2075 7064  .  87..Until upd
+00008090: 6174 696e 6720 7468 6520 666f 726d 3a0a  ating the form:.
+000080a0: 0a20 203e 3e3e 2065 6469 7466 6f72 6d2e  .  >>> editform.
+000080b0: 7265 7175 6573 7420 3d20 7265 7175 6573  request = reques
+000080c0: 740a 2020 3e3e 3e20 6576 656e 746c 6f67  t.  >>> eventlog
+000080d0: 3d5b 5d0a 0a20 203e 3e3e 2065 6469 7466  =[]..  >>> editf
+000080e0: 6f72 6d2e 7570 6461 7465 2829 0a0a 2020  orm.update()..  
+000080f0: 3e3e 3e20 6e65 7773 7562 2e66 6f6f 6669  >>> newsub.foofi
+00008100: 656c 640a 2020 3433 0a20 203e 3e3e 206e  eld.  43.  >>> n
+00008110: 6577 7375 622e 6261 7266 6965 6c64 0a20  ewsub.barfield. 
+00008120: 2035 350a 0a20 203e 3e3e 206c 656e 2865   55..  >>> len(e
+00008130: 7665 6e74 6c6f 6729 0a20 2032 0a20 203e  ventlog).  2.  >
+00008140: 3e3e 2070 7269 6e74 4576 656e 7473 2829  >> printEvents()
+00008150: 0a20 203c 7a6f 7065 2e2e 2e4f 626a 6563  .  <zope...Objec
+00008160: 744d 6f64 6966 6965 6445 7665 6e74 206f  tModifiedEvent o
+00008170: 626a 6563 7420 6174 202e 2e2e 3e0a 2020  bject at ...>.  
+00008180: 7079 616d 735f 666f 726d 2e74 6573 7469  pyams_form.testi
+00008190: 6e67 2e49 4d79 5375 624f 626a 6563 740a  ng.IMySubObject.
+000081a0: 2020 5b27 6261 7266 6965 6c64 272c 2027    ['barfield', '
+000081b0: 666f 6f66 6965 6c64 275d 0a20 203c 7a6f  foofield'].  <zo
+000081c0: 7065 2e2e 2e4f 626a 6563 744d 6f64 6966  pe...ObjectModif
+000081d0: 6965 6445 7665 6e74 206f 626a 6563 7420  iedEvent object 
+000081e0: 6174 202e 2e2e 3e0a 2020 7079 616d 735f  at ...>.  pyams_
+000081f0: 666f 726d 2e74 6573 7469 6e67 2e49 4d79  form.testing.IMy
+00008200: 4f62 6a65 6374 0a20 205b 276e 616d 6527  Object.  ['name'
+00008210: 2c20 2773 7562 6f62 6a65 6374 275d 0a0a  , 'subobject']..
+00008220: 0a4f 626a 6563 7420 696e 2061 6e20 4f62  .Object in an Ob
+00008230: 6a65 6374 2073 6974 7561 7469 6f6e 0a3d  ject situation.=
 00008240: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00008250: 3d3d 0a0a 0a57 6520 6465 6669 6e65 2061  ==...We define a
-00008260: 6e20 696e 7465 7266 6163 6520 636f 6e74  n interface cont
-00008270: 6169 6e69 6e67 2061 2073 7562 6f62 6a65  aining a subobje
-00008280: 6374 2c20 616e 6420 616e 2061 6464 666f  ct, and an addfo
-00008290: 726d 2066 6f72 2069 743a 0a0a 2020 3e3e  rm for it:..  >>
-000082a0: 3e20 6672 6f6d 2070 7961 6d73 5f66 6f72  > from pyams_for
-000082b0: 6d20 696d 706f 7274 2066 6f72 6d2c 2066  m import form, f
-000082c0: 6965 6c64 0a20 203e 3e3e 2066 726f 6d20  ield.  >>> from 
-000082d0: 7079 616d 735f 666f 726d 2e74 6573 7469  pyams_form.testi
-000082e0: 6e67 2069 6d70 6f72 7420 494d 7943 6f6d  ng import IMyCom
-000082f0: 706c 6578 4f62 6a65 6374 0a0a 4e6f 7465  plexObject..Note
-00008300: 2c20 7468 6174 2063 7265 6174 696e 6720  , that creating 
-00008310: 616e 206f 626a 6563 7420 7769 6c6c 2070  an object will p
-00008320: 7269 6e74 2073 6f6d 6520 696e 666f 726d  rint some inform
-00008330: 6174 696f 6e20 6162 6f75 7420 6974 3a0a  ation about it:.
-00008340: 0a20 203e 3e3e 2063 6c61 7373 204d 7941  .  >>> class MyA
-00008350: 6464 466f 726d 2866 6f72 6d2e 4164 6446  ddForm(form.AddF
-00008360: 6f72 6d29 3a0a 2020 2e2e 2e20 2020 2020  orm):.  ...     
-00008370: 6669 656c 6473 203d 2066 6965 6c64 2e46  fields = field.F
-00008380: 6965 6c64 7328 494d 7943 6f6d 706c 6578  ields(IMyComplex
-00008390: 4f62 6a65 6374 290a 2020 2e2e 2e20 2020  Object).  ...   
-000083a0: 2020 6465 6620 6372 6561 7465 2873 656c    def create(sel
-000083b0: 662c 2064 6174 6129 3a0a 2020 2e2e 2e20  f, data):.  ... 
-000083c0: 2020 2020 2020 2020 7072 696e 7428 224d          print("M
-000083d0: 7941 6464 466f 726d 2e63 7265 6174 6522  yAddForm.create"
-000083e0: 2c20 7374 7228 6461 7461 2929 0a20 202e  , str(data)).  .
-000083f0: 2e2e 2020 2020 2020 2020 2072 6574 7572  ..         retur
-00008400: 6e20 4d79 4f62 6a65 6374 282a 2a64 6174  n MyObject(**dat
-00008410: 6129 0a20 202e 2e2e 2020 2020 2064 6566  a).  ...     def
-00008420: 2061 6464 2873 656c 662c 206f 626a 293a   add(self, obj):
-00008430: 0a20 202e 2e2e 2020 2020 2020 2020 2073  .  ...         s
-00008440: 656c 662e 636f 6e74 6578 745b 6f62 6a2e  elf.context[obj.
-00008450: 6e61 6d65 5d20 3d20 6f62 6a0a 2020 2e2e  name] = obj.  ..
-00008460: 2e20 2020 2020 6465 6620 6e65 7874 5f75  .     def next_u
-00008470: 726c 2873 656c 6629 3a0a 2020 2e2e 2e20  rl(self):.  ... 
-00008480: 2020 2020 2020 2020 7061 7373 0a0a 5765          pass..We
-00008490: 2063 7265 6174 6520 7468 6520 666f 726d   create the form
-000084a0: 2061 6e64 2074 7279 2074 6f20 7570 6461   and try to upda
-000084b0: 7465 2069 743a 0a0a 2020 3e3e 3e20 7265  te it:..  >>> re
-000084c0: 7175 6573 7420 3d20 5465 7374 5265 7175  quest = TestRequ
-000084d0: 6573 7428 290a 0a20 203e 3e3e 206d 7961  est()..  >>> mya
-000084e0: 6464 666f 726d 203d 2020 4d79 4164 6446  ddform =  MyAddF
-000084f0: 6f72 6d28 726f 6f74 2c20 7265 7175 6573  orm(root, reques
-00008500: 7429 0a0a 2020 3e3e 3e20 6d79 6164 6466  t)..  >>> myaddf
-00008510: 6f72 6d2e 7570 6461 7465 2829 0a0a 4173  orm.update()..As
-00008520: 2075 7375 616c 2c20 7468 6520 666f 726d   usual, the form
-00008530: 2063 6f6e 7461 696e 7320 6120 7769 6467   contains a widg
-00008540: 6574 206d 616e 6167 6572 2077 6974 6820  et manager with 
-00008550: 7468 6520 6578 7065 6374 6564 2077 6964  the expected wid
-00008560: 6765 740a 0a20 203e 3e3e 206c 6973 7428  get..  >>> list(
-00008570: 6d79 6164 6466 6f72 6d2e 7769 6467 6574  myaddform.widget
-00008580: 732e 6b65 7973 2829 290a 2020 5b27 7375  s.keys()).  ['su
-00008590: 626f 626a 6563 7427 2c20 276e 616d 6527  bobject', 'name'
-000085a0: 5d0a 2020 3e3e 3e20 6c69 7374 286d 7961  ].  >>> list(mya
-000085b0: 6464 666f 726d 2e77 6964 6765 7473 2e76  ddform.widgets.v
-000085c0: 616c 7565 7328 2929 0a20 205b 3c4f 626a  alues()).  [<Obj
-000085d0: 6563 7457 6964 6765 7420 2766 6f72 6d2e  ectWidget 'form.
-000085e0: 7769 6467 6574 732e 7375 626f 626a 6563  widgets.subobjec
-000085f0: 7427 3e2c 203c 5465 7874 5769 6467 6574  t'>, <TextWidget
-00008600: 2027 666f 726d 2e77 6964 6765 7473 2e6e   'form.widgets.n
-00008610: 616d 6527 3e5d 0a0a 5468 6520 6164 6466  ame'>]..The addf
-00008620: 6f72 6d20 6861 7320 6f75 7220 4f62 6a65  orm has our Obje
-00008630: 6374 5769 6467 6574 2077 6869 6368 2069  ctWidget which i
-00008640: 6e20 7475 726e 2063 6f6e 7461 696e 7320  n turn contains 
-00008650: 7468 6520 7375 622d 7769 6467 6574 733a  the sub-widgets:
-00008660: 0a0a 2020 3e3e 3e20 6c69 7374 286d 7961  ..  >>> list(mya
-00008670: 6464 666f 726d 2e77 6964 6765 7473 5b27  ddform.widgets['
-00008680: 7375 626f 626a 6563 7427 5d2e 7769 6467  subobject'].widg
-00008690: 6574 732e 6b65 7973 2829 290a 2020 5b27  ets.keys()).  ['
-000086a0: 7375 6266 6965 6c64 272c 2027 6d6f 6f66  subfield', 'moof
-000086b0: 6965 6c64 275d 0a0a 2020 3e3e 3e20 6c69  ield']..  >>> li
-000086c0: 7374 286d 7961 6464 666f 726d 2e77 6964  st(myaddform.wid
-000086d0: 6765 7473 5b27 7375 626f 626a 6563 7427  gets['subobject'
-000086e0: 5d2e 7769 6467 6574 735b 2773 7562 6669  ].widgets['subfi
-000086f0: 656c 6427 5d2e 7769 6467 6574 732e 6b65  eld'].widgets.ke
-00008700: 7973 2829 290a 2020 5b27 666f 6f66 6965  ys()).  ['foofie
-00008710: 6c64 272c 2027 6261 7266 6965 6c64 275d  ld', 'barfield']
-00008720: 0a0a 4966 2077 6520 7761 6e74 2074 6f20  ..If we want to 
-00008730: 7265 6e64 6572 2074 6865 2061 6464 666f  render the addfo
-00008740: 726d 2c20 7765 206d 7573 7420 6769 7665  rm, we must give
-00008750: 2069 7420 6120 7465 6d70 6c61 7465 3a0a   it a template:.
-00008760: 0a20 203e 3e3e 2061 6464 5465 6d70 6c61  .  >>> addTempla
-00008770: 7465 286d 7961 6464 666f 726d 290a 0a4e  te(myaddform)..N
-00008780: 6f77 2072 656e 6465 7269 6e67 2074 6865  ow rendering the
-00008790: 2061 6464 666f 726d 2072 656e 6465 7273   addform renders
-000087a0: 2074 6865 2073 7562 666f 726d 2061 7320   the subform as 
-000087b0: 7765 6c6c 3a0a 0a20 203e 3e3e 2070 7269  well:..  >>> pri
-000087c0: 6e74 2866 6f72 6d61 745f 6874 6d6c 286d  nt(format_html(m
-000087d0: 7961 6464 666f 726d 2e72 656e 6465 7228  yaddform.render(
-000087e0: 2929 290a 2020 3c66 6f72 6d20 6163 7469  ))).  <form acti
-000087f0: 6f6e 3d22 2e22 3e0a 2020 2020 3c64 6976  on=".">.    <div
-00008800: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
-00008810: 2020 2020 3c6c 6162 656c 2066 6f72 3d22      <label for="
-00008820: 666f 726d 2d77 6964 6765 7473 2d73 7562  form-widgets-sub
-00008830: 6f62 6a65 6374 223e 6d79 206f 626a 6563  object">my objec
-00008840: 743c 2f6c 6162 656c 3e0a 2020 2020 2020  t</label>.      
-00008850: 3c64 6976 2063 6c61 7373 3d22 6f62 6a65  <div class="obje
-00008860: 6374 2d77 6964 6765 7420 7265 7175 6972  ct-widget requir
-00008870: 6564 223e 0a20 2020 2020 2020 2020 2020  ed">.           
-00008880: 2020 203c 6469 7620 636c 6173 733d 226c     <div class="l
-00008890: 6162 656c 223e 0a20 2020 2020 2020 2020  abel">.         
-000088a0: 2020 2020 2020 2020 2020 2020 203c 6c61               <la
-000088b0: 6265 6c20 666f 723d 2266 6f72 6d2d 7769  bel for="form-wi
-000088c0: 6467 6574 732d 7375 626f 626a 6563 742d  dgets-subobject-
-000088d0: 7769 6467 6574 732d 7375 6266 6965 6c64  widgets-subfield
-000088e0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00008250: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 0a57  ============...W
+00008260: 6520 6465 6669 6e65 2061 6e20 696e 7465  e define an inte
+00008270: 7266 6163 6520 636f 6e74 6169 6e69 6e67  rface containing
+00008280: 2061 2073 7562 6f62 6a65 6374 2c20 616e   a subobject, an
+00008290: 6420 616e 2061 6464 666f 726d 2066 6f72  d an addform for
+000082a0: 2069 743a 0a0a 2020 3e3e 3e20 6672 6f6d   it:..  >>> from
+000082b0: 2070 7961 6d73 5f66 6f72 6d20 696d 706f   pyams_form impo
+000082c0: 7274 2066 6f72 6d2c 2066 6965 6c64 0a20  rt form, field. 
+000082d0: 203e 3e3e 2066 726f 6d20 7079 616d 735f   >>> from pyams_
+000082e0: 666f 726d 2e74 6573 7469 6e67 2069 6d70  form.testing imp
+000082f0: 6f72 7420 494d 7943 6f6d 706c 6578 4f62  ort IMyComplexOb
+00008300: 6a65 6374 0a0a 4e6f 7465 2c20 7468 6174  ject..Note, that
+00008310: 2063 7265 6174 696e 6720 616e 206f 626a   creating an obj
+00008320: 6563 7420 7769 6c6c 2070 7269 6e74 2073  ect will print s
+00008330: 6f6d 6520 696e 666f 726d 6174 696f 6e20  ome information 
+00008340: 6162 6f75 7420 6974 3a0a 0a20 203e 3e3e  about it:..  >>>
+00008350: 2063 6c61 7373 204d 7941 6464 466f 726d   class MyAddForm
+00008360: 2866 6f72 6d2e 4164 6446 6f72 6d29 3a0a  (form.AddForm):.
+00008370: 2020 2e2e 2e20 2020 2020 6669 656c 6473    ...     fields
+00008380: 203d 2066 6965 6c64 2e46 6965 6c64 7328   = field.Fields(
+00008390: 494d 7943 6f6d 706c 6578 4f62 6a65 6374  IMyComplexObject
+000083a0: 290a 2020 2e2e 2e20 2020 2020 6465 6620  ).  ...     def 
+000083b0: 6372 6561 7465 2873 656c 662c 2064 6174  create(self, dat
+000083c0: 6129 3a0a 2020 2e2e 2e20 2020 2020 2020  a):.  ...       
+000083d0: 2020 7072 696e 7428 224d 7941 6464 466f    print("MyAddFo
+000083e0: 726d 2e63 7265 6174 6522 2c20 7374 7228  rm.create", str(
+000083f0: 6461 7461 2929 0a20 202e 2e2e 2020 2020  data)).  ...    
+00008400: 2020 2020 2072 6574 7572 6e20 4d79 4f62       return MyOb
+00008410: 6a65 6374 282a 2a64 6174 6129 0a20 202e  ject(**data).  .
+00008420: 2e2e 2020 2020 2064 6566 2061 6464 2873  ..     def add(s
+00008430: 656c 662c 206f 626a 293a 0a20 202e 2e2e  elf, obj):.  ...
+00008440: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00008450: 6e74 6578 745b 6f62 6a2e 6e61 6d65 5d20  ntext[obj.name] 
+00008460: 3d20 6f62 6a0a 2020 2e2e 2e20 2020 2020  = obj.  ...     
+00008470: 6465 6620 6e65 7874 5f75 726c 2873 656c  def next_url(sel
+00008480: 6629 3a0a 2020 2e2e 2e20 2020 2020 2020  f):.  ...       
+00008490: 2020 7061 7373 0a0a 5765 2063 7265 6174    pass..We creat
+000084a0: 6520 7468 6520 666f 726d 2061 6e64 2074  e the form and t
+000084b0: 7279 2074 6f20 7570 6461 7465 2069 743a  ry to update it:
+000084c0: 0a0a 2020 3e3e 3e20 7265 7175 6573 7420  ..  >>> request 
+000084d0: 3d20 5465 7374 5265 7175 6573 7428 290a  = TestRequest().
+000084e0: 0a20 203e 3e3e 206d 7961 6464 666f 726d  .  >>> myaddform
+000084f0: 203d 2020 4d79 4164 6446 6f72 6d28 726f   =  MyAddForm(ro
+00008500: 6f74 2c20 7265 7175 6573 7429 0a0a 2020  ot, request)..  
+00008510: 3e3e 3e20 6d79 6164 6466 6f72 6d2e 7570  >>> myaddform.up
+00008520: 6461 7465 2829 0a0a 4173 2075 7375 616c  date()..As usual
+00008530: 2c20 7468 6520 666f 726d 2063 6f6e 7461  , the form conta
+00008540: 696e 7320 6120 7769 6467 6574 206d 616e  ins a widget man
+00008550: 6167 6572 2077 6974 6820 7468 6520 6578  ager with the ex
+00008560: 7065 6374 6564 2077 6964 6765 740a 0a20  pected widget.. 
+00008570: 203e 3e3e 206c 6973 7428 6d79 6164 6466   >>> list(myaddf
+00008580: 6f72 6d2e 7769 6467 6574 732e 6b65 7973  orm.widgets.keys
+00008590: 2829 290a 2020 5b27 7375 626f 626a 6563  ()).  ['subobjec
+000085a0: 7427 2c20 276e 616d 6527 5d0a 2020 3e3e  t', 'name'].  >>
+000085b0: 3e20 6c69 7374 286d 7961 6464 666f 726d  > list(myaddform
+000085c0: 2e77 6964 6765 7473 2e76 616c 7565 7328  .widgets.values(
+000085d0: 2929 0a20 205b 3c4f 626a 6563 7457 6964  )).  [<ObjectWid
+000085e0: 6765 7420 2766 6f72 6d2e 7769 6467 6574  get 'form.widget
+000085f0: 732e 7375 626f 626a 6563 7427 3e2c 203c  s.subobject'>, <
+00008600: 5465 7874 5769 6467 6574 2027 666f 726d  TextWidget 'form
+00008610: 2e77 6964 6765 7473 2e6e 616d 6527 3e5d  .widgets.name'>]
+00008620: 0a0a 5468 6520 6164 6466 6f72 6d20 6861  ..The addform ha
+00008630: 7320 6f75 7220 4f62 6a65 6374 5769 6467  s our ObjectWidg
+00008640: 6574 2077 6869 6368 2069 6e20 7475 726e  et which in turn
+00008650: 2063 6f6e 7461 696e 7320 7468 6520 7375   contains the su
+00008660: 622d 7769 6467 6574 733a 0a0a 2020 3e3e  b-widgets:..  >>
+00008670: 3e20 6c69 7374 286d 7961 6464 666f 726d  > list(myaddform
+00008680: 2e77 6964 6765 7473 5b27 7375 626f 626a  .widgets['subobj
+00008690: 6563 7427 5d2e 7769 6467 6574 732e 6b65  ect'].widgets.ke
+000086a0: 7973 2829 290a 2020 5b27 7375 6266 6965  ys()).  ['subfie
+000086b0: 6c64 272c 2027 6d6f 6f66 6965 6c64 275d  ld', 'moofield']
+000086c0: 0a0a 2020 3e3e 3e20 6c69 7374 286d 7961  ..  >>> list(mya
+000086d0: 6464 666f 726d 2e77 6964 6765 7473 5b27  ddform.widgets['
+000086e0: 7375 626f 626a 6563 7427 5d2e 7769 6467  subobject'].widg
+000086f0: 6574 735b 2773 7562 6669 656c 6427 5d2e  ets['subfield'].
+00008700: 7769 6467 6574 732e 6b65 7973 2829 290a  widgets.keys()).
+00008710: 2020 5b27 666f 6f66 6965 6c64 272c 2027    ['foofield', '
+00008720: 6261 7266 6965 6c64 275d 0a0a 4966 2077  barfield']..If w
+00008730: 6520 7761 6e74 2074 6f20 7265 6e64 6572  e want to render
+00008740: 2074 6865 2061 6464 666f 726d 2c20 7765   the addform, we
+00008750: 206d 7573 7420 6769 7665 2069 7420 6120   must give it a 
+00008760: 7465 6d70 6c61 7465 3a0a 0a20 203e 3e3e  template:..  >>>
+00008770: 2061 6464 5465 6d70 6c61 7465 286d 7961   addTemplate(mya
+00008780: 6464 666f 726d 290a 0a4e 6f77 2072 656e  ddform)..Now ren
+00008790: 6465 7269 6e67 2074 6865 2061 6464 666f  dering the addfo
+000087a0: 726d 2072 656e 6465 7273 2074 6865 2073  rm renders the s
+000087b0: 7562 666f 726d 2061 7320 7765 6c6c 3a0a  ubform as well:.
+000087c0: 0a20 203e 3e3e 2070 7269 6e74 2866 6f72  .  >>> print(for
+000087d0: 6d61 745f 6874 6d6c 286d 7961 6464 666f  mat_html(myaddfo
+000087e0: 726d 2e72 656e 6465 7228 2929 290a 2020  rm.render())).  
+000087f0: 3c66 6f72 6d20 6163 7469 6f6e 3d22 2e22  <form action="."
+00008800: 3e0a 2020 2020 3c64 6976 2063 6c61 7373  >.    <div class
+00008810: 3d22 726f 7722 3e0a 2020 2020 2020 3c6c  ="row">.      <l
+00008820: 6162 656c 2066 6f72 3d22 666f 726d 2d77  abel for="form-w
+00008830: 6964 6765 7473 2d73 7562 6f62 6a65 6374  idgets-subobject
+00008840: 223e 6d79 206f 626a 6563 743c 2f6c 6162  ">my object</lab
+00008850: 656c 3e0a 2020 2020 2020 3c64 6976 2063  el>.      <div c
+00008860: 6c61 7373 3d22 6f62 6a65 6374 2d77 6964  lass="object-wid
+00008870: 6765 7420 7265 7175 6972 6564 223e 0a20  get required">. 
+00008880: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00008890: 7620 636c 6173 733d 226c 6162 656c 223e  v class="label">
+000088a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000088b0: 2020 2020 2020 203c 6c61 6265 6c20 666f         <label fo
+000088c0: 723d 2266 6f72 6d2d 7769 6467 6574 732d  r="form-widgets-
+000088d0: 7375 626f 626a 6563 742d 7769 6467 6574  subobject-widget
+000088e0: 732d 7375 6266 6965 6c64 223e 0a20 2020  s-subfield">.   
 000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008900: 203c 7370 616e 3e53 6563 6f6e 642d 7375   <span>Second-su
-00008910: 626f 626a 6563 743c 2f73 7061 6e3e 0a20  bobject</span>. 
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
-00008940: 616e 2063 6c61 7373 3d22 7265 7175 6972  an class="requir
-00008950: 6564 223e 2a3c 2f73 7061 6e3e 0a20 2020  ed">*</span>.   
-00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008970: 2020 203c 2f6c 6162 656c 3e0a 2020 2020     </label>.    
-00008980: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00008990: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-000089a0: 6469 7620 636c 6173 733d 2277 6964 6765  div class="widge
-000089b0: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-000089c0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-000089d0: 6c61 7373 3d22 6f62 6a65 6374 2d77 6964  lass="object-wid
-000089e0: 6765 7420 7265 7175 6972 6564 223e 0a20  get required">. 
-000089f0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00008a00: 7620 636c 6173 733d 226c 6162 656c 223e  v class="label">
-00008a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008a20: 2020 2020 2020 203c 6c61 6265 6c20 666f         <label fo
-00008a30: 723d 2266 6f72 6d2d 7769 6467 6574 732d  r="form-widgets-
-00008a40: 7375 626f 626a 6563 742d 7769 6467 6574  subobject-widget
-00008a50: 732d 7375 6266 6965 6c64 2d77 6964 6765  s-subfield-widge
-00008a60: 7473 2d66 6f6f 6669 656c 6422 3e0a 2020  ts-foofield">.  
-00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a80: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
-00008a90: 6e3e 4d79 2066 6f6f 2066 6965 6c64 3c2f  n>My foo field</
-00008aa0: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
+00008900: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+00008910: 3e53 6563 6f6e 642d 7375 626f 626a 6563  >Second-subobjec
+00008920: 743c 2f73 7061 6e3e 0a20 2020 2020 2020  t</span>.       
+00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008940: 2020 2020 2020 203c 7370 616e 2063 6c61         <span cla
+00008950: 7373 3d22 7265 7175 6972 6564 223e 2a3c  ss="required">*<
+00008960: 2f73 7061 6e3e 0a20 2020 2020 2020 2020  /span>.         
+00008970: 2020 2020 2020 2020 2020 2020 203c 2f6c               </l
+00008980: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
+00008990: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+000089a0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+000089b0: 6173 733d 2277 6964 6765 7422 3e0a 2020  ass="widget">.  
+000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089d0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000089e0: 6f62 6a65 6374 2d77 6964 6765 7420 7265  object-widget re
+000089f0: 7175 6972 6564 223e 0a20 2020 2020 2020  quired">.       
+00008a00: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00008a10: 733d 226c 6162 656c 223e 0a20 2020 2020  s="label">.     
+00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a30: 203c 6c61 6265 6c20 666f 723d 2266 6f72   <label for="for
+00008a40: 6d2d 7769 6467 6574 732d 7375 626f 626a  m-widgets-subobj
+00008a50: 6563 742d 7769 6467 6574 732d 7375 6266  ect-widgets-subf
+00008a60: 6965 6c64 2d77 6964 6765 7473 2d66 6f6f  ield-widgets-foo
+00008a70: 6669 656c 6422 3e0a 2020 2020 2020 2020  field">.        
+00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a90: 2020 2020 2020 3c73 7061 6e3e 4d79 2066        <span>My f
+00008aa0: 6f6f 2066 6965 6c64 3c2f 7370 616e 3e0a  oo field</span>.
 00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ac0: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
-00008ad0: 2272 6571 7569 7265 6422 3e2a 3c2f 7370  "required">*</sp
-00008ae0: 616e 3e0a 2020 2020 2020 2020 2020 2020  an>.            
-00008af0: 2020 2020 2020 2020 2020 3c2f 6c61 6265            </labe
-00008b00: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
-00008b10: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00008b20: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00008b30: 3d22 7769 6467 6574 223e 0a20 2020 2020  ="widget">.     
-00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b50: 203c 696e 7075 7420 7479 7065 3d22 7465   <input type="te
-00008b60: 7874 220a 2020 2020 2020 2020 2069 643d  xt".         id=
-00008b70: 2266 6f72 6d2d 7769 6467 6574 732d 7375  "form-widgets-su
-00008b80: 626f 626a 6563 742d 7769 6467 6574 732d  bobject-widgets-
-00008b90: 7375 6266 6965 6c64 2d77 6964 6765 7473  subfield-widgets
-00008ba0: 2d66 6f6f 6669 656c 6422 0a20 2020 2020  -foofield".     
-00008bb0: 2020 2020 6e61 6d65 3d22 666f 726d 2e77      name="form.w
-00008bc0: 6964 6765 7473 2e73 7562 6f62 6a65 6374  idgets.subobject
-00008bd0: 2e77 6964 6765 7473 2e73 7562 6669 656c  .widgets.subfiel
-00008be0: 642e 7769 6467 6574 732e 666f 6f66 6965  d.widgets.foofie
-00008bf0: 6c64 220a 2020 2020 2020 2020 2063 6c61  ld".         cla
-00008c00: 7373 3d22 7465 7874 2d77 6964 6765 7420  ss="text-widget 
-00008c10: 7265 7175 6972 6564 2069 6e74 2d66 6965  required int-fie
-00008c20: 6c64 220a 2020 2020 2020 2020 2076 616c  ld".         val
-00008c30: 7565 3d22 312c 3131 3122 202f 3e0a 2020  ue="1,111" />.  
-00008c40: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00008c50: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00008c60: 203c 6469 7620 636c 6173 733d 226c 6162   <div class="lab
-00008c70: 656c 223e 0a20 2020 2020 2020 2020 2020  el">.           
-00008c80: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
-00008c90: 6c20 666f 723d 2266 6f72 6d2d 7769 6467  l for="form-widg
-00008ca0: 6574 732d 7375 626f 626a 6563 742d 7769  ets-subobject-wi
-00008cb0: 6467 6574 732d 7375 6266 6965 6c64 2d77  dgets-subfield-w
-00008cc0: 6964 6765 7473 2d62 6172 6669 656c 6422  idgets-barfield"
-00008cd0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00008ad0: 7061 6e20 636c 6173 733d 2272 6571 7569  pan class="requi
+00008ae0: 7265 6422 3e2a 3c2f 7370 616e 3e0a 2020  red">*</span>.  
+00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b00: 2020 2020 3c2f 6c61 6265 6c3e 0a20 2020      </label>.   
+00008b10: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00008b20: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00008b30: 3c64 6976 2063 6c61 7373 3d22 7769 6467  <div class="widg
+00008b40: 6574 223e 0a20 2020 2020 2020 2020 2020  et">.           
+00008b50: 2020 2020 2020 2020 2020 203c 696e 7075             <inpu
+00008b60: 7420 7479 7065 3d22 7465 7874 220a 2020  t type="text".  
+00008b70: 2020 2020 2020 2069 643d 2266 6f72 6d2d         id="form-
+00008b80: 7769 6467 6574 732d 7375 626f 626a 6563  widgets-subobjec
+00008b90: 742d 7769 6467 6574 732d 7375 6266 6965  t-widgets-subfie
+00008ba0: 6c64 2d77 6964 6765 7473 2d66 6f6f 6669  ld-widgets-foofi
+00008bb0: 656c 6422 0a20 2020 2020 2020 2020 6e61  eld".         na
+00008bc0: 6d65 3d22 666f 726d 2e77 6964 6765 7473  me="form.widgets
+00008bd0: 2e73 7562 6f62 6a65 6374 2e77 6964 6765  .subobject.widge
+00008be0: 7473 2e73 7562 6669 656c 642e 7769 6467  ts.subfield.widg
+00008bf0: 6574 732e 666f 6f66 6965 6c64 220a 2020  ets.foofield".  
+00008c00: 2020 2020 2020 2063 6c61 7373 3d22 7465         class="te
+00008c10: 7874 2d77 6964 6765 7420 7265 7175 6972  xt-widget requir
+00008c20: 6564 2069 6e74 2d66 6965 6c64 220a 2020  ed int-field".  
+00008c30: 2020 2020 2020 2076 616c 7565 3d22 312c         value="1,
+00008c40: 3131 3122 202f 3e0a 2020 2020 2020 2020  111" />.        
+00008c50: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00008c60: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00008c70: 636c 6173 733d 226c 6162 656c 223e 0a20  class="label">. 
+00008c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c90: 2020 2020 203c 6c61 6265 6c20 666f 723d       <label for=
+00008ca0: 2266 6f72 6d2d 7769 6467 6574 732d 7375  "form-widgets-su
+00008cb0: 626f 626a 6563 742d 7769 6467 6574 732d  bobject-widgets-
+00008cc0: 7375 6266 6965 6c64 2d77 6964 6765 7473  subfield-widgets
+00008cd0: 2d62 6172 6669 656c 6422 3e0a 2020 2020  -barfield">.    
 00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cf0: 3c73 7061 6e3e 4d79 2064 6561 7220 6261  <span>My dear ba
-00008d00: 723c 2f73 7061 6e3e 0a20 2020 2020 2020  r</span>.       
-00008d10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00008d20: 2f6c 6162 656c 3e0a 2020 2020 2020 2020  /label>.        
-00008d30: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00008d40: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00008d50: 636c 6173 733d 2277 6964 6765 7422 3e0a  class="widget">.
-00008d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d70: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
-00008d80: 653d 2274 6578 7422 0a20 2020 2020 2020  e="text".       
-00008d90: 2020 6964 3d22 666f 726d 2d77 6964 6765    id="form-widge
-00008da0: 7473 2d73 7562 6f62 6a65 6374 2d77 6964  ts-subobject-wid
-00008db0: 6765 7473 2d73 7562 6669 656c 642d 7769  gets-subfield-wi
-00008dc0: 6467 6574 732d 6261 7266 6965 6c64 220a  dgets-barfield".
-00008dd0: 2020 2020 2020 2020 206e 616d 653d 2266           name="f
-00008de0: 6f72 6d2e 7769 6467 6574 732e 7375 626f  orm.widgets.subo
-00008df0: 626a 6563 742e 7769 6467 6574 732e 7375  bject.widgets.su
-00008e00: 6266 6965 6c64 2e77 6964 6765 7473 2e62  bfield.widgets.b
-00008e10: 6172 6669 656c 6422 0a20 2020 2020 2020  arfield".       
-00008e20: 2020 636c 6173 733d 2274 6578 742d 7769    class="text-wi
-00008e30: 6467 6574 2069 6e74 2d66 6965 6c64 220a  dget int-field".
-00008e40: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
-00008e50: 322c 3232 3222 202f 3e0a 2020 2020 2020  2,222" />.      
-00008e60: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00008e70: 2020 2020 203c 696e 7075 7420 6e61 6d65       <input name
-00008e80: 3d22 666f 726d 2e77 6964 6765 7473 2e73  ="form.widgets.s
-00008e90: 7562 6f62 6a65 6374 2e77 6964 6765 7473  ubobject.widgets
-00008ea0: 2e73 7562 6669 656c 642d 656d 7074 792d  .subfield-empty-
-00008eb0: 6d61 726b 6572 2220 7479 7065 3d22 6869  marker" type="hi
-00008ec0: 6464 656e 2220 7661 6c75 653d 2231 222f  dden" value="1"/
-00008ed0: 3e0a 2020 3c2f 6469 763e 0a20 2020 2020  >.  </div>.     
-00008ee0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00008ef0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00008f00: 6976 2063 6c61 7373 3d22 6c61 6265 6c22  iv class="label"
-00008f10: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00008f20: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
-00008f30: 6f72 3d22 666f 726d 2d77 6964 6765 7473  or="form-widgets
-00008f40: 2d73 7562 6f62 6a65 6374 2d77 6964 6765  -subobject-widge
-00008f50: 7473 2d6d 6f6f 6669 656c 6422 3e0a 2020  ts-moofield">.  
-00008f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f70: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
-00008f80: 6e3e 536f 6d65 7468 696e 673c 2f73 7061  n>Something</spa
-00008f90: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00008cf0: 2020 2020 2020 2020 2020 3c73 7061 6e3e            <span>
+00008d00: 4d79 2064 6561 7220 6261 723c 2f73 7061  My dear bar</spa
+00008d10: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00008d20: 2020 2020 2020 2020 203c 2f6c 6162 656c           </label
+00008d30: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00008d40: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00008d50: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00008d60: 2277 6964 6765 7422 3e0a 2020 2020 2020  "widget">.      
+00008d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d80: 3c69 6e70 7574 2074 7970 653d 2274 6578  <input type="tex
+00008d90: 7422 0a20 2020 2020 2020 2020 6964 3d22  t".         id="
+00008da0: 666f 726d 2d77 6964 6765 7473 2d73 7562  form-widgets-sub
+00008db0: 6f62 6a65 6374 2d77 6964 6765 7473 2d73  object-widgets-s
+00008dc0: 7562 6669 656c 642d 7769 6467 6574 732d  ubfield-widgets-
+00008dd0: 6261 7266 6965 6c64 220a 2020 2020 2020  barfield".      
+00008de0: 2020 206e 616d 653d 2266 6f72 6d2e 7769     name="form.wi
+00008df0: 6467 6574 732e 7375 626f 626a 6563 742e  dgets.subobject.
+00008e00: 7769 6467 6574 732e 7375 6266 6965 6c64  widgets.subfield
+00008e10: 2e77 6964 6765 7473 2e62 6172 6669 656c  .widgets.barfiel
+00008e20: 6422 0a20 2020 2020 2020 2020 636c 6173  d".         clas
+00008e30: 733d 2274 6578 742d 7769 6467 6574 2069  s="text-widget i
+00008e40: 6e74 2d66 6965 6c64 220a 2020 2020 2020  nt-field".      
+00008e50: 2020 2076 616c 7565 3d22 322c 3232 3222     value="2,222"
+00008e60: 202f 3e0a 2020 2020 2020 2020 2020 2020   />.            
+00008e70: 2020 3c2f 6469 763e 0a20 2020 2020 203c    </div>.      <
+00008e80: 696e 7075 7420 6e61 6d65 3d22 666f 726d  input name="form
+00008e90: 2e77 6964 6765 7473 2e73 7562 6f62 6a65  .widgets.subobje
+00008ea0: 6374 2e77 6964 6765 7473 2e73 7562 6669  ct.widgets.subfi
+00008eb0: 656c 642d 656d 7074 792d 6d61 726b 6572  eld-empty-marker
+00008ec0: 2220 7479 7065 3d22 6869 6464 656e 2220  " type="hidden" 
+00008ed0: 7661 6c75 653d 2231 2220 2f3e 0a20 203c  value="1" />.  <
+00008ee0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00008ef0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00008f00: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00008f10: 6173 733d 226c 6162 656c 223e 0a20 2020  ass="label">.   
+00008f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f30: 2020 203c 6c61 6265 6c20 666f 723d 2266     <label for="f
+00008f40: 6f72 6d2d 7769 6467 6574 732d 7375 626f  orm-widgets-subo
+00008f50: 626a 6563 742d 7769 6467 6574 732d 6d6f  bject-widgets-mo
+00008f60: 6f66 6965 6c64 223e 0a20 2020 2020 2020  ofield">.       
+00008f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f80: 2020 2020 2020 203c 7370 616e 3e53 6f6d         <span>Som
+00008f90: 6574 6869 6e67 3c2f 7370 616e 3e0a 2020  ething</span>.  
 00008fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fb0: 203c 7370 616e 2063 6c61 7373 3d22 7265   <span class="re
-00008fc0: 7175 6972 6564 223e 2a3c 2f73 7061 6e3e  quired">*</span>
-00008fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008fe0: 2020 2020 2020 203c 2f6c 6162 656c 3e0a         </label>.
-00008ff0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00009000: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00009010: 2020 203c 6469 7620 636c 6173 733d 2277     <div class="w
-00009020: 6964 6765 7422 3e0a 2020 2020 2020 2020  idget">.        
-00009030: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00009040: 6e70 7574 2074 7970 653d 2274 6578 7422  nput type="text"
-00009050: 0a20 2020 2020 2020 2020 6964 3d22 666f  .         id="fo
-00009060: 726d 2d77 6964 6765 7473 2d73 7562 6f62  rm-widgets-subob
-00009070: 6a65 6374 2d77 6964 6765 7473 2d6d 6f6f  ject-widgets-moo
-00009080: 6669 656c 6422 0a20 2020 2020 2020 2020  field".         
-00009090: 6e61 6d65 3d22 666f 726d 2e77 6964 6765  name="form.widge
-000090a0: 7473 2e73 7562 6f62 6a65 6374 2e77 6964  ts.subobject.wid
-000090b0: 6765 7473 2e6d 6f6f 6669 656c 6422 0a20  gets.moofield". 
-000090c0: 2020 2020 2020 2020 636c 6173 733d 2274          class="t
-000090d0: 6578 742d 7769 6467 6574 2072 6571 7569  ext-widget requi
-000090e0: 7265 6420 7465 7874 6c69 6e65 2d66 6965  red textline-fie
-000090f0: 6c64 220a 2020 2020 2020 2020 2076 616c  ld".         val
-00009100: 7565 3d22 2220 2f3e 0a20 2020 2020 2020  ue="" />.       
-00009110: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00009120: 2020 2020 3c69 6e70 7574 206e 616d 653d      <input name=
-00009130: 2266 6f72 6d2e 7769 6467 6574 732e 7375  "form.widgets.su
-00009140: 626f 626a 6563 742d 656d 7074 792d 6d61  bobject-empty-ma
-00009150: 726b 6572 2220 7479 7065 3d22 6869 6464  rker" type="hidd
-00009160: 656e 2220 7661 6c75 653d 2231 222f 3e0a  en" value="1"/>.
-00009170: 2020 3c2f 6469 763e 0a20 2020 203c 2f64    </div>.    </d
-00009180: 6976 3e0a 2020 2020 3c64 6976 2063 6c61  iv>.    <div cla
-00009190: 7373 3d22 726f 7722 3e0a 2020 2020 2020  ss="row">.      
-000091a0: 3c6c 6162 656c 2066 6f72 3d22 666f 726d  <label for="form
-000091b0: 2d77 6964 6765 7473 2d6e 616d 6522 3e6e  -widgets-name">n
-000091c0: 616d 653c 2f6c 6162 656c 3e0a 2020 2020  ame</label>.    
-000091d0: 2020 3c69 6e70 7574 2074 7970 653d 2274    <input type="t
-000091e0: 6578 7422 0a20 2020 2020 2020 2020 6964  ext".         id
-000091f0: 3d22 666f 726d 2d77 6964 6765 7473 2d6e  ="form-widgets-n
-00009200: 616d 6522 0a20 2020 2020 2020 2020 6e61  ame".         na
-00009210: 6d65 3d22 666f 726d 2e77 6964 6765 7473  me="form.widgets
-00009220: 2e6e 616d 6522 0a20 2020 2020 2020 2020  .name".         
-00009230: 636c 6173 733d 2274 6578 742d 7769 6467  class="text-widg
-00009240: 6574 2072 6571 7569 7265 6420 7465 7874  et required text
-00009250: 6c69 6e65 2d66 6965 6c64 220a 2020 2020  line-field".    
-00009260: 2020 2020 2076 616c 7565 3d22 2220 2f3e       value="" />
-00009270: 0a20 2020 203c 2f64 6976 3e0a 2020 2020  .    </div>.    
-00009280: 3c64 6976 2063 6c61 7373 3d22 6163 7469  <div class="acti
-00009290: 6f6e 223e 0a20 2020 2020 203c 696e 7075  on">.      <inpu
-000092a0: 7420 7479 7065 3d22 7375 626d 6974 220a  t type="submit".
-000092b0: 2020 2020 2020 2020 2069 643d 2266 6f72           id="for
-000092c0: 6d2d 6275 7474 6f6e 732d 6164 6422 0a20  m-buttons-add". 
-000092d0: 2020 2020 2020 2020 6e61 6d65 3d22 666f          name="fo
-000092e0: 726d 2e62 7574 746f 6e73 2e61 6464 220a  rm.buttons.add".
-000092f0: 2020 2020 2020 2020 2063 6c61 7373 3d22           class="
-00009300: 7375 626d 6974 2d77 6964 6765 7420 6275  submit-widget bu
-00009310: 7474 6f6e 2d66 6965 6c64 220a 2020 2020  tton-field".    
-00009320: 2020 2020 2076 616c 7565 3d22 4164 6422       value="Add"
-00009330: 202f 3e0a 2020 2020 3c2f 6469 763e 0a20   />.    </div>. 
-00009340: 203c 2f66 6f72 6d3e 0a0a 0a43 6f76 6572   </form>...Cover
-00009350: 6167 6520 6861 7070 696e 6573 730a 2323  age happiness.##
-00009360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00009370: 0a0a 436f 6e76 6572 7469 6e67 204e 4f5f  ..Converting NO_
-00009380: 5641 4c55 4520 686f 6c64 7320 4e6f 6e65  VALUE holds None
-00009390: 3a0a 0a20 203e 3e3e 2066 726f 6d20 7079  :..  >>> from py
-000093a0: 616d 735f 7574 696c 732e 696e 7465 7266  ams_utils.interf
-000093b0: 6163 6573 2e66 6f72 6d20 696d 706f 7274  aces.form import
-000093c0: 204e 4f5f 5641 4c55 450a 2020 3e3e 3e20   NO_VALUE.  >>> 
-000093d0: 636f 6e76 6572 7465 722e 746f 5f66 6965  converter.to_fie
-000093e0: 6c64 5f76 616c 7565 284e 4f5f 5641 4c55  ld_value(NO_VALU
-000093f0: 4529 2069 7320 4e6f 6e65 0a20 2054 7275  E) is None.  Tru
-00009400: 650a 0a0a 5468 6973 2069 7320 6120 636f  e...This is a co
-00009410: 6d70 6c69 6361 7465 6420 6361 7365 2e0a  mplicated case..
-00009420: 4861 7070 656e 7320 7768 656e 2074 6865  Happens when the
-00009430: 2063 6f6e 7465 7874 2069 7320 6120 6469   context is a di
-00009440: 6374 2c20 616e 6420 7468 6520 6469 6374  ct, and the dict
-00009450: 206d 6973 7365 7320 7468 6520 6669 656c   misses the fiel
-00009460: 642e 0a28 4e6f 7465 2c20 7765 2772 6520  d..(Note, we're 
-00009470: 6d61 6b69 6e67 2060 6073 7562 5f5f 6f62  making ``sub__ob
-00009480: 6a65 6374 6060 2069 6e73 7465 6164 206f  ject`` instead o
-00009490: 6620 6060 7375 626f 626a 6563 7460 6029  f ``subobject``)
-000094a0: 0a0a 2020 3e3e 3e20 636f 6e74 6578 7420  ..  >>> context 
-000094b0: 3d20 6469 6374 2873 7562 5f5f 6f62 6a65  = dict(sub__obje
-000094c0: 6374 3d4e 6f6e 652c 2066 6f6f 3d31 3233  ct=None, foo=123
-000094d0: 2c20 6261 723d 3435 3629 0a0a 416c 6c20  , bar=456)..All 
-000094e0: 7468 6520 7374 6f72 7920 7468 6520 6372  the story the cr
-000094f0: 6561 7465 2061 2077 6964 6765 743a 0a0a  eate a widget:..
-00009500: 2020 3e3e 3e20 6669 656c 6420 3d20 7a6f    >>> field = zo
-00009510: 7065 2e73 6368 656d 612e 4f62 6a65 6374  pe.schema.Object
-00009520: 280a 2020 2e2e 2e20 2020 2020 5f5f 6e61  (.  ...     __na
-00009530: 6d65 5f5f 3d27 7375 626f 626a 6563 7427  me__='subobject'
-00009540: 2c0a 2020 2e2e 2e20 2020 2020 7469 746c  ,.  ...     titl
-00009550: 653d 276d 7920 6f62 6a65 6374 2077 6964  e='my object wid
-00009560: 6765 7427 2c0a 2020 2e2e 2e20 2020 2020  get',.  ...     
-00009570: 7363 6865 6d61 3d49 4d79 5375 624f 626a  schema=IMySubObj
-00009580: 6563 7429 0a0a 2020 3e3e 3e20 7776 203d  ect)..  >>> wv =
-00009590: 2070 7961 6d73 5f66 6f72 6d2e 6f62 6a65   pyams_form.obje
-000095a0: 6374 2e4f 626a 6563 7457 6964 6765 7456  ct.ObjectWidgetV
-000095b0: 616c 7565 280a 2020 2e2e 2e20 2020 2020  alue(.  ...     
-000095c0: 7b27 666f 6f66 6965 6c64 273a 2027 3227  {'foofield': '2'
-000095d0: 2c20 2762 6172 6669 656c 6427 3a20 2739  , 'barfield': '9
-000095e0: 3939 277d 290a 0a20 203e 3e3e 2072 6571  99'})..  >>> req
-000095f0: 7565 7374 203d 2054 6573 7452 6571 7565  uest = TestReque
-00009600: 7374 2829 0a20 203e 3e3e 2077 6964 6765  st().  >>> widge
-00009610: 7420 3d20 7079 616d 735f 666f 726d 2e62  t = pyams_form.b
-00009620: 726f 7773 6572 2e6f 626a 6563 742e 4f62  rowser.object.Ob
-00009630: 6a65 6374 5769 6467 6574 2872 6571 7565  jectWidget(reque
-00009640: 7374 290a 2020 3e3e 3e20 7769 6467 6574  st).  >>> widget
-00009650: 203d 2046 6965 6c64 5769 6467 6574 2866   = FieldWidget(f
-00009660: 6965 6c64 2c20 7769 6467 6574 290a 2020  ield, widget).  
-00009670: 3e3e 3e20 7769 6467 6574 2e63 6f6e 7465  >>> widget.conte
-00009680: 7874 203d 2063 6f6e 7465 7874 0a20 203e  xt = context.  >
-00009690: 3e3e 2077 6964 6765 742e 7661 6c75 6520  >> widget.value 
-000096a0: 3d20 7776 0a20 203e 3e3e 2077 6964 6765  = wv.  >>> widge
-000096b0: 742e 7570 6461 7465 2829 0a20 203e 3e3e  t.update().  >>>
-000096c0: 2063 6f6e 7665 7274 6572 203d 2069 6e74   converter = int
-000096d0: 6572 6661 6365 732e 4944 6174 6143 6f6e  erfaces.IDataCon
-000096e0: 7665 7274 6572 2877 6964 6765 7429 0a0a  verter(widget)..
-000096f0: 416e 6420 7374 696c 6c20 7765 2067 6574  And still we get
-00009700: 2061 204d 7953 7562 4f62 6a65 6374 2c20   a MySubObject, 
-00009710: 6e6f 2066 6169 6c75 7265 3a0a 0a20 203e  no failure:..  >
-00009720: 3e3e 2076 616c 7565 203d 2063 6f6e 7665  >> value = conve
-00009730: 7274 6572 2e74 6f5f 6669 656c 645f 7661  rter.to_field_va
-00009740: 6c75 6528 7776 290a 2020 3e3e 3e20 7661  lue(wv).  >>> va
-00009750: 6c75 650a 2020 3c70 7961 6d73 5f66 6f72  lue.  <pyams_for
-00009760: 6d2e 7465 7374 696e 672e 4d79 5375 624f  m.testing.MySubO
-00009770: 626a 6563 7420 6f62 6a65 6374 2061 7420  bject object at 
-00009780: 2e2e 2e3e 0a20 203e 3e3e 2076 616c 7565  ...>.  >>> value
-00009790: 2e66 6f6f 6669 656c 640a 2020 320a 2020  .foofield.  2.  
-000097a0: 3e3e 3e20 7661 6c75 652e 6261 7266 6965  >>> value.barfie
-000097b0: 6c64 0a20 2039 3939 0a0a 0a45 6173 7920  ld.  999...Easy 
-000097c0: 2861 6674 6572 2074 6865 2070 7265 7669  (after the previ
-000097d0: 6f75 7329 2e0a 496e 2063 6173 6520 7468  ous)..In case th
-000097e0: 6520 7072 6576 696f 7573 2076 616c 7565  e previous value
-000097f0: 206f 6e20 7468 6520 636f 6e74 6578 7420   on the context 
-00009800: 6973 204e 6f6e 6520 286f 7220 6d69 7373  is None (or miss
-00009810: 696e 6729 2e0a 5765 206e 6565 6420 746f  ing)..We need to
-00009820: 2063 7265 6174 6520 6120 6e65 7720 6f62   create a new ob
-00009830: 6a65 6374 2074 6f20 6265 2061 626c 6520  ject to be able 
-00009840: 746f 2073 6574 2070 726f 7065 7274 6965  to set propertie
-00009850: 7320 6f6e 2e0a 0a20 203e 3e3e 2063 6f6e  s on...  >>> con
-00009860: 7465 7874 5b27 7375 626f 626a 6563 7427  text['subobject'
-00009870: 5d20 3d20 4e6f 6e65 0a20 203e 3e3e 2076  ] = None.  >>> v
-00009880: 616c 7565 203d 2063 6f6e 7665 7274 6572  alue = converter
-00009890: 2e74 6f5f 6669 656c 645f 7661 6c75 6528  .to_field_value(
-000098a0: 7776 290a 2020 3e3e 3e20 7661 6c75 650a  wv).  >>> value.
-000098b0: 2020 3c70 7961 6d73 5f66 6f72 6d2e 7465    <pyams_form.te
-000098c0: 7374 696e 672e 4d79 5375 624f 626a 6563  sting.MySubObjec
-000098d0: 7420 6f62 6a65 6374 2061 7420 2e2e 2e3e  t object at ...>
-000098e0: 0a20 203e 3e3e 2076 616c 7565 2e66 6f6f  .  >>> value.foo
-000098f0: 6669 656c 640a 2020 320a 2020 3e3e 3e20  field.  2.  >>> 
-00009900: 7661 6c75 652e 6261 7266 6965 6c64 0a20  value.barfield. 
-00009910: 2039 3939 0a0a 496e 2063 6173 6520 7468   999..In case th
-00009920: 6572 6520 6973 2073 6f6d 6574 6869 6e67  ere is something
-00009930: 2074 6861 7420 6361 6e6e 6f74 2062 6520   that cannot be 
-00009940: 6164 6170 7465 6420 746f 2074 6865 2072  adapted to the r
-00009950: 6967 6874 2069 6e74 6572 6661 6365 2c0a  ight interface,.
-00009960: 6974 206a 7573 7420 6275 7270 733a 0a28  it just burps:.(
-00009970: 6d69 6768 7420 6265 2061 6e20 6964 6561  might be an idea
-00009980: 2074 6f20 6372 6561 7465 2069 6e20 7468   to create in th
-00009990: 6973 2063 6173 6520 616c 736f 2061 206e  is case also a n
-000099a0: 6577 2062 6c61 6e6b 206f 626a 6563 7429  ew blank object)
-000099b0: 0a0a 2020 3e3e 3e20 636f 6e74 6578 745b  ..  >>> context[
-000099c0: 2773 7562 6f62 6a65 6374 275d 203d 2027  'subobject'] = '
-000099d0: 6272 7574 616c 270a 2020 3e3e 3e20 636f  brutal'.  >>> co
-000099e0: 6e76 6572 7465 722e 746f 5f66 6965 6c64  nverter.to_field
-000099f0: 5f76 616c 7565 2877 7629 0a20 2054 7261  _value(wv).  Tra
-00009a00: 6365 6261 636b 2028 6d6f 7374 2072 6563  ceback (most rec
-00009a10: 656e 7420 6361 6c6c 206c 6173 7429 3a0a  ent call last):.
-00009a20: 2020 2e2e 2e0a 2020 5479 7065 4572 726f    ....  TypeErro
-00009a30: 723a 2028 2743 6f75 6c64 206e 6f74 2061  r: ('Could not a
-00009a40: 6461 7074 272c 2027 6272 7574 616c 272c  dapt', 'brutal',
-00009a50: 0a20 203c 496e 7465 7266 6163 6543 6c61  .  <InterfaceCla
-00009a60: 7373 2070 7961 6d73 5f66 6f72 6d2e 7465  ss pyams_form.te
-00009a70: 7374 696e 672e 494d 7953 7562 4f62 6a65  sting.IMySubObje
-00009a80: 6374 3e29 0a0a 2020 3e3e 3e20 636f 6e74  ct>)..  >>> cont
-00009a90: 6578 745b 2773 7562 6f62 6a65 6374 275d  ext['subobject']
-00009aa0: 203d 204e 6f6e 650a 0a0a 4f6e 6520 6d6f   = None...One mo
-00009ab0: 7265 2e0a 5661 6c75 6520 746f 2063 6f6e  re..Value to con
-00009ac0: 7665 7274 206d 6973 7365 7320 6120 6669  vert misses a fi
-00009ad0: 656c 642e 2053 686f 756c 6420 6e65 7665  eld. Should neve
-00009ae0: 7220 6861 7070 656e 2061 6374 7561 6c6c  r happen actuall
-00009af0: 793a 0a0a 2020 3e3e 3e20 7776 203d 2070  y:..  >>> wv = p
-00009b00: 7961 6d73 5f66 6f72 6d2e 6f62 6a65 6374  yams_form.object
-00009b10: 2e4f 626a 6563 7457 6964 6765 7456 616c  .ObjectWidgetVal
-00009b20: 7565 280a 2020 2e2e 2e20 2020 2020 7b27  ue(.  ...     {'
-00009b30: 666f 6f66 6965 6c64 273a 2027 3227 7d29  foofield': '2'})
-00009b40: 0a20 203e 3e3e 2076 616c 7565 203d 2063  .  >>> value = c
-00009b50: 6f6e 7665 7274 6572 2e74 6f5f 6669 656c  onverter.to_fiel
-00009b60: 645f 7661 6c75 6528 7776 290a 0a4b 6e6f  d_value(wv)..Kno
-00009b70: 776e 2070 726f 7065 7274 7920 6973 2073  wn property is s
-00009b80: 6574 3a0a 0a20 203e 3e3e 2076 616c 7565  et:..  >>> value
-00009b90: 2e66 6f6f 6669 656c 640a 2020 320a 0a55  .foofield.  2..U
-00009ba0: 6e6b 6e6f 776e 2073 7469 636b 7320 7469  nknown sticks ti
-00009bb0: 2069 7427 7320 6465 6661 756c 7420 7661   it's default va
-00009bc0: 6c75 653a 0a0a 2020 3e3e 3e20 7661 6c75  lue:..  >>> valu
-00009bd0: 652e 6261 7266 6965 6c64 0a20 2032 3232  e.barfield.  222
-00009be0: 320a 0a0a 5465 7374 7320 636c 6561 6e75  2...Tests cleanu
-00009bf0: 703a 0a0a 2020 3e3e 3e20 7465 6172 446f  p:..  >>> tearDo
-00009c00: 776e 2829 0a                             wn().
+00008fb0: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
+00008fc0: 6e20 636c 6173 733d 2272 6571 7569 7265  n class="require
+00008fd0: 6422 3e2a 3c2f 7370 616e 3e0a 2020 2020  d">*</span>.    
+00008fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ff0: 2020 3c2f 6c61 6265 6c3e 0a20 2020 2020    </label>.     
+00009000: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00009010: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00009020: 6976 2063 6c61 7373 3d22 7769 6467 6574  iv class="widget
+00009030: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00009040: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
+00009050: 7479 7065 3d22 7465 7874 220a 2020 2020  type="text".    
+00009060: 2020 2020 2069 643d 2266 6f72 6d2d 7769       id="form-wi
+00009070: 6467 6574 732d 7375 626f 626a 6563 742d  dgets-subobject-
+00009080: 7769 6467 6574 732d 6d6f 6f66 6965 6c64  widgets-moofield
+00009090: 220a 2020 2020 2020 2020 206e 616d 653d  ".         name=
+000090a0: 2266 6f72 6d2e 7769 6467 6574 732e 7375  "form.widgets.su
+000090b0: 626f 626a 6563 742e 7769 6467 6574 732e  bobject.widgets.
+000090c0: 6d6f 6f66 6965 6c64 220a 2020 2020 2020  moofield".      
+000090d0: 2020 2063 6c61 7373 3d22 7465 7874 2d77     class="text-w
+000090e0: 6964 6765 7420 7265 7175 6972 6564 2074  idget required t
+000090f0: 6578 746c 696e 652d 6669 656c 6422 0a20  extline-field". 
+00009100: 2020 2020 2020 2020 7661 6c75 653d 2222          value=""
+00009110: 202f 3e0a 2020 2020 2020 2020 2020 2020   />.            
+00009120: 2020 3c2f 6469 763e 0a20 2020 2020 203c    </div>.      <
+00009130: 696e 7075 7420 6e61 6d65 3d22 666f 726d  input name="form
+00009140: 2e77 6964 6765 7473 2e73 7562 6f62 6a65  .widgets.subobje
+00009150: 6374 2d65 6d70 7479 2d6d 6172 6b65 7222  ct-empty-marker"
+00009160: 2074 7970 653d 2268 6964 6465 6e22 2076   type="hidden" v
+00009170: 616c 7565 3d22 3122 202f 3e0a 2020 3c2f  alue="1" />.  </
+00009180: 6469 763e 0a20 2020 203c 2f64 6976 3e0a  div>.    </div>.
+00009190: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000091a0: 726f 7722 3e0a 2020 2020 2020 3c6c 6162  row">.      <lab
+000091b0: 656c 2066 6f72 3d22 666f 726d 2d77 6964  el for="form-wid
+000091c0: 6765 7473 2d6e 616d 6522 3e6e 616d 653c  gets-name">name<
+000091d0: 2f6c 6162 656c 3e0a 2020 2020 2020 3c69  /label>.      <i
+000091e0: 6e70 7574 2074 7970 653d 2274 6578 7422  nput type="text"
+000091f0: 0a20 2020 2020 2020 2020 6964 3d22 666f  .         id="fo
+00009200: 726d 2d77 6964 6765 7473 2d6e 616d 6522  rm-widgets-name"
+00009210: 0a20 2020 2020 2020 2020 6e61 6d65 3d22  .         name="
+00009220: 666f 726d 2e77 6964 6765 7473 2e6e 616d  form.widgets.nam
+00009230: 6522 0a20 2020 2020 2020 2020 636c 6173  e".         clas
+00009240: 733d 2274 6578 742d 7769 6467 6574 2072  s="text-widget r
+00009250: 6571 7569 7265 6420 7465 7874 6c69 6e65  equired textline
+00009260: 2d66 6965 6c64 220a 2020 2020 2020 2020  -field".        
+00009270: 2076 616c 7565 3d22 2220 2f3e 0a20 2020   value="" />.   
+00009280: 203c 2f64 6976 3e0a 2020 2020 3c64 6976   </div>.    <div
+00009290: 2063 6c61 7373 3d22 6163 7469 6f6e 223e   class="action">
+000092a0: 0a20 2020 2020 203c 696e 7075 7420 7479  .      <input ty
+000092b0: 7065 3d22 7375 626d 6974 220a 2020 2020  pe="submit".    
+000092c0: 2020 2020 2069 643d 2266 6f72 6d2d 6275       id="form-bu
+000092d0: 7474 6f6e 732d 6164 6422 0a20 2020 2020  ttons-add".     
+000092e0: 2020 2020 6e61 6d65 3d22 666f 726d 2e62      name="form.b
+000092f0: 7574 746f 6e73 2e61 6464 220a 2020 2020  uttons.add".    
+00009300: 2020 2020 2063 6c61 7373 3d22 7375 626d       class="subm
+00009310: 6974 2d77 6964 6765 7420 6275 7474 6f6e  it-widget button
+00009320: 2d66 6965 6c64 220a 2020 2020 2020 2020  -field".        
+00009330: 2076 616c 7565 3d22 4164 6422 202f 3e0a   value="Add" />.
+00009340: 2020 2020 3c2f 6469 763e 0a20 203c 2f66      </div>.  </f
+00009350: 6f72 6d3e 0a0a 0a43 6f76 6572 6167 6520  orm>...Coverage 
+00009360: 6861 7070 696e 6573 730a 2323 2323 2323  happiness.######
+00009370: 2323 2323 2323 2323 2323 2323 0a0a 436f  ############..Co
+00009380: 6e76 6572 7469 6e67 204e 4f5f 5641 4c55  nverting NO_VALU
+00009390: 4520 686f 6c64 7320 4e6f 6e65 3a0a 0a20  E holds None:.. 
+000093a0: 203e 3e3e 2066 726f 6d20 7079 616d 735f   >>> from pyams_
+000093b0: 7574 696c 732e 696e 7465 7266 6163 6573  utils.interfaces
+000093c0: 2e66 6f72 6d20 696d 706f 7274 204e 4f5f  .form import NO_
+000093d0: 5641 4c55 450a 2020 3e3e 3e20 636f 6e76  VALUE.  >>> conv
+000093e0: 6572 7465 722e 746f 5f66 6965 6c64 5f76  erter.to_field_v
+000093f0: 616c 7565 284e 4f5f 5641 4c55 4529 2069  alue(NO_VALUE) i
+00009400: 7320 4e6f 6e65 0a20 2054 7275 650a 0a0a  s None.  True...
+00009410: 5468 6973 2069 7320 6120 636f 6d70 6c69  This is a compli
+00009420: 6361 7465 6420 6361 7365 2e0a 4861 7070  cated case..Happ
+00009430: 656e 7320 7768 656e 2074 6865 2063 6f6e  ens when the con
+00009440: 7465 7874 2069 7320 6120 6469 6374 2c20  text is a dict, 
+00009450: 616e 6420 7468 6520 6469 6374 206d 6973  and the dict mis
+00009460: 7365 7320 7468 6520 6669 656c 642e 0a28  ses the field..(
+00009470: 4e6f 7465 2c20 7765 2772 6520 6d61 6b69  Note, we're maki
+00009480: 6e67 2060 6073 7562 5f5f 6f62 6a65 6374  ng ``sub__object
+00009490: 6060 2069 6e73 7465 6164 206f 6620 6060  `` instead of ``
+000094a0: 7375 626f 626a 6563 7460 6029 0a0a 2020  subobject``)..  
+000094b0: 3e3e 3e20 636f 6e74 6578 7420 3d20 6469  >>> context = di
+000094c0: 6374 2873 7562 5f5f 6f62 6a65 6374 3d4e  ct(sub__object=N
+000094d0: 6f6e 652c 2066 6f6f 3d31 3233 2c20 6261  one, foo=123, ba
+000094e0: 723d 3435 3629 0a0a 416c 6c20 7468 6520  r=456)..All the 
+000094f0: 7374 6f72 7920 7468 6520 6372 6561 7465  story the create
+00009500: 2061 2077 6964 6765 743a 0a0a 2020 3e3e   a widget:..  >>
+00009510: 3e20 6669 656c 6420 3d20 7a6f 7065 2e73  > field = zope.s
+00009520: 6368 656d 612e 4f62 6a65 6374 280a 2020  chema.Object(.  
+00009530: 2e2e 2e20 2020 2020 5f5f 6e61 6d65 5f5f  ...     __name__
+00009540: 3d27 7375 626f 626a 6563 7427 2c0a 2020  ='subobject',.  
+00009550: 2e2e 2e20 2020 2020 7469 746c 653d 276d  ...     title='m
+00009560: 7920 6f62 6a65 6374 2077 6964 6765 7427  y object widget'
+00009570: 2c0a 2020 2e2e 2e20 2020 2020 7363 6865  ,.  ...     sche
+00009580: 6d61 3d49 4d79 5375 624f 626a 6563 7429  ma=IMySubObject)
+00009590: 0a0a 2020 3e3e 3e20 7776 203d 2070 7961  ..  >>> wv = pya
+000095a0: 6d73 5f66 6f72 6d2e 6f62 6a65 6374 2e4f  ms_form.object.O
+000095b0: 626a 6563 7457 6964 6765 7456 616c 7565  bjectWidgetValue
+000095c0: 280a 2020 2e2e 2e20 2020 2020 7b27 666f  (.  ...     {'fo
+000095d0: 6f66 6965 6c64 273a 2027 3227 2c20 2762  ofield': '2', 'b
+000095e0: 6172 6669 656c 6427 3a20 2739 3939 277d  arfield': '999'}
+000095f0: 290a 0a20 203e 3e3e 2072 6571 7565 7374  )..  >>> request
+00009600: 203d 2054 6573 7452 6571 7565 7374 2829   = TestRequest()
+00009610: 0a20 203e 3e3e 2077 6964 6765 7420 3d20  .  >>> widget = 
+00009620: 7079 616d 735f 666f 726d 2e62 726f 7773  pyams_form.brows
+00009630: 6572 2e6f 626a 6563 742e 4f62 6a65 6374  er.object.Object
+00009640: 5769 6467 6574 2872 6571 7565 7374 290a  Widget(request).
+00009650: 2020 3e3e 3e20 7769 6467 6574 203d 2046    >>> widget = F
+00009660: 6965 6c64 5769 6467 6574 2866 6965 6c64  ieldWidget(field
+00009670: 2c20 7769 6467 6574 290a 2020 3e3e 3e20  , widget).  >>> 
+00009680: 7769 6467 6574 2e63 6f6e 7465 7874 203d  widget.context =
+00009690: 2063 6f6e 7465 7874 0a20 203e 3e3e 2077   context.  >>> w
+000096a0: 6964 6765 742e 7661 6c75 6520 3d20 7776  idget.value = wv
+000096b0: 0a20 203e 3e3e 2077 6964 6765 742e 7570  .  >>> widget.up
+000096c0: 6461 7465 2829 0a20 203e 3e3e 2063 6f6e  date().  >>> con
+000096d0: 7665 7274 6572 203d 2069 6e74 6572 6661  verter = interfa
+000096e0: 6365 732e 4944 6174 6143 6f6e 7665 7274  ces.IDataConvert
+000096f0: 6572 2877 6964 6765 7429 0a0a 416e 6420  er(widget)..And 
+00009700: 7374 696c 6c20 7765 2067 6574 2061 204d  still we get a M
+00009710: 7953 7562 4f62 6a65 6374 2c20 6e6f 2066  ySubObject, no f
+00009720: 6169 6c75 7265 3a0a 0a20 203e 3e3e 2076  ailure:..  >>> v
+00009730: 616c 7565 203d 2063 6f6e 7665 7274 6572  alue = converter
+00009740: 2e74 6f5f 6669 656c 645f 7661 6c75 6528  .to_field_value(
+00009750: 7776 290a 2020 3e3e 3e20 7661 6c75 650a  wv).  >>> value.
+00009760: 2020 3c70 7961 6d73 5f66 6f72 6d2e 7465    <pyams_form.te
+00009770: 7374 696e 672e 4d79 5375 624f 626a 6563  sting.MySubObjec
+00009780: 7420 6f62 6a65 6374 2061 7420 2e2e 2e3e  t object at ...>
+00009790: 0a20 203e 3e3e 2076 616c 7565 2e66 6f6f  .  >>> value.foo
+000097a0: 6669 656c 640a 2020 320a 2020 3e3e 3e20  field.  2.  >>> 
+000097b0: 7661 6c75 652e 6261 7266 6965 6c64 0a20  value.barfield. 
+000097c0: 2039 3939 0a0a 0a45 6173 7920 2861 6674   999...Easy (aft
+000097d0: 6572 2074 6865 2070 7265 7669 6f75 7329  er the previous)
+000097e0: 2e0a 496e 2063 6173 6520 7468 6520 7072  ..In case the pr
+000097f0: 6576 696f 7573 2076 616c 7565 206f 6e20  evious value on 
+00009800: 7468 6520 636f 6e74 6578 7420 6973 204e  the context is N
+00009810: 6f6e 6520 286f 7220 6d69 7373 696e 6729  one (or missing)
+00009820: 2e0a 5765 206e 6565 6420 746f 2063 7265  ..We need to cre
+00009830: 6174 6520 6120 6e65 7720 6f62 6a65 6374  ate a new object
+00009840: 2074 6f20 6265 2061 626c 6520 746f 2073   to be able to s
+00009850: 6574 2070 726f 7065 7274 6965 7320 6f6e  et properties on
+00009860: 2e0a 0a20 203e 3e3e 2063 6f6e 7465 7874  ...  >>> context
+00009870: 5b27 7375 626f 626a 6563 7427 5d20 3d20  ['subobject'] = 
+00009880: 4e6f 6e65 0a20 203e 3e3e 2076 616c 7565  None.  >>> value
+00009890: 203d 2063 6f6e 7665 7274 6572 2e74 6f5f   = converter.to_
+000098a0: 6669 656c 645f 7661 6c75 6528 7776 290a  field_value(wv).
+000098b0: 2020 3e3e 3e20 7661 6c75 650a 2020 3c70    >>> value.  <p
+000098c0: 7961 6d73 5f66 6f72 6d2e 7465 7374 696e  yams_form.testin
+000098d0: 672e 4d79 5375 624f 626a 6563 7420 6f62  g.MySubObject ob
+000098e0: 6a65 6374 2061 7420 2e2e 2e3e 0a20 203e  ject at ...>.  >
+000098f0: 3e3e 2076 616c 7565 2e66 6f6f 6669 656c  >> value.foofiel
+00009900: 640a 2020 320a 2020 3e3e 3e20 7661 6c75  d.  2.  >>> valu
+00009910: 652e 6261 7266 6965 6c64 0a20 2039 3939  e.barfield.  999
+00009920: 0a0a 496e 2063 6173 6520 7468 6572 6520  ..In case there 
+00009930: 6973 2073 6f6d 6574 6869 6e67 2074 6861  is something tha
+00009940: 7420 6361 6e6e 6f74 2062 6520 6164 6170  t cannot be adap
+00009950: 7465 6420 746f 2074 6865 2072 6967 6874  ted to the right
+00009960: 2069 6e74 6572 6661 6365 2c0a 6974 206a   interface,.it j
+00009970: 7573 7420 6275 7270 733a 0a28 6d69 6768  ust burps:.(migh
+00009980: 7420 6265 2061 6e20 6964 6561 2074 6f20  t be an idea to 
+00009990: 6372 6561 7465 2069 6e20 7468 6973 2063  create in this c
+000099a0: 6173 6520 616c 736f 2061 206e 6577 2062  ase also a new b
+000099b0: 6c61 6e6b 206f 626a 6563 7429 0a0a 2020  lank object)..  
+000099c0: 3e3e 3e20 636f 6e74 6578 745b 2773 7562  >>> context['sub
+000099d0: 6f62 6a65 6374 275d 203d 2027 6272 7574  object'] = 'brut
+000099e0: 616c 270a 2020 3e3e 3e20 636f 6e76 6572  al'.  >>> conver
+000099f0: 7465 722e 746f 5f66 6965 6c64 5f76 616c  ter.to_field_val
+00009a00: 7565 2877 7629 0a20 2054 7261 6365 6261  ue(wv).  Traceba
+00009a10: 636b 2028 6d6f 7374 2072 6563 656e 7420  ck (most recent 
+00009a20: 6361 6c6c 206c 6173 7429 3a0a 2020 2e2e  call last):.  ..
+00009a30: 2e0a 2020 5479 7065 4572 726f 723a 2028  ..  TypeError: (
+00009a40: 2743 6f75 6c64 206e 6f74 2061 6461 7074  'Could not adapt
+00009a50: 272c 2027 6272 7574 616c 272c 0a20 203c  ', 'brutal',.  <
+00009a60: 496e 7465 7266 6163 6543 6c61 7373 2070  InterfaceClass p
+00009a70: 7961 6d73 5f66 6f72 6d2e 7465 7374 696e  yams_form.testin
+00009a80: 672e 494d 7953 7562 4f62 6a65 6374 3e29  g.IMySubObject>)
+00009a90: 0a0a 2020 3e3e 3e20 636f 6e74 6578 745b  ..  >>> context[
+00009aa0: 2773 7562 6f62 6a65 6374 275d 203d 204e  'subobject'] = N
+00009ab0: 6f6e 650a 0a0a 4f6e 6520 6d6f 7265 2e0a  one...One more..
+00009ac0: 5661 6c75 6520 746f 2063 6f6e 7665 7274  Value to convert
+00009ad0: 206d 6973 7365 7320 6120 6669 656c 642e   misses a field.
+00009ae0: 2053 686f 756c 6420 6e65 7665 7220 6861   Should never ha
+00009af0: 7070 656e 2061 6374 7561 6c6c 793a 0a0a  ppen actually:..
+00009b00: 2020 3e3e 3e20 7776 203d 2070 7961 6d73    >>> wv = pyams
+00009b10: 5f66 6f72 6d2e 6f62 6a65 6374 2e4f 626a  _form.object.Obj
+00009b20: 6563 7457 6964 6765 7456 616c 7565 280a  ectWidgetValue(.
+00009b30: 2020 2e2e 2e20 2020 2020 7b27 666f 6f66    ...     {'foof
+00009b40: 6965 6c64 273a 2027 3227 7d29 0a20 203e  ield': '2'}).  >
+00009b50: 3e3e 2076 616c 7565 203d 2063 6f6e 7665  >> value = conve
+00009b60: 7274 6572 2e74 6f5f 6669 656c 645f 7661  rter.to_field_va
+00009b70: 6c75 6528 7776 290a 0a4b 6e6f 776e 2070  lue(wv)..Known p
+00009b80: 726f 7065 7274 7920 6973 2073 6574 3a0a  roperty is set:.
+00009b90: 0a20 203e 3e3e 2076 616c 7565 2e66 6f6f  .  >>> value.foo
+00009ba0: 6669 656c 640a 2020 320a 0a55 6e6b 6e6f  field.  2..Unkno
+00009bb0: 776e 2073 7469 636b 7320 7469 2069 7427  wn sticks ti it'
+00009bc0: 7320 6465 6661 756c 7420 7661 6c75 653a  s default value:
+00009bd0: 0a0a 2020 3e3e 3e20 7661 6c75 652e 6261  ..  >>> value.ba
+00009be0: 7266 6965 6c64 0a20 2032 3232 320a 0a0a  rfield.  2222...
+00009bf0: 5465 7374 7320 636c 6561 6e75 703a 0a0a  Tests cleanup:..
+00009c00: 2020 3e3e 3e20 7465 6172 446f 776e 2829    >>> tearDown()
+00009c10: 0a                                       .
```

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-objectmulti.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-objectmulti.rst`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-0-widgets-barfield"
          name="foo.0.widgets.barfield"
          class="text-widget int-field"
          value="666" />
               </div>
-      <input name="foo.0-empty-marker" type="hidden" value="1"/>
+      <input name="foo.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="foo-buttons-add"
@@ -224,15 +224,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-0-widgets-barfield"
          name="foo.0.widgets.barfield"
          class="text-widget int-field"
          value="666" />
               </div>
-      <input name="foo.0-empty-marker" type="hidden" value="1"/>
+      <input name="foo.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
       <div id="foo-1-row"
                class="row">
         <div class="label">
@@ -272,15 +272,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-1-widgets-barfield"
          name="foo.1.widgets.barfield"
          class="text-widget int-field"
          value="321" />
               </div>
-      <input name="foo.1-empty-marker" type="hidden" value="1"/>
+      <input name="foo.1-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="foo-buttons-add"
@@ -354,15 +354,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-0-widgets-barfield"
          name="foo.0.widgets.barfield"
          class="text-widget int-field"
          value="666" />
               </div>
-      <input name="foo.0-empty-marker" type="hidden" value="1"/>
+      <input name="foo.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
       <div id="foo-1-row"
                class="row">
         <div class="label">
@@ -402,15 +402,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-1-widgets-barfield"
          name="foo.1.widgets.barfield"
          class="text-widget int-field"
          value="321" />
               </div>
-      <input name="foo.1-empty-marker" type="hidden" value="1"/>
+      <input name="foo.1-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
       <div id="foo-2-row"
                class="row">
         <div class="label">
@@ -450,15 +450,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-2-widgets-barfield"
          name="foo.2.widgets.barfield"
          class="text-widget int-field"
          value="2,222" />
               </div>
-      <input name="foo.2-empty-marker" type="hidden" value="1"/>
+      <input name="foo.2-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="foo-buttons-add"
@@ -549,15 +549,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-0-widgets-barfield"
          name="foo.0.widgets.barfield"
          class="text-widget int-field"
          value="666" />
               </div>
-      <input name="foo.0-empty-marker" type="hidden" value="1"/>
+      <input name="foo.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
       <div id="foo-1-row"
                class="row">
         <div class="label">
@@ -597,15 +597,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-1-widgets-barfield"
          name="foo.1.widgets.barfield"
          class="text-widget int-field"
          value="321" />
               </div>
-      <input name="foo.1-empty-marker" type="hidden" value="1"/>
+      <input name="foo.1-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
       <div id="foo-2-row"
                class="row">
         <div class="label">
@@ -645,15 +645,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-2-widgets-barfield"
          name="foo.2.widgets.barfield"
          class="text-widget int-field"
          value="98" />
               </div>
-      <input name="foo.2-empty-marker" type="hidden" value="1"/>
+      <input name="foo.2-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="foo-buttons-add"
@@ -747,15 +747,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-0-widgets-barfield"
          name="foo.0.widgets.barfield"
          class="text-widget int-field"
          value="666" />
               </div>
-      <input name="foo.0-empty-marker" type="hidden" value="1"/>
+      <input name="foo.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
       <div id="foo-1-row"
                class="row">
         <div class="label">
@@ -795,15 +795,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-1-widgets-barfield"
          name="foo.1.widgets.barfield"
          class="text-widget int-field"
          value="98" />
               </div>
-      <input name="foo.1-empty-marker" type="hidden" value="1"/>
+      <input name="foo.1-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="foo-buttons-add"
@@ -894,15 +894,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-0-widgets-barfield"
          name="foo.0.widgets.barfield"
          class="text-widget int-field"
          value="666" />
               </div>
-      <input name="foo.0-empty-marker" type="hidden" value="1"/>
+      <input name="foo.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
       <div id="foo-1-row"
                class="row">
         <div class="label">
@@ -944,15 +944,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-1-widgets-barfield"
          name="foo.1.widgets.barfield"
          class="text-widget int-field"
          value="98" />
               </div>
-      <input name="foo.1-empty-marker" type="hidden" value="1"/>
+      <input name="foo.1-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="foo-buttons-add"
@@ -1033,15 +1033,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-0-widgets-barfield"
          name="foo.0.widgets.barfield"
          class="text-widget int-field"
          value="666" />
               </div>
-      <input name="foo.0-empty-marker" type="hidden" value="1"/>
+      <input name="foo.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
       <div id="foo-1-row"
                class="row">
         <div class="widget">
@@ -1075,15 +1075,15 @@
               <div class="widget">
                       <input type="text"
          id="foo-1-widgets-barfield"
          name="foo.1.widgets.barfield"
          class="text-widget int-field"
          value="321" />
               </div>
-      <input name="foo.1-empty-marker" type="hidden" value="1"/>
+      <input name="foo.1-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="foo-buttons-add"
@@ -1267,15 +1267,15 @@
               <div class="widget">
                       <input type="text"
          id="form-widgets-list_of_objects-0-widgets-barfield"
          name="form.widgets.list_of_objects.0.widgets.barfield"
          class="text-widget int-field"
          value="2,222" />
               </div>
-      <input name="form.widgets.list_of_objects.0-empty-marker" type="hidden" value="1"/>
+      <input name="form.widgets.list_of_objects.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="form-widgets-list_of_objects-buttons-add"
@@ -1418,15 +1418,15 @@
               <div class="widget">
                       <input type="text"
          id="form-widgets-list_of_objects-0-widgets-barfield"
          name="form.widgets.list_of_objects.0.widgets.barfield"
          class="text-widget int-field"
          value="99" />
               </div>
-      <input name="form.widgets.list_of_objects.0-empty-marker" type="hidden" value="1"/>
+      <input name="form.widgets.list_of_objects.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="form-widgets-list_of_objects-buttons-add"
@@ -1557,15 +1557,15 @@
               <div class="widget">
                       <input type="text"
          id="form-widgets-list_of_objects-0-widgets-barfield"
          name="form.widgets.list_of_objects.0.widgets.barfield"
          class="text-widget int-field"
          value="55" />
               </div>
-      <input name="form.widgets.list_of_objects.0-empty-marker" type="hidden" value="1"/>
+      <input name="form.widgets.list_of_objects.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="form-widgets-list_of_objects-buttons-add"
@@ -1721,15 +1721,15 @@
               <div class="widget">
                       <input type="text"
          id="form-widgets-list_of_objects-0-widgets-barfield"
          name="form.widgets.list_of_objects.0.widgets.barfield"
          class="text-widget int-field"
          value="bad" />
               </div>
-      <input name="form.widgets.list_of_objects.0-empty-marker" type="hidden" value="1"/>
+      <input name="form.widgets.list_of_objects.0-empty-marker" type="hidden" value="1" />
   </div>
           </div>
         </div>
       </div>
     <div class="buttons">
         <input type="submit"
          id="form-widgets-list_of_objects-buttons-add"
```

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-orderedselect.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-orderedselect.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-password.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-password.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-radio.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-radio.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-select-missing-terms.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-select-missing-terms.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-select-source.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-select-source.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-select.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-select.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-submit.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-submit.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-text.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-text.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-textarea.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-textarea.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget-textlines.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget-textlines.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/doctests/widget.rst` & `pyams_form-1.8.1/src/pyams_form/doctests/widget.rst`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/error.py` & `pyams_form-1.8.1/src/pyams_form/error.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/events.py` & `pyams_form-1.8.1/src/pyams_form/events.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/field.py` & `pyams_form-1.8.1/src/pyams_form/field.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/form.py` & `pyams_form-1.8.1/src/pyams_form/form.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/group.py` & `pyams_form-1.8.1/src/pyams_form/group.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/hint.py` & `pyams_form-1.8.1/src/pyams_form/hint.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/include.py` & `pyams_form-1.8.1/src/pyams_form/include.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/__init__.py` & `pyams_form-1.8.1/src/pyams_form/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/button.py` & `pyams_form-1.8.1/src/pyams_form/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/error.py` & `pyams_form-1.8.1/src/pyams_form/interfaces/error.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/form.py` & `pyams_form-1.8.1/src/pyams_form/interfaces/form.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/button-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/button-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/checkbox-display.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/checkbox-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/checkbox-hidden.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/checkbox-hidden.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/checkbox-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/checkbox-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/file-display.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/file-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/file-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/file-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/image-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/image-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/multi-display.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/multi-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/multi-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/multi-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/object-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/object-input.pt`

 * *Files 2% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 		<tal:if condition="widget.error">
 			${structure:widget.error.render()}
 		</tal:if>
 		<div class="widget">
 			${structure:widget.render()}
 		</div>
 	</tal:block>
-	<input name="${view.name}-empty-marker" type="hidden" value="1"/>
+	<input name="${view.name}-empty-marker" type="hidden" value="1" />
 </div>
```

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/orderedselect-display.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/orderedselect-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/orderedselect-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/orderedselect-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/password-display.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/password-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/password-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/password-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/radio-display-single.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/radio-display-single.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/radio-display.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/radio-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/radio-input-single.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/radio-input-single.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/select-display.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/select-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/select-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/select-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/submit-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/submit-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/text-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/text-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/textarea-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/textarea-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/textlines-display.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/textlines-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/templates/textlines-input.pt` & `pyams_form-1.8.1/src/pyams_form/interfaces/templates/textlines-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/interfaces/widget.py` & `pyams_form-1.8.1/src/pyams_form/interfaces/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.mo` & `pyams_form-1.8.1/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.mo`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.po` & `pyams_form-1.8.1/src/pyams_form/locales/fr/LC_MESSAGES/pyams_form.po`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/locales/pyams_form.pot` & `pyams_form-1.8.1/src/pyams_form/locales/pyams_form.pot`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/object.py` & `pyams_form-1.8.1/src/pyams_form/object.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/outputchecker.py` & `pyams_form-1.8.1/src/pyams_form/outputchecker.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/subform.py` & `pyams_form-1.8.1/src/pyams_form/subform.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/template.py` & `pyams_form-1.8.1/src/pyams_form/template.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/term.py` & `pyams_form-1.8.1/src/pyams_form/term.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/testing.py` & `pyams_form-1.8.1/src/pyams_form/testing.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/__init__.py` & `pyams_form-1.8.1/src/pyams_form/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/templates/file-testing-input.pt` & `pyams_form-1.8.1/src/pyams_form/tests/templates/file-testing-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/templates/integration-edit.pt` & `pyams_form-1.8.1/src/pyams_form/tests/templates/integration-edit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/templates/simple-caredit-subforms.pt` & `pyams_form-1.8.1/src/pyams_form/tests/templates/simple-caredit-subforms.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/templates/simple-caredit.pt` & `pyams_form-1.8.1/src/pyams_form/tests/templates/simple-caredit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/templates/simple-edit-with-providers.pt` & `pyams_form-1.8.1/src/pyams_form/tests/templates/simple-edit-with-providers.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/templates/simple-edit-with-subforms.pt` & `pyams_form-1.8.1/src/pyams_form/tests/templates/simple-edit-with-subforms.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/templates/simple-edit.pt` & `pyams_form-1.8.1/src/pyams_form/tests/templates/simple-edit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/templates/simple-groupedit.pt` & `pyams_form-1.8.1/src/pyams_form/tests/templates/simple-groupedit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/templates/simple-nested-groupedit.pt` & `pyams_form-1.8.1/src/pyams_form/tests/templates/simple-nested-groupedit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/templates/simple-owneredit.pt` & `pyams_form-1.8.1/src/pyams_form/tests/templates/simple-owneredit.pt`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/test_utilsdocs.py` & `pyams_form-1.8.1/src/pyams_form/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/tests/test_utilsdocstrings.py` & `pyams_form-1.8.1/src/pyams_form/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/util.py` & `pyams_form-1.8.1/src/pyams_form/util.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/validator.py` & `pyams_form-1.8.1/src/pyams_form/validator.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/value.py` & `pyams_form-1.8.1/src/pyams_form/value.py`

 * *Files identical despite different names*

### Comparing `pyams_form-1.8.0/src/pyams_form/widget.py` & `pyams_form-1.8.1/src/pyams_form/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from pyams_form.interfaces.error import IErrorViewSnippet
 from pyams_form.interfaces.form import IContextAware, IFormAware
 from pyams_form.interfaces.widget import IAfterWidgetUpdateEvent, IFieldWidget, IMultiWidget, \
     ISequenceWidget, IWidget, IWidgetEvent
 from pyams_form.template import get_widget_layout, get_widget_template
 from pyams_form.util import sorted_none
 from pyams_form.value import ComputedValueCreator, StaticValueCreator
-from pyams_utils.interfaces.form import IDataManager, NO_VALUE
+from pyams_utils.interfaces.form import IDataManager, NO_VALUE, NO_VALUE_STRING
 from pyams_utils.registry import query_utility
 
 
 __docformat__ = 'restructuredtext'
 
 
 PLACEHOLDER = object()
@@ -239,15 +239,15 @@
     based values. e.g. IList of ITextLine
     """
 
     value = ()
     terms = None
     separator = ','
 
-    no_value_token = '--NOVALUE--'
+    no_value_token = NO_VALUE_STRING
 
     @property
     def display_value(self):
         """Widget display value"""
         value = []
         for token in self.value:
             # Ignore no value entries. They are in the request only.
```

### Comparing `pyams_form-1.8.0/src/pyams_form.egg-info/PKG-INFO` & `pyams_form-1.8.1/src/pyams_form.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-form
-Version: 1.8.0
+Version: 1.8.1
 Summary: PyAMS forms management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -50,14 +50,18 @@
 ** Package API is also converted to common Python standards, using snake_case for variables and
 methods.
 
 
 Changelog
 =========
 
+1.8.1
+-----
+ - small templates updates
+
 1.8.0
 -----
  - added support for optional *factory* argument when using *form_and_handler* decorator
  - added optional *notify* argument to form *extract_data* method; you can set this argument
    to *False* when you don't want to generate extra events on a manual data extraction
 
 1.7.4
```

### Comparing `pyams_form-1.8.0/src/pyams_form.egg-info/SOURCES.txt` & `pyams_form-1.8.1/src/pyams_form.egg-info/SOURCES.txt`

 * *Files identical despite different names*

