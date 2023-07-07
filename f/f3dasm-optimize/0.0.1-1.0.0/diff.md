# Comparing `tmp/f3dasm_optimize-0.0.1.tar.gz` & `tmp/f3dasm_optimize-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/martin/Documents/GitHub/f3dasm_optimize/dist/.tmp-c3i77eb9/f3dasm_optimize-0.0.1.tar", last modified: Wed Jun 14 13:05:16 2023, max compression
+gzip compressed data, was "f3dasm_optimize-1.0.0.tar", last modified: Fri Jul  7 13:50:58 2023, max compression
```

## Comparing `f3dasm_optimize-0.0.1.tar` & `f3dasm_optimize-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,43 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1511 2023-06-14 13:02:10.000000 f3dasm_optimize-0.0.1/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-06-14 13:00:50.000000 f3dasm_optimize-0.0.1/MANIFEST.in
--rw-rw-r--   0 martin    (1000) martin    (1000)     1757 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      970 2023-06-14 13:00:50.000000 f3dasm_optimize-0.0.1/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-06-14 13:00:50.000000 f3dasm_optimize-0.0.1/VERSION
--rw-rw-r--   0 martin    (1000) martin    (1000)      100 2023-06-14 13:00:50.000000 f3dasm_optimize-0.0.1/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-06-14 13:00:50.000000 f3dasm_optimize-0.0.1/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      985 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/src/f3dasm_optimize/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1003 2023-06-14 13:00:50.000000 f3dasm_optimize-0.0.1/src/f3dasm_optimize/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      859 2023-06-14 13:00:50.000000 f3dasm_optimize-0.0.1/src/f3dasm_optimize/example_module.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/src/f3dasm_optimize.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1757 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/src/f3dasm_optimize.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      343 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/src/f3dasm_optimize.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/src/f3dasm_optimize.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       16 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/src/f3dasm_optimize.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-14 13:05:16.000000 f3dasm_optimize-0.0.1/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)      102 2023-06-14 13:02:02.000000 f3dasm_optimize-0.0.1/tests/test_add_one.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:50:58.666439 f3dasm_optimize-1.0.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1511 2023-06-14 13:02:10.000000 f3dasm_optimize-1.0.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-06-14 13:00:50.000000 f3dasm_optimize-1.0.0/MANIFEST.in
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1777 2023-07-07 13:50:58.666439 f3dasm_optimize-1.0.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      970 2023-06-14 13:00:50.000000 f3dasm_optimize-1.0.0/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-07-07 13:47:50.000000 f3dasm_optimize-1.0.0/VERSION
+-rw-rw-r--   0 martin    (1000) martin    (1000)      100 2023-06-14 13:00:50.000000 f3dasm_optimize-1.0.0/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       92 2023-07-07 11:49:46.000000 f3dasm_optimize-1.0.0/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1005 2023-07-07 13:50:58.666439 f3dasm_optimize-1.0.0/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:50:58.662439 f3dasm_optimize-1.0.0/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:50:58.662439 f3dasm_optimize-1.0.0/src/f3dasm_optimize/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3095 2023-07-07 11:20:38.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2144 2023-06-16 09:08:46.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/_all_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5604 2023-07-07 11:20:21.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/_imports.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1296 2023-04-12 07:58:51.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/_protocol.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      251 2023-06-15 13:31:30.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/_version.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1780 2023-06-15 09:39:31.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/adam.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1690 2023-06-15 09:37:15.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/adamax.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:50:58.666439 f3dasm_optimize-1.0.0/src/f3dasm_optimize/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-11-03 14:34:52.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4745 2023-06-23 14:05:57.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/adapters/pygmo_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3422 2023-06-15 09:38:34.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/adapters/scipy_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4117 2023-07-07 11:23:59.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/adapters/tensorflow_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3629 2023-06-15 09:37:20.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/bayesianoptimization.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1612 2023-06-15 09:37:28.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/cmaes.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1396 2023-06-15 09:37:30.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/cobyla.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2243 2023-06-15 09:37:32.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/differentialevolution.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2132 2023-06-15 09:37:34.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/ftrl.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1688 2023-06-15 09:37:39.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/nadam.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1703 2023-06-15 09:37:42.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/pso.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1731 2023-06-15 09:37:51.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/rmsprop.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1856 2023-06-15 09:37:54.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/sade.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1512 2023-06-15 09:37:59.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/sea.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2059 2023-06-15 09:38:01.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/sga.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1594 2023-06-15 09:38:03.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/sgd.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1997 2023-06-15 09:38:05.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/simulatedannealing.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1992 2023-06-15 09:38:13.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize/xnes.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:50:58.666439 f3dasm_optimize-1.0.0/src/f3dasm_optimize.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1777 2023-07-07 13:50:58.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1169 2023-07-07 13:50:58.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-07 13:50:58.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       96 2023-07-07 13:50:58.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       16 2023-07-07 13:50:58.000000 f3dasm_optimize-1.0.0/src/f3dasm_optimize.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `f3dasm_optimize-0.0.1/LICENSE` & `f3dasm_optimize-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-0.0.1/PKG-INFO` & `f3dasm_optimize-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: f3dasm_optimize
-Version: 0.0.1
+Version: 1.0.0
 Summary: f3dasm_optimize: Your one line description of the package
 Home-page: https://github.com/bessagroup/f3dasm_optimize
-Author: Your Name
-Author-email: youremailadress@email.com
+Author: Martin van der Schelling
+Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD-3-Clause License
 Keywords: keyword1,keyword2,keyword3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href=""><img alt="logo" src="https://user-images.githubusercontent.com/25851824/200928507-a65327f9-bc70-4c12-beaa-bc6ba74d968e.svg" width="60%"></a>
 </p>
 
 ## Bessa Group Python repository template
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: f3dasm_optimize Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: f3dasm_optimize Version: 1.0.0 Summary:
 f3dasm_optimize: Your one line description of the package Home-page: https://
-github.com/bessagroup/f3dasm_optimize Author: Your Name Author-email:
-youremailadress@email.com License: BSD-3-Clause License Keywords:
+github.com/bessagroup/f3dasm_optimize Author: Martin van der Schelling Author-
+email: M.P.vanderSchelling@tudelft.nl License: BSD-3-Clause License Keywords:
 keyword1,keyword2,keyword3 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Requires-Python:
->=3.7 Description-Content-Type: text/markdown
+>=3.8 Description-Content-Type: text/markdown
                                     [logo]
 ## Bessa Group Python repository template **Authors**: - Martin van der
 Schelling ([M.P.vanderSchelling@tudelft.nl](mailto:
 M.P.vanderSchelling@tudelft.nl)) **Authors afilliation:** - Bessa Research
 Group @ Delft University of Technology **Maintainer:** - Martin van der
 Schelling ([M.P.vanderSchelling@tudelft.nl](mailto:
 M.P.vanderSchelling@tudelft.nl)) **Maintainer afilliation:** - Bessa Research
```

### Comparing `f3dasm_optimize-0.0.1/README.md` & `f3dasm_optimize-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-0.0.1/setup.cfg` & `f3dasm_optimize-1.0.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = f3dasm_optimize
 version = file: VERSION
-author = Your Name
-author_email = youremailadress@email.com
+author = Martin van der Schelling
+author_email = M.P.vanderSchelling@tudelft.nl
 description = f3dasm_optimize: Your one line description of the package
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = keyword1, keyword2, keyword3
 url = https://github.com/bessagroup/f3dasm_optimize
 license = BSD-3-Clause License
 license_files = file: LICENSE
@@ -21,15 +21,15 @@
 	Programming Language :: Python :: 3
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = file: requirements.txt
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `f3dasm_optimize-0.0.1/src/f3dasm_optimize.egg-info/PKG-INFO` & `f3dasm_optimize-1.0.0/src/f3dasm_optimize.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: f3dasm-optimize
-Version: 0.0.1
+Version: 1.0.0
 Summary: f3dasm_optimize: Your one line description of the package
 Home-page: https://github.com/bessagroup/f3dasm_optimize
-Author: Your Name
-Author-email: youremailadress@email.com
+Author: Martin van der Schelling
+Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD-3-Clause License
 Keywords: keyword1,keyword2,keyword3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href=""><img alt="logo" src="https://user-images.githubusercontent.com/25851824/200928507-a65327f9-bc70-4c12-beaa-bc6ba74d968e.svg" width="60%"></a>
 </p>
 
 ## Bessa Group Python repository template
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: f3dasm-optimize Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: f3dasm-optimize Version: 1.0.0 Summary:
 f3dasm_optimize: Your one line description of the package Home-page: https://
-github.com/bessagroup/f3dasm_optimize Author: Your Name Author-email:
-youremailadress@email.com License: BSD-3-Clause License Keywords:
+github.com/bessagroup/f3dasm_optimize Author: Martin van der Schelling Author-
+email: M.P.vanderSchelling@tudelft.nl License: BSD-3-Clause License Keywords:
 keyword1,keyword2,keyword3 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Requires-Python:
->=3.7 Description-Content-Type: text/markdown
+>=3.8 Description-Content-Type: text/markdown
                                     [logo]
 ## Bessa Group Python repository template **Authors**: - Martin van der
 Schelling ([M.P.vanderSchelling@tudelft.nl](mailto:
 M.P.vanderSchelling@tudelft.nl)) **Authors afilliation:** - Bessa Research
 Group @ Delft University of Technology **Maintainer:** - Martin van der
 Schelling ([M.P.vanderSchelling@tudelft.nl](mailto:
 M.P.vanderSchelling@tudelft.nl)) **Maintainer afilliation:** - Bessa Research
```

