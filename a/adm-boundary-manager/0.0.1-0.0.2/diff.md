# Comparing `tmp/adm-boundary-manager-0.0.1.tar.gz` & `tmp/adm-boundary-manager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adm-boundary-manager-0.0.1.tar", last modified: Thu Jul  6 14:02:30 2023, max compression
+gzip compressed data, was "adm-boundary-manager-0.0.2.tar", last modified: Fri Jul  7 08:15:09 2023, max compression
```

## Comparing `adm-boundary-manager-0.0.1.tar` & `adm-boundary-manager-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:02:30.042166 adm-boundary-manager-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-06 14:02:30.042166 adm-boundary-manager-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:02:30.042166 adm-boundary-manager-0.0.1/adm_boundary_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-06 14:02:30.000000 adm-boundary-manager-0.0.1/adm_boundary_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-06 14:02:30.000000 adm-boundary-manager-0.0.1/adm_boundary_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:02:30.000000 adm-boundary-manager-0.0.1/adm_boundary_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-06 14:02:30.000000 adm-boundary-manager-0.0.1/adm_boundary_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 14:02:30.000000 adm-boundary-manager-0.0.1/adm_boundary_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:02:30.042166 adm-boundary-manager-0.0.1/adminboundarymanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/boundary_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:02:30.042166 adm-boundary-manager-0.0.1/adminboundarymanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:02:30.038166 adm-boundary-manager-0.0.1/adminboundarymanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:02:30.042166 adm-boundary-manager-0.0.1/adminboundarymanager/templates/adminboundarymanager/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/adminboundarymanager/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 14:02:14.000000 adm-boundary-manager-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-06 14:02:30.042166 adm-boundary-manager-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:15:09.183096 adm-boundary-manager-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-07 08:15:09.187096 adm-boundary-manager-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:15:09.183096 adm-boundary-manager-0.0.2/adm_boundary_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-07 08:15:09.000000 adm-boundary-manager-0.0.2/adm_boundary_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-07 08:15:09.000000 adm-boundary-manager-0.0.2/adm_boundary_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:15:09.000000 adm-boundary-manager-0.0.2/adm_boundary_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 08:15:09.000000 adm-boundary-manager-0.0.2/adm_boundary_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 08:15:09.000000 adm-boundary-manager-0.0.2/adm_boundary_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:15:09.183096 adm-boundary-manager-0.0.2/adminboundarymanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/boundary_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:15:09.183096 adm-boundary-manager-0.0.2/adminboundarymanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:15:09.179095 adm-boundary-manager-0.0.2/adminboundarymanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:15:09.183096 adm-boundary-manager-0.0.2/adminboundarymanager/templates/adminboundarymanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/adminboundarymanager/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 08:14:49.000000 adm-boundary-manager-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 08:15:09.187096 adm-boundary-manager-0.0.2/setup.cfg
```

### Comparing `adm-boundary-manager-0.0.1/PKG-INFO` & `adm-boundary-manager-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adm-boundary-manager
-Version: 0.0.1
+Version: 0.0.2
 Summary: Load, manage and visualize Administrative Boundaries Data in Wagtail
 Home-page: https://github.com/wmo-raf/adm-boundary-manager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `adm-boundary-manager-0.0.1/adm_boundary_manager.egg-info/PKG-INFO` & `adm-boundary-manager-0.0.2/adm_boundary_manager.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adm-boundary-manager
-Version: 0.0.1
+Version: 0.0.2
 Summary: Load, manage and visualize Administrative Boundaries Data in Wagtail
 Home-page: https://github.com/wmo-raf/adm-boundary-manager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `adm-boundary-manager-0.0.1/adm_boundary_manager.egg-info/SOURCES.txt` & `adm-boundary-manager-0.0.2/adm_boundary_manager.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,10 +19,11 @@
 adminboundarymanager/tests.py
 adminboundarymanager/urls.py
 adminboundarymanager/utils.py
 adminboundarymanager/views.py
 adminboundarymanager/wagtail_hooks.py
 adminboundarymanager/migrations/0001_initial.py
 adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
+adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
 adminboundarymanager/migrations/__init__.py
 adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
 adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
```

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/boundary_loader.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/boundary_loader.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/countries.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/countries.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/errors.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/errors.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/forms.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/forms.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/migrations/0001_initial.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/models.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/models.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/serializers.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/serializers.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html` & `adm-boundary-manager-0.0.2/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html` & `adm-boundary-manager-0.0.2/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/urls.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/urls.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/utils.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/utils.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/views.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
         sql = f"""WITH
             bounds AS (
               SELECT ST_TileEnvelope({z}, {x}, {y}) AS geom
             ),
             mvtgeom AS (
               SELECT ST_AsMVTGeom(ST_Transform(t.geom, 3857), bounds.geom) AS geom,
-                t.name_0, t.name_1, t.name_2, t.name_3, t.name_4, t.gid_0, t.gid_1, t.gid_2, t.gid_3, t.gid_4, t.level
+               t.id, t.name_0, t.name_1, t.name_2, t.name_3, t.name_4, t.gid_0, t.gid_1, t.gid_2, t.gid_3, t.gid_4, t.level
               FROM {self.table_name} t, bounds
               WHERE ST_Intersects(ST_Transform(t.geom, 4326), ST_Transform(bounds.geom, 4326)) {boundary_filter}
             )
             SELECT ST_AsMVT(mvtgeom, 'default') FROM mvtgeom;
             """
         close_old_connections()
         with connection.cursor() as cursor:
```

### Comparing `adm-boundary-manager-0.0.1/adminboundarymanager/wagtail_hooks.py` & `adm-boundary-manager-0.0.2/adminboundarymanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.1/setup.cfg` & `adm-boundary-manager-0.0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = adm-boundary-manager
-version = 0.0.1
+version = 0.0.2
 description = Load, manage and visualize Administrative Boundaries Data in Wagtail
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/adm-boundary-manager
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

