# Comparing `tmp/population_trend-5.0.0.tar.gz` & `tmp/population_trend-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "population_trend-5.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "population_trend-5.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `population_trend-5.0.0.tar` & `population_trend-5.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1037 2023-07-06 20:19:02.812134 population_trend-5.0.0/README.md
--rw-r--r--   0        0        0      251 2023-07-06 20:19:02.816134 population_trend-5.0.0/population_trend/__init__.py
--rw-r--r--   0        0        0     7212 2023-07-06 20:19:02.816134 population_trend-5.0.0/population_trend/calculate_growth_rates.py
--rw-r--r--   0        0        0     2602 2023-07-06 20:19:02.816134 population_trend-5.0.0/population_trend/cli.py
--rw-r--r--   0        0        0      403 2023-07-06 20:19:02.816134 population_trend-5.0.0/population_trend/filter_data.py
--rw-r--r--   0        0        0     5550 2023-07-06 20:19:02.816134 population_trend-5.0.0/population_trend/population_growth_model.py
--rw-r--r--   0        0        0      495 2023-07-06 20:19:02.816134 population_trend-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1037 2023-07-07 17:59:08.007665 population_trend-5.0.1/README.md
+-rw-r--r--   0        0        0      251 2023-07-07 17:59:08.007665 population_trend-5.0.1/population_trend/__init__.py
+-rw-r--r--   0        0        0     7212 2023-07-07 17:59:08.007665 population_trend-5.0.1/population_trend/calculate_growth_rates.py
+-rw-r--r--   0        0        0     2451 2023-07-07 17:59:08.007665 population_trend-5.0.1/population_trend/cli.py
+-rw-r--r--   0        0        0      403 2023-07-07 17:59:08.007665 population_trend-5.0.1/population_trend/filter_data.py
+-rw-r--r--   0        0        0     6056 2023-07-07 17:59:08.007665 population_trend-5.0.1/population_trend/population_growth_model.py
+-rw-r--r--   0        0        0      495 2023-07-07 17:59:08.007665 population_trend-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-5.0.1/PKG-INFO
```

### Comparing `population_trend-5.0.0/README.md` & `population_trend-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `population_trend-5.0.0/population_trend/calculate_growth_rates.py` & `population_trend-5.0.1/population_trend/calculate_growth_rates.py`

 * *Files identical despite different names*

### Comparing `population_trend-5.0.0/population_trend/cli.py` & `population_trend-5.0.1/population_trend/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,19 +54,14 @@
     with open(intervals_path, "r") as read_file:
         intervals_json = json.load(read_file)
     lambda_latex = intervals_json["lambda_latex_interval"]
 
     Modelo_Tendencia_Poblacional = Population_Trend_Model(
         fit_data, intervals_json, variable_of_interest
     )
-    Graficador = Plotter_Population_Trend_Model(fit_data)
+    Graficador = Plotter_Population_Trend_Model(fit_data, Modelo_Tendencia_Poblacional)
     Graficador.plot_smooth(Modelo_Tendencia_Poblacional)
     Graficador.plot_model(Modelo_Tendencia_Poblacional)
-    Graficador.plot_data(variable_of_interest)
+    Graficador.plot_data()
     legend_mpl_object = Graficador.set_legend_location(island)
-    Graficador.set_x_lim()
-    Graficador.set_y_lim(fit_data[variable_of_interest])
-    Graficador.set_labels()
-    Graficador.set_ticks()
-    Graficador.draw()
     Graficador.plot_growth_rate_interval(legend_mpl_object, lambda_latex)
     Graficador.savefig(island, output_path)
```

### Comparing `population_trend-5.0.0/population_trend/population_growth_model.py` & `population_trend-5.0.1/population_trend/population_growth_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,17 @@
     return upper_limit
 
 
 class Population_Trend_Model:
     def __init__(self, fit_data, json_parameters, interest_variable):
         self.intervals = json_parameters["intervals"]
         self.model_domain = calculate_model_domain(fit_data)
+        self.interest_variable = interest_variable
         self.initial_population = lambda_calculator(
-            fit_data["Temporada"], fit_data[interest_variable]
+            fit_data["Temporada"], fit_data[self.interest_variable]
         )
         self.bootstrap_distribution = json_parameters["bootstrap_distribution"]
 
     def intern_model(self, i):
         return power_law(
             self.model_domain, self.bootstrap_distribution[i][0], self.bootstrap_distribution[i][1]
         )
@@ -47,21 +48,22 @@
 
     @property
     def max_model(self):
         return power_law(self.model_domain, self.intervals[2][0], self.intervals[2][1])
 
 
 class Plotter_Population_Trend_Model:
-    def __init__(self, data):
+    def __init__(self, data, population_model):
         self.fig, self.ax = geci_plot()
         self.data = data
         self.plot_seasons = self.data["Temporada"][:] - self.data["Temporada"].iloc[0] + 1
         self.ticks_text = normalize_seasons(self.data)
         self.ticks_positions = ticks_positions_array(self.ticks_text)
         self.plot_domain = np.linspace(self.ticks_positions.min(), self.ticks_positions.max(), 100)
+        self.interest_variable = population_model.interest_variable
 
     def plot_smooth(self, Population_Trend_Model):
         self.ax.fill_between(
             self.plot_domain,
             Population_Trend_Model.min_model,
             Population_Trend_Model.med_model,
             label="Confidence zone",
@@ -75,41 +77,48 @@
         )
         self.ax.fill_between(
             self.plot_domain,
             Population_Trend_Model.min_model,
             Population_Trend_Model.max_model,
             color="powderblue",
         )
-        for i in range(0, len(Population_Trend_Model.bootstrap_distribution) - 1, 10):
+        number_of_samples = len(Population_Trend_Model.bootstrap_distribution)
+        for i in range(0, number_of_samples - 1, 10):
             self.ax.fill_between(
                 self.plot_domain,
                 Population_Trend_Model.intern_model(i),
                 Population_Trend_Model.med_model,
                 color="powderblue",
             )
             self.ax.fill_between(
                 self.plot_domain,
                 Population_Trend_Model.intern_model(i),
                 Population_Trend_Model.intern_model(i + 1),
                 color="powderblue",
             )
+        self.ax.fill_between(
+            self.plot_domain,
+            Population_Trend_Model.intern_model(i + 1),
+            Population_Trend_Model.med_model,
+            color="powderblue",
+        )
 
     def plot_model(self, Population_Trend_Model):
         plt.plot(
             self.plot_domain,
             Population_Trend_Model.med_model,
             label="Population growth model",
             color="b",
         )
         return self.fig
 
-    def plot_data(self, variable_to_bootstrap):
+    def plot_data(self):
         plt.plot(
             self.plot_seasons,
-            self.data[variable_to_bootstrap],
+            self.data[self.interest_variable],
             "-Dk",
             label="Active Nests",
         )
 
     def plot_growth_rate_interval(self, legend_mpl_object, lambda_latex):
         legend_box_positions = legend_mpl_object.get_window_extent()
         self.ax.annotate(
@@ -117,18 +126,18 @@
             (legend_box_positions.p0[0], legend_box_positions.p1[1] - 320),
             xycoords="figure pixels",
             fontsize=25,
             color="k",
             alpha=1,
         )
 
-    def set_y_lim(self, fit_data):
+    def set_y_lim(self):
         self.ax.set_ylim(
             0,
-            calculate_upper_limit(fit_data),
+            calculate_upper_limit(self.data[self.interest_variable]),
         )
 
     def set_x_lim(self):
         plt.xlim(
             self.ticks_positions.min() - 0.2,
             self.ticks_positions.max(),
         )
@@ -147,14 +156,19 @@
         plt.yticks(size=20)
 
     def draw(self):
         plt.gcf().subplots_adjust(bottom=0.2)
         plt.draw()
 
     def savefig(self, islet, output_path=None):
+        self.set_x_lim()
+        self.set_y_lim()
+        self.set_labels()
+        self.set_ticks()
+        self.draw()
         if output_path is None:
             plt.savefig(
                 "reports/figures/cormorant_population_trend_{}".format(
                     islet.replace(" ", "_").lower()
                 ),
                 dpi=300,
             )
```

### Comparing `population_trend-5.0.0/PKG-INFO` & `population_trend-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: population_trend
-Version: 5.0.0
+Version: 5.0.1
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
-Metadata-Version: 2.1 Name: population_trend Version: 5.0.0 Summary: A template
+Metadata-Version: 2.1 Name: population_trend Version: 5.0.1 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/population_trend Author:
 Ciencia de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-
 Python: >=3.9 Description-Content-Type: text/markdown Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
 bootstrapping-tools==3.0.0 Requires-Dist: geci-plots Requires-Dist: typer
 [https://www.islas.org.mx/img/logo.svg] # Dummy Transformations Para usar este
 repo como plantilla debemos hacer lo siguiente: 1. Presiona el botÃ³n verde que
```

