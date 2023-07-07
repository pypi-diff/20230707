# Comparing `tmp/pyams_security_views-1.8.5.tar.gz` & `tmp/pyams_security_views-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_security_views-1.8.5.tar", last modified: Wed Apr 12 16:58:00 2023, max compression
+gzip compressed data, was "dist/pyams_security_views-1.9.1.tar", last modified: Fri Jul  7 15:33:36 2023, max compression
```

## Comparing `pyams_security_views-1.8.5.tar` & `pyams_security_views-1.9.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4070 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/docs/
--rwxrwxrwx   0 root         (0) root         (0)     2391 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2643 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/api/
--rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/api/principal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    10432 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1337 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2894 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/interfaces/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9151 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo
--rw-rw-rw-   0 root         (0) root         (0)    15221 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po
--rw-rw-rw-   0 root         (0) root         (0)    10468 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/pyams_security_views.pot
--rw-rw-rw-   0 root         (0) root         (0)     2135 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/login.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10446 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/templates/login-logo.pt
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/templates/login-viewlet.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/tests/
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1843 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1885 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/widget/
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/widget/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/widget/permission.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/widget/principal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7022 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3229 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/login.py
--rw-rw-rw-   0 root         (0) root         (0)     4652 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3237 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/notifications.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4196 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     8987 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/group.py
--rw-rw-rw-   0 root         (0) root         (0)    20959 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/userfolder.py
--rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     3578 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4070 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1998 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      284 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4203 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     2524 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2643 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/api/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3705 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/api/principal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    10293 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1337 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4913 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/interfaces/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10671 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo
+-rw-rw-rw-   0 root         (0) root         (0)    17388 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po
+-rw-rw-rw-   0 root         (0) root         (0)    11751 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/locales/pyams_security_views.pot
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12335 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/skin/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/skin/templates/login-logo.pt
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/skin/templates/login-viewlet.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/widget/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/widget/permission.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/widget/principal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7022 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4894 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/notifications.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4196 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/plugin/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/plugin/group.py
+-rw-rw-rw-   0 root         (0) root         (0)    21189 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/plugin/userfolder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5900 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2023-07-07 15:33:17.000000 pyams_security_views-1.9.1/src/pyams_security_views/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4203 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      284 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-07 15:33:36.000000 pyams_security_views-1.9.1/src/pyams_security_views.egg-info/top_level.txt
```

### Comparing `pyams_security_views-1.8.5/LICENSE` & `pyams_security_views-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/PKG-INFO` & `pyams_security_views-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_security_views
-Version: 1.8.5
+Version: 1.9.1
 Summary: Pyramid views for PyAMS_security package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -46,14 +46,23 @@
 interface (based on PyAMS_zmi package), custom widgets and a small Cornice REST API to look for
 principals.
 
 
 Changelog
 =========
 
+1.9.1
+-----
+ - updated doctests
+
+1.9.0
+-----
+ - added support for user registration
+ - added support for local user password change
+
 1.8.5
 -----
  - refactored Colander API schemas for better OpenAPI specifications
 
 1.8.4
 -----
  - updated login form templates
```

### Comparing `pyams_security_views-1.8.5/docs/HISTORY.rst` & `pyams_security_views-1.9.1/docs/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+1.9.1
+-----
+ - updated doctests
+
+1.9.0
+-----
+ - added support for user registration
+ - added support for local user password change
+
 1.8.5
 -----
  - refactored Colander API schemas for better OpenAPI specifications
 
 1.8.4
 -----
  - updated login form templates
```

### Comparing `pyams_security_views-1.8.5/docs/README.rst` & `pyams_security_views-1.9.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/setup.py` & `pyams_security_views-1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.8.5'
+version = '1.9.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'cornice_swagger',
     'pyams_i18n_views',
     'pyams_zmi',
     'pyramid_zcml',
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/__init__.py` & `pyams_security_views-1.9.1/src/pyams_security_views/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/api/__init__.py` & `pyams_security_views-1.9.1/src/pyams_security_views/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/api/principal.py` & `pyams_security_views-1.9.1/src/pyams_security_views/api/principal.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,20 @@
 
 from colander import MappingSchema, SchemaNode, SequenceSchema, String, drop
 from cornice import Service
 from cornice.validators import colander_validator
 from pyramid.httpexceptions import HTTPOk
 
 from pyams_security.interfaces import ISecurityManager
-from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
+from pyams_security.interfaces.base import USE_INTERNAL_API_PERMISSION
 from pyams_security.rest import check_cors_origin, set_cors_headers
 from pyams_security_views.interfaces import REST_PRINCIPALS_SEARCH_ROUTE
 from pyams_utils.registry import query_utility
 from pyams_utils.rest import BaseResponseSchema, STATUS, rest_responses
 
-
 __docformat__ = 'restructuredtext'
 
 
 TEST_MODE = sys.argv[-1].endswith('/test')
 
 
 class PrincipalsSearchQuery(MappingSchema):
@@ -83,15 +82,15 @@
 
 
 principals_get_responses = rest_responses.copy()
 principals_get_responses[HTTPOk.code] = PrincipalsGetterResponse(
     description="Search results")
 
 
-@principals_service.get(permission=VIEW_SYSTEM_PERMISSION,
+@principals_service.get(permission=USE_INTERNAL_API_PERMISSION,
                         schema=PrincipalsSearchRequest(),
                         validators=(check_cors_origin, colander_validator, set_cors_headers),
                         response_schemas=principals_get_responses)
 def get_principals(request):
     """Returns list of principals matching given query"""
     params = request.params if TEST_MODE else request.validated.get('querystring', {})
     query = params.get('term')
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/doctests/README.rst` & `pyams_security_views-1.9.1/src/pyams_security_views/doctests/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     >>> include_utils(config)
     >>> from pyams_viewlet import includeme as include_viewlet
     >>> include_viewlet(config)
     >>> from pyams_site import includeme as include_site
     >>> include_site(config)
     >>> from pyams_security import includeme as include_security
     >>> include_security(config)
+    >>> from pyams_layer import includeme as include_layer
+    >>> include_layer(config)
     >>> from pyams_form import includeme as include_form
     >>> include_form(config)
     >>> from pyams_skin import includeme as include_skin
     >>> include_skin(config)
     >>> from pyams_zmi import includeme as include_zmi
     >>> include_zmi(config)
     >>> from pyams_security_views import includeme as include_security_views
@@ -106,17 +108,14 @@
         </tbody>
     </table>
     <input type="hidden"
            id="form-widgets-authentication_plugins_names"
            name="form.widgets.authentication_plugins_names"
            value="__system__;__internal__" />
 
-    >>> form.groups[0].widgets.keys()
-    odict_keys(['open_registration', 'users_folder'])
-
     >>> output = form.render()
 
 
 Security policy edit form
 -------------------------
 
     >>> from pyams_security_views.zmi.policy import ProtectedObjectSecurityPolicyEditForm
@@ -167,42 +166,39 @@
     >>> request = DummyRequest(context=app)
     >>> alsoProvides(request, IAdminLayer)
 
     >>> from pyams_security_views.zmi.login import LoginFormConfigurationForm
     >>> form = LoginFormConfigurationForm(app, request)
     >>> form.update()
     >>> form.widgets.keys()
-    odict_keys(['logo', 'header', 'header_renderer', 'footer', 'footer_renderer'])
+    odict_keys(['skin', 'logo', 'header', 'header_renderer', 'footer', 'footer_renderer'])
 
     >>> output = form.render()
 
 
 Login form
 ----------
 
     >>> from pyams_layer.interfaces import IPyAMSLayer
     >>> from pyams_security_views.skin.login import LoginForm
-    >>> request = DummyRequest(is_xhr=False, params={
+    >>> request = DummyRequest(root=app, is_xhr=False, params={
     ...     'login_form.widgets.login': 'admin',
     ...     'login_form.widgets.password': 'admin',
     ...     'login_form.buttons.login': 'Connect'
     ... })
     >>> alsoProvides(request, IPyAMSLayer)
     >>> form = LoginForm(app, request)
     >>> form.update()
     >>> form.widgets.keys()
     odict_keys(['hash', 'login', 'password'])
 
     >>> output = form.render()
     >>> print(output)
-    <section class="rounded-lg"
+    <section class="rounded-lg "
              data-ams-modules="form plugins">
-        <h2 class="bg-secondary-modal d-flex flex-wrap pl-3 py-2-modal">
-            <span class="flex-grow-1">You must authenticate</span>
-        </h2>
         <form class="ams-form "
               id="login_form"
               name="login_form"
               action="http://example.com"
               method="post"
               data-async
               data-ams-data='{"ams-warn-on-change": false, "ams-modules": "callbacks helpers", "ams-callback": "MyAMS.helpers.setLoginHash"}'>
```

#### html2text {}

```diff
@@ -7,18 +7,19 @@
 include_zodbconn(config) >>> from cornice import includeme as include_cornice
 >>> include_cornice(config) >>> from cornice_swagger import includeme as
 include_swagger >>> include_swagger(config) >>> from pyams_utils import
 includeme as include_utils >>> include_utils(config) >>> from pyams_viewlet
 import includeme as include_viewlet >>> include_viewlet(config) >>> from
 pyams_site import includeme as include_site >>> include_site(config) >>> from
 pyams_security import includeme as include_security >>> include_security
-(config) >>> from pyams_form import includeme as include_form >>> include_form
-(config) >>> from pyams_skin import includeme as include_skin >>> include_skin
-(config) >>> from pyams_zmi import includeme as include_zmi >>> include_zmi
-(config) >>> from pyams_security_views import includeme as
+(config) >>> from pyams_layer import includeme as include_layer >>>
+include_layer(config) >>> from pyams_form import includeme as include_form >>>
+include_form(config) >>> from pyams_skin import includeme as include_skin >>>
+include_skin(config) >>> from pyams_zmi import includeme as include_zmi >>>
+include_zmi(config) >>> from pyams_security_views import includeme as
 include_security_views >>> include_security_views(config) >>> from
 pyams_i18n_views import includeme as include_i18n_view >>> include_i18n_view
 (config) >>> from pyams_utils.registry import get_utility, set_local_registry
 >>> registry = config.registry >>> set_local_registry(registry) >>> from
 pyams_site.generations import upgrade_site >>> request = DummyRequest() >>> app
 = upgrade_site(request) Upgrading PyAMS timezone to generation 1... Upgrading
 PyAMS security to generation 2... >>> from zope.traversing.interfaces import
@@ -41,25 +42,24 @@
 - >>> from pyams_security_views.api.principal import get_principals >>> request
 = DummyRequest(params={'term': 'admin'}) >>> pprint.pprint(get_principals
 (request)) {'results': [{'id': 'system:admin', 'text': 'System manager
 authentication'}], 'status': 'success'} Login form configuration edit form ----
 ------------------------------ >>> request = DummyRequest(context=app) >>>
 alsoProvides(request, IAdminLayer) >>> from pyams_security_views.zmi.login
 import LoginFormConfigurationForm >>> form = LoginFormConfigurationForm(app,
-request) >>> form.update() >>> form.widgets.keys() odict_keys(['logo',
+request) >>> form.update() >>> form.widgets.keys() odict_keys(['skin', 'logo',
 'header', 'header_renderer', 'footer', 'footer_renderer']) >>> output =
 form.render() Login form ---------- >>> from pyams_layer.interfaces import
 IPyAMSLayer >>> from pyams_security_views.skin.login import LoginForm >>>
-request = DummyRequest(is_xhr=False, params={ ... 'login_form.widgets.login':
-'admin', ... 'login_form.widgets.password': 'admin', ...
-'login_form.buttons.login': 'Connect' ... }) >>> alsoProvides(request,
-IPyAMSLayer) >>> form = LoginForm(app, request) >>> form.update() >>>
+request = DummyRequest(root=app, is_xhr=False, params={ ...
+'login_form.widgets.login': 'admin', ... 'login_form.widgets.password':
+'admin', ... 'login_form.buttons.login': 'Connect' ... }) >>> alsoProvides
+(request, IPyAMSLayer) >>> form = LoginForm(app, request) >>> form.update() >>>
 form.widgets.keys() odict_keys(['hash', 'login', 'password']) >>> output =
 form.render() >>> print(output)
-***** You must authenticate *****
  Please enter valid credentials
  Login
 [admin               ]
  Password
 [********************]
   Connect Reset
  Tests cleanup: >>> tearDown()
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/include.py` & `pyams_security_views-1.9.1/src/pyams_security_views/include.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/interfaces/__init__.py` & `pyams_security_views-1.9.1/src/pyams_security_views/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo` & `pyams_security_views-1.9.1/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -45,14 +45,17 @@
 
 msgid "Add local users folder..."
 msgstr "Ajouter un dossier d'utilisateurs locaux..."
 
 msgid "Add user"
 msgstr "Ajouter un utilisateur"
 
+msgid "Allow password reset"
+msgstr "Permettre la réinitialisation du mot de passe"
+
 msgid ""
 "Before disabling plug-in, you should verify that you have other "
 "administration access!"
 msgstr ""
 "Avant de désactiver ce compte, vérifiez bien que vous disposez d'au moins un "
 "autre accès administrateur !"
 
@@ -81,14 +84,17 @@
 
 msgid "Disabled user!"
 msgstr "Compte désactivé !"
 
 msgid "Enable"
 msgstr "Activer"
 
+msgid "Enable free registration?"
+msgstr "Autoriser l'inscription libre"
+
 msgid "Enabled user!"
 msgstr "Compte activé !"
 
 msgid "Footer renderer"
 msgstr "Mode de rendu"
 
 msgid "Form properties"
@@ -102,14 +108,24 @@
 
 msgid "Group: {}"
 msgstr "Groupe : {}"
 
 msgid "Header renderer"
 msgstr "Mode de rendu"
 
+msgid "If 'Yes', any use will be able to create a new user account"
+msgstr ""
+"Si 'oui', toute personne visitant le site sera à même de s'enregistrer et de "
+"faire une demande de création de compte utilisateur"
+
+msgid "If 'Yes', users will be able reset their password"
+msgstr ""
+"Si 'oui', les utilisateurs auront la possibilité de réinitialiser leur mot "
+"de passe en cas d'oubli"
+
 msgid ""
 "If you disable CORS origins check, any CORS request will be accepted.\n"
 "Otherwise, only origins specified below will be allowed.\n"
 "Please note that you don't have to set main site URL(s) below, only "
 "\"external\" URLs have to be defined."
 msgstr ""
 "Si vous désactivez le contrôle sur l'origine des requêtes, toutes les "
@@ -135,37 +151,45 @@
 msgid "Login"
 msgstr "Identifiant"
 
 msgid "Login footer"
 msgstr "Pied de page"
 
 msgid "Login form"
-msgstr "Page de connexion"
+msgstr "Écran de connexion"
 
 msgid "Login form configuration"
-msgstr "Page de connexion"
+msgstr "Configuration de l'écran de connexion"
 
 msgid "Login header"
 msgstr "Chapô"
 
 msgid "Login logo"
 msgstr "Logo de connexion"
 
+msgid "Login skin"
+msgstr "Thème graphique"
+
 msgid "Mail address"
 msgstr "Adresse de messagerie"
 
 msgid "Management interface"
 msgstr "Interface d'administration"
 
 msgid ""
 "Missing security manager utility. Please contact your system administrator!"
 msgstr ""
 "Aucun gestionnaire de sécurité n'est disponible. Veuillez contacter votre "
 "administrateur !"
 
+msgid "Name of users folder used to store registered principals"
+msgstr ""
+"Nom du module utilisé pour identifier les utilisateurs qui se seront "
+"enregistrés"
+
 msgid "New plug-in properties"
 msgstr "Propriétés du nouveau module"
 
 msgid "New plug-in: {}"
 msgstr "Nouveau module : {}"
 
 msgid "New user was created successfully!"
@@ -196,20 +220,21 @@
 msgid ""
 "Open registration can be used when you want external users to be able to "
 "freely register their user account.\n"
 "You then have to select the users folder into which their profile will be "
 "stored.\n"
 "THIS CAN BE DANGEROUS! You should enable this feature carefully..."
 msgstr ""
-"L'inscription publique peut être utilisée lorsque vous souhaitez que des "
-"utilisateurs externes de votre service puissent s'enregistrer librement.\n"
+"L'inscription libre peut être utilisée lorsque vous souhaitez que des "
+"utilisateurs externes à votre service puissent s'enregistrer librement.\n"
 "Vous devez dans ce cas sélectionner le dossier dédié dans lequel seront "
 "stockés leurs profils utilisateurs.\n"
-"ATTENTION : cette option peut être dangereuse ! Ne l'activez donc qu'avec "
-"précaution..."
+"ATTENTION : cette option peut être dangereuse et ne doit donc être activée "
+"qu'avec précaution ! Vous devez notamment vous assurer qu'aucune permission "
+"importante n'a été accordée aux utilisateurs authentifiés..."
 
 msgid "Password"
 msgstr "Mot de passe"
 
 msgid "Please enter valid credentials"
 msgstr "Paramètres de connexion"
 
@@ -233,17 +258,23 @@
 
 msgid "Refresh activation secret and send a new activation link to this user"
 msgstr "Génère une nouvelle clé d'activation qui sera envoyée à l'utilisateur"
 
 msgid "Refresh secret"
 msgstr "Réinitialiser le secret"
 
+msgid "Register"
+msgstr "Inscription"
+
 msgid "Reset"
 msgstr "Annuler"
 
+msgid "Reset password"
+msgstr "Mot de passe oublié"
+
 msgid "Roles are not defined for this context!"
 msgstr "Aucun rôle n'est défini dans ce contexte !"
 
 msgid "Search into folder"
 msgstr "Rechercher dans le dossier"
 
 msgid "Search results"
@@ -272,14 +303,20 @@
 
 msgid "Text renderer used for the footer"
 msgstr "Vous pouvez sélectionner le mode de rendu utilisé pour le pied de page"
 
 msgid "Text renderer used for the header"
 msgstr "Vous pouvez sélectionner le mode de rendu utilisé pour le chapô"
 
+msgid "This is the skin applied to the login screen"
+msgstr ""
+"Thème graphique appliqué à l'écran de connexion ; si vous choisissez "
+"l'option \"PyAMS: skin MyAMS\", c'est le thème graphique paramétré par "
+"défaut dans la configuration de la ZMI qui sera appliqué"
+
 msgid ""
 "This profile has been deactivated!<br /> A new activation code has been "
 "created and sent to this user!"
 msgstr ""
 "Le compte a été désactivé !<br />Un nouveau lien d'activation a été créé et "
 "transmis à l'utilisateur..."
 
@@ -310,15 +347,23 @@
 
 msgid "User roles"
 msgstr "Habilitations"
 
 msgid "User: {}"
 msgstr "Utilisateur : {}"
 
+msgid "Users folder"
+msgstr "Dossier d'utilisateurs"
+
 msgid "Users search form"
 msgstr "Rechercher des utilisateurs"
 
 msgid "Warning!"
 msgstr "ATTENTION !"
 
+msgid "You can't activate open registration without selecting a users folder"
+msgstr ""
+"Vous ne pouvez pas activer les fonctions d'inscription libre sans "
+"sélectionner un dossier de stockage des utilisateurs concernés"
+
 msgid "You must authenticate"
 msgstr "Vous devez vous authentifier !"
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po` & `pyams_security_views-1.9.1/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,70 +1,24 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2023-04-12 16:00+0200\n"
+"POT-Creation-Date: 2023-07-05 10:02+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 3.10.dev0\n"
 
-#: src/pyams_security_views/widget/principal.py:71
-msgid "No selected principal"
-msgstr "Aucun mandataire sélectionné"
-
-#: src/pyams_security_views/zmi/rest.py:51
-#: src/pyams_security_views/zmi/rest.py:61
-msgid "CORS configuration"
-msgstr "Configuration CORS"
-
-#: src/pyams_security_views/zmi/rest.py:96
-msgid ""
-"If you disable CORS origins check, any CORS request will be accepted.\n"
-"Otherwise, only origins specified below will be allowed.\n"
-"Please note that you don't have to set main site URL(s) below, only "
-"\"external\" URLs have to be defined."
-msgstr ""
-"Si vous désactivez le contrôle sur l'origine des requêtes, toutes les "
-"requêtes CORS seront acceptées !\n"
-"Dans le cas contraire, seules les requêtes dont l'origine est indiquée ci-"
-"dessous seront acceptées.\n"
-"Veuillez noter que vous n'avez pas à indiquer l'URL d'accès au site, celle-"
-"ci sera toujours acceptée ; seules les origines \"externes\" doivent être "
-"précisées."
-
-#: src/pyams_security_views/zmi/notifications.py:50
-msgid "Notifications"
-msgstr "Notifications"
-
-#: src/pyams_security_views/zmi/notifications.py:60
-msgid "Notifications settings"
-msgstr "Paramétrage des notifications"
-
-#: src/pyams_security_views/zmi/notifications.py:85
-msgid ""
-"Notifications are used to send messages to users during their registration "
-"process.\n"
-"Applications can also send messages during their normal process."
-msgstr ""
-"Les notifications sont utilisées pour envoyer des messages aux utilisateurs. "
-"Elles sont notamment nécessaires pour prendre en charge leur processus "
-"d'enregistrement, aussi bien lorsqu'il s'agit d'une inscription publique (si "
-"vous activez cette option) que dans le cadre d'un enregistrement par un "
-"administrateur.\n"
-"Les applications peuvent également envoyer des messages dans le cadre de "
-"leur processus de fonctionnement normal."
-
 #: src/pyams_security_views/zmi/policy.py:59
 #: src/pyams_security_views/zmi/policy.py:98
 #: src/pyams_security_views/zmi/policy.py:112
 msgid "User roles"
 msgstr "Habilitations"
 
 #: src/pyams_security_views/zmi/policy.py:67
@@ -76,34 +30,51 @@
 msgstr "Aucun rôle n'est défini dans ce contexte !"
 
 #: src/pyams_security_views/zmi/policy.py:141
 msgid "Security policy"
 msgstr "Politique de sécurité"
 
 #: src/pyams_security_views/zmi/policy.py:151
-#: src/pyams_security_views/zmi/manager.py:48
-#: src/pyams_security_views/zmi/manager.py:69
+#: src/pyams_security_views/zmi/manager.py:45
+#: src/pyams_security_views/zmi/manager.py:66
 msgid "Security manager"
 msgstr "Gestionnaire de sécurité"
 
 #: src/pyams_security_views/zmi/policy.py:152
 msgid "Security policy management"
 msgstr "Paramètres de la politique de sécurité"
 
-#: src/pyams_security_views/zmi/login.py:45
-msgid "Login form"
-msgstr "Page de connexion"
+#: src/pyams_security_views/zmi/rest.py:51
+#: src/pyams_security_views/zmi/rest.py:61
+msgid "CORS configuration"
+msgstr "Configuration CORS"
 
-#: src/pyams_security_views/zmi/login.py:54
-msgid "Login form configuration"
-msgstr "Page de connexion"
+#: src/pyams_security_views/zmi/rest.py:96
+msgid ""
+"If you disable CORS origins check, any CORS request will be accepted.\n"
+"Otherwise, only origins specified below will be allowed.\n"
+"Please note that you don't have to set main site URL(s) below, only "
+"\"external\" URLs have to be defined."
+msgstr ""
+"Si vous désactivez le contrôle sur l'origine des requêtes, toutes les "
+"requêtes CORS seront acceptées !\n"
+"Dans le cas contraire, seules les requêtes dont l'origine est indiquée ci-"
+"dessous seront acceptées.\n"
+"Veuillez noter que vous n'avez pas à indiquer l'URL d'accès au site, celle-"
+"ci sera toujours acceptée ; seules les origines \"externes\" doivent être "
+"précisées."
 
-#: src/pyams_security_views/zmi/login.py:55
-msgid "Form properties"
-msgstr "Propriétés du formulaire"
+#: src/pyams_security_views/zmi/manager.py:55
+#: src/pyams_security_views/zmi/manager.py:67
+msgid "Properties"
+msgstr "Propriétés"
+
+#: src/pyams_security_views/zmi/manager.py:83
+msgid "Management interface"
+msgstr "Interface d'administration"
 
 #: src/pyams_security_views/zmi/__init__.py:56
 #: src/pyams_security_views/zmi/__init__.py:79
 msgid "Security"
 msgstr "Sécurité"
 
 #: src/pyams_security_views/zmi/__init__.py:118
@@ -118,60 +89,63 @@
 msgid "Security plug-ins"
 msgstr "Modules de sécurité"
 
 #: src/pyams_security_views/zmi/__init__.py:193
 msgid "List of security plug-ins"
 msgstr "Liste des modules de sécurité"
 
-#: src/pyams_security_views/zmi/manager.py:58
-#: src/pyams_security_views/zmi/manager.py:70
-msgid "Properties"
-msgstr "Propriétés"
+#: src/pyams_security_views/zmi/login.py:50
+msgid "Login form"
+msgstr "Écran de connexion"
+
+#: src/pyams_security_views/zmi/login.py:60
+msgid "Login form configuration"
+msgstr "Configuration de l'écran de connexion"
+
+#: src/pyams_security_views/zmi/login.py:61
+msgid "Form properties"
+msgstr "Propriétés du formulaire"
 
-#: src/pyams_security_views/zmi/manager.py:97
+#: src/pyams_security_views/zmi/login.py:96
 msgid ""
 "Open registration can be used when you want external users to be able to "
 "freely register their user account.\n"
 "You then have to select the users folder into which their profile will be "
 "stored.\n"
 "THIS CAN BE DANGEROUS! You should enable this feature carefully..."
 msgstr ""
-"L'inscription publique peut être utilisée lorsque vous souhaitez que des "
-"utilisateurs externes de votre service puissent s'enregistrer librement.\n"
+"L'inscription libre peut être utilisée lorsque vous souhaitez que des "
+"utilisateurs externes à votre service puissent s'enregistrer librement.\n"
 "Vous devez dans ce cas sélectionner le dossier dédié dans lequel seront "
 "stockés leurs profils utilisateurs.\n"
-"ATTENTION : cette option peut être dangereuse ! Ne l'activez donc qu'avec "
-"précaution..."
-
-#: src/pyams_security_views/zmi/manager.py:110
-msgid "Management interface"
-msgstr "Interface d'administration"
-
-#: src/pyams_security_views/zmi/plugin/__init__.py:66
-#, python-format
-msgid "New plug-in: {}"
-msgstr "Nouveau module : {}"
-
-#: src/pyams_security_views/zmi/plugin/__init__.py:68
-msgid "New plug-in properties"
-msgstr "Propriétés du nouveau module"
+"ATTENTION : cette option peut être dangereuse et ne doit donc être activée "
+"qu'avec précaution ! Vous devez notamment vous assurer qu'aucune permission "
+"importante n'a été accordée aux utilisateurs authentifiés..."
 
-#: src/pyams_security_views/zmi/plugin/__init__.py:97
-msgid "Specified prefix is already used!"
-msgstr "Le préfixe indiqué est déjà utilisé !"
+#: src/pyams_security_views/zmi/notifications.py:50
+msgid "Notifications"
+msgstr "Notifications"
 
-#: src/pyams_security_views/zmi/plugin/__init__.py:136
-#: src/pyams_security_views/zmi/plugin/__init__.py:163
-#, python-format
-msgid "Plug-in: {}"
-msgstr "Module : {}"
+#: src/pyams_security_views/zmi/notifications.py:60
+msgid "Notifications settings"
+msgstr "Paramétrage des notifications"
 
-#: src/pyams_security_views/zmi/plugin/__init__.py:165
-msgid "Plug-in properties"
-msgstr "Propriétés du module"
+#: src/pyams_security_views/zmi/notifications.py:85
+msgid ""
+"Notifications are used to send messages to users during their registration "
+"process.\n"
+"Applications can also send messages during their normal process."
+msgstr ""
+"Les notifications sont utilisées pour envoyer des messages aux utilisateurs. "
+"Elles sont notamment nécessaires pour prendre en charge leur processus "
+"d'enregistrement, aussi bien lorsqu'il s'agit d'une inscription publique (si "
+"vous activez cette option) que dans le cadre d'un enregistrement par un "
+"administrateur.\n"
+"Les applications peuvent également envoyer des messages dans le cadre de "
+"leur processus de fonctionnement normal."
 
 #: src/pyams_security_views/zmi/plugin/group.py:65
 msgid "Add groups folder..."
 msgstr "Ajouter un dossier de groupes..."
 
 #: src/pyams_security_views/zmi/plugin/group.py:103
 #: src/pyams_security_views/zmi/plugin/userfolder.py:153
@@ -210,15 +184,15 @@
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:100
 #: src/pyams_security_views/zmi/plugin/userfolder.py:114
 msgid "Users search form"
 msgstr "Rechercher des utilisateurs"
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:141
-#: src/pyams_security_views/interfaces/login.py:69
+#: src/pyams_security_views/interfaces/login.py:101
 msgid "Login"
 msgstr "Identifiant"
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:165
 msgid "Mail address"
 msgstr "Adresse de messagerie"
 
@@ -239,15 +213,15 @@
 msgstr "Ajouter un utilisateur"
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:247
 msgid "Add local user"
 msgstr "Ajouter un utilisateur"
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:281
-#: src/pyams_security_views/zmi/plugin/userfolder.py:556
+#: src/pyams_security_views/zmi/plugin/userfolder.py:560
 msgid "User password was not confirmed correctly."
 msgstr "Le mot de passe n'a pas été confirmé correctement."
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:295
 msgid "New user was created successfully!"
 msgstr "Le compte utilisateur a été créé avec succès !"
 
@@ -264,15 +238,15 @@
 msgstr "Activer"
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:314
 msgid "Disable"
 msgstr "Désactiver"
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:328
-#: src/pyams_security_views/zmi/plugin/userfolder.py:543
+#: src/pyams_security_views/zmi/plugin/userfolder.py:547
 #, python-format
 msgid "User: {}"
 msgstr "Utilisateur : {}"
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:330
 msgid "User properties"
 msgstr "Propriétés de l'utilisateur"
@@ -287,43 +261,43 @@
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:368
 msgid "Disable user profile temporarily will forbid login with this account..."
 msgstr ""
 "Désactiver ce compte utilisateur empêchera toute connexion jusqu'à sa "
 "réactivation..."
 
-#: src/pyams_security_views/zmi/plugin/userfolder.py:452
+#: src/pyams_security_views/zmi/plugin/userfolder.py:456
 msgid ""
 "This profile has been deactivated!<br /> A new activation code has been "
 "created and sent to this user!"
 msgstr ""
 "Le compte a été désactivé !<br />Un nouveau lien d'activation a été créé et "
 "transmis à l'utilisateur..."
 
-#: src/pyams_security_views/zmi/plugin/userfolder.py:480
+#: src/pyams_security_views/zmi/plugin/userfolder.py:484
 msgid "Enabled user!"
 msgstr "Compte activé !"
 
-#: src/pyams_security_views/zmi/plugin/userfolder.py:482
+#: src/pyams_security_views/zmi/plugin/userfolder.py:486
 msgid "User has been enabled and can now log-in!"
 msgstr ""
 "Le compte utilisateur a été activé et peut maintenant être utilisé pour se "
 "connecter !"
 
-#: src/pyams_security_views/zmi/plugin/userfolder.py:508
+#: src/pyams_security_views/zmi/plugin/userfolder.py:512
 msgid "Disabled user!"
 msgstr "Compte désactivé !"
 
-#: src/pyams_security_views/zmi/plugin/userfolder.py:510
+#: src/pyams_security_views/zmi/plugin/userfolder.py:514
 msgid "User has been disabled and can't log in anymore!"
 msgstr ""
 "Le compte utilisateur a été désactivé et ne peut plus être utilisé pour se "
 "connecter..."
 
-#: src/pyams_security_views/zmi/plugin/userfolder.py:545
+#: src/pyams_security_views/zmi/plugin/userfolder.py:549
 msgid "Change user password"
 msgstr "Modifier le mot de passe"
 
 #: src/pyams_security_views/zmi/plugin/admin.py:46
 msgid "Add admin authentication..."
 msgstr "Ajouter un utilisateur système..."
 
@@ -348,94 +322,178 @@
 msgstr ""
 "<strong>Prenez soin de bien redéfinir le mot de passe lorsque vous utilisez "
 "certains navigateurs qui forcent l'auto-complétion !!!</strong><br />En "
 "effaçant le mot de passe, le compte restera actif mais sans possibilité de "
 "se connecter (il restera utilisable pour des tâches internes) ; en indiquant "
 "la valeur '*****', le mot de passe ne sera pas modifié..."
 
-#: src/pyams_security_views/skin/login.py:83
-msgid "You must authenticate"
-msgstr "Vous devez vous authentifier !"
+#: src/pyams_security_views/zmi/plugin/__init__.py:66
+#, python-format
+msgid "New plug-in: {}"
+msgstr "Nouveau module : {}"
 
-#: src/pyams_security_views/skin/login.py:84
-msgid "Please enter valid credentials"
-msgstr "Paramètres de connexion"
+#: src/pyams_security_views/zmi/plugin/__init__.py:68
+msgid "New plug-in properties"
+msgstr "Propriétés du nouveau module"
 
-#: src/pyams_security_views/skin/login.py:153
-msgid ""
-"Missing security manager utility. Please contact your system administrator!"
-msgstr ""
-"Aucun gestionnaire de sécurité n'est disponible. Veuillez contacter votre "
-"administrateur !"
+#: src/pyams_security_views/zmi/plugin/__init__.py:97
+msgid "Specified prefix is already used!"
+msgstr "Le préfixe indiqué est déjà utilisé !"
 
-#: src/pyams_security_views/skin/login.py:159
-msgid "Invalid credentials!"
-msgstr "Vos paramètres de connexion sont incorrects !"
+#: src/pyams_security_views/zmi/plugin/__init__.py:136
+#: src/pyams_security_views/zmi/plugin/__init__.py:163
+#, python-format
+msgid "Plug-in: {}"
+msgstr "Module : {}"
+
+#: src/pyams_security_views/zmi/plugin/__init__.py:165
+msgid "Plug-in properties"
+msgstr "Propriétés du module"
+
+#: src/pyams_security_views/interfaces/login.py:37
+msgid "Login skin"
+msgstr "Thème graphique"
 
-#: src/pyams_security_views/interfaces/login.py:34
+#: src/pyams_security_views/interfaces/login.py:38
+msgid "This is the skin applied to the login screen"
+msgstr ""
+"Thème graphique appliqué à l'écran de connexion ; si vous choisissez "
+"l'option \"PyAMS: skin MyAMS\", c'est le thème graphique paramétré par "
+"défaut dans la configuration de la ZMI qui sera appliqué"
+
+#: src/pyams_security_views/interfaces/login.py:43
 msgid "Login logo"
 msgstr "Logo de connexion"
 
-#: src/pyams_security_views/interfaces/login.py:35
+#: src/pyams_security_views/interfaces/login.py:44
 msgid "Image used in login form"
 msgstr "Image affichée dans le formulaire de connexion"
 
-#: src/pyams_security_views/interfaces/login.py:38
+#: src/pyams_security_views/interfaces/login.py:47
 msgid "Login header"
 msgstr "Chapô"
 
-#: src/pyams_security_views/interfaces/login.py:39
+#: src/pyams_security_views/interfaces/login.py:48
 msgid "This text will be displayed in login page header"
 msgstr "Ce texte sera affiché au-dessus du formulaire de connexion"
 
-#: src/pyams_security_views/interfaces/login.py:42
+#: src/pyams_security_views/interfaces/login.py:51
 msgid "Header renderer"
 msgstr "Mode de rendu"
 
-#: src/pyams_security_views/interfaces/login.py:43
+#: src/pyams_security_views/interfaces/login.py:52
 msgid "Text renderer used for the header"
 msgstr "Vous pouvez sélectionner le mode de rendu utilisé pour le chapô"
 
-#: src/pyams_security_views/interfaces/login.py:48
+#: src/pyams_security_views/interfaces/login.py:57
 msgid "Login footer"
 msgstr "Pied de page"
 
-#: src/pyams_security_views/interfaces/login.py:49
+#: src/pyams_security_views/interfaces/login.py:58
 msgid "This text will be displayed in login page footer"
 msgstr "Ce texte sera affiché en-dessous du formulaire de connexion"
 
-#: src/pyams_security_views/interfaces/login.py:52
+#: src/pyams_security_views/interfaces/login.py:61
 msgid "Footer renderer"
 msgstr "Mode de rendu"
 
-#: src/pyams_security_views/interfaces/login.py:53
+#: src/pyams_security_views/interfaces/login.py:62
 msgid "Text renderer used for the footer"
 msgstr "Vous pouvez sélectionner le mode de rendu utilisé pour le pied de page"
 
-#: src/pyams_security_views/interfaces/login.py:66
+#: src/pyams_security_views/interfaces/login.py:67
+msgid "Enable free registration?"
+msgstr "Autoriser l'inscription libre"
+
+#: src/pyams_security_views/interfaces/login.py:68
+msgid "If 'Yes', any use will be able to create a new user account"
+msgstr ""
+"Si 'oui', toute personne visitant le site sera à même de s'enregistrer et de "
+"faire une demande de création de compte utilisateur"
+
+#: src/pyams_security_views/interfaces/login.py:73
+msgid "Users folder"
+msgstr "Dossier d'utilisateurs"
+
+#: src/pyams_security_views/interfaces/login.py:74
+msgid "Name of users folder used to store registered principals"
+msgstr ""
+"Nom du module utilisé pour identifier les utilisateurs qui se seront "
+"enregistrés"
+
+#: src/pyams_security_views/interfaces/login.py:82
+msgid "You can't activate open registration without selecting a users folder"
+msgstr ""
+"Vous ne pouvez pas activer les fonctions d'inscription libre sans "
+"sélectionner un dossier de stockage des utilisateurs concernés"
+
+#: src/pyams_security_views/interfaces/login.py:85
+msgid "Allow password reset"
+msgstr "Permettre la réinitialisation du mot de passe"
+
+#: src/pyams_security_views/interfaces/login.py:86
+msgid "If 'Yes', users will be able reset their password"
+msgstr ""
+"Si 'oui', les utilisateurs auront la possibilité de réinitialiser leur mot "
+"de passe en cas d'oubli"
+
+#: src/pyams_security_views/interfaces/login.py:98
 msgid "Redirection hash"
 msgstr "Hash de redirection"
 
-#: src/pyams_security_views/interfaces/login.py:71
+#: src/pyams_security_views/interfaces/login.py:103
 msgid "Password"
 msgstr "Mot de passe"
 
-#: src/pyams_security_views/interfaces/login.py:78
-#: src/pyams_security_views/interfaces/login.py:88
+#: src/pyams_security_views/interfaces/login.py:110
+#: src/pyams_security_views/interfaces/login.py:126
+msgid "Register"
+msgstr "Inscription"
+
+#: src/pyams_security_views/interfaces/login.py:113
+#: src/pyams_security_views/interfaces/login.py:129
+msgid "Reset password"
+msgstr "Mot de passe oublié"
+
+#: src/pyams_security_views/interfaces/login.py:116
+#: src/pyams_security_views/interfaces/login.py:132
 msgid "Connect"
 msgstr "Connexion"
 
-#: src/pyams_security_views/interfaces/login.py:81
+#: src/pyams_security_views/interfaces/login.py:119
 msgid "Reset"
 msgstr "Annuler"
 
-#: src/pyams_security_views/interfaces/login.py:91
+#: src/pyams_security_views/interfaces/login.py:135
 msgid "Cancel"
 msgstr "Annuler"
 
+#: src/pyams_security_views/widget/principal.py:71
+msgid "No selected principal"
+msgstr "Aucun mandataire sélectionné"
+
+#: src/pyams_security_views/skin/login.py:95
+msgid "Please enter valid credentials"
+msgstr "Paramètres de connexion"
+
+#: src/pyams_security_views/skin/login.py:110
+msgid "You must authenticate"
+msgstr "Vous devez vous authentifier !"
+
+#: src/pyams_security_views/skin/login.py:219
+msgid ""
+"Missing security manager utility. Please contact your system administrator!"
+msgstr ""
+"Aucun gestionnaire de sécurité n'est disponible. Veuillez contacter votre "
+"administrateur !"
+
+#: src/pyams_security_views/skin/login.py:225
+msgid "Invalid credentials!"
+msgstr "Vos paramètres de connexion sont incorrects !"
+
 #~ msgid "Principals search string"
 #~ msgstr "Requête de recherche des mandataires"
 
 #~ msgid "Principal ID"
 #~ msgstr "ID du mandataire"
 
 #~ msgid "Principal title"
@@ -446,17 +504,14 @@
 
 #~ msgid "Groups folder plug-in"
 #~ msgstr "Groupes d'utilisateurs"
 
 #~ msgid "System authentication plug-in"
 #~ msgstr "Utilisateur système"
 
-#~ msgid "Users folder plug-in"
-#~ msgstr "Dossier d'utilisateurs"
-
 #~ msgid "Add groups folder plug-in"
 #~ msgstr "Ajouter un dossier de groupes d'utilisateurs"
 
 #~ msgid "Add admin authentication plug-in"
 #~ msgstr "Ajouter un utilisateur système"
 
 #~ msgid "Add users folder plug-in"
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/locales/pyams_security_views.pot` & `pyams_security_views-1.9.1/src/pyams_security_views/locales/pyams_security_views.pot`

 * *Files 2% similar despite different names*

```diff
@@ -2,54 +2,24 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2023-04-12 16:00+0200\n"
+"POT-Creation-Date: 2023-07-05 10:02+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.15.0\n"
 
-#: ./src/pyams_security_views/widget/principal.py:71
-msgid "No selected principal"
-msgstr ""
-
-#: ./src/pyams_security_views/zmi/rest.py:51
-#: ./src/pyams_security_views/zmi/rest.py:61
-msgid "CORS configuration"
-msgstr ""
-
-#: ./src/pyams_security_views/zmi/rest.py:96
-msgid ""
-"If you disable CORS origins check, any CORS request will be accepted.\n"
-"Otherwise, only origins specified below will be allowed.\n"
-"Please note that you don't have to set main site URL(s) below, only \"external\" URLs have to be defined."
-msgstr ""
-
-#: ./src/pyams_security_views/zmi/notifications.py:50
-msgid "Notifications"
-msgstr ""
-
-#: ./src/pyams_security_views/zmi/notifications.py:60
-msgid "Notifications settings"
-msgstr ""
-
-#: ./src/pyams_security_views/zmi/notifications.py:85
-msgid ""
-"Notifications are used to send messages to users during their registration process.\n"
-"Applications can also send messages during their normal process."
-msgstr ""
-
 #: ./src/pyams_security_views/zmi/policy.py:59
 #: ./src/pyams_security_views/zmi/policy.py:98
 #: ./src/pyams_security_views/zmi/policy.py:112
 msgid "User roles"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/policy.py:67
@@ -61,33 +31,42 @@
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/policy.py:141
 msgid "Security policy"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/policy.py:151
-#: ./src/pyams_security_views/zmi/manager.py:48
-#: ./src/pyams_security_views/zmi/manager.py:69
+#: ./src/pyams_security_views/zmi/manager.py:45
+#: ./src/pyams_security_views/zmi/manager.py:66
 msgid "Security manager"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/policy.py:152
 msgid "Security policy management"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/login.py:45
-msgid "Login form"
+#: ./src/pyams_security_views/zmi/rest.py:51
+#: ./src/pyams_security_views/zmi/rest.py:61
+msgid "CORS configuration"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/login.py:54
-msgid "Login form configuration"
+#: ./src/pyams_security_views/zmi/rest.py:96
+msgid ""
+"If you disable CORS origins check, any CORS request will be accepted.\n"
+"Otherwise, only origins specified below will be allowed.\n"
+"Please note that you don't have to set main site URL(s) below, only \"external\" URLs have to be defined."
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/login.py:55
-msgid "Form properties"
+#: ./src/pyams_security_views/zmi/manager.py:55
+#: ./src/pyams_security_views/zmi/manager.py:67
+msgid "Properties"
+msgstr ""
+
+#: ./src/pyams_security_views/zmi/manager.py:83
+msgid "Management interface"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/__init__.py:56
 #: ./src/pyams_security_views/zmi/__init__.py:79
 msgid "Security"
 msgstr ""
 
@@ -103,51 +82,45 @@
 msgid "Security plug-ins"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/__init__.py:193
 msgid "List of security plug-ins"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/manager.py:58
-#: ./src/pyams_security_views/zmi/manager.py:70
-msgid "Properties"
-msgstr ""
-
-#: ./src/pyams_security_views/zmi/manager.py:97
-msgid ""
-"Open registration can be used when you want external users to be able to freely register their user account.\n"
-"You then have to select the users folder into which their profile will be stored.\n"
-"THIS CAN BE DANGEROUS! You should enable this feature carefully..."
+#: ./src/pyams_security_views/zmi/login.py:50
+msgid "Login form"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/manager.py:110
-msgid "Management interface"
+#: ./src/pyams_security_views/zmi/login.py:60
+msgid "Login form configuration"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/__init__.py:66
-#, python-format
-msgid "New plug-in: {}"
+#: ./src/pyams_security_views/zmi/login.py:61
+msgid "Form properties"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/__init__.py:68
-msgid "New plug-in properties"
+#: ./src/pyams_security_views/zmi/login.py:96
+msgid ""
+"Open registration can be used when you want external users to be able to freely register their user account.\n"
+"You then have to select the users folder into which their profile will be stored.\n"
+"THIS CAN BE DANGEROUS! You should enable this feature carefully..."
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/__init__.py:97
-msgid "Specified prefix is already used!"
+#: ./src/pyams_security_views/zmi/notifications.py:50
+msgid "Notifications"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/__init__.py:136
-#: ./src/pyams_security_views/zmi/plugin/__init__.py:163
-#, python-format
-msgid "Plug-in: {}"
+#: ./src/pyams_security_views/zmi/notifications.py:60
+msgid "Notifications settings"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/__init__.py:165
-msgid "Plug-in properties"
+#: ./src/pyams_security_views/zmi/notifications.py:85
+msgid ""
+"Notifications are used to send messages to users during their registration process.\n"
+"Applications can also send messages during their normal process."
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/group.py:65
 msgid "Add groups folder..."
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/group.py:103
@@ -187,15 +160,15 @@
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:100
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:114
 msgid "Users search form"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:141
-#: ./src/pyams_security_views/interfaces/login.py:69
+#: ./src/pyams_security_views/interfaces/login.py:101
 msgid "Login"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:165
 msgid "Mail address"
 msgstr ""
 
@@ -216,15 +189,15 @@
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:247
 msgid "Add local user"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:281
-#: ./src/pyams_security_views/zmi/plugin/userfolder.py:556
+#: ./src/pyams_security_views/zmi/plugin/userfolder.py:560
 msgid "User password was not confirmed correctly."
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:295
 msgid "New user was created successfully!"
 msgstr ""
 
@@ -241,15 +214,15 @@
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:314
 msgid "Disable"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:328
-#: ./src/pyams_security_views/zmi/plugin/userfolder.py:543
+#: ./src/pyams_security_views/zmi/plugin/userfolder.py:547
 #, python-format
 msgid "User: {}"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:330
 msgid "User properties"
 msgstr ""
@@ -262,37 +235,37 @@
 msgid "Re-enable user profile"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:368
 msgid "Disable user profile temporarily will forbid login with this account..."
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/userfolder.py:452
+#: ./src/pyams_security_views/zmi/plugin/userfolder.py:456
 msgid ""
 "This profile has been deactivated!<br /> A new activation code has been "
 "created and sent to this user!"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/userfolder.py:480
+#: ./src/pyams_security_views/zmi/plugin/userfolder.py:484
 msgid "Enabled user!"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/userfolder.py:482
+#: ./src/pyams_security_views/zmi/plugin/userfolder.py:486
 msgid "User has been enabled and can now log-in!"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/userfolder.py:508
+#: ./src/pyams_security_views/zmi/plugin/userfolder.py:512
 msgid "Disabled user!"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/userfolder.py:510
+#: ./src/pyams_security_views/zmi/plugin/userfolder.py:514
 msgid "User has been disabled and can't log in anymore!"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/userfolder.py:545
+#: ./src/pyams_security_views/zmi/plugin/userfolder.py:549
 msgid "Change user password"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/admin.py:46
 msgid "Add admin authentication..."
 msgstr ""
 
@@ -310,84 +283,157 @@
 msgid ""
 "<strong>Be careful to redefine the password when using some browsers which "
 "are forcing autocompletion!!!</strong><br />Clearing the password will keep "
 "the plug-in active but without the option to log-in with this account; "
 "setting the password value to '*****' will leave the password as-is..."
 msgstr ""
 
-#: ./src/pyams_security_views/skin/login.py:83
-msgid "You must authenticate"
+#: ./src/pyams_security_views/zmi/plugin/__init__.py:66
+#, python-format
+msgid "New plug-in: {}"
 msgstr ""
 
-#: ./src/pyams_security_views/skin/login.py:84
-msgid "Please enter valid credentials"
+#: ./src/pyams_security_views/zmi/plugin/__init__.py:68
+msgid "New plug-in properties"
 msgstr ""
 
-#: ./src/pyams_security_views/skin/login.py:153
-msgid ""
-"Missing security manager utility. Please contact your system administrator!"
+#: ./src/pyams_security_views/zmi/plugin/__init__.py:97
+msgid "Specified prefix is already used!"
 msgstr ""
 
-#: ./src/pyams_security_views/skin/login.py:159
-msgid "Invalid credentials!"
+#: ./src/pyams_security_views/zmi/plugin/__init__.py:136
+#: ./src/pyams_security_views/zmi/plugin/__init__.py:163
+#, python-format
+msgid "Plug-in: {}"
+msgstr ""
+
+#: ./src/pyams_security_views/zmi/plugin/__init__.py:165
+msgid "Plug-in properties"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:37
+msgid "Login skin"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:34
+#: ./src/pyams_security_views/interfaces/login.py:38
+msgid "This is the skin applied to the login screen"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:43
 msgid "Login logo"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:35
+#: ./src/pyams_security_views/interfaces/login.py:44
 msgid "Image used in login form"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:38
+#: ./src/pyams_security_views/interfaces/login.py:47
 msgid "Login header"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:39
+#: ./src/pyams_security_views/interfaces/login.py:48
 msgid "This text will be displayed in login page header"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:42
+#: ./src/pyams_security_views/interfaces/login.py:51
 msgid "Header renderer"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:43
+#: ./src/pyams_security_views/interfaces/login.py:52
 msgid "Text renderer used for the header"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:48
+#: ./src/pyams_security_views/interfaces/login.py:57
 msgid "Login footer"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:49
+#: ./src/pyams_security_views/interfaces/login.py:58
 msgid "This text will be displayed in login page footer"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:52
+#: ./src/pyams_security_views/interfaces/login.py:61
 msgid "Footer renderer"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:53
+#: ./src/pyams_security_views/interfaces/login.py:62
 msgid "Text renderer used for the footer"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:66
+#: ./src/pyams_security_views/interfaces/login.py:67
+msgid "Enable free registration?"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:68
+msgid "If 'Yes', any use will be able to create a new user account"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:73
+msgid "Users folder"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:74
+msgid "Name of users folder used to store registered principals"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:82
+msgid "You can't activate open registration without selecting a users folder"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:85
+msgid "Allow password reset"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:86
+msgid "If 'Yes', users will be able reset their password"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:98
 msgid "Redirection hash"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:71
+#: ./src/pyams_security_views/interfaces/login.py:103
 msgid "Password"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:78
-#: ./src/pyams_security_views/interfaces/login.py:88
+#: ./src/pyams_security_views/interfaces/login.py:110
+#: ./src/pyams_security_views/interfaces/login.py:126
+msgid "Register"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:113
+#: ./src/pyams_security_views/interfaces/login.py:129
+msgid "Reset password"
+msgstr ""
+
+#: ./src/pyams_security_views/interfaces/login.py:116
+#: ./src/pyams_security_views/interfaces/login.py:132
 msgid "Connect"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:81
+#: ./src/pyams_security_views/interfaces/login.py:119
 msgid "Reset"
 msgstr ""
 
-#: ./src/pyams_security_views/interfaces/login.py:91
+#: ./src/pyams_security_views/interfaces/login.py:135
 msgid "Cancel"
 msgstr ""
+
+#: ./src/pyams_security_views/widget/principal.py:71
+msgid "No selected principal"
+msgstr ""
+
+#: ./src/pyams_security_views/skin/login.py:95
+msgid "Please enter valid credentials"
+msgstr ""
+
+#: ./src/pyams_security_views/skin/login.py:110
+msgid "You must authenticate"
+msgstr ""
+
+#: ./src/pyams_security_views/skin/login.py:219
+msgid ""
+"Missing security manager utility. Please contact your system administrator!"
+msgstr ""
+
+#: ./src/pyams_security_views/skin/login.py:225
+msgid "Invalid credentials!"
+msgstr ""
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/login.py` & `pyams_security_views-1.9.1/src/pyams_security_views/login.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,19 +28,23 @@
 __docformat__ = 'restructuredtext'
 
 
 @factory_config(ILoginConfiguration)
 class LoginConfiguration(Persistent, Contained):
     """Site login configuration"""
 
+    skin = FieldProperty(ILoginConfiguration['skin'])
     logo = FileProperty(ILoginConfiguration['logo'])
     header = FieldProperty(ILoginConfiguration['header'])
     header_renderer = FieldProperty(ILoginConfiguration['header_renderer'])
     footer = FieldProperty(ILoginConfiguration['footer'])
     footer_renderer = FieldProperty(ILoginConfiguration['footer_renderer'])
+    open_registration = FieldProperty(ILoginConfiguration['open_registration'])
+    users_folder = FieldProperty(ILoginConfiguration['users_folder'])
+    allow_password_reset = FieldProperty(ILoginConfiguration['allow_password_reset'])
 
 
 LOGIN_CONFIGURATION_KEY = 'pyams_security.login.configuration'
 """Annotations key used to store login configuration"""
 
 
 @adapter_config(required=ISiteRoot, provides=ILoginConfiguration)
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/site.py` & `pyams_security_views-1.9.1/src/pyams_security_views/site.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/skin/__init__.py` & `pyams_security_views-1.9.1/src/pyams_security_views/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/skin/login.py` & `pyams_security_views-1.9.1/src/pyams_security_views/skin/login.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
 """PyAMS_security_views.skin.login module
 
-This modules defines login and modal login views.
+This module defines login and modal login views.
 These views are automatically associated with Pyramid forbidden views.
 """
 
 from pyramid.csrf import new_csrf_token
 from pyramid.decorator import reify
 from pyramid.events import subscriber
 from pyramid.httpexceptions import HTTPForbidden, HTTPFound
@@ -25,92 +25,144 @@
 from pyramid.view import forbidden_view_config, view_config
 from zope.interface import Interface, Invalid, implementer
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_form.ajax import ajax_form_config
 from pyams_form.button import Buttons, handler
 from pyams_form.field import Fields
+from pyams_form.form import AddForm
 from pyams_form.interfaces import HIDDEN_MODE
 from pyams_form.interfaces.form import IAJAXFormRenderer, IDataExtractedEvent
 from pyams_i18n.interfaces import II18n
-from pyams_layer.interfaces import IPyAMSLayer, IResources
+from pyams_layer.interfaces import IPyAMSLayer
+from pyams_layer.skin import apply_skin
 from pyams_security.credential import Credentials
 from pyams_security.interfaces import ISecurityManager, LOGIN_REFERER_KEY
 from pyams_security_views.interfaces.login import ILoginConfiguration, ILoginFormButtons, \
-    ILoginFormFields, ILoginView, IModalLoginFormButtons
+    ILoginFormFields, ILoginPageTarget, ILoginView, IModalLoginFormButtons
+from pyams_security.interfaces.profile import IUserRegistrationViews
 from pyams_skin.interfaces.view import IModalFullPage, IModalPage
 from pyams_skin.interfaces.viewlet import IFooterViewletManager, IHeaderViewletManager
 from pyams_template.template import template_config
 from pyams_utils.adapter import ContextRequestViewAdapter, NullAdapter, adapter_config
 from pyams_utils.interfaces.data import IObjectData
 from pyams_utils.registry import query_utility
 from pyams_utils.text import text_to_html
 from pyams_viewlet.manager import viewletmanager_config
 from pyams_viewlet.viewlet import Viewlet, viewlet_config
-from pyams_zmi.form import AdminAddForm
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.zmi.viewlet.toolbar import ModalToolbarViewletManager
 
-
 __docformat__ = 'restructuredtext'
 
 from pyams_security_views import _  # pylint: disable=ungrouped-imports
 
 
 @forbidden_view_config(request_type=IPyAMSLayer)
 def ForbiddenView(request):  # pylint: disable=invalid-name
     """Default forbidden view"""
     request.session[LOGIN_REFERER_KEY] = request.url
-    return HTTPFound('login.html')
+    return HTTPFound('login.html?forbidden=true')
 
 
 @forbidden_view_config(request_type=IPyAMSLayer, renderer='json', xhr=True)
 def ForbiddenAJAXView(request):  # pylint: disable=invalid-name
     """AJAX forbidden view"""
     request.response.status = HTTPForbidden.code
     return {
         'status': 'modal',
-        'location': 'login-dialog.html'
+        'location': 'login-dialog.html?forbidden=true'
     }
 
 
+def get_login_buttons(interface, request):
+    """Login buttons getter"""
+    buttons = Buttons(interface)
+    login_configuration = ILoginConfiguration(request.root)
+    if not login_configuration.open_registration:
+        buttons = buttons.omit('register')
+    if not login_configuration.allow_password_reset:
+        buttons = buttons.omit('reset_password')
+    return buttons
+
+
 @ajax_form_config(name='login.html',
                   layer=IPyAMSLayer)  # pylint: disable=abstract-method
 @implementer(IModalFullPage, ILoginView, IObjectData)
-class LoginForm(AdminAddForm):
+class LoginForm(AddForm):
     """Login form"""
 
     prefix = 'login_form.'
-    title = _("You must authenticate")
     legend = _("Please enter valid credentials")
 
     modal_class = FieldProperty(IModalFullPage['modal_class'])
 
     fields = Fields(ILoginFormFields)
-    buttons = Buttons(ILoginFormButtons)
+
+    def __init__(self, context, request):
+        super().__init__(context, request)
+        login_config = ILoginConfiguration(self.request.root)
+        apply_skin(self.request, login_config.skin)
+
+    @reify
+    def title(self):
+        """Form title getter"""
+        if 'forbidden' in self.request.params:
+            return _("You must authenticate")
+        return None
+
+    @property
+    def title_class(self):
+        return 'alert alert-info' if self.title else ''
+
+    @property
+    def buttons(self):
+        """Form buttons getter"""
+        return get_login_buttons(ILoginFormButtons, self.request)
 
     edit_permission = None
 
     object_data = {
         'ams-warn-on-change': False,
         'ams-modules': 'callbacks helpers',
         'ams-callback': 'MyAMS.helpers.setLoginHash'
     }
 
     def update(self):
         super().update()
         new_csrf_token(self.request)
 
+    def update_actions(self):
+        super().update_actions()
+        registration_views = self.request.registry.queryMultiAdapter((self.context, self.request),
+                                                                     IUserRegistrationViews)
+        action = self.actions.get('register')
+        if action is not None:
+            if registration_views is None:
+                action.add_class('hidden')
+            else:
+                action.add_class('btn-info')
+                if 'reset_password' not in self.actions:
+                    action.add_class('mr-auto')
+                action.href = registration_views.register_view
+        action = self.actions.get('reset_password')
+        if action is not None:
+            if registration_views is None:
+                action.add_class('hidden')
+            else:
+                action.add_class('btn-secondary mr-auto')
+                action.href = registration_views.password_reset_view
+
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         hash = self.widgets.get('hash')
         if hash is not None:
             hash.mode = HIDDEN_MODE
 
-    @handler(buttons['login'])
+    @handler(ILoginFormButtons['login'])
     def login_handler(self, action):  # pylint: disable=unused-argument
         """Login button handler"""
         data, errors = self.extract_data()
         if errors:
             self.status = self.form_errors_message
             return None
         principal_id = data.get('principal_id')
@@ -119,31 +171,45 @@
             headers = remember(request, principal_id)
             response = request.response
             response.headerlist.extend(headers)
             if not self.request.is_xhr:
                 response.status_code = 302
                 session = request.session
                 hash = data.get('hash', '')
-                if LOGIN_REFERER_KEY in session:
-                    response.location = f'{session[LOGIN_REFERER_KEY]}{hash}'
-                    del session[LOGIN_REFERER_KEY]
+                login_target = request.registry.queryMultiAdapter((self.context, self.request, self),
+                                                                  ILoginPageTarget)
+                if login_target is not None:
+                    response.location = login_target
                 else:
-                    response.location = f'/{hash}'
+                    if LOGIN_REFERER_KEY in session:
+                        response.location = f'{session[LOGIN_REFERER_KEY]}{hash}'
+                        del session[LOGIN_REFERER_KEY]
+                    else:
+                        response.location = f'/{hash}'
             return response
         return None
 
 
 @ajax_form_config(name='login-dialog.html',
                   layer=IPyAMSLayer)  # pylint: disable=abstract-method
 @implementer(IModalPage, ILoginView)
 class ModalLoginForm(LoginForm):
     """Modal login form"""
 
     modal_class = 'modal-lg'
-    buttons = Buttons(IModalLoginFormButtons)
+
+    @property
+    def buttons(self):
+        """Form buttons getter"""
+        return get_login_buttons(IModalLoginFormButtons, self.request)
+
+    @handler(IModalLoginFormButtons['login'])
+    def login_handler(self, action):
+        """Login button handler"""
+        return super().login_handler(self, action)
 
 
 @subscriber(IDataExtractedEvent, form_selector=ILoginView)
 def handle_login_form_data(event):
     """Check credentials after data extraction"""
     data = event.data
     if 'principal_id' in data:
@@ -175,38 +241,14 @@
             status['location'] = f"{session[LOGIN_REFERER_KEY] or '/'}{hash}"
             del session[LOGIN_REFERER_KEY]
         else:
             status['location'] = f'/{hash}'
         return status
 
 
-try:
-    from pyams_zmi.interfaces.configuration import IZMIConfiguration, MYAMS_BUNDLES
-
-    @adapter_config(required=(Interface, IPyAMSLayer, ILoginView),
-                    provides=IResources)
-    class LoginViewResourcesAdapter(ContextRequestViewAdapter):
-        """Login view resources adapter"""
-
-        weight = 10
-
-        @property
-        def resources(self):
-            """Resources getter"""
-            request = self.request
-            configuration = IZMIConfiguration(request.root, None)
-            if configuration is not None:
-                # yield MyAMS bundle
-                bundle, _label = MYAMS_BUNDLES.get(configuration.myams_bundle)
-                yield bundle
-
-except ImportError:
-    pass
-
-
 @viewlet_config(name='login.logo',
                 layer=IPyAMSLayer, view=ILoginView,
                 manager=IHeaderViewletManager, weight=1)
 @template_config(template='templates/login-logo.pt')
 class LoginLogoViewlet(Viewlet):
     """Login logo viewlet"""
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/tests/__init__.py` & `pyams_security_views-1.9.1/src/pyams_security_views/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/tests/test_utilsdocs.py` & `pyams_security_views-1.9.1/src/pyams_security_views/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/tests/test_utilsdocstrings.py` & `pyams_security_views-1.9.1/src/pyams_security_views/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/widget/__init__.py` & `pyams_security_views-1.9.1/src/pyams_security_views/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/widget/interfaces.py` & `pyams_security_views-1.9.1/src/pyams_security_views/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/widget/permission.py` & `pyams_security_views-1.9.1/src/pyams_security_views/widget/permission.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/widget/principal.py` & `pyams_security_views-1.9.1/src/pyams_security_views/widget/principal.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/__init__.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/interfaces.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/manager.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,31 +15,28 @@
 This module provides views and content providers used to manage security manager properties.
 """
 
 from zope.interface import Interface, implementer
 
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
-from pyams_form.interfaces.form import IGroup, IInnerSubForm
+from pyams_form.interfaces.form import IInnerSubForm
 from pyams_form.subform import InnerEditForm
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces import ISecurityManager
 from pyams_security.interfaces.base import MANAGE_SECURITY_PERMISSION
 from pyams_security_views.zmi import ISecurityMenu
 from pyams_security_views.zmi.interfaces import ISecurityPropertiesEditForm
 from pyams_security_views.zmi.widget import SecurityManagerPluginsFieldWidget
-from pyams_skin.interfaces.viewlet import IHeaderViewletManager
-from pyams_skin.viewlet.help import AlertMessage
 from pyams_utils.adapter import adapter_config
 from pyams_viewlet.viewlet import viewlet_config
-from pyams_zmi.form import AdminEditForm, FormGroupChecker
+from pyams_zmi.form import AdminEditForm
 from pyams_zmi.interfaces import IAdminLayer, IObjectLabel
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
-
 __docformat__ = 'restructuredtext'
 
 from pyams_security_views import _  # pylint: disable=ungrouped-imports
 
 
 @adapter_config(required=(ISecurityManager, IAdminLayer, Interface),
                 provides=IObjectLabel)
@@ -73,38 +70,14 @@
                                              'authentication_plugins_names',
                                              'directory_plugins_names')
     fields['credentials_plugins_names'].widget_factory = SecurityManagerPluginsFieldWidget
     fields['authentication_plugins_names'].widget_factory = SecurityManagerPluginsFieldWidget
     fields['directory_plugins_names'].widget_factory = SecurityManagerPluginsFieldWidget
 
 
-@adapter_config(name='security-registration',
-                required=(ISecurityManager, IAdminLayer, SecurityPropertiesEditForm),
-                provides=IGroup)
-class SecurityRegistrationGroup(FormGroupChecker):
-    """Security manager registration fields"""
-
-    fields = Fields(ISecurityManager).select('open_registration', 'users_folder')
-
-
-@viewlet_config(name='security-registration.header',
-                context=ISecurityManager, layer=IAdminLayer, view=SecurityRegistrationGroup,
-                manager=IHeaderViewletManager, weight=1)
-class SecurityRegistrationHeader(AlertMessage):
-    """Security registration header"""
-
-    status = 'info'
-
-    _message = _("Open registration can be used when you want external users to be able to "
-                 "freely register their user account.\n"
-                 "You then have to select the users folder into which their profile will be "
-                 "stored.\n"
-                 "THIS CAN BE DANGEROUS! You should enable this feature carefully...")
-
-
 @adapter_config(name='security-zmi',
                 required=(ISecurityManager, IAdminLayer, SecurityPropertiesEditForm),
                 provides=IInnerSubForm)
 class SecurityZMIEditForm(InnerEditForm):
     """Security manager administration interface edit form"""
 
     legend = _("Management interface")
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/notifications.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/notifications.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/__init__.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/admin.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/plugin/admin.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/group.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/plugin/group.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/userfolder.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/plugin/userfolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,14 +376,18 @@
             self.widgets['activation_secret'].mode = DISPLAY_MODE
         if 'activation_hash' in self.widgets:
             self.widgets['activation_hash'].mode = DISPLAY_MODE
         if 'activated' in self.widgets:
             self.widgets['activated'].mode = DISPLAY_MODE
         if 'activation_date' in self.widgets:
             self.widgets['activation_date'].mode = DISPLAY_MODE
+        if 'password_hash' in self.widgets:
+            self.widgets['password_hash'].mode = DISPLAY_MODE
+        if 'password_hash_validity' in self.widgets:
+            self.widgets['password_hash_validity'].mode = DISPLAY_MODE
 
     @handler(ILocalUserEditFormButtons['apply'])
     def handle_apply(self, action):
         super().handle_apply(self, action)  # pylint: disable=too-many-function-args
 
     @handler(ILocalUserEditFormButtons['refresh'])
     def handle_refresh(self, action):
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/policy.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/policy.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/rest.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views/zmi/widget.py` & `pyams_security_views-1.9.1/src/pyams_security_views/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views.egg-info/PKG-INFO` & `pyams_security_views-1.9.1/src/pyams_security_views.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-security-views
-Version: 1.8.5
+Version: 1.9.1
 Summary: Pyramid views for PyAMS_security package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -46,14 +46,23 @@
 interface (based on PyAMS_zmi package), custom widgets and a small Cornice REST API to look for
 principals.
 
 
 Changelog
 =========
 
+1.9.1
+-----
+ - updated doctests
+
+1.9.0
+-----
+ - added support for user registration
+ - added support for local user password change
+
 1.8.5
 -----
  - refactored Colander API schemas for better OpenAPI specifications
 
 1.8.4
 -----
  - updated login form templates
```

### Comparing `pyams_security_views-1.8.5/src/pyams_security_views.egg-info/SOURCES.txt` & `pyams_security_views-1.9.1/src/pyams_security_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

