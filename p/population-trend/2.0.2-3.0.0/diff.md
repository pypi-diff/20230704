# Comparing `tmp/population_trend-2.0.2.tar.gz` & `tmp/population_trend-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "population_trend-2.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "population_trend-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `population_trend-2.0.2.tar` & `population_trend-3.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1037 2023-07-03 19:25:56.647534 population_trend-2.0.2/README.md
--rw-r--r--   0        0        0      163 2023-07-03 19:25:56.647534 population_trend-2.0.2/population_trend/__init__.py
--rw-r--r--   0        0        0     1982 2023-07-03 19:25:56.647534 population_trend-2.0.2/population_trend/cli.py
--rw-r--r--   0        0        0      403 2023-07-03 19:25:56.647534 population_trend-2.0.2/population_trend/filter_data.py
--rw-r--r--   0        0        0     4316 2023-07-03 19:25:56.647534 population_trend-2.0.2/population_trend/population_growth_model.py
--rw-r--r--   0        0        0      495 2023-07-03 19:25:56.647534 population_trend-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1037 2023-07-04 00:00:06.907205 population_trend-3.0.0/README.md
+-rw-r--r--   0        0        0      163 2023-07-04 00:00:06.907205 population_trend-3.0.0/population_trend/__init__.py
+-rw-r--r--   0        0        0     1894 2023-07-04 00:00:06.907205 population_trend-3.0.0/population_trend/cli.py
+-rw-r--r--   0        0        0      403 2023-07-04 00:00:06.907205 population_trend-3.0.0/population_trend/filter_data.py
+-rw-r--r--   0        0        0     4361 2023-07-04 00:00:06.907205 population_trend-3.0.0/population_trend/population_growth_model.py
+-rw-r--r--   0        0        0      495 2023-07-04 00:00:06.907205 population_trend-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-3.0.0/PKG-INFO
```

### Comparing `population_trend-2.0.2/README.md` & `population_trend-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `population_trend-2.0.2/population_trend/cli.py` & `population_trend-3.0.0/population_trend/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     fit_data = pd.read_csv(data_path)
     with open(intervals_path, "r") as read_file:
         intervals_json = json.load(read_file)
     intervals = intervals_json["intervals"]
     lambda_latex = intervals_json["lambda_latex_interval"]
 
     Modelo_Tendencia_Poblacional = Population_Trend_Model(fit_data, intervals, variable_of_interest)
-    Graficador = Plotter_Population_Trend_Model()
+    Graficador = Plotter_Population_Trend_Model(fit_data)
     Graficador.plot_smooth(Modelo_Tendencia_Poblacional)
     Graficador.plot_model(Modelo_Tendencia_Poblacional)
-    Graficador.plot_data(Modelo_Tendencia_Poblacional, fit_data[variable_of_interest])
+    Graficador.plot_data(variable_of_interest)
     legend_mpl_object = Graficador.set_legend_location(island)
-    Graficador.set_x_lim(Modelo_Tendencia_Poblacional)
+    Graficador.set_x_lim()
     Graficador.set_y_lim(fit_data[variable_of_interest])
     Graficador.set_labels()
-    Graficador.set_ticks(Modelo_Tendencia_Poblacional)
+    Graficador.set_ticks()
     Graficador.draw()
     Graficador.plot_growth_rate_interval(legend_mpl_object, lambda_latex)
     Graficador.savefig(island, output_path)
```

### Comparing `population_trend-2.0.2/population_trend/population_growth_model.py` & `population_trend-3.0.0/population_trend/population_growth_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,85 @@
 import numpy as np
 from geci_plots import geci_plot, roundup, ticks_positions_array, order_magnitude
 from bootstrapping_tools import power_law, lambda_calculator
 import matplotlib.pyplot as plt
 
 
-def resample_seasons(df):
+def normalize_seasons(df):
     first_season = int(df.Temporada.min())
     last_season = int(df.Temporada.max())
     return np.linspace(first_season, last_season, last_season - first_season + 1).astype(int)
 
 
+def calculate_model_domain(data):
+    last_value = data.Temporada.max() - data.Temporada.min()
+    return np.linspace(0, last_value, 100)
+
+
 def calculate_upper_limit(data_interest_variable):
     upper_limit = roundup(
         data_interest_variable.max() * 1.2,
         10 ** order_magnitude(data_interest_variable),
     )
     return upper_limit
 
 
 class Population_Trend_Model:
     def __init__(self, fit_data, intervals, interest_variable):
         self.intervals = intervals
-        self.plot_seasons = fit_data["Temporada"][:] - fit_data["Temporada"].iloc[0] + 1
-        self.ticks_text = resample_seasons(fit_data)
-        self.ticks_positions = ticks_positions_array(self.ticks_text)
-        self.time_to_model = np.linspace(
-            self.ticks_positions.min(), self.ticks_positions.max(), 100
-        )
+        self.model_domain = calculate_model_domain(fit_data)
         self.initial_population = lambda_calculator(
             fit_data["Temporada"], fit_data[interest_variable]
         )[1]
 
     @property
     def model_min(self):
-        return power_law(self.time_to_model, self.intervals[0], self.initial_population)
+        return power_law(self.model_domain, self.intervals[0], self.initial_population)
 
     @property
     def model_med(self):
-        return power_law(self.time_to_model, self.intervals[1], self.initial_population)
+        return power_law(self.model_domain, self.intervals[1], self.initial_population)
 
     @property
     def model_max(self):
-        return power_law(self.time_to_model, self.intervals[2], self.initial_population)
+        return power_law(self.model_domain, self.intervals[2], self.initial_population)
 
 
 class Plotter_Population_Trend_Model:
-    def __init__(self):
+    def __init__(self, data):
         self.fig, self.ax = geci_plot()
+        self.data = data
+        self.plot_seasons = self.data["Temporada"][:] - self.data["Temporada"].iloc[0] + 1
+        self.ticks_text = normalize_seasons(self.data)
+        self.ticks_positions = ticks_positions_array(self.ticks_text)
+        self.plot_domain = np.linspace(self.ticks_positions.min(), self.ticks_positions.max(), 100)
 
     def plot_smooth(self, Population_Trend_Model):
         self.ax.fill_between(
-            Population_Trend_Model.time_to_model,
+            self.plot_domain,
             Population_Trend_Model.model_min,
             Population_Trend_Model.model_max,
             alpha=0.2,
             label="Confidence zone",
             color="b",
         )
 
     def plot_model(self, Population_Trend_Model):
         plt.plot(
-            Population_Trend_Model.time_to_model,
+            self.plot_domain,
             Population_Trend_Model.model_med,
             label="Population growth model",
             color="b",
         )
         return self.fig
 
-    def plot_data(self, Population_Trend_Model, fit_data):
+    def plot_data(self, variable_to_bootstrap):
         plt.plot(
-            Population_Trend_Model.plot_seasons,
-            fit_data,
+            self.plot_seasons,
+            self.data[variable_to_bootstrap],
             "-Dk",
             label="Active Nests",
         )
 
     def plot_growth_rate_interval(self, legend_mpl_object, lambda_latex):
         legend_box_positions = legend_mpl_object.get_window_extent()
         self.ax.annotate(
@@ -88,28 +93,28 @@
 
     def set_y_lim(self, fit_data):
         self.ax.set_ylim(
             0,
             calculate_upper_limit(fit_data),
         )
 
-    def set_x_lim(self, Population_Trend_Model):
+    def set_x_lim(self):
         plt.xlim(
-            Population_Trend_Model.ticks_positions.min() - 0.2,
-            Population_Trend_Model.ticks_positions.max(),
+            self.ticks_positions.min() - 0.2,
+            self.ticks_positions.max(),
         )
 
     def set_labels(self):
         plt.ylabel("Number of breeding pairs", size=20)
         plt.xlabel("Seasons", size=20)
 
-    def set_ticks(self, Population_Trend_Model):
+    def set_ticks(self):
         plt.xticks(
-            Population_Trend_Model.ticks_positions,
-            Population_Trend_Model.ticks_text,
+            self.ticks_positions,
+            self.ticks_text,
             rotation=90,
             size=20,
         )
         plt.yticks(size=20)
 
     def draw(self):
         plt.gcf().subplots_adjust(bottom=0.2)
```

### Comparing `population_trend-2.0.2/PKG-INFO` & `population_trend-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: population_trend
-Version: 2.0.2
+Version: 3.0.0
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
-Metadata-Version: 2.1 Name: population_trend Version: 2.0.2 Summary: A template
+Metadata-Version: 2.1 Name: population_trend Version: 3.0.0 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/population_trend Author:
 Ciencia de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-
 Python: >=3.9 Description-Content-Type: text/markdown Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
 bootstrapping-tools==1.1.1 Requires-Dist: geci-plots Requires-Dist: typer
 [https://www.islas.org.mx/img/logo.svg] # Dummy Transformations Para usar este
 repo como plantilla debemos hacer lo siguiente: 1. Presiona el botÃ³n verde que
```

