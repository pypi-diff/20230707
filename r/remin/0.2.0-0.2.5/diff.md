# Comparing `tmp/remin-0.2.0.tar.gz` & `tmp/remin-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remin-0.2.0.tar", last modified: Tue Jun 27 19:12:03 2023, max compression
+gzip compressed data, was "remin-0.2.5.tar", last modified: Thu Jul  6 21:01:34 2023, max compression
```

## Comparing `remin-0.2.0.tar` & `remin-0.2.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.071271 remin-0.2.0/
--rw-rw-r--   0 salih     (1000) salih     (1000)     1854 2023-06-22 11:31:23.000000 remin-0.2.0/.gitignore
--rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.2.0/LICENSE
--rw-rw-r--   0 salih     (1000) salih     (1000)      349 2023-04-17 09:36:47.000000 remin-0.2.0/Makefile
--rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-06-27 19:12:03.071271 remin-0.2.0/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)     2625 2023-04-17 01:40:58.000000 remin-0.2.0/README.md
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.067271 remin-0.2.0/examples/
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.067271 remin-0.2.0/examples/heat/
--rw-rw-r--   0 salih     (1000) salih     (1000)      526 2023-04-25 20:20:42.000000 remin-0.2.0/examples/heat/model.py
--rw-rw-r--   0 salih     (1000) salih     (1000)      760 2023-04-25 20:35:46.000000 remin-0.2.0/examples/heat/postprocess.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1515 2023-05-06 19:07:30.000000 remin-0.2.0/examples/heat/training.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.067271 remin-0.2.0/examples/schrodinger/
--rw-rw-r--   0 salih     (1000) salih     (1000)     1918 2023-06-22 11:46:30.000000 remin-0.2.0/examples/schrodinger/functrain.py
--rw-rw-r--   0 salih     (1000) salih     (1000)      373 2023-06-22 11:37:25.000000 remin-0.2.0/examples/schrodinger/model.py
--rw-rw-r--   0 salih     (1000) salih     (1000)      834 2023-06-22 11:39:25.000000 remin-0.2.0/examples/schrodinger/postprocess.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1912 2023-06-22 11:40:09.000000 remin-0.2.0/examples/schrodinger/train.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.067271 remin-0.2.0/examples/wave/
--rw-rw-r--   0 salih     (1000) salih     (1000)      562 2023-06-22 11:54:24.000000 remin-0.2.0/examples/wave/model.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1605 2023-06-22 11:54:24.000000 remin-0.2.0/examples/wave/postprocess.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     2100 2023-06-22 11:54:24.000000 remin-0.2.0/examples/wave/train.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     2144 2023-06-22 11:54:24.000000 remin-0.2.0/examples/wave/train_batched.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1295 2023-06-27 15:23:02.000000 remin-0.2.0/pyproject.toml
--rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.2.0/requirements.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-06-27 19:12:03.071271 remin-0.2.0/setup.cfg
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.067271 remin-0.2.0/src/
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.071271 remin-0.2.0/src/remin/
--rw-rw-r--   0 salih     (1000) salih     (1000)     7272 2023-06-27 15:22:50.000000 remin-0.2.0/src/remin/__init__.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     5795 2023-05-23 18:09:37.000000 remin-0.2.0/src/remin/callbacks.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     7307 2023-06-22 12:01:19.000000 remin-0.2.0/src/remin/domain.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1045 2023-05-11 10:55:40.000000 remin-0.2.0/src/remin/func.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     5286 2023-06-22 10:30:58.000000 remin-0.2.0/src/remin/residual.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.071271 remin-0.2.0/src/remin/solver/
--rw-rw-r--   0 salih     (1000) salih     (1000)      117 2023-05-08 21:15:07.000000 remin-0.2.0/src/remin/solver/__init__.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1794 2023-05-11 14:29:44.000000 remin-0.2.0/src/remin/solver/residual_loss.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     3456 2023-05-23 18:12:53.000000 remin-0.2.0/src/remin/solver/solver.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     3475 2023-05-11 14:29:36.000000 remin-0.2.0/src/remin/solver/trainer.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-06-27 19:12:03.071271 remin-0.2.0/src/remin.egg-info/
--rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)      806 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/SOURCES.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/dependency_links.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       37 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/entry_points.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/requires.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-06-27 19:12:03.000000 remin-0.2.0/src/remin.egg-info/top_level.txt
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-07-06 21:01:34.457101 remin-0.2.5/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1854 2023-06-22 11:31:23.000000 remin-0.2.5/.gitignore
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.2.5/LICENSE
+-rw-rw-r--   0 salih     (1000) salih     (1000)      349 2023-04-17 09:36:47.000000 remin-0.2.5/Makefile
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3176 2023-07-06 21:01:34.457101 remin-0.2.5/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)     2637 2023-07-06 20:57:43.000000 remin-0.2.5/README.md
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-07-06 21:01:34.453101 remin-0.2.5/examples/
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-07-06 21:01:34.453101 remin-0.2.5/examples/heat/
+-rw-rw-r--   0 salih     (1000) salih     (1000)      526 2023-04-25 20:20:42.000000 remin-0.2.5/examples/heat/model.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      760 2023-04-25 20:35:46.000000 remin-0.2.5/examples/heat/postprocess.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1515 2023-05-06 19:07:30.000000 remin-0.2.5/examples/heat/training.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-07-06 21:01:34.457101 remin-0.2.5/examples/schrodinger/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1918 2023-06-22 11:46:30.000000 remin-0.2.5/examples/schrodinger/functrain.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      373 2023-06-22 11:37:25.000000 remin-0.2.5/examples/schrodinger/model.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      834 2023-06-22 11:39:25.000000 remin-0.2.5/examples/schrodinger/postprocess.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1912 2023-06-22 11:40:09.000000 remin-0.2.5/examples/schrodinger/train.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-07-06 21:01:34.457101 remin-0.2.5/examples/wave/
+-rw-rw-r--   0 salih     (1000) salih     (1000)      562 2023-06-22 11:54:24.000000 remin-0.2.5/examples/wave/model.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1605 2023-06-22 11:54:24.000000 remin-0.2.5/examples/wave/postprocess.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     2100 2023-06-22 11:54:24.000000 remin-0.2.5/examples/wave/train.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     2144 2023-06-22 11:54:24.000000 remin-0.2.5/examples/wave/train_batched.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1295 2023-07-06 20:59:38.000000 remin-0.2.5/pyproject.toml
+-rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.2.5/requirements.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-07-06 21:01:34.457101 remin-0.2.5/setup.cfg
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-07-06 21:01:34.453101 remin-0.2.5/src/
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-07-06 21:01:34.457101 remin-0.2.5/src/remin/
+-rw-rw-r--   0 salih     (1000) salih     (1000)    11479 2023-07-06 20:59:31.000000 remin-0.2.5/src/remin/__init__.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     7977 2023-07-06 20:58:23.000000 remin-0.2.5/src/remin/callbacks.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     7307 2023-06-22 12:01:19.000000 remin-0.2.5/src/remin/domain.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1045 2023-05-11 10:55:40.000000 remin-0.2.5/src/remin/func.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     5286 2023-06-22 10:30:58.000000 remin-0.2.5/src/remin/residual.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-07-06 21:01:34.457101 remin-0.2.5/src/remin/solver/
+-rw-rw-r--   0 salih     (1000) salih     (1000)      117 2023-05-08 21:15:07.000000 remin-0.2.5/src/remin/solver/__init__.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1794 2023-05-11 14:29:44.000000 remin-0.2.5/src/remin/solver/residual_loss.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3588 2023-07-06 19:57:34.000000 remin-0.2.5/src/remin/solver/solver.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3475 2023-05-11 14:29:36.000000 remin-0.2.5/src/remin/solver/trainer.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-07-06 21:01:34.457101 remin-0.2.5/src/remin.egg-info/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3176 2023-07-06 21:01:34.000000 remin-0.2.5/src/remin.egg-info/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)      806 2023-07-06 21:01:34.000000 remin-0.2.5/src/remin.egg-info/SOURCES.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-07-06 21:01:34.000000 remin-0.2.5/src/remin.egg-info/dependency_links.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       37 2023-07-06 21:01:34.000000 remin-0.2.5/src/remin.egg-info/entry_points.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-07-06 21:01:34.000000 remin-0.2.5/src/remin.egg-info/requires.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-07-06 21:01:34.000000 remin-0.2.5/src/remin.egg-info/top_level.txt
```

### Comparing `remin-0.2.0/.gitignore` & `remin-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/LICENSE` & `remin-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/examples/heat/model.py` & `remin-0.2.5/examples/heat/model.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/examples/heat/postprocess.py` & `remin-0.2.5/examples/heat/postprocess.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/examples/heat/training.py` & `remin-0.2.5/examples/heat/training.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/examples/schrodinger/functrain.py` & `remin-0.2.5/examples/schrodinger/functrain.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/examples/schrodinger/postprocess.py` & `remin-0.2.5/examples/schrodinger/postprocess.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/examples/schrodinger/train.py` & `remin-0.2.5/examples/schrodinger/train.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/examples/wave/model.py` & `remin-0.2.5/examples/wave/model.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/examples/wave/postprocess.py` & `remin-0.2.5/examples/wave/postprocess.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/examples/wave/train.py` & `remin-0.2.5/examples/wave/train.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/examples/wave/train_batched.py` & `remin-0.2.5/examples/wave/train_batched.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/pyproject.toml` & `remin-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "remin"
-version = "0.2.0"
+version = "0.2.5"
 authors = [
     { name="Salih Taşdelen", email="salih.tasdelen@hotmail.com"},
 ]
 description = "PINN solver implemented in Pytorch"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `remin-0.2.0/src/remin/callbacks.py` & `remin-0.2.5/src/remin/callbacks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from time import thread_time
 from typing import Dict, List, Any
 import numpy as np
 import matplotlib.pyplot as plt
+import csv
 
 
 class Callback:
     # Callback interface
     def __init__(self) -> None:
         self.state_dict: Dict[str, Any] = {}
 
@@ -65,15 +66,15 @@
         super().__init__()
         self.t0 = 0
 
     def on_train_begin(self):
         self.t0 = thread_time()
 
     def on_train_end(self):
-        print(f'Total training time: {((thread_time() - self.t0) / 60):7.3f}mins.')
+        print(f'\nTotal training time: {((thread_time() - self.t0) / 60):7.3f}mins.')
 
 
 class LogCallback(Callback):
 
     def __init__(self, log_epoch=100, log_progress=10) -> None:
         super().__init__()
         self.log_epoch = log_epoch
@@ -87,25 +88,31 @@
 
     def on_epoch_begin(self):
         self.t0 = thread_time()
 
     def on_epoch_end(self):
         epoch = self.state_dict['epoch']
         epochs = self.state_dict['epochs']
-        resloss = self.state_dict['resloss']
-        metloss = self.state_dict['metloss']
+        resloss = self.state_dict['residual']
+        metloss = self.state_dict['metric']
 
         self.t_ave = (self.t_ave * epoch + (thread_time() - self.t0)) / (epoch + 1)
         if epoch % self.log_progress == 0:
             prefix = f'Loss: {resloss:10.6f}'
             if self.metric:
                 prefix += f' - Metric Loss: {metloss:10.6f}'
             self._printProgress(epoch, epochs, self.log_epoch, prefix,
                                 f'{(self.t_ave*1e3):7.3f}ms/epoch')
 
+    def on_train_end(self):
+        if self.state_dict['epoch'] == self.state_dict['epochs']:
+            print(
+                f'\nTraining over:\n\tBest Loss Achieved: {self.state_dict["best"]:10.6f}'
+            )
+
     @staticmethod
     def _printProgress(epoch,
                        epochs,
                        log_epoch,
                        prefix='',
                        suffix='',
                        length=20,
@@ -126,15 +133,15 @@
     def __init__(self, best_suffix='_best.pt', final_suffix='_final.pt') -> None:
         super().__init__()
         self.best_loss = float('inf')
         self.best_suffix = best_suffix
         self.final_suffix = final_suffix
 
     def on_epoch_end(self):
-        resloss = self.state_dict['resloss']
+        resloss = self.state_dict['residual']
         epoch = self.state_dict['epoch']
         solver = self.state_dict['solver']
         if resloss < self.best_loss:
             self.best_loss = resloss
             solver.save(epoch, self.best_suffix)
 
     def on_train_end(self):
@@ -142,15 +149,15 @@
         epoch = self.state_dict['epoch']
         solver.save(epoch, self.final_suffix)
 
 
 class PlotCallback(Callback):
 
     def __init__(self,
-                 state='resloss',
+                 state='residual',
                  size_inches=(10, 5),
                  color='red',
                  linestyle='-',
                  linewidth=2,
                  title='Residual Loss(L)',
                  ylabel='Loss',
                  xlabel='Epoch',
@@ -181,15 +188,71 @@
     def on_epoch_end(self):
         self.losses[self.state_dict['epoch'] - 1] = self.state_dict[self.state]
 
     def on_train_end(self):
         fig, ax = plt.subplots(1, 1)
         if self.size_inches:
             fig.set_size_inches(*self.size_inches)
-        ax.plot(self.losses,
+        ax.plot(self.losses[:self.state_dict['epoch']],
                 color=self.color,
                 linestyle=self.linestyle,
                 linewidth=self.linewidth)
         ax.set_yscale(self.yscale)
         ax.set(title=self.title, ylabel=self.ylabel, xlabel=self.xlabel)
         ax.grid(self.grid_on)
         plt.savefig(self.save_path + self.fig_name, dpi=self.dpi)
+
+
+class CSVCallback(Callback):
+
+    def __init__(self, name: str = 'training_data.csv') -> None:
+        super().__init__()
+        self.name = name
+        self.fields = ['epoch', 'residual', 'metric']
+
+    def on_train_begin(self):
+        self.data = np.zeros((self.state_dict['epochs'], len(self.fields)))
+        self.save_path = self.state_dict['solver'].save_path
+
+    def on_epoch_end(self):
+        for i, field in enumerate(self.fields):
+            self.data[self.state_dict['epoch'] - 1, i] = self.state_dict[field]
+
+    def on_train_end(self):
+        with open(self.save_path + '/' + self.name, 'w') as csvfile:
+            csvwriter = csv.writer(csvfile)
+
+            csvwriter.writerow(self.fields)
+            csvwriter.writerows(self.data[:self.state_dict['epoch']])
+
+
+class EarlyStoppingCallback(Callback):
+
+    def __init__(self, min_delta=0, patience=8, restore_best_weights=False) -> None:
+        super().__init__()
+        self.min_delta = min_delta
+        self.max_patience = patience
+        self.patience = 0
+        self.restore_best_weights = restore_best_weights
+        self.saved_loss = float('inf')
+        self.best_loss = float('inf')
+
+    def on_epoch_end(self):
+        resloss = self.state_dict['residual']
+
+        if self.patience >= self.max_patience:
+            print(
+                f'''\nEarly Stopping at {self.state_dict['epoch']}/{self.state_dict['epochs']}:
+        Residual Loss: {resloss:10.6f}
+        Saved Loss:    {self.saved_loss:10.6f}
+        Best Loss:     {self.best_loss:10.6f}''')
+            return 1
+
+        if (self.saved_loss - resloss) / resloss * 100 > self.min_delta:
+            self.patience = 0
+            if self.restore_best_weights:
+                self.saved_loss = self.state_dict['best']
+            else:
+                self.saved_loss = resloss
+        else:
+            #print(resloss - self.saved_loss)
+            self.patience += 1
```

### Comparing `remin-0.2.0/src/remin/domain.py` & `remin-0.2.5/src/remin/domain.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/src/remin/func.py` & `remin-0.2.5/src/remin/func.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/src/remin/residual.py` & `remin-0.2.5/src/remin/residual.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/src/remin/solver/residual_loss.py` & `remin-0.2.5/src/remin/solver/residual_loss.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/src/remin/solver/solver.py` & `remin-0.2.5/src/remin/solver/solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,17 @@
         if callbacks is None:
             callbacks = [SaveCallback(), LogCallback()]
 
         self.state_dict = {
             'solver': self,
             'epoch': None,
             'epochs': None,
-            'resloss': None,
-            'metloss': None
+            'residual': None,
+            'metric': None,
+            'best': float('inf')
         }
         self.callback = UnionCallback(self.state_dict, *callbacks)
 
     def load(self, filename):
         assert self.model is not None
         state_dict = torch.load(filename)
         self.model.load_state_dict(state_dict['model_state_dict'])
@@ -83,15 +84,17 @@
 
         self.update_state(epochs=epochs)
 
         self.callback.on_train_begin()
         for epoch in range(1, epochs + 1):
             self.callback.on_epoch_begin()
             resloss = self.trainer()
+            if resloss < self.state_dict['best']:
+                self.update_state(best=resloss)
             if self.trainer.metric_loss:
                 metloss = self.trainer.eval_loss()
-                self.update_state(metloss=metloss)
-            self.update_state(resloss=resloss, epoch=epoch)
+                self.update_state(metric=metloss)
+            self.update_state(residual=resloss, epoch=epoch)
             if self.callback.on_epoch_end():
                 break
         self.callback.on_train_end()
         self.epoch = epoch
```

### Comparing `remin-0.2.0/src/remin/solver/trainer.py` & `remin-0.2.5/src/remin/solver/trainer.py`

 * *Files identical despite different names*

### Comparing `remin-0.2.0/src/remin.egg-info/SOURCES.txt` & `remin-0.2.5/src/remin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

