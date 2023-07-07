# Comparing `tmp/pyams_utils-1.9.1.tar.gz` & `tmp/pyams_utils-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_utils-1.9.1.tar", last modified: Sat Jul 31 18:47:35 2021, max compression
+gzip compressed data, was "dist/pyams_utils-1.9.2.tar", last modified: Sat Sep 11 11:41:59 2021, max compression
```

## Comparing `pyams_utils-1.9.1.tar` & `pyams_utils-1.9.2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/
--rw-rw-rw-   0 root         (0) root         (0)      104 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7862 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)     4051 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/docs/HISTORY.txt
--rw-rw-rw-   0 root         (0) root         (0)     1415 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/docs/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3036 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils/
--rw-rw-rw-   0 root         (0) root         (0)     1382 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8495 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     1698 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/attr.py
--rw-rw-rw-   0 root         (0) root         (0)     4081 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/cache.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/configure.zcml
--rw-rw-rw-   0 root         (0) root         (0)     5619 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3278 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/context.py
--rw-rw-rw-   0 root         (0) root         (0)     3773 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/data.py
--rw-rw-rw-   0 root         (0) root         (0)    11196 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/date.py
--rw-rw-rw-   0 root         (0) root         (0)     2227 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     3486 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/dict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     1807 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     8037 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/adapter.rst
--rw-rw-rw-   0 root         (0) root         (0)     1133 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/attr.rst
--rw-rw-rw-   0 root         (0) root         (0)     2514 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/cache.rst
--rw-rw-rw-   0 root         (0) root         (0)     4621 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/container.rst
--rw-rw-rw-   0 root         (0) root         (0)     2484 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/context.rst
--rw-rw-rw-   0 root         (0) root         (0)     2033 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/data.rst
--rw-rw-rw-   0 root         (0) root         (0)     4540 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/dates.rst
--rw-rw-rw-   0 root         (0) root         (0)     2075 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/factory.rst
--rw-rw-rw-   0 root         (0) root         (0)     5612 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/fanstatic.rst
--rw-rw-rw-   0 root         (0) root         (0)      499 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/i18n.rst
--rw-rw-rw-   0 root         (0) root         (0)     4263 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/inherit.rst
--rw-rw-rw-   0 root         (0) root         (0)     3042 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/intids.rst
--rw-rw-rw-   0 root         (0) root         (0)     2895 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/list.rst
--rw-rw-rw-   0 root         (0) root         (0)      924 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/location.rst
--rw-rw-rw-   0 root         (0) root         (0)      966 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/lock.rst
--rw-rw-rw-   0 root         (0) root         (0)     3268 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/progress.rst
--rw-rw-rw-   0 root         (0) root         (0)     2743 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/property.rst
--rw-rw-rw-   0 root         (0) root         (0)      896 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/protocol-http.rst
--rw-rw-rw-   0 root         (0) root         (0)      222 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/protocol-socket.rst
--rw-rw-rw-   0 root         (0) root         (0)     2770 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/protocol-xmlrpc.rst
--rw-rw-rw-   0 root         (0) root         (0)     4274 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/pygments.rst
--rw-rw-rw-   0 root         (0) root         (0)     8265 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/registry.rst
--rw-rw-rw-   0 root         (0) root         (0)     7778 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/request.rst
--rw-rw-rw-   0 root         (0) root         (0)     1211 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/rest.rst
--rw-rw-rw-   0 root         (0) root         (0)     8339 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/schema.rst
--rw-rw-rw-   0 root         (0) root         (0)     1954 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/session.rst
--rw-rw-rw-   0 root         (0) root         (0)     1348 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/size.rst
--rw-rw-rw-   0 root         (0) root         (0)     3638 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/tales.rst
--rw-rw-rw-   0 root         (0) root         (0)     6141 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/text.rst
--rw-rw-rw-   0 root         (0) root         (0)     3302 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/timezone.rst
--rw-rw-rw-   0 root         (0) root         (0)    10365 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/traversing.rst
--rw-rw-rw-   0 root         (0) root         (0)     5061 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/url.rst
--rw-rw-rw-   0 root         (0) root         (0)     1227 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/wsgi.rst
--rw-rw-rw-   0 root         (0) root         (0)     4498 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/doctests/zodb.rst
--rw-rw-rw-   0 root         (0) root         (0)     5859 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/encoding.py
--rw-rw-rw-   0 root         (0) root         (0)     4890 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5640 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/fanstatic.py
--rw-rw-rw-   0 root         (0) root         (0)     5526 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/html.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     2636 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/include.py
--rw-rw-rw-   0 root         (0) root         (0)     3598 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/inherit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     3326 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/data.py
--rw-rw-rw-   0 root         (0) root         (0)     1834 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/form.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/inherit.py
--rw-rw-rw-   0 root         (0) root         (0)     1205 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/intids.py
--rw-rw-rw-   0 root         (0) root         (0)     1960 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/pygments.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/size.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/tales.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/text.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/timezone.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/traversing.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/tree.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/url.py
--rw-rw-rw-   0 root         (0) root         (0)     3159 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/interfaces/zeo.py
--rw-rw-rw-   0 root         (0) root         (0)     4226 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/intids.py
--rw-rw-rw-   0 root         (0) root         (0)     1762 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/json.py
--rw-rw-rw-   0 root         (0) root         (0)     4333 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    13824 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/locales/fr/LC_MESSAGES/pyams_utils.mo
--rw-rw-rw-   0 root         (0) root         (0)    20051 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/locales/fr/LC_MESSAGES/pyams_utils.po
--rw-rw-rw-   0 root         (0) root         (0)    15214 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/locales/pyams_utils.pot
--rw-rw-rw-   0 root         (0) root         (0)     1128 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/location.py
--rw-rw-rw-   0 root         (0) root         (0)     2912 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/lock.py
--rw-rw-rw-   0 root         (0) root         (0)     6092 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2428 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/property.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils/protocol/
--rwxrwxrwx   0 root         (0) root         (0)        2 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/protocol/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/protocol/http.py
--rw-rw-rw-   0 root         (0) root         (0)      902 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/protocol/tcp.py
--rwxrwxrwx   0 root         (0) root         (0)     7939 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/protocol/xmlrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     5456 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/pygments.py
--rw-rw-rw-   0 root         (0) root         (0)     9175 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    10498 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/request.py
--rw-rw-rw-   0 root         (0) root         (0)     3272 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     7182 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     1653 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/size.py
--rw-rw-rw-   0 root         (0) root         (0)     4438 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/tales.py
--rw-rw-rw-   0 root         (0) root         (0)     4492 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1272 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1825 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1858 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     9628 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils/timezone/
--rw-rw-rw-   0 root         (0) root         (0)     2772 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/timezone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/timezone/utility.py
--rw-rw-rw-   0 root         (0) root         (0)     1122 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/timezone/vocabulary.py
--rw-rw-rw-   0 root         (0) root         (0)    10538 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/traversing.py
--rwxrwxrwx   0 root         (0) root         (0)     9433 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/unicode.py
--rw-rw-rw-   0 root         (0) root         (0)     8105 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/url.py
--rw-rw-rw-   0 root         (0) root         (0)     3954 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/vocabulary.py
--rw-rw-rw-   0 root         (0) root         (0)     1910 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/wsgi.py
--rw-rw-rw-   0 root         (0) root         (0)    11138 2021-07-31 18:47:18.000000 pyams_utils-1.9.1/src/pyams_utils/zodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7862 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3727 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      458 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2021-07-31 18:47:35.000000 pyams_utils-1.9.1/src/pyams_utils.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7962 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/PKG-INFO
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     4119 2021-09-11 11:35:17.000000 pyams_utils-1.9.2/docs/HISTORY.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/docs/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3036 2021-09-11 11:35:17.000000 pyams_utils-1.9.2/setup.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2021-07-12 21:51:28.000000 pyams_utils-1.9.2/src/pyams_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8495 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/attr.py
+-rw-rw-rw-   0 root         (0) root         (0)     4081 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/configure.zcml
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2021-07-12 21:51:28.000000 pyams_utils-1.9.2/src/pyams_utils/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3278 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     3773 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11196 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3486 2021-07-12 21:51:28.000000 pyams_utils-1.9.2/src/pyams_utils/dict.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8037 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/adapter.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/attr.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/cache.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4621 2021-07-12 21:51:28.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/container.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2484 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/context.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/data.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4540 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/dates.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/factory.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5612 2021-06-01 13:51:57.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/fanstatic.rst
+-rw-rw-rw-   0 root         (0) root         (0)      499 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/i18n.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4263 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/inherit.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2021-07-12 21:51:28.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/intids.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2895 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/list.rst
+-rw-rw-rw-   0 root         (0) root         (0)      924 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/location.rst
+-rw-rw-rw-   0 root         (0) root         (0)      966 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/lock.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3268 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/progress.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2743 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/property.rst
+-rw-rw-rw-   0 root         (0) root         (0)      896 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/protocol-http.rst
+-rw-rw-rw-   0 root         (0) root         (0)      222 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/protocol-socket.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2770 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/protocol-xmlrpc.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4274 2021-07-12 21:51:28.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/pygments.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8265 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/registry.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7778 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/request.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/rest.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8339 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/schema.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/session.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/size.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3638 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/tales.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6141 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/text.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/timezone.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10365 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/traversing.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5061 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/url.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/wsgi.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/doctests/zodb.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5859 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4890 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5719 2021-09-11 11:35:17.000000 pyams_utils-1.9.2/src/pyams_utils/fanstatic.py
+-rw-rw-rw-   0 root         (0) root         (0)     5526 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     2636 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     3598 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/inherit.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     3326 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/inherit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/intids.py
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/pygments.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/size.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/tales.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/timezone.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/traversing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/tree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/interfaces/zeo.py
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2021-07-12 21:51:28.000000 pyams_utils-1.9.2/src/pyams_utils/intids.py
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     4333 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/list.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils/locales/
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils/locales/fr/
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    13824 2021-07-31 19:28:27.000000 pyams_utils-1.9.2/src/pyams_utils/locales/fr/LC_MESSAGES/pyams_utils.mo
+-rw-rw-rw-   0 root         (0) root         (0)    20051 2021-07-31 19:28:27.000000 pyams_utils-1.9.2/src/pyams_utils/locales/fr/LC_MESSAGES/pyams_utils.po
+-rw-rw-rw-   0 root         (0) root         (0)    15214 2021-07-31 19:28:27.000000 pyams_utils-1.9.2/src/pyams_utils/locales/pyams_utils.pot
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/location.py
+-rw-rw-rw-   0 root         (0) root         (0)     2912 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     6092 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2428 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/property.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils/protocol/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/protocol/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/protocol/http.py
+-rw-rw-rw-   0 root         (0) root         (0)      902 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/protocol/tcp.py
+-rwxrwxrwx   0 root         (0) root         (0)     7939 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/protocol/xmlrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5456 2021-07-12 21:51:28.000000 pyams_utils-1.9.2/src/pyams_utils/pygments.py
+-rw-rw-rw-   0 root         (0) root         (0)     9175 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    10498 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     3272 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     7182 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1653 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/size.py
+-rw-rw-rw-   0 root         (0) root         (0)     4438 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/tales.py
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/testing.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1825 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     9628 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/text.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils/timezone/
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/timezone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/timezone/utility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/timezone/vocabulary.py
+-rw-rw-rw-   0 root         (0) root         (0)    10538 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/traversing.py
+-rwxrwxrwx   0 root         (0) root         (0)     9433 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/unicode.py
+-rw-rw-rw-   0 root         (0) root         (0)     8105 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     3954 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/vocabulary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/wsgi.py
+-rw-rw-rw-   0 root         (0) root         (0)    11138 2021-05-31 00:46:20.000000 pyams_utils-1.9.2/src/pyams_utils/zodb.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7962 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3727 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      458 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2021-09-11 11:41:59.000000 pyams_utils-1.9.2/src/pyams_utils.egg-info/top_level.txt
```

### Comparing `pyams_utils-1.9.1/PKG-INFO` & `pyams_utils-1.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_utils
-Version: 1.9.1
+Version: 1.9.2
 Summary: PyAMS generic modules
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Description: ===================
         PyAMS_utils package
@@ -44,14 +44,18 @@
         Most PyAMS_utils modules are documented using doctests in the /doctests/ sub-directory.
         
         
         
         Changelog
         =========
         
+        1.9.2
+        -----
+         - updated path getter of external Fanstatic resources
+        
         1.9.1
         -----
          - locales and translations updates
         
         1.9.0
         -----
          - added simple container class to handle internal sequence
```

### Comparing `pyams_utils-1.9.1/docs/HISTORY.txt` & `pyams_utils-1.9.2/docs/HISTORY.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 
 Changelog
 =========
 
+1.9.2
+-----
+ - updated path getter of external Fanstatic resources
+
 1.9.1
 -----
  - locales and translations updates
 
 1.9.0
 -----
  - added simple container class to handle internal sequence
```

### Comparing `pyams_utils-1.9.1/docs/README.txt` & `pyams_utils-1.9.2/docs/README.txt`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/setup.py` & `pyams_utils-1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.txt')
 HISTORY = os.path.join(DOCS, 'HISTORY.txt')
 
-version = '1.9.1'
+version = '1.9.2'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'zope.site',
     'pyramid_chameleon',
     'pyramid_zcml'
 ]
```

### Comparing `pyams_utils-1.9.1/src/pyams_utils/__init__.py` & `pyams_utils-1.9.2/src/pyams_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/adapter.py` & `pyams_utils-1.9.2/src/pyams_utils/adapter.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/attr.py` & `pyams_utils-1.9.2/src/pyams_utils/attr.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/cache.py` & `pyams_utils-1.9.2/src/pyams_utils/cache.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/container.py` & `pyams_utils-1.9.2/src/pyams_utils/container.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/context.py` & `pyams_utils-1.9.2/src/pyams_utils/context.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/data.py` & `pyams_utils-1.9.2/src/pyams_utils/data.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/date.py` & `pyams_utils-1.9.2/src/pyams_utils/date.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/decorator.py` & `pyams_utils-1.9.2/src/pyams_utils/decorator.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/dict.py` & `pyams_utils-1.9.2/src/pyams_utils/dict.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/README.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/adapter.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/adapter.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/attr.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/attr.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/cache.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/cache.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/container.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/container.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/context.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/context.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/data.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/data.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/dates.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/dates.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/factory.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/factory.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/fanstatic.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/fanstatic.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/inherit.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/inherit.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/intids.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/intids.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/list.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/list.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/location.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/location.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/lock.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/lock.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/progress.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/progress.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/property.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/property.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/protocol-http.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/protocol-http.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/protocol-xmlrpc.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/protocol-xmlrpc.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/pygments.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/pygments.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/registry.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/registry.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/request.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/request.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/rest.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/rest.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/schema.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/schema.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/session.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/session.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/size.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/size.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/tales.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/tales.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/text.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/text.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/timezone.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/timezone.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/traversing.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/traversing.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/url.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/url.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/wsgi.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/wsgi.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/doctests/zodb.rst` & `pyams_utils-1.9.2/src/pyams_utils/doctests/zodb.rst`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/encoding.py` & `pyams_utils-1.9.2/src/pyams_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/factory.py` & `pyams_utils-1.9.2/src/pyams_utils/factory.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/fanstatic.py` & `pyams_utils-1.9.2/src/pyams_utils/fanstatic.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,16 @@
         if self.resource_type == 'js':
             return render_js(self.relpath, self.defer)
         return ''
 
 
 def get_resource_path(resource, signature='--static--', versioning=True):
     """Get path for given resource"""
+    if isinstance(resource, ExternalResource):
+        return resource.relpath
     res = NeededResources(publisher_signature=signature, versioning=versioning)
     return '{0}/{1}'.format(res.library_url(resource.library), resource.relpath)
 
 
 @adapter_config(name='resource_path',
                 required=(Interface, Interface, Interface),
                 provides=ITALESExtension)
```

### Comparing `pyams_utils-1.9.1/src/pyams_utils/html.py` & `pyams_utils-1.9.2/src/pyams_utils/html.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/i18n.py` & `pyams_utils-1.9.2/src/pyams_utils/i18n.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/include.py` & `pyams_utils-1.9.2/src/pyams_utils/include.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/inherit.py` & `pyams_utils-1.9.2/src/pyams_utils/inherit.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/__init__.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/data.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/data.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/form.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/form.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/inherit.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/inherit.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/intids.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/intids.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/pygments.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/pygments.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/size.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/size.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/tales.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/tales.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/text.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/text.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/timezone.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/timezone.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/traversing.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/traversing.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/tree.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/tree.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/url.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/url.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/interfaces/zeo.py` & `pyams_utils-1.9.2/src/pyams_utils/interfaces/zeo.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/intids.py` & `pyams_utils-1.9.2/src/pyams_utils/intids.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/json.py` & `pyams_utils-1.9.2/src/pyams_utils/json.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/list.py` & `pyams_utils-1.9.2/src/pyams_utils/list.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/locales/fr/LC_MESSAGES/pyams_utils.mo` & `pyams_utils-1.9.2/src/pyams_utils/locales/fr/LC_MESSAGES/pyams_utils.mo`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/locales/fr/LC_MESSAGES/pyams_utils.po` & `pyams_utils-1.9.2/src/pyams_utils/locales/fr/LC_MESSAGES/pyams_utils.po`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/locales/pyams_utils.pot` & `pyams_utils-1.9.2/src/pyams_utils/locales/pyams_utils.pot`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/location.py` & `pyams_utils-1.9.2/src/pyams_utils/location.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/lock.py` & `pyams_utils-1.9.2/src/pyams_utils/lock.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/progress.py` & `pyams_utils-1.9.2/src/pyams_utils/progress.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/property.py` & `pyams_utils-1.9.2/src/pyams_utils/property.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/protocol/http.py` & `pyams_utils-1.9.2/src/pyams_utils/protocol/http.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/protocol/tcp.py` & `pyams_utils-1.9.2/src/pyams_utils/protocol/tcp.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/protocol/xmlrpc.py` & `pyams_utils-1.9.2/src/pyams_utils/protocol/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/pygments.py` & `pyams_utils-1.9.2/src/pyams_utils/pygments.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/registry.py` & `pyams_utils-1.9.2/src/pyams_utils/registry.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/request.py` & `pyams_utils-1.9.2/src/pyams_utils/request.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/rest.py` & `pyams_utils-1.9.2/src/pyams_utils/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/schema.py` & `pyams_utils-1.9.2/src/pyams_utils/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/session.py` & `pyams_utils-1.9.2/src/pyams_utils/session.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/size.py` & `pyams_utils-1.9.2/src/pyams_utils/size.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/tales.py` & `pyams_utils-1.9.2/src/pyams_utils/tales.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/testing.py` & `pyams_utils-1.9.2/src/pyams_utils/testing.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/tests/__init__.py` & `pyams_utils-1.9.2/src/pyams_utils/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/tests/test_utilsdocs.py` & `pyams_utils-1.9.2/src/pyams_utils/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/tests/test_utilsdocstrings.py` & `pyams_utils-1.9.2/src/pyams_utils/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/text.py` & `pyams_utils-1.9.2/src/pyams_utils/text.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/timezone/__init__.py` & `pyams_utils-1.9.2/src/pyams_utils/timezone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/timezone/utility.py` & `pyams_utils-1.9.2/src/pyams_utils/timezone/utility.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/timezone/vocabulary.py` & `pyams_utils-1.9.2/src/pyams_utils/timezone/vocabulary.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/traversing.py` & `pyams_utils-1.9.2/src/pyams_utils/traversing.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/unicode.py` & `pyams_utils-1.9.2/src/pyams_utils/unicode.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/url.py` & `pyams_utils-1.9.2/src/pyams_utils/url.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/vocabulary.py` & `pyams_utils-1.9.2/src/pyams_utils/vocabulary.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/wsgi.py` & `pyams_utils-1.9.2/src/pyams_utils/wsgi.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils/zodb.py` & `pyams_utils-1.9.2/src/pyams_utils/zodb.py`

 * *Files identical despite different names*

### Comparing `pyams_utils-1.9.1/src/pyams_utils.egg-info/PKG-INFO` & `pyams_utils-1.9.2/src/pyams_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-utils
-Version: 1.9.1
+Version: 1.9.2
 Summary: PyAMS generic modules
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Description: ===================
         PyAMS_utils package
@@ -44,14 +44,18 @@
         Most PyAMS_utils modules are documented using doctests in the /doctests/ sub-directory.
         
         
         
         Changelog
         =========
         
+        1.9.2
+        -----
+         - updated path getter of external Fanstatic resources
+        
         1.9.1
         -----
          - locales and translations updates
         
         1.9.0
         -----
          - added simple container class to handle internal sequence
```

### Comparing `pyams_utils-1.9.1/src/pyams_utils.egg-info/SOURCES.txt` & `pyams_utils-1.9.2/src/pyams_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

