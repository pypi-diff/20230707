# Comparing `tmp/pure_ocean_breeze-4.0.4.tar.gz` & `tmp/pure_ocean_breeze-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-4.0.4.tar", last modified: Tue Jul  4 07:38:53 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-4.0.5.tar", last modified: Fri Jul  7 02:35:15 2023, max compression
```

## Comparing `pure_ocean_breeze-4.0.4.tar` & `pure_ocean_breeze-4.0.5.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.640640 pure_ocean_breeze-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 07:38:53.640640 pure_ocean_breeze-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    66656 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   267121 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.640640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.640640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 07:38:53.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-04 07:38:53.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:38:53.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-04 07:38:53.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 07:38:53.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:38:53.640640 pure_ocean_breeze-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.221577 pure_ocean_breeze-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-07 02:35:15.221577 pure_ocean_breeze-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.181577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.185577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66719 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.185577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.189577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.189577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   268539 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.189577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.193577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.193577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.193577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.197577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.197577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.201577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.201577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.201577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.201577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.205577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.205577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.205577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.209577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.213577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.213577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.213577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.217577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.217577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.217577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.217577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.221577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.221577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.181577 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-07 02:35:15.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-07 02:35:15.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 02:35:15.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-07 02:35:15.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 02:35:15.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 02:35:15.221577 pure_ocean_breeze-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/setup.py
```

### Comparing `pure_ocean_breeze-4.0.4/LICENSE` & `pure_ocean_breeze-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/PKG-INFO` & `pure_ocean_breeze-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 4.0.4
+Version: 4.0.5
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.0.4/README.md` & `pure_ocean_breeze-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-07-04 09:39:33"
-__version__ = "4.0.4"
+__updated__ = "2023-07-04 16:16:50"
+__version__ = "4.0.5"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 针对一些不常见的文件格式，读取数据文件的一些工具函数，以及其他数据工具
 """
 
-__updated__ = "2023-06-28 16:09:30"
+__updated__ = "2023-07-07 10:32:50"
 
 import os
 import pandas as pd
 import tqdm.auto
 import datetime
 import scipy.io as scio
 import numpy as np
@@ -1093,39 +1093,39 @@
         return True
     else:
         print("不存在空值")
         return False
 
 
 @do_on_dfs
-def get_abs(df: pd.DataFrame, median: bool = 0, square: bool = 0) -> pd.DataFrame:
+def get_abs(df: pd.DataFrame, quantile: float=None, square: bool = 0) -> pd.DataFrame:
     """均值距离化：计算因子与截面均值的距离
 
     Parameters
     ----------
     df : pd.DataFrame
         未均值距离化的因子，index为时间，columns为股票代码
-    median : bool, optional
-        为1则计算到中位数的距离, by default 0
+    quantile : bool, optional
+        为1则计算到某个分位点的距离, by default None
     square : bool, optional
         为1则计算距离的平方, by default 0
 
     Returns
     -------
     `pd.DataFrame`
         均值距离化之后的因子值
     """
     if not square:
-        if median:
-            return np.abs((df.T - df.T.median()).T)
+        if quantile is not None:
+            return np.abs((df.T - df.T.quantile(quantile)).T)
         else:
             return np.abs((df.T - df.T.mean()).T)
     else:
-        if median:
-            return ((df.T - df.T.median()).T) ** 2
+        if quantile is not None:
+            return ((df.T - df.T.quantile(quantile)).T) ** 2
         else:
             return ((df.T - df.T.mean()).T) ** 2
 
 
 @do_on_dfs
 def get_normal(df: pd.DataFrame) -> pd.DataFrame:
     """将因子横截面正态化
@@ -1844,15 +1844,15 @@
         变化后非负的因子值
     """
     return (df.T - df.T.min()).T
 
 
 @do_on_dfs
 def clip_mad(
-    df: pd.DataFrame, n: float = 3, replace: bool = 1, keep_trend: bool = 1
+    df: pd.DataFrame, n: float = 5, replace: bool = 1, keep_trend: bool = 1
 ) -> pd.DataFrame:
     if keep_trend:
         df = df.stack().reset_index()
         df.columns = ["date", "code", "fac"]
 
         def clip_sing(x: pd.DataFrame, n: float = 3):
             median = x.fac.quantile(0.5)
```

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-07-04 15:30:48"
+__updated__ = "2023-07-07 10:21:18"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -1344,22 +1344,22 @@
                 if corrs.shape[0] <= 30:
                     ...
                 elif corrs.shape[0] <= 60:
                     corrs = corrs.reset_index()
                     corrs.columns = ["因子名称", "相关系数"]
                     corrs1 = corrs.iloc[:30, :]
                     corrs2 = corrs.iloc[30:, :].reset_index(drop=True)
-                    corrs = pd.concat([corrs1, corrs2], axis=1).fillna('')
+                    corrs = pd.concat([corrs1, corrs2], axis=1).fillna("")
                 elif corrs.shape[0] <= 90:
                     corrs = corrs.reset_index()
                     corrs.columns = ["因子名称", "相关系数"]
                     corrs1 = corrs.iloc[:30, :]
                     corrs2 = corrs.iloc[30:60, :].reset_index(drop=True)
                     corrs3 = corrs.iloc[60:90, :].reset_index(drop=True)
-                    corrs = pd.concat([corrs1, corrs2, corrs3], axis=1).fillna('')
+                    corrs = pd.concat([corrs1, corrs2, corrs3], axis=1).fillna("")
             else:
                 olds = [df] + olds
                 corrs = show_corrs(olds, old_orders, method=method)
         else:
             corrs = show_corrs(olds, old_orders, method=method)
     return corrs.sort_index()
 
@@ -3409,16 +3409,20 @@
                 to_save.columns = ["date", "code", "fac"]
                 self.factor_steps.write_via_df(
                     to_save, self.factor_file_pinyin, tuple_col="fac"
                 )
                 return df
 
             if n_jobs > 1:
-                with WorkerPool(n_jobs=n_jobs) as pool:
-                    factor_new_more = pool.map(cal_one, cuts, progress_bar=True)
+                with concurrent.futures.ThreadPoolExecutor(
+                    max_workers=n_jobs
+                ) as executor:
+                    factor_new_more = list(
+                        tqdm.auto.tqdm(executor.map(cal_one, cuts), total=len(cuts))
+                    )
                 factor_new = factor_new + factor_new_more
             else:
                 # 开始计算因子值
                 for date1, date2 in tqdm.auto.tqdm(cuts, desc="不知乘月几人归，落月摇情满江树。"):
                     df = cal_one(date1, date2)
                     factor_new.append(df)
         else:
@@ -3456,16 +3460,20 @@
                         to_save, self.factor_file_pinyin, tuple_col="fac"
                     )
                     return df
 
             pairs = self.forward_dates(dates, many_days=many_days)
             cuts2 = tuple(zip(pairs, dates))
             if n_jobs > 1:
-                with WorkerPool(n_jobs=n_jobs) as pool:
-                    factor_new_more = pool.map(cal_two, cuts2, progress_bar=True)
+                with concurrent.futures.ThreadPoolExecutor(
+                    max_workers=n_jobs
+                ) as executor:
+                    factor_new_more = list(
+                        tqdm.auto.tqdm(executor.map(cal_two, cuts2), total=len(cuts2))
+                    )
                 factor_new = factor_new + factor_new_more
             else:
                 # 开始计算因子值
                 for date1, date2 in tqdm.auto.tqdm(cuts2, desc="知不可乎骤得，托遗响于悲风。"):
                     df = cal_two(date1, date2)
                     factor_new.append(df)
 
@@ -3563,43 +3571,23 @@
                 res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
                 res = res[["fac"]].reset_index()
                 res.columns = ["code", "fac"]
                 return res
 
         return full_run
 
-    @kk.desktop_sender(title="嘿，分钟数据处理完啦～🎈")
-    def get_daily_factors(
+    def get_daily_factors_one(
         self,
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
         show_time: bool = 0,
         many_days: int = 1,
         n_jobs: int = 1,
-    ) -> None:
-        """每次抽取chunksize天的截面上全部股票的分钟数据
-        对每天的股票的数据计算因子值
-
-        Parameters
-        ----------
-        func : Callable
-            用于计算因子值的函数
-        fields : str, optional
-            股票数据涉及到哪些字段，排除不必要的字段，可以节约读取数据的时间，形如'date,code,num,close,amount,open'
-            提取出的数据，自动按照code,date,num排序，因此code,date,num是必不可少的字段, by default "*"
-        chunksize : int, optional
-            每次读取的截面上的天数, by default 10
-        show_time : bool, optional
-            展示每次读取数据所需要的时间, by default 0
-        many_days : int, optional
-            计算某天的因子值时，需要使用之前多少天的数据
-        n_jobs : int, optional
-            并行数量, by default 1
-        """
+    ):
         if len(self.dates_new) > 0:
             for interval in self.dates_new_intervals:
                 df = self.select_any_calculate(
                     dates=interval,
                     func=func,
                     fields=fields,
                     chunksize=chunksize,
@@ -3635,29 +3623,96 @@
         else:
             self.factor = drop_duplicates_index(self.factor_old)
             # 存入本地
             self.factor.to_parquet(self.factor_file)
             new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
             logger.info(f"当前截止到{new_end_date}的因子值已经是最新的了")
 
+    @kk.desktop_sender(title="嘿，分钟数据处理完啦～🎈")
+    def get_daily_factors_two(
+        self,
+        func: Callable,
+        fields: str = "*",
+        chunksize: int = 10,
+        show_time: bool = 0,
+        many_days: int = 1,
+        n_jobs: int = 1,
+    ):
+        self.get_daily_factors_one(
+            func=func,
+            fields=fields,
+            chunksize=chunksize,
+            show_time=show_time,
+            many_days=many_days,
+            n_jobs=n_jobs,
+        )
+
+    def get_daily_factors(
+        self,
+        func: Callable,
+        fields: str = "*",
+        chunksize: int = 10,
+        show_time: bool = 0,
+        many_days: int = 1,
+        n_jobs: int = 1,
+    ) -> None:
+        """每次抽取chunksize天的截面上全部股票的分钟数据
+        对每天的股票的数据计算因子值
+
+        Parameters
+        ----------
+        func : Callable
+            用于计算因子值的函数
+        fields : str, optional
+            股票数据涉及到哪些字段，排除不必要的字段，可以节约读取数据的时间，形如'date,code,num,close,amount,open'
+            提取出的数据，自动按照code,date,num排序，因此code,date,num是必不可少的字段, by default "*"
+        chunksize : int, optional
+            每次读取的截面上的天数, by default 10
+        show_time : bool, optional
+            展示每次读取数据所需要的时间, by default 0
+        many_days : int, optional
+            计算某天的因子值时，需要使用之前多少天的数据
+        n_jobs : int, optional
+            并行数量, by default 1
+        """
+        try:
+            self.get_daily_factors_two(
+                func=func,
+                fields=fields,
+                chunksize=chunksize,
+                show_time=show_time,
+                many_days=many_days,
+                n_jobs=n_jobs,
+            )
+        except Exception:
+            self.get_daily_factors_one(
+                func=func,
+                fields=fields,
+                chunksize=chunksize,
+                show_time=show_time,
+                many_days=many_days,
+                n_jobs=n_jobs,
+            )
+
     def drop_table(self):
         """直接删除存储在questdb中的暂存数据"""
         try:
             self.factor_steps.do_order(f"drop table '{self.factor_file_pinyin}'")
             logger.success(f"暂存在questdb中的数据表格'{self.factor_file_pinyin}'已经删除")
         except Exception:
             logger.warning(f"您要删除的表格'{self.factor_file_pinyin}'已经不存在了，请检查")
 
 
 class pure_coldwinter(object):
     # DONE: 可以自由添加其他要剔除的因子，或者替换某些要剔除的因子
 
+    @classmethod
+    @lru_cache(maxsize=None)
     def __init__(
-        self,
-        facs_dict: Dict = None,
+        cls,
         momentum: bool = 1,
         earningsyield: bool = 1,
         growth: bool = 1,
         liquidity: bool = 1,
         size: bool = 1,
         leverage: bool = 1,
         beta: bool = 1,
@@ -3688,25 +3743,24 @@
         nonlinearsize : bool, optional
             是否删去非线性市值因子, by default 1
         residualvolatility : bool, optional
             是否删去残差波动率因子, by default 1
         booktoprice : bool, optional
             是否删去账面市值比因子, by default 1
         """
-        self.homeplace = HomePlace()
+        cls.homeplace = HomePlace()
         # barra因子数据
-        styles = os.listdir(self.homeplace.barra_data_file)
-        styles = [i for i in styles if i.endswith(".parquet")]
+        styles = os.listdir(cls.homeplace.barra_data_file)
+        styles = [i for i in styles if (i.endswith(".parquet")) and (i[0] != ".")]
         barras = {}
         for s in styles:
             k = s.split(".")[0]
-            v = pd.read_parquet(self.homeplace.barra_data_file + s)
+            v = pd.read_parquet(cls.homeplace.barra_data_file + s).resample("M").last()
             barras[k] = v
         rename_dict = {
-            "fac": "因子自身",
             "size": "市值",
             "nonlinearsize": "非线性市值",
             "booktoprice": "估值",
             "earningsyield": "盈利",
             "growth": "成长",
             "leverage": "杠杆",
             "liquidity": "流动性",
@@ -3742,79 +3796,60 @@
             barras = {k: v for k, v in barras.items() if k != "residualvolatility"}
             rename_dict = {
                 k: v for k, v in rename_dict.items() if k != "residualvolatility"
             }
         if booktoprice == 0:
             barras = {k: v for k, v in barras.items() if k != "booktoprice"}
             rename_dict = {k: v for k, v in rename_dict.items() if k != "booktoprice"}
-        if facs_dict is not None:
-            barras.update(facs_dict)
-        self.barras = barras
-        self.rename_dict = rename_dict
+        facs_dict = {
+            "反转_20天收益率均值": boom_one(read_daily(ret=1)),
+            "波动_20天收益率标准差": read_daily(ret=1)
+            .rolling(20, min_periods=10)
+            .std()
+            .resample("M")
+            .last(),
+            "换手_20天换手率均值": boom_one(read_daily(tr=1)),
+        }
+        barras.update(facs_dict)
+        rename_dict.update({k: k for k in facs_dict.keys()})
+        cls.barras = barras
+        cls.rename_dict = rename_dict
         sort_names = list(rename_dict.values())
-        if facs_dict is not None:
-            sort_names = sort_names + list(facs_dict.keys())
-        sort_names = [i for i in sort_names if i != "因子自身"]
-        self.sort_names = sort_names
+        cls.sort_names = sort_names
+        cls.barras_together = merge_many(
+            list(barras.values()), list(barras.keys()), how="inner"
+        )
 
     def __call__(self):
         """返回纯净因子值"""
         return self.snow_fac
 
-    def set_factors_df_wide(self, df):
+    def set_factors_df_wide(self, df: pd.DataFrame, other_factors: dict = None):
         """传入因子数据，时间为索引，代码为列名"""
-        df1 = df.copy()
-        # df1.index=df1.index-pd.DateOffset(months=1)
-        df1 = df1.resample("M").last()
-        df1 = df1.stack().reset_index()
-        df1.columns = ["date", "code", "fac"]
-        self.factors = df1.copy()
-
-    def daily_to_monthly(self, df):
-        """将日度的barra因子月度化"""
         df = df.resample("M").last()
-        return df
-
-    def get_monthly_barras_industrys(self):
-        """将barra因子和行业哑变量变成月度数据"""
-        for key, value in self.barras.items():
-            self.barras[key] = self.daily_to_monthly(value)
-
-    def wide_to_long(self, df, name):
-        """将宽数据变成长数据，便于后续拼接"""
-        df = df.stack().reset_index()
-        df.columns = ["date", "code", name]
-        df = df.set_index(["date", "code"])
-        return df
-
-    def get_wide_barras_industrys(self):
-        """将barra因子和行业哑变量都变成长数据"""
-        for key, value in self.barras.items():
-            self.barras[key] = self.wide_to_long(value, key)
-
-    def get_corr_pri_ols_pri(self):
-        """拼接barra因子和行业哑变量，生成用于求相关系数和纯净因子的数据表"""
-        if self.factors.shape[0] > 1:
-            self.factors = self.factors.set_index(["date", "code"])
-        self.corr_pri = pd.concat(
-            [self.factors] + list(self.barras.values()), axis=1
-        ).dropna()
-
-    # DONE: 修改风格因子展示顺序至报告的顺序
-    def get_corr(self):
-        """计算每一期的相关系数，再求平均值"""
-        self.corr_by_step = self.corr_pri.groupby(["date"]).apply(
-            lambda x: x.rank().corr().head(1)
-        )
-        self.__corr = self.corr_by_step.mean()
-        self.__corr = self.__corr.rename(index=self.rename_dict)
-        self.__corr = self.__corr.to_frame("相关系数").T
-
+        self.__corr = [
+            df.corrwith(i, axis=1).mean() for i in list(self.barras.values())
+        ]
+        self.__corr = (
+            pd.Series(
+                self.__corr, index=[self.rename_dict[i] for i in self.barras.keys()]
+            )
+            .to_frame("相关系数")
+            .T
+        )
         self.__corr = self.__corr[self.sort_names]
-        self.__corr = self.__corr.T
+        df = df.stack().reset_index()
+        df.columns = ["date", "code", "fac"]
+        self.factors = df
+        self.corr_pri = pd.merge(df, self.barras_together, on=["date", "code"]).dropna()
+        if other_factors is not None:
+            other_factors = merge_many(
+                list(other_factors.values()), list(other_factors.keys()), how="inner"
+            )
+            self.corr_pri = pd.merge(self.corr_pri, other_factors, on=["date", "code"])
 
     @property
     def corr(self) -> pd.DataFrame:
         """因子和10个常用风格因子的相关系数
 
         Returns
         -------
@@ -3837,26 +3872,22 @@
         df = df.assign(snow_fac=df.fac - to_minus - ols_b)
         df = df[["snow_fac"]]
         df = df.rename(columns={"snow_fac": "fac"})
         return df
 
     def get_snow_fac(self):
         """获得纯净因子"""
-        self.snow_fac = self.corr_pri.groupby(["date"]).apply(self.ols_in_group)
+        self.snow_fac = (
+            self.corr_pri.set_index(["date", "code"])
+            .groupby(["date"])
+            .apply(self.ols_in_group)
+        )
         self.snow_fac = self.snow_fac.unstack()
         self.snow_fac.columns = list(map(lambda x: x[1], list(self.snow_fac.columns)))
 
-    def run(self):
-        """运行一些必要的函数"""
-        self.get_monthly_barras_industrys()
-        self.get_wide_barras_industrys()
-        self.get_corr_pri_ols_pri()
-        self.get_corr()
-        self.get_snow_fac()
-
 
 @do_on_dfs
 class pure_snowtrain(object):
     """直接返回纯净因子"""
 
     def __init__(
         self,
@@ -3899,28 +3930,27 @@
             是否删去非线性市值因子, by default 1
         residualvolatility : bool, optional
             是否删去残差波动率因子, by default 1
         booktoprice : bool, optional
             是否删去账面市值比因子, by default 1
         """
         self.winter = pure_coldwinter(
-            facs_dict=facs_dict,
             momentum=momentum,
             earningsyield=earningsyield,
             growth=growth,
             liquidity=liquidity,
             size=size,
             leverage=leverage,
             beta=beta,
             nonlinearsize=nonlinearsize,
             residualvolatility=residualvolatility,
             booktoprice=booktoprice,
         )
-        self.winter.set_factors_df_wide(factors.copy())
-        self.winter.run()
+        self.winter.set_factors_df_wide(factors, facs_dict)
+        self.winter.get_snow_fac()
         self.corr = self.winter.corr
 
     def __call__(self) -> pd.DataFrame:
         """获得纯净化之后的因子值
 
         Returns
         -------
@@ -3933,15 +3963,15 @@
         """展示因子与barra风格因子的相关系数
 
         Returns
         -------
         pd.DataFrame
             相关系数表格
         """
-        return self.corr.T.applymap(lambda x: to_percent(x))
+        return self.corr.applymap(lambda x: to_percent(x))
 
 
 class pure_newyear(object):
     """转为生成25分组和百分组的收益矩阵而封装"""
 
     def __init__(
         self,
@@ -6198,16 +6228,20 @@
                 to_save.columns = ["date", "code", "fac"]
                 self.factor_steps.write_via_df(
                     to_save, self.factor_file_pinyin, tuple_col="fac"
                 )
                 return df
 
             if n_jobs > 1:
-                with WorkerPool(n_jobs=n_jobs) as pool:
-                    factor_new_more = pool.map(cal_one, cuts, progress_bar=True)
+                with concurrent.futures.ThreadPoolExecutor(
+                    max_workers=n_jobs
+                ) as executor:
+                    factor_new_more = list(
+                        tqdm.auto.tqdm(executor.map(cal_one, cuts), total=len(cuts))
+                    )
                 factor_new = factor_new + factor_new_more
             else:
                 # 开始计算因子值
                 for date1, date2 in tqdm.auto.tqdm(cuts, desc="不知乘月几人归，落月摇情满江树。"):
                     df = cal_one(date1, date2)
                     factor_new.append(df)
         else:
@@ -6243,16 +6277,20 @@
                         to_save, self.factor_file_pinyin, tuple_col="fac"
                     )
                     return df
 
             pairs = self.forward_dates(dates, many_days=many_days)
             cuts2 = tuple(zip(pairs, dates))
             if n_jobs > 1:
-                with WorkerPool(n_jobs=n_jobs) as pool:
-                    factor_new_more = pool.map(cal_two, cuts2, progress_bar=True)
+                with concurrent.futures.ThreadPoolExecutor(
+                    max_workers=n_jobs
+                ) as executor:
+                    factor_new_more = list(
+                        tqdm.auto.tqdm(executor.map(cal_two, cuts2), total=len(cuts2))
+                    )
                 factor_new = factor_new + factor_new_more
             else:
                 # 开始计算因子值
                 for date1, date2 in tqdm.auto.tqdm(cuts2, desc="知不可乎骤得，托遗响于悲风。"):
                     df = cal_two(date1, date2)
                     factor_new.append(df)
 
@@ -6568,31 +6606,43 @@
         """
         return self.factor.copy()
 
     def select_one_calculate(
         self,
         date: pd.Timestamp,
         func: Callable,
-        fields: str='*',
+        fields: str = "*",
         resample_frequency: str = None,
         opens_in: bool = 0,
         highs_in: bool = 0,
         lows_in: bool = 0,
         amounts_in: bool = 0,
         merge_them: bool = 0,
     ) -> None:
         the_func = partial(func)
         if not isinstance(date, int):
             date = int(datetime.datetime.strftime(date, "%Y%m%d"))
-        parquet_name=homeplace.tick_by_tick_data+ str(date)[:4]+ "-"+ str(date)[4:6]+ "-"+ str(date)[6:]+ ".parquet"
+        parquet_name = (
+            homeplace.tick_by_tick_data
+            + str(date)[:4]
+            + "-"
+            + str(date)[4:6]
+            + "-"
+            + str(date)[6:]
+            + ".parquet"
+        )
         if resample_frequency is not None:
-            fields='date,code,price,amount'
+            fields = "date,code,price,amount"
         # 开始计算因子值
-        cursor=duckdb.connect()
-        df=cursor.execute(f"select {fields} from '{parquet_name}';").arrow().to_pandas()
+        cursor = duckdb.connect()
+        df = (
+            cursor.execute(f"select {fields} from '{parquet_name}';")
+            .arrow()
+            .to_pandas()
+        )
         date = df.date.iloc[0]
         date0 = pd.Timestamp(year=date.year, month=date.month, day=date.day)
         age_here = self.age.loc[pd.Timestamp(pd.Timestamp(df.date.iloc[0]).date())]
         age_here = age_here.where(age_here > 180, np.nan).dropna()
         state_here = self.state.loc[pd.Timestamp(pd.Timestamp(df.date.iloc[0]).date())]
         state_here = state_here.where(state_here > 0, np.nan).dropna()
         df = df[df.code.isin(age_here.index)]
@@ -6701,19 +6751,19 @@
             0, "date", pd.Timestamp(year=date.year, month=date.month, day=date.day)
         )
         if (df is not None) and (df.shape[0] > 0):
             self.factor_steps.write_via_df(df, self.factor_file_pinyin, tuple_col="fac")
             df = df.pivot(columns="code", index="date", values="fac")
             return df
 
-    @kk.desktop_sender(title="铛铛，逐笔数据处理完啦～🎈")
     def get_daily_factors(
         self,
         func: Callable,
         n_jobs: int = 1,
+        fields: str = "*",
         resample_frequency: str = None,
         opens_in: bool = 0,
         highs_in: bool = 0,
         lows_in: bool = 0,
         amounts_in: bool = 0,
         merge_them: bool = 0,
     ) -> None:
@@ -6743,26 +6793,36 @@
             在resample_frequency不为None的情况下，可以使用此参数，提前计算好成交额矩阵(index为时间,columns为股票代码,values为成交量)，
             可在循环计算的函数中使用`self.amounts`来调用计算好的值，by default 0
         merge_them : bool, optional
             在resample_frequency不为None的情况下，可以使用此参数，将计算好的因子值合并到一起，生成类似于分钟数据的sql形式，by default 0
         """
         if len(self.dates_new) > 0:
             if n_jobs > 1:
-                with concurrent.futures.ThreadPoolExecutor(max_workers=n_jobs) as executor:
-                    self.factor_new=list(tqdm.auto.tqdm(executor.map(
-                        lambda x: self.select_one_calculate(
-                            date=x,
-                            func=func,
-                            resample_frequency=resample_frequency,
-                            opens_in=opens_in,
-                            highs_in=highs_in,
-                            lows_in=lows_in,
-                            moneys_in=amounts_in,
-                            merge_them=merge_them,
-                        ),self.dates_new),total=len(self.dates_new)))
+                with concurrent.futures.ThreadPoolExecutor(
+                    max_workers=n_jobs
+                ) as executor:
+                    self.factor_new = list(
+                        tqdm.auto.tqdm(
+                            executor.map(
+                                lambda x: self.select_one_calculate(
+                                    date=x,
+                                    func=func,
+                                    fields=fields,
+                                    resample_frequency=resample_frequency,
+                                    opens_in=opens_in,
+                                    highs_in=highs_in,
+                                    lows_in=lows_in,
+                                    amounts_in=amounts_in,
+                                    merge_them=merge_them,
+                                ),
+                                self.dates_new,
+                            ),
+                            total=len(self.dates_new),
+                        )
+                    )
             else:
                 for date in tqdm.auto.tqdm(self.dates_new, "您现在处于单核运算状态，建议仅在调试时使用单核"):
                     df = self.select_one_calculate(
                         date=date,
                         func=func,
                         resample_frequency=resample_frequency,
                         opens_in=opens_in,
@@ -6770,15 +6830,17 @@
                         lows_in=lows_in,
                         amounts_in=amounts_in,
                         merge_them=merge_them,
                     )
                     self.factor_new.append(df)
             # 拼接新的和旧的
             if self.factor_old is not None:
-                self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
+                self.factor = pd.concat(
+                    [self.factor_old] + self.factor_new
+                ).sort_index()
             else:
                 self.factor = self.factor_new.sort_index()
             self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
             new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
             # 存入本地
             self.factor.to_parquet(self.factor_file)
             logger.info(f"截止到{new_end_date}的因子值计算完了")
```

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 4.0.4
+Version: 4.0.5
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.4/setup.py` & `pure_ocean_breeze-4.0.5/setup.py`

 * *Files identical despite different names*

