# Comparing `tmp/zigpy-znp-0.9.2.tar.gz` & `tmp/zigpy-znp-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-znp-0.9.2.tar", last modified: Tue Nov 29 23:28:55 2022, max compression
+gzip compressed data, was "zigpy-znp-0.9.3.tar", last modified: Wed Feb 22 17:56:03 2023, max compression
```

## Comparing `zigpy-znp-0.9.2.tar` & `zigpy-znp-0.9.3.tar`

### file list

```diff
@@ -1,67 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:55.056323 zigpy-znp-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11424 2022-11-29 23:28:55.056323 zigpy-znp-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9747 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1803 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      775 2022-11-29 23:28:55.056323 zigpy-znp-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       69 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:55.048323 zigpy-znp-0.9.2/zigpy_znp/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    38681 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:55.052323 zigpy-znp-0.9.2/zigpy_znp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      799 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12964 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/af.py
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     6637 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/app_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    23116 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/mac.py
--rw-r--r--   0 runner    (1001) docker     (122)      794 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (122)     7080 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/sapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    21892 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/sys.py
--rw-r--r--   0 runner    (1001) docker     (122)     2919 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/ubl.py
--rw-r--r--   0 runner    (1001) docker     (122)    17818 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    47070 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/zdo.py
--rw-r--r--   0 runner    (1001) docker     (122)     6268 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/zgp.py
--rw-r--r--   0 runner    (1001) docker     (122)      991 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/commands/znp.py
--rw-r--r--   0 runner    (1001) docker     (122)     4214 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      819 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/const.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2772 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/frames.py
--rw-r--r--   0 runner    (1001) docker     (122)      710 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)    13722 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/nvram.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:55.052323 zigpy-znp-0.9.2/zigpy_znp/tools/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6507 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3006 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/energy_scan.py
--rw-r--r--   0 runner    (1001) docker     (122)     2652 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/flash_read.py
--rw-r--r--   0 runner    (1001) docker     (122)     5355 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/flash_write.py
--rw-r--r--   0 runner    (1001) docker     (122)     3774 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/network_backup.py
--rw-r--r--   0 runner    (1001) docker     (122)     4379 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/network_restore.py
--rw-r--r--   0 runner    (1001) docker     (122)     4732 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/network_scan.py
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/nvram_read.py
--rw-r--r--   0 runner    (1001) docker     (122)     2250 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/nvram_reset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/tools/nvram_write.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:55.056323 zigpy-znp-0.9.2/zigpy_znp/types/
--rw-r--r--   0 runner    (1001) docker     (122)      274 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7785 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (122)    18541 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/types/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     6405 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/types/cstruct.py
--rw-r--r--   0 runner    (1001) docker     (122)    10860 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/types/named.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/types/nvids.py
--rw-r--r--   0 runner    (1001) docker     (122)     6651 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/types/structs.py
--rw-r--r--   0 runner    (1001) docker     (122)      200 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/types/zigpy_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     5732 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/uart.py
--rw-r--r--   0 runner    (1001) docker     (122)     5934 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:55.056323 zigpy-znp-0.9.2/zigpy_znp/zigbee/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/zigbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    44624 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/zigbee/application.py
--rw-r--r--   0 runner    (1001) docker     (122)     5669 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/zigbee/device.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:55.056323 zigpy-znp-0.9.2/zigpy_znp/znp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/znp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16280 2022-11-29 23:28:49.000000 zigpy-znp-0.9.2/zigpy_znp/znp/security.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 23:28:55.048323 zigpy-znp-0.9.2/zigpy_znp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11424 2022-11-29 23:28:54.000000 zigpy-znp-0.9.2/zigpy_znp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1473 2022-11-29 23:28:55.000000 zigpy-znp-0.9.2/zigpy_znp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 23:28:54.000000 zigpy-znp-0.9.2/zigpy_znp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      225 2022-11-29 23:28:54.000000 zigpy-znp-0.9.2/zigpy_znp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-11-29 23:28:54.000000 zigpy-znp-0.9.2/zigpy_znp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:56:03.393822 zigpy-znp-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-02-22 17:56:03.393822 zigpy-znp-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 17:56:03.393822 zigpy-znp-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:56:03.385822 zigpy-znp-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/tests/test_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/tests/test_nvids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/tests/test_trace_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/tests/test_types_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12206 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/tests/test_types_cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/tests/test_types_named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/tests/test_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:56:03.385822 zigpy-znp-0.9.3/zigpy_znp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38872 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:56:03.389822 zigpy-znp-0.9.3/zigpy_znp/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/af.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23116 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/mac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/sapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21892 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/sys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/ubl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47070 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/zdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/zgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/commands/znp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/nvram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:56:03.389822 zigpy-znp-0.9.3/zigpy_znp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/energy_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/flash_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/flash_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/network_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/network_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/network_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/nvram_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/nvram_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/tools/nvram_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:56:03.393822 zigpy-znp-0.9.3/zigpy_znp/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/types/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/types/cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/types/nvids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/types/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/types/zigpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:56:03.393822 zigpy-znp-0.9.3/zigpy_znp/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/zigbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44858 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/zigbee/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/zigbee/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:56:03.393822 zigpy-znp-0.9.3/zigpy_znp/znp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/znp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-02-22 17:55:54.000000 zigpy-znp-0.9.3/zigpy_znp/znp/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:56:03.389822 zigpy-znp-0.9.3/zigpy_znp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-02-22 17:56:03.000000 zigpy-znp-0.9.3/zigpy_znp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-02-22 17:56:03.000000 zigpy-znp-0.9.3/zigpy_znp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 17:56:03.000000 zigpy-znp-0.9.3/zigpy_znp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-22 17:56:03.000000 zigpy-znp-0.9.3/zigpy_znp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-22 17:56:03.000000 zigpy-znp-0.9.3/zigpy_znp.egg-info/top_level.txt
```

### Comparing `zigpy-znp-0.9.2/LICENSE` & `zigpy-znp-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/PKG-INFO` & `zigpy-znp-0.9.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,175 +1,174 @@
 Metadata-Version: 2.1
 Name: zigpy-znp
-Version: 0.9.2
+Version: 0.9.3
 Summary: A library for zigpy which communicates with TI ZNP radios
-Home-page: https://github.com/zigpy/zigpy-znp
-Author: Alexei Chetroi
-Author-email: alexei.chetroi@outlook.com
+Author-email: Alexei Chetroi <alexei.chetroi@outlook.com>
 License: GPL-3.0
-Description: # zigpy-znp
-        
-        [![Build Status](https://github.com/zigpy/zigpy-znp/workflows/CI/badge.svg)](https://github.com/zigpy/zigpy-znp/actions)
-        [![Coverage Status](https://codecov.io/gh/zigpy/zigpy-znp/branch/dev/graph/badge.svg?token=Y1994N9D74)](https://codecov.io/gh/zigpy/zigpy-znp)
-        
-        **[zigpy-znp](https://github.com/zigpy/zigpy-znp/)** is a Python library that adds support for common [Texas Instruments ZNP (Zigbee Network Processors)](http://dev.ti.com/tirex/content/simplelink_zigbee_sdk_plugin_2_20_00_06/docs/zigbee_user_guide/html/zigbee/introduction.html) [Zigbee](https://www.zigbee.org) radio modules to [zigpy](https://github.com/zigpy/), a Python Zigbee stack project.
-        
-        Together with zigpy and compatible home automation software (namely Home Assistant's [ZHA (Zigbee Home Automation) integration component](https://www.home-assistant.io/integrations/zha/)), you can directly control Zigbee devices such as Philips Hue, GE, OSRAM LIGHTIFY, Xiaomi/Aqara, IKEA Tradfri, Samsung SmartThings, and many more.
-        
-        # Installation
-        
-        ## Python module
-        Install the Python module within your virtual environment:
-        
-        ```console
-        $ virtualenv -p python3.8 venv                                # if you don't already have one
-        $ source venv/bin/activate
-        (venv) $ pip install git+https://github.com/zigpy/zigpy-znp/  # latest commit from Git
-        (venv) $ pip install zigpy-znp                                # or, latest stable from PyPI
-        ```
-        
-        ## Home Assistant
-        Stable releases of zigpy-znp are automatically installed when you install the ZHA component.
-        
-        ### Testing `dev` with Home Assistant Core
-        
-        Upgrade the package within your virtual environment (requires `git`):
-        
-        ```console
-        (venv) $ pip install git+https://github.com/zigpy/zigpy-znp/
-        ```
-        
-        Launch Home Assistant with the `--skip-pip` command line option to prevent zigpy-znp from being downgraded. Running with this option may prevent newly added integrations from installing required packages.
-        
-        ### Testing `dev` with Home Assistant OS
-        
-         - Add https://github.com/home-assistant/hassio-addons-development as an addon repository.
-         - Install the "Custom deps deployment" addon.
-         - Add the following to your `configuration.yaml` file:
-           ```yaml
-           apk: []
-           pypi:
-             - git+https://github.com/zigpy/zigpy-znp/
-        	 ```
-        
-        # Configuration
-        Below are the defaults with the top-level Home Assistant `zha:` key.
-        **You do not need to copy this configuration, it is provided only for reference**:
-        
-        ```yaml
-        zha:
-          zigpy_config:
-            znp_config:
-              # Only if your stick has a built-in power amplifier (i.e. CC1352P and CC2592)
-              # If set, must be between:
-              #  * CC1352/2652:  -22 and 19
-              #  * CC253x:       -22 and 22
-              tx_power:  
-        
-              # Only if your stick has a controllable LED (the CC2531)
-              # If set, must be one of: off, on, blink, flash, toggle
-              led_mode: off
-        
-        
-              ### Internal configuration, there's no reason to touch these values
-        
-              # Skips the 60s bootloader delay on CC2531 sticks
-              skip_bootloader: True
-        
-              # Timeout for synchronous requests' responses
-              sreq_timeout: 15
-        
-              # Timeout for asynchronous requests' callback responses
-              arsp_timeout: 30
-        
-              # Delay between auto-reconnect attempts in case the device gets disconnected
-              auto_reconnect_retry_delay: 5
-        
-              # Pin states for skipping the bootloader
-              connect_rts_pin_states: [off, on, off]
-              connect_dtr_pin_states: [off, off, off]
-        ```
-        
-        # Tools
-        Various command line Zigbee utilities are a part of the zigpy-znp package and can be run
-        with `python -m zigpy_znp.tools.name_of_tool`. More detailed documentation can be found
-        in **[`TOOLS.md`](./TOOLS.md)** but a brief description of each tool is included below:
-        
-         - **`energy_scan`**: Performs a continuous energy scan to check for non-Zigbee interference.
-         - **`flash_read`**: For CC2531s, reads firmware from flash.
-         - **`flash_write`**: For CC2531s, writes a firmware `.bin` to flash.
-         - **`form_network`**: Forms a network with randomized settings on channel 15.
-         - **`network_backup`**: Backs up the network data and device information into a human-readable JSON document.
-         - **`network_restore`**: Restores a JSON network backup to the adapter.
-         - **`network_scan`**: Actively sends beacon requests for network stumbling.
-         - **`nvram_read`**: Reads all possible NVRAM entries into a JSON document.
-         - **`nvram_reset`**: Deletes all possible NVRAM entries
-         - **`nvram_write`**: Writes all NVRAM entries from a JSON document.
-        
-        # Hardware requirements
-        USB-adapters, GPIO-modules, and development-boards flashed with TI's Z-Stack are compatible with zigpy-znp:
-        
-         - CC2652P/CC2652R/CC2652RB USB stick and dev board hardware
-         - CC1352P/CC1352R USB stick and dev board hardware
-         - CC2538 + CC2592 USB stick and dev board hardware (**not recommended, old hardware and end-of-life firmware**)
-         - CC2531 USB stick hardware (**not recommended for Zigbee networks with more than 20 devices**)
-         - CC2530 + CC2591/CC2592 USB stick hardware (**not recommended for Zigbee networks with more than 20 devices**)
-        
-        Tip! Adapters listed as "[Texas Instruments sticks compatible with Zigbee2MQTT](https://www.zigbee2mqtt.io/information/supported_adapters)" also works with zigpy-znp.
-        
-        ## Reference hardware for this project
-        These specific adapters are used as reference hardware for development and testing by zigpy-znp developers:
-        
-         - [TI LAUNCHXL-CC26X2R1](https://www.ti.com/tool/LAUNCHXL-CC26X2R1) running [Z-Stack 3 firmware (based on version 4.40.00.44)](https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0/bin). You can flash `CC2652R_20210120.hex` using [TI's UNIFLASH](https://www.ti.com/tool/download/UNIFLASH).
-         - [Electrolama zzh CC2652R](https://electrolama.com/projects/zig-a-zig-ah/) and [Slaesh CC2652R](https://slae.sh/projects/cc2652/) sticks running [Z-Stack 3 firmware (based on version 4.40.00.44)](https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0/bin). You can flash `CC2652R_20210120.hex` or `CC2652RB_20210120.hex` respectively using [cc2538-bsl](https://github.com/JelmerT/cc2538-bsl).
-         - CC2531 running [Z-Stack Home 1.2](https://github.com/Koenkk/Z-Stack-firmware/blob/master/coordinator/Z-Stack_Home_1.2/bin/default/CC2531_DEFAULT_20190608.zip). You can flash `CC2531ZNP-Prod.bin` to your stick directly with `zigpy_znp`: `python -m zigpy_znp.tools.flash_write -i /path/to/CC2531ZNP-Prod.bin /dev/serial/by-id/YOUR-CC2531` if your stick already has a serial bootloader.
-        
-        ## Texas Instruments Chip Part Numbers
-        Texas Instruments (TI) has quite a few different wireless MCU chips and they are all used/mentioned in open-source Zigbee world which can be daunting if you are just starting out. Here is a quick summary of part numbers and key features.
-        
-        ### Supported newer generation TI chips
-        
-        #### 2.4GHz frequency only chips
-        - CC2652R: 2.4GHz only wireless MCU for IEEE 802.15.4 multi-protocol (Zigbee, Bluetooth, Thread, IEEE 802.15.4g IPv6-enabled smart objects like 6LoWPAN, and proprietary systems). Cortex-M0 core for radio stack and Cortex-M4F core for application use, plenty of RAM. Free compiler option from TI.
-        - CC2652RB: Pin compatible "Crystal-less" CC2652R (so you could use it if you were to build your own zzh and omit the crystal) but not firmware compatible.
-        - CC2652P: CC2652R with a built-in RF PA. Not pin or firmware compatible with CC2652R/CC2652RB. 
-        
-        #### Multi frequency chips
-        - CC1352R: Sub 1 GHz & 2.4 GHz wireless MCU. Essentially CC2652R with an extra sub-1GHz radio.
-        - CC1352P: CC1352R with a built in RF PA.
-        
-        ### Supported older generation TI chips
-        - CC2538: 2.4GHz Zigbee, 6LoWPAN, and IEEE 802.15.4 wireless MCU. ARM Cortex-M3 core with with 512kB Flash and 32kB RAM.
-        - CC2531: CC2530 with a built-in UART/TTL to USB Bridge. Used in the cheap "Zigbee sticks" sold everywhere. Intel 8051 core, 256 Flash, only has 8kB RAM.
-        - CC2530: 2.4GHz Zigbee and IEEE 802.15.4 wireless MCU. Intel 8051 core, 256 Flash, only has 8kB RAM.
-        
-        ### Auxiliary TI chips
-        - CC2591 and CC2592: 2.4 GHz range extenders. These are not wireless MCUs, just auxiliary PA (Power Amplifier) and LNA (Low Noise Amplifier) in the same package to improve RF (Radio Frequency) range of any 2.4 GHz radio chip.
-        
-        # Releases via PyPI
-        
-        Tagged versions will also be released via PyPI
-        
-         - https://pypi.org/project/zigpy-znp/
-         - https://pypi.org/project/zigpy-znp/#history
-         - https://pypi.org/project/zigpy-znp/#files
-        
-        # External documentation and reference
-        
-        - http://www.ti.com/tool/LAUNCHXL-CC26X2R1
-        - http://www.ti.com/tool/LAUNCHXL-CC1352P
-        
-        # How to contribute
-        
-        If you are looking to make a code or documentation contribution to this project we suggest that you follow the steps in these guides:
-        - https://github.com/firstcontributions/first-contributions/blob/master/README.md
-        - https://github.com/firstcontributions/first-contributions/blob/master/github-desktop-tutorial.md
-        
-        # Related projects
-        
-        ### Zigpy
-        **[zigpy](https://github.com/zigpy/zigpy)** is [Zigbee protocol stack](https://en.wikipedia.org/wiki/Zigbee) integration project to implement the **[Zigbee Home Automation](https://www.zigbee.org/)** standard as a Python library. Zigbee Home Automation integration with zigpy allows you to connect one of many off-the-shelf Zigbee adapters using one of the available Zigbee radio library modules compatible with zigpy to control Zigbee devices. There is currently support for controlling Zigbee device types such as binary sensors (e.g. motion and door sensors), analog sensors (e.g. temperature sensors), lightbulbs, switches, and fans. Zigpy is tightly integrated with [Home Assistant](https://www.home-assistant.io)'s [ZHA component](https://www.home-assistant.io/components/zha/) and provides a user-friendly interface for working with a Zigbee network.
-        
-Platform: UNKNOWN
+Project-URL: repository, https://github.com/zigpy/zigpy-znp
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
+Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+
+# zigpy-znp
+
+[![Build Status](https://github.com/zigpy/zigpy-znp/workflows/CI/badge.svg)](https://github.com/zigpy/zigpy-znp/actions)
+[![Coverage Status](https://codecov.io/gh/zigpy/zigpy-znp/branch/dev/graph/badge.svg?token=Y1994N9D74)](https://codecov.io/gh/zigpy/zigpy-znp)
+
+**[zigpy-znp](https://github.com/zigpy/zigpy-znp/)** is a Python library that adds support for common [Texas Instruments ZNP (Zigbee Network Processors)](http://dev.ti.com/tirex/content/simplelink_zigbee_sdk_plugin_2_20_00_06/docs/zigbee_user_guide/html/zigbee/introduction.html) [Zigbee](https://www.zigbee.org) radio modules to [zigpy](https://github.com/zigpy/), a Python Zigbee stack project.
+
+Together with zigpy and compatible home automation software (namely Home Assistant's [ZHA (Zigbee Home Automation) integration component](https://www.home-assistant.io/integrations/zha/)), you can directly control Zigbee devices such as Philips Hue, GE, OSRAM LIGHTIFY, Xiaomi/Aqara, IKEA Tradfri, Samsung SmartThings, and many more.
+
+# Installation
+
+## Python module
+Install the Python module within your virtual environment:
+
+```console
+$ virtualenv -p python3.8 venv                                # if you don't already have one
+$ source venv/bin/activate
+(venv) $ pip install git+https://github.com/zigpy/zigpy-znp/  # latest commit from Git
+(venv) $ pip install zigpy-znp                                # or, latest stable from PyPI
+```
+
+## Home Assistant
+Stable releases of zigpy-znp are automatically installed when you install the ZHA component.
+
+### Testing `dev` with Home Assistant Core
+
+Upgrade the package within your virtual environment (requires `git`):
+
+```console
+(venv) $ pip install git+https://github.com/zigpy/zigpy-znp/
+```
+
+Launch Home Assistant with the `--skip-pip` command line option to prevent zigpy-znp from being downgraded. Running with this option may prevent newly added integrations from installing required packages.
+
+### Testing `dev` with Home Assistant OS
+
+ - Add https://github.com/home-assistant/hassio-addons-development as an addon repository.
+ - Install the "Custom deps deployment" addon.
+ - Add the following to your `configuration.yaml` file:
+   ```yaml
+   apk: []
+   pypi:
+     - git+https://github.com/zigpy/zigpy-znp/
+	 ```
+
+# Configuration
+Below are the defaults with the top-level Home Assistant `zha:` key.
+**You do not need to copy this configuration, it is provided only for reference**:
+
+```yaml
+zha:
+  zigpy_config:
+    znp_config:
+      # Only if your stick has a built-in power amplifier (i.e. CC1352P and CC2592)
+      # If set, must be between:
+      #  * CC1352/2652:  -22 and 19
+      #  * CC253x:       -22 and 22
+      tx_power:  
+
+      # Only if your stick has a controllable LED (the CC2531)
+      # If set, must be one of: off, on, blink, flash, toggle
+      led_mode: off
+
+
+      ### Internal configuration, there's no reason to touch these values
+
+      # Skips the 60s bootloader delay on CC2531 sticks
+      skip_bootloader: True
+
+      # Timeout for synchronous requests' responses
+      sreq_timeout: 15
+
+      # Timeout for asynchronous requests' callback responses
+      arsp_timeout: 30
+
+      # Delay between auto-reconnect attempts in case the device gets disconnected
+      auto_reconnect_retry_delay: 5
+
+      # Pin states for skipping the bootloader
+      connect_rts_pin_states: [off, on, off]
+      connect_dtr_pin_states: [off, off, off]
+```
+
+# Tools
+Various command line Zigbee utilities are a part of the zigpy-znp package and can be run
+with `python -m zigpy_znp.tools.name_of_tool`. More detailed documentation can be found
+in **[`TOOLS.md`](./TOOLS.md)** but a brief description of each tool is included below:
+
+ - **`energy_scan`**: Performs a continuous energy scan to check for non-Zigbee interference.
+ - **`flash_read`**: For CC2531s, reads firmware from flash.
+ - **`flash_write`**: For CC2531s, writes a firmware `.bin` to flash.
+ - **`form_network`**: Forms a network with randomized settings on channel 15.
+ - **`network_backup`**: Backs up the network data and device information into a human-readable JSON document.
+ - **`network_restore`**: Restores a JSON network backup to the adapter.
+ - **`network_scan`**: Actively sends beacon requests for network stumbling.
+ - **`nvram_read`**: Reads all possible NVRAM entries into a JSON document.
+ - **`nvram_reset`**: Deletes all possible NVRAM entries
+ - **`nvram_write`**: Writes all NVRAM entries from a JSON document.
+
+# Hardware requirements
+USB-adapters, GPIO-modules, and development-boards flashed with TI's Z-Stack are compatible with zigpy-znp:
+
+ - CC2652P/CC2652R/CC2652RB USB stick and dev board hardware
+ - CC1352P/CC1352R USB stick and dev board hardware
+ - CC2538 + CC2592 USB stick and dev board hardware (**not recommended, old hardware and end-of-life firmware**)
+ - CC2531 USB stick hardware (**not recommended for Zigbee networks with more than 20 devices**)
+ - CC2530 + CC2591/CC2592 USB stick hardware (**not recommended for Zigbee networks with more than 20 devices**)
+
+Tip! Adapters listed as "[Texas Instruments sticks compatible with Zigbee2MQTT](https://www.zigbee2mqtt.io/information/supported_adapters)" also works with zigpy-znp.
+
+## Reference hardware for this project
+These specific adapters are used as reference hardware for development and testing by zigpy-znp developers:
+
+ - [TI LAUNCHXL-CC26X2R1](https://www.ti.com/tool/LAUNCHXL-CC26X2R1) running [Z-Stack 3 firmware (based on version 4.40.00.44)](https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0/bin). You can flash `CC2652R_20210120.hex` using [TI's UNIFLASH](https://www.ti.com/tool/download/UNIFLASH).
+ - [Electrolama zzh CC2652R](https://electrolama.com/projects/zig-a-zig-ah/) and [Slaesh CC2652R](https://slae.sh/projects/cc2652/) sticks running [Z-Stack 3 firmware (based on version 4.40.00.44)](https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0/bin). You can flash `CC2652R_20210120.hex` or `CC2652RB_20210120.hex` respectively using [cc2538-bsl](https://github.com/JelmerT/cc2538-bsl).
+ - CC2531 running [Z-Stack Home 1.2](https://github.com/Koenkk/Z-Stack-firmware/blob/master/coordinator/Z-Stack_Home_1.2/bin/default/CC2531_DEFAULT_20190608.zip). You can flash `CC2531ZNP-Prod.bin` to your stick directly with `zigpy_znp`: `python -m zigpy_znp.tools.flash_write -i /path/to/CC2531ZNP-Prod.bin /dev/serial/by-id/YOUR-CC2531` if your stick already has a serial bootloader.
+
+## Texas Instruments Chip Part Numbers
+Texas Instruments (TI) has quite a few different wireless MCU chips and they are all used/mentioned in open-source Zigbee world which can be daunting if you are just starting out. Here is a quick summary of part numbers and key features.
+
+### Supported newer generation TI chips
+
+#### 2.4GHz frequency only chips
+- CC2652R: 2.4GHz only wireless MCU for IEEE 802.15.4 multi-protocol (Zigbee, Bluetooth, Thread, IEEE 802.15.4g IPv6-enabled smart objects like 6LoWPAN, and proprietary systems). Cortex-M0 core for radio stack and Cortex-M4F core for application use, plenty of RAM. Free compiler option from TI.
+- CC2652RB: Pin compatible "Crystal-less" CC2652R (so you could use it if you were to build your own zzh and omit the crystal) but not firmware compatible.
+- CC2652P: CC2652R with a built-in RF PA. Not pin or firmware compatible with CC2652R/CC2652RB. 
+
+#### Multi frequency chips
+- CC1352R: Sub 1 GHz & 2.4 GHz wireless MCU. Essentially CC2652R with an extra sub-1GHz radio.
+- CC1352P: CC1352R with a built in RF PA.
+
+### Supported older generation TI chips
+- CC2538: 2.4GHz Zigbee, 6LoWPAN, and IEEE 802.15.4 wireless MCU. ARM Cortex-M3 core with with 512kB Flash and 32kB RAM.
+- CC2531: CC2530 with a built-in UART/TTL to USB Bridge. Used in the cheap "Zigbee sticks" sold everywhere. Intel 8051 core, 256 Flash, only has 8kB RAM.
+- CC2530: 2.4GHz Zigbee and IEEE 802.15.4 wireless MCU. Intel 8051 core, 256 Flash, only has 8kB RAM.
+
+### Auxiliary TI chips
+- CC2591 and CC2592: 2.4 GHz range extenders. These are not wireless MCUs, just auxiliary PA (Power Amplifier) and LNA (Low Noise Amplifier) in the same package to improve RF (Radio Frequency) range of any 2.4 GHz radio chip.
+
+# Releases via PyPI
+
+Tagged versions will also be released via PyPI
+
+ - https://pypi.org/project/zigpy-znp/
+ - https://pypi.org/project/zigpy-znp/#history
+ - https://pypi.org/project/zigpy-znp/#files
+
+# External documentation and reference
+
+- http://www.ti.com/tool/LAUNCHXL-CC26X2R1
+- http://www.ti.com/tool/LAUNCHXL-CC1352P
+
+# How to contribute
+
+If you are looking to make a code or documentation contribution to this project we suggest that you follow the steps in these guides:
+- https://github.com/firstcontributions/first-contributions/blob/master/README.md
+- https://github.com/firstcontributions/first-contributions/blob/master/github-desktop-tutorial.md
+
+# Related projects
+
+### Zigpy
+**[zigpy](https://github.com/zigpy/zigpy)** is [Zigbee protocol stack](https://en.wikipedia.org/wiki/Zigbee) integration project to implement the **[Zigbee Home Automation](https://www.zigbee.org/)** standard as a Python library. Zigbee Home Automation integration with zigpy allows you to connect one of many off-the-shelf Zigbee adapters using one of the available Zigbee radio library modules compatible with zigpy to control Zigbee devices. There is currently support for controlling Zigbee device types such as binary sensors (e.g. motion and door sensors), analog sensors (e.g. temperature sensors), lightbulbs, switches, and fans. Zigpy is tightly integrated with [Home Assistant](https://www.home-assistant.io)'s [ZHA component](https://www.home-assistant.io/components/zha/) and provides a user-friendly interface for working with a Zigbee network.
```

### Comparing `zigpy-znp-0.9.2/README.md` & `zigpy-znp-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/api.py` & `zigpy-znp-0.9.3/zigpy_znp/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 import itertools
 import contextlib
 import dataclasses
 from collections import Counter, defaultdict
 
 import zigpy.state
 import async_timeout
+import pkg_resources
 import zigpy.zdo.types as zdo_t
 import zigpy.exceptions
 from zigpy.exceptions import NetworkNotFormed
 
-import zigpy_znp
 import zigpy_znp.const as const
 import zigpy_znp.types as t
 import zigpy_znp.config as conf
 import zigpy_znp.logger as log
 import zigpy_znp.commands as c
 from zigpy_znp import uart
 from zigpy_znp.nvram import NVRAMHelper
@@ -132,17 +132,18 @@
         )
 
         nwk_frame_counter = await security.read_nwk_frame_counter(
             self, ext_pan_id=nib.extendedPANID
         )
 
         version = await self.request(c.SYS.Version.Req())
+        package_version = pkg_resources.get_distribution("zigpy_znp").version
 
         network_info = zigpy.state.NetworkInfo(
-            source=f"zigpy-znp@{zigpy_znp.__version__}",
+            source=f"zigpy-znp@{package_version}",
             extended_pan_id=nib.extendedPANID,
             pan_id=nib.nwkPanId,
             nwk_update_id=nib.nwkUpdateId,
             channel=nib.nwkLogicalChannel,
             channel_mask=nib.channelList,
             security_level=nib.SecurityLevel,
             network_key=zigpy.state.Key(
@@ -964,14 +965,17 @@
             raise ValueError(
                 f"Command has no response so response_params={response_params} "
                 f"will have no effect"
             )
 
         frame = request.to_frame(align=self.nvram.align_structs)
 
+        if self._uart is None:
+            raise RuntimeError("Coordinator is disconnected, cannot send request")
+
         # We should only be sending one SREQ at a time, according to the spec
         async with self._sync_request_lock:
             LOGGER.debug("Sending request: %s", request)
 
             # If our request has no response, we cannot wait for one
             if not request.Rsp:
                 LOGGER.debug("Request has no response, not waiting for one.")
```

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/__init__.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/af.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/af.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/app.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/app.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/app_config.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/app_config.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/mac.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/mac.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/rpc_error.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/rpc_error.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/sapi.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/sapi.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/sys.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/sys.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/ubl.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/ubl.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/util.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/util.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/zdo.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/zdo.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/zgp.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/zgp.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/commands/znp.py` & `zigpy-znp-0.9.3/zigpy_znp/commands/znp.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/config.py` & `zigpy-znp-0.9.3/zigpy_znp/config.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/const.py` & `zigpy-znp-0.9.3/zigpy_znp/const.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/frames.py` & `zigpy-znp-0.9.3/zigpy_znp/frames.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/logger.py` & `zigpy-znp-0.9.3/zigpy_znp/logger.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/nvram.py` & `zigpy-znp-0.9.3/zigpy_znp/nvram.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/tools/common.py` & `zigpy-znp-0.9.3/zigpy_znp/tools/common.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/tools/energy_scan.py` & `zigpy-znp-0.9.3/zigpy_znp/tools/energy_scan.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/tools/flash_read.py` & `zigpy-znp-0.9.3/zigpy_znp/tools/flash_read.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/tools/flash_write.py` & `zigpy-znp-0.9.3/zigpy_znp/tools/flash_write.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/tools/network_backup.py` & `zigpy-znp-0.9.3/zigpy_znp/tools/network_backup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import sys
 import json
 import asyncio
 import logging
 import datetime
 
 import zigpy.state
+import pkg_resources
 
-import zigpy_znp
 import zigpy_znp.types as t
 from zigpy_znp.api import ZNP
 from zigpy_znp.tools.common import ClosableFileType, setup_parser, validate_backup_json
 from zigpy_znp.zigbee.application import ControllerApplication
 
 LOGGER = logging.getLogger(__name__)
 
@@ -80,15 +80,16 @@
     obj = zigpy_state_to_json_backup(
         network_info=znp.network_info,
         node_info=znp.node_info,
     )
 
     now = datetime.datetime.now().astimezone()
 
-    obj["metadata"]["source"] = f"zigpy-znp@{zigpy_znp.__version__}"
+    package_version = pkg_resources.get_distribution("zigpy_znp").version
+    obj["metadata"]["source"] = f"zigpy-znp@{package_version}"
     obj["metadata"]["internal"] = {
         "creation_time": now.isoformat(timespec="seconds"),
         "zstack": {
             "version": znp.version,
         },
     }
```

### Comparing `zigpy-znp-0.9.2/zigpy_znp/tools/network_restore.py` & `zigpy-znp-0.9.3/zigpy_znp/tools/network_restore.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/tools/network_scan.py` & `zigpy-znp-0.9.3/zigpy_znp/tools/network_scan.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/tools/nvram_read.py` & `zigpy-znp-0.9.3/zigpy_znp/tools/nvram_read.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/tools/nvram_reset.py` & `zigpy-znp-0.9.3/zigpy_znp/tools/nvram_reset.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/tools/nvram_write.py` & `zigpy-znp-0.9.3/zigpy_znp/tools/nvram_write.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/types/basic.py` & `zigpy-znp-0.9.3/zigpy_znp/types/basic.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/types/commands.py` & `zigpy-znp-0.9.3/zigpy_znp/types/commands.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/types/cstruct.py` & `zigpy-znp-0.9.3/zigpy_znp/types/cstruct.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/types/named.py` & `zigpy-znp-0.9.3/zigpy_znp/types/named.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/types/nvids.py` & `zigpy-znp-0.9.3/zigpy_znp/types/nvids.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/types/structs.py` & `zigpy-znp-0.9.3/zigpy_znp/types/structs.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/uart.py` & `zigpy-znp-0.9.3/zigpy_znp/uart.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/utils.py` & `zigpy-znp-0.9.3/zigpy_znp/utils.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/zigbee/application.py` & `zigpy-znp-0.9.3/zigpy_znp/zigbee/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import zigpy.types
 import zigpy.config
 import zigpy.device
 import async_timeout
 import zigpy.profiles
 import zigpy.zdo.types as zdo_t
 import zigpy.application
+import zigpy.config.defaults
 from zigpy.exceptions import DeliveryError
 
 import zigpy_znp.const as const
 import zigpy_znp.types as t
 import zigpy_znp.config as conf
 import zigpy_znp.commands as c
 from zigpy_znp.api import ZNP
@@ -179,15 +180,15 @@
         """
 
         network_info.stack_specific.setdefault("zstack", {})
 
         if "tclk_seed" not in network_info.stack_specific["zstack"]:
             network_info.stack_specific["zstack"]["tclk_seed"] = os.urandom(16).hex()
 
-        return await self._znp.write_network_info(
+        await self._znp.write_network_info(
             network_info=network_info, node_info=node_info
         )
 
     async def start_network(self, *, read_only=False):
         if self.state.node_info == zigpy.state.NodeInfo():
             await self.load_network_info()
 
@@ -224,15 +225,18 @@
         if self.znp_config[conf.CONF_MAX_CONCURRENT_REQUESTS] is not None:
             raise RuntimeError(
                 "`zigpy_config:znp_config:max_concurrent_requests` is deprecated,"
                 " move this key up to `zigpy_config:max_concurrent_requests` instead."
             )
 
         # Now that we know what device we are, set the max concurrent requests
-        if self._config[conf.CONF_MAX_CONCURRENT_REQUESTS] is None:
+        if self._config[conf.CONF_MAX_CONCURRENT_REQUESTS] in (
+            None,
+            zigpy.config.defaults.CONF_MAX_CONCURRENT_REQUESTS_DEFAULT,
+        ):
             max_concurrent_requests = 16 if self._znp.nvram.align_structs else 2
         else:
             max_concurrent_requests = self._config[conf.CONF_MAX_CONCURRENT_REQUESTS]
 
         # Update the max value of the concurrent request semaphore at runtime
         self._concurrent_requests_semaphore.max_value = max_concurrent_requests
 
@@ -831,14 +835,17 @@
                 TSN=sequence,
                 Options=options,
                 Radius=radius,
                 SourceRoute=relays,  # force the packet to go through specific parents
                 Data=data,
             )
 
+        if self._znp is None:
+            raise DeliveryError("Coordinator is disconnected, cannot send request")
+
         # Z-Stack requires special treatment when sending ZDO requests
         if dst_ep == ZDO_ENDPOINT:
             # XXX: Joins *must* be sent via a ZDO command, even if they are directly
             # addressing another device. The router will receive the ZDO request and a
             # device will try to join, but Z-Stack will never send the network key.
             if cluster == zdo_t.ZDOCmd.Mgmt_Permit_Joining_req:
                 if dst_addr.mode == t.AddrMode.Broadcast:
```

### Comparing `zigpy-znp-0.9.2/zigpy_znp/zigbee/device.py` & `zigpy-znp-0.9.3/zigpy_znp/zigbee/device.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp/znp/security.py` & `zigpy-znp-0.9.3/zigpy_znp/znp/security.py`

 * *Files identical despite different names*

### Comparing `zigpy-znp-0.9.2/zigpy_znp.egg-info/PKG-INFO` & `zigpy-znp-0.9.3/zigpy_znp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,175 +1,174 @@
 Metadata-Version: 2.1
 Name: zigpy-znp
-Version: 0.9.2
+Version: 0.9.3
 Summary: A library for zigpy which communicates with TI ZNP radios
-Home-page: https://github.com/zigpy/zigpy-znp
-Author: Alexei Chetroi
-Author-email: alexei.chetroi@outlook.com
+Author-email: Alexei Chetroi <alexei.chetroi@outlook.com>
 License: GPL-3.0
-Description: # zigpy-znp
-        
-        [![Build Status](https://github.com/zigpy/zigpy-znp/workflows/CI/badge.svg)](https://github.com/zigpy/zigpy-znp/actions)
-        [![Coverage Status](https://codecov.io/gh/zigpy/zigpy-znp/branch/dev/graph/badge.svg?token=Y1994N9D74)](https://codecov.io/gh/zigpy/zigpy-znp)
-        
-        **[zigpy-znp](https://github.com/zigpy/zigpy-znp/)** is a Python library that adds support for common [Texas Instruments ZNP (Zigbee Network Processors)](http://dev.ti.com/tirex/content/simplelink_zigbee_sdk_plugin_2_20_00_06/docs/zigbee_user_guide/html/zigbee/introduction.html) [Zigbee](https://www.zigbee.org) radio modules to [zigpy](https://github.com/zigpy/), a Python Zigbee stack project.
-        
-        Together with zigpy and compatible home automation software (namely Home Assistant's [ZHA (Zigbee Home Automation) integration component](https://www.home-assistant.io/integrations/zha/)), you can directly control Zigbee devices such as Philips Hue, GE, OSRAM LIGHTIFY, Xiaomi/Aqara, IKEA Tradfri, Samsung SmartThings, and many more.
-        
-        # Installation
-        
-        ## Python module
-        Install the Python module within your virtual environment:
-        
-        ```console
-        $ virtualenv -p python3.8 venv                                # if you don't already have one
-        $ source venv/bin/activate
-        (venv) $ pip install git+https://github.com/zigpy/zigpy-znp/  # latest commit from Git
-        (venv) $ pip install zigpy-znp                                # or, latest stable from PyPI
-        ```
-        
-        ## Home Assistant
-        Stable releases of zigpy-znp are automatically installed when you install the ZHA component.
-        
-        ### Testing `dev` with Home Assistant Core
-        
-        Upgrade the package within your virtual environment (requires `git`):
-        
-        ```console
-        (venv) $ pip install git+https://github.com/zigpy/zigpy-znp/
-        ```
-        
-        Launch Home Assistant with the `--skip-pip` command line option to prevent zigpy-znp from being downgraded. Running with this option may prevent newly added integrations from installing required packages.
-        
-        ### Testing `dev` with Home Assistant OS
-        
-         - Add https://github.com/home-assistant/hassio-addons-development as an addon repository.
-         - Install the "Custom deps deployment" addon.
-         - Add the following to your `configuration.yaml` file:
-           ```yaml
-           apk: []
-           pypi:
-             - git+https://github.com/zigpy/zigpy-znp/
-        	 ```
-        
-        # Configuration
-        Below are the defaults with the top-level Home Assistant `zha:` key.
-        **You do not need to copy this configuration, it is provided only for reference**:
-        
-        ```yaml
-        zha:
-          zigpy_config:
-            znp_config:
-              # Only if your stick has a built-in power amplifier (i.e. CC1352P and CC2592)
-              # If set, must be between:
-              #  * CC1352/2652:  -22 and 19
-              #  * CC253x:       -22 and 22
-              tx_power:  
-        
-              # Only if your stick has a controllable LED (the CC2531)
-              # If set, must be one of: off, on, blink, flash, toggle
-              led_mode: off
-        
-        
-              ### Internal configuration, there's no reason to touch these values
-        
-              # Skips the 60s bootloader delay on CC2531 sticks
-              skip_bootloader: True
-        
-              # Timeout for synchronous requests' responses
-              sreq_timeout: 15
-        
-              # Timeout for asynchronous requests' callback responses
-              arsp_timeout: 30
-        
-              # Delay between auto-reconnect attempts in case the device gets disconnected
-              auto_reconnect_retry_delay: 5
-        
-              # Pin states for skipping the bootloader
-              connect_rts_pin_states: [off, on, off]
-              connect_dtr_pin_states: [off, off, off]
-        ```
-        
-        # Tools
-        Various command line Zigbee utilities are a part of the zigpy-znp package and can be run
-        with `python -m zigpy_znp.tools.name_of_tool`. More detailed documentation can be found
-        in **[`TOOLS.md`](./TOOLS.md)** but a brief description of each tool is included below:
-        
-         - **`energy_scan`**: Performs a continuous energy scan to check for non-Zigbee interference.
-         - **`flash_read`**: For CC2531s, reads firmware from flash.
-         - **`flash_write`**: For CC2531s, writes a firmware `.bin` to flash.
-         - **`form_network`**: Forms a network with randomized settings on channel 15.
-         - **`network_backup`**: Backs up the network data and device information into a human-readable JSON document.
-         - **`network_restore`**: Restores a JSON network backup to the adapter.
-         - **`network_scan`**: Actively sends beacon requests for network stumbling.
-         - **`nvram_read`**: Reads all possible NVRAM entries into a JSON document.
-         - **`nvram_reset`**: Deletes all possible NVRAM entries
-         - **`nvram_write`**: Writes all NVRAM entries from a JSON document.
-        
-        # Hardware requirements
-        USB-adapters, GPIO-modules, and development-boards flashed with TI's Z-Stack are compatible with zigpy-znp:
-        
-         - CC2652P/CC2652R/CC2652RB USB stick and dev board hardware
-         - CC1352P/CC1352R USB stick and dev board hardware
-         - CC2538 + CC2592 USB stick and dev board hardware (**not recommended, old hardware and end-of-life firmware**)
-         - CC2531 USB stick hardware (**not recommended for Zigbee networks with more than 20 devices**)
-         - CC2530 + CC2591/CC2592 USB stick hardware (**not recommended for Zigbee networks with more than 20 devices**)
-        
-        Tip! Adapters listed as "[Texas Instruments sticks compatible with Zigbee2MQTT](https://www.zigbee2mqtt.io/information/supported_adapters)" also works with zigpy-znp.
-        
-        ## Reference hardware for this project
-        These specific adapters are used as reference hardware for development and testing by zigpy-znp developers:
-        
-         - [TI LAUNCHXL-CC26X2R1](https://www.ti.com/tool/LAUNCHXL-CC26X2R1) running [Z-Stack 3 firmware (based on version 4.40.00.44)](https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0/bin). You can flash `CC2652R_20210120.hex` using [TI's UNIFLASH](https://www.ti.com/tool/download/UNIFLASH).
-         - [Electrolama zzh CC2652R](https://electrolama.com/projects/zig-a-zig-ah/) and [Slaesh CC2652R](https://slae.sh/projects/cc2652/) sticks running [Z-Stack 3 firmware (based on version 4.40.00.44)](https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0/bin). You can flash `CC2652R_20210120.hex` or `CC2652RB_20210120.hex` respectively using [cc2538-bsl](https://github.com/JelmerT/cc2538-bsl).
-         - CC2531 running [Z-Stack Home 1.2](https://github.com/Koenkk/Z-Stack-firmware/blob/master/coordinator/Z-Stack_Home_1.2/bin/default/CC2531_DEFAULT_20190608.zip). You can flash `CC2531ZNP-Prod.bin` to your stick directly with `zigpy_znp`: `python -m zigpy_znp.tools.flash_write -i /path/to/CC2531ZNP-Prod.bin /dev/serial/by-id/YOUR-CC2531` if your stick already has a serial bootloader.
-        
-        ## Texas Instruments Chip Part Numbers
-        Texas Instruments (TI) has quite a few different wireless MCU chips and they are all used/mentioned in open-source Zigbee world which can be daunting if you are just starting out. Here is a quick summary of part numbers and key features.
-        
-        ### Supported newer generation TI chips
-        
-        #### 2.4GHz frequency only chips
-        - CC2652R: 2.4GHz only wireless MCU for IEEE 802.15.4 multi-protocol (Zigbee, Bluetooth, Thread, IEEE 802.15.4g IPv6-enabled smart objects like 6LoWPAN, and proprietary systems). Cortex-M0 core for radio stack and Cortex-M4F core for application use, plenty of RAM. Free compiler option from TI.
-        - CC2652RB: Pin compatible "Crystal-less" CC2652R (so you could use it if you were to build your own zzh and omit the crystal) but not firmware compatible.
-        - CC2652P: CC2652R with a built-in RF PA. Not pin or firmware compatible with CC2652R/CC2652RB. 
-        
-        #### Multi frequency chips
-        - CC1352R: Sub 1 GHz & 2.4 GHz wireless MCU. Essentially CC2652R with an extra sub-1GHz radio.
-        - CC1352P: CC1352R with a built in RF PA.
-        
-        ### Supported older generation TI chips
-        - CC2538: 2.4GHz Zigbee, 6LoWPAN, and IEEE 802.15.4 wireless MCU. ARM Cortex-M3 core with with 512kB Flash and 32kB RAM.
-        - CC2531: CC2530 with a built-in UART/TTL to USB Bridge. Used in the cheap "Zigbee sticks" sold everywhere. Intel 8051 core, 256 Flash, only has 8kB RAM.
-        - CC2530: 2.4GHz Zigbee and IEEE 802.15.4 wireless MCU. Intel 8051 core, 256 Flash, only has 8kB RAM.
-        
-        ### Auxiliary TI chips
-        - CC2591 and CC2592: 2.4 GHz range extenders. These are not wireless MCUs, just auxiliary PA (Power Amplifier) and LNA (Low Noise Amplifier) in the same package to improve RF (Radio Frequency) range of any 2.4 GHz radio chip.
-        
-        # Releases via PyPI
-        
-        Tagged versions will also be released via PyPI
-        
-         - https://pypi.org/project/zigpy-znp/
-         - https://pypi.org/project/zigpy-znp/#history
-         - https://pypi.org/project/zigpy-znp/#files
-        
-        # External documentation and reference
-        
-        - http://www.ti.com/tool/LAUNCHXL-CC26X2R1
-        - http://www.ti.com/tool/LAUNCHXL-CC1352P
-        
-        # How to contribute
-        
-        If you are looking to make a code or documentation contribution to this project we suggest that you follow the steps in these guides:
-        - https://github.com/firstcontributions/first-contributions/blob/master/README.md
-        - https://github.com/firstcontributions/first-contributions/blob/master/github-desktop-tutorial.md
-        
-        # Related projects
-        
-        ### Zigpy
-        **[zigpy](https://github.com/zigpy/zigpy)** is [Zigbee protocol stack](https://en.wikipedia.org/wiki/Zigbee) integration project to implement the **[Zigbee Home Automation](https://www.zigbee.org/)** standard as a Python library. Zigbee Home Automation integration with zigpy allows you to connect one of many off-the-shelf Zigbee adapters using one of the available Zigbee radio library modules compatible with zigpy to control Zigbee devices. There is currently support for controlling Zigbee device types such as binary sensors (e.g. motion and door sensors), analog sensors (e.g. temperature sensors), lightbulbs, switches, and fans. Zigpy is tightly integrated with [Home Assistant](https://www.home-assistant.io)'s [ZHA component](https://www.home-assistant.io/components/zha/) and provides a user-friendly interface for working with a Zigbee network.
-        
-Platform: UNKNOWN
+Project-URL: repository, https://github.com/zigpy/zigpy-znp
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
+Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+
+# zigpy-znp
+
+[![Build Status](https://github.com/zigpy/zigpy-znp/workflows/CI/badge.svg)](https://github.com/zigpy/zigpy-znp/actions)
+[![Coverage Status](https://codecov.io/gh/zigpy/zigpy-znp/branch/dev/graph/badge.svg?token=Y1994N9D74)](https://codecov.io/gh/zigpy/zigpy-znp)
+
+**[zigpy-znp](https://github.com/zigpy/zigpy-znp/)** is a Python library that adds support for common [Texas Instruments ZNP (Zigbee Network Processors)](http://dev.ti.com/tirex/content/simplelink_zigbee_sdk_plugin_2_20_00_06/docs/zigbee_user_guide/html/zigbee/introduction.html) [Zigbee](https://www.zigbee.org) radio modules to [zigpy](https://github.com/zigpy/), a Python Zigbee stack project.
+
+Together with zigpy and compatible home automation software (namely Home Assistant's [ZHA (Zigbee Home Automation) integration component](https://www.home-assistant.io/integrations/zha/)), you can directly control Zigbee devices such as Philips Hue, GE, OSRAM LIGHTIFY, Xiaomi/Aqara, IKEA Tradfri, Samsung SmartThings, and many more.
+
+# Installation
+
+## Python module
+Install the Python module within your virtual environment:
+
+```console
+$ virtualenv -p python3.8 venv                                # if you don't already have one
+$ source venv/bin/activate
+(venv) $ pip install git+https://github.com/zigpy/zigpy-znp/  # latest commit from Git
+(venv) $ pip install zigpy-znp                                # or, latest stable from PyPI
+```
+
+## Home Assistant
+Stable releases of zigpy-znp are automatically installed when you install the ZHA component.
+
+### Testing `dev` with Home Assistant Core
+
+Upgrade the package within your virtual environment (requires `git`):
+
+```console
+(venv) $ pip install git+https://github.com/zigpy/zigpy-znp/
+```
+
+Launch Home Assistant with the `--skip-pip` command line option to prevent zigpy-znp from being downgraded. Running with this option may prevent newly added integrations from installing required packages.
+
+### Testing `dev` with Home Assistant OS
+
+ - Add https://github.com/home-assistant/hassio-addons-development as an addon repository.
+ - Install the "Custom deps deployment" addon.
+ - Add the following to your `configuration.yaml` file:
+   ```yaml
+   apk: []
+   pypi:
+     - git+https://github.com/zigpy/zigpy-znp/
+	 ```
+
+# Configuration
+Below are the defaults with the top-level Home Assistant `zha:` key.
+**You do not need to copy this configuration, it is provided only for reference**:
+
+```yaml
+zha:
+  zigpy_config:
+    znp_config:
+      # Only if your stick has a built-in power amplifier (i.e. CC1352P and CC2592)
+      # If set, must be between:
+      #  * CC1352/2652:  -22 and 19
+      #  * CC253x:       -22 and 22
+      tx_power:  
+
+      # Only if your stick has a controllable LED (the CC2531)
+      # If set, must be one of: off, on, blink, flash, toggle
+      led_mode: off
+
+
+      ### Internal configuration, there's no reason to touch these values
+
+      # Skips the 60s bootloader delay on CC2531 sticks
+      skip_bootloader: True
+
+      # Timeout for synchronous requests' responses
+      sreq_timeout: 15
+
+      # Timeout for asynchronous requests' callback responses
+      arsp_timeout: 30
+
+      # Delay between auto-reconnect attempts in case the device gets disconnected
+      auto_reconnect_retry_delay: 5
+
+      # Pin states for skipping the bootloader
+      connect_rts_pin_states: [off, on, off]
+      connect_dtr_pin_states: [off, off, off]
+```
+
+# Tools
+Various command line Zigbee utilities are a part of the zigpy-znp package and can be run
+with `python -m zigpy_znp.tools.name_of_tool`. More detailed documentation can be found
+in **[`TOOLS.md`](./TOOLS.md)** but a brief description of each tool is included below:
+
+ - **`energy_scan`**: Performs a continuous energy scan to check for non-Zigbee interference.
+ - **`flash_read`**: For CC2531s, reads firmware from flash.
+ - **`flash_write`**: For CC2531s, writes a firmware `.bin` to flash.
+ - **`form_network`**: Forms a network with randomized settings on channel 15.
+ - **`network_backup`**: Backs up the network data and device information into a human-readable JSON document.
+ - **`network_restore`**: Restores a JSON network backup to the adapter.
+ - **`network_scan`**: Actively sends beacon requests for network stumbling.
+ - **`nvram_read`**: Reads all possible NVRAM entries into a JSON document.
+ - **`nvram_reset`**: Deletes all possible NVRAM entries
+ - **`nvram_write`**: Writes all NVRAM entries from a JSON document.
+
+# Hardware requirements
+USB-adapters, GPIO-modules, and development-boards flashed with TI's Z-Stack are compatible with zigpy-znp:
+
+ - CC2652P/CC2652R/CC2652RB USB stick and dev board hardware
+ - CC1352P/CC1352R USB stick and dev board hardware
+ - CC2538 + CC2592 USB stick and dev board hardware (**not recommended, old hardware and end-of-life firmware**)
+ - CC2531 USB stick hardware (**not recommended for Zigbee networks with more than 20 devices**)
+ - CC2530 + CC2591/CC2592 USB stick hardware (**not recommended for Zigbee networks with more than 20 devices**)
+
+Tip! Adapters listed as "[Texas Instruments sticks compatible with Zigbee2MQTT](https://www.zigbee2mqtt.io/information/supported_adapters)" also works with zigpy-znp.
+
+## Reference hardware for this project
+These specific adapters are used as reference hardware for development and testing by zigpy-znp developers:
+
+ - [TI LAUNCHXL-CC26X2R1](https://www.ti.com/tool/LAUNCHXL-CC26X2R1) running [Z-Stack 3 firmware (based on version 4.40.00.44)](https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0/bin). You can flash `CC2652R_20210120.hex` using [TI's UNIFLASH](https://www.ti.com/tool/download/UNIFLASH).
+ - [Electrolama zzh CC2652R](https://electrolama.com/projects/zig-a-zig-ah/) and [Slaesh CC2652R](https://slae.sh/projects/cc2652/) sticks running [Z-Stack 3 firmware (based on version 4.40.00.44)](https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0/bin). You can flash `CC2652R_20210120.hex` or `CC2652RB_20210120.hex` respectively using [cc2538-bsl](https://github.com/JelmerT/cc2538-bsl).
+ - CC2531 running [Z-Stack Home 1.2](https://github.com/Koenkk/Z-Stack-firmware/blob/master/coordinator/Z-Stack_Home_1.2/bin/default/CC2531_DEFAULT_20190608.zip). You can flash `CC2531ZNP-Prod.bin` to your stick directly with `zigpy_znp`: `python -m zigpy_znp.tools.flash_write -i /path/to/CC2531ZNP-Prod.bin /dev/serial/by-id/YOUR-CC2531` if your stick already has a serial bootloader.
+
+## Texas Instruments Chip Part Numbers
+Texas Instruments (TI) has quite a few different wireless MCU chips and they are all used/mentioned in open-source Zigbee world which can be daunting if you are just starting out. Here is a quick summary of part numbers and key features.
+
+### Supported newer generation TI chips
+
+#### 2.4GHz frequency only chips
+- CC2652R: 2.4GHz only wireless MCU for IEEE 802.15.4 multi-protocol (Zigbee, Bluetooth, Thread, IEEE 802.15.4g IPv6-enabled smart objects like 6LoWPAN, and proprietary systems). Cortex-M0 core for radio stack and Cortex-M4F core for application use, plenty of RAM. Free compiler option from TI.
+- CC2652RB: Pin compatible "Crystal-less" CC2652R (so you could use it if you were to build your own zzh and omit the crystal) but not firmware compatible.
+- CC2652P: CC2652R with a built-in RF PA. Not pin or firmware compatible with CC2652R/CC2652RB. 
+
+#### Multi frequency chips
+- CC1352R: Sub 1 GHz & 2.4 GHz wireless MCU. Essentially CC2652R with an extra sub-1GHz radio.
+- CC1352P: CC1352R with a built in RF PA.
+
+### Supported older generation TI chips
+- CC2538: 2.4GHz Zigbee, 6LoWPAN, and IEEE 802.15.4 wireless MCU. ARM Cortex-M3 core with with 512kB Flash and 32kB RAM.
+- CC2531: CC2530 with a built-in UART/TTL to USB Bridge. Used in the cheap "Zigbee sticks" sold everywhere. Intel 8051 core, 256 Flash, only has 8kB RAM.
+- CC2530: 2.4GHz Zigbee and IEEE 802.15.4 wireless MCU. Intel 8051 core, 256 Flash, only has 8kB RAM.
+
+### Auxiliary TI chips
+- CC2591 and CC2592: 2.4 GHz range extenders. These are not wireless MCUs, just auxiliary PA (Power Amplifier) and LNA (Low Noise Amplifier) in the same package to improve RF (Radio Frequency) range of any 2.4 GHz radio chip.
+
+# Releases via PyPI
+
+Tagged versions will also be released via PyPI
+
+ - https://pypi.org/project/zigpy-znp/
+ - https://pypi.org/project/zigpy-znp/#history
+ - https://pypi.org/project/zigpy-znp/#files
+
+# External documentation and reference
+
+- http://www.ti.com/tool/LAUNCHXL-CC26X2R1
+- http://www.ti.com/tool/LAUNCHXL-CC1352P
+
+# How to contribute
+
+If you are looking to make a code or documentation contribution to this project we suggest that you follow the steps in these guides:
+- https://github.com/firstcontributions/first-contributions/blob/master/README.md
+- https://github.com/firstcontributions/first-contributions/blob/master/github-desktop-tutorial.md
+
+# Related projects
+
+### Zigpy
+**[zigpy](https://github.com/zigpy/zigpy)** is [Zigbee protocol stack](https://en.wikipedia.org/wiki/Zigbee) integration project to implement the **[Zigbee Home Automation](https://www.zigbee.org/)** standard as a Python library. Zigbee Home Automation integration with zigpy allows you to connect one of many off-the-shelf Zigbee adapters using one of the available Zigbee radio library modules compatible with zigpy to control Zigbee devices. There is currently support for controlling Zigbee device types such as binary sensors (e.g. motion and door sensors), analog sensors (e.g. temperature sensors), lightbulbs, switches, and fans. Zigpy is tightly integrated with [Home Assistant](https://www.home-assistant.io)'s [ZHA component](https://www.home-assistant.io/components/zha/) and provides a user-friendly interface for working with a Zigbee network.
```

