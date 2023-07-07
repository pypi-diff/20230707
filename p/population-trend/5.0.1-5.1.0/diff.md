# Comparing `tmp/population_trend-5.0.1.tar.gz` & `tmp/population_trend-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "population_trend-5.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "population_trend-5.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `population_trend-5.0.1.tar` & `population_trend-5.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1037 2023-07-07 17:59:08.007665 population_trend-5.0.1/README.md
--rw-r--r--   0        0        0      251 2023-07-07 17:59:08.007665 population_trend-5.0.1/population_trend/__init__.py
--rw-r--r--   0        0        0     7212 2023-07-07 17:59:08.007665 population_trend-5.0.1/population_trend/calculate_growth_rates.py
--rw-r--r--   0        0        0     2451 2023-07-07 17:59:08.007665 population_trend-5.0.1/population_trend/cli.py
--rw-r--r--   0        0        0      403 2023-07-07 17:59:08.007665 population_trend-5.0.1/population_trend/filter_data.py
--rw-r--r--   0        0        0     6056 2023-07-07 17:59:08.007665 population_trend-5.0.1/population_trend/population_growth_model.py
--rw-r--r--   0        0        0      495 2023-07-07 17:59:08.007665 population_trend-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1037 2023-07-07 19:57:52.888421 population_trend-5.1.0/README.md
+-rw-r--r--   0        0        0      251 2023-07-07 19:57:52.892421 population_trend-5.1.0/population_trend/__init__.py
+-rw-r--r--   0        0        0     7237 2023-07-07 19:57:52.892421 population_trend-5.1.0/population_trend/calculate_growth_rates.py
+-rw-r--r--   0        0        0     2542 2023-07-07 19:57:52.892421 population_trend-5.1.0/population_trend/cli.py
+-rw-r--r--   0        0        0      403 2023-07-07 19:57:52.892421 population_trend-5.1.0/population_trend/filter_data.py
+-rw-r--r--   0        0        0     6056 2023-07-07 19:57:52.892421 population_trend-5.1.0/population_trend/population_growth_model.py
+-rw-r--r--   0        0        0      495 2023-07-07 19:57:52.892421 population_trend-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-5.1.0/PKG-INFO
```

### Comparing `population_trend-5.0.1/README.md` & `population_trend-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `population_trend-5.0.1/population_trend/calculate_growth_rates.py` & `population_trend-5.1.0/population_trend/calculate_growth_rates.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,18 @@
         porcentaje_cambio = calculate_porcentual_diff(
             model.iloc[-1], cantidad_nidos["Maxima_cantidad_nidos"].iloc[0]
         )
     return porcentaje_cambio
 
 
 class Bootstrap_from_time_series_parameterizer:
-    def __init__(self, blocks_length=3, N=2000):
+    def __init__(self, blocks_length=3, N=2000, column_name="Maxima_cantidad_nidos"):
         self.parameters = dict(
             dataframe=None,
-            column_name="Maxima_cantidad_nidos",
+            column_name=column_name,
             N=N,
             return_distribution=True,
             blocks_length=blocks_length,
         )
 
     def set_data(self, data):
         self.parameters["dataframe"] = data
```

### Comparing `population_trend-5.0.1/population_trend/cli.py` & `population_trend-5.1.0/population_trend/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 
 
 @app.command(help="Write json with bootstrap intervals")
 def write_bootstrap_intervals_json(
     data_path: str = "data/processed/gumu_guadalupe_burrows.csv",
     blocks_length: int = 3,
     bootstrap_number: int = 2000,
+    variable_of_interest: str = "Maxima_cantidad_nidos",
     output_path: str = "reports/non-tabular/gumu_guadalupe_boostrap_intervals.json",
 ):
     data = pd.read_csv(data_path)
     parametrizer = Bootstrap_from_time_series_parameterizer(
-        blocks_length=blocks_length, N=bootstrap_number
+        blocks_length=blocks_length, N=bootstrap_number, column_name=variable_of_interest
     )
     parametrizer.set_data(data)
     bootstrap = Bootstrap_from_time_series(parametrizer)
     bootstrap.save_intervals(output_path)
 
 
 @app.command(help="Write csv with ouput-path")
```

### Comparing `population_trend-5.0.1/population_trend/population_growth_model.py` & `population_trend-5.1.0/population_trend/population_growth_model.py`

 * *Files identical despite different names*

### Comparing `population_trend-5.0.1/PKG-INFO` & `population_trend-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: population_trend
-Version: 5.0.1
+Version: 5.1.0
 Summary: A template Python module
 Home-page: https://github.com/IslasGECI/population_trend
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: population_trend Version: 5.0.1 Summary: A template
+Metadata-Version: 2.1 Name: population_trend Version: 5.1.0 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/population_trend Author:
 Ciencia de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-
 Python: >=3.9 Description-Content-Type: text/markdown Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
 bootstrapping-tools==3.0.0 Requires-Dist: geci-plots Requires-Dist: typer
 [https://www.islas.org.mx/img/logo.svg] # Dummy Transformations Para usar este
 repo como plantilla debemos hacer lo siguiente: 1. Presiona el botÃ³n verde que
```

