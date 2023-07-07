# Comparing `tmp/pyappbundler-0.1.2.tar.gz` & `tmp/pyappbundler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappbundler-0.1.2.tar", last modified: Thu Jul  6 15:32:58 2023, max compression
+gzip compressed data, was "pyappbundler-0.1.3.tar", last modified: Thu Jul  6 15:44:44 2023, max compression
```

## Comparing `pyappbundler-0.1.2.tar` & `pyappbundler-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 15:32:58.926449 pyappbundler-0.1.2/
--rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      730 2023-07-06 15:32:58.926449 pyappbundler-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 15:32:58.920447 pyappbundler-0.1.2/pyappbundler/
--rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.2/pyappbundler/__init__.py
--rw-rw-rw-   0        0        0     2544 2023-07-06 15:29:57.000000 pyappbundler-0.1.2/pyappbundler/__main__.py
--rw-rw-rw-   0        0        0       22 2023-07-06 15:07:54.000000 pyappbundler-0.1.2/pyappbundler/_version.py
--rw-rw-rw-   0        0        0     4879 2023-07-06 15:06:52.000000 pyappbundler-0.1.2/pyappbundler/pyappbundler.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:32:58.925448 pyappbundler-0.1.2/pyappbundler/templates/
--rw-rw-rw-   0        0        0     1537 2023-07-05 15:18:33.000000 pyappbundler-0.1.2/pyappbundler/templates/iss.tmpl
-drwxrwxrwx   0        0        0        0 2023-07-06 15:32:58.924448 pyappbundler-0.1.2/pyappbundler.egg-info/
--rw-rw-rw-   0        0        0      730 2023-07-06 15:32:58.000000 pyappbundler-0.1.2/pyappbundler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-06 15:32:58.000000 pyappbundler-0.1.2/pyappbundler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 15:32:58.000000 pyappbundler-0.1.2/pyappbundler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-06 15:32:58.000000 pyappbundler-0.1.2/pyappbundler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-06 15:32:58.000000 pyappbundler-0.1.2/pyappbundler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 15:32:58.926449 pyappbundler-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:44:44.851300 pyappbundler-0.1.3/
+-rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      730 2023-07-06 15:44:44.850299 pyappbundler-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 15:44:44.846298 pyappbundler-0.1.3/pyappbundler/
+-rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.3/pyappbundler/__init__.py
+-rw-rw-rw-   0        0        0     2544 2023-07-06 15:29:57.000000 pyappbundler-0.1.3/pyappbundler/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-07-06 15:43:29.000000 pyappbundler-0.1.3/pyappbundler/_version.py
+-rw-rw-rw-   0        0        0     4834 2023-07-06 15:43:44.000000 pyappbundler-0.1.3/pyappbundler/pyappbundler.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:44:44.850299 pyappbundler-0.1.3/pyappbundler/templates/
+-rw-rw-rw-   0        0        0     1537 2023-07-05 15:18:33.000000 pyappbundler-0.1.3/pyappbundler/templates/iss.tmpl
+drwxrwxrwx   0        0        0        0 2023-07-06 15:44:44.849299 pyappbundler-0.1.3/pyappbundler.egg-info/
+-rw-rw-rw-   0        0        0      730 2023-07-06 15:44:44.000000 pyappbundler-0.1.3/pyappbundler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-06 15:44:44.000000 pyappbundler-0.1.3/pyappbundler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:44:44.000000 pyappbundler-0.1.3/pyappbundler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-06 15:44:44.000000 pyappbundler-0.1.3/pyappbundler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 15:44:44.000000 pyappbundler-0.1.3/pyappbundler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:44:44.851300 pyappbundler-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.3/setup.py
```

### Comparing `pyappbundler-0.1.2/LICENSE` & `pyappbundler-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.2/PKG-INFO` & `pyappbundler-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.2
+Version: 0.1.3
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.2/pyappbundler/__main__.py` & `pyappbundler-0.1.3/pyappbundler/__main__.py`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.2/pyappbundler/pyappbundler.py` & `pyappbundler-0.1.3/pyappbundler/pyappbundler.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,38 +59,38 @@
         self.dist, self.build = Path(dist).resolve(), Path(build).resolve()
 
         self.res_dirs, self.pyinst_flags = res_dirs, pyinst_flags
         self.no_clean_dist = no_clean_dist
 
     def clean_dist(self):
         if self.no_clean_dist:
-            logging.info(f'Cancel cleaning "{self.dist_path}" directory.')
+            logging.info(f'Cancel cleaning "{self.dist}" directory.')
             return self
 
         #
-        logging.info(f'Cleaning "{self.dist_path}" directory...')
+        logging.info(f'Cleaning "{self.dist}" directory...')
 
-        if not self.dist_path.exists():
-            self.dist_path.mkdir(parents=True)
+        if not self.dist.exists():
+            self.dist.mkdir(parents=True)
             logging.info(
-                f'"{self.dist_path}" directory doesn\'t exist!'
+                f'"{self.dist}" directory doesn\'t exist!'
                 ' The new one has been created.')
             return
 
-        if not self.dist_path.is_dir():
+        if not self.dist.is_dir():
             raise FileNotFoundError(
-                f'Directory expected, but "{self.dist_path}" is not!')
+                f'Directory expected, but "{self.dist}" is not!')
 
-        for path in self.dist_path.iterdir():
+        for path in self.dist.iterdir():
             if path.is_file():
                 path.unlink()
             elif path.is_dir():
                 shutil.rmtree(path)
 
-        logging.info(f'"{self.dist_path}" directory has been cleaned!\n')
+        logging.info(f'"{self.dist}" directory has been cleaned!\n')
 
         return self
 
     def build_exe(self):
         logging.info(f'Building exe with PyInstaller...')
 
         args = [
```

### Comparing `pyappbundler-0.1.2/pyappbundler/templates/iss.tmpl` & `pyappbundler-0.1.3/pyappbundler/templates/iss.tmpl`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.2/pyappbundler.egg-info/PKG-INFO` & `pyappbundler-0.1.3/pyappbundler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.2
+Version: 0.1.3
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.2/pyproject.toml` & `pyappbundler-0.1.3/pyproject.toml`

 * *Files identical despite different names*

