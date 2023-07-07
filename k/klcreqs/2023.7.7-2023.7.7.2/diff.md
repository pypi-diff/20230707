# Comparing `tmp/klcreqs-2023.7.7.tar.gz` & `tmp/klcreqs-2023.7.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klcreqs-2023.7.7.tar", last modified: Fri Jul  7 18:59:29 2023, max compression
+gzip compressed data, was "klcreqs-2023.7.7.2.tar", last modified: Fri Jul  7 19:02:56 2023, max compression
```

## Comparing `klcreqs-2023.7.7.tar` & `klcreqs-2023.7.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 18:59:29.631401 klcreqs-2023.7.7/
--rw-rw-rw-   0        0        0      228 2023-07-07 18:59:29.630405 klcreqs-2023.7.7/PKG-INFO
--rw-rw-rw-   0        0        0     2587 2023-02-22 21:31:43.000000 klcreqs-2023.7.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 18:59:29.618437 klcreqs-2023.7.7/klcreqs/
--rw-rw-rw-   0        0        0       19 2022-10-19 22:05:31.000000 klcreqs-2023.7.7/klcreqs/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-07-07 18:57:28.000000 klcreqs-2023.7.7/klcreqs/constants.py
--rw-rw-rw-   0        0        0    13924 2023-06-14 21:30:54.000000 klcreqs-2023.7.7/klcreqs/core.py
-drwxrwxrwx   0        0        0        0 2023-07-07 18:59:29.628410 klcreqs-2023.7.7/klcreqs.egg-info/
--rw-rw-rw-   0        0        0      228 2023-07-07 18:59:29.000000 klcreqs-2023.7.7/klcreqs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-07 18:59:29.000000 klcreqs-2023.7.7/klcreqs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 18:59:29.000000 klcreqs-2023.7.7/klcreqs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 18:59:29.000000 klcreqs-2023.7.7/klcreqs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-07 18:59:29.000000 klcreqs-2023.7.7/klcreqs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 18:59:29.631401 klcreqs-2023.7.7/setup.cfg
--rw-rw-rw-   0        0        0      576 2023-07-07 18:48:58.000000 klcreqs-2023.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:02:56.059712 klcreqs-2023.7.7.2/
+-rw-rw-rw-   0        0        0      230 2023-07-07 19:02:56.057717 klcreqs-2023.7.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2587 2023-02-22 21:31:43.000000 klcreqs-2023.7.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 19:02:56.039769 klcreqs-2023.7.7.2/klcreqs/
+-rw-rw-rw-   0        0        0       40 2023-07-07 19:01:43.000000 klcreqs-2023.7.7.2/klcreqs/__init__.py
+-rw-rw-rw-   0        0        0     1760 2023-07-07 19:01:28.000000 klcreqs-2023.7.7.2/klcreqs/constants.py
+-rw-rw-rw-   0        0        0    13924 2023-06-14 21:30:54.000000 klcreqs-2023.7.7.2/klcreqs/core.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:02:56.049738 klcreqs-2023.7.7.2/klcreqs.egg-info/
+-rw-rw-rw-   0        0        0      230 2023-07-07 19:02:55.000000 klcreqs-2023.7.7.2/klcreqs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-07 19:02:55.000000 klcreqs-2023.7.7.2/klcreqs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 19:02:55.000000 klcreqs-2023.7.7.2/klcreqs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 19:02:55.000000 klcreqs-2023.7.7.2/klcreqs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 19:02:55.000000 klcreqs-2023.7.7.2/klcreqs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 19:02:56.059712 klcreqs-2023.7.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      578 2023-07-07 19:02:31.000000 klcreqs-2023.7.7.2/setup.py
```

### Comparing `klcreqs-2023.7.7/README.md` & `klcreqs-2023.7.7.2/README.md`

 * *Files identical despite different names*

### Comparing `klcreqs-2023.7.7/klcreqs/constants.py` & `klcreqs-2023.7.7.2/klcreqs/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,11 +46,14 @@
 cross_sectional_endpoint = 'https://api.factset.com/formula-api/v1/cross-sectional'
 timeseries_endpoint = "https://api.factset.com/formula-api/v1/time-series"
 status_endpoint = 'https://api.factset.com/formula-api/v1/batch-status'
 result_endpoint = 'https://api.factset.com/formula-api/v1/batch-result'
 intang_path = r'CLIENT:/GK_INDEXES/GLOBAL_INDEXES/MID-LARGE/AC/KLSUX_AC.OFDB'
 uri = urllib.parse.quote(intang_path, safe="")
 url = f'{ofdb_endpoint}{uri}/dates'
-rebals_rtrv = json.loads(requests.get(url, auth=authorization, headers=headers).text)
+
+def get_rebal():
+    rebals_rtrv = json.loads(requests.get(url, auth=authorization, headers=headers).text)
 # print(rebals_rtrv)
-with open(r'rebals.txt', 'w') as f:
-    f.write(str(rebals_rtrv[0]))
+    with open(r'rebals.txt', 'w') as f:
+        f.write(str(rebals_rtrv[0]))
+    return rebals_rtrv[0]
```

### Comparing `klcreqs-2023.7.7/klcreqs/core.py` & `klcreqs-2023.7.7.2/klcreqs/core.py`

 * *Files identical despite different names*

### Comparing `klcreqs-2023.7.7/setup.py` & `klcreqs-2023.7.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 if __name__ == "__main__":
     setup(
         name="klcreqs",
-        version="2023.07.07",
+        version="2023.07.07.2",
         description="library for streamlining api requests",
         long_description="coming soon",
         readme="README.md",
         author='Thomas Nemechek',
         author_email='tnemechek@klcapital.com',
         classifiers=["Programming Language :: Python"],
         packages=['klcreqs'],
```

