# Comparing `tmp/seamm-installer-2023.4.2.tar.gz` & `tmp/seamm-installer-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm-installer-2023.4.2.tar", last modified: Sun Apr  2 16:10:10 2023, max compression
+gzip compressed data, was "seamm-installer-2023.6.7.tar", last modified: Fri Jul  7 13:35:45 2023, max compression
```

## Comparing `seamm-installer-2023.4.2.tar` & `seamm-installer-2023.6.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:10:10.288222 seamm-installer-2023.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-02 16:10:10.288222 seamm-installer-2023.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:10:10.276222 seamm-installer-2023.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8568 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:10:10.288222 seamm-installer-2023.4.2/seamm_installer/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-02 16:10:10.288222 seamm-installer-2023.4.2/seamm_installer/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:10:10.284222 seamm-installer-2023.4.2/seamm_installer/data/
--rw-r--r--   0 runner    (1001) docker     (123)   250762 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/SEAMM.icns
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/development.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:10:10.284222 seamm-installer-2023.4.2/seamm_installer/data/linux_icons/
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/linux_icons/128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/linux_icons/16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/linux_icons/24x24.png
--rw-r--r--   0 runner    (1001) docker     (123)    20257 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/linux_icons/256x256.png
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/linux_icons/32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/linux_icons/48x48.png
--rw-r--r--   0 runner    (1001) docker     (123)    48610 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/linux_icons/512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/linux_icons/64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/seamm.ini
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/data/seamm.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    50770 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/install.py
--rw-r--r--   0 runner    (1001) docker     (123)    27101 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/installer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15092 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/mac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/my.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/seamm_installer/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:10:10.284222 seamm-installer-2023.4.2/seamm_installer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-02 16:10:10.000000 seamm-installer-2023.4.2/seamm_installer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-02 16:10:10.000000 seamm-installer-2023.4.2/seamm_installer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 16:10:10.000000 seamm-installer-2023.4.2/seamm_installer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-02 16:10:10.000000 seamm-installer-2023.4.2/seamm_installer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-02 16:10:10.000000 seamm-installer-2023.4.2/seamm_installer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-02 16:10:10.000000 seamm-installer-2023.4.2/seamm_installer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 16:09:48.000000 seamm-installer-2023.4.2/seamm_installer.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-02 16:10:10.288222 seamm-installer-2023.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:10:10.288222 seamm-installer-2023.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:10:10.288222 seamm-installer-2023.4.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/tests/data/seamm.ini
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/tests/test_seamm_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-02 16:09:42.000000 seamm-installer-2023.4.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:35:45.116311 seamm-installer-2023.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-07 13:35:45.116311 seamm-installer-2023.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:35:45.104311 seamm-installer-2023.6.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8568 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:35:45.120311 seamm-installer-2023.6.7/seamm_installer/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-07 13:35:45.120311 seamm-installer-2023.6.7/seamm_installer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:35:45.112311 seamm-installer-2023.6.7/seamm_installer/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   250762 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/SEAMM.icns
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/development.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:35:45.116311 seamm-installer-2023.6.7/seamm_installer/data/linux_icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/linux_icons/128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/linux_icons/16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/linux_icons/24x24.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20257 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/linux_icons/256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/linux_icons/32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/linux_icons/48x48.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48610 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/linux_icons/512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/linux_icons/64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/seamm.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/data/seamm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50770 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27101 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/installer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15092 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/mac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/my.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/seamm_installer/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:35:45.112311 seamm-installer-2023.6.7/seamm_installer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-07 13:35:45.000000 seamm-installer-2023.6.7/seamm_installer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-07 13:35:45.000000 seamm-installer-2023.6.7/seamm_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:35:45.000000 seamm-installer-2023.6.7/seamm_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 13:35:45.000000 seamm-installer-2023.6.7/seamm_installer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 13:35:45.000000 seamm-installer-2023.6.7/seamm_installer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 13:35:45.000000 seamm-installer-2023.6.7/seamm_installer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:35:24.000000 seamm-installer-2023.6.7/seamm_installer.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-07 13:35:45.116311 seamm-installer-2023.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:35:45.116311 seamm-installer-2023.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:35:45.116311 seamm-installer-2023.6.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/tests/data/seamm.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/tests/test_seamm_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-07 13:35:17.000000 seamm-installer-2023.6.7/versioneer.py
```

### Comparing `seamm-installer-2023.4.2/CONTRIBUTING.rst` & `seamm-installer-2023.6.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/LICENSE` & `seamm-installer-2023.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/PKG-INFO` & `seamm-installer-2023.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm-installer
-Version: 2023.4.2
+Version: 2023.6.7
 Summary: The installer/updater for SEAMM (Simulation Environment for Atomistic and Molecular Simulations).
 Home-page: https://github.com/molssi-seamm/seamm_installer
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3+
 Keywords: SEAMM,plug-in,flowchart,installer,updater
 Platform: Linux
@@ -89,14 +89,16 @@
 
 
 
 =======
 History
 =======
 
+2023.6.7 Bugfix: Ensuring the LaunchAgents directory exists on Mac
+
 2023.4.2 Bugfix: Updating full conda environment breaks pinning.
    So removed that capability.
    
 2023.4.1.1 Bugfix: Problem with JobServer service
 
 2023.4.1 Bugfix: get latest version from Zenodo
```

### Comparing `seamm-installer-2023.4.2/README.rst` & `seamm-installer-2023.6.7/README.rst`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/docs/Makefile` & `seamm-installer-2023.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/docs/conf.py` & `seamm-installer-2023.6.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/docs/installation.rst` & `seamm-installer-2023.6.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/docs/make.bat` & `seamm-installer-2023.6.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/__init__.py` & `seamm-installer-2023.6.7/seamm_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/__main__.py` & `seamm-installer-2023.6.7/seamm_installer/__main__.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/apps.py` & `seamm-installer-2023.6.7/seamm_installer/apps.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/cache.py` & `seamm-installer-2023.6.7/seamm_installer/cache.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/cli.py` & `seamm-installer-2023.6.7/seamm_installer/cli.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/conda.py` & `seamm-installer-2023.6.7/seamm_installer/conda.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/configuration.py` & `seamm-installer-2023.6.7/seamm_installer/configuration.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/SEAMM.icns` & `seamm-installer-2023.6.7/seamm_installer/data/SEAMM.icns`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/development.yml` & `seamm-installer-2023.6.7/seamm_installer/data/development.yml`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/linux_icons/128x128.png` & `seamm-installer-2023.6.7/seamm_installer/data/linux_icons/128x128.png`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/linux_icons/16x16.png` & `seamm-installer-2023.6.7/seamm_installer/data/linux_icons/16x16.png`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/linux_icons/24x24.png` & `seamm-installer-2023.6.7/seamm_installer/data/linux_icons/24x24.png`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/linux_icons/256x256.png` & `seamm-installer-2023.6.7/seamm_installer/data/linux_icons/256x256.png`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/linux_icons/32x32.png` & `seamm-installer-2023.6.7/seamm_installer/data/linux_icons/32x32.png`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/linux_icons/48x48.png` & `seamm-installer-2023.6.7/seamm_installer/data/linux_icons/48x48.png`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/linux_icons/512x512.png` & `seamm-installer-2023.6.7/seamm_installer/data/linux_icons/512x512.png`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/linux_icons/64x64.png` & `seamm-installer-2023.6.7/seamm_installer/data/linux_icons/64x64.png`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/data/seamm.ini` & `seamm-installer-2023.6.7/seamm_installer/data/seamm.ini`

 * *Files 6% similar despite different names*

```diff
@@ -70,10 +70,10 @@
 # while 'all' requests using all the physical memory.
 # The default is 'available'.
 # max-memory = available
 
 ######################################
 # Options for the Dashboard          #
 ######################################
-secret-key = 
+secret-key = b'\xd2/T`\x80\xb4\xa9\xfe7k\x05]\x16\xe5\x90\x125\xe8\x99(\xe2\x9b{\x16\x9aH\xfa\x88\x14@\xe2\xcc'
 debug = False
```

### Comparing `seamm-installer-2023.4.2/seamm_installer/datastore.py` & `seamm-installer-2023.6.7/seamm_installer/datastore.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/gui.py` & `seamm-installer-2023.6.7/seamm_installer/gui.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/install.py` & `seamm-installer-2023.6.7/seamm_installer/install.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/installer_base.py` & `seamm-installer-2023.6.7/seamm_installer/installer_base.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/linux.py` & `seamm-installer-2023.6.7/seamm_installer/linux.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/mac.py` & `seamm-installer-2023.6.7/seamm_installer/mac.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,15 @@
             plist["UserName"] = username
 
         # Reset the service data so it is re-read
         self._data = None
 
         # Write the file ... we may not have permission, so catch that.
         try:
+            launchd_path.mkdir(parents=True, exist_ok=True)
             with plist_path.open(mode="wb") as fd:
                 plistlib.dump(plist, fd)
         except PermissionError:
             path = Path("~/Downloads").expanduser() / f"{identifier}.plist"
             with path.open(mode="wb") as fd:
                 plistlib.dump(plist, fd)
             print(f"\nYou do not have permission to write to {launchd_path}.")
```

### Comparing `seamm-installer-2023.4.2/seamm_installer/metadata.py` & `seamm-installer-2023.6.7/seamm_installer/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "rdkit-step",
     "read-structure-step",
     "set-cell-step",
     "strain-step",
     "supercell-step",
     "torchani-step",
     "table-step",
+    "thermal-conductivity-step",
 )
 external_plug_ins = []
 
 excluded_plug_ins = (
     "chemical-formula",
     "cms-plots",
     "seamm-dashboard-client",
```

### Comparing `seamm-installer-2023.4.2/seamm_installer/pip.py` & `seamm-installer-2023.6.7/seamm_installer/pip.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/services.py` & `seamm-installer-2023.6.7/seamm_installer/services.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/show.py` & `seamm-installer-2023.6.7/seamm_installer/show.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/uninstall.py` & `seamm-installer-2023.6.7/seamm_installer/uninstall.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/update.py` & `seamm-installer-2023.6.7/seamm_installer/update.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer/util.py` & `seamm-installer-2023.6.7/seamm_installer/util.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/seamm_installer.egg-info/PKG-INFO` & `seamm-installer-2023.6.7/seamm_installer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm-installer
-Version: 2023.4.2
+Version: 2023.6.7
 Summary: The installer/updater for SEAMM (Simulation Environment for Atomistic and Molecular Simulations).
 Home-page: https://github.com/molssi-seamm/seamm_installer
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3+
 Keywords: SEAMM,plug-in,flowchart,installer,updater
 Platform: Linux
@@ -89,14 +89,16 @@
 
 
 
 =======
 History
 =======
 
+2023.6.7 Bugfix: Ensuring the LaunchAgents directory exists on Mac
+
 2023.4.2 Bugfix: Updating full conda environment breaks pinning.
    So removed that capability.
    
 2023.4.1.1 Bugfix: Problem with JobServer service
 
 2023.4.1 Bugfix: get latest version from Zenodo
```

### Comparing `seamm-installer-2023.4.2/seamm_installer.egg-info/SOURCES.txt` & `seamm-installer-2023.6.7/seamm_installer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/setup.py` & `seamm-installer-2023.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/tests/conftest.py` & `seamm-installer-2023.6.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/tests/data/seamm.ini` & `seamm-installer-2023.6.7/tests/data/seamm.ini`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/tests/test_configuration.py` & `seamm-installer-2023.6.7/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `seamm-installer-2023.4.2/versioneer.py` & `seamm-installer-2023.6.7/versioneer.py`

 * *Files identical despite different names*

