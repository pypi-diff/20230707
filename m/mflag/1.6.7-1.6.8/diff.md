# Comparing `tmp/mflag-1.6.7.tar.gz` & `tmp/mflag-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mflag-1.6.7.tar", last modified: Mon Jun 26 13:15:26 2023, max compression
+gzip compressed data, was "mflag-1.6.8.tar", last modified: Fri Jul  7 11:36:22 2023, max compression
```

## Comparing `mflag-1.6.7.tar` & `mflag-1.6.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.356387 mflag-1.6.7/
--rwxrwxrwx   0 root         (0) root         (0)     1071 2023-06-24 10:44:31.000000 mflag-1.6.7/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-26 13:15:26.356224 mflag-1.6.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2026 2023-06-24 10:44:31.000000 mflag-1.6.7/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.352756 mflag-1.6.7/mflag/
--rwxrwxrwx   0 root         (0) root         (0)      226 2023-06-26 13:13:23.000000 mflag-1.6.7/mflag/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.354441 mflag-1.6.7/mflag/src/
--rwxrwxrwx   0 root         (0) root         (0)     4559 2023-06-26 13:11:50.000000 mflag-1.6.7/mflag/src/flag.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.351447 mflag-1.6.7/mflag/src/rcmng/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.354963 mflag-1.6.7/mflag/src/rcmng/client/
--rwxrwxrwx   0 root         (0) root         (0)     1631 2023-06-24 10:41:50.000000 mflag-1.6.7/mflag/src/rcmng/client/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      433 2023-06-24 09:19:59.000000 mflag-1.6.7/mflag/src/rcmng/client/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.355433 mflag-1.6.7/mflag/src/rcmng/server/
--rwxrwxrwx   0 root         (0) root         (0)     6832 2023-06-24 10:42:40.000000 mflag-1.6.7/mflag/src/rcmng/server/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      255 2023-06-24 08:55:53.000000 mflag-1.6.7/mflag/src/rcmng/server/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.355935 mflag-1.6.7/mflag/src/rcmng/submit/
--rwxrwxrwx   0 root         (0) root         (0)      844 2023-06-24 10:18:10.000000 mflag-1.6.7/mflag/src/rcmng/submit/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      444 2023-06-24 10:33:05.000000 mflag-1.6.7/mflag/src/rcmng/submit/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.354189 mflag-1.6.7/mflag.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-26 13:15:26.000000 mflag-1.6.7/mflag.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      401 2023-06-26 13:15:26.000000 mflag-1.6.7/mflag.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-26 13:15:26.000000 mflag-1.6.7/mflag.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       26 2023-06-26 13:15:26.000000 mflag-1.6.7/mflag.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-06-26 13:15:26.000000 mflag-1.6.7/mflag.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-26 13:15:26.356447 mflag-1.6.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      516 2023-06-26 13:13:56.000000 mflag-1.6.7/setup.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     1071 2023-06-24 10:44:31.000000 mflag-1.6.8/LICENSE
+-rw-r--r--   0 moses     (1000) sftpgroup  (1002)     2209 2023-07-07 11:36:22.879390 mflag-1.6.8/PKG-INFO
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     2026 2023-06-24 10:44:31.000000 mflag-1.6.8/README.md
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.878390 mflag-1.6.8/mflag/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      226 2023-07-05 10:21:55.000000 mflag-1.6.8/mflag/__init__.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/mflag/src/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     4559 2023-06-26 13:11:50.000000 mflag-1.6.8/mflag/src/flag.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.878390 mflag-1.6.8/mflag/src/rcmng/
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/mflag/src/rcmng/client/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     1631 2023-06-24 10:41:50.000000 mflag-1.6.8/mflag/src/rcmng/client/__init__.py
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      433 2023-06-24 09:19:59.000000 mflag-1.6.8/mflag/src/rcmng/client/run.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/mflag/src/rcmng/server/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     6819 2023-07-05 10:21:40.000000 mflag-1.6.8/mflag/src/rcmng/server/__init__.py
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      255 2023-06-24 08:55:53.000000 mflag-1.6.8/mflag/src/rcmng/server/run.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/mflag/src/rcmng/submit/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      844 2023-06-24 10:18:10.000000 mflag-1.6.8/mflag/src/rcmng/submit/__init__.py
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      444 2023-06-24 10:33:05.000000 mflag-1.6.8/mflag/src/rcmng/submit/run.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/mflag.egg-info/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     2209 2023-07-07 11:36:22.000000 mflag-1.6.8/mflag.egg-info/PKG-INFO
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      401 2023-07-07 11:36:22.000000 mflag-1.6.8/mflag.egg-info/SOURCES.txt
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)        1 2023-07-07 11:36:22.000000 mflag-1.6.8/mflag.egg-info/dependency_links.txt
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)       26 2023-07-07 11:36:22.000000 mflag-1.6.8/mflag.egg-info/requires.txt
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)        6 2023-07-07 11:36:22.000000 mflag-1.6.8/mflag.egg-info/top_level.txt
+-rw-r--r--   0 moses     (1000) sftpgroup  (1002)       38 2023-07-07 11:36:22.879390 mflag-1.6.8/setup.cfg
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      516 2023-06-26 13:13:56.000000 mflag-1.6.8/setup.py
```

### Comparing `mflag-1.6.7/LICENSE` & `mflag-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mflag-1.6.7/PKG-INFO` & `mflag-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflag
-Version: 1.6.7
+Version: 1.6.8
 Summary: put/remove flags for files and folders
 Author: Moses Dastmard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mflag: powerful Python toolkit for mark/unmark files and directories 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/mflag/)
```

### Comparing `mflag-1.6.7/README.md` & `mflag-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `mflag-1.6.7/mflag/src/flag.py` & `mflag-1.6.8/mflag/src/flag.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.7/mflag/src/rcmng/client/__init__.py` & `mflag-1.6.8/mflag/src/rcmng/client/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.7/mflag/src/rcmng/server/__init__.py` & `mflag-1.6.8/mflag/src/rcmng/server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     id_ = "DIFF"
     cpu_reserved, mem_reserved = get_reserved_resource(reserved_usage)
     cpu_usage, mem_usage, swap_usage = get_mean_resource_history(usage_history)
     date_ = now_ + timedelta(seconds=60)
     cpu_diff = round(cpu_usage - cpu_reserved, 2)
     cpu_diff = max(-100, min(cpu_diff, 100))
     mem_diff = round(mem_usage - mem_reserved, 2)
-    mem_diff = max(-MEM_SIZE, min(mem_diff, MEM_SIZE)) + swap_usage
+    mem_diff = max(-MEM_SIZE, min(mem_diff, MEM_SIZE))
     data_ = {
         "cpu": cpu_diff,
         "mem": mem_diff,
         "expiration": date_,
     }
     if id_ in reserved_usage.keys():
         if reserved_usage[id_]["expiration"] < now_:
```

### Comparing `mflag-1.6.7/mflag/src/rcmng/submit/__init__.py` & `mflag-1.6.8/mflag/src/rcmng/submit/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.7/mflag.egg-info/PKG-INFO` & `mflag-1.6.8/mflag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflag
-Version: 1.6.7
+Version: 1.6.8
 Summary: put/remove flags for files and folders
 Author: Moses Dastmard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mflag: powerful Python toolkit for mark/unmark files and directories 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/mflag/)
```

### Comparing `mflag-1.6.7/setup.py` & `mflag-1.6.8/setup.py`

 * *Files identical despite different names*

