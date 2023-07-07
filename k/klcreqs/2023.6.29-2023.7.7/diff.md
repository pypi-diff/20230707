# Comparing `tmp/klcreqs-2023.6.29.tar.gz` & `tmp/klcreqs-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klcreqs-2023.6.29.tar", last modified: Thu Jun 29 20:00:48 2023, max compression
+gzip compressed data, was "klcreqs-2023.7.7.tar", last modified: Fri Jul  7 18:59:29 2023, max compression
```

## Comparing `klcreqs-2023.6.29.tar` & `klcreqs-2023.7.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:00:48.626442 klcreqs-2023.6.29/
--rw-rw-rw-   0        0        0      229 2023-06-29 20:00:48.624447 klcreqs-2023.6.29/PKG-INFO
--rw-rw-rw-   0        0        0     2587 2023-02-22 21:31:43.000000 klcreqs-2023.6.29/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 20:00:48.607493 klcreqs-2023.6.29/klcreqs/
--rw-rw-rw-   0        0        0       19 2022-10-19 22:05:31.000000 klcreqs-2023.6.29/klcreqs/__init__.py
--rw-rw-rw-   0        0        0     1825 2023-04-05 22:48:56.000000 klcreqs-2023.6.29/klcreqs/constants.py
--rw-rw-rw-   0        0        0    13924 2023-06-14 21:30:54.000000 klcreqs-2023.6.29/klcreqs/core.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:00:48.619462 klcreqs-2023.6.29/klcreqs.egg-info/
--rw-rw-rw-   0        0        0      229 2023-06-29 20:00:47.000000 klcreqs-2023.6.29/klcreqs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-06-29 20:00:47.000000 klcreqs-2023.6.29/klcreqs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:00:47.000000 klcreqs-2023.6.29/klcreqs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-29 20:00:47.000000 klcreqs-2023.6.29/klcreqs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-29 20:00:47.000000 klcreqs-2023.6.29/klcreqs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 20:00:48.627443 klcreqs-2023.6.29/setup.cfg
--rw-rw-rw-   0        0        0      576 2023-06-29 19:55:31.000000 klcreqs-2023.6.29/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:59:29.631401 klcreqs-2023.7.7/
+-rw-rw-rw-   0        0        0      228 2023-07-07 18:59:29.630405 klcreqs-2023.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2587 2023-02-22 21:31:43.000000 klcreqs-2023.7.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 18:59:29.618437 klcreqs-2023.7.7/klcreqs/
+-rw-rw-rw-   0        0        0       19 2022-10-19 22:05:31.000000 klcreqs-2023.7.7/klcreqs/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-07-07 18:57:28.000000 klcreqs-2023.7.7/klcreqs/constants.py
+-rw-rw-rw-   0        0        0    13924 2023-06-14 21:30:54.000000 klcreqs-2023.7.7/klcreqs/core.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:59:29.628410 klcreqs-2023.7.7/klcreqs.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-07 18:59:29.000000 klcreqs-2023.7.7/klcreqs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-07 18:59:29.000000 klcreqs-2023.7.7/klcreqs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 18:59:29.000000 klcreqs-2023.7.7/klcreqs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 18:59:29.000000 klcreqs-2023.7.7/klcreqs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 18:59:29.000000 klcreqs-2023.7.7/klcreqs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 18:59:29.631401 klcreqs-2023.7.7/setup.cfg
+-rw-rw-rw-   0        0        0      576 2023-07-07 18:48:58.000000 klcreqs-2023.7.7/setup.py
```

### Comparing `klcreqs-2023.6.29/README.md` & `klcreqs-2023.7.7/README.md`

 * *Files identical despite different names*

### Comparing `klcreqs-2023.6.29/klcreqs/constants.py` & `klcreqs-2023.7.7/klcreqs/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 import time
 import urllib
 import urllib.parse
 from tqdm import tqdm
 
 
 requests.packages.urllib3.disable_warnings()
-a = pd.read_csv(r'C:\KL_Capital Dropbox\Python\py4klc\a.csv')
+a = pd.read_csv(r'a.csv')
 user_serial = a.loc[2,'a']
 key = a.loc[2,'b']
 authorization = (user_serial, key)
 
 
 class auth:
-    a = pd.read_csv(r'C:\KL_Capital Dropbox\Python\py4klc\a.csv')
+    a = pd.read_csv(r'a.csv')
     auths = []
     for r in a.index: 
         auths.append(tuple(a.loc[r].to_list()))
 
     def __init__(self):
         self.n = 0
         self.auth = auth.auths[self.n]
@@ -38,19 +38,19 @@
         else:
             self.n = 0
         self.auth = auth.auths[self.n]
         return self.auth
 
 # formula api config
 headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
-ofdb_endpoint = "https://api.factset.com/analytics/ofdb/v1/database/"
+ofdb_endpoint = "https://api.factset.com/analytics/ofdb/v2/database/"
 cross_sectional_endpoint = 'https://api.factset.com/formula-api/v1/cross-sectional'
 timeseries_endpoint = "https://api.factset.com/formula-api/v1/time-series"
 status_endpoint = 'https://api.factset.com/formula-api/v1/batch-status'
 result_endpoint = 'https://api.factset.com/formula-api/v1/batch-result'
 intang_path = r'CLIENT:/GK_INDEXES/GLOBAL_INDEXES/MID-LARGE/AC/KLSUX_AC.OFDB'
 uri = urllib.parse.quote(intang_path, safe="")
 url = f'{ofdb_endpoint}{uri}/dates'
 rebals_rtrv = json.loads(requests.get(url, auth=authorization, headers=headers).text)
 # print(rebals_rtrv)
-# with open(r'C:\\KL_Capital Dropbox\\Python\\py4klc\\py4klc\\rebals.txt', 'w') as f:
-#     f.write(str(rebals_rtrv[0]))
+with open(r'rebals.txt', 'w') as f:
+    f.write(str(rebals_rtrv[0]))
```

### Comparing `klcreqs-2023.6.29/klcreqs/core.py` & `klcreqs-2023.7.7/klcreqs/core.py`

 * *Files identical despite different names*

### Comparing `klcreqs-2023.6.29/setup.py` & `klcreqs-2023.7.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 if __name__ == "__main__":
     setup(
         name="klcreqs",
-        version="2023.06.29",
+        version="2023.07.07",
         description="library for streamlining api requests",
         long_description="coming soon",
         readme="README.md",
         author='Thomas Nemechek',
         author_email='tnemechek@klcapital.com',
         classifiers=["Programming Language :: Python"],
         packages=['klcreqs'],
```

