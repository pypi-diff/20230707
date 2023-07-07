# Comparing `tmp/combidata-0.2.1.2.tar.gz` & `tmp/combidata-0.2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combidata-0.2.1.2.tar", last modified: Sat Jul  1 13:05:10 2023, max compression
+gzip compressed data, was "combidata-0.2.1.3.tar", last modified: Fri Jul  7 17:26:10 2023, max compression
```

## Comparing `combidata-0.2.1.2.tar` & `combidata-0.2.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 13:05:10.019649 combidata-0.2.1.2/
--rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.1.2/LICENSE
--rw-rw-rw-   0        0        0    10467 2023-07-01 13:05:10.018649 combidata-0.2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9684 2023-06-30 14:16:48.000000 combidata-0.2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 13:05:09.864072 combidata-0.2.1.2/combidata/
--rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.1.2/combidata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:05:10.009654 combidata-0.2.1.2/combidata/classes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1.2/combidata/classes/__init__.py
--rw-rw-rw-   0        0        0     2831 2023-04-01 06:03:08.000000 combidata-0.2.1.2/combidata/classes/case.py
--rw-rw-rw-   0        0        0     2458 2023-07-01 13:04:26.000000 combidata-0.2.1.2/combidata/classes/combination.py
--rw-rw-rw-   0        0        0     6255 2023-06-30 14:01:33.000000 combidata-0.2.1.2/combidata/classes/data_generator.py
--rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.1.2/combidata/classes/process.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:05:10.015649 combidata-0.2.1.2/combidata/processes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1.2/combidata/processes/__init__.py
--rw-rw-rw-   0        0        0     5249 2023-04-01 05:47:28.000000 combidata-0.2.1.2/combidata/processes/combine.py
--rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.1.2/combidata/processes/form.py
--rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.1.2/combidata/processes/genetate.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:05:09.888589 combidata-0.2.1.2/combidata.egg-info/
--rw-rw-rw-   0        0        0    10467 2023-07-01 13:05:09.000000 combidata-0.2.1.2/combidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-01 13:05:09.000000 combidata-0.2.1.2/combidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 13:05:09.000000 combidata-0.2.1.2/combidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-01 13:05:09.000000 combidata-0.2.1.2/combidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      555 2023-07-01 13:04:26.000000 combidata-0.2.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 13:05:10.019649 combidata-0.2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-07-01 13:04:26.000000 combidata-0.2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:05:10.017650 combidata-0.2.1.2/tests/
--rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.1.2/tests/test_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.940743 combidata-0.2.1.3/
+-rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.1.3/LICENSE
+-rw-rw-rw-   0        0        0    10467 2023-07-07 17:26:10.939745 combidata-0.2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9684 2023-06-30 14:16:48.000000 combidata-0.2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.903745 combidata-0.2.1.3/combidata/
+-rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.1.3/combidata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.931744 combidata-0.2.1.3/combidata/classes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1.3/combidata/classes/__init__.py
+-rw-rw-rw-   0        0        0     2831 2023-04-01 06:03:08.000000 combidata-0.2.1.3/combidata/classes/case.py
+-rw-rw-rw-   0        0        0     3071 2023-07-07 15:54:44.000000 combidata-0.2.1.3/combidata/classes/combination.py
+-rw-rw-rw-   0        0        0     6255 2023-06-30 14:01:33.000000 combidata-0.2.1.3/combidata/classes/data_generator.py
+-rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.1.3/combidata/classes/process.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.936748 combidata-0.2.1.3/combidata/processes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1.3/combidata/processes/__init__.py
+-rw-rw-rw-   0        0        0     5249 2023-04-01 05:47:28.000000 combidata-0.2.1.3/combidata/processes/combine.py
+-rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.1.3/combidata/processes/form.py
+-rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.1.3/combidata/processes/genetate.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.924744 combidata-0.2.1.3/combidata.egg-info/
+-rw-rw-rw-   0        0        0    10467 2023-07-07 17:26:10.000000 combidata-0.2.1.3/combidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-07 17:26:10.000000 combidata-0.2.1.3/combidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:26:10.000000 combidata-0.2.1.3/combidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 17:26:10.000000 combidata-0.2.1.3/combidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      555 2023-07-07 17:22:34.000000 combidata-0.2.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:26:10.940743 combidata-0.2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-07-07 17:22:34.000000 combidata-0.2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:26:10.938744 combidata-0.2.1.3/tests/
+-rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.1.3/tests/test_generator.py
```

### Comparing `combidata-0.2.1.2/LICENSE` & `combidata-0.2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1.2/PKG-INFO` & `combidata-0.2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.1.2
+Version: 0.2.1.3
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `combidata-0.2.1.2/README.md` & `combidata-0.2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1.2/combidata/classes/case.py` & `combidata-0.2.1.3/combidata/classes/case.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1.2/combidata/classes/combination.py` & `combidata-0.2.1.3/combidata/classes/combination.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import traceback
+
+
 def step_not_done(current_step_name, combi):
     if isinstance(combi, list):
         for combination in combi:
             if combination.step_done != current_step_name and combination.step_done != "STOP":
                 return True
     else:
         if combi.step_done != current_step_name and combi.step_done != "STOP":
@@ -56,14 +59,22 @@
                     if start_step := self.tools.get("start_step"):
                         start_step(self.tools.get("id"), current_step.name)
                     try:
                         current_step.activate(self)
                     except Exception as e:
                         self.step_done = "STOP"
                         if end_step := self.tools.get("end_step"):
-                            end_step(self.tools.get("id"), str(e))
+                            temp_exep = f"An exception occurred: {type(e).__name__}. "
+                            temp_exep += f"Error message: {str(e)}. "
+                            traceback_list = traceback.extract_tb(e.__traceback__)
+                            if traceback_list:
+                                last_traceback = traceback_list[-1]
+                                file_name = last_traceback.filename
+                                line_number = last_traceback.lineno
+                                temp_exep += f"Occurred at: {file_name}:{line_number}. "
+                            end_step(self.tools.get("id"), temp_exep)
                         else:
                             raise e
                     else:
                         if end_step := self.tools.get("end_step"):
                             end_step(self.tools.get("id"))
```

### Comparing `combidata-0.2.1.2/combidata/classes/data_generator.py` & `combidata-0.2.1.3/combidata/classes/data_generator.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1.2/combidata/processes/combine.py` & `combidata-0.2.1.3/combidata/processes/combine.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1.2/combidata/processes/form.py` & `combidata-0.2.1.3/combidata/processes/form.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1.2/combidata/processes/genetate.py` & `combidata-0.2.1.3/combidata/processes/genetate.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1.2/combidata.egg-info/PKG-INFO` & `combidata-0.2.1.3/combidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.1.2
+Version: 0.2.1.3
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `combidata-0.2.1.2/pyproject.toml` & `combidata-0.2.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     "testing API",
     "testing",
     "autotesting"
 ]
 urls = {Homepage = "https://github.com/Warrfie/combidata"}
 authors = [{name = "MaximKuklikov(Warrfie)", email = "warrfie@gmail.com"}]
 requires-python = ">=3.10"
-version="0.2.1.2"
+version="0.2.1.3"
```

### Comparing `combidata-0.2.1.2/setup.py` & `combidata-0.2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="combidata",
-    version="0.2.1.2",
+    version="0.2.1.3",
     description="Package for random data generation and combination different cases",
     long_description=long_description,
     url="https://github.com/Warrfie/combidata",
     author="Kuklikov Maxim (Warrfie)",
     author_email="warrfie@gmail.com",
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `combidata-0.2.1.2/tests/test_generator.py` & `combidata-0.2.1.3/tests/test_generator.py`

 * *Files identical despite different names*

