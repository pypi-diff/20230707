# Comparing `tmp/rateToolsAC4RM-0.2.tar.gz` & `tmp/rateToolsAC4RM-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rateToolsAC4RM-0.2.tar", last modified: Fri Jul  7 20:24:30 2023, max compression
+gzip compressed data, was "rateToolsAC4RM-0.3.tar", last modified: Fri Jul  7 20:27:41 2023, max compression
```

## Comparing `rateToolsAC4RM-0.2.tar` & `rateToolsAC4RM-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 20:24:30.816186 rateToolsAC4RM-0.2/
--rw-r--r--   0 tleitch1   (501) staff       (20)      189 2023-07-07 20:24:30.816460 rateToolsAC4RM-0.2/PKG-INFO
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 20:24:30.809707 rateToolsAC4RM-0.2/rateToolsAC4RM/
--rw-rw-r--   0 tleitch1   (501) staff       (20)      272 2023-07-07 20:05:55.000000 rateToolsAC4RM-0.2/rateToolsAC4RM/__init__.py
--rw-r--r--   0 tleitch1   (501) staff       (20)     4679 2023-07-07 20:22:17.000000 rateToolsAC4RM-0.2/rateToolsAC4RM/rateTools.py
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 20:24:30.815166 rateToolsAC4RM-0.2/rateToolsAC4RM.egg-info/
--rw-r--r--   0 tleitch1   (501) staff       (20)      189 2023-07-07 20:24:30.000000 rateToolsAC4RM-0.2/rateToolsAC4RM.egg-info/PKG-INFO
--rw-r--r--   0 tleitch1   (501) staff       (20)      262 2023-07-07 20:24:30.000000 rateToolsAC4RM-0.2/rateToolsAC4RM.egg-info/SOURCES.txt
--rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-07-07 20:24:30.000000 rateToolsAC4RM-0.2/rateToolsAC4RM.egg-info/dependency_links.txt
--rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-06-20 03:42:27.000000 rateToolsAC4RM-0.2/rateToolsAC4RM.egg-info/not-zip-safe
--rw-r--r--   0 tleitch1   (501) staff       (20)       15 2023-07-07 20:24:30.000000 rateToolsAC4RM-0.2/rateToolsAC4RM.egg-info/top_level.txt
--rw-rw-r--   0 tleitch1   (501) staff       (20)       38 2023-07-07 20:24:30.817541 rateToolsAC4RM-0.2/setup.cfg
--rw-rw-r--   0 tleitch1   (501) staff       (20)      226 2023-07-07 20:24:01.000000 rateToolsAC4RM-0.2/setup.py
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 20:27:41.444172 rateToolsAC4RM-0.3/
+-rw-r--r--   0 tleitch1   (501) staff       (20)      189 2023-07-07 20:27:41.444339 rateToolsAC4RM-0.3/PKG-INFO
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 20:27:41.439393 rateToolsAC4RM-0.3/rateToolsAC4RM/
+-rw-rw-r--   0 tleitch1   (501) staff       (20)      272 2023-07-07 20:05:55.000000 rateToolsAC4RM-0.3/rateToolsAC4RM/__init__.py
+-rw-r--r--   0 tleitch1   (501) staff       (20)     4673 2023-07-07 20:27:09.000000 rateToolsAC4RM-0.3/rateToolsAC4RM/rateTools.py
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 20:27:41.443112 rateToolsAC4RM-0.3/rateToolsAC4RM.egg-info/
+-rw-r--r--   0 tleitch1   (501) staff       (20)      189 2023-07-07 20:27:41.000000 rateToolsAC4RM-0.3/rateToolsAC4RM.egg-info/PKG-INFO
+-rw-r--r--   0 tleitch1   (501) staff       (20)      262 2023-07-07 20:27:41.000000 rateToolsAC4RM-0.3/rateToolsAC4RM.egg-info/SOURCES.txt
+-rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-07-07 20:27:41.000000 rateToolsAC4RM-0.3/rateToolsAC4RM.egg-info/dependency_links.txt
+-rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-06-20 03:42:27.000000 rateToolsAC4RM-0.3/rateToolsAC4RM.egg-info/not-zip-safe
+-rw-r--r--   0 tleitch1   (501) staff       (20)       15 2023-07-07 20:27:41.000000 rateToolsAC4RM-0.3/rateToolsAC4RM.egg-info/top_level.txt
+-rw-rw-r--   0 tleitch1   (501) staff       (20)       38 2023-07-07 20:27:41.445177 rateToolsAC4RM-0.3/setup.cfg
+-rw-rw-r--   0 tleitch1   (501) staff       (20)      226 2023-07-07 20:27:04.000000 rateToolsAC4RM-0.3/setup.py
```

### Comparing `rateToolsAC4RM-0.2/rateToolsAC4RM/rateTools.py` & `rateToolsAC4RM-0.3/rateToolsAC4RM/rateTools.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,13 +152,13 @@
 # following function assumes rates are all 1 year apart
 from scipy.optimize import fsolve
 
 def swapMkt(yc,face=1000):
   swap=[]
   for  year in yc.itertuples():
     # solve for breakeven swap rate given dcf
-    be = lambda rate : rt.pv(rt.bulletSwap(year.t,rate,1000),yc['dcf'])-1000.  
+    be = lambda rate : rt.pv(bulletSwap(year.t,rate,1000),yc['dcf'])-1000.  
     rateBE=fsolve(be,year.rate) 
-    swap.append([year.t,rateBE[0],rt.bulletSwap(year.t,rateBE,face)])
+    swap.append([year.t,rateBE[0],bulletSwap(year.t,rateBE,face)])
   return swap
```

