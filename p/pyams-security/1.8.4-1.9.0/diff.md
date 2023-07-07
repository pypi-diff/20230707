# Comparing `tmp/pyams_security-1.8.4.tar.gz` & `tmp/pyams_security-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_security-1.8.4.tar", last modified: Fri Feb 18 13:10:29 2022, max compression
+gzip compressed data, was "dist/pyams_security-1.9.0.tar", last modified: Sat Apr 16 15:29:08 2022, max compression
```

## Comparing `pyams_security-1.8.4.tar` & `pyams_security-1.9.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-02-18 13:10:06.000000 pyams_security-1.8.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6459 2022-02-18 13:10:29.000000 pyams_security-1.8.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/docs/
--rwxrwxrwx   0 root         (0) root         (0)     3088 2022-02-18 13:10:06.000000 pyams_security-1.8.4/docs/HISTORY.txt
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-02-18 13:10:06.000000 pyams_security-1.8.4/docs/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-02-18 13:10:29.000000 pyams_security-1.8.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3007 2022-02-18 13:10:06.000000 pyams_security-1.8.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/
--rw-rw-rw-   0 root         (0) root         (0)      867 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/api/
--rw-rw-rw-   0 root         (0) root         (0)     1292 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/credential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     1792 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1244 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/credentials.rst
--rw-rw-rw-   0 root         (0) root         (0)     6595 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/manager.rst
--rw-rw-rw-   0 root         (0) root         (0)     2176 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/notifications.rst
--rw-rw-rw-   0 root         (0) root         (0)     7314 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/passwords.rst
--rw-rw-rw-   0 root         (0) root         (0)     1876 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/plugins.rst
--rw-rw-rw-   0 root         (0) root         (0)     6264 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/policy.rst
--rw-rw-rw-   0 root         (0) root         (0)    16078 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/principals.rst
--rw-rw-rw-   0 root         (0) root         (0)     3685 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/profiles.rst
--rw-rw-rw-   0 root         (0) root         (0)     6539 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/roles.rst
--rw-rw-rw-   0 root         (0) root         (0)    18673 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/security.rst
--rw-rw-rw-   0 root         (0) root         (0)    18803 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/doctests/users.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/generations/
--rw-rw-rw-   0 root         (0) root         (0)     4447 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/generations/evolve1.py
--rw-rw-rw-   0 root         (0) root         (0)     4773 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/include.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    26194 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3392 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/interfaces/base.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/interfaces/names.py
--rw-rw-rw-   0 root         (0) root         (0)     4234 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/interfaces/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/interfaces/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1556 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/interfaces/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15810 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo
--rw-rw-rw-   0 root         (0) root         (0)    26709 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po
--rw-rw-rw-   0 root         (0) root         (0)    15089 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/locales/pyams_security.pot
--rw-rw-rw-   0 root         (0) root         (0)     2433 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/password.py
--rw-rw-rw-   0 root         (0) root         (0)     4192 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/permission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     1507 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4090 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/plugin/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     8229 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/plugin/group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/plugin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1109 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/plugin/templates/register-body.pt
--rw-rw-rw-   0 root         (0) root         (0)      544 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/plugin/templates/register-info.pt
--rw-rw-rw-   0 root         (0) root         (0)      393 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/plugin/templates/register-message.pt
--rw-rw-rw-   0 root         (0) root         (0)    14605 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/plugin/userfolder.py
--rw-rw-rw-   0 root         (0) root         (0)     5437 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     2926 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/principal.py
--rw-rw-rw-   0 root         (0) root         (0)     4550 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/property.py
--rw-rw-rw-   0 root         (0) root         (0)     5026 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/role.py
--rw-rw-rw-   0 root         (0) root         (0)     5067 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12442 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/security.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2760 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     9955 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/utility.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2022-02-18 13:10:06.000000 pyams_security-1.8.4/src/pyams_security/vocabulary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6459 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2379 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      404 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-02-18 13:10:29.000000 pyams_security-1.8.4/src/pyams_security.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2022-04-16 15:28:44.000000 pyams_security-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6602 2022-04-16 15:29:08.000000 pyams_security-1.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     3191 2022-04-16 15:28:44.000000 pyams_security-1.9.0/docs/HISTORY.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2022-04-16 15:28:44.000000 pyams_security-1.9.0/docs/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-04-16 15:29:08.000000 pyams_security-1.9.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3007 2022-04-16 15:28:44.000000 pyams_security-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/
+-rw-rw-rw-   0 root         (0) root         (0)      867 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/credential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/credentials.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6595 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/manager.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/notifications.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7314 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/passwords.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/plugins.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/policy.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16091 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/principals.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3685 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/profiles.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6539 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/roles.rst
+-rw-rw-rw-   0 root         (0) root         (0)    18673 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/security.rst
+-rw-rw-rw-   0 root         (0) root         (0)    18831 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/doctests/users.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/generations/evolve1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4810 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    11007 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3392 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/interfaces/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/interfaces/names.py
+-rw-rw-rw-   0 root         (0) root         (0)     4234 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/interfaces/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)    15657 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/interfaces/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/interfaces/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/interfaces/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15810 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo
+-rw-rw-rw-   0 root         (0) root         (0)    26709 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po
+-rw-rw-rw-   0 root         (0) root         (0)    15089 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/locales/pyams_security.pot
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2957 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/password.py
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/permission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/plugin/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8272 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/plugin/group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/plugin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/plugin/templates/register-body.pt
+-rw-rw-rw-   0 root         (0) root         (0)      544 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/plugin/templates/register-info.pt
+-rw-rw-rw-   0 root         (0) root         (0)      393 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/plugin/templates/register-message.pt
+-rw-rw-rw-   0 root         (0) root         (0)    14643 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/plugin/userfolder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5481 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/principal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4556 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/property.py
+-rw-rw-rw-   0 root         (0) root         (0)     5026 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/role.py
+-rw-rw-rw-   0 root         (0) root         (0)     5067 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12485 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/security.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     9992 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/utility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2022-04-16 15:28:44.000000 pyams_security-1.9.0/src/pyams_security/vocabulary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6602 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2419 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      404 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-04-16 15:29:08.000000 pyams_security-1.9.0/src/pyams_security.egg-info/top_level.txt
```

### Comparing `pyams_security-1.8.4/PKG-INFO` & `pyams_security-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_security
-Version: 1.8.4
+Version: 1.9.0
 Summary: PyAMS security management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Description: ======================
         PyAMS_security package
@@ -40,14 +40,19 @@
         Finally, PyAMS_security provides ACLs and roles management, as well as custom schema fields to
         store roles assigned to principals.
         
         
         Changelog
         =========
         
+        1.9.0
+        -----
+         - moved security plugins interfaces to dedicated module
+         - added support for Python 3.10
+        
         1.8.4
         -----
          - added method to security manager to get a raw principal, bypassing cache
         
         1.8.3
         -----
          - updated translations
```

### Comparing `pyams_security-1.8.4/docs/HISTORY.txt` & `pyams_security-1.9.0/docs/HISTORY.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+1.9.0
+-----
+ - moved security plugins interfaces to dedicated module
+ - added support for Python 3.10
+
 1.8.4
 -----
  - added method to security manager to get a raw principal, bypassing cache
 
 1.8.3
 -----
  - updated translations
```

### Comparing `pyams_security-1.8.4/docs/README.txt` & `pyams_security-1.9.0/docs/README.txt`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/setup.py` & `pyams_security-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.txt')
 HISTORY = os.path.join(DOCS, 'HISTORY.txt')
 
-version = '1.8.4'
+version = '1.9.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_catalog',
     'pyams_zmi'
 ]
```

### Comparing `pyams_security-1.8.4/src/pyams_security/__init__.py` & `pyams_security-1.9.0/src/pyams_security/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/api/__init__.py` & `pyams_security-1.9.0/src/pyams_security/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/credential.py` & `pyams_security-1.9.0/src/pyams_security/credential.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 This module defines credentials class.
 """
 
 from zope.interface import implementer
 from zope.schema.fieldproperty import FieldProperty
 
-from pyams_security.interfaces import ICredentials
+from pyams_security.interfaces.plugin import ICredentials
 
 
 __docformat__ = 'restructuredtext'
 
 
 @implementer(ICredentials)
 class Credentials:
```

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/README.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/credentials.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/credentials.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/manager.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/manager.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/notifications.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/notifications.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/passwords.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/passwords.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/plugins.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/plugins.rst`

 * *Files 5% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     >>> from pyams_security.plugin import PluginSelector
 
     >>> selector = PluginSelector('admin', config)
     >>> selector.text()
     'plugin_selector = admin'
 
-    >>> from pyams_security.interfaces import AuthenticatedPrincipalEvent
+    >>> from pyams_security.interfaces.plugin import AuthenticatedPrincipalEvent
     >>> event = AuthenticatedPrincipalEvent('admin', 'admin')
     >>> selector(event)
     True
 
 You can also define a subscriber predicate using a class or an interface; we just have to
 call the "factory_config" decorator for testing:
 
     >>> from pyams_utils.testing import call_decorator
     >>> from pyams_utils.factory import factory_config
-    >>> from pyams_security.interfaces import IAdminAuthenticationPlugin
+    >>> from pyams_security.interfaces.plugin import IAdminAuthenticationPlugin
     >>> from pyams_security.plugin.admin import AdminAuthenticationPlugin
 
     >>> call_decorator(config, factory_config, AdminAuthenticationPlugin,
     ...                IAdminAuthenticationPlugin)
 
     >>> plugin = AdminAuthenticationPlugin()
```

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/policy.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/policy.rst`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     >>> config.set_authentication_policy(policy)
 
 The "admin" principal is created automatically on database upgrade; this first admin user is
 required for first management tasks, his password ("admin") should be changed as soon as possble!!
 
     >>> request = new_test_request('admin', 'admin', registry=config.registry)
 
-    >>> from pyams_security.interfaces import ADMIN_USER_NAME
+    >>> from pyams_security.interfaces.names import ADMIN_USER_NAME
     >>> admin = sm.get(ADMIN_USER_NAME)
     >>> admin
     <...AdminAuthenticationPlugin object at 0x...>
     >>> admin in sm.credentials_plugins
     False
     >>> admin in sm.authentication_plugins
     True
@@ -106,15 +106,15 @@
 
 Once registered, authentication policy is used automatically by Pyramid requests to extract
 informations; to be able to extract credentials (which are actually handled by
 external plug-ins), we will create a fake plug-in which will extract credentials from request
 environment:
 
     >>> from zope.interface import implementer
-    >>> from pyams_security.interfaces import ICredentialsPlugin
+    >>> from pyams_security.interfaces.plugin import ICredentialsPlugin
     >>> from pyams_security.credential import Credentials
 
     >>> @implementer(ICredentialsPlugin)
     ... class FakeCredentialsPlugin:
     ...     title = "Fake credentials plugin"
     ...     prefix = 'fake'
     ...     enabled = True
```

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/principals.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/principals.rst`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 Beyond system principals provided by Pyramid, PyAMS allows to create so called "admin principals";
 these are administration accounts, which are created automatically on first database upgrade!
 
 Two accounts are created on upgrade: a "normal" account called "admin" (with default password
 "admin"), and a "service" account called "internal"; the later one is used to handle
 internal administration tasks.
 
-    >>> from pyams_security.interfaces import ADMIN_USER_NAME, INTERNAL_USER_NAME
+    >>> from pyams_security.interfaces.names import ADMIN_USER_NAME, INTERNAL_USER_NAME
     >>> admin = sm[ADMIN_USER_NAME]
     >>> admin.__name__
     '__system__'
     >>> admin.login
     'admin'
     >>> admin.title
     'System manager authentication'
@@ -265,15 +265,15 @@
 principals associated with a given request:
 
     >>> request = DummyRequest()
     >>> policy.effective_principals(request)
     {'system.Everyone'}
 
     >>> from zope.interface import implementer
-    >>> from pyams_security.interfaces import ICredentialsPlugin
+    >>> from pyams_security.interfaces.plugin import ICredentialsPlugin
     >>> from pyams_security.credential import Credentials
 
     >>> @implementer(ICredentialsPlugin)
     ... class FakeCredentialsPlugin:
     ...
     ...     title = "Fake credentials plugin"
     ...     prefix = 'fake'
```

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/profiles.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/profiles.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/roles.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/roles.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/security.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/security.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/doctests/users.rst` & `pyams_security-1.9.0/src/pyams_security/doctests/users.rst`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
 Let's also try to validate a few attributes:
 
     >>> user4 = LocalUser()
     >>> user4.email = 'bob'
     >>> user4.password = 'none'
 
-    >>> from pyams_security.interfaces import ILocalUser
+    >>> from pyams_security.interfaces.plugin import ILocalUser
     >>> ILocalUser.validateInvariants(user4)
     Traceback (most recent call last):
     ...
     zope.interface.exceptions.Invalid: Given email address is not valid!
 
 
 Let's now try to authenticate:
@@ -350,16 +350,16 @@
 
 Principals groups
 -----------------
 
 Groups can be used to group principals together; permissions and roles can then be assigned to
 all group members in a single operation:
 
-    >>> from pyams_security.interfaces import PrincipalsAddedToGroupEvent, \
-    ...                                       PrincipalsRemovedFromGroupEvent
+    >>> from pyams_security.interfaces.plugin import PrincipalsAddedToGroupEvent, \
+    ...                                              PrincipalsRemovedFromGroupEvent
     >>> from pyams_security.plugin.group import Group, GroupsFolder, \
     ...                                         handle_added_group, handle_added_principals, \
     ...                                         handle_removed_principals
 
 We start by creating a local groups folder:
 
     >>> groups_folder = GroupsFolder()
@@ -510,15 +510,15 @@
 implementations; PyAMS_security only provides a few interfaces, it's up to you to implement
 them.
 
 You will also have to enable this auto-registration, and to select a users folder where these
 principals will be stored:
 
     >>> from zope.interface import implementer
-    >>> from pyams_security.interfaces import IUserRegistrationInfo
+    >>> from pyams_security.interfaces.plugin import IUserRegistrationInfo
 
     >>> @implementer(IUserRegistrationInfo)
     ... class UserRegistration:
     ...     login = None
     ...     email = 'bob'
     ...     password = 'password'
     ...     confirmed_password = 'another_password'
```

### Comparing `pyams_security-1.8.4/src/pyams_security/generations/__init__.py` & `pyams_security-1.9.0/src/pyams_security/generations/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 # FOR A PARTICULAR PURPOSE.
 #
 
 """PyAMS_security.generations main module
 
 """
 
-import sys
 from importlib import import_module
 
+import sys
 from zope.lifecycleevent import ObjectCreatedEvent
 from zope.principalannotation.interfaces import IPrincipalAnnotationUtility
 from zope.principalannotation.utility import PrincipalAnnotationUtility
 
-from pyams_security.interfaces import ADMIN_USER_LOGIN, ADMIN_USER_NAME, INTERNAL_USER_LOGIN, \
-    INTERNAL_USER_NAME, ISecurityManager, SYSTEM_PREFIX
+from pyams_security.interfaces import ISecurityManager
+from pyams_security.interfaces.names import ADMIN_USER_LOGIN, INTERNAL_USER_LOGIN, \
+    INTERNAL_USER_NAME
+from pyams_security.interfaces.names import ADMIN_USER_NAME, SYSTEM_PREFIX
 from pyams_security.plugin.admin import AdminAuthenticationPlugin
 from pyams_site.generations import check_required_utilities
 from pyams_site.interfaces import ISiteGenerations
 from pyams_utils.registry import get_current_registry, utility_config
 
 
 __docformat__ = 'restructuredtext'
```

### Comparing `pyams_security-1.8.4/src/pyams_security/generations/evolve1.py` & `pyams_security-1.9.0/src/pyams_security/generations/evolve1.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/include.py` & `pyams_security-1.9.0/src/pyams_security/include.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 from pyramid.settings import asbool
 from zope.interface import classImplements
 from zope.password.interfaces import IPasswordManager
 from zope.password.password import MD5PasswordManager, PlainTextPasswordManager, \
     SHA1PasswordManager, SSHAPasswordManager
 
-from pyams_security.interfaces import ADMIN_USER_ID, IDefaultProtectionPolicy, \
-    SYSTEM_ADMIN_ROLE, SYSTEM_VIEWER_ROLE
+from pyams_security.interfaces import IDefaultProtectionPolicy
 from pyams_security.interfaces.base import MANAGE_PERMISSION, MANAGE_ROLES_PERMISSION, \
     MANAGE_SECURITY_PERMISSION, MANAGE_SYSTEM_PERMISSION, PUBLIC_PERMISSION, \
     ROLE_ID, VIEW_PERMISSION, VIEW_SYSTEM_PERMISSION
+from pyams_security.interfaces.names import ADMIN_USER_ID, SYSTEM_ADMIN_ROLE, SYSTEM_VIEWER_ROLE
 from pyams_security.permission import register_permission
 from pyams_security.plugin import PluginSelector
 from pyams_security.role import RoleSelector, register_role, upgrade_role
 from pyams_security.security import ProtectedObjectMixin
 from pyams_security.utility import get_principal
 from pyams_site.site import BaseSiteRoot
```

### Comparing `pyams_security-1.8.4/src/pyams_security/index.py` & `pyams_security-1.9.0/src/pyams_security/index.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/interfaces/base.py` & `pyams_security-1.9.0/src/pyams_security/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/interfaces/notification.py` & `pyams_security-1.9.0/src/pyams_security/interfaces/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/interfaces/profile.py` & `pyams_security-1.9.0/src/pyams_security/interfaces/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/interfaces/site.py` & `pyams_security-1.9.0/src/pyams_security/interfaces/site.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 #
 
 """PyAMS_security.interfaces.site module
 
 This module defines site root roles interface.
 """
 
-from pyams_security.interfaces import IContentRoles, SYSTEM_ADMIN_ROLE, SYSTEM_VIEWER_ROLE
+from pyams_security.interfaces import IContentRoles
+from pyams_security.interfaces.names import SYSTEM_ADMIN_ROLE, SYSTEM_VIEWER_ROLE
 from pyams_security.schema import PrincipalsSetField
 
 
 __docformat__ = 'restructuredtext'
 
 from pyams_security import _
```

### Comparing `pyams_security-1.8.4/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo` & `pyams_security-1.9.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po` & `pyams_security-1.9.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/locales/pyams_security.pot` & `pyams_security-1.9.0/src/pyams_security/locales/pyams_security.pot`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/notification.py` & `pyams_security-1.9.0/src/pyams_security/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/password.py` & `pyams_security-1.9.0/src/pyams_security/password.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from hashlib import pbkdf2_hmac, sha512
 from hmac import compare_digest
 from os import urandom
 
 from zope.password.interfaces import IPasswordManager
 from zope.password.password import _PrefixedPasswordManager, _encoder
 
-from pyams_security.interfaces import SALT_SIZE
+from pyams_security.interfaces.plugin import SALT_SIZE
 from pyams_utils.registry import utility_config
 
 
 __docformat__ = 'restructuredtext'
 
 
 @utility_config(name='SSHA512',
```

### Comparing `pyams_security-1.8.4/src/pyams_security/permission.py` & `pyams_security-1.9.0/src/pyams_security/permission.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/plugin/__init__.py` & `pyams_security-1.9.0/src/pyams_security/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/plugin/admin.py` & `pyams_security-1.9.0/src/pyams_security/plugin/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from persistent import Persistent
 from zope.container.contained import Contained
 from zope.interface import implementer
 from zope.password.interfaces import IPasswordManager
 from zope.schema.fieldproperty import FieldProperty
 
-from pyams_security.interfaces import IAdminAuthenticationPlugin, IDirectoryPlugin
+from pyams_security.interfaces.plugin import IAdminAuthenticationPlugin, IDirectoryPlugin
 from pyams_security.principal import PrincipalInfo
 from pyams_utils.factory import factory_config
 from pyams_utils.registry import get_utility
 
 
 __docformat__ = 'restructuredtext'
```

### Comparing `pyams_security-1.8.4/src/pyams_security/plugin/group.py` & `pyams_security-1.9.0/src/pyams_security/plugin/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 
 """PyAMS_security.plugin.group module
 
 This module defines local groups of principals.
 """
 
 import logging
-
 from BTrees import OOBTree  # pylint: disable=no-name-in-module
 from persistent import Persistent
 from pyramid.events import subscriber
 from zope.container.contained import Contained
 from zope.container.folder import Folder
 from zope.lifecycleevent.interfaces import IObjectAddedEvent
 from zope.schema.fieldproperty import FieldProperty
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
-from pyams_security.interfaces import GROUP_ID_FORMATTER, IGroupsFolderPlugin, ILocalGroup, \
-    IPrincipalsAddedToGroupEvent, IPrincipalsRemovedFromGroupEvent, ISecurityManager, \
+from pyams_security.interfaces import ISecurityManager
+from pyams_security.interfaces.names import GROUP_ID_FORMATTER, LOCAL_GROUPS_VOCABULARY_NAME
+from pyams_security.interfaces.plugin import IGroupsFolderPlugin, ILocalGroup, \
+    IPrincipalsAddedToGroupEvent, IPrincipalsRemovedFromGroupEvent, \
     PrincipalsAddedToGroupEvent, PrincipalsRemovedFromGroupEvent
-from pyams_security.interfaces.names import LOCAL_GROUPS_VOCABULARY_NAME
 from pyams_security.principal import PrincipalInfo
 from pyams_utils.factory import factory_config
 from pyams_utils.registry import query_utility
 from pyams_utils.request import check_request
 from pyams_utils.vocabulary import vocabulary_config
```

### Comparing `pyams_security-1.8.4/src/pyams_security/plugin/templates/register-body.pt` & `pyams_security-1.9.0/src/pyams_security/plugin/templates/register-body.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/plugin/templates/register-info.pt` & `pyams_security-1.9.0/src/pyams_security/plugin/templates/register-info.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/plugin/userfolder.py` & `pyams_security-1.9.0/src/pyams_security/plugin/userfolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 from zope.container.folder import Folder
 from zope.interface import Invalid
 from zope.password.interfaces import IPasswordManager
 from zope.schema.fieldproperty import FieldProperty
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
 from pyams_i18n.interfaces import II18n
-from pyams_security.interfaces import ILocalUser, ISecurityManager, IUsersFolderPlugin, \
-    PRINCIPAL_ID_FORMATTER, SALT_SIZE
+from pyams_security.interfaces import ISecurityManager
+from pyams_security.interfaces.plugin import ILocalUser, IUsersFolderPlugin, SALT_SIZE
 from pyams_security.interfaces.base import IPrincipalInfo
-from pyams_security.interfaces.names import USERS_FOLDERS_VOCABULARY_NAME
+from pyams_security.interfaces.names import PRINCIPAL_ID_FORMATTER, USERS_FOLDERS_VOCABULARY_NAME
 from pyams_security.interfaces.notification import INotificationSettings
 from pyams_security.principal import PrincipalInfo
 from pyams_utils.adapter import ContextAdapter, adapter_config
 from pyams_utils.factory import factory_config
 from pyams_utils.html import html_to_text
 from pyams_utils.registry import get_utility, query_utility
 from pyams_utils.request import check_request
```

### Comparing `pyams_security-1.8.4/src/pyams_security/policy.py` & `pyams_security-1.9.0/src/pyams_security/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 from ZODB.POSException import ConnectionStateError
 from pyramid.authentication import AuthTktCookieHelper
 from pyramid.interfaces import IAuthenticationPolicy
 from pyramid.security import Authenticated, Everyone
 from zope.interface import implementer
 
-from pyams_security.interfaces import ICredentialsPlugin, ISecurityManager
+from pyams_security.interfaces import ISecurityManager
+from pyams_security.interfaces.plugin import ICredentialsPlugin
 from pyams_utils.registry import get_all_utilities_registered_for, query_utility
 from pyams_utils.wsgi import wsgi_environ_cache
 
 
 LOGGER = logging.getLogger('PyAMS (security)')
```

### Comparing `pyams_security-1.8.4/src/pyams_security/principal.py` & `pyams_security-1.9.0/src/pyams_security/principal.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 """
 
 from zope.annotation.interfaces import IAnnotations
 from zope.interface import implementer
 from zope.principalannotation.interfaces import IPrincipalAnnotationUtility
 from zope.schema.fieldproperty import FieldProperty
 
-from pyams_security.interfaces import UNKNOWN_PRINCIPAL_ID
 from pyams_security.interfaces.base import IPrincipalInfo
+from pyams_security.interfaces.names import UNKNOWN_PRINCIPAL_ID
 from pyams_utils.adapter import adapter_config
 from pyams_utils.registry import query_utility
 
 
 __docformat__ = 'restructuredtext'
 
 from pyams_security import _  # pylint: disable=ungrouped-imports
```

### Comparing `pyams_security-1.8.4/src/pyams_security/profile.py` & `pyams_security-1.9.0/src/pyams_security/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from zope.container.contained import Contained
 from zope.interface import Interface
 from zope.intid.interfaces import IIntIds
 from zope.location import locate
 from zope.traversing.interfaces import ITraversable
 
 from pyams_file.property import FileProperty
-from pyams_security.interfaces import ADMIN_USER_ID
 from pyams_security.interfaces.base import IPrincipalInfo, PUBLIC_PERMISSION
+from pyams_security.interfaces.names import ADMIN_USER_ID
 from pyams_security.interfaces.profile import IPublicProfile, PUBLIC_PROFILE_KEY
 from pyams_utils.adapter import ContextRequestAdapter, adapter_config, get_annotation_adapter
 from pyams_utils.factory import factory_config
 from pyams_utils.interfaces.tales import ITALESExtension
 from pyams_utils.registry import get_utility
 from pyams_utils.request import check_request, query_request
```

### Comparing `pyams_security-1.8.4/src/pyams_security/property.py` & `pyams_security-1.9.0/src/pyams_security/property.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/role.py` & `pyams_security-1.9.0/src/pyams_security/role.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/schema.py` & `pyams_security-1.9.0/src/pyams_security/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/security.py` & `pyams_security-1.9.0/src/pyams_security/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 from pyramid.location import lineage
 from pyramid.security import ALL_PERMISSIONS, Allow, Authenticated, DENY_ALL, Deny, Everyone
 from zope.annotation import IAttributeAnnotatable
 from zope.container.contained import Contained
 from zope.interface import implementer
 from zope.schema.fieldproperty import FieldProperty
 
-from pyams_security.interfaces import ADMIN_USER_ID, GrantedRoleEvent, IContentRoles, \
+from pyams_security.interfaces import GrantedRoleEvent, IContentRoles, \
     IDefaultProtectionPolicy, IProtectedObject, IRoleProtectedObject, ISecurityContext, \
     RevokedRoleEvent
 from pyams_security.interfaces.base import IPrincipalInfo, IRole, PUBLIC_PERMISSION, ROLE_ID
+from pyams_security.interfaces.names import ADMIN_USER_ID
 from pyams_security.permission import get_edit_permission
 from pyams_utils.adapter import adapter_config, get_annotation_adapter
 from pyams_utils.factory import factory_config
 from pyams_utils.registry import get_pyramid_registry, query_utility
 from pyams_utils.request import check_request, request_property
```

### Comparing `pyams_security-1.8.4/src/pyams_security/site.py` & `pyams_security-1.9.0/src/pyams_security/site.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 This module defines standard system manager role supported by site's root.
 """
 
 __docformat__ = 'restructuredtext'
 
 from zope.interface import implementer
 
-from pyams_security.interfaces import IRolesPolicy, SYSTEM_ADMIN_ROLE
+from pyams_security.interfaces import IRolesPolicy
+from pyams_security.interfaces.names import SYSTEM_ADMIN_ROLE
 from pyams_security.interfaces.site import ISiteRootRoles
 from pyams_security.property import RolePrincipalsFieldProperty
 from pyams_security.security import ProtectedObjectRoles
 from pyams_site.interfaces import ISiteRoot
 from pyams_utils.adapter import ContextAdapter, adapter_config
```

### Comparing `pyams_security-1.8.4/src/pyams_security/tests/__init__.py` & `pyams_security-1.9.0/src/pyams_security/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/tests/test_utilsdocs.py` & `pyams_security-1.9.0/src/pyams_security/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/tests/test_utilsdocstrings.py` & `pyams_security-1.9.0/src/pyams_security/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security/utility.py` & `pyams_security-1.9.0/src/pyams_security/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,23 @@
 
 """PyAMS_security.utility module
 
 This module defines the SecurityManager utility and custom Pyramid authentication policy.
 """
 
 import logging
-
 from beaker.cache import cache_region
 from pyramid.location import lineage
 from zope.container.folder import Folder
 from zope.schema.fieldproperty import FieldProperty
 
-from pyams_security.interfaces import AuthenticatedPrincipalEvent, IAuthenticationPlugin, \
-    ICredentialsPlugin, IDirectoryPlugin, IGroupsAwareDirectoryPlugin, \
-    IProtectedObject, ISecurityManager
+from pyams_security.interfaces import IProtectedObject, ISecurityManager
 from pyams_security.interfaces.base import ROLE_ID
+from pyams_security.interfaces.plugin import AuthenticatedPrincipalEvent, IAuthenticationPlugin, \
+    ICredentialsPlugin, IDirectoryPlugin, IGroupsAwareDirectoryPlugin
 from pyams_security.principal import MissingPrincipal, UnknownPrincipal
 from pyams_utils.factory import factory_config
 from pyams_utils.registry import get_all_utilities_registered_for, get_utilities_for, \
     query_utility
 from pyams_utils.request import check_request
```

### Comparing `pyams_security-1.8.4/src/pyams_security/vocabulary.py` & `pyams_security-1.9.0/src/pyams_security/vocabulary.py`

 * *Files identical despite different names*

### Comparing `pyams_security-1.8.4/src/pyams_security.egg-info/PKG-INFO` & `pyams_security-1.9.0/src/pyams_security.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-security
-Version: 1.8.4
+Version: 1.9.0
 Summary: PyAMS security management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Description: ======================
         PyAMS_security package
@@ -40,14 +40,19 @@
         Finally, PyAMS_security provides ACLs and roles management, as well as custom schema fields to
         store roles assigned to principals.
         
         
         Changelog
         =========
         
+        1.9.0
+        -----
+         - moved security plugins interfaces to dedicated module
+         - added support for Python 3.10
+        
         1.8.4
         -----
          - added method to security manager to get a raw principal, bypassing cache
         
         1.8.3
         -----
          - updated translations
```

### Comparing `pyams_security-1.8.4/src/pyams_security.egg-info/SOURCES.txt` & `pyams_security-1.9.0/src/pyams_security.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 src/pyams_security/doctests/users.rst
 src/pyams_security/generations/__init__.py
 src/pyams_security/generations/evolve1.py
 src/pyams_security/interfaces/__init__.py
 src/pyams_security/interfaces/base.py
 src/pyams_security/interfaces/names.py
 src/pyams_security/interfaces/notification.py
+src/pyams_security/interfaces/plugin.py
 src/pyams_security/interfaces/profile.py
 src/pyams_security/interfaces/site.py
 src/pyams_security/locales/pyams_security.pot
 src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo
 src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po
 src/pyams_security/plugin/__init__.py
 src/pyams_security/plugin/admin.py
```

