# Comparing `tmp/astro-tiptop-1.0.tar.gz` & `tmp/astro-tiptop-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-tiptop-1.0.tar", last modified: Tue May  9 09:41:13 2023, max compression
+gzip compressed data, was "astro-tiptop-1.1.tar", last modified: Fri Jul  7 09:12:17 2023, max compression
```

## Comparing `astro-tiptop-1.0.tar` & `astro-tiptop-1.1.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-09 09:41:13.338021 astro-tiptop-1.0/
--rw-r--r--   0 simon     (1000) simon     (1000)     1818 2023-05-04 08:35:07.000000 astro-tiptop-1.0/.gitignore
--rw-r--r--   0 simon     (1000) simon     (1000)      209 2023-05-02 09:52:09.000000 astro-tiptop-1.0/.readthedocs.yml
--rw-r--r--   0 simon     (1000) simon     (1000)     1074 2023-01-10 10:40:57.000000 astro-tiptop-1.0/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)       25 2023-04-06 16:06:53.000000 astro-tiptop-1.0/MANIFEST.in
--rw-r--r--   0 simon     (1000) simon     (1000)     1037 2023-05-09 09:41:13.338021 astro-tiptop-1.0/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      703 2023-05-02 09:52:52.000000 astro-tiptop-1.0/README.md
--rw-r--r--   0 simon     (1000) simon     (1000)     1345 2023-01-10 11:36:42.000000 astro-tiptop-1.0/TIPTOP-EXAMPLE.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)      481 2023-04-07 11:14:02.000000 astro-tiptop-1.0/TIPTOP-EXAMPLE.py
--rw-r--r--   0 simon     (1000) simon     (1000)    12147 2023-01-10 11:36:42.000000 astro-tiptop-1.0/TIPTOP-GUI.ipynb
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-09 09:41:13.338021 astro-tiptop-1.0/astro_tiptop.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     1037 2023-05-09 09:41:13.000000 astro-tiptop-1.0/astro_tiptop.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      885 2023-05-09 09:41:13.000000 astro-tiptop-1.0/astro_tiptop.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-05-09 09:41:13.000000 astro-tiptop-1.0/astro_tiptop.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       94 2023-05-09 09:41:13.000000 astro-tiptop-1.0/astro_tiptop.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        7 2023-05-09 09:41:13.000000 astro-tiptop-1.0/astro_tiptop.egg-info/top_level.txt
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-09 09:41:13.338021 astro-tiptop-1.0/docs/
--rw-r--r--   0 simon     (1000) simon     (1000)      638 2023-01-10 10:40:57.000000 astro-tiptop-1.0/docs/Makefile
--rw-r--r--   0 simon     (1000) simon     (1000)      769 2023-01-10 10:40:57.000000 astro-tiptop-1.0/docs/make.bat
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-09 09:41:13.338021 astro-tiptop-1.0/docs/source/
--rw-r--r--   0 simon     (1000) simon     (1000)       73 2023-05-04 08:35:07.000000 astro-tiptop-1.0/docs/source/api.rst
--rw-r--r--   0 simon     (1000) simon     (1000)     2099 2023-04-07 12:52:07.000000 astro-tiptop-1.0/docs/source/conf.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1314 2023-01-10 10:40:57.000000 astro-tiptop-1.0/docs/source/howto.rst
--rw-r--r--   0 simon     (1000) simon     (1000)     1689 2023-05-09 08:47:43.000000 astro-tiptop-1.0/docs/source/index.rst
--rw-r--r--   0 simon     (1000) simon     (1000)    20254 2023-05-04 08:35:07.000000 astro-tiptop-1.0/docs/source/parameterFile.rst
--rw-r--r--   0 simon     (1000) simon     (1000)     1546 2023-05-04 08:35:07.000000 astro-tiptop-1.0/docs/source/usage.rst
--rw-r--r--   0 simon     (1000) simon     (1000)     7841 2023-05-04 08:35:07.000000 astro-tiptop-1.0/docs/source/wishList.rst
--rw-r--r--   0 simon     (1000) simon     (1000)   165545 2023-04-07 15:03:15.000000 astro-tiptop-1.0/main_sphere_test.ipynb
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-09 09:41:13.338021 astro-tiptop-1.0/perfTest/
--rw-r--r--   0 simon     (1000) simon     (1000)     1212 2023-01-18 12:23:46.000000 astro-tiptop-1.0/perfTest/ERIS.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     1642 2023-01-18 12:23:46.000000 astro-tiptop-1.0/perfTest/ERIS_LGS.ini
--rwxr-xr-x   0 simon     (1000) simon     (1000)     7603 2023-01-10 10:40:57.000000 astro-tiptop-1.0/perfTest/HarmoniLTAO_1.ini
--rwxr-xr-x   0 simon     (1000) simon     (1000)     7490 2023-01-10 10:40:57.000000 astro-tiptop-1.0/perfTest/HarmoniLTAO_2.ini
--rwxr-xr-x   0 simon     (1000) simon     (1000)     7514 2023-01-10 10:40:57.000000 astro-tiptop-1.0/perfTest/HarmoniLTAO_3.ini
--rwxr-xr-x   0 simon     (1000) simon     (1000)     7448 2023-01-10 10:40:57.000000 astro-tiptop-1.0/perfTest/HarmoniSCAO_1.ini
--rwxr-xr-x   0 simon     (1000) simon     (1000)     7436 2023-01-10 10:40:57.000000 astro-tiptop-1.0/perfTest/HarmoniSCAO_2.ini
--rwxr-xr-x   0 simon     (1000) simon     (1000)     7436 2023-01-10 10:40:57.000000 astro-tiptop-1.0/perfTest/HarmoniSCAO_3.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     2466 2023-01-10 10:40:57.000000 astro-tiptop-1.0/perfTest/MAVIS.ini
--rw-r--r--   0 simon     (1000) simon     (1000)      960 2023-01-10 10:40:57.000000 astro-tiptop-1.0/perfTest/SOUL.ini
--rw-r--r--   0 simon     (1000) simon     (1000)     1032 2023-01-10 10:40:57.000000 astro-tiptop-1.0/perfTest/SPHERE.ini
--rw-r--r--   0 simon     (1000) simon     (1000)      184 2023-01-10 10:40:57.000000 astro-tiptop-1.0/perfTest.sh
--rw-r--r--   0 simon     (1000) simon     (1000)      712 2023-05-09 09:26:39.000000 astro-tiptop-1.0/pyproject.toml
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-05-09 09:41:13.338021 astro-tiptop-1.0/setup.cfg
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-09 09:41:13.338021 astro-tiptop-1.0/tiptop/
--rw-r--r--   0 simon     (1000) simon     (1000)       72 2023-04-07 12:52:07.000000 astro-tiptop-1.0/tiptop/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      155 2023-05-09 09:41:13.000000 astro-tiptop-1.0/tiptop/_version.py
--rw-r--r--   0 simon     (1000) simon     (1000)    14954 2023-04-07 12:52:07.000000 astro-tiptop-1.0/tiptop/tiptop.py
--rwxr-xr-x   0 simon     (1000) simon     (1000)     1419 2023-01-10 10:40:58.000000 astro-tiptop-1.0/tiptop/tiptopCLT.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6961 2023-04-07 15:08:36.000000 astro-tiptop-1.0/tiptop/tiptopGUI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.155058 astro-tiptop-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.147058 astro-tiptop-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.151058 astro-tiptop-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 09:11:59.000000 astro-tiptop-1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-07 09:11:59.000000 astro-tiptop-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-07 09:11:59.000000 astro-tiptop-1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 09:11:59.000000 astro-tiptop-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 09:11:59.000000 astro-tiptop-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-07 09:12:17.155058 astro-tiptop-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-07 09:11:59.000000 astro-tiptop-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-07 09:11:59.000000 astro-tiptop-1.1/TIPTOP-EXAMPLE.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-07 09:11:59.000000 astro-tiptop-1.1/TIPTOP-EXAMPLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-07-07 09:11:59.000000 astro-tiptop-1.1/TIPTOP-GUI.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.151058 astro-tiptop-1.1/astro_tiptop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-07 09:12:17.000000 astro-tiptop-1.1/astro_tiptop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-07 09:12:17.000000 astro-tiptop-1.1/astro_tiptop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:12:17.000000 astro-tiptop-1.1/astro_tiptop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-07 09:12:17.000000 astro-tiptop-1.1/astro_tiptop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 09:12:17.000000 astro-tiptop-1.1/astro_tiptop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.151058 astro-tiptop-1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.151058 astro-tiptop-1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/parameterFile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/wishList.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   165545 2023-07-07 09:11:59.000000 astro-tiptop-1.1/main_sphere_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.155058 astro-tiptop-1.1/perfTest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/ERIS.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/ERIS_LGS.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7610 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniLTAO_1.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7496 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniLTAO_2.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7520 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniLTAO_3.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5789 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniSCAO_1.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5777 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniSCAO_2.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5777 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniSCAO_3.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/MAVIS.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/SOUL.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/SPHERE.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-07 09:11:59.000000 astro-tiptop-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:12:17.155058 astro-tiptop-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.155058 astro-tiptop-1.1/tiptop/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 09:11:59.000000 astro-tiptop-1.1/tiptop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 09:12:16.000000 astro-tiptop-1.1/tiptop/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-07-07 09:11:59.000000 astro-tiptop-1.1/tiptop/tiptop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-07-07 09:11:59.000000 astro-tiptop-1.1/tiptop/tiptopCLT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-07 09:11:59.000000 astro-tiptop-1.1/tiptop/tiptopGUI.py
```

### Comparing `astro-tiptop-1.0/.gitignore` & `astro-tiptop-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/LICENSE` & `astro-tiptop-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/PKG-INFO` & `astro-tiptop-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-tiptop
-Version: 1.0
+Version: 1.1
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/TIPTOP
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: gpu
```

### Comparing `astro-tiptop-1.0/README.md` & `astro-tiptop-1.1/README.md`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/TIPTOP-EXAMPLE.ipynb` & `astro-tiptop-1.1/TIPTOP-EXAMPLE.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/TIPTOP-GUI.ipynb` & `astro-tiptop-1.1/TIPTOP-GUI.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/astro_tiptop.egg-info/PKG-INFO` & `astro-tiptop-1.1/astro_tiptop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-tiptop
-Version: 1.0
+Version: 1.1
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/TIPTOP
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: gpu
```

### Comparing `astro-tiptop-1.0/astro_tiptop.egg-info/SOURCES.txt` & `astro-tiptop-1.1/astro_tiptop.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.md
 TIPTOP-EXAMPLE.ipynb
 TIPTOP-EXAMPLE.py
 TIPTOP-GUI.ipynb
 main_sphere_test.ipynb
 perfTest.sh
 pyproject.toml
+.github/workflows/publish.yml
 astro_tiptop.egg-info/PKG-INFO
 astro_tiptop.egg-info/SOURCES.txt
 astro_tiptop.egg-info/dependency_links.txt
 astro_tiptop.egg-info/requires.txt
 astro_tiptop.egg-info/top_level.txt
 docs/Makefile
 docs/make.bat
```

### Comparing `astro-tiptop-1.0/docs/Makefile` & `astro-tiptop-1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/docs/make.bat` & `astro-tiptop-1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/docs/source/conf.py` & `astro-tiptop-1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/docs/source/howto.rst` & `astro-tiptop-1.1/docs/source/howto.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/docs/source/index.rst` & `astro-tiptop-1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/docs/source/parameterFile.rst` & `astro-tiptop-1.1/docs/source/parameterFile.rst`

 * *Files 2% similar despite different names*

```diff
@@ -255,22 +255,22 @@
    Even if ``Zenith`` is defined, this is optionnal.
 
 .. option:: Height
    
    **Optional**, 
    *Type : float*, 
    *Default : 0.0*, 
-   altitude of the guide stars (0 if infinite). Consider that all guide star are at the same heigh.
+   altitude of the guide stars (0 if infinite). Consider that all guide star are at the same height.
 
 
 [sources_LO]
 ^^^^^^^^^^^^
 .. note::
 
-   This section is completely optional
+   This section is completely optional (``[sensor_LO]`` section is required to have the LO part simulated)
 
 
 .. option:: Wavelength
 
    **Required**, 
    *type : float*, 
    Sensing wavelength for Low Order modes in meters
@@ -519,15 +519,15 @@
 
 
 [sensor_LO]
 ^^^^^^^^^^^
 
 .. note::
 
-   This section is optional
+   This section is optional, if this section is not present only the HO part will be used (for ex. to simulate a SCAO NGS).
 
 
 .. option:: PixelScale
 
    **Required**, 
    *type: float*, 
    LO WFS pixel scale in [mas]
@@ -735,15 +735,16 @@
 ^^^^^
 
 .. option:: LoopGain_HO
 
    **Optional**, 
    *Type : float*, 
    *Default : 0.5*, 
-   High Order Loop gain
+   High Order Loop gain.
+   If system to be simulated is a multi-conjugate system this parameter is not used.
 
 .. option:: SensorFrameRate_HO
 
    **Optional**, 
    *type: float*, 
    *Default : 500.0*,
    High Order loop frequency in [Hz]
@@ -754,33 +755,34 @@
    *type: int*, 
    *Default : 2*, 
    High Order loop delay in [frame]
 
 .. option:: LoopGain_LO
 
    **Optional**, 
-   *type: float*?, 
+   *type: float or string*, 
    *default: None*,
-   not used, auto matically optimized by tiptop.
+   if set to 'optimize', gain is auto matically optimized by tiptop, otherwise the float value set is used.
    Low Order loop gain
 
 .. option:: SensorFrameRate_LO
 
    **Required**, 
    *type: float*, 
    *default: None*,
    Loop frequency in [Hz]
-   This is confusing : this is not optional if the ``[sensor_LO]`` is set.  
+   If ``[sensor_LO]`` section is present it must be set.  
 
 .. option:: LoopDelaySteps_LO
 
    **Optional**, 
    *type: int*, 
    *default: None*,
    Low Order loop delays in [frames]
+   If ``[sensor_LO]`` section is present it must be set.
 
 .. option:: ResidualError
 
    **Optional**
    *Type : ?*
    *Default: None*
    ?
```

### Comparing `astro-tiptop-1.0/docs/source/usage.rst` & `astro-tiptop-1.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/docs/source/wishList.rst` & `astro-tiptop-1.1/docs/source/wishList.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/main_sphere_test.ipynb` & `astro-tiptop-1.1/main_sphere_test.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/perfTest/ERIS.ini` & `astro-tiptop-1.1/perfTest/ERIS.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/perfTest/ERIS_LGS.ini` & `astro-tiptop-1.1/perfTest/ERIS_LGS.ini`

 * *Files 8% similar despite different names*

```diff
@@ -69,12 +69,13 @@
 NumberActuators = [40]
 DmPitchs = [0.2]
 DmHeights = [0.0]
 AoArea = 'circle'
 
 [RTC]
 LoopGain_HO = 0.3
+LoopGain_LO = 'optimize'
 SensorFrameRate_HO = 1000.0
 LoopDelaySteps_HO = 3
 SensorFrameRate_LO = 1000.0
 LoopDelaySteps_LO = 3
```

### Comparing `astro-tiptop-1.0/perfTest/HarmoniLTAO_1.ini` & `astro-tiptop-1.1/perfTest/HarmoniLTAO_1.ini`

 * *Files 2% similar despite different names*

```diff
@@ -171,12 +171,12 @@
 ;HO Loop gain - required
 LoopGain_HO = 0.5
 ;HO loop frequency in [Hz] - required
 SensorFrameRate_HO = 500.0
 ;HO loop frame delay - required
 LoopDelaySteps_HO = 1
 ; LO loop gain - optional - default: Nome
-LoopGain_LO = 0.5
+LoopGain_LO = 'optimize'
 ;Loop frequency in Hz  - optional - default: None
 SensorFrameRate_LO = 500.0
 ;Corresponding delays (in frames)  - optional - default: None
 LoopDelaySteps_LO = 3
```

### Comparing `astro-tiptop-1.0/perfTest/HarmoniLTAO_2.ini` & `astro-tiptop-1.1/perfTest/HarmoniLTAO_2.ini`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ;altitude of the guide stars (0 if infinite) - optional - default: 0.0
 Height = 90e3
 
 [sources_LO]
 ;Sensing wavelength for LO modes in meters - required
 Wavelength = 850e-9
 ;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
-Zenith = [60.]
+Zenith = [10.]
 Azimuth = [0.0]
 
 [sensor_science]
 ;pixel/spaxel scale in mas - required
 PixelScale = 4.0
 ;Field of view in pixel - optional - default: 150
 FieldOfView = 640
@@ -169,12 +169,12 @@
 ;HO Loop gain - required
 LoopGain_HO = 0.5                                   
 ;HO loop frequency in [Hz] - required
 SensorFrameRate_HO = 500.0
 ;HO loop frame delay - required
 LoopDelaySteps_HO = 1   
 ; LO loop gain - optional - default: Nome
-LoopGain_LO = 0.5
+LoopGain_LO = 'optimize'
 ;Loop frequency in Hz  - optional - default: None
 SensorFrameRate_LO = 500.0
 ;Corresponding delays (in frames)  - optional - default: None
-LoopDelaySteps_LO = 3
+LoopDelaySteps_LO = 3
```

### Comparing `astro-tiptop-1.0/perfTest/HarmoniLTAO_3.ini` & `astro-tiptop-1.1/perfTest/HarmoniLTAO_3.ini`

 * *Files 1% similar despite different names*

```diff
@@ -169,12 +169,12 @@
 ;HO Loop gain - required
 LoopGain_HO = 0.5                                   
 ;HO loop frequency in [Hz] - required
 SensorFrameRate_HO = 500.0
 ;HO loop frame delay - required
 LoopDelaySteps_HO = 1   
 ; LO loop gain - optional - default: Nome
-LoopGain_LO = 0.5
+LoopGain_LO = 'optimize'
 ;Loop frequency in Hz  - optional - default: None
 SensorFrameRate_LO = 500.0
 ;Corresponding delays (in frames)  - optional - default: None
-LoopDelaySteps_LO = 3
+LoopDelaySteps_LO = 3
```

### Comparing `astro-tiptop-1.0/perfTest/HarmoniSCAO_1.ini` & `astro-tiptop-1.1/perfTest/HarmoniSCAO_1.ini`

 * *Files 13% similar despite different names*

```diff
@@ -46,21 +46,14 @@
 Wavelength = 950e-9
 ;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
 Zenith = [0.0]
 Azimuth = [0.0]
 ;altitude of the guide stars (0 if infinite) - optional - default: 0.0
 Height = 0.0
 
-[sources_LO]
-;Sensing wavelength for HO modes in meters - required
-Wavelength = 1650e-9
-;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
-Zenith = [0.0]
-Azimuth = [0.0]
-
 [sensor_science]
 ;pixel/spaxel scale in mas - required
 PixelScale = 4.0
 ;Field of view in pixel - optional - default: 150
 FieldOfView = 640
 
 [sensor_HO]
@@ -104,46 +97,14 @@
 Algorithm = 'wcog' 
 ;Number of pixels for windiwing the low order WFS pixels - optional - default: 2      
 WindowRadiusWCoG = 6
 ;Threshold Number of pixels for windowing the low order WFS pixels - optional - default: 0.0        
 ThresholdWCoG = 0.0
 ;New value for pixels lower than threshold - optional - default: 0.0        
 NewValueThrPix = 0.0
- 
-[sensor_LO]
-;LO WFS pixel scale in [mas] - required
-PixelScale = 5.0
-;Number of pixels per subaperture - required 
-FieldOfView = 200 
-;binning factor - optional - default: 1
-Binning = 1   
-;detected flux in [nph/frame/subaperture] - required           
-NumberPhotons = [200] 
-;HO spot scale in [mas] - optional - defaut: [[0.0, 0.0, 0.0]]
-SpotFWHM = [[0.0,0.0,0.0]]   
-;ron in [e-] - optional - default: 0.0        
-SigmaRON = 0.0   
-;dark current[e-/s/pix] - optional - default: 0.0        
-Dark = 30.0
-;sky background [e-/s/pix] - optional - default: 0.0          
-SkyBackground = 35.0
-;Pixel gain - optional - default:1.0
-Gain = 1.0  
-;excess noise factor - optional - default: 2.0                     
-ExcessNoiseFactor = 2.0 
-;number of WFS lenslets - required
-NumberLenslets = [4]
-;CoG computation algorithm - optional  - default:'wcog'
-Algorithm = 'wcog' 
-;Number of pixels for windiwing the low order WFS pixels - optional - default: 2      
-WindowRadiusWCoG = 2
-;Threshold Number of pixels for windowing the low order WFS pixels - optional - default: 0.0        
-ThresholdWCoG = 0.0
-;New value for pixels lower than threshold - optional - default: 0.0        
-NewValueThrPix = 0.0
 
 [DM]
 ;DM actuators pitch in meters - required
 NumberActuators = [80]
 ;DM actuators pitch in meters - required
 DmPitchs = [0.38]
 ;DM influence function model - optional - default: 'gaussian'
@@ -167,14 +128,8 @@
 
 [RTC]
 ;HO Loop gain - required
 LoopGain_HO = 0.8                                
 ;HO loop frequency in [Hz] - required
 SensorFrameRate_HO = 500.0
 ;HO loop frame delay - required
-LoopDelaySteps_HO = 1   
-; LO loop gain - optional - default: Nome
-LoopGain_LO = 0.5
-;Loop frequency in Hz  - optional - default: None
-SensorFrameRate_LO = 500.0
-;Corresponding delays (in frames)  - optional - default: None
-LoopDelaySteps_LO = 1
+LoopDelaySteps_HO = 1
```

### Comparing `astro-tiptop-1.0/perfTest/HarmoniSCAO_2.ini` & `astro-tiptop-1.1/perfTest/HarmoniSCAO_2.ini`

 * *Files 14% similar despite different names*

```diff
@@ -45,21 +45,14 @@
 Wavelength = 950e-9
 ;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
 Zenith = [15.]
 Azimuth = [0.0]
 ;altitude of the guide stars (0 if infinite) - optional - default: 0.0
 Height = 0.0
 
-[sources_LO]
-;Sensing wavelength for HO modes in meters - required
-Wavelength = 1650e-9
-;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
-Zenith = [0.0]
-Azimuth = [0.0]
-
 [sensor_science]
 ;pixel/spaxel scale in mas - required
 PixelScale = 4.0
 ;Field of view in pixel - optional - default: 150
 FieldOfView = 640
 
 [sensor_HO]
@@ -103,46 +96,14 @@
 Algorithm = 'wcog' 
 ;Number of pixels for windiwing the low order WFS pixels - optional - default: 2      
 WindowRadiusWCoG = 6
 ;Threshold Number of pixels for windowing the low order WFS pixels - optional - default: 0.0        
 ThresholdWCoG = 0.0
 ;New value for pixels lower than threshold - optional - default: 0.0        
 NewValueThrPix = 0.0
- 
-[sensor_LO]
-;LO WFS pixel scale in [mas] - required
-PixelScale = 5.0
-;Number of pixels per subaperture - required 
-FieldOfView = 200 
-;binning factor - optional - default: 1
-Binning = 1   
-;detected flux in [nph/frame/subaperture] - required           
-NumberPhotons = [200] 
-;HO spot scale in [mas] - optional - defaut: [[0.0, 0.0, 0.0]]
-SpotFWHM = [[0.0,0.0,0.0]]   
-;ron in [e-] - optional - default: 0.0        
-SigmaRON = 30.0   
-;dark current[e-/s/pix] - optional - default: 0.0        
-Dark = 0.0
-;sky background [e-/s/pix] - optional - default: 0.0          
-SkyBackground = 35.0
-;Pixel gain - optional - default:1.0
-Gain = 1.0  
-;excess noise factor - optional - default: 2.0                     
-ExcessNoiseFactor = 2.0 
-;number of WFS lenslets - required
-NumberLenslets = [4]
-;CoG computation algorithm - optional  - default:'wcog'
-Algorithm = 'wcog' 
-;Number of pixels for windiwing the low order WFS pixels - optional - default: 2      
-WindowRadiusWCoG = 2
-;Threshold Number of pixels for windowing the low order WFS pixels - optional - default: 0.0        
-ThresholdWCoG = 0.0
-;New value for pixels lower than threshold - optional - default: 0.0        
-NewValueThrPix = 0.0
 
 [DM]
 ;DM actuators pitch in meters - required
 NumberActuators = [80]
 ;DM actuators pitch in meters - required
 DmPitchs = [0.38]
 ;DM influence function model - optional - default: 'gaussian'
@@ -166,14 +127,8 @@
 
 [RTC]
 ;HO Loop gain - required
 LoopGain_HO = 0.8                                
 ;HO loop frequency in [Hz] - required
 SensorFrameRate_HO = 500.0
 ;HO loop frame delay - required
-LoopDelaySteps_HO = 1   
-; LO loop gain - optional - default: Nome
-LoopGain_LO = 0.5
-;Loop frequency in Hz  - optional - default: None
-SensorFrameRate_LO = 500.0
-;Corresponding delays (in frames)  - optional - default: None
-LoopDelaySteps_LO = 1
+LoopDelaySteps_HO = 1
```

### Comparing `astro-tiptop-1.0/perfTest/HarmoniSCAO_3.ini` & `astro-tiptop-1.1/perfTest/HarmoniSCAO_3.ini`

 * *Files 20% similar despite different names*

```diff
@@ -45,21 +45,14 @@
 Wavelength = 950e-9
 ;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
 Zenith = [0.0]
 Azimuth = [0.0]
 ;altitude of the guide stars (0 if infinite) - optional - default: 0.0
 Height = 0.0
 
-[sources_LO]
-;Sensing wavelength for HO modes in meters - required
-Wavelength = 1650e-9
-;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
-Zenith = [0.0]
-Azimuth = [0.0]
-
 [sensor_science]
 ;pixel/spaxel scale in mas - required
 PixelScale = 4.0
 ;Field of view in pixel - optional - default: 150
 FieldOfView = 640
 
 [sensor_HO]
@@ -103,46 +96,14 @@
 Algorithm = 'wcog' 
 ;Number of pixels for windiwing the low order WFS pixels - optional - default: 2      
 WindowRadiusWCoG = 6
 ;Threshold Number of pixels for windowing the low order WFS pixels - optional - default: 0.0        
 ThresholdWCoG = 0.0
 ;New value for pixels lower than threshold - optional - default: 0.0        
 NewValueThrPix = 0.0
- 
-[sensor_LO]
-;LO WFS pixel scale in [mas] - required
-PixelScale = 5.0
-;Number of pixels per subaperture - required 
-FieldOfView = 200 
-;binning factor - optional - default: 1
-Binning = 1   
-;detected flux in [nph/frame/subaperture] - required           
-NumberPhotons = [200] 
-;HO spot scale in [mas] - optional - defaut: [[0.0, 0.0, 0.0]]
-SpotFWHM = [[0.0,0.0,0.0]]   
-;ron in [e-] - optional - default: 0.0        
-SigmaRON = 30.0   
-;dark current[e-/s/pix] - optional - default: 0.0        
-Dark = 0.0
-;sky background [e-/s/pix] - optional - default: 0.0          
-SkyBackground = 35.0
-;Pixel gain - optional - default:1.0
-Gain = 1.0  
-;excess noise factor - optional - default: 2.0                     
-ExcessNoiseFactor = 2.0 
-;number of WFS lenslets - required
-NumberLenslets = [4]
-;CoG computation algorithm - optional  - default:'wcog'
-Algorithm = 'wcog' 
-;Number of pixels for windiwing the low order WFS pixels - optional - default: 2      
-WindowRadiusWCoG = 2
-;Threshold Number of pixels for windowing the low order WFS pixels - optional - default: 0.0        
-ThresholdWCoG = 0.0
-;New value for pixels lower than threshold - optional - default: 0.0        
-NewValueThrPix = 0.0
 
 [DM]
 ;DM actuators pitch in meters - required
 NumberActuators = [80]
 ;DM actuators pitch in meters - required
 DmPitchs = [0.38]
 ;DM influence function model - optional - default: 'gaussian'
@@ -166,14 +127,8 @@
 
 [RTC]
 ;HO Loop gain - required
 LoopGain_HO = 0.8                                
 ;HO loop frequency in [Hz] - required
 SensorFrameRate_HO = 500.0
 ;HO loop frame delay - required
-LoopDelaySteps_HO = 1   
-; LO loop gain - optional - default: Nome
-LoopGain_LO = 0.5
-;Loop frequency in Hz  - optional - default: None
-SensorFrameRate_LO = 500.0
-;Corresponding delays (in frames)  - optional - default: None
-LoopDelaySteps_LO = 1
+LoopDelaySteps_HO = 1
```

### Comparing `astro-tiptop-1.0/perfTest/MAVIS.ini` & `astro-tiptop-1.1/perfTest/MAVIS.ini`

 * *Files 3% similar despite different names*

```diff
@@ -73,11 +73,11 @@
 NumberReconstructedLayers = 10
 AoArea = 'circle'
 
 [RTC]
 LoopGain_HO = 0.3
 SensorFrameRate_HO = 1000.0
 LoopDelaySteps_HO = 2
-LoopGain_LO = 0.3
+LoopGain_LO = 'optimize'
 SensorFrameRate_LO = 1000.0
 LoopDelaySteps_LO = 2
```

### Comparing `astro-tiptop-1.0/perfTest/SOUL.ini` & `astro-tiptop-1.1/perfTest/SOUL.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/perfTest/SPHERE.ini` & `astro-tiptop-1.1/perfTest/SPHERE.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/tiptop/tiptop.py` & `astro-tiptop-1.1/tiptop/tiptop.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,37 @@
 from mastsel import *
 
 from datetime import datetime
 
 rc("text", usetex=False)
 
 def overallSimulation(path, parametersFile, outputDir, outputFile, doConvolve=False,
-                      doPlot=False, verbose=False, returnRes=False, addSrAndFwhm=False):
+                      doPlot=False, returnRes=False, addSrAndFwhm=False,
+                      verbose=False, getHoErrorBreakDown=False):
     """
     function to run the entire tiptop simulation based on the imput file
 
     :param path2param: required, path to the parameter file
     :type path2param: str
     :param paramFileName: required, name of the parameter file to be used without the extention
     :type paramFileName: str
     :param outpuDir: required, path to the folder in which to write the output
     :type outputDir: str
     :param doConvolve: optional default: False, if you want to use the natural convolution operation  set to True
     :type doConvolve: bool
     :param doPlot: optional default: False, if you want to see the result in python set this to True
     :type doPlot: bool
-    :param verbose: optional default: False, If you want all messages set this to True
-    :type verbose: bool
-    :param returnRes: optionnal default: False, The function will return the result in the environment if set to True, else it saves the result only in a .fits file.
+    :param returnRes: optional default: False, The function will return the result in the environment if set to True, else it saves the result only in a .fits file.
     :type returnRes: bool
-    :param addSrAndFwhm: optionnal default: False, The function will add in the header of the fits file SR anf FWHM for each PSF.
+    :param addSrAndFwhm: optional default: False, The function will add in the header of the fits file SR anf FWHM for each PSF.
     :type addSrAndFwhm: bool
+    :param verbose: optional default: False, If you want all messages set this to True
+    :type verbose: bool
+    :param getHoErrorBreakDown: optional default: False, If you want HO error breakdosn set this to True
+    :type getHoErrorBreakDown: bool
 
     :return: TBD
     :rtype: TBD
 
     """
 
     # initiate the parser
@@ -78,16 +81,18 @@
             LO_az      = my_yaml_dict['sources_LO']['Azimuth']
             LO_fluxes  = my_yaml_dict['sensor_LO']['NumberPhotons']
             fr         = my_yaml_dict['RTC']['SensorFrameRate_LO']
 
         if 'jitter_FWHM' in my_yaml_dict['telescope'].keys():
             jitter_FWHM = my_yaml_dict['telescope']['jitter_FWHM']
 
-        fao = fourierModel( fullPathFilename_yml, calcPSF=False, verbose=False
-                           , display=False, getPSDatNGSpositions=True)
+        fao = fourierModel( fullPathFilename_yml, calcPSF=False, verbose=verbose
+                           , display=False, getPSDatNGSpositions=True
+                           , computeFocalAnisoCov=False, TiltFilter=LOisOn
+                           , getErrorBreakDown=getHoErrorBreakDown)
 
     elif os.path.exists(fullPathFilename_ini):
         parser           = ConfigParser()
         parser.read(fullPathFilename_ini);
         # read main parameters
         tel_radius = eval(parser.get('telescope', 'TelescopeDiameter'))/2  # mas
         wvl_temp = eval(parser.get('sources_science', 'Wavelength'))
@@ -115,16 +120,19 @@
             LO_zen     = eval(parser.get('sources_LO', 'Zenith'))
             LO_az      = eval(parser.get('sources_LO', 'Azimuth'))
             LO_fluxes  = eval(parser.get('sensor_LO', 'NumberPhotons'))
             fr         = eval(parser.get('RTC', 'SensorFrameRate_LO'))
         if parser.has_option('telescope', 'jitter_FWHM'):
             jitter_FWHM = eval(parser.get('telescope', 'jitter_FWHM'))
 
-        fao = fourierModel( fullPathFilename_ini, calcPSF=False, verbose=False
-                           , display=False, getPSDatNGSpositions=True, computeFocalAnisoCov=False)
+        fao = fourierModel( fullPathFilename_ini, calcPSF=False, verbose=verbose
+                           , display=False, getPSDatNGSpositions=True
+                           , computeFocalAnisoCov=False, TiltFilter=LOisOn
+                           , getErrorBreakDown=getHoErrorBreakDown)
+        
     else:
         raise FileNotFoundError('No .yml or .ini can be found in '+ path)
 
     if LOisOn:
         # NGSs positions
         NGS_flux = []
         polarNGSCoordsList = []
@@ -174,15 +182,15 @@
             # Get the PSF
             psfLE          = longExposurePsf(mask, psd )
             psfLongExpArr.append(psfLE)
             # Get SR and FWHM in mas at the NGSs positions at the sensing wavelength
             SR             = np.exp(-computedPSD.sum()* scaleFactor) # Strehl-ratio at the sensing wavelength
             NGS_SR.append(SR)
             FWHMx,FWHMy    = getFWHM( psfLE.sampling, pixelscale, method='contour', nargout=2)
-            FWHM           = max(FWHMx, FWHMy) #0.5*(FWHMx+FWHMy) #average over major and minor axes
+            FWHM           = np.sqrt(FWHMx*FWHMy) #max(FWHMx, FWHMy) #0.5*(FWHMx+FWHMy) #average over major and minor axes
             # note : the uncertainities on the FWHM seems to create a bug in mavisLO
             NGS_FWHM_mas.append(FWHM)
             if verbose:
                 print('SR(@',int(wavelength*1e9),'nm)  :', SR)
                 print('FWHM(@',int(wavelength*1e9),'nm):', FWHM)
 
         return NGS_SR, psdArray, psfLongExpArr, NGS_FWHM_mas
@@ -232,15 +240,15 @@
         if returnRes == False:
             cov_ellipses       = mLO.ellipsesFromCovMats(Ctot)
             if verbose:
                 for n in range(cov_ellipses.shape[0]):
                     print('cov_ellipses #',n,': ',cov_ellipses[n,:], ' (unit: rad, mas, mas)')
             # FINAl CONVOLUTION
             if verbose:
-                print('******** FINAl CONVOLUTION')
+                print('******** FINAL CONVOLUTION')
             results = []
             for ellp, psfLongExp in zip(cov_ellipses, psfLongExpPointingsArr):
                 results.append(convolve(psfLongExp, residualToSpectrum(ellp, wvl
                                                                        , N, 1/(fao.ao.cam.fovInPix
                                                                                * fao.freq.psInMas[0]))))
 
     if doPlot:
@@ -274,25 +282,34 @@
         psdOL.sampling = cp.asarray(fao.ao.atm.spectrum(k) * pf * (fao.freq.wvlRef/np.pi)**2) # the PSD must be provided in m^2.m^2
         # Get the OPEN-LOOP PSF
         psfOL = longExposurePsf(mask, psdOL)
         if doPlot:
             fig, ax1 = plt.subplots(1,1)
             im = ax1.imshow(np.log(np.abs(psfOL.sampling) + 1e-20), cmap='hot')
             ax1.set_title('open loop PSF', color='black')
+            
+        # DIFFRACTION LIMITED PSD
+        psdDL = Field(wvl, N, freq_range, 'rad')
+        psfDL = longExposurePsf(mask, psdDL)
+        if doPlot:
+            fig, ax2 = plt.subplots(1,1)
+            im = ax2.imshow(np.log(np.abs(psfDL.sampling) + 1e-20), cmap='hot')
+            ax2.set_title('diffraction limited PSF', color='black')
 
         # save PSF cube in fits
         hdul1 = fits.HDUList()
         cube =[]
         hdul1.append(fits.PrimaryHDU())
         for img in results:
             cube.append(img.sampling)
 
         cube = np.array(cube)
         hdul1.append(fits.ImageHDU(data=cube))
         hdul1.append(fits.ImageHDU(data=psfOL.sampling)) # append open-loop PSF
+        hdul1.append(fits.ImageHDU(data=psfDL.sampling)) # append diffraction limited PSF
 
         #############################
         # header
         hdr0 = hdul1[0].header
         now = datetime.now()
         hdr0['TIME'] = now.strftime("%Y%m%d_%H%M%S")
         # parameters in the header
@@ -320,17 +337,23 @@
             hdr1['CCY'+str(i).zfill(4)] = pp[1,i]
         if addSrAndFwhm:
             for i in range(cube.shape[0]):
                 hdr1['SR'+str(i).zfill(4)]   = getStrehl(cube[i,:,:], fao.ao.tel.pupil, fao.freq.sampRef)
             for i in range(cube.shape[0]):
                 hdr1['FWHM'+str(i).zfill(4)] = getFWHM(cube[i,:,:], fao.freq.psInMas[0], method='contour', nargout=1)
 
-        # header of the coordinates
+        # header of the OPEN-LOOP PSF
         hdr2 = hdul1[2].header
         hdr2['TIME'] = now.strftime("%Y%m%d_%H%M%S")
         hdr2['CONTENT'] = "OPEN-LOOP PSF"
         hdr2['SIZE'] = str(psfOL.sampling.shape)
+        
+        # header of the DIFFRACTION LIMITED PSF
+        hdr3 = hdul1[3].header
+        hdr3['TIME'] = now.strftime("%Y%m%d_%H%M%S")
+        hdr3['CONTENT'] = "DIFFRACTION LIMITED PSF"
+        hdr3['SIZE'] = str(psfDL.sampling.shape)
         #############################
 
         hdul1.writeto( os.path.join(outputDir, outputFile + '.fits'), overwrite=True)
         if verbose:
             print("Output cube shape:", cube.shape)
```

### Comparing `astro-tiptop-1.0/tiptop/tiptopCLT.py` & `astro-tiptop-1.1/tiptop/tiptopCLT.py`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.0/tiptop/tiptopGUI.py` & `astro-tiptop-1.1/tiptop/tiptopGUI.py`

 * *Files identical despite different names*

