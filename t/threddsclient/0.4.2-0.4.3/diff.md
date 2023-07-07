# Comparing `tmp/threddsclient-0.4.2.tar.gz` & `tmp/threddsclient-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/threddsclient-0.4.2.tar", last modified: Wed Nov 20 10:30:28 2019, max compression
+gzip compressed data, was "threddsclient-0.4.3.tar", last modified: Fri Jul  7 14:32:07 2023, max compression
```

## Comparing `threddsclient-0.4.2.tar` & `threddsclient-0.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2019-11-20 10:30:28.000000 threddsclient-0.4.2/
--rw-r--r--   0 pingu      (501) staff       (20)       96 2019-11-20 09:24:15.000000 threddsclient-0.4.2/AUTHORS.rst
--rw-r--r--   0 pingu      (501) staff       (20)     1134 2019-11-20 10:17:32.000000 threddsclient-0.4.2/CHANGES.rst
--rw-r--r--   0 pingu      (501) staff       (20)    11324 2018-10-05 08:14:55.000000 threddsclient-0.4.2/LICENCE.txt
--rw-r--r--   0 pingu      (501) staff       (20)       78 2018-10-05 08:14:55.000000 threddsclient-0.4.2/MANIFEST.in
--rw-r--r--   0 pingu      (501) staff       (20)     8078 2019-11-20 10:30:28.000000 threddsclient-0.4.2/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)     4374 2019-11-20 10:12:17.000000 threddsclient-0.4.2/README.rst
--rw-r--r--   0 pingu      (501) staff       (20)       37 2018-10-05 17:57:16.000000 threddsclient-0.4.2/requirements-dev.txt
--rw-r--r--   0 pingu      (501) staff       (20)       29 2018-10-05 08:14:55.000000 threddsclient-0.4.2/requirements.txt
--rw-r--r--   0 pingu      (501) staff       (20)      548 2019-11-20 10:30:28.000000 threddsclient-0.4.2/setup.cfg
--rw-r--r--   0 pingu      (501) staff       (20)     1059 2019-11-20 09:24:15.000000 threddsclient-0.4.2/setup.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2019-11-20 10:30:28.000000 threddsclient-0.4.2/tests/
--rw-r--r--   0 pingu      (501) staff       (20)     2985 2018-10-05 17:57:16.000000 threddsclient-0.4.2/tests/test_birdhouse_sample.py
--rw-r--r--   0 pingu      (501) staff       (20)     2345 2018-10-05 17:57:16.000000 threddsclient-0.4.2/tests/test_catalog.py
--rw-r--r--   0 pingu      (501) staff       (20)     2260 2018-10-05 17:57:16.000000 threddsclient-0.4.2/tests/test_dataset.py
--rw-r--r--   0 pingu      (501) staff       (20)    10499 2018-10-05 17:57:16.000000 threddsclient-0.4.2/tests/test_noaa_sample.py
--rw-r--r--   0 pingu      (501) staff       (20)      953 2018-10-05 17:57:16.000000 threddsclient-0.4.2/tests/test_online.py
--rw-r--r--   0 pingu      (501) staff       (20)      530 2018-10-05 17:57:16.000000 threddsclient-0.4.2/tests/test_utils.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2019-11-20 10:30:28.000000 threddsclient-0.4.2/threddsclient/
--rw-r--r--   0 pingu      (501) staff       (20)       98 2019-11-20 10:16:12.000000 threddsclient-0.4.2/threddsclient/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     5105 2018-10-05 08:14:55.000000 threddsclient-0.4.2/threddsclient/catalog.py
--rw-r--r--   0 pingu      (501) staff       (20)     2324 2019-11-20 09:24:15.000000 threddsclient-0.4.2/threddsclient/client.py
--rw-r--r--   0 pingu      (501) staff       (20)     6274 2019-11-20 09:24:15.000000 threddsclient-0.4.2/threddsclient/nodes.py
--rw-r--r--   0 pingu      (501) staff       (20)     1127 2019-11-20 09:24:15.000000 threddsclient-0.4.2/threddsclient/utils.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2019-11-20 10:30:28.000000 threddsclient-0.4.2/threddsclient.egg-info/
--rw-r--r--   0 pingu      (501) staff       (20)     8078 2019-11-20 10:30:28.000000 threddsclient-0.4.2/threddsclient.egg-info/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)      598 2019-11-20 10:30:28.000000 threddsclient-0.4.2/threddsclient.egg-info/SOURCES.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2019-11-20 10:30:28.000000 threddsclient-0.4.2/threddsclient.egg-info/dependency_links.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2018-10-05 08:33:32.000000 threddsclient-0.4.2/threddsclient.egg-info/not-zip-safe
--rw-r--r--   0 pingu      (501) staff       (20)       29 2019-11-20 10:30:28.000000 threddsclient-0.4.2/threddsclient.egg-info/requires.txt
--rw-r--r--   0 pingu      (501) staff       (20)       14 2019-11-20 10:30:28.000000 threddsclient-0.4.2/threddsclient.egg-info/top_level.txt
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-07 14:32:07.684966 threddsclient-0.4.3/
+-rw-r--r--   0 pingu      (501) staff       (20)       96 2023-07-07 14:28:04.000000 threddsclient-0.4.3/AUTHORS.rst
+-rw-r--r--   0 pingu      (501) staff       (20)     1212 2023-07-07 14:32:00.000000 threddsclient-0.4.3/CHANGES.rst
+-rw-r--r--   0 pingu      (501) staff       (20)    11324 2023-07-07 14:28:04.000000 threddsclient-0.4.3/LICENCE.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       78 2023-07-07 14:28:04.000000 threddsclient-0.4.3/MANIFEST.in
+-rw-r--r--   0 pingu      (501) staff       (20)     6208 2023-07-07 14:32:07.685189 threddsclient-0.4.3/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)     4374 2023-07-07 14:28:04.000000 threddsclient-0.4.3/README.rst
+-rw-r--r--   0 pingu      (501) staff       (20)       37 2023-07-07 14:28:04.000000 threddsclient-0.4.3/requirements-dev.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       29 2023-07-07 14:28:04.000000 threddsclient-0.4.3/requirements.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      548 2023-07-07 14:32:07.686100 threddsclient-0.4.3/setup.cfg
+-rw-r--r--   0 pingu      (501) staff       (20)     1059 2023-07-07 14:32:00.000000 threddsclient-0.4.3/setup.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-07 14:32:07.674707 threddsclient-0.4.3/tests/
+-rw-r--r--   0 pingu      (501) staff       (20)     2985 2023-07-07 14:28:04.000000 threddsclient-0.4.3/tests/test_birdhouse_sample.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2345 2023-07-07 14:28:04.000000 threddsclient-0.4.3/tests/test_catalog.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2260 2023-07-07 14:28:04.000000 threddsclient-0.4.3/tests/test_dataset.py
+-rw-r--r--   0 pingu      (501) staff       (20)    10499 2023-07-07 14:28:04.000000 threddsclient-0.4.3/tests/test_noaa_sample.py
+-rw-r--r--   0 pingu      (501) staff       (20)      953 2023-07-07 14:32:00.000000 threddsclient-0.4.3/tests/test_online.py
+-rw-r--r--   0 pingu      (501) staff       (20)      530 2023-07-07 14:28:04.000000 threddsclient-0.4.3/tests/test_utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-07 14:32:07.678711 threddsclient-0.4.3/threddsclient/
+-rw-r--r--   0 pingu      (501) staff       (20)       98 2023-07-07 14:28:04.000000 threddsclient-0.4.3/threddsclient/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     5121 2023-07-07 14:28:04.000000 threddsclient-0.4.3/threddsclient/catalog.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2324 2023-07-07 14:28:04.000000 threddsclient-0.4.3/threddsclient/client.py
+-rw-r--r--   0 pingu      (501) staff       (20)     6274 2023-07-07 14:28:04.000000 threddsclient-0.4.3/threddsclient/nodes.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1127 2023-07-07 14:28:04.000000 threddsclient-0.4.3/threddsclient/utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-07-07 14:32:07.684396 threddsclient-0.4.3/threddsclient.egg-info/
+-rw-r--r--   0 pingu      (501) staff       (20)     6208 2023-07-07 14:32:07.000000 threddsclient-0.4.3/threddsclient.egg-info/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)      598 2023-07-07 14:32:07.000000 threddsclient-0.4.3/threddsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        1 2023-07-07 14:32:07.000000 threddsclient-0.4.3/threddsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        1 2023-07-07 14:30:19.000000 threddsclient-0.4.3/threddsclient.egg-info/not-zip-safe
+-rw-r--r--   0 pingu      (501) staff       (20)       29 2023-07-07 14:32:07.000000 threddsclient-0.4.3/threddsclient.egg-info/requires.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       14 2023-07-07 14:32:07.000000 threddsclient-0.4.3/threddsclient.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `threddsclient-0.4.2/CHANGES.rst` & `threddsclient-0.4.3/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 Changes
 =======
 
+0.4.3 (2023-05-31)
+==================
+
+* fix xml parsing for recent versions
+
 0.4.2 (2019-11-20)
 ==================
 
 * fixed conda links in Readme.
 
 0.4.1 (2019-11-06)
 ==================
```

### Comparing `threddsclient-0.4.2/LICENCE.txt` & `threddsclient-0.4.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/README.rst` & `threddsclient-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/setup.cfg` & `threddsclient-0.4.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.2
+current_version = 0.4.3
 commit = True
 tag = True
 
 [metadata]
 description-file = README.rst
 
 [bumpversion:file:threddsclient/__init__.py]
```

### Comparing `threddsclient-0.4.2/setup.py` & `threddsclient-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/tests/test_birdhouse_sample.py` & `threddsclient-0.4.3/tests/test_birdhouse_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     assert len(cat.services[0].services) == 4
     assert len(cat.get_services('all')) == 4
 
 
 def test_birdhouse_top():
     xml = """
     <catalog xmlns="http://www.unidata.ucar.edu/namespaces/thredds/InvCatalog/v1.0" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.0.1">  # noqa
-      <service name="all" serviceType="Compound" base="">
+      <service name="all" serviceType="compound" base="">
         <service name="service4" serviceType="HTTPServer" base="/thredds/fileServer/" />
         <service name="odap" serviceType="OPENDAP" base="/thredds/dodsC/" />
         <service name="wcs" serviceType="WCS" base="/thredds/wcs/" />
         <service name="wms" serviceType="WMS" base="/thredds/wms/" />
       </service>
       <dataset name="Test all files in a directory" ID="testDatasetScan">
         <metadata inherited="true">
```

### Comparing `threddsclient-0.4.2/tests/test_catalog.py` & `threddsclient-0.4.3/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/tests/test_dataset.py` & `threddsclient-0.4.3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/tests/test_noaa_sample.py` & `threddsclient-0.4.3/tests/test_noaa_sample.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/tests/test_online.py` & `threddsclient-0.4.3/tests/test_online.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/tests/test_utils.py` & `threddsclient-0.4.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/threddsclient/catalog.py` & `threddsclient-0.4.3/threddsclient/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     def get_services(self, service_name):
         """
         Returns a list of services with names matching `service_name`
         """
         services = []
         for service in self.services:
             if service.name == service_name:
-                if service.service_type == 'Compound':
+                if service.service_type.lower() == 'Compound'.lower():
                     services.extend(service.services)
                 else:
                     services.append(service)
         return services
 
     def download_urls(self):
         """
```

### Comparing `threddsclient-0.4.2/threddsclient/client.py` & `threddsclient-0.4.3/threddsclient/client.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/threddsclient/nodes.py` & `threddsclient-0.4.3/threddsclient/nodes.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/threddsclient/utils.py` & `threddsclient-0.4.3/threddsclient/utils.py`

 * *Files identical despite different names*

### Comparing `threddsclient-0.4.2/threddsclient.egg-info/SOURCES.txt` & `threddsclient-0.4.3/threddsclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

