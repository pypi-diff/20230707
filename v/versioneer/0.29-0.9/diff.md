# Comparing `tmp/versioneer-0.29.tar.gz` & `tmp/versioneer-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versioneer-0.29.tar", last modified: Fri Jul  7 14:54:42 2023, max compression
+gzip compressed data, was "dist/versioneer-0.9.tar", last modified: Thu Mar 13 00:45:59 2014, max compression
```

## Comparing `versioneer-0.29.tar` & `versioneer-0.9.tar`

### file list

```diff
@@ -1,113 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.201598 versioneer-0.29/
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-07 14:54:25.000000 versioneer-0.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-07 14:54:25.000000 versioneer-0.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-07 14:54:25.000000 versioneer-0.29/NOTES
--rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-07-07 14:54:42.201598 versioneer-0.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-07-07 14:54:25.000000 versioneer-0.29/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-07 14:54:42.201598 versioneer-0.29/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12130 2023-07-07 14:54:25.000000 versioneer-0.29/details.md
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-07 14:54:25.000000 versioneer-0.29/developers.md
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 14:54:25.000000 versioneer-0.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:54:42.201598 versioneer-0.29/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5557 2023-07-07 14:54:25.000000 versioneer-0.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.193598 versioneer-0.29/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:25.000000 versioneer-0.29/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-07-07 14:54:25.000000 versioneer-0.29/src/cmdclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-07 14:54:25.000000 versioneer-0.29/src/from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-07 14:54:25.000000 versioneer-0.29/src/from_parentdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-07-07 14:54:25.000000 versioneer-0.29/src/get_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.193598 versioneer-0.29/src/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:25.000000 versioneer-0.29/src/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-07-07 14:54:25.000000 versioneer-0.29/src/git/from_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-07 14:54:25.000000 versioneer-0.29/src/git/from_vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-07 14:54:25.000000 versioneer-0.29/src/git/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-07 14:54:25.000000 versioneer-0.29/src/git/long_get_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-07 14:54:25.000000 versioneer-0.29/src/git/long_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-07-07 14:54:25.000000 versioneer-0.29/src/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-07 14:54:25.000000 versioneer-0.29/src/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-07-07 14:54:25.000000 versioneer-0.29/src/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-07-07 14:54:25.000000 versioneer-0.29/src/setupfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-07 14:54:25.000000 versioneer-0.29/src/subprocess_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp/bin/rundemo
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.189598 versioneer-0.29/test/demoapp/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp/src/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp/src/demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp-pyproject/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-pyproject/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp-pyproject/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-pyproject/bin/rundemo
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-pyproject/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-pyproject/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.189598 versioneer-0.29/test/demoapp-pyproject/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp-pyproject/src/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-pyproject/src/demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp-script-only/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-script-only/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-script-only/README
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-script-only/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-script-only/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-script-only/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp-script-only/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp-script-only/src/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-script-only/src/demo/placeholder
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp-script-only/src/rundemo-template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp2-setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools/README
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.189598 versioneer-0.29/test/demoapp2-setuptools/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp2-setuptools/src/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools/src/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools/src/demo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.189598 versioneer-0.29/test/demoapp2-setuptools-subproject/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp2-setuptools-subproject/subproject/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools-subproject/subproject/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools-subproject/subproject/README
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools-subproject/subproject/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools-subproject/subproject/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.189598 versioneer-0.29/test/demoapp2-setuptools-subproject/subproject/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.197598 versioneer-0.29/test/demoapp2-setuptools-subproject/subproject/src/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools-subproject/subproject/src/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoapp2-setuptools-subproject/subproject/src/demo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.201598 versioneer-0.29/test/demoappext-setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoappext-setuptools/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoappext-setuptools/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.201598 versioneer-0.29/test/demoappext-setuptools/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoappext-setuptools/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   111960 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoappext-setuptools/demo/ext.c
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoappext-setuptools/demo/ext.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoappext-setuptools/demo/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoappext-setuptools/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-07 14:54:25.000000 versioneer-0.29/test/demoappext-setuptools/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.201598 versioneer-0.29/test/demolib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:25.000000 versioneer-0.29/test/demolib/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 14:54:25.000000 versioneer-0.29/test/demolib/README
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 14:54:25.000000 versioneer-0.29/test/demolib/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 14:54:25.000000 versioneer-0.29/test/demolib/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.189598 versioneer-0.29/test/demolib/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.201598 versioneer-0.29/test/demolib/src/demolib/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:54:25.000000 versioneer-0.29/test/demolib/src/demolib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.201598 versioneer-0.29/test/git/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-07 14:54:25.000000 versioneer-0.29/test/git/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    32272 2023-07-07 14:54:25.000000 versioneer-0.29/test/git/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)    26429 2023-07-07 14:54:25.000000 versioneer-0.29/test/git/test_invocations.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-07 14:54:25.000000 versioneer-0.29/test/run_pyflakes_src.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-07 14:54:25.000000 versioneer-0.29/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-07 14:54:25.000000 versioneer-0.29/test/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-07-07 14:54:25.000000 versioneer-0.29/test/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-07 14:54:25.000000 versioneer-0.29/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:42.201598 versioneer-0.29/versioneer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-07-07 14:54:42.000000 versioneer-0.29/versioneer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-07 14:54:42.000000 versioneer-0.29/versioneer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:54:42.000000 versioneer-0.29/versioneer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 14:54:42.000000 versioneer-0.29/versioneer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 14:54:42.000000 versioneer-0.29/versioneer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 14:54:42.000000 versioneer-0.29/versioneer.egg-info/top_level.txt
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2014-03-13 00:45:59.000000 versioneer-0.9/
+-rw-r--r--   0 warner     (502) staff       (20)      303 2014-03-11 19:46:41.000000 versioneer-0.9/.travis.yml
+-rw-r--r--   0 warner     (502) staff       (20)      354 2014-03-13 00:31:11.000000 versioneer-0.9/MANIFEST.in
+-rw-r--r--   0 warner     (502) staff       (20)     3752 2011-11-16 01:04:22.000000 versioneer-0.9/NOTES
+-rw-r--r--   0 warner     (502) staff       (20)      857 2014-03-13 00:45:59.000000 versioneer-0.9/PKG-INFO
+-rw-r--r--   0 warner     (502) staff       (20)     9982 2014-03-11 20:36:38.000000 versioneer-0.9/README.md
+-rwxr-xr-x   0 warner     (502) staff       (20)     3908 2014-03-13 00:43:18.000000 versioneer-0.9/setup.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2014-03-13 00:45:59.000000 versioneer-0.9/src/
+-rw-r--r--   0 warner     (502) staff       (20)        0 2013-08-20 23:11:01.000000 versioneer-0.9/src/__init__.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2014-03-13 00:45:59.000000 versioneer-0.9/src/git/
+-rw-r--r--   0 warner     (502) staff       (20)        0 2013-08-20 23:11:01.000000 versioneer-0.9/src/git/__init__.py
+-rw-r--r--   0 warner     (502) staff       (20)     1696 2014-02-17 20:47:45.000000 versioneer-0.9/src/git/install.py
+-rw-r--r--   0 warner     (502) staff       (20)     1900 2014-03-13 00:39:13.000000 versioneer-0.9/src/git/long-version.py
+-rw-r--r--   0 warner     (502) staff       (20)     3920 2014-02-17 20:47:45.000000 versioneer-0.9/src/git/middle.py
+-rw-r--r--   0 warner     (502) staff       (20)      305 2014-03-13 00:39:20.000000 versioneer-0.9/src/header.py
+-rw-r--r--   0 warner     (502) staff       (20)      392 2014-03-13 00:40:54.000000 versioneer-0.9/src/installer.py
+-rw-r--r--   0 warner     (502) staff       (20)      529 2013-11-28 08:21:08.000000 versioneer-0.9/src/parentdir.py
+-rw-r--r--   0 warner     (502) staff       (20)     1122 2014-02-17 20:47:45.000000 versioneer-0.9/src/subprocess_helper.py
+-rw-r--r--   0 warner     (502) staff       (20)     6388 2014-03-13 00:40:13.000000 versioneer-0.9/src/trailer.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2014-03-13 00:45:59.000000 versioneer-0.9/test/
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2014-03-13 00:45:59.000000 versioneer-0.9/test/demoapp/
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2014-03-13 00:45:59.000000 versioneer-0.9/test/demoapp/bin/
+-rw-r--r--   0 warner     (502) staff       (20)      257 2013-08-28 23:43:26.000000 versioneer-0.9/test/demoapp/bin/rundemo
+-rw-r--r--   0 warner     (502) staff       (20)       22 2013-08-20 23:11:01.000000 versioneer-0.9/test/demoapp/MANIFEST.in
+-rw-r--r--   0 warner     (502) staff       (20)        8 2013-08-20 23:11:01.000000 versioneer-0.9/test/demoapp/README
+-rw-r--r--   0 warner     (502) staff       (20)      554 2013-08-20 23:11:01.000000 versioneer-0.9/test/demoapp/setup.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2014-03-13 00:45:59.000000 versioneer-0.9/test/demoapp/src/
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2014-03-13 00:45:59.000000 versioneer-0.9/test/demoapp/src/demo/
+-rw-r--r--   0 warner     (502) staff       (20)        1 2013-08-20 23:11:01.000000 versioneer-0.9/test/demoapp/src/demo/__init__.py
+-rw-r--r--   0 warner     (502) staff       (20)    10811 2014-02-17 20:47:45.000000 versioneer-0.9/test/test_git.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `versioneer-0.29/NOTES` & `versioneer-0.9/NOTES`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         invoked after self.filelist is created (but not populated), could be
         used to invoke extra commands
       - self.make_release_tree() is what creates the tree that will be
         archived.. could override that, modify _version.py on the way out
         - good to know: make_release_tree() creates hardlinks if possible. If
           'setup.py build' does this too, that would explain why it's not
           always necessary to rebuild when source files are changed.
-        - need to ensure _version.py is not a link before changing it
+        - need to delink _version.py before changing it
         - make_release_tree(base_dir, files) creates os.path.join(base_dir,f)
           for f in files
 **** let's investigate this:
      - 'setup.py build' runs superclass, looks for .git, if present:
        - use git-describe
        - locate build/STUFF/../_version.py
        - replace it with one-line string variable set
```

### Comparing `versioneer-0.29/src/git/install.py` & `versioneer-0.9/src/git/install.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,50 @@
-import os # --STRIP DURING BUILD
-import sys # --STRIP DURING BUILD
-from typing import Optional # --STRIP DURING BUILD
-from subprocess_helper import run_command # --STRIP DURING BUILD
-
-def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
-    """Git-specific installation logic for Versioneer.
-
-    For Git, this means creating/changing .gitattributes to mark _version.py
-    for export-subst keyword substitution.
-    """
+import os.path
+import sys
+
+# os.path.relpath only appeared in Python-2.6 . Define it here for 2.5.
+def os_path_relpath(path, start=os.path.curdir):
+    """Return a relative version of a path"""
+
+    if not path:
+        raise ValueError("no path specified")
+
+    start_list = [x for x in os.path.abspath(start).split(os.path.sep) if x]
+    path_list = [x for x in os.path.abspath(path).split(os.path.sep) if x]
+
+    # Work out how much of the filepath is shared by start and path.
+    i = len(os.path.commonprefix([start_list, path_list]))
+
+    rel_list = [os.path.pardir] * (len(start_list)-i) + path_list[i:]
+    if not rel_list:
+        return os.path.curdir
+    return os.path.join(*rel_list)
+
+def do_vcs_install(versionfile_source, ipy):
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [versionfile_source]
-    if ipy:
-        files.append(ipy)
-    if "VERSIONEER_PEP518" not in globals():
-        try:
-            my_path = __file__
-            if my_path.endswith((".pyc", ".pyo")):
-                my_path = os.path.splitext(my_path)[0] + ".py"
-            versioneer_file = os.path.relpath(my_path)
-        except NameError:
-            versioneer_file = "versioneer.py"
-        files.append(versioneer_file)
+    files = [versionfile_source, ipy]
+    try:
+        me = __file__
+        if me.endswith(".pyc") or me.endswith(".pyo"):
+            me = os.path.splitext(me)[0] + ".py"
+        versioneer_file = os_path_relpath(me)
+    except NameError:
+        versioneer_file = "versioneer.py"
+    files.append(versioneer_file)
     present = False
     try:
-        with open(".gitattributes", "r") as fobj:
-            for line in fobj:
-                if line.strip().startswith(versionfile_source):
-                    if "export-subst" in line.strip().split()[1:]:
-                        present = True
-                        break
-    except OSError:
-        pass
+        f = open(".gitattributes", "r")
+        for line in f.readlines():
+            if line.strip().startswith(versionfile_source):
+                if "export-subst" in line.strip().split()[1:]:
+                    present = True
+        f.close()
+    except EnvironmentError:
+        pass    
     if not present:
-        with open(".gitattributes", "a+") as fobj:
-            fobj.write(f"{versionfile_source} export-subst\n")
+        f = open(".gitattributes", "a+")
+        f.write("%s export-subst\n" % versionfile_source)
+        f.close()
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
-
-
```

