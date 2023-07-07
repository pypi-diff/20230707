# Comparing `tmp/ldst_monitor-1.0.4.tar.gz` & `tmp/ldst_monitor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldst_monitor-1.0.4.tar", last modified: Fri Jul  7 03:36:17 2023, max compression
+gzip compressed data, was "ldst_monitor-1.0.5.tar", last modified: Fri Jul  7 03:54:56 2023, max compression
```

## Comparing `ldst_monitor-1.0.4.tar` & `ldst_monitor-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:36:17.806349 ldst_monitor-1.0.4/
--rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-07 03:36:17.805953 ldst_monitor-1.0.4/PKG-INFO
--rwxrwxrwx   0 happy     (1000) happy     (1000)      467 2023-07-07 03:36:05.000000 ldst_monitor-1.0.4/pyproject.toml
--rwxrwxrwx   0 happy     (1000) happy     (1000)       38 2023-07-07 03:36:17.806501 ldst_monitor-1.0.4/setup.cfg
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:36:17.793498 ldst_monitor-1.0.4/src/
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:36:17.798955 ldst_monitor-1.0.4/src/ldst_monitor/
--rwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 14:33:12.000000 ldst_monitor-1.0.4/src/ldst_monitor/__init__.py
--rwxrwxrwx   0 happy     (1000) happy     (1000)     1321 2023-07-06 14:55:29.000000 ldst_monitor-1.0.4/src/ldst_monitor/ding.py
--rwxrwxrwx   0 happy     (1000) happy     (1000)      987 2023-07-06 14:55:51.000000 ldst_monitor-1.0.4/src/ldst_monitor/main.py
--rwxrwxrwx   0 happy     (1000) happy     (1000)     2653 2023-07-06 16:01:17.000000 ldst_monitor-1.0.4/src/ldst_monitor/monitor.py
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:36:17.804648 ldst_monitor-1.0.4/src/ldst_monitor.egg-info/
--rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-07 03:36:17.000000 ldst_monitor-1.0.4/src/ldst_monitor.egg-info/PKG-INFO
--rwxrwxrwx   0 happy     (1000) happy     (1000)      281 2023-07-07 03:36:17.000000 ldst_monitor-1.0.4/src/ldst_monitor.egg-info/SOURCES.txt
--rwxrwxrwx   0 happy     (1000) happy     (1000)        1 2023-07-07 03:36:17.000000 ldst_monitor-1.0.4/src/ldst_monitor.egg-info/dependency_links.txt
--rwxrwxrwx   0 happy     (1000) happy     (1000)       13 2023-07-07 03:36:17.000000 ldst_monitor-1.0.4/src/ldst_monitor.egg-info/top_level.txt
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:54:56.953503 ldst_monitor-1.0.5/
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-07 03:54:56.953141 ldst_monitor-1.0.5/PKG-INFO
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      488 2023-07-07 03:52:54.000000 ldst_monitor-1.0.5/pyproject.toml
+-rwxrwxrwx   0 happy     (1000) happy     (1000)       38 2023-07-07 03:54:56.953641 ldst_monitor-1.0.5/setup.cfg
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:54:56.940660 ldst_monitor-1.0.5/src/
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:54:56.945811 ldst_monitor-1.0.5/src/ldst_monitor/
+-rwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 14:33:12.000000 ldst_monitor-1.0.5/src/ldst_monitor/__init__.py
+-rwxrwxrwx   0 happy     (1000) happy     (1000)     1321 2023-07-06 14:55:29.000000 ldst_monitor-1.0.5/src/ldst_monitor/ding.py
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      987 2023-07-06 14:55:51.000000 ldst_monitor-1.0.5/src/ldst_monitor/main.py
+-rwxrwxrwx   0 happy     (1000) happy     (1000)     2653 2023-07-06 16:01:17.000000 ldst_monitor-1.0.5/src/ldst_monitor/monitor.py
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:54:56.951751 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-07 03:54:56.000000 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/PKG-INFO
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      320 2023-07-07 03:54:56.000000 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/SOURCES.txt
+-rwxrwxrwx   0 happy     (1000) happy     (1000)        1 2023-07-07 03:54:56.000000 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/dependency_links.txt
+-rwxrwxrwx   0 happy     (1000) happy     (1000)       23 2023-07-07 03:54:56.000000 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/requires.txt
+-rwxrwxrwx   0 happy     (1000) happy     (1000)       13 2023-07-07 03:54:56.000000 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/top_level.txt
```

### Comparing `ldst_monitor-1.0.4/src/ldst_monitor/ding.py` & `ldst_monitor-1.0.5/src/ldst_monitor/ding.py`

 * *Files identical despite different names*

### Comparing `ldst_monitor-1.0.4/src/ldst_monitor/main.py` & `ldst_monitor-1.0.5/src/ldst_monitor/main.py`

 * *Files identical despite different names*

### Comparing `ldst_monitor-1.0.4/src/ldst_monitor/monitor.py` & `ldst_monitor-1.0.5/src/ldst_monitor/monitor.py`

 * *Files identical despite different names*

