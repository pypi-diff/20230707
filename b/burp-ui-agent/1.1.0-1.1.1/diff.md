# Comparing `tmp/burp-ui-agent-1.1.0.tar.gz` & `tmp/burp-ui-agent-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burp-ui-agent-1.1.0.tar", last modified: Mon May  1 19:46:47 2023, max compression
+gzip compressed data, was "burp-ui-agent-1.1.1.tar", last modified: Fri Jul  7 18:25:04 2023, max compression
```

## Comparing `burp-ui-agent-1.1.0.tar` & `burp-ui-agent-1.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/
--rw-r--r--   0 master    (1000) master    (1000)      152 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/MANIFEST.in
--rw-r--r--   0 master    (1000) master    (1000)      776 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/PKG-INFO
--rw-r--r--   0 master    (1000) master    (1000)       44 2017-05-09 16:54:40.000000 burp-ui-agent-1.1.0/README
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.401666 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/
--rw-r--r--   0 master    (1000) master    (1000)      776 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/PKG-INFO
--rw-r--r--   0 master    (1000) master    (1000)     1941 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/SOURCES.txt
--rw-r--r--   0 master    (1000) master    (1000)        1 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/dependency_links.txt
--rw-r--r--   0 master    (1000) master    (1000)       59 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/entry_points.txt
--rw-r--r--   0 master    (1000) master    (1000)       74 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/requires.txt
--rw-r--r--   0 master    (1000) master    (1000)       13 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burp_ui_agent.egg-info/top_level.txt
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.401666 burp-ui-agent-1.1.0/burpui_agent/
--rw-r--r--   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/RELEASE
--rw-r--r--   0 master    (1000) master    (1000)        6 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/VERSION
--rw-r--r--   0 master    (1000) master    (1000)      278 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)     2648 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/__main__.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.417666 burp-ui-agent-1.1.0/burpui_agent/__pycache__/
--rw-r--r--   0 master    (1000) master    (1000)      421 2021-05-14 20:26:36.000000 burp-ui-agent-1.1.0/burpui_agent/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 master    (1000) master    (1000)      429 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 master    (1000) master    (1000)      994 2021-05-14 20:26:36.000000 burp-ui-agent-1.1.0/burpui_agent/__pycache__/desc.cpython-36.pyc
--rw-r--r--   0 master    (1000) master    (1000)     1008 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/__pycache__/desc.cpython-39.pyc
--rw-r--r--   0 master    (1000) master    (1000)     2058 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/_compat.py
--rw-r--r--   0 master    (1000) master    (1000)     1202 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/_json.py
--rw-r--r--   0 master    (1000) master    (1000)    10045 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/config.py
--rw-r--r--   0 master    (1000) master    (1000)    23767 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/datastructures.py
--rw-r--r--   0 master    (1000) master    (1000)     2768 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/decorators.py
--rw-r--r--   0 master    (1000) master    (1000)      964 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/desc.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.417666 burp-ui-agent-1.1.0/burpui_agent/engines/
--rw-r--r--   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/engines/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    14171 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/engines/agent.py
--rw-r--r--   0 master    (1000) master    (1000)      871 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/exceptions.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.417666 burp-ui-agent-1.1.0/burpui_agent/misc/
--rw-r--r--   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/misc/__init__.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.417666 burp-ui-agent-1.1.0/burpui_agent/misc/backend/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)     1168 2020-05-08 22:06:12.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-18 09:19:37.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2020-05-08 22:06:12.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    47346 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/burp1.py
--rw-r--r--   0 master    (1000) master    (1000)    30620 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)    41267 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/interface.py
--rw-r--r--   0 master    (1000) master    (1000)    23472 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/multi.py
--rw-r--r--   0 master    (1000) master    (1000)    38354 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/parallel.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/burpui_agent/misc/backend/utils/
--rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/utils/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    12735 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/utils/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)      398 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/burpui_agent/misc/backend/utils/constant.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/burpui_agent/misc/parser/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 12:38:25.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      431 2021-10-04 08:39:12.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-03 09:34:38.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2021-10-04 08:39:12.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    37464 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/burp1.py
--rw-r--r--   0 master    (1000) master    (1000)    13883 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)    43592 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/doc.py
--rw-r--r--   0 master    (1000) master    (1000)    17679 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/interface.py
--rw-r--r--   0 master    (1000) master    (1000)     8075 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/openssl.py
--rw-r--r--   0 master    (1000) master    (1000)    57165 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/burpui_agent/misc/parser/utils.py
--rw-r--r--   0 master    (1000) master    (1000)     2913 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/security.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/burpui_agent/tools/
--rw-r--r--   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/tools/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)     3289 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/tools/logging.py
--rw-r--r--   0 master    (1000) master    (1000)     8182 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/burpui_agent/utils.py
--rw-r--r--   0 master    (1000) master    (1000)       73 2023-05-01 19:46:47.000000 burp-ui-agent-1.1.0/requirements.txt
--rw-r--r--   0 master    (1000) master    (1000)       38 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/setup.cfg
--rwxr-xr-x   0 master    (1000) master    (1000)     5429 2023-05-01 18:42:40.000000 burp-ui-agent-1.1.0/setup.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.393665 burp-ui-agent-1.1.0/share/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.393665 burp-ui-agent-1.1.0/share/burpui/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:46:47.421666 burp-ui-agent-1.1.0/share/burpui/etc/
--rw-r--r--   0 master    (1000) master    (1000)     2912 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.0/share/burpui/etc/buiagent.sample.cfg
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.284256 burp-ui-agent-1.1.1/
+-rw-r--r--   0 master    (1000) master    (1000)      152 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.1/MANIFEST.in
+-rw-r--r--   0 master    (1000) master    (1000)      776 2023-07-07 18:25:04.284256 burp-ui-agent-1.1.1/PKG-INFO
+-rw-r--r--   0 master    (1000) master    (1000)       44 2017-05-09 16:54:40.000000 burp-ui-agent-1.1.1/README
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.268256 burp-ui-agent-1.1.1/burp_ui_agent.egg-info/
+-rw-r--r--   0 master    (1000) master    (1000)      776 2023-07-07 18:25:04.000000 burp-ui-agent-1.1.1/burp_ui_agent.egg-info/PKG-INFO
+-rw-r--r--   0 master    (1000) master    (1000)     1941 2023-07-07 18:25:04.000000 burp-ui-agent-1.1.1/burp_ui_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 master    (1000) master    (1000)        1 2023-07-07 18:25:04.000000 burp-ui-agent-1.1.1/burp_ui_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 master    (1000) master    (1000)       59 2023-07-07 18:25:04.000000 burp-ui-agent-1.1.1/burp_ui_agent.egg-info/entry_points.txt
+-rw-r--r--   0 master    (1000) master    (1000)       74 2023-07-07 18:25:04.000000 burp-ui-agent-1.1.1/burp_ui_agent.egg-info/requires.txt
+-rw-r--r--   0 master    (1000) master    (1000)       13 2023-07-07 18:25:04.000000 burp-ui-agent-1.1.1/burp_ui_agent.egg-info/top_level.txt
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.272256 burp-ui-agent-1.1.1/burpui_agent/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/RELEASE
+-rw-r--r--   0 master    (1000) master    (1000)        6 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/VERSION
+-rw-r--r--   0 master    (1000) master    (1000)      278 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)     2648 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/__main__.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.276256 burp-ui-agent-1.1.1/burpui_agent/__pycache__/
+-rw-r--r--   0 master    (1000) master    (1000)      421 2021-05-14 20:26:36.000000 burp-ui-agent-1.1.1/burpui_agent/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 master    (1000) master    (1000)      429 2023-07-07 18:25:04.000000 burp-ui-agent-1.1.1/burpui_agent/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 master    (1000) master    (1000)      994 2021-05-14 20:26:36.000000 burp-ui-agent-1.1.1/burpui_agent/__pycache__/desc.cpython-36.pyc
+-rw-r--r--   0 master    (1000) master    (1000)     1008 2023-07-07 18:25:04.000000 burp-ui-agent-1.1.1/burpui_agent/__pycache__/desc.cpython-39.pyc
+-rw-r--r--   0 master    (1000) master    (1000)     2058 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/_compat.py
+-rw-r--r--   0 master    (1000) master    (1000)     1202 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/_json.py
+-rw-r--r--   0 master    (1000) master    (1000)    10045 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/config.py
+-rw-r--r--   0 master    (1000) master    (1000)    23767 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/datastructures.py
+-rw-r--r--   0 master    (1000) master    (1000)     2768 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/decorators.py
+-rw-r--r--   0 master    (1000) master    (1000)      964 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/desc.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.276256 burp-ui-agent-1.1.1/burpui_agent/engines/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.000000 burp-ui-agent-1.1.1/burpui_agent/engines/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    14171 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/engines/agent.py
+-rw-r--r--   0 master    (1000) master    (1000)      871 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/exceptions.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.276256 burp-ui-agent-1.1.1/burpui_agent/misc/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.000000 burp-ui-agent-1.1.1/burpui_agent/misc/__init__.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.280256 burp-ui-agent-1.1.1/burpui_agent/misc/backend/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.280256 burp-ui-agent-1.1.1/burpui_agent/misc/backend/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)     1168 2020-05-08 22:06:12.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-18 09:19:37.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2020-05-08 22:06:12.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    47346 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/burp1.py
+-rw-r--r--   0 master    (1000) master    (1000)    30620 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)    41267 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)    23472 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/multi.py
+-rw-r--r--   0 master    (1000) master    (1000)    38354 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/parallel.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.280256 burp-ui-agent-1.1.1/burpui_agent/misc/backend/utils/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/utils/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    12735 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/utils/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)      398 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.1/burpui_agent/misc/backend/utils/constant.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.280256 burp-ui-agent-1.1.1/burpui_agent/misc/parser/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.280256 burp-ui-agent-1.1.1/burpui_agent/misc/parser/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 12:38:25.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      431 2021-10-04 08:39:12.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-03 09:34:38.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2021-10-04 08:39:12.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    37464 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/burp1.py
+-rw-r--r--   0 master    (1000) master    (1000)    13883 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)    43592 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/doc.py
+-rw-r--r--   0 master    (1000) master    (1000)    17679 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)     8075 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/openssl.py
+-rw-r--r--   0 master    (1000) master    (1000)    57165 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/burpui_agent/misc/parser/utils.py
+-rw-r--r--   0 master    (1000) master    (1000)     2913 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/security.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.280256 burp-ui-agent-1.1.1/burpui_agent/tools/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/tools/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)     3289 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/tools/logging.py
+-rw-r--r--   0 master    (1000) master    (1000)     8182 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/burpui_agent/utils.py
+-rw-r--r--   0 master    (1000) master    (1000)       73 2023-07-07 18:25:03.000000 burp-ui-agent-1.1.1/requirements.txt
+-rw-r--r--   0 master    (1000) master    (1000)       38 2023-07-07 18:25:04.284256 burp-ui-agent-1.1.1/setup.cfg
+-rwxr-xr-x   0 master    (1000) master    (1000)     5429 2023-07-07 18:23:10.000000 burp-ui-agent-1.1.1/setup.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.256255 burp-ui-agent-1.1.1/share/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.256255 burp-ui-agent-1.1.1/share/burpui/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-07-07 18:25:04.280256 burp-ui-agent-1.1.1/share/burpui/etc/
+-rw-r--r--   0 master    (1000) master    (1000)     2912 2022-11-06 21:20:42.000000 burp-ui-agent-1.1.1/share/burpui/etc/buiagent.sample.cfg
```

### Comparing `burp-ui-agent-1.1.0/PKG-INFO` & `burp-ui-agent-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burp-ui-agent
-Version: 1.1.0
+Version: 1.1.1
 Summary: Burp-UI is a web-ui for burp backup written in python with Flask and jQuery/Bootstrap
 Home-page: https://git.ziirish.me/ziirish/burp-ui
 Author: Benjamin SANS (Ziirish)
 Author-email: hi+burpui@ziirish.me
 License: BSD 3-clause
 Keywords: burp web ui backup monitoring
 Platform: UNKNOWN
```

### Comparing `burp-ui-agent-1.1.0/burp_ui_agent.egg-info/PKG-INFO` & `burp-ui-agent-1.1.1/burp_ui_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burp-ui-agent
-Version: 1.1.0
+Version: 1.1.1
 Summary: Burp-UI is a web-ui for burp backup written in python with Flask and jQuery/Bootstrap
 Home-page: https://git.ziirish.me/ziirish/burp-ui
 Author: Benjamin SANS (Ziirish)
 Author-email: hi+burpui@ziirish.me
 License: BSD 3-clause
 Keywords: burp web ui backup monitoring
 Platform: UNKNOWN
```

### Comparing `burp-ui-agent-1.1.0/burp_ui_agent.egg-info/SOURCES.txt` & `burp-ui-agent-1.1.1/burp_ui_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/__main__.py` & `burp-ui-agent-1.1.1/burpui_agent/__main__.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/__pycache__/desc.cpython-36.pyc` & `burp-ui-agent-1.1.1/burpui_agent/__pycache__/desc.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/__pycache__/desc.cpython-39.pyc` & `burp-ui-agent-1.1.1/burpui_agent/__pycache__/desc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon May  1 19:46:47 2023 UTC, .py size: 964 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2717 5064 c403 0000  a.......'.Pd....
+00000000: 610d 0d0a 0000 0000 7f58 a864 c403 0000  a........X.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6403 5a02 6404  Z.d.d.l.Z.d.Z.d.
 00000040: 5a03 6405 5a04 6406 5a05 6407 5a00 6408  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a06 6409 5a07 6508 6501 6a09 a00a 6501  Z.d.Z.e.e.j...e.
 00000060: 6a09 a00b 6501 6a09 a00c 650d a101 a101  j...e.j...e.....
 00000070: 640a a102 8301 a00e a100 a00f a100 5a10  d.............Z.
```

### Comparing `burp-ui-agent-1.1.0/burpui_agent/_compat.py` & `burp-ui-agent-1.1.1/burpui_agent/_compat.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/_json.py` & `burp-ui-agent-1.1.1/burpui_agent/_json.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/config.py` & `burp-ui-agent-1.1.1/burpui_agent/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/datastructures.py` & `burp-ui-agent-1.1.1/burpui_agent/datastructures.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/decorators.py` & `burp-ui-agent-1.1.1/burpui_agent/decorators.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/desc.py` & `burp-ui-agent-1.1.1/burpui_agent/desc.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/engines/agent.py` & `burp-ui-agent-1.1.1/burpui_agent/engines/agent.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/exceptions.py` & `burp-ui-agent-1.1.1/burpui_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/config.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/backend/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/backend/.ropeproject/globalnames` & `burp-ui-agent-1.1.1/burpui_agent/misc/backend/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/backend/burp1.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/backend/burp1.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/backend/burp2.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/backend/burp2.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/backend/interface.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/backend/interface.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/backend/multi.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/backend/multi.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/backend/parallel.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/backend/parallel.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/backend/utils/burp2.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/backend/utils/burp2.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/parser/.ropeproject/config.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/parser/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/parser/burp1.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/parser/burp1.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/parser/burp2.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/parser/burp2.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/parser/doc.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/parser/doc.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/parser/interface.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/parser/interface.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/parser/openssl.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/parser/openssl.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/misc/parser/utils.py` & `burp-ui-agent-1.1.1/burpui_agent/misc/parser/utils.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/security.py` & `burp-ui-agent-1.1.1/burpui_agent/security.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/tools/logging.py` & `burp-ui-agent-1.1.1/burpui_agent/tools/logging.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/burpui_agent/utils.py` & `burp-ui-agent-1.1.1/burpui_agent/utils.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/setup.py` & `burp-ui-agent-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `burp-ui-agent-1.1.0/share/burpui/etc/buiagent.sample.cfg` & `burp-ui-agent-1.1.1/share/burpui/etc/buiagent.sample.cfg`

 * *Files identical despite different names*

