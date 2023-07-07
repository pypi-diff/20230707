# Comparing `tmp/anta-0.5.0.tar.gz` & `tmp/anta-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anta-0.5.0.tar", last modified: Fri Mar 31 09:47:49 2023, max compression
+gzip compressed data, was "anta-0.6.0.tar", last modified: Fri Jul  7 10:29:38 2023, max compression
```

## Comparing `anta-0.5.0.tar` & `anta-0.6.0.tar`

### file list

```diff
@@ -1,69 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.180183 anta-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-03-31 09:47:38.000000 anta-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-31 09:47:38.000000 anta-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-03-31 09:47:49.176183 anta-0.5.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3747 2023-03-31 09:47:38.000000 anta-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.172183 anta-0.5.0/anta/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-31 09:47:38.000000 anta-0.5.0/anta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.172183 anta-0.5.0/anta/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.176183 anta-0.5.0/anta/cli/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/check/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/check/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.176183 anta-0.5.0/anta/cli/exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/exec/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/exec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.176183 anta-0.5.0/anta/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/get/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/get/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-31 09:47:38.000000 anta-0.5.0/anta/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-03-31 09:47:38.000000 anta-0.5.0/anta/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.176183 anta-0.5.0/anta/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-03-31 09:47:38.000000 anta-0.5.0/anta/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-31 09:47:38.000000 anta-0.5.0/anta/inventory/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-03-31 09:47:38.000000 anta-0.5.0/anta/inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-31 09:47:38.000000 anta-0.5.0/anta/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.176183 anta-0.5.0/anta/reporter/
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-03-31 09:47:38.000000 anta-0.5.0/anta/reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-31 09:47:38.000000 anta-0.5.0/anta/reporter/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.176183 anta-0.5.0/anta/result_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-03-31 09:47:38.000000 anta-0.5.0/anta/result_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-31 09:47:38.000000 anta-0.5.0/anta/result_manager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-31 09:47:38.000000 anta-0.5.0/anta/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.176183 anta-0.5.0/anta/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/mlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/multicast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.176183 anta-0.5.0/anta/tests/routing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/routing/bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/routing/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/routing/ospf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/software.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tests/vxlan.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-31 09:47:38.000000 anta-0.5.0/anta/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.172183 anta-0.5.0/anta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-03-31 09:47:49.000000 anta-0.5.0/anta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-31 09:47:49.000000 anta-0.5.0/anta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 09:47:49.000000 anta-0.5.0/anta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 09:47:49.000000 anta-0.5.0/anta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-31 09:47:49.000000 anta-0.5.0/anta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-31 09:47:49.000000 anta-0.5.0/anta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-03-31 09:47:38.000000 anta-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:47:49.176183 anta-0.5.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10005 2023-03-31 09:47:38.000000 anta-0.5.0/scripts/check-devices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2825 2023-03-31 09:47:38.000000 anta-0.5.0/scripts/clear-counters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5378 2023-03-31 09:47:38.000000 anta-0.5.0/scripts/collect-eos-commands.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5091 2023-03-31 09:47:38.000000 anta-0.5.0/scripts/collect-scheduled-show-tech.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3861 2023-03-31 09:47:38.000000 anta-0.5.0/scripts/create-devices-inventory-from-cvp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3264 2023-03-31 09:47:38.000000 anta-0.5.0/scripts/evpn-blacklist-recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 09:47:49.180183 anta-0.5.0/setup.cfg
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.622272 anta-0.6.0/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    11345 2022-07-20 14:15:12.000000 anta-0.6.0/LICENSE
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)       21 2023-03-31 08:52:22.000000 anta-0.6.0/MANIFEST.in
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    18259 2023-07-07 10:29:38.621614 anta-0.6.0/PKG-INFO
+-rwxr-xr-x   0 guillaumemulocher   (501) staff       (20)     3789 2023-07-07 10:29:22.000000 anta-0.6.0/README.md
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.583246 anta-0.6.0/anta/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1102 2023-07-06 12:52:04.000000 anta-0.6.0/anta/__init__.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.586721 anta-0.6.0/anta/cli/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4082 2023-07-06 16:02:24.000000 anta-0.6.0/anta/cli/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      284 2023-07-07 09:53:40.000000 anta-0.6.0/anta/cli/console.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.587368 anta-0.6.0/anta/cli/debug/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-04-27 09:11:04.000000 anta-0.6.0/anta/cli/debug/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3571 2023-07-07 09:53:40.000000 anta-0.6.0/anta/cli/debug/commands.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.589091 anta-0.6.0/anta/cli/exec/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-02-14 08:55:44.000000 anta-0.6.0/anta/cli/exec/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3308 2023-07-04 13:25:37.000000 anta-0.6.0/anta/cli/exec/commands.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7155 2023-07-07 08:14:08.000000 anta-0.6.0/anta/cli/exec/utils.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.590189 anta-0.6.0/anta/cli/get/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-03-31 09:09:54.000000 anta-0.6.0/anta/cli/get/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3708 2023-07-06 12:52:04.000000 anta-0.6.0/anta/cli/get/commands.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1748 2023-04-27 09:11:04.000000 anta-0.6.0/anta/cli/get/utils.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.591713 anta-0.6.0/anta/cli/nrfu/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-07-03 15:42:22.000000 anta-0.6.0/anta/cli/nrfu/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4799 2023-07-07 08:14:08.000000 anta-0.6.0/anta/cli/nrfu/commands.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4573 2023-07-07 08:14:08.000000 anta-0.6.0/anta/cli/nrfu/utils.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4343 2023-07-06 16:02:24.000000 anta-0.6.0/anta/cli/utils.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3780 2023-07-07 08:14:08.000000 anta-0.6.0/anta/decorators.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    13884 2023-07-07 09:53:40.000000 anta-0.6.0/anta/device.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.593011 anta-0.6.0/anta/inventory/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7250 2023-07-07 08:14:08.000000 anta-0.6.0/anta/inventory/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      252 2023-07-03 15:42:22.000000 anta-0.6.0/anta/inventory/exceptions.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2368 2023-07-06 12:52:04.000000 anta-0.6.0/anta/inventory/models.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3249 2023-07-06 12:52:04.000000 anta-0.6.0/anta/loader.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    12824 2023-07-07 08:14:08.000000 anta-0.6.0/anta/models.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.594030 anta-0.6.0/anta/reporter/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    10362 2023-07-06 12:52:04.000000 anta-0.6.0/anta/reporter/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1305 2023-04-27 09:11:04.000000 anta-0.6.0/anta/reporter/models.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.594816 anta-0.6.0/anta/result_manager/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7677 2023-07-06 16:02:24.000000 anta-0.6.0/anta/result_manager/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4163 2023-07-06 12:52:04.000000 anta-0.6.0/anta/result_manager/models.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2894 2023-07-07 08:14:08.000000 anta-0.6.0/anta/runner.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.615466 anta-0.6.0/anta/tests/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-07-03 15:42:22.000000 anta-0.6.0/anta/tests/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    15959 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/aaa.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1498 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/configuration.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1629 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/connectivity.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     6469 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/field_notices.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     8554 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/hardware.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    15459 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/interfaces.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    10182 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/logging.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     9689 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/mlag.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3228 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/multicast.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2341 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/profiles.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.617133 anta-0.6.0/anta/tests/routing/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-07-22 08:02:04.000000 anta-0.6.0/anta/tests/routing/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    11774 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/routing/bgp.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4579 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/routing/generic.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3640 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/routing/ospf.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    12534 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/security.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     5452 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/snmp.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3646 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/software.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     8447 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/stp.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7616 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/system.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2293 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/vxlan.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.619181 anta-0.6.0/anta/tools/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-04-27 09:11:04.000000 anta-0.6.0/anta/tools/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1716 2023-07-03 15:42:22.000000 anta-0.6.0/anta/tools/get_value.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      614 2023-07-03 15:42:22.000000 anta-0.6.0/anta/tools/misc.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      795 2023-07-03 15:42:22.000000 anta-0.6.0/anta/tools/pydantic.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.585390 anta-0.6.0/anta.egg-info/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    18259 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/PKG-INFO
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1514 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        1 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)       38 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/entry_points.txt
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      495 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/requires.txt
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        5 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/top_level.txt
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     5816 2023-07-07 10:29:22.000000 anta-0.6.0/pyproject.toml
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)       38 2023-07-07 10:29:38.622343 anta-0.6.0/setup.cfg
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.619891 anta-0.6.0/tests/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-07-20 14:15:12.000000 anta-0.6.0/tests/__init__.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.620489 anta-0.6.0/tests/data/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-07-20 14:15:12.000000 anta-0.6.0/tests/data/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7834 2023-07-03 15:42:22.000000 anta-0.6.0/tests/data/json_data.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.620997 anta-0.6.0/tests/units/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-07-20 14:15:12.000000 anta-0.6.0/tests/units/__init__.py
```

### Comparing `anta-0.5.0/LICENSE` & `anta-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anta-0.5.0/PKG-INFO` & `anta-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anta
-Version: 0.5.0
+Version: 0.6.0
 Summary: Arista Network Test Automation (ANTA) Framework
 Author-email: Khelil Sator <ksator@arista.com>
 Maintainer-email: Khelil Sator <ksator@arista.com>, Matthieu Tâche <mtache@arista.com>, Khelil Sator <ksator@arista.com>, Guillaume Mulocher <gmulocher@arista.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -202,17 +202,17 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Project-URL: Homepage, https://arista-netdevops-community.github.io/network-test-automation/
-Project-URL: Bug Tracker, https://github.com/arista-netdevops-community/network-test-automation/issues
-Project-URL: Contributing, https://github.com/arista-netdevops-community/network-test-automation/blob/master/CONTRIBUTING.md
+Project-URL: Homepage, https://www.anta.ninja
+Project-URL: Bug Tracker, https://github.com/arista-netdevops-community/anta/issues
+Project-URL: Contributing, https://github.com/arista-netdevops-community/anta/blob/master/CONTRIBUTING.md
 Keywords: test,anta,Arista,network,automation,networking,devops,netdevops
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -226,20 +226,22 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-[![License](https://img.shields.io/badge/license-Apache%202.0-brightgreen.svg)](https://github.com/arista-netdevops-community/network-test-automation/blob/master/LICENSE)
-[![CI](https://github.com/arista-netdevops-community/network-test-automation/actions/workflows/test.yml/badge.svg)](https://github.com/arista-netdevops-community/network-test-automation/actions)
-[![github release](https://img.shields.io/github/release/arista-netdevops-community/network-test-automation.svg)](https://github.com/arista-netdevops-community/network-test-automation/releases/)
+[![License](https://img.shields.io/badge/license-Apache%202.0-brightgreen.svg)](https://github.com/arista-netdevops-community/anta/blob/master/LICENSE)
+[![Linting and Testing Anta](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml/badge.svg)](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml)
+[![github release](https://img.shields.io/github/release/arista-netdevops-community/anta.svg)](https://github.com/arista-netdevops-community/anta/releases/)
 
 # Arista Network Test Automation (ANTA) Framework
 
+__WARNING:__ Documentation is work in progress for version 0.6.0 available in Pypi.
+
 This repository is a Python package to automate tests on Arista devices.
 
 - The package name is ANTA, which stands for **Arista Network Test Automation**.
 - This package provides a set of tests to validate the state of your network.
 - This package can be imported in Python scripts:
   - To automate NRFU (Network Ready For Use) test on a preproduction network
   - To automate tests on a live network (periodically or on demand)
@@ -250,48 +252,52 @@
 # Install ANTA CLI
 $ pip install anta
 
 # Run ANTA CLI
 $ anta
 Usage: anta [OPTIONS] COMMAND [ARGS]...
 
-  Arista Network Test CLI
+  Arista Network Test Automation (ANTA) CLI
 
 Options:
-  --username TEXT         Username to connect to EOS  [env var: ANTA_USERNAME]
-  --password TEXT         Password to connect to EOS  [env var: ANTA_PASSWORD]
-  --timeout INTEGER       Connection timeout (default 5)  [env var: ANTA_TIMEOUT]
-  --enable-password TEXT  Enable password if required to connect  [env var: ANTA_ENABLE_PASSWORD]
-  -i, --inventory PATH    Path to your inventory file  [env var: ANTA_INVENTORY]
-  --timeout INTEGER       Connection timeout (default 5)  [env var: ANTA_TIMEOUT]
-  --help                  Show this message and exit.
+  --version                       Show the version and exit.
+  --username TEXT                 Username to connect to EOS  [env var:
+                                  ANTA_USERNAME; required]
+  --password TEXT                 Password to connect to EOS  [env var:
+                                  ANTA_PASSWORD; required]
+  --timeout INTEGER               Global connection timeout  [env var:
+                                  ANTA_TIMEOUT; default: 5]
+  --insecure                      Disable SSH Host Key validation  [env var:
+                                  ANTA_INSECURE]
+  --enable-password TEXT          Enable password if required to connect  [env
+                                  var: ANTA_ENABLE_PASSWORD]
+  -i, --inventory FILE            Path to the inventory YAML file  [env var:
+                                  ANTA_INVENTORY; required]
+  --log-level, --log [CRITICAL|ERROR|WARNING|INFO|DEBUG]
+                                  ANTA logging level  [env var:
+                                  ANTA_LOG_LEVEL; default: INFO]
+  --ignore-status                 Always exit with success  [env var:
+                                  ANTA_IGNORE_STATUS]
+  --ignore-error                  Only report failures and not errors  [env
+                                  var: ANTA_IGNORE_ERROR]
+  --help                          Show this message and exit.
 
 Commands:
-  exec  Execute commands to inventory devices
-  get   Get data from/to ANTA
-  nrfu  Run NRFU against inventory devices
+  debug  Debug commands for building ANTA
+  exec   Execute commands to inventory devices
+  get    Get data from/to ANTA
+  nrfu   Run NRFU against inventory devices
 ```
 
-<img src="https://github.com/arista-netdevops-community/network-test-automation/raw/master/docs/imgs/anta-nrfu-table-group-by-test-output.png"></img>
-
-In addition, previous scripts are now marked as __deprecated__ and will be removed in a future release:
-
-- `check-devices.py` is an easy to use script to test your network with ANTA.
-- `collect-eos-commands.py` to collect commands output from devices
-- `collect-sheduled-show-tech.py` to collect the scheduled show tech-support files from devices
-- `clear-counters.py` to clear counters on devices
-- `evpn-blacklist-recovery.py` to clear the list of MAC addresses which are blacklisted in EVPN
-- `create-devices-inventory-from-cvp.py`: Build inventory for scripts from Arista Cloudvision (CVP)
-
-> Most of these scripts use eAPI (EOS API). You can find examples of EOS automation with eAPI in this [repository](https://github.com/arista-netdevops-community/arista_eos_automation_with_eAPI).
+<img src="https://github.com/arista-netdevops-community/anta/raw/master/docs/imgs/anta-nrfu-table-group-by-test-output.png"></img>
 
 # Documentation
 
-The documentation is published on [ANTA package website](https://arista-netdevops-community.github.io/network-test-automation/)
+The documentation is published on [ANTA package website](https://www.anta.ninja)
 
 # Contribution guide
 
-Contributions are welcome. Please refer to the [contribution guide](https://raw.githubusercontent.com/arista-netdevops-community/network-test-automation/master/docs/contribution.md)
+Contributions are welcome. Please refer to the [contribution guide](https://raw.githubusercontent.com/arista-netdevops-community/anta/master/docs/contribution.md)
 
 # Credits
 
 Thank you to [Angélique Phillipps](https://github.com/aphillipps), [Colin MacGiollaEáin](https://github.com/colinmacgiolla), [Khelil Sator](https://github.com/ksator), [Matthieu Tache](https://github.com/mtache), [Onur Gashi](https://github.com/onurgashi), [Paul Lavelle](https://github.com/paullavelle), [Guillaume Mulocher](https://github.com/gmuloc) and [Thomas Grimonet](https://github.com/titom73) for their contributions and guidances.
```

### Comparing `anta-0.5.0/anta/__init__.py` & `anta-0.6.0/anta/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
-anta init
+Arista Network Test Automation (ANTA) Framework
 """
 import importlib.metadata
+import os
 
 __version__ = importlib.metadata.version("anta")
 __credits__ = [
     "Angélique Phillipps",
     "Colin MacGiollaEáin",
     "Khelil Sator",
     "Matthieu Tâche",
     "Onur Gashi",
     "Paul Lavelle",
     "Guillaume Mulocher",
     "Thomas Grimonet",
 ]
 __copyright__ = "Copyright 2022, Arista EMEA AS"
 
+# Global ANTA debug environment variable. Can be set using the cli 'anta --debug'.
+__DEBUG__ = bool(os.environ.get("ANTA_DEBUG", "").lower() == "true")
+
 
 # Source: https://rich.readthedocs.io/en/stable/appendix/colors.html
 # pylint: disable=R0903
 class RICH_COLOR_PALETTE:
     """Color code for text rendering."""
 
     ERROR = "indian_red"
@@ -30,9 +34,9 @@
 
 
 # Dictionary to use in a Rich.Theme: custom_theme = Theme(RICH_COLOR_THEME)
 RICH_COLOR_THEME = {
     "success": RICH_COLOR_PALETTE.SUCCESS,
     "skipped": RICH_COLOR_PALETTE.SKIPPED,
     "failure": RICH_COLOR_PALETTE.FAILURE,
-    "error": RICH_COLOR_PALETTE.ERROR
+    "error": RICH_COLOR_PALETTE.ERROR,
 }
```

### Comparing `anta-0.5.0/anta/cli/exec/commands.py` & `anta-0.6.0/anta/cli/get/commands.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,94 @@
 #!/usr/bin/env python
 # coding: utf-8 -*-
+# pylint: disable = redefined-outer-name
 
 """
-Commands for Anta CLI to execute EOS commands.
+Commands for Anta CLI to run check commands.
 """
 
 import asyncio
+import json
 import logging
-import sys
+import os
+from typing import List, Optional
 
 import click
-from yaml import safe_load
+from cvprac.cvp_client import CvpClient
+from cvprac.cvp_client_errors import CvpApiError
+from rich.pretty import pretty_repr
+
+from anta.cli.console import console
+from anta.cli.utils import parse_tags
+from anta.models import DEFAULT_TAG
 
-from anta.cli.exec.utils import clear_counters_utils, collect_scheduled_show_tech, collect_commands
-from anta.cli.utils import setup_logging
-from anta.inventory import AntaInventory
-from anta.inventory.models import DEFAULT_TAG
+from .utils import create_inventory, get_cv_token
 
 logger = logging.getLogger(__name__)
 
 
-@click.command()
-@click.pass_context
-# Generic options
-@click.option('--tags', '-t', default='all', help='List of tags using coma as separator: tag1,tag2,tag3', type=str)
-# Debug stuf
-@click.option('--log-level', '--log', help='Logging level of the command', default='info',
-              type=click.Choice(['debug', 'info', 'warning', 'critical'], case_sensitive=False))
-def clear_counters(ctx: click.Context, log_level: str, tags: str) -> None:
-    """Clear counter statistics on EOS devices"""
-
-    setup_logging(level=log_level)
-
-    inventory_anta = AntaInventory(
-        inventory_file=ctx.obj['inventory'],
-        username=ctx.obj['username'],
-        password=ctx.obj['password'],
-        enable_password=ctx.obj['enable_password']
-    )
-    asyncio.run(clear_counters_utils(
-        inventory_anta, ctx.obj['enable_password'], tags=tags.split(','))
-        )
+@click.command(no_args_is_help=True)
+@click.option("--cvp-ip", "-ip", default=None, help="CVP IP Address", type=str, required=True)
+@click.option("--cvp-username", "-u", default=None, help="CVP Username", type=str, required=True)
+@click.option("--cvp-password", "-p", default=None, help="CVP Password / token", type=str, required=True)
+@click.option("--cvp-container", "-c", default=None, help="Container where devices are configured", type=str, required=False)
+@click.option("--inventory-directory", "-d", default=None, help="Path to save inventory file", type=click.Path())
+def from_cvp(inventory_directory: str, cvp_ip: str, cvp_username: str, cvp_password: str, cvp_container: str) -> None:
+    """Build ANTA inventory from Cloudvision"""
+    # pylint: disable=too-many-arguments
+    logger.info(f"Getting auth token from {cvp_ip} for user {cvp_username}")
+    token = get_cv_token(cvp_ip=cvp_ip, cvp_username=cvp_username, cvp_password=cvp_password)
+
+    # Create output directory
+    cwd = os.getcwd()
+    out_dir = os.path.dirname(f"{cwd}/{inventory_directory}/")
+    if not os.path.exists(out_dir):
+        logger.info(f"Creating inventory folder {out_dir}")
+        os.makedirs(out_dir)
+
+    clnt = CvpClient()
+    try:
+        clnt.connect(nodes=[cvp_ip], username="", password="", api_token=token)
+    except CvpApiError as error:
+        logger.error(f"Error connecting to cvp: {error}")
+    logger.info(f"Connected to CVP {cvp_ip}")
+
+    cvp_inventory = None
+    if cvp_container is None:
+        # Get a list of all devices
+        logger.info(f"Getting full inventory from {cvp_ip}")
+        cvp_inventory = clnt.api.get_inventory()
+    else:
+        # Get devices under a container
+        logger.info(f"Getting inventory for container {cvp_container} from {cvp_ip}")
+        cvp_inventory = clnt.api.get_devices_in_container(cvp_container)
+    create_inventory(cvp_inventory, out_dir, cvp_container)
 
 
 @click.command()
 @click.pass_context
-# Generic options
-@click.option('--tags', '-t', default=DEFAULT_TAG, help='List of tags using coma as separator: tag1,tag2,tag3', type=str, required=False)
-@click.option('--commands-list', '-c', show_envvar=True, type=click.Path(), help='File with list of commands to grab', required=True)
-@click.option('--output-directory', '-outut', '-o', show_envvar=True, type=click.Path(), help='Path where to save commands output', required=False)
-# Debug stuf
-@click.option('--log-level', '--log', help='Logging level of the command', default='info',
-              type=click.Choice(['debug', 'info', 'warning', 'critical'], case_sensitive=False))
-def snapshot(ctx: click.Context, commands_list: str, log_level: str, output_directory: str, tags: str) -> None:
-    """Collect commands output from devices in inventory"""
-    setup_logging(level=log_level)
-    try:
-        with open(commands_list, "r", encoding="UTF-8") as file:
-            file_content = file.read()
-            eos_commands = safe_load(file_content)
-    except FileNotFoundError:
-        logger.error(f"Error reading {commands_list}")
-        sys.exit(1)
-    inventory = AntaInventory(
-        inventory_file=ctx.obj['inventory'],
-        username=ctx.obj['username'],
-        password=ctx.obj['password'],
-        enable_password=ctx.obj['enable_password']
-    )
-    asyncio.run(collect_commands(inventory, ctx.obj['enable_password'],
-                eos_commands, output_directory, tags=tags.split(',')))
+@click.option("--tags", "-t", help="List of tags using comma as separator: tag1,tag2,tag3", type=str, required=False, callback=parse_tags)
+@click.option("--connected/--not-connected", help="Display inventory after connection has been created", default=False, required=False)
+def inventory(ctx: click.Context, tags: Optional[List[str]], connected: bool) -> None:
+    """Show inventory loaded in ANTA."""
+
+    logger.debug(f"Requesting devices for tags: {tags}")
+    console.print("Current inventory content is:", style="white on blue")
+
+    if connected:
+        asyncio.run(ctx.obj["inventory"].connect_inventory())
+
+    inventory_result = ctx.obj["inventory"].get_inventory(tags=tags)
+    console.print(pretty_repr(inventory_result))
 
 
 @click.command()
 @click.pass_context
-@click.option('--output', '-o', default='./tech-support/', help='Path for tests catalog', type=click.Path(), required=False)
-@click.option('--ssh-port', '-ssh', default=22, help='SSH port to use for connection', type=int, required=False)
-@click.option('--tags', '-t', default=DEFAULT_TAG, help='List of tags using coma as separator: tag1,tag2,tag3', type=str, required=False)
-# Debug stuf
-@click.option('--log-level', '--log', help='Logging level of the command', default='info',
-              type=click.Choice(['debug', 'info', 'warning', 'critical'], case_sensitive=False))
-def collect_tech_support(ctx: click.Context, output: str, ssh_port: int, log_level: str, tags: str) -> bool:
-    """Collect scheduled tech-support from eos devices."""
-    setup_logging(level=log_level)
-    inventory = AntaInventory(
-        inventory_file=ctx.obj['inventory'],
-        username=ctx.obj['username'],
-        password=ctx.obj['password'],
-        enable_password=ctx.obj['enable_password']
-    )
-    asyncio.run(collect_scheduled_show_tech(inventory, output, tags=tags.split(','), ssh_port=ssh_port))
-    return True
+def tags(ctx: click.Context) -> None:
+    """Get list of configured tags in user inventory."""
+    tags_found = []
+    for device in ctx.obj["inventory"]:
+        tags_found += device.tags
+    tags_found = sorted(set(tags_found))
+    console.print("Tags found:")
+    console.print_json(json.dumps(tags_found, indent=2))
+    console.print(f"\n* note that tag [green]{DEFAULT_TAG}[/green] has been added by anta")
```

### Comparing `anta-0.5.0/anta/cli/exec/utils.py` & `anta-0.6.0/anta/cli/exec/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,182 +2,157 @@
 # coding: utf-8 -*-
 
 """
 Exec CLI helpers
 """
 
 import asyncio
+import itertools
+import json
 import logging
-import os
-import traceback
-from time import gmtime, strftime
-from typing import Dict, List, Tuple
+from pathlib import Path
+from typing import Dict, List, Literal, Optional
 
 from aioeapi import EapiCommandError
-from scp import SCPClient
 
+from anta import __DEBUG__
+from anta.device import AntaDevice
 from anta.inventory import AntaInventory
-from anta.inventory.models import InventoryDevice
-
-EOS_TECH_SUPPORT_ARCHIVE_ZIP = "/mnt/flash/schedule/all_files.zip"
+from anta.models import AntaCommand
+from anta.tools.misc import exc_to_str
 
+EOS_SCHEDULED_TECH_SUPPORT = "/mnt/flash/schedule/tech-support"
 
 logger = logging.getLogger(__name__)
 
 
-async def clear_counters_utils(anta_inventory: AntaInventory, enable_pass: str, tags: List[str]) -> None:
+async def clear_counters_utils(anta_inventory: AntaInventory, tags: Optional[List[str]] = None) -> None:
     """
-    clear counters
+    Clear counters
     """
-    async def clear(dev: InventoryDevice) -> None:
-        logger.info(f'Clearing counter for {dev.name} ({dev.hw_model})')
-        commands = [{"cmd": "enable", "input": enable_pass}, "clear counters"]
+
+    async def clear(dev: AntaDevice) -> None:
+        commands = [AntaCommand(command="clear counters")]
         if dev.hw_model not in ["cEOSLab", "vEOS-lab"]:
-            commands.append("clear hardware counter drop")
-        try:
-            await dev.session.cli(commands=commands)
-            logger.info(f"Cleared counters on {dev.name}")
-        # In this case we want to catch all exceptions
-        except Exception as e:  # pylint: disable=broad-except
-            logger.error(f"Could not clear counters on device {dev.name}")
-            logger.debug(
-                f"Exception raised for device {dev.name} - {type(e).__name__}: {str(e)}"
-            )
-            logger.debug(traceback.format_exc())
+            commands.append(AntaCommand(command="clear hardware counter drop"))
+        await dev.collect_commands(commands=commands)
+        for command in commands:
+            if not command.collected:
+                logger.error(f"Could not clear counters on device {dev.name}: {command.failed}")
+        logger.info(f"Cleared counters on {dev.name} ({dev.hw_model})")
 
-    logger.info('Reading inventory')
+    logger.info("Connecting to devices...")
     await anta_inventory.connect_inventory()
-    devices = anta_inventory.get_inventory(established_only=True, tags=tags)
-    logger.info('Execute command to remote devices')
+    devices = anta_inventory.get_inventory(established_only=True, tags=tags).values()
+    logger.info("Clearing counters on remote devices...")
     await asyncio.gather(*(clear(device) for device in devices))
 
 
-def device_directories_snapshot(
-    device: InventoryDevice, root_dir: str
-) -> Tuple[str, str, str, str]:
-    """
-    Create device directories
-    """
-    cwd = os.getcwd()
-    output_directory = os.path.dirname(f"{cwd}/{root_dir}/")
-    device_directory = f"{output_directory}/{device.name}"
-    json_directory = f"{device_directory}/json"
-    text_directory = f"{device_directory}/text"
-    for directory in [
-        output_directory,
-        device_directory,
-        json_directory,
-        text_directory,
-    ]:
-        if not os.path.exists(directory):
-            os.makedirs(directory)
-    return output_directory, device_directory, json_directory, text_directory
-
-
-async def collect_commands(inv: AntaInventory,  enable_pass: str, commands: Dict[str, str], root_dir: str, tags: List[str]) -> None:
+async def collect_commands(
+    inv: AntaInventory,
+    commands: Dict[str, str],
+    root_dir: Path,
+    tags: Optional[List[str]] = None,
+) -> None:
     """
     Collect EOS commands
     """
-    logger.info("Connecting to devices...")
-    await inv.connect_inventory()
-    devices = inv.get_inventory(established_only=True, tags=tags)
-    for device in devices:  # TODO: should use asyncio.gather instead of a loop.
-        logger.info("----")
-        logger.info(f"Collecting show commands output to device {device.name}")
-        output_dir = device_directories_snapshot(device, root_dir)
-        try:
-            if "json_format" in commands:
-                for command in commands["json_format"]:
-                    result = await device.session.cli(
-                        commands=[
-                            {"cmd": "enable", "input": enable_pass}, command],
-                        ofmt='json'
-                    )
-                    outfile = f"{output_dir[2]}/{command}"
-                    with open(outfile, "w", encoding="UTF-8") as out_fd:
-                        out_fd.write(str(result[1]))
-                    logger.info(
-                        f"  * Collected command '{command}' on {device.name}")
-            if "text_format" in commands:
-                for command in commands["text_format"]:
-                    result = await device.session.cli(
-                        commands=[
-                            {"cmd": "enable", "input": enable_pass}, command],
-                        ofmt='text'
-                    )
-                    outfile = f"{output_dir[3]}/{command}"
-                    with open(outfile, "w", encoding="UTF-8") as out_fd:
-                        out_fd.write(f'{device.name}# {command}\n\r')
-                        out_fd.write(result[1])
-                    logger.info(
-                        f"  * Collected command '{command}' on {device.name}")
-        except EapiCommandError as e:
-            logger.error(f"Command failed on {device.name}: {e.errmsg}")
-        except Exception as e:  # pylint: disable=broad-except
-            logger.error(f"Could not collect commands on device {device.name}")
-            logger.debug(
-                f"Exception raised for device {device.name} - {type(e).__name__}: {str(e)}"
-            )
-            logger.debug(traceback.format_exc())
 
+    async def collect(dev: AntaDevice, command: str, outformat: Literal["json", "text"]) -> None:
+        outdir = Path() / root_dir / dev.name / outformat
+        outdir.mkdir(parents=True, exist_ok=True)
+        c = AntaCommand(command=command, ofmt=outformat)
+        await dev.collect(c)
+        if not c.collected and c.failed is not None:
+            logger.error(f"Could not collect commands on device {dev.name}: {exc_to_str(c.failed)}")
+            return
+        if c.ofmt == "json":
+            outfile = outdir / f"{command}.json"
+            content = json.dumps(c.json_output, indent=2)
+        elif c.ofmt == "text":
+            outfile = outdir / f"{command}.log"
+            content = c.text_output
+        with outfile.open(mode="w", encoding="UTF-8") as f:
+            f.write(content)
+        logger.info(f"Collected command '{command}' from device {dev.name} ({dev.hw_model})")
 
-def device_directories_show_tech_support(dev: str, root_dir: str) -> str:
-    """
-    return a tuple containing the show_tech_directory and the device_directory
-    """
-    device_directory = f"{os.getcwd()}/{root_dir}/{dev}"
-    os.makedirs(device_directory, exist_ok=True)
-    return device_directory
+    logger.info("Connecting to devices...")
+    await inv.connect_inventory()
+    devices = inv.get_inventory(established_only=True, tags=tags).values()
+    logger.info("Collecting commands from remote devices")
+    coros = [collect(device, command, "json") for device, command in itertools.product(devices, commands["json_format"])]
+    coros += [collect(device, command, "text") for device, command in itertools.product(devices, commands["text_format"])]
+    res = await asyncio.gather(*coros, return_exceptions=True)
+    for r in res:
+        if isinstance(r, Exception):
+            message = "Error when collecting commands"
+            if __DEBUG__:
+                logger.exception(message, exc_info=r)
+            else:
+                logger.error(f"{message}: {exc_to_str(r)}")
 
 
-async def collect_scheduled_show_tech(inv: AntaInventory, root_dir: str, tags: List[str], ssh_port: int = 22) -> None:
+async def collect_scheduled_show_tech(inv: AntaInventory, root_dir: Path, configure: bool, tags: Optional[List[str]] = None, latest: Optional[int] = None) -> None:
     """
     Collect scheduled show-tech on devices
     """
-    # Set date here so we have same timestamp for all devices.
-    date_current = strftime("%d %b %Y %H:%M:%S", gmtime())
-    logger.info("Connecting to devices...")
-    await inv.connect_inventory()
-    devices = inv.get_inventory(established_only=True, tags=tags)
-    if len(devices) > 0:
-        # Collect all the tech-support files stored on Arista switches flash and copy them locally
-        for device in devices:  # TODO: should use asyncio.gather instead of a loop.
-            try:
-                # Create one zip file named all_files.zip on the device with the all the show tech-support files in it
-                await device.session.cli(
-                    command=f"bash timeout 30 zip {EOS_TECH_SUPPORT_ARCHIVE_ZIP} /mnt/flash/schedule/tech-support/*"
-                )
-                logger.info(f"Created {EOS_TECH_SUPPORT_ARCHIVE_ZIP} on device {device.name}")
 
-            except EapiCommandError as e:
-                logger.error(f"Unable to create tech-support archove on {device.name}: {e.errmsg}")
+    async def collect(device: AntaDevice) -> None:
+        """
+        Collect all the tech-support files stored on Arista switches flash and copy them locally
+        """
+        try:
+            # Get the tech-support filename to retrieve
+            cmd = f"bash timeout 10 ls -1t {EOS_SCHEDULED_TECH_SUPPORT}"
+            if latest:
+                cmd += f" | head -{latest}"
+            command = AntaCommand(command=cmd, ofmt="text")
+            await device.collect(command=command)
+            if command.collected and command.text_output:
+                filenames = list(map(lambda f: Path(f"{EOS_SCHEDULED_TECH_SUPPORT}/{f}"), command.text_output.splitlines()))
+            else:
+                logger.error(f"Unable to get tech-support filenames on {device.name}: verify that {EOS_SCHEDULED_TECH_SUPPORT} is not empty")
+                return
 
             # Create directories
-            tech_support_root_local_path = device_directories_show_tech_support(
-                device.name, root_dir)
+            outdir = Path() / root_dir / f"{device.name.lower()}"
+            outdir.mkdir(parents=True, exist_ok=True)
 
-            # Connect to the device using SSH
-            ssh = device.create_ssh_socket(ssh_port=ssh_port)
+            # Check if 'aaa authorization exec default local' is present in the running-config
+            command = AntaCommand(command="show running-config | include aaa authorization exec default local", ofmt="text")
+            await device.collect(command=command)
+
+            if command.collected and not command.text_output:
+                logger.debug(f"'aaa authorization exec default local' is not configured on device {device.name}")
+                if configure:
+                    # TODO - @mtache - add `config` field to `AntaCommand` object to handle this use case.
+                    commands = [
+                        {"cmd": "enable", "input": device._enable_password},  # type: ignore[attr-defined] # pylint: disable=protected-access
+                        "configure terminal",
+                        "aaa authorization exec default local",
+                    ]
+                    command = AntaCommand(command="show running-config | include aaa authorization exec default local", ofmt="text")
+                    logger.debug(f"Configuring 'aaa authorization exec default local' on device {device.name}")
+                    await device.session.cli(commands=commands)  # type: ignore[attr-defined]
+                    logger.info(f"Configured 'aaa authorization exec default local' on device {device.name}")
+                else:
+                    logger.error(f"Unable to collect tech-support on {device.name}: configuration 'aaa authorization exec default local' is not present")
+                    return
+            logger.debug(f"'aaa authorization exec default local' is already configured on device {device.name}")
 
-            try:
-                # Get the zipped file all_files.zip using SCP and save it locally
-                tech_support_device_local_path = f"{tech_support_root_local_path}/{date_current}_{device.name.lower()}.zip"
-                with SCPClient(ssh.get_transport()) as scp:
-                    scp.get(EOS_TECH_SUPPORT_ARCHIVE_ZIP, local_path=tech_support_device_local_path)
-
-            except Exception as e:  # pylint: disable=broad-except
-                logger.error(
-                    f"Could not collect show tech files on device {device.name}"
-                )
-                logger.debug(
-                    f"Exception raised for device {device.name} - {type(e).__name__}: {str(e)}"
-                )
-                logger.debug(traceback.format_exc())
-
-            try:
-                # Delete the created zip file on the device
-                await device.session.cli(command=f"bash timeout 30 rm {EOS_TECH_SUPPORT_ARCHIVE_ZIP}")
-                logger.info(f"Deleted {EOS_TECH_SUPPORT_ARCHIVE_ZIP} on {device.name}")
-            except EapiCommandError as e:
-                logger.error(f"Unable to delete tech-support archive on {device.name}: {e.errmsg}")
+            await device.copy(sources=filenames, destination=outdir, direction="from")
+            logger.info(f"Collected {len(filenames)} scheduled tech-support from {device.name}")
 
-        logger.info("Done collecting scheduled show-tech")
+        except EapiCommandError as e:
+            logger.error(f"Unable to collect tech-support on {device.name}: {e.errmsg}")
+        # In this case we want to catch all exceptions
+        except Exception as e:  # pylint: disable=broad-except
+            message = f"Unable to collect tech-support on device {device.name}"
+            if __DEBUG__:
+                logger.exception(message)
+            else:
+                logger.error(f"{message}: {exc_to_str(e)}")
+
+    logger.info("Connecting to devices...")
+    await inv.connect_inventory()
+    devices = inv.get_inventory(established_only=True, tags=tags).values()
+    await asyncio.gather(*(collect(device) for device in devices))
```

### Comparing `anta-0.5.0/anta/cli/get/utils.py` & `anta-0.6.0/anta/cli/get/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,37 +24,26 @@
     """Generate AUTH token from CVP using password"""
 
     # use CVP REST API to generate a token
     URL = f"https://{cvp_ip}/cvpservice/login/authenticate.do"
     payload = json.dumps({"userId": cvp_username, "password": cvp_password})
     headers = {"Content-Type": "application/json", "Accept": "application/json"}
 
-    response = requests.request(
-        "POST", URL, headers=headers, data=payload, verify=False, timeout=10
-    )
+    response = requests.request("POST", URL, headers=headers, data=payload, verify=False, timeout=10)
     return response.json()["sessionId"]
 
 
-def create_inventory(
-    inv: List[Dict[str, Any]], directory: str, container: str
-) -> None:
+def create_inventory(inv: List[Dict[str, Any]], directory: str, container: str) -> None:
     """
     create an inventory file
     """
-    i: Dict[str, Dict[str, Any]] = {
-        AntaInventory.INVENTORY_ROOT_KEY: {"hosts": []}}
-    logger.debug(f'Received {len(inv)} device(s) from CVP')
+    i: Dict[str, Dict[str, Any]] = {AntaInventory.INVENTORY_ROOT_KEY: {"hosts": []}}
+    logger.debug(f"Received {len(inv)} device(s) from CVP")
     for dev in inv:
         logger.info(f'   * adding entry for {dev["hostname"]}')
-        i[AntaInventory.INVENTORY_ROOT_KEY]["hosts"].append(
-            {
-                "host": dev["ipAddress"],
-                "name": dev['hostname'],
-                "tags": [dev['containerName'].lower()]
-            }
-        )
+        i[AntaInventory.INVENTORY_ROOT_KEY]["hosts"].append({"host": dev["ipAddress"], "name": dev["hostname"], "tags": [dev["containerName"].lower()]})
     # write the devices IP address in a file
-    inv_file = 'inventory' if container is None else f'inventory-{container}'
+    inv_file = "inventory" if container is None else f"inventory-{container}"
     out_file = f"{directory}/{inv_file}.yml"
     with open(out_file, "w", encoding="UTF-8") as out_fd:
         out_fd.write(yaml.dump(i))
-    logger.info(f'Inventory file has been created in {out_file}')
+    logger.info(f"Inventory file has been created in {out_file}")
```

### Comparing `anta-0.5.0/anta/reporter/__init__.py` & `anta-0.6.0/anta/reporter/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """
 Report management for ANTA.
 """
 
+# pylint: disable = too-few-public-methods
+
 import logging
-from typing import Any, List, Optional
+import os.path
+import pathlib
+from typing import Any, Dict, List, Optional
 
+from jinja2 import Template
 from rich.table import Table
 
 from anta import RICH_COLOR_PALETTE
 from anta.result_manager import ResultManager
 
 from .models import ColorManager
 
@@ -19,28 +24,20 @@
     """TableReport Generate a Table based on TestResult."""
 
     def __init__(self) -> None:
         """
         __init__ Class constructor
         """
         self.colors = []
-        self.colors.append(
-            ColorManager(level="success", color=RICH_COLOR_PALETTE.SUCCESS)
-        )
-        self.colors.append(
-            ColorManager(level="failure", color=RICH_COLOR_PALETTE.FAILURE)
-        )
+        self.colors.append(ColorManager(level="success", color=RICH_COLOR_PALETTE.SUCCESS))
+        self.colors.append(ColorManager(level="failure", color=RICH_COLOR_PALETTE.FAILURE))
         self.colors.append(ColorManager(level="error", color=RICH_COLOR_PALETTE.ERROR))
-        self.colors.append(
-            ColorManager(level="skipped", color=RICH_COLOR_PALETTE.SKIPPED)
-        )
-
-    def _split_list_to_txt_list(
-        self, usr_list: List[str], delimiter: Optional[str] = None
-    ) -> str:
+        self.colors.append(ColorManager(level="skipped", color=RICH_COLOR_PALETTE.SKIPPED))
+
+    def _split_list_to_txt_list(self, usr_list: List[str], delimiter: Optional[str] = None) -> str:
         """
         Split list to multi-lines string
 
         Args:
             usr_list (List[str]): List of string to concatenate
             delimiter (str, optional): A delimiter to use to start string. Defaults to None.
 
@@ -62,17 +59,15 @@
             table (Table): A rich Table instance
 
         Returns:
             Table: A rich Table instance with headers
         """
         for idx, header in enumerate(headers):
             if idx == 0:
-                table.add_column(
-                    header, justify="left", style=RICH_COLOR_PALETTE.HEADER, no_wrap=True
-                )
+                table.add_column(header, justify="left", style=RICH_COLOR_PALETTE.HEADER, no_wrap=True)
             else:
                 table.add_column(header, justify="left")
         return table
 
     def _color_result(self, status: str, output_type: str = "Text") -> Any:
         """
         Helper to implement color based on test status.
@@ -82,29 +77,16 @@
         Args:
             status (str): status value to colorized
             output_type (str, optional): Which format to output code. Defaults to 'Text'.
 
         Returns:
             Any: Can be either str or Text with Style
         """
-        if (
-            len(
-                [
-                    result
-                    for result in self.colors
-                    if str(result.level).upper() == status.upper()
-                ]
-            )
-            == 1
-        ):
-            code: ColorManager = [
-                result
-                for result in self.colors
-                if str(result.level).upper() == status.upper()
-            ][0]
+        if len([result for result in self.colors if str(result.level).upper() == status.upper()]) == 1:
+            code: ColorManager = [result for result in self.colors if str(result.level).upper() == status.upper()][0]
             return code.style_rich() if output_type == "Text" else code.string()
         return None
 
     def report_all(
         self,
         result_manager: ResultManager,
         host: Optional[str] = None,
@@ -122,34 +104,24 @@
             testcase (str, optional): A test name to search for. Defaults to None.
             title (str, optional): Title for the report. Defaults to 'All tests results'.
 
         Returns:
             Table: A fully populated rich Table
         """
         table = Table(title=title)
-        headers = ["Device IP", "Test Name", "Test Status", "Message(s)"]
+        headers = ["Device IP", "Test Name", "Test Status", "Message(s)", "Test description", "Test category"]
         table = self._build_headers(headers=headers, table=table)
 
         for result in result_manager.get_results(output_format="list"):
             # pylint: disable=R0916
-            if (
-                (host is None and testcase is None)
-                or (host is not None and str(result.name) == host)
-                or (testcase is not None and testcase == str(result.test))
-            ):
-                logger.debug(
-                    f"adding new entry in table: {result.name} / {result.test} / {result.result}"
-                )
+            if (host is None and testcase is None) or (host is not None and str(result.name) == host) or (testcase is not None and testcase == str(result.test)):
                 state = self._color_result(status=str(result.result), output_type="str")
-                message = (
-                    self._split_list_to_txt_list(result.messages)
-                    if len(result.messages) > 0
-                    else ""
-                )
-                table.add_row(str(result.name), result.test, state, message)
+                message = self._split_list_to_txt_list(result.messages) if len(result.messages) > 0 else ""
+                test_categories = ", ".join(result.test_category)
+                table.add_row(str(result.name), result.test, state, message, result.test_description, test_categories)
         return table
 
     def report_summary_tests(
         self,
         result_manager: ResultManager,
         testcase: Optional[str] = None,
         title: str = "Summary per test case",
@@ -177,31 +149,19 @@
             "# of errors",
             "List of failed or error nodes",
         ]
         table = self._build_headers(headers=headers, table=table)
         for testcase_read in result_manager.get_testcases():
             if testcase is None or str(testcase_read) == testcase:
                 results = result_manager.get_result_by_test(testcase_read)
-                nb_failure = len(
-                    [result for result in results if result.result == "failure"]
-                )
-                nb_error = len(
-                    [result for result in results if result.result == "error"]
-                )
-                list_failure = [
-                    str(result.name)
-                    for result in results
-                    if result.result in ["failure", "error"]
-                ]
-                nb_success = len(
-                    [result for result in results if result.result == "success"]
-                )
-                nb_skipped = len(
-                    [result for result in results if result.result == "skipped"]
-                )
+                nb_failure = len([result for result in results if result.result == "failure"])
+                nb_error = len([result for result in results if result.result == "error"])
+                list_failure = [str(result.name) for result in results if result.result in ["failure", "error"]]
+                nb_success = len([result for result in results if result.result == "success"])
+                nb_skipped = len([result for result in results if result.result == "skipped"])
                 table.add_row(
                     testcase_read,
                     str(nb_success),
                     str(nb_skipped),
                     str(nb_failure),
                     str(nb_error),
                     str(list_failure),
@@ -238,33 +198,64 @@
         ]
         table = self._build_headers(headers=headers, table=table)
         for host_read in result_manager.get_hosts():
             if host is None or str(host_read) == host:
                 results = result_manager.get_result_by_host(host_read)
                 logger.debug("data to use for computation")
                 logger.debug(f"{host}: {results}")
-                nb_failure = len(
-                    [result for result in results if result.result == "failure"]
-                )
-                nb_error = len(
-                    [result for result in results if result.result == "error"]
-                )
-                list_failure = [
-                    str(result.test)
-                    for result in results
-                    if result.result in ["failure", "error"]
-                ]
-                nb_success = len(
-                    [result for result in results if result.result == "success"]
-                )
-                nb_skipped = len(
-                    [result for result in results if result.result == "skipped"]
-                )
+                nb_failure = len([result for result in results if result.result == "failure"])
+                nb_error = len([result for result in results if result.result == "error"])
+                list_failure = [str(result.test) for result in results if result.result in ["failure", "error"]]
+                nb_success = len([result for result in results if result.result == "success"])
+                nb_skipped = len([result for result in results if result.result == "skipped"])
                 table.add_row(
                     str(host_read),
                     str(nb_success),
                     str(nb_skipped),
                     str(nb_failure),
                     str(nb_error),
                     str(list_failure),
                 )
         return table
+
+
+class ReportJinja:
+    """Report builder based on a Jinja2 template."""
+
+    def __init__(self, template_path: pathlib.Path) -> None:
+        if os.path.isfile(template_path):
+            self.tempalte_path = template_path
+        else:
+            raise FileNotFoundError(f"template file is not found: {template_path}")
+
+    def render(self, data: List[Dict[str, Any]], trim_blocks: bool = True, lstrip_blocks: bool = True) -> str:
+        """
+        Build a report based on a Jinja2 template
+
+        Report is built based on a J2 template provided by user.
+        Data structure sent to template is:
+
+        >>> data = ResultManager.get_results(output_format="json")
+        >>> print(data)
+        [
+            {
+                name: ...,
+                test: ...,
+                result: ...,
+                messages: [...]
+                test_category: ...,
+                test_description: ...,
+            }
+        ]
+
+        Args:
+            data (List[Dict[str, Any]]): List of results from ResultManager.get_results
+            trim_blocks (bool, optional): enable trim_blocks for J2 rendering. Defaults to True.
+            lstrip_blocks (bool, optional): enable lstrip_blocks for J2 rendering. Defaults to True.
+
+        Returns:
+            str: rendered template
+        """
+        with open(self.tempalte_path, encoding="utf-8") as file_:
+            template = Template(file_.read(), trim_blocks=trim_blocks, lstrip_blocks=lstrip_blocks)
+
+        return template.render({"data": data})
```

### Comparing `anta-0.5.0/anta/reporter/models.py` & `anta-0.6.0/anta/reporter/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from pydantic import BaseModel, validator
 from rich.text import Text
 
 from ..result_manager.models import RESULT_OPTIONS
 
 
 class ColorManager(BaseModel):
-    """Color mangement for status report.
+    """Color management for status report.
 
     Attributes:
         level (str): Test result value.
         color (str): Associated color.
     """
+
     level: str
     color: str
 
-    @validator('level', allow_reuse=True)
+    @validator("level", allow_reuse=True)
     def name_must_be_in(cls, v: str) -> str:
         """
         Status validator
 
         Validate status is a supported one
 
         Args:
@@ -29,15 +30,15 @@
         Raises:
             ValueError: If level is unsupported
 
         Returns:
             str: level value
         """
         if v not in RESULT_OPTIONS:
-            raise ValueError(f'must be one of {RESULT_OPTIONS}')
+            raise ValueError(f"must be one of {RESULT_OPTIONS}")
         return v
 
     def style_rich(self) -> Text:
         """
         Build a rich Text syntax with color
 
         Returns:
@@ -48,8 +49,8 @@
     def string(self) -> str:
         """
         Build an str with color code
 
         Returns:
             str: String with level and its associated color
         """
-        return f'[{self.color}]{self.level}'
+        return f"[{self.color}]{self.level}"
```

### Comparing `anta-0.5.0/anta/result_manager/__init__.py` & `anta-0.6.0/anta/result_manager/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,101 +2,143 @@
 Result Manager Module for ANTA.
 """
 
 import json
 import logging
 from typing import Any, List
 
-from anta.result_manager.models import ListResult, TestResult
-from anta.tools import pydantic_to_dict
+from anta.result_manager.models import RESULT_OPTIONS, ListResult, TestResult
+from anta.tools.pydantic import pydantic_to_dict
 
 logger = logging.getLogger(__name__)
 
 
 class ResultManager:
     """
     Helper to manage Test Results and generate reports.
 
     Examples:
 
         Create Inventory:
 
-            inventory_anta = AntaInventory(
+            inventory_anta = AntaInventory.parse(
                 inventory_file='examples/inventory.yml',
                 username='ansible',
                 password='ansible',
-                timeout=0.5,
-                auto_connect=True
+                timeout=0.5
             )
 
         Create Result Manager:
 
             manager = ResultManager()
 
         Run tests for all connected devices:
 
             for device in inventory_anta.get_inventory():
                 manager.add_test_result(
-                    verify_eos_version(
-                        device=device, versions=['4.28.0F']
-                    )
+                    VerifyNTP(device=device).test()
                 )
                 manager.add_test_result(
-                    verify_uptime(
-                        device=device, minimum=1
-                    )
+                    VerifyEOSVersion(device=device).test(version='4.28.3M')
                 )
 
         Print result in native format:
 
             manager.get_results()
             [
                 TestResult(
                     host=IPv4Address('192.168.0.10'),
-                    test='verify_eos_version',
+                    test='VerifyNTP',
                     result='failure',
-                    message="device is running version 4.27.3F-26379303.4273F (engineering build) and test expect ['4.28.0F']"
+                    message="device is not running NTP correctly"
                 ),
                 TestResult(
                     host=IPv4Address('192.168.0.10'),
-                    test='verify_eos_version',
+                    test='VerifyEOSVersion',
                     result='success',
                     message=None
                 ),
             ]
     """
 
     def __init__(self) -> None:
-        """ Class constructor."""
-        logger.debug('Instantiate result-manager')
+        """
+        Class constructor.
+
+        The status of the class is initialized to "unset"
+
+        Then when adding a test with a status that is NOT 'error' the following
+        table shows the updated status:
+
+        | Current Status |         Added test Status       | Updated Status |
+        | -------------- | ------------------------------- | -------------- |
+        |      unset     |              Any                |       Any      |
+        |     skipped    |         unset, skipped          |     skipped    |
+        |     skipped    |            success              |     success    |
+        |     skipped    |            failure              |     failure    |
+        |     success    |     unset, skipped, success     |     success    |
+        |     success    |            failure              |     failure    |
+        |     failure    | unset, skipped success, failure |     failure    |
+
+        If the status of the added test is error, the status is untouched and the
+        error_status is set to True.
+        """
+        logger.debug("Instantiate result-manager")
         self._result_entries = ListResult()
+        # Initialize status
+        self.status = "unset"
+        self.error_status = False
 
     def __len__(self) -> int:
         """
         Implement __len__ method to count number of results.
         """
         return len(self._result_entries)
 
+    def __update_status(self, test_status: str) -> None:
+        """
+        Update ResultManager status based on the table above.
+        """
+        if test_status not in RESULT_OPTIONS:
+            raise ValueError("{test_status} is not a valid result option")
+        if test_status == "error":
+            self.error_status = True
+            return
+
+        if self.status == "unset":
+            self.status = test_status
+        elif self.status == "skipped" and test_status in {"success", "failure"}:
+            self.status = test_status
+        elif self.status == "success" and test_status == "failure":
+            self.status = "failure"
+
     def add_test_result(self, entry: TestResult) -> None:
         """Add a result to the list
 
         Args:
             entry (TestResult): TestResult data to add to the report
         """
-        logger.info(f'add new test result to manager: {entry}')
+        logger.debug(entry)
         self._result_entries.append(entry)
+        self.__update_status(entry.result)
 
     def add_test_results(self, entries: List[TestResult]) -> None:
         """Add a list of results to the list
 
         Args:
             entries (List[TestResult]): list of TestResult data to add to the report
         """
-        logger.info(f'add new list of results to manager: {[str(r) for r in entries]}')
-        self._result_entries.extend(entries)
+        for e in entries:
+            self.add_test_result(e)
+
+    def get_status(self, ignore_error: bool = False) -> str:
+        """
+        Returns the current status including error_status if ignore_error is False
+        """
+        return "error" if self.error_status and not ignore_error else self.status
 
     def get_results(self, output_format: str = "native") -> Any:
         """
         Expose list of all test results in different format
 
         Support multiple format:
           - native: ListResults format
@@ -105,16 +147,15 @@
 
         Args:
             output_format (str, optional): format selector. Can be either native/list/json. Defaults to 'native'.
 
         Returns:
             any: List of results.
         """
-        logger.info(f'retrieve list of result using output_format {output_format}')
-        if output_format == 'list':
+        if output_format == "list":
             return list(self._result_entries)
 
         if output_format == "json":
             return json.dumps(pydantic_to_dict(self._result_entries), indent=4)
 
         # Default return for native format.
         return self._result_entries
@@ -126,22 +167,16 @@
         Args:
             test_name (str): Test name to use to filter results
             output_format (str, optional): format selector. Can be either native/list. Defaults to 'native'.
 
         Returns:
             list[TestResult]: List of results related to the test.
         """
-        logger.info(
-            f'retrieve list of result using output_format {output_format} for test {test_name}')
         if output_format == "list":
-            return [
-                result
-                for result in self._result_entries
-                if str(result.test) == test_name
-            ]
+            return [result for result in self._result_entries if str(result.test) == test_name]
 
         result_manager_filtered = ListResult()
         for result in self._result_entries:
             if result.test == test_name:
                 result_manager_filtered.append(result)
         return result_manager_filtered
 
@@ -152,49 +187,41 @@
         Args:
             host_ip (str): IP Address of the host to use to filter results.
             output_format (str, optional): format selector. Can be either native/list. Defaults to 'native'.
 
         Returns:
             Any: List of results related to the host.
         """
-        logger.info(
-            f'retrieve list of result using output_format {output_format} for host {host_ip}')
         if output_format == "list":
-            return [
-                result for result in self._result_entries if str(result.name) == host_ip
-            ]
+            return [result for result in self._result_entries if str(result.name) == host_ip]
 
         result_manager_filtered = ListResult()
         for result in self._result_entries:
             if str(result.name) == host_ip:
                 result_manager_filtered.append(result)
         return result_manager_filtered
 
     def get_testcases(self) -> List[str]:
         """
         Get list of name of all test cases in current manager.
 
         Returns:
             List[str]: List of names for all tests.
         """
-        logger.info('build list of testcases registered in result-manager')
         result_list = []
         for testcase in self._result_entries:
             if str(testcase.test) not in result_list:
                 result_list.append(str(testcase.test))
-        logger.debug(f'list of tests name: {result_list}')
         return result_list
 
     def get_hosts(self) -> List[str]:
         """
         Get list of IP addresses in current manager.
 
         Returns:
             List[str]: List of IP addresses.
         """
-        logger.info('build list of host ip registered in result-manager')
         result_list = []
         for testcase in self._result_entries:
             if str(testcase.name) not in result_list:
                 result_list.append(str(testcase.name))
-        logger.debug(f'list of tests name: {result_list}')
         return result_list
```

### Comparing `anta-0.5.0/anta/result_manager/models.py` & `anta-0.6.0/anta/result_manager/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 """Models related to anta.result_manager module."""
 
 from typing import Iterator, List
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, RootModel, validator
 
-RESULT_OPTIONS = ['unset', 'success', 'failure', 'error', 'skipped']
+RESULT_OPTIONS = ["unset", "success", "failure", "error", "skipped"]
 
 
 class TestResult(BaseModel):
     """
-    Describe result of a test from a single device.
+    Describe the result of a test from a single device.
 
     Attributes:
         name (str): Device name where the test has run.
         test (str): Test name runs on the device.
-        results (str): Result of the test. Can be one of unset / failure / success.
-        message (str, optional): Message to report after the test.
+        test_category (List[str]): List of test categories the test belongs to.
+        test_description (str): Test description.
+        results (str): Result of the test. Can be one of ["unset", "success", "failure", "error", "skipped"].
+        message (str, optional): Message to report after the test if any.
     """
+
     name: str
     test: str
-    result: str = 'unset'
+    test_category: List[str]
+    test_description: str
+    result: str = "unset"
     messages: List[str] = []
 
-    @validator('result', allow_reuse=True)
+    @classmethod
+    @validator("result", allow_reuse=True)
     def name_must_be_in(cls, v: str) -> str:
         """
         Status validator
 
         Validate status is a supported one
 
         Args:
@@ -35,105 +41,112 @@
         Raises:
             ValueError: If status is unsupported
 
         Returns:
             str: status value
         """
         if v not in RESULT_OPTIONS:
-            raise ValueError(f'must be one of {RESULT_OPTIONS}')
+            raise ValueError(f"must be one of {RESULT_OPTIONS}")
         return v
 
-    def is_success(self, message: str = '') -> bool:
+    def is_success(self, message: str = "") -> bool:
         """
         Helper to set status to success
 
         Args:
             message (str): Optional message related to the test
 
         Returns:
             bool: Always true
         """
-        return self._set_status('success', message)
+        return self._set_status("success", message)
 
-    def is_failure(self, message: str = '') -> bool:
+    def is_failure(self, message: str = "") -> bool:
         """
         Helper to set status to failure
 
         Args:
             message (str): Optional message related to the test
 
         Returns:
             bool: Always true
         """
-        return self._set_status('failure', message)
+        return self._set_status("failure", message)
 
-    def is_skipped(self, message: str = '') -> bool:
+    def is_skipped(self, message: str = "") -> bool:
         """
         Helper to set status to skipped
 
         Args:
             message (str): Optional message related to the test
 
         Returns:
             bool: Always true
         """
-        return self._set_status('skipped', message)
+        return self._set_status("skipped", message)
 
-    def is_error(self, message: str = '') -> bool:
+    def is_error(self, message: str = "") -> bool:
         """
         Helper to set status to error
 
         Args:
             message (str): Optional message related to the test
 
         Returns:
             bool: Always true
         """
-        return self._set_status('error', message)
+        return self._set_status("error", message)
 
-    def _set_status(self, status: str, message: str = '') -> bool:
+    def _set_status(self, status: str, message: str = "") -> bool:
         """
         Set status and insert optional message
 
         Args:
             status (str): status of the test
             message (str): optional message
 
         Returns:
             bool: Always true
         """
         self.result = status
-        if message != '':
+        if message != "":
             self.messages.append(message)
         return True
 
+    def __str__(self) -> str:
+        """
+        Returns a human readable string of this TestResult
+        """
+        return f"Test {self.test} on device {self.name} has result {self.result}"
+
 
-class ListResult(BaseModel):
+class ListResult(RootModel[List[TestResult]]):
     """
     List result for all tests on all devices.
 
     Attributes:
         __root__ (List[TestResult]): A list of TestResult objects.
     """
-    # pylint: disable=R0801
 
-    __root__: List[TestResult] = []
+    root: List[TestResult] = []
 
     def extend(self, values: List[TestResult]) -> None:
         """Add support for extend method."""
-        self.__root__.extend(values)
+        self.root.extend(values)
 
     def append(self, value: TestResult) -> None:
         """Add support for append method."""
-        self.__root__.append(value)
+        self.root.append(value)
 
-    def __iter__(self) -> Iterator[TestResult]:
+    def __iter__(self) -> Iterator[TestResult]:  # type: ignore
         """Use custom iter method."""
-        return iter(self.__root__)
+        # TODO - mypy is not happy because we overwrite BaseModel.__iter__
+        # return type and are breaking Liskov Substitution Principle.
+        return iter(self.root)
 
     def __getitem__(self, item: int) -> TestResult:
         """Use custom getitem method."""
-        return self.__root__[item]
+        return self.root[item]
 
     def __len__(self) -> int:
         """Support for length of __root__"""
-        return len(self.__root__)
+        return len(self.root)
```

### Comparing `anta-0.5.0/anta/tests/hardware.py` & `anta-0.6.0/anta/tests/hardware.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,247 +1,215 @@
 """
 Test functions related to the hardware or environement
 """
-import logging
+from __future__ import annotations
+
 from typing import List, Optional
 
 from anta.decorators import skip_on_platforms
-from anta.inventory.models import InventoryDevice
-from anta.result_manager.models import TestResult
-from anta.tests import anta_test
-
-logger = logging.getLogger(__name__)
+from anta.models import AntaCommand, AntaTest
 
 
-@skip_on_platforms(["cEOSLab", "vEOS-lab"])
-@anta_test
-async def verify_transceivers_manufacturers(
-    device: InventoryDevice,
-    result: TestResult,
-    manufacturers: Optional[List[str]] = None,
-) -> TestResult:
+class VerifyTransceiversManufacturers(AntaTest):
     """
-    Verifies the device is only using transceivers from supported manufacturers.
-
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
-        manufacturers (list): List of allowed transceivers manufacturers.
-
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "skipped" if the test was not executed because no manufacturers were given
-        * result = "success" if the device is only using transceivers from supported manufacturers.
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
-
+    Verifies Manufacturers of all Transceivers.
     """
 
-    if not manufacturers:
-        result.is_skipped(
-            "verify_transceivers_manufacturers was not run as no "
-            "manufacturers were given"
-        )
-        return result
-
-    response = await device.session.cli(command="show inventory", ofmt="json")
-    logger.debug(f"query result is: {response}")
-
-    wrong_manufacturers = {
-        interface: value["mfgName"]
-        for interface, value in response["xcvrSlots"].items()
-        if value["mfgName"] not in manufacturers
-    }
-
-    if not wrong_manufacturers:
-        result.is_success()
-    else:
-        result.is_failure(
-            "The following interfaces have transceivers from unauthorized manufacturers"
-        )
-        result.messages.append(str(wrong_manufacturers))
-
-    return result
-
-
-@skip_on_platforms(["cEOSLab", "vEOS-lab"])
-@anta_test
-async def verify_system_temperature(
-    device: InventoryDevice, result: TestResult
-) -> TestResult:
-
-    """
-    Verifies the device temperature is currently OK
-    and the device did not report any temperature alarm in the past.
-
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
-
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "success" if the device temperature is OK.
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
-
-    """
-    response = await device.session.cli(
-        command="show system environment temperature", ofmt="json"
-    )
-    logger.debug(f"query result is: {response}")
-
-    if response["systemStatus"] == "temperatureOk":
-        result.is_success()
-    else:
-        result.is_failure(
-            f"Device temperature is not OK, systemStatus: {response['systemStatus'] }"
-        )
-
-    return result
-
+    name = "VerifyTransceiversManufacturers"
+    description = ""
+    categories = ["hardware"]
+    commands = [AntaCommand(command="show inventory", ofmt="json")]
+
+    @skip_on_platforms(["cEOSLab", "vEOS-lab"])
+    @AntaTest.anta_test
+    def test(self, manufacturers: Optional[List[str]] = None) -> None:
+        """
+        Run VerifyTransceiversManufacturers validation
+
+        Args:
+            manufacturers: List of allowed transceivers manufacturers.
+        """
+        if not manufacturers:
+            self.result.is_skipped(f"{self.__class__.name} was not run as no manufacturers were given")
+        else:
+            command_output = self.instance_commands[0].json_output
+            wrong_manufacturers = {interface: value["mfgName"] for interface, value in command_output["xcvrSlots"].items() if value["mfgName"] not in manufacturers}
+            if not wrong_manufacturers:
+                self.result.is_success()
+            else:
+                self.result.is_failure("The following interfaces have transceivers from unauthorized manufacturers")
+                self.result.messages.append(str(wrong_manufacturers))
+
+
+class VerifyTemperature(AntaTest):
+    """
+    Verifies device temparture is currently OK (temperatureOK).
+    """
+
+    name = "VerifyTemperature"
+    description = "Verifies device temparture is currently OK (temperatureOK)"
+    categories = ["hardware"]
+    commands = [AntaCommand(command="show system environment temperature", ofmt="json")]
+
+    @skip_on_platforms(["cEOSLab", "vEOS-lab"])
+    @AntaTest.anta_test
+    def test(self) -> None:
+        """Run VerifyTemperature validation"""
+        command_output = self.instance_commands[0].json_output
+        temperature_status = command_output["systemStatus"] if "systemStatus" in command_output.keys() else ""
+        if temperature_status == "temperatureOk":
+            self.result.is_success()
+        else:
+            self.result.is_failure(f"Device temperature is not OK, systemStatus: {temperature_status }")
+
+
+class VerifyTransceiversTemperature(AntaTest):
+    """
+    Verifies Transceivers temperature is currently OK.
+    """
+
+    name = "VerifyTransceiversTemperature"
+    description = "Verifies Transceivers temperature is currently OK"
+    categories = ["hardware"]
+    commands = [AntaCommand(command="show system environment temperature transceiver", ofmt="json")]
+
+    @skip_on_platforms(["cEOSLab", "vEOS-lab"])
+    @AntaTest.anta_test
+    def test(self) -> None:
+        """Run VerifyTransceiversTemperature validation"""
+        command_output = self.instance_commands[0].json_output
+        sensors = command_output["tempSensors"] if "tempSensors" in command_output.keys() else ""
+        wrong_sensors = {
+            sensor["name"]: {
+                "hwStatus": sensor["hwStatus"],
+                "alertCount": sensor["alertCount"],
+            }
+            for sensor in sensors
+            if sensor["hwStatus"] != "ok" or sensor["alertCount"] != 0
+        }
+        if not wrong_sensors:
+            self.result.is_success()
+        else:
+            self.result.is_failure("The following sensors do not have the correct temperature or had alarms in the past:")
+            self.result.messages.append(str(wrong_sensors))
 
-@skip_on_platforms(["cEOSLab", "vEOS-lab"])
-@anta_test
-async def verify_transceiver_temperature(
-    device: InventoryDevice, result: TestResult
-) -> TestResult:
 
+class VerifyEnvironmentSystemCooling(AntaTest):
     """
-    Verifies the transceivers temperature is currently OK
-    and the device did not report any alarm in the past for its transceivers temperature.
-
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
-
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "success" if the device transceivers temperature of the device is currently OK
-                             AND the device did not report any alarm in the past for its transceivers temperature.
-        * result = "failure" otherwise,
-        * result = "error" if any exception is caught
-
+    Verifies the System Cooling is ok.
     """
-    response = await device.session.cli(
-        command="show system environment temperature transceiver", ofmt="json"
-    )
-    logger.debug(f"query result is: {response}")
 
-    # Get the list of sensors
-    sensors = response["tempSensors"]
+    name = "VerifyEnvironmentSystemCooling"
+    description = "Verifies the fans status is OK for fans"
+    categories = ["hardware"]
+    commands = [AntaCommand(command="show system environment cooling", ofmt="json")]
 
-    wrong_sensors = {
-        sensor["name"]: {
-            "hwStatus": sensor["hwStatus"],
-            "alertCount": sensor["alertCount"],
-        }
-        for sensor in sensors
-        if sensor["hwStatus"] != "ok" or sensor["alertCount"] != 0
-    }
-    if not wrong_sensors:
-        result.is_success()
-    else:
-        result.is_failure(
-            "The following sensors do not have the correct temperature or had alarms in the past:"
-        )
-        result.messages.append(str(wrong_sensors))
+    @skip_on_platforms(["cEOSLab", "vEOS-lab"])
+    @AntaTest.anta_test
+    def test(self) -> None:
+        """Run VerifyEnvironmentCooling validation"""
 
-    return result
+        command_output = self.instance_commands[0].json_output
+        sys_status = command_output["systemStatus"] if "systemStatus" in command_output.keys() else ""
 
+        self.result.is_success()
+        if sys_status != "coolingOk":
+            self.result.is_failure(f"Device System cooling is not OK: {sys_status}")
 
-@skip_on_platforms(["cEOSLab", "vEOS-lab"])
-@anta_test
-async def verify_environment_cooling(
-    device: InventoryDevice, result: TestResult
-) -> TestResult:
 
+class VerifyEnvironmentCooling(AntaTest):
     """
-    Verifies the fans status is OK.
-
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
-
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "success" if the fans status is OK.
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
+    Verifies the fans status is in the accepted states list.
 
+    Default accepted states list is ['ok']
     """
-    response = await device.session.cli(command="show system environment cooling", ofmt="json")
-    logger.debug(f"query result is: {response}")
 
-    if response["systemStatus"] == "coolingOk":
-        result.is_success()
-    else:
-        result.is_failure(
-            f"Device cooling is not OK, systemStatus: {response['systemStatus'] }"
-        )
+    name = "VerifyEnvironmentCooling"
+    description = "Verifies the fans status is OK for fans"
+    categories = ["hardware"]
+    commands = [AntaCommand(command="show system environment cooling", ofmt="json")]
 
-    return result
+    @skip_on_platforms(["cEOSLab", "vEOS-lab"])
+    @AntaTest.anta_test
+    def test(self, accepted_states: Optional[List[str]] = None) -> None:
+        """
+        Run VerifyEnvironmentCooling validation
 
+        Args:
+            accepted_states: Accepted states list for fan status
+        """
+        if accepted_states is None:
+            accepted_states = ["ok"]
 
-@skip_on_platforms(["cEOSLab", "vEOS-lab"])
-@anta_test
-async def verify_environment_power(device: InventoryDevice, result: TestResult) -> TestResult:
-
-    """
-    Verifies the power supplies status is OK.
+        command_output = self.instance_commands[0].json_output
+        self.result.is_success()
+        # First go through power supplies fans
+        for power_supply in command_output.get("powerSupplySlots", []):
+            for fan in power_supply.get("fans", []):
+                if (state := fan["status"]) not in accepted_states:
+                    if self.result.result == "success":
+                        self.result.is_failure(f"Some fans state are not in the accepted list: {accepted_states}.")
+                    self.result.is_failure(f"Fan {fan['label']} on PowerSupply {power_supply['label']} has state '{state}'.")
+        # Then go through Fan Trays
+        for fan_tray in command_output.get("fanTraySlots", []):
+            for fan in fan_tray.get("fans", []):
+                if (state := fan["status"]) not in accepted_states:
+                    if self.result.result == "success":
+                        self.result.is_failure(f"Some fans state are not in the accepted list: {accepted_states}.")
+                    self.result.is_failure(f"Fan {fan['label']} on Fan Tray {fan_tray['label']} has state '{state}'.")
 
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
-
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "success" if the power supplies status is OK.
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
 
+class VerifyEnvironmentPower(AntaTest):
     """
-    response = await device.session.cli(command="show system environment power", ofmt="json")
-    logger.debug(f"query result is: {response}")
-
-    wrong_power_supplies = {
-        powersupply: {"state": value["state"]}
-        for powersupply, value in response["powerSupplies"].items()
-        if value["state"] != "ok"
-    }
-    if not wrong_power_supplies:
-        result.is_success()
-    else:
-        result.is_failure("The following power suppliers are not ok:")
-        result.messages.append(str(wrong_power_supplies))
-
-    return result
-
-
-@skip_on_platforms(["cEOSLab", "vEOS-lab"])
-@anta_test
-async def verify_adverse_drops(device: InventoryDevice, result: TestResult) -> TestResult:
+    Verifies the power supplies status is in the accepted states list
 
+    The default accepted states list is ['ok']
     """
-    Verifies there is no adverse drops on DCS-7280E and DCS-7500E switches.
 
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
+    name = "VerifyEnvironmentPower"
+    description = "Verifies the power supplies status is OK"
+    categories = ["hardware"]
+    commands = [AntaCommand(command="show system environment power", ofmt="json")]
 
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "success" if the device (DCS-7280E and DCS-7500E) doesnt reports adverse drops.
-        * result = "failure" if the device (DCS-7280E and DCS-7500E) report adverse drops.
-        * result = "error" if any exception is caught
+    @skip_on_platforms(["cEOSLab", "vEOS-lab"])
+    @AntaTest.anta_test
+    def test(self, accepted_states: Optional[List[str]] = None) -> None:
+        """
+        Run VerifyEnvironmentPower validation
 
-    """
-    response = await device.session.cli(command="show hardware counter drop", ofmt="json")
-    logger.debug(f"query result is: {response}")
-
-    if response["totalAdverseDrops"] == 0:
-        result.is_success()
-    else:
-        result.is_failure(
-            f"Device TotalAdverseDrops counter is {response['totalAdverseDrops']}."
-        )
-
-    return result
+        Args:
+            accepted_states: Accepted states list for power supplies
+        """
+        if accepted_states is None:
+            accepted_states = ["ok"]
+        command_output = self.instance_commands[0].json_output
+        power_supplies = command_output["powerSupplies"] if "powerSupplies" in command_output.keys() else "{}"
+        wrong_power_supplies = {
+            powersupply: {"state": value["state"]} for powersupply, value in dict(power_supplies).items() if value["state"] not in accepted_states
+        }
+        if not wrong_power_supplies:
+            self.result.is_success()
+        else:
+            self.result.is_failure(f"The following power supplies states are not in the accepted_states list {accepted_states}")
+            self.result.messages.append(str(wrong_power_supplies))
+
+
+class VerifyAdverseDrops(AntaTest):
+    """
+    Verifies there is no adverse drops on DCS7280E and DCS7500E.
+    """
+
+    name = "VerifyAdverseDrops"
+    description = "Verifies there is no adverse drops on DCS7280E and DCS7500E"
+    categories = ["hardware"]
+    commands = [AntaCommand(command="show hardware counter drop", ofmt="json")]
+
+    @skip_on_platforms(["cEOSLab", "vEOS-lab"])
+    @AntaTest.anta_test
+    def test(self) -> None:
+        """Run VerifyAdverseDrops validation"""
+        command_output = self.instance_commands[0].json_output
+        total_adverse_drop = command_output["totalAdverseDrops"] if "totalAdverseDrops" in command_output.keys() else ""
+        if total_adverse_drop == 0:
+            self.result.is_success()
+        else:
+            self.result.is_failure(f"Device TotalAdverseDrops counter is {total_adverse_drop}")
```

### Comparing `anta-0.5.0/anta/tests/routing/bgp.py` & `anta-0.6.0/anta/tests/routing/bgp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,21 @@
 """
 BGP test functions
 """
-import logging
-from typing import Any, Dict
+
+from typing import Any, Dict, Optional
 
 from anta.decorators import check_bgp_family_enable
-from anta.inventory.models import InventoryDevice
-from anta.result_manager.models import TestResult
-from anta.tests import anta_test
-
-logger = logging.getLogger(__name__)
+from anta.models import AntaCommand, AntaTemplate, AntaTest
 
 
-@anta_test
-@check_bgp_family_enable("ipv4")
-async def verify_bgp_ipv4_unicast_state(
-    device: InventoryDevice, result: TestResult
-) -> TestResult:
+def _check_bgp_vrfs(bgp_vrfs: Dict[str, Any]) -> Dict[str, Any]:
     """
-    Verifies all IPv4 unicast BGP sessions are established (for all VRF)
-    and all BGP messages queues for these sessions are empty (for all VRF).
-
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
-
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "skipped" if no BGP vrf are returned by the device
-        * result = "success" if all IPv4 unicast BGP sessions are established (for all VRF)
-                             and all BGP messages queues for these sessions are empty (for all VRF).
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
+    TODO
     """
-    response = await device.session.cli(
-        command="show bgp ipv4 unicast summary vrf all", ofmt="json"
-    )
-    logger.debug(f"query result is: {response}")
-
-    bgp_vrfs = response["vrfs"]
-
     state_issue: Dict[str, Any] = {}
     for vrf in bgp_vrfs:
         for peer in bgp_vrfs[vrf]["peers"]:
             if (
                 (bgp_vrfs[vrf]["peers"][peer]["peerState"] != "Established")
                 or (bgp_vrfs[vrf]["peers"][peer]["inMsgQueue"] != 0)
                 or (bgp_vrfs[vrf]["peers"][peer]["outMsgQueue"] != 0)
@@ -55,307 +27,272 @@
                             "peerState": bgp_vrfs[vrf]["peers"][peer]["peerState"],
                             "inMsgQueue": bgp_vrfs[vrf]["peers"][peer]["inMsgQueue"],
                             "outMsgQueue": bgp_vrfs[vrf]["peers"][peer]["outMsgQueue"],
                         }
                     }
                 )
 
-    if not state_issue:
-        result.is_success()
-    else:
-        result.is_failure(f"Some IPv4 Unicast BGP Peer are not up: {state_issue}")
-
-    return result
+    return state_issue
 
 
-@anta_test
-@check_bgp_family_enable("ipv4")
-async def verify_bgp_ipv4_unicast_count(
-    device: InventoryDevice, result: TestResult, number: int, vrf: str = "default"
-) -> TestResult:
+class VerifyBGPIPv4UnicastState(AntaTest):
+    """
+    Verifies all IPv4 unicast BGP sessions are established (for all VRF)
+    and all BGP messages queues for these sessions are empty (for all VRF).
+
+    * self.result = "skipped" if no BGP vrf are returned by the device
+    * self.result = "success" if all IPv4 unicast BGP sessions are established (for all VRF)
+                         and all BGP messages queues for these sessions are empty (for all VRF).
+    * self.result = "failure" otherwise.
+    """
+
+    name = "VerifyBGPIPv4UnicastState"
+    description = "Verifies all IPv4 unicast BGP sessions are established (for all VRF) and all BGP messages queues for these sessions are empty (for all VRF)."
+    categories = ["routing", "bgp"]
+    commands = [AntaCommand(command="show bgp ipv4 unicast summary vrf all")]
+
+    @check_bgp_family_enable("ipv4")
+    @AntaTest.anta_test
+    def test(self) -> None:
+        """Run VerifyBGPIPv4UnicastState validation"""
+
+        command_output = self.instance_commands[0].json_output
+        state_issue = _check_bgp_vrfs(command_output["vrfs"])
+
+        if not state_issue:
+            self.result.is_success()
+        else:
+            self.result.is_failure(f"Some IPv4 Unicast BGP Peer are not up: {state_issue}")
+
+
+class VerifyBGPIPv4UnicastCount(AntaTest):
     """
     Verifies all IPv4 unicast BGP sessions are established
     and all BGP messages queues for these sessions are empty
     and the actual number of BGP IPv4 unicast neighbors is the one we expect.
 
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
-        number (int): Expected number of BGP IPv4 unicast neighbors
-        vrf(str): VRF to verify. default is "default".
-
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "skipped" if the `number` or `vrf` parameter is missing
-        * result = "success" if all IPv4 unicast BGP sessions are established
-                             and if all BGP messages queues for these sessions are empty
-                             and if the actual number of BGP IPv4 unicast neighbors is equal to `number.
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
-    """
-    if not number or not vrf:
-        result.is_skipped(
-            "verify_bgp_ipv4_unicast_count could not run because number of vrf was not supplied"
-        )
-        return result
+    * self.result = "skipped" if the `number` or `vrf` parameter is missing
+    * self.result = "success" if all IPv4 unicast BGP sessions are established
+                         and if all BGP messages queues for these sessions are empty
+                         and if the actual number of BGP IPv4 unicast neighbors is equal to `number.
+    * self.result = "failure" otherwise.
+    """
 
-    response = await device.session.cli(
-        command=f"show bgp ipv4 unicast summary vrf {vrf}", ofmt="json"
+    name = "VerifyBGPIPv4UnicastCount"
+    description = (
+        "Verifies all IPv4 unicast BGP sessions are established and all their BGP messages queues are empty and "
+        " the actual number of BGP IPv4 unicast neighbors is the one we expect."
     )
-    logger.debug(f"query result is: {response}")
+    categories = ["routing", "bgp"]
+    template = AntaTemplate(template="show bgp ipv4 unicast summary vrf {vrf}")
+
+    @check_bgp_family_enable("ipv4")
+    @AntaTest.anta_test
+    def test(self, number: Optional[int] = None) -> None:
+        """
+        Run VerifyBGPIPv4UnicastCount validation
+
+        Args:
+            number: The expected number of BGP IPv4 unicast neighbors.
+            vrf: VRF to verify (template parameter)
+        """
+
+        if not number:
+            self.result.is_skipped("VerifyBGPIPv4UnicastCount could not run because number was not supplied")
+            return
+
+        self.result.is_success()
+
+        for command in self.instance_commands:
+            if command.params and "vrf" in command.params:
+                vrf = command.params["vrf"]
 
-    bgp_vrfs = response["vrfs"]
+            peers = command.json_output["vrfs"][vrf]["peers"]
+            state_issue = _check_bgp_vrfs(command.json_output["vrfs"])
 
-    peer_state_issue = {}
-    peer_number = len(bgp_vrfs[vrf]["peers"])
+            if len(peers) != number:
+                self.result.is_failure(f"Expecting {number} BGP peer in vrf {vrf} and got {len(peers)}")
+            if state_issue:
+                self.result.is_failure(f"The following IPv4 peers are not established: {state_issue}")
 
-    for peer in bgp_vrfs[vrf]["peers"]:
-        if (
-            (bgp_vrfs[vrf]["peers"][peer]["peerState"] != "Established")
-            or (bgp_vrfs[vrf]["peers"][peer]["inMsgQueue"] != 0)
-            or (bgp_vrfs[vrf]["peers"][peer]["outMsgQueue"] != 0)
-        ):
-            peer_state_issue[peer] = {
-                "peerState": bgp_vrfs[vrf]["peers"][peer]["peerState"],
-                "inMsgQueue": bgp_vrfs[vrf]["peers"][peer]["inMsgQueue"],
-                "outMsgQueue": bgp_vrfs[vrf]["peers"][peer]["outMsgQueue"],
-            }
-
-    if peer_number == number:
-        result.is_success()
-    else:
-        result.is_failure()
-        if peer_number != number:
-            result.is_failure(
-                f"Expecting {number} BGP peer in vrf {vrf} and got {peer_number}"
-            )
-
-    return result
-
-
-@anta_test
-@check_bgp_family_enable("ipv6")
-async def verify_bgp_ipv6_unicast_state(
-    device: InventoryDevice, result: TestResult
-) -> TestResult:
+
+class VerifyBGPIPv6UnicastState(AntaTest):
     """
     Verifies all IPv6 unicast BGP sessions are established (for all VRF)
     and all BGP messages queues for these sessions are empty (for all VRF).
 
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
-
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "skipped" if no BGP vrf are returned by the device
-        * result = "success" if all IPv6 unicast BGP sessions are established (for all VRF)
-                             and all BGP messages queues for these sessions are empty (for all VRF).
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
+    * self.result = "skipped" if no BGP vrf are returned by the device
+    * self.result = "success" if all IPv6 unicast BGP sessions are established (for all VRF)
+                         and all BGP messages queues for these sessions are empty (for all VRF).
+    * self.result = "failure" otherwise.
     """
-    response = await device.session.cli(
-        command="show bgp ipv6 unicast summary vrf all", ofmt="json"
-    )
 
-    logger.debug(f"query result is: {response}")
-    bgp_vrfs = response["vrfs"]
+    name = "VerifyBGPIPv6UnicastState"
+    description = "Verifies all IPv6 unicast BGP sessions are established (for all VRF) and all BGP messages queues for these sessions are empty (for all VRF)."
+    categories = ["routing", "bgp"]
+    commands = [AntaCommand(command="show bgp ipv6 unicast summary vrf all")]
 
-    state_issue: Dict[str, Any] = {}
-    for vrf in bgp_vrfs:
-        for peer in bgp_vrfs[vrf]["peers"]:
-            if (
-                (bgp_vrfs[vrf]["peers"][peer]["peerState"] != "Established")
-                or (bgp_vrfs[vrf]["peers"][peer]["inMsgQueue"] != 0)
-                or (bgp_vrfs[vrf]["peers"][peer]["outMsgQueue"] != 0)
-            ):
-                vrf_dict = state_issue.setdefault(vrf, {})
-                vrf_dict.update(
-                    {
-                        peer: {
-                            "peerState": bgp_vrfs[vrf]["peers"][peer]["peerState"],
-                            "inMsgQueue": bgp_vrfs[vrf]["peers"][peer]["inMsgQueue"],
-                            "outMsgQueue": bgp_vrfs[vrf]["peers"][peer]["outMsgQueue"],
-                        }
-                    }
-                )
+    @check_bgp_family_enable("ipv6")
+    @AntaTest.anta_test
+    def test(self) -> None:
+        """Run VerifyBGPIPv6UnicastState validation"""
 
-    if not state_issue:
-        result.is_success()
-    else:
-        result.is_failure(f"Some IPv6 Unicast BGP Peer are not up: {state_issue}")
+        command_output = self.instance_commands[0].json_output
 
-    return result
+        state_issue = _check_bgp_vrfs(command_output["vrfs"])
 
+        if not state_issue:
+            self.result.is_success()
+        else:
+            self.result.is_failure(f"Some IPv4 Unicast BGP Peer are not up: {state_issue}")
 
-@anta_test
-@check_bgp_family_enable("evpn")
-async def verify_bgp_evpn_state(device: InventoryDevice, result: TestResult) -> TestResult:
 
+class VerifyBGPEVPNState(AntaTest):
     """
     Verifies all EVPN BGP sessions are established (default VRF).
 
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
+    * self.result = "skipped" if no BGP EVPN peers are returned by the device
+    * self.result = "success" if all EVPN BGP sessions are established.
+    * self.result = "failure" otherwise.
+    """
+
+    name = "VerifyBGPEVPNState"
+    description = "Verifies all EVPN BGP sessions are established (default VRF)."
+    categories = ["routing", "bgp"]
+    commands = [AntaCommand(command="show bgp evpn summary")]
+
+    @check_bgp_family_enable("evpn")
+    @AntaTest.anta_test
+    def test(self) -> None:
+        """Run VerifyBGPEVPNState validation"""
 
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "skipped" if no BGP EVPN peers are returned by the device
-        * result = "success" if all EVPN BGP sessions are established.
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
-
-    """
-    response = await device.session.cli(command="show bgp evpn summary", ofmt="json")
-    logger.debug(f"query result is: {response}")
-
-    bgp_vrfs = response["vrfs"]
-
-    peers = bgp_vrfs["default"]["peers"]
-    non_established_peers = [
-        peer
-        for peer, peer_dict in peers.items()
-        if peer_dict["peerState"] != "Established"
-    ]
-
-    if not non_established_peers:
-        result.is_success()
-    else:
-        result.is_failure(
-            f"The following EVPN peers are not established: {non_established_peers}"
-        )
-
-    return result
-
-
-@anta_test
-@check_bgp_family_enable("evpn")
-async def verify_bgp_evpn_count(
-    device: InventoryDevice, result: TestResult, number: int
-) -> TestResult:
+        command_output = self.instance_commands[0].json_output
+
+        bgp_vrfs = command_output["vrfs"]
+
+        peers = bgp_vrfs["default"]["peers"]
+        non_established_peers = [peer for peer, peer_dict in peers.items() if peer_dict["peerState"] != "Established"]
+
+        if not non_established_peers:
+            self.result.is_success()
+        else:
+            self.result.is_failure(f"The following EVPN peers are not established: {non_established_peers}")
+
+
+class VerifyBGPEVPNCount(AntaTest):
     """
     Verifies all EVPN BGP sessions are established (default VRF)
     and the actual number of BGP EVPN neighbors is the one we expect (default VRF).
 
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
-        number (int): The expected number of BGP EVPN neighbors in the default VRF.
-
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "skipped" if the `number` parameter is missing
-        * result = "success" if all EVPN BGP sessions are Established and if the actual
-                             number of BGP EVPN neighbors is the one we expect.
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
-
-    """
-    if not number:
-        result.is_skipped(
-            "verify_bgp_evpn_count could not run because number was not supplied."
-        )
-        return result
-
-    response = await device.session.cli(command="show bgp evpn summary", ofmt="json")
-    logger.debug(f"query result is: {response}")
-
-    peers = response["vrfs"]["default"]["peers"]
-
-    if len(peers) == number:
-        result.is_success()
-    else:
-        result.is_failure()
-        if len(peers) != number:
-            result.messages.append(
-                f"Expecting {number} BGP EVPN peers and got {len(peers)}"
-            )
-
-    return result
-
-
-@anta_test
-@check_bgp_family_enable("rtc")
-async def verify_bgp_rtc_state(device: InventoryDevice, result: TestResult) -> TestResult:
+    * self.result = "skipped" if the `number` parameter is missing
+    * self.result = "success" if all EVPN BGP sessions are Established and if the actual
+                         number of BGP EVPN neighbors is the one we expect.
+    * self.result = "failure" otherwise.
+    """
+
+    name = "VerifyBGPEVPNCount"
+    description = "Verifies all EVPN BGP sessions are established (default VRF) and the actual number of BGP EVPN neighbors is the one we expect (default VRF)."
+    categories = ["routing", "bgp"]
+    commands = [AntaCommand(command="show bgp evpn summary")]
+
+    @check_bgp_family_enable("evpn")
+    @AntaTest.anta_test
+    def test(self, number: Optional[int] = None) -> None:
+        """
+        Run VerifyBGPEVPNCount validation
+
+        Args:
+            number: The expected number of BGP EVPN neighbors in the default VRF.
+        """
+        if not number:
+            self.result.is_skipped("VerifyBGPEVPNCount could not run because number was not supplied.")
+            return
+
+        command_output = self.instance_commands[0].json_output
+
+        peers = command_output["vrfs"]["default"]["peers"]
+        non_established_peers = [peer for peer, peer_dict in peers.items() if peer_dict["peerState"] != "Established"]
+
+        if not non_established_peers and len(peers) == number:
+            self.result.is_success()
+        else:
+            self.result.is_failure()
+            if len(peers) != number:
+                self.result.is_failure(f"Expecting {number} BGP EVPN peers and got {len(peers)}")
+            if non_established_peers:
+                self.result.is_failure(f"The following EVPN peers are not established: {non_established_peers}")
+
+
+class VerifyBGPRTCState(AntaTest):
     """
     Verifies all RTC BGP sessions are established (default VRF).
 
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
+    * self.result = "skipped" if no BGP RTC peers are returned by the device
+    * self.result = "success" if all RTC BGP sessions are established.
+    * self.result = "failure" otherwise.
+    """
+
+    name = "VerifyBGPRTCState"
+    description = "Verifies all RTC BGP sessions are established (default VRF)."
+    categories = ["routing", "bgp"]
+    commands = [AntaCommand(command="show bgp rt-membership summary")]
+
+    @check_bgp_family_enable("rtc")
+    @AntaTest.anta_test
+    def test(self) -> None:
+        """Run VerifyBGPRTCState validation"""
+
+        command_output = self.instance_commands[0].json_output
+
+        bgp_vrfs = command_output["vrfs"]
 
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "skipped" if no BGP RTC peers are returned by the device
-        * result = "success" if all RTC BGP sessions are Established.
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
-
-    """
-    response = await device.session.cli(command="show bgp rt-membership summary", ofmt="json")
-    logger.debug(f"query result is: {response}")
-
-    peers = response["vrfs"]["default"]["peers"]
-    non_established_peers = [
-        peer
-        for peer, peer_dict in peers.items()
-        if peer_dict["peerState"] != "Established"
-    ]
-
-    if not non_established_peers:
-        result.is_success()
-    else:
-        result.is_failure(
-            f"The following RTC peers are not established: {non_established_peers}"
-        )
-
-    return result
-
-
-@anta_test
-@check_bgp_family_enable("rtc")
-async def verify_bgp_rtc_count(
-    device: InventoryDevice, result: TestResult, number: int
-) -> TestResult:
+        peers = bgp_vrfs["default"]["peers"]
+        non_established_peers = [peer for peer, peer_dict in peers.items() if peer_dict["peerState"] != "Established"]
+
+        if not non_established_peers:
+            self.result.is_success()
+        else:
+            self.result.is_failure(f"The following RTC peers are not established: {non_established_peers}")
+
+
+class VerifyBGPRTCCount(AntaTest):
     """
     Verifies all RTC BGP sessions are established (default VRF)
     and the actual number of BGP RTC neighbors is the one we expect (default VRF).
 
-    Args:
-        device (InventoryDevice): InventoryDevice instance containing all devices information.
-        number (int): The expected number of BGP RTC neighbors (default VRF).
-
-    Returns:
-        TestResult instance with
-        * result = "unset" if the test has not been executed
-        * result = "skipped" if the `number` parameter is missing
-        * result = "success" if all RTC BGP sessions are established
-                             and if the actual number of BGP RTC neighbors is the one we expect.
-        * result = "failure" otherwise.
-        * result = "error" if any exception is caught
-
-    """
-    if not number:
-        result.is_skipped(
-            "verify_bgp_rtc_count could not run because number was not supplied"
-        )
-        return result
-
-    response = await device.session.cli(command="show bgp rt-membership summary", ofmt="json")
-    logger.debug(f"query result is: {response}")
-
-    peers = response["vrfs"]["default"]["peers"]
-    non_established_peers = [
-        peer
-        for peer, peer_dict in peers.items()
-        if peer_dict["peerState"] != "Established"
-    ]
-
-    if not non_established_peers and len(peers) == number:
-        result.is_success()
-    else:
-        result.is_failure()
-        if len(peers) != number:
-            result.is_failure(f"Expecting {number} BGP RTC peers and got {len(peers)}")
-
-    return result
+    * self.result = "skipped" if the `number` parameter is missing
+    * self.result = "success" if all RTC BGP sessions are Established and if the actual
+                         number of BGP RTC neighbors is the one we expect.
+    * self.result = "failure" otherwise.
+    """
+
+    name = "VerifyBGPRTCCount"
+    description = "Verifies all RTC BGP sessions are established (default VRF) and the actual number of BGP RTC neighbors is the one we expect (default VRF)."
+    categories = ["routing", "bgp"]
+    commands = [AntaCommand(command="show bgp rt-membership summary")]
+
+    @check_bgp_family_enable("rtc")
+    @AntaTest.anta_test
+    def test(self, number: Optional[int] = None) -> None:
+        """
+        Run VerifyBGPRTCCount validation
+
+        Args:
+            number: The expected number of BGP RTC neighbors (default VRF).
+        """
+        if not number:
+            self.result.is_skipped("VerifyBGPRTCCount could not run because number was not supplied")
+            return
+
+        command_output = self.instance_commands[0].json_output
+
+        peers = command_output["vrfs"]["default"]["peers"]
+        non_established_peers = [peer for peer, peer_dict in peers.items() if peer_dict["peerState"] != "Established"]
+
+        if not non_established_peers and len(peers) == number:
+            self.result.is_success()
+        else:
+            self.result.is_failure()
+            if len(peers) != number:
+                self.result.is_failure(f"Expecting {number} BGP RTC peers and got {len(peers)}")
+            if non_established_peers:
+                self.result.is_failure(f"The following RTC peers are not established: {non_established_peers}")
```

### Comparing `anta-0.5.0/anta/tools.py` & `anta-0.6.0/anta/tools/pydantic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
-Toolkit for ANTA.
+Toolkit for ANTA to play with Pydantic.
 """
 
+from __future__ import annotations
+
 import logging
-from typing import Any, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Sequence
 
-from .inventory.models import InventoryDevices
-from .result_manager.models import ListResult
+if TYPE_CHECKING:
+    from anta.result_manager.models import ListResult
 
 logger = logging.getLogger(__name__)
 
 
-def pydantic_to_dict(pydantic_list: Union[InventoryDevices, ListResult]) -> Any:
+def pydantic_to_dict(pydantic_list: ListResult) -> List[Dict[str, Sequence[Any]]]:
     """
-    Convert Pydantic object into a dict
+    Convert Pydantic object into a list of dict
 
     Mimic .dict() option from pydantic but overwrite IPv4Address nodes
 
     Args:
         pydantic_list: Iterable pydantic object
 
     Returns:
-        dict: dictionary object
+        List[Dict[str, str]]: the list of dict
     """
     result = []
     for device in pydantic_list:
-        dev_dict = {k: str(v) for k, v in device}
+        dev_dict = {k: str(v) if not isinstance(v, list) else v for k, v in device}
         result.append(dev_dict)
     return result
```

### Comparing `anta-0.5.0/anta.egg-info/PKG-INFO` & `anta-0.6.0/anta.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anta
-Version: 0.5.0
+Version: 0.6.0
 Summary: Arista Network Test Automation (ANTA) Framework
 Author-email: Khelil Sator <ksator@arista.com>
 Maintainer-email: Khelil Sator <ksator@arista.com>, Matthieu Tâche <mtache@arista.com>, Khelil Sator <ksator@arista.com>, Guillaume Mulocher <gmulocher@arista.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -202,17 +202,17 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Project-URL: Homepage, https://arista-netdevops-community.github.io/network-test-automation/
-Project-URL: Bug Tracker, https://github.com/arista-netdevops-community/network-test-automation/issues
-Project-URL: Contributing, https://github.com/arista-netdevops-community/network-test-automation/blob/master/CONTRIBUTING.md
+Project-URL: Homepage, https://www.anta.ninja
+Project-URL: Bug Tracker, https://github.com/arista-netdevops-community/anta/issues
+Project-URL: Contributing, https://github.com/arista-netdevops-community/anta/blob/master/CONTRIBUTING.md
 Keywords: test,anta,Arista,network,automation,networking,devops,netdevops
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -226,20 +226,22 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-[![License](https://img.shields.io/badge/license-Apache%202.0-brightgreen.svg)](https://github.com/arista-netdevops-community/network-test-automation/blob/master/LICENSE)
-[![CI](https://github.com/arista-netdevops-community/network-test-automation/actions/workflows/test.yml/badge.svg)](https://github.com/arista-netdevops-community/network-test-automation/actions)
-[![github release](https://img.shields.io/github/release/arista-netdevops-community/network-test-automation.svg)](https://github.com/arista-netdevops-community/network-test-automation/releases/)
+[![License](https://img.shields.io/badge/license-Apache%202.0-brightgreen.svg)](https://github.com/arista-netdevops-community/anta/blob/master/LICENSE)
+[![Linting and Testing Anta](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml/badge.svg)](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml)
+[![github release](https://img.shields.io/github/release/arista-netdevops-community/anta.svg)](https://github.com/arista-netdevops-community/anta/releases/)
 
 # Arista Network Test Automation (ANTA) Framework
 
+__WARNING:__ Documentation is work in progress for version 0.6.0 available in Pypi.
+
 This repository is a Python package to automate tests on Arista devices.
 
 - The package name is ANTA, which stands for **Arista Network Test Automation**.
 - This package provides a set of tests to validate the state of your network.
 - This package can be imported in Python scripts:
   - To automate NRFU (Network Ready For Use) test on a preproduction network
   - To automate tests on a live network (periodically or on demand)
@@ -250,48 +252,52 @@
 # Install ANTA CLI
 $ pip install anta
 
 # Run ANTA CLI
 $ anta
 Usage: anta [OPTIONS] COMMAND [ARGS]...
 
-  Arista Network Test CLI
+  Arista Network Test Automation (ANTA) CLI
 
 Options:
-  --username TEXT         Username to connect to EOS  [env var: ANTA_USERNAME]
-  --password TEXT         Password to connect to EOS  [env var: ANTA_PASSWORD]
-  --timeout INTEGER       Connection timeout (default 5)  [env var: ANTA_TIMEOUT]
-  --enable-password TEXT  Enable password if required to connect  [env var: ANTA_ENABLE_PASSWORD]
-  -i, --inventory PATH    Path to your inventory file  [env var: ANTA_INVENTORY]
-  --timeout INTEGER       Connection timeout (default 5)  [env var: ANTA_TIMEOUT]
-  --help                  Show this message and exit.
+  --version                       Show the version and exit.
+  --username TEXT                 Username to connect to EOS  [env var:
+                                  ANTA_USERNAME; required]
+  --password TEXT                 Password to connect to EOS  [env var:
+                                  ANTA_PASSWORD; required]
+  --timeout INTEGER               Global connection timeout  [env var:
+                                  ANTA_TIMEOUT; default: 5]
+  --insecure                      Disable SSH Host Key validation  [env var:
+                                  ANTA_INSECURE]
+  --enable-password TEXT          Enable password if required to connect  [env
+                                  var: ANTA_ENABLE_PASSWORD]
+  -i, --inventory FILE            Path to the inventory YAML file  [env var:
+                                  ANTA_INVENTORY; required]
+  --log-level, --log [CRITICAL|ERROR|WARNING|INFO|DEBUG]
+                                  ANTA logging level  [env var:
+                                  ANTA_LOG_LEVEL; default: INFO]
+  --ignore-status                 Always exit with success  [env var:
+                                  ANTA_IGNORE_STATUS]
+  --ignore-error                  Only report failures and not errors  [env
+                                  var: ANTA_IGNORE_ERROR]
+  --help                          Show this message and exit.
 
 Commands:
-  exec  Execute commands to inventory devices
-  get   Get data from/to ANTA
-  nrfu  Run NRFU against inventory devices
+  debug  Debug commands for building ANTA
+  exec   Execute commands to inventory devices
+  get    Get data from/to ANTA
+  nrfu   Run NRFU against inventory devices
 ```
 
-<img src="https://github.com/arista-netdevops-community/network-test-automation/raw/master/docs/imgs/anta-nrfu-table-group-by-test-output.png"></img>
-
-In addition, previous scripts are now marked as __deprecated__ and will be removed in a future release:
-
-- `check-devices.py` is an easy to use script to test your network with ANTA.
-- `collect-eos-commands.py` to collect commands output from devices
-- `collect-sheduled-show-tech.py` to collect the scheduled show tech-support files from devices
-- `clear-counters.py` to clear counters on devices
-- `evpn-blacklist-recovery.py` to clear the list of MAC addresses which are blacklisted in EVPN
-- `create-devices-inventory-from-cvp.py`: Build inventory for scripts from Arista Cloudvision (CVP)
-
-> Most of these scripts use eAPI (EOS API). You can find examples of EOS automation with eAPI in this [repository](https://github.com/arista-netdevops-community/arista_eos_automation_with_eAPI).
+<img src="https://github.com/arista-netdevops-community/anta/raw/master/docs/imgs/anta-nrfu-table-group-by-test-output.png"></img>
 
 # Documentation
 
-The documentation is published on [ANTA package website](https://arista-netdevops-community.github.io/network-test-automation/)
+The documentation is published on [ANTA package website](https://www.anta.ninja)
 
 # Contribution guide
 
-Contributions are welcome. Please refer to the [contribution guide](https://raw.githubusercontent.com/arista-netdevops-community/network-test-automation/master/docs/contribution.md)
+Contributions are welcome. Please refer to the [contribution guide](https://raw.githubusercontent.com/arista-netdevops-community/anta/master/docs/contribution.md)
 
 # Credits
 
 Thank you to [Angélique Phillipps](https://github.com/aphillipps), [Colin MacGiollaEáin](https://github.com/colinmacgiolla), [Khelil Sator](https://github.com/ksator), [Matthieu Tache](https://github.com/mtache), [Onur Gashi](https://github.com/onurgashi), [Paul Lavelle](https://github.com/paullavelle), [Guillaume Mulocher](https://github.com/gmuloc) and [Thomas Grimonet](https://github.com/titom73) for their contributions and guidances.
```

### Comparing `anta-0.5.0/pyproject.toml` & `anta-0.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # content of pyproject.toml
-
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anta"
-version = "v0.5.0"
+version = "v0.6.0"
 readme = "README.md"
 authors = [{ name = "Khelil Sator", email = "ksator@arista.com" }]
 maintainers = [
   { name = "Khelil Sator", email = "ksator@arista.com" },
   { name = "Matthieu Tâche", email = "mtache@arista.com" },
   { name = "Khelil Sator", email = "ksator@arista.com" },
   { name = "Guillaume Mulocher", email = "gmulocher@arista.com" },
 ]
 description = "Arista Network Test Automation (ANTA) Framework"
 license = { file = "LICENSE" }
 dependencies = [
   "aio-eapi==0.3.0",
   "click==8.1.3",
   "click-help-colors==0.9.1",
-  "cvprac>=1.2.0",
-  "netaddr>=0.8.0",
-  "paramiko",
-  "pydantic>=1.9.1",
-  "PyYAML>=6.0",
-  "requests",
-  "rich>=12.5.1",
-  "scp",
+  "cvprac~=1.3",
+  "netaddr==0.8.0",
+  "pydantic~=2.0",
+  "PyYAML==6.0",
+  "requests>=2.27",
+  "rich~=13.4",
+  "asyncssh==2.13.1",
+  "Jinja2==3.1.2",
 ]
 keywords = ["test", "anta", "Arista", "network", "automation", "networking", "devops", "netdevops"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -49,56 +48,80 @@
     "Topic :: System :: Networking",
 ]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = [
   "bump2version==1.0.1",
+  "black==23.3.0",
   "flake8==6.0.0",
   "isort==5.10.1",
-  "mypy==0.991",
-  "mypy-extensions>=0.4.3",
+  "mypy~=1.4",
+  "mypy-extensions~=1.0",
   "pre-commit>=2.20.0",
-  "pylint>=2.16.1",
+  "pylint>=2.17",
   "pytest>=7.1.2",
   "pytest-cov>=2.11.1",
   "pytest-dependency",
   "pytest-html>=3.1.1",
   "pytest-metadata>=1.11.0",
-  "pylint-pydantic>=0.1.4",
+  "pylint-pydantic>=0.2.0",
   "tox==4.0.11",
   "types-PyYAML",
   "types-paramiko",
   "types-requests",
   "typing-extensions",
   "yamllint",
 ]
 
 [project.urls]
-Homepage = "https://arista-netdevops-community.github.io/network-test-automation/"
-"Bug Tracker" = "https://github.com/arista-netdevops-community/network-test-automation/issues"
-Contributing = "https://github.com/arista-netdevops-community/network-test-automation/blob/master/CONTRIBUTING.md"
+Homepage = "https://www.anta.ninja"
+"Bug Tracker" = "https://github.com/arista-netdevops-community/anta/issues"
+Contributing = "https://github.com/arista-netdevops-community/anta/blob/master/CONTRIBUTING.md"
 
 [project.scripts]
-anta = "anta.cli.cli:cli"
+anta = "anta.cli:cli"
+
 
+################################
+# Tools
+################################
 [tool.setuptools.packages.find]
 include = ["anta*"]
 namespaces = false
 
+################################
+# Linting
+################################
+[tool.isort]
+profile = "black"
+line_length = 165
+
+[tool.black]
+line-length = 165
+force-exclude = """
+(
+.*data.py|
+)
+"""
+
+################################
+# Typing
 # mypy as per https://pydantic-docs.helpmanual.io/mypy_plugin/#enabling-the-plugin
+################################
 [tool.mypy]
 plugins = [
   "pydantic.mypy",
   ]
-follow_imports = "skip"
+# Comment below for better type checking
+#follow_imports = "skip"
 ignore_missing_imports = true
 warn_redundant_casts = true
-# Note: tox find some unused type ignore which are required for pre-commit.. to
-# investigate
+# Note: tox find some unused type ignore which are required for pre-commit
+# To investigate
 # warn_unused_ignores = true
 disallow_any_generics = true
 check_untyped_defs = true
 no_implicit_reexport = true
 strict_optional = true
 
 # for strict mypy: (this is the tricky one :-))
@@ -108,73 +131,109 @@
 
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
+################################
+# Testing
+################################
+[tool.pytest.ini_options]
+# TODO - may need cov-append for Tox
+# When run from anta directory this will read cov-config from pyproject.toml
+addopts = "-ra -q -s -vv --capture=tee-sys --cov --cov-report term:skip-covered --color yes"
+log_level = "DEBUG"
+log_cli = true
+render_collapsed = true
+filterwarnings = [
+  "ignore::urllib3.exceptions.InsecureRequestWarning"
+]
+
+[tool.coverage.run]
+branch = true
+source = ["anta"]
+parallel = true
+# omit=anta/tests/*
+
+[tool.coverage.report]
+# Regexes for lines to exclude from consideration
+exclude_lines = [
+    # Have to re-enable the standard pragma
+    "pragma = no cover",
+
+    # Don't complain about missing debug-only code:
+    "def __repr__",
+    "if self\\.debug",
+
+    # Don't complain if tests don't hit defensive assertion code:
+    "raise AssertionError",
+    "raise NotImplementedError",
+
+    # Don't complain if non-runnable code isn't run:
+    "if 0:",
+    "if __name__ == .__main__.:",
+
+    # Don't complain about abstract methods, they aren't run:
+    "@(abc\\.)?abstractmethod",
+]
+
+ignore_errors = true
 
+[tool.coverage.html]
+directory = "coverage_html_report"
+
+################################
+# Tox
+################################
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 min_version = 4.0
 envlist =
   clean,
-  py{38,39,310},
   lint,
   type,
+  py{38,39,310,311},
   report
 
 [gh-actions]
 python =
   3.8: py38
   3.9: py39
-  3.10: py310, lint, type, report
+  3.10: erase, py310, report
+  3.11: py311
 
 [testenv]
 description = run the test driver with {basepython}
 extras = dev
 commands =
-   pytest  {tty:--color=yes}
+   pytest
 
 [testenv:lint]
 description = check the code style
 commands =
+  black --check --diff --color .
+  isort --check --diff --color .
   flake8 --max-line-length=165 --config=/dev/null anta
-  flake8 --max-line-length=165 --config=/dev/null scripts
   flake8 --max-line-length=165 --config=/dev/null tests
   pylint anta
-  pylint scripts
 
 [testenv:type]
 description = check typing
 commands =
   type: mypy --config-file=pyproject.toml anta
-  type: mypy --config-file=pyproject.toml scripts
 
 [testenv:clean]
 deps = coverage[toml]
 skip_install = true
 commands = coverage erase
 
 [testenv:report]
 deps = coverage[toml]
-# TODO adding -i for now
-commands = coverage report -i 
+commands =
+  coverage --version
+  coverage report --rcfile=pyproject.toml
 # add the following to make the report fail under some percentage
 # commands = coverage report --fail-under=80
 depends = py310
-
 """
-
-[tool.pytest.ini_options]
-addopts = "-ra -q -s -vv --capture=tee-sys --ignore=tests/scripts --cov --cov-append"
-log_level = "INFO"
-log_cli = "True"
-
-[tool.coverage.run]
-source = ['anta']
-# omit = []
-
-[tool.isort]
-profile = "black"
-line_length = 165
```

