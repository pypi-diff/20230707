# Comparing `tmp/BCemu-1.1.tar.gz` & `tmp/BCemu-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BCemu-1.1.tar", last modified: Tue Apr  4 13:53:20 2023, max compression
+gzip compressed data, was "BCemu-1.1.1.tar", last modified: Fri Jul  7 17:04:24 2023, max compression
```

## Comparing `BCemu-1.1.tar` & `BCemu-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 sambit     (504) staff       (20)        0 2023-04-04 13:53:20.029782 BCemu-1.1/
-drwxr-xr-x   0 sambit     (504) staff       (20)        0 2023-04-04 13:53:20.028155 BCemu-1.1/BCemu.egg-info/
--rw-r--r--   0 sambit     (504) staff       (20)     5805 2023-04-04 13:53:19.000000 BCemu-1.1/BCemu.egg-info/PKG-INFO
--rw-r--r--   0 sambit     (504) staff       (20)      314 2023-04-04 13:53:20.000000 BCemu-1.1/BCemu.egg-info/SOURCES.txt
--rw-r--r--   0 sambit     (504) staff       (20)        1 2023-04-04 13:53:19.000000 BCemu-1.1/BCemu.egg-info/dependency_links.txt
--rw-r--r--   0 sambit     (504) staff       (20)        1 2023-04-04 09:23:47.000000 BCemu-1.1/BCemu.egg-info/not-zip-safe
--rw-r--r--   0 sambit     (504) staff       (20)       67 2023-04-04 13:53:19.000000 BCemu-1.1/BCemu.egg-info/requires.txt
--rw-r--r--   0 sambit     (504) staff       (20)        6 2023-04-04 13:53:19.000000 BCemu-1.1/BCemu.egg-info/top_level.txt
--rw-r--r--   0 sambit     (504) staff       (20)     1074 2022-04-01 07:23:56.000000 BCemu-1.1/LICENSE
--rw-r--r--   0 sambit     (504) staff       (20)     5805 2023-04-04 13:53:20.029672 BCemu-1.1/PKG-INFO
--rw-r--r--   0 sambit     (504) staff       (20)     5531 2022-04-01 07:23:56.000000 BCemu-1.1/README.md
--rw-r--r--   0 sambit     (504) staff       (20)       38 2023-04-04 13:53:20.029820 BCemu-1.1/setup.cfg
--rwxr-xr-x   0 sambit     (504) staff       (20)      901 2023-04-04 13:50:44.000000 BCemu-1.1/setup.py
-drwxr-xr-x   0 sambit     (504) staff       (20)        0 2023-04-04 13:53:20.029301 BCemu-1.1/src/
--rw-r--r--   0 sambit     (504) staff       (20)    13885 2023-04-04 13:27:44.000000 BCemu-1.1/src/BaryonEffectsEmulator.py
--rwxr-xr-x   0 sambit     (504) staff       (20)      433 2022-04-01 07:23:56.000000 BCemu-1.1/src/__init__.py
--rw-r--r--   0 sambit     (504) staff       (20)     1722 2022-04-01 07:23:56.000000 BCemu-1.1/src/download.py
--rw-r--r--   0 sambit     (504) staff       (20)     6157 2022-04-01 07:23:56.000000 BCemu-1.1/src/functions.py
-drwxr-xr-x   0 sambit     (504) staff       (20)        0 2023-04-04 13:53:20.029472 BCemu-1.1/src/input_data/
--rw-r--r--   0 sambit     (504) staff       (20)       92 2022-04-01 07:23:56.000000 BCemu-1.1/src/input_data/README.rst
--rw-r--r--   0 sambit     (504) staff       (20)     1606 2022-04-01 07:23:56.000000 BCemu-1.1/src/kpls.py
+drwxr-xr-x   0 sambit     (504) staff       (20)        0 2023-07-07 17:04:24.413969 BCemu-1.1.1/
+drwxr-xr-x   0 sambit     (504) staff       (20)        0 2023-07-07 17:04:24.412139 BCemu-1.1.1/BCemu.egg-info/
+-rw-r--r--   0 sambit     (504) staff       (20)     5810 2023-07-07 17:04:24.000000 BCemu-1.1.1/BCemu.egg-info/PKG-INFO
+-rw-r--r--   0 sambit     (504) staff       (20)      331 2023-07-07 17:04:24.000000 BCemu-1.1.1/BCemu.egg-info/SOURCES.txt
+-rw-r--r--   0 sambit     (504) staff       (20)        1 2023-07-07 17:04:24.000000 BCemu-1.1.1/BCemu.egg-info/dependency_links.txt
+-rw-r--r--   0 sambit     (504) staff       (20)        1 2023-07-07 17:04:24.000000 BCemu-1.1.1/BCemu.egg-info/not-zip-safe
+-rw-r--r--   0 sambit     (504) staff       (20)       67 2023-07-07 17:04:24.000000 BCemu-1.1.1/BCemu.egg-info/requires.txt
+-rw-r--r--   0 sambit     (504) staff       (20)        6 2023-07-07 17:04:24.000000 BCemu-1.1.1/BCemu.egg-info/top_level.txt
+-rw-r--r--   0 sambit     (504) staff       (20)     1074 2022-04-01 07:23:56.000000 BCemu-1.1.1/LICENSE
+-rw-r--r--   0 sambit     (504) staff       (20)     5810 2023-07-07 17:04:24.413836 BCemu-1.1.1/PKG-INFO
+-rw-r--r--   0 sambit     (504) staff       (20)     5534 2023-07-07 16:57:27.000000 BCemu-1.1.1/README.md
+-rw-r--r--   0 sambit     (504) staff       (20)       38 2023-07-07 17:04:24.414044 BCemu-1.1.1/setup.cfg
+-rwxr-xr-x   0 sambit     (504) staff       (20)      903 2023-07-07 17:01:50.000000 BCemu-1.1.1/setup.py
+drwxr-xr-x   0 sambit     (504) staff       (20)        0 2023-07-07 17:04:24.413256 BCemu-1.1.1/src/
+-rw-r--r--   0 sambit     (504) staff       (20)    13902 2023-07-07 17:00:00.000000 BCemu-1.1.1/src/BaryonEffectsEmulator.py
+-rwxr-xr-x   0 sambit     (504) staff       (20)      433 2022-04-01 07:23:56.000000 BCemu-1.1.1/src/__init__.py
+-rw-r--r--   0 sambit     (504) staff       (20)     1722 2022-04-01 07:23:56.000000 BCemu-1.1.1/src/download.py
+-rw-r--r--   0 sambit     (504) staff       (20)     6157 2022-04-01 07:23:56.000000 BCemu-1.1.1/src/functions.py
+drwxr-xr-x   0 sambit     (504) staff       (20)        0 2023-07-07 17:04:24.413409 BCemu-1.1.1/src/input_data/
+-rw-r--r--   0 sambit     (504) staff       (20)       92 2022-04-01 07:23:56.000000 BCemu-1.1.1/src/input_data/README.rst
+-rw-r--r--   0 sambit     (504) staff       (20)     1606 2022-04-01 07:23:56.000000 BCemu-1.1.1/src/kpls.py
+drwxr-xr-x   0 sambit     (504) staff       (20)        0 2023-07-07 17:04:24.413619 BCemu-1.1.1/tests/
+-rw-r--r--   0 sambit     (504) staff       (20)      871 2022-04-01 07:23:56.000000 BCemu-1.1.1/tests/test_Sk.py
```

### Comparing `BCemu-1.1/BCemu.egg-info/PKG-INFO` & `BCemu-1.1.1/BCemu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BCemu
-Version: 1.1
+Version: 1.1.1
 Summary: Using emulators to implement baryonic effects.
 Home-page: https://github.com/sambit-giri/BCemu.git
 Author: Sambit Giri
 Author-email: sambit.giri@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -82,15 +82,15 @@
 
 ```
 
 <img src="images/Sk_z0_7param.png" width="400">
 
 The package also has a three parameter barynification model. Model A assumes all the three parameters to be independent of redshift while model B assumes the parameters to be redshift dependent via the following form: 
 
-![](https://latex.codecogs.com/svg.latex?\inline&space;X(z)&space;=&space;X_0(1&plus;z)^\nu).
+![](https://latex.codecogs.com/svg.latex?\inline&space;X(z)&space;=&space;X_0(1&plus;z)^{-\nu}).
 
 Below an example fit to the BAHAMAS simulation result is shown.
 
 ```python
 import numpy as np 
 import matplotlib.pyplot as plt
 import BCemu
```

### Comparing `BCemu-1.1/LICENSE` & `BCemu-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BCemu-1.1/PKG-INFO` & `BCemu-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BCemu
-Version: 1.1
+Version: 1.1.1
 Summary: Using emulators to implement baryonic effects.
 Home-page: https://github.com/sambit-giri/BCemu.git
 Author: Sambit Giri
 Author-email: sambit.giri@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -82,15 +82,15 @@
 
 ```
 
 <img src="images/Sk_z0_7param.png" width="400">
 
 The package also has a three parameter barynification model. Model A assumes all the three parameters to be independent of redshift while model B assumes the parameters to be redshift dependent via the following form: 
 
-![](https://latex.codecogs.com/svg.latex?\inline&space;X(z)&space;=&space;X_0(1&plus;z)^\nu).
+![](https://latex.codecogs.com/svg.latex?\inline&space;X(z)&space;=&space;X_0(1&plus;z)^{-\nu}).
 
 Below an example fit to the BAHAMAS simulation result is shown.
 
 ```python
 import numpy as np 
 import matplotlib.pyplot as plt
 import BCemu
```

### Comparing `BCemu-1.1/README.md` & `BCemu-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 ```
 
 <img src="images/Sk_z0_7param.png" width="400">
 
 The package also has a three parameter barynification model. Model A assumes all the three parameters to be independent of redshift while model B assumes the parameters to be redshift dependent via the following form: 
 
-![](https://latex.codecogs.com/svg.latex?\inline&space;X(z)&space;=&space;X_0(1&plus;z)^\nu).
+![](https://latex.codecogs.com/svg.latex?\inline&space;X(z)&space;=&space;X_0(1&plus;z)^{-\nu}).
 
 Below an example fit to the BAHAMAS simulation result is shown.
 
 ```python
 import numpy as np 
 import matplotlib.pyplot as plt
 import BCemu
```

### Comparing `BCemu-1.1/setup.py` & `BCemu-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from setuptools import setup, find_packages
 #from distutils.core import setup
 
 BCMemu_link = 'https://github.com/sambit-giri/BCemu.git'
 
 setup(name='BCemu',
-      version='1.1',
+      version='1.1.1',
       description='Using emulators to implement baryonic effects.',
       url=BCMemu_link,
       author='Sambit Giri',
       author_email='sambit.giri@gmail.com',
       # packages=find_packages("src"),
       # package_dir={"": "src"},
       package_dir = {'BCemu' : 'src'},
```

### Comparing `BCemu-1.1/src/BaryonEffectsEmulator.py` & `BCemu-1.1.1/src/BaryonEffectsEmulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 		emulators = []
 		zs = []
 		for ke in self.emul_names:
 			zs.append(float(ke))
 			emu = pickle.load(open(self.emul_names[ke],'rb'))
 			emu.options['print_prediction'] = False
 			emulators.append(emu)
-		print('Emulators loaded.')
+		if self.verbose: print('Emulators loaded.')
 		self.emulators = np.array(emulators)
 		self.emul_zs   = np.array(zs)
 
 	def update_cosmology(self, Ob, Om):
 		self.fb = Ob/Om
 		if self.verbose: print('Baryon fraction is set to {:.3f}'.format(self.fb))
 
@@ -228,15 +228,15 @@
 			pp, kk = self.run(BCM_params, z=z)
 		else:
 			p0p0, kk = self.run(BCM_params, z=0)
 			p0p5, kk = self.run(BCM_params, z=0.5)
 			p1p0, kk = self.run(BCM_params, z=1)
 			p1p5, kk = self.run(BCM_params, z=1.5)
 			p2p0, kk = self.run(BCM_params, z=2)
-			P = np.array([p0p0,p0p5,p1p5,p1p5,p2p0])
+			P = np.array([p0p0,p0p5,p1p0,p1p5,p2p0])
 			pp = np.array([splev(z,splrep([0,0.5,1,1.5,2], P[:,ii], s=0, k=1)) 
 									for ii,ki in enumerate(kk)])
 			if z>2:
 				if str(self.above_zmax).lower()=='zmax':
 					print('Redshift z>2 is outside the training set and therefore set to suppressions at z=2.')
 					pp = p2p0
 				else:
```

### Comparing `BCemu-1.1/src/download.py` & `BCemu-1.1.1/src/download.py`

 * *Files identical despite different names*

### Comparing `BCemu-1.1/src/functions.py` & `BCemu-1.1.1/src/functions.py`

 * *Files identical despite different names*

### Comparing `BCemu-1.1/src/kpls.py` & `BCemu-1.1.1/src/kpls.py`

 * *Files identical despite different names*

