# Comparing `tmp/rqsdk-1.5.1.tar.gz` & `tmp/rqsdk-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rqsdk-1.5.1.tar", last modified: Fri Jun 16 08:17:43 2023, max compression
+gzip compressed data, was "dist/rqsdk-1.5.2.tar", last modified: Fri Jul  7 09:38:54 2023, max compression
```

## Comparing `rqsdk-1.5.1.tar` & `rqsdk-1.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-16 08:17:43.561169 rqsdk-1.5.1/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      256 2023-06-16 08:17:37.000000 rqsdk-1.5.1/HISTORY.md
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      173 2023-06-16 08:17:37.000000 rqsdk-1.5.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-06-16 08:17:43.561169 rqsdk-1.5.1/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1111 2023-06-16 08:17:37.000000 rqsdk-1.5.1/README.md
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-16 08:17:43.570169 rqsdk-1.5.1/rqsdk/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      752 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      680 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/__main__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      497 2023-06-16 08:17:43.570169 rqsdk-1.5.1/rqsdk/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    13017 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/cmds.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1738 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/const.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     6715 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/license_helper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      319 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/proxy_helper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2453 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/script_update.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      741 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/testing.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-16 08:17:43.561169 rqsdk-1.5.1/rqsdk.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      438 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)       44 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3363 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        6 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      244 2023-06-16 08:17:43.562169 rqsdk-1.5.1/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3129 2023-06-16 08:17:37.000000 rqsdk-1.5.1/setup.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    79860 2023-06-16 08:17:37.000000 rqsdk-1.5.1/versioneer.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-07-07 09:38:54.989753 rqsdk-1.5.2/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      256 2023-07-07 09:38:52.000000 rqsdk-1.5.2/HISTORY.md
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      173 2023-07-07 09:38:52.000000 rqsdk-1.5.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-07-07 09:38:54.989753 rqsdk-1.5.2/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1111 2023-07-07 09:38:52.000000 rqsdk-1.5.2/README.md
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-07-07 09:38:54.990753 rqsdk-1.5.2/rqsdk/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      752 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      680 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/__main__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      497 2023-07-07 09:38:54.990753 rqsdk-1.5.2/rqsdk/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    13017 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/cmds.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1738 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/const.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     6715 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/license_helper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      319 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/proxy_helper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2453 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/script_update.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      741 2023-07-07 09:38:52.000000 rqsdk-1.5.2/rqsdk/testing.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-07-07 09:38:54.987753 rqsdk-1.5.2/rqsdk.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      438 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)       44 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3417 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        6 2023-07-07 09:38:54.000000 rqsdk-1.5.2/rqsdk.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      244 2023-07-07 09:38:54.990753 rqsdk-1.5.2/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3140 2023-07-07 09:38:52.000000 rqsdk-1.5.2/setup.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    79860 2023-07-07 09:38:52.000000 rqsdk-1.5.2/versioneer.py
```

### Comparing `rqsdk-1.5.1/PKG-INFO` & `rqsdk-1.5.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqsdk
-Version: 1.5.1
+Version: 1.5.2
 Summary: Ricequant Native SDK
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Keywords: rqsdk
 Platform: UNKNOWN
```

### Comparing `rqsdk-1.5.1/README.md` & `rqsdk-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.1/rqsdk/__init__.py` & `rqsdk-1.5.2/rqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.1/rqsdk/__main__.py` & `rqsdk-1.5.2/rqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.1/rqsdk/cmds.py` & `rqsdk-1.5.2/rqsdk/cmds.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.1/rqsdk/const.py` & `rqsdk-1.5.2/rqsdk/const.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.1/rqsdk/license_helper.py` & `rqsdk-1.5.2/rqsdk/license_helper.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.1/rqsdk/script_update.py` & `rqsdk-1.5.2/rqsdk/script_update.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.1/rqsdk/testing.py` & `rqsdk-1.5.2/rqsdk/testing.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.1/rqsdk.egg-info/PKG-INFO` & `rqsdk-1.5.2/rqsdk.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqsdk
-Version: 1.5.1
+Version: 1.5.2
 Summary: Ricequant Native SDK
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Keywords: rqsdk
 Platform: UNKNOWN
```

### Comparing `rqsdk-1.5.1/rqsdk.egg-info/requires.txt` & `rqsdk-1.5.2/rqsdk.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-wcwidth
+requests
 tabulate
 rqdatac>=2.9.44
-click>=7.0
-rqdatac_fund==1.0.*,>=1.0.18
+wcwidth
 patsy>=0.5.1
-requests
-pyjwt==1.7.1
+rqdatac_fund==1.0.*,>=1.0.18
 statsmodels>=0.12.1
+click>=7.0
 pandas>=0.24.2
+pyjwt==1.7.1
 
 [:python_version <= "3.6"]
+cryptography==2.9.2
 python-rapidjson<=1.5
 numpy>=1.19.5
-cryptography==2.9.2
 
 [:python_version <= "3.7"]
 scipy<=1.7.3
 
 [:python_version == "3.7"]
 numpy>=1.20.0
 
 [:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [:python_version >= "3.8"]
-scipy>=1.8.0
 numpy>=1.23.0
+scipy<=1.10.1,>=1.8.0
 
 [rqalpha_plus]
-rqalpha-mod-ricequant-data==2.4.0
+rqalpha-mod-spot==1.0.9
+rqalpha-plus==4.2.4
+rqalpha-mod-option==1.1.23
 tabulate
+rqalpha-mod-ricequant-data==2.4.0
 rqdatac>=2.9.44
-rqalpha==5.1.0
-ta-lib>=0.4.20
-rqalpha-mod-convertible==1.2.15
+rqalpha-mod-fund==0.0.12
+rqdatac_fund==1.0.*,>=1.0.18
+statsmodels>=0.12.1
 rqalpha-mod-rqfactor==1.0.10
 matplotlib>=3.1.0
-h5py>=3.0.0
-rqdatac_fund==1.0.*,>=1.0.18
-requests
-pandas>=0.24.2
+rqalpha==5.1.1
 rqalpha-mod-optimizer2==1.0.8
-rqalpha-mod-fund==0.0.12
-rqrisk==1.0.7
+rqfactor==1.3.*,>=1.3.1
+requests
 rqalpha-mod-incremental==0.0.8
+rqalpha-mod-convertible==1.2.15
+h5py>=3.0.0
+hdf5plugin
+rqrisk==1.0.7
+ta-lib>=0.4.20
 wcwidth
-rqalpha-mod-option==1.1.23
-click>=7.0
 patsy>=0.5.1
-rqalpha-mod-spot==1.0.9
+pandas>=0.24.2
+click>=7.0
 pyjwt==1.7.1
-statsmodels>=0.12.1
-rqalpha-plus==4.2.4
-hdf5plugin
-rqfactor==1.3.*,>=1.3.1
 
 [rqalpha_plus:python_version <= "3.6"]
-cryptography==2.9.2
-numpy>=1.19.5
 python-rapidjson<=1.5
+numpy>=1.19.5
+cryptography==2.9.2
 
 [rqalpha_plus:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqalpha_plus:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqalpha_plus:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqalpha_plus:python_version >= "3.8"]
-scipy>=1.8.0
+scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
 
 [rqdatac]
-wcwidth
+requests
 tabulate
 rqdatac>=2.9.44
-click>=7.0
-rqdatac_fund==1.0.*,>=1.0.18
+wcwidth
 patsy>=0.5.1
-requests
-pyjwt==1.7.1
+rqdatac_fund==1.0.*,>=1.0.18
 statsmodels>=0.12.1
+click>=7.0
 pandas>=0.24.2
+pyjwt==1.7.1
 
 [rqdatac:python_version <= "3.6"]
+cryptography==2.9.2
 python-rapidjson<=1.5
 numpy>=1.19.5
-cryptography==2.9.2
 
 [rqdatac:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqdatac:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqdatac:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqdatac:python_version >= "3.8"]
-scipy>=1.8.0
 numpy>=1.23.0
+scipy<=1.10.1,>=1.8.0
 
 [rqfactor]
 tabulate
 rqdatac>=2.9.44
-ta-lib>=0.4.20
 rqdatac_fund==1.0.*,>=1.0.18
+statsmodels>=0.12.1
+rqfactor==1.3.*,>=1.3.1
 requests
-pandas>=0.24.2
+ta-lib>=0.4.20
 wcwidth
-click>=7.0
 patsy>=0.5.1
+pandas>=0.24.2
+click>=7.0
 pyjwt==1.7.1
-statsmodels>=0.12.1
-rqfactor==1.3.*,>=1.3.1
 
 [rqfactor:python_version <= "3.6"]
-cryptography==2.9.2
-numpy>=1.19.5
 python-rapidjson<=1.5
+numpy>=1.19.5
+cryptography==2.9.2
 
 [rqfactor:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqfactor:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqfactor:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqfactor:python_version >= "3.8"]
-scipy>=1.8.0
+scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
 
 [rqoptimizer]
+ecos==2.0.10
 rqoptimizer2==1.2.*,>=1.2.17
 tabulate
 rqdatac>=2.9.44
-scs==2.1.4
 rqdatac_fund==1.0.*,>=1.0.18
+statsmodels>=0.12.1
+rqoptimizer==1.2.*,>=1.2.17
 requests
-pandas>=0.24.2
-ecos==2.0.10
 osqp==0.6.2.post5
+scs==2.1.4
 wcwidth
-click>=7.0
 patsy>=0.5.1
+pandas>=0.24.2
+click>=7.0
 pyjwt==1.7.1
-statsmodels>=0.12.1
-rqoptimizer==1.2.*,>=1.2.17
 
 [rqoptimizer:python_version <= "3.6"]
-cryptography==2.9.2
-numpy>=1.19.5
 python-rapidjson<=1.5
+numpy>=1.19.5
+cryptography==2.9.2
 
 [rqoptimizer:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqoptimizer:python_version == "3.6"]
 cvxpy==1.1.18
 
@@ -169,40 +169,40 @@
 [rqoptimizer:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqoptimizer:python_version >= "3.7"]
 cvxpy==1.2.0
 
 [rqoptimizer:python_version >= "3.8"]
-scipy>=1.8.0
+scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
 
 [rqpattr]
 tabulate
 rqdatac>=2.9.44
+rqpattr>=0.0.2
 rqdatac_fund==1.0.*,>=1.0.18
+statsmodels>=0.12.1
 requests
-pandas>=0.24.2
-rqpattr>=0.0.2
 wcwidth
-click>=7.0
 patsy>=0.5.1
+pandas>=0.24.2
+click>=7.0
 pyjwt==1.7.1
-statsmodels>=0.12.1
 
 [rqpattr:python_version <= "3.6"]
-cryptography==2.9.2
-numpy>=1.19.5
 python-rapidjson<=1.5
+numpy>=1.19.5
+cryptography==2.9.2
 
 [rqpattr:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqpattr:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqpattr:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqpattr:python_version >= "3.8"]
-scipy>=1.8.0
+scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
```

### Comparing `rqsdk-1.5.1/setup.py` & `rqsdk-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "pyopenssl>22.0.0; python_version > '3.7'",  #  cryptography 的版本由 pyopenssl 来指定
     "cryptography==2.9.2; python_version <= '3.6'",  # python 3.6.0有点过分,pip更新报错，cryptography版本太高也报错
     "click>=7.0",
     "pyjwt==1.7.1",
     "patsy>=0.5.1",
     "statsmodels>=0.12.1",
     "scipy <= 1.7.3; python_version <= '3.7'",
-    "scipy >= 1.8.0; python_version >= '3.8'",
+    "scipy >= 1.8.0, <= 1.10.1; python_version >= '3.8'",
     "numpy>=1.19.5; python_version <= '3.6'",
     "numpy>=1.20.0; python_version == '3.7'",
     "numpy>=1.23.0; python_version >= '3.8'",  # numpy 1.23.0 修改了类型大小
     "pandas >= 0.24.2",
     "python-rapidjson <= 1.5; python_version <= '3.6'",  # rapidjson 1.6 开始不再提供 python 3.6 的 whl 包
     "rqdatac>=2.9.44",
     "rqdatac_fund==1.0.*,>=1.0.18"
@@ -34,15 +34,15 @@
     "cvxpy==1.1.18 ; python_version == '3.6'",
     "cvxpy==1.2.0 ; python_version >= '3.7'",
     "osqp==0.6.2.post5",
     "rqoptimizer==1.2.*,>=1.2.17",
     "rqoptimizer2==1.2.*,>=1.2.17",
 }
 version_map["rqalpha_plus"] = version_map["rqfactor"] | {
-    "rqalpha==5.1.0",
+    "rqalpha==5.1.1",
     "rqalpha-mod-option==1.1.23",
     "rqalpha-mod-optimizer2==1.0.8",
     "rqalpha-mod-convertible==1.2.15",
     "rqalpha-mod-ricequant-data==2.4.0",
     "rqalpha-mod-rqfactor==1.0.10",
     "rqalpha-mod-spot==1.0.9",
     "rqalpha-mod-fund==0.0.12",
```

### Comparing `rqsdk-1.5.1/versioneer.py` & `rqsdk-1.5.2/versioneer.py`

 * *Files identical despite different names*

