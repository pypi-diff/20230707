# Comparing `tmp/klcreqs-2023.7.7.3.tar.gz` & `tmp/klcreqs-2023.7.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klcreqs-2023.7.7.3.tar", last modified: Fri Jul  7 19:28:46 2023, max compression
+gzip compressed data, was "klcreqs-2023.7.7.4.tar", last modified: Fri Jul  7 20:01:04 2023, max compression
```

## Comparing `klcreqs-2023.7.7.3.tar` & `klcreqs-2023.7.7.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 19:28:46.989612 klcreqs-2023.7.7.3/
--rw-rw-rw-   0        0        0      230 2023-07-07 19:28:46.988614 klcreqs-2023.7.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     2587 2023-02-22 21:31:43.000000 klcreqs-2023.7.7.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 19:28:46.976648 klcreqs-2023.7.7.3/klcreqs/
--rw-rw-rw-   0        0        0       40 2023-07-07 19:01:43.000000 klcreqs-2023.7.7.3/klcreqs/__init__.py
--rw-rw-rw-   0        0        0     1840 2023-07-07 19:19:01.000000 klcreqs-2023.7.7.3/klcreqs/constants.py
--rw-rw-rw-   0        0        0    13924 2023-07-07 19:18:52.000000 klcreqs-2023.7.7.3/klcreqs/core.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:28:46.986621 klcreqs-2023.7.7.3/klcreqs.egg-info/
--rw-rw-rw-   0        0        0      230 2023-07-07 19:28:46.000000 klcreqs-2023.7.7.3/klcreqs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-07 19:28:46.000000 klcreqs-2023.7.7.3/klcreqs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 19:28:46.000000 klcreqs-2023.7.7.3/klcreqs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 19:28:46.000000 klcreqs-2023.7.7.3/klcreqs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-07 19:28:46.000000 klcreqs-2023.7.7.3/klcreqs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 19:28:46.989612 klcreqs-2023.7.7.3/setup.cfg
--rw-rw-rw-   0        0        0      578 2023-07-07 19:16:05.000000 klcreqs-2023.7.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:01:04.561644 klcreqs-2023.7.7.4/
+-rw-rw-rw-   0        0        0      230 2023-07-07 20:01:04.560646 klcreqs-2023.7.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2587 2023-02-22 21:31:43.000000 klcreqs-2023.7.7.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 20:01:04.541696 klcreqs-2023.7.7.4/klcreqs/
+-rw-rw-rw-   0        0        0       40 2023-07-07 19:01:43.000000 klcreqs-2023.7.7.4/klcreqs/__init__.py
+-rw-rw-rw-   0        0        0     1853 2023-07-07 19:58:49.000000 klcreqs-2023.7.7.4/klcreqs/constants.py
+-rw-rw-rw-   0        0        0    13924 2023-07-07 19:29:41.000000 klcreqs-2023.7.7.4/klcreqs/core.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:01:04.551674 klcreqs-2023.7.7.4/klcreqs.egg-info/
+-rw-rw-rw-   0        0        0      230 2023-07-07 20:01:04.000000 klcreqs-2023.7.7.4/klcreqs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-07 20:01:04.000000 klcreqs-2023.7.7.4/klcreqs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 20:01:04.000000 klcreqs-2023.7.7.4/klcreqs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 20:01:04.000000 klcreqs-2023.7.7.4/klcreqs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 20:01:04.000000 klcreqs-2023.7.7.4/klcreqs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 20:01:04.561644 klcreqs-2023.7.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      578 2023-07-07 20:00:56.000000 klcreqs-2023.7.7.4/setup.py
```

### Comparing `klcreqs-2023.7.7.3/README.md` & `klcreqs-2023.7.7.4/README.md`

 * *Files identical despite different names*

### Comparing `klcreqs-2023.7.7.3/klcreqs/constants.py` & `klcreqs-2023.7.7.4/klcreqs/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,11 +49,12 @@
 result_endpoint = 'https://api.factset.com/formula-api/v1/batch-result'
 intang_path = r'CLIENT:/GK_INDEXES/GLOBAL_INDEXES/MID-LARGE/AC/KLSUX_AC.OFDB'
 uri = urllib.parse.quote(intang_path, safe="")
 url = f'{ofdb_endpoint}{uri}/dates'
 
 def get_rebal():
     rebals_rtrv = json.loads(requests.get(url, auth=authorization, headers=headers).text)
-# print(rebals_rtrv)
-    with open(r'rebals.txt', 'w') as f:
-        f.write(str(rebals_rtrv[0]))
-    return rebals_rtrv[0]
+    # with open(r'rebals.txt', 'w') as f:
+    #     f.write(str(rebals_rtrv[0]))
+    return rebals_rtrv['data'][0]
+
+rebal = get_rebal()
```

### Comparing `klcreqs-2023.7.7.3/klcreqs/core.py` & `klcreqs-2023.7.7.4/klcreqs/core.py`

 * *Files identical despite different names*

### Comparing `klcreqs-2023.7.7.3/setup.py` & `klcreqs-2023.7.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 if __name__ == "__main__":
     setup(
         name="klcreqs",
-        version="2023.07.07.3",
+        version="2023.07.07.4",
         description="library for streamlining api requests",
         long_description="coming soon",
         readme="README.md",
         author='Thomas Nemechek',
         author_email='tnemechek@klcapital.com',
         classifiers=["Programming Language :: Python"],
         packages=['klcreqs'],
```

