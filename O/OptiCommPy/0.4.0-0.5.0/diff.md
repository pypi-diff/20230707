# Comparing `tmp/OptiCommPy-0.4.0.tar.gz` & `tmp/OptiCommPy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OptiCommPy-0.4.0.tar", last modified: Sun Jul  2 19:40:57 2023, max compression
+gzip compressed data, was "OptiCommPy-0.5.0.tar", last modified: Fri Jul  7 20:45:59 2023, max compression
```

## Comparing `OptiCommPy-0.4.0.tar` & `OptiCommPy-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 19:40:57.100672 OptiCommPy-0.4.0/
--rw-rw-rw-   0        0        0    35823 2022-08-27 14:09:58.000000 OptiCommPy-0.4.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-02 19:40:57.094671 OptiCommPy-0.4.0/OptiCommPy.egg-info/
--rw-rw-rw-   0        0        0     3869 2023-07-02 19:40:56.000000 OptiCommPy-0.4.0/OptiCommPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-07-02 19:40:56.000000 OptiCommPy-0.4.0/OptiCommPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 19:40:56.000000 OptiCommPy-0.4.0/OptiCommPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-07-02 19:40:56.000000 OptiCommPy-0.4.0/OptiCommPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 19:40:56.000000 OptiCommPy-0.4.0/OptiCommPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3869 2023-07-02 19:40:57.099670 OptiCommPy-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3182 2023-04-06 02:54:53.000000 OptiCommPy-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 19:40:57.098668 OptiCommPy-0.4.0/optic/
--rw-rw-rw-   0        0        0       14 2022-08-27 14:09:58.000000 OptiCommPy-0.4.0/optic/__init__.py
--rw-rw-rw-   0        0        0      105 2022-08-27 14:09:58.000000 OptiCommPy-0.4.0/optic/core.py
--rw-rw-rw-   0        0        0     9450 2023-07-02 19:21:41.000000 OptiCommPy-0.4.0/optic/plot.py
--rw-rw-rw-   0        0        0      307 2022-08-27 14:09:58.000000 OptiCommPy-0.4.0/runner
--rw-rw-rw-   0        0        0       42 2023-07-02 19:40:57.100672 OptiCommPy-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2123 2023-07-02 19:34:49.000000 OptiCommPy-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:45:59.053876 OptiCommPy-0.5.0/
+-rw-rw-rw-   0        0        0    35823 2022-08-27 14:09:58.000000 OptiCommPy-0.5.0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-07 20:45:58.906882 OptiCommPy-0.5.0/OptiCommPy.egg-info/
+-rw-rw-rw-   0        0        0     3866 2023-07-07 20:45:58.000000 OptiCommPy-0.5.0/OptiCommPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-07-07 20:45:58.000000 OptiCommPy-0.5.0/OptiCommPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 20:45:58.000000 OptiCommPy-0.5.0/OptiCommPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-07-07 20:45:58.000000 OptiCommPy-0.5.0/OptiCommPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 20:45:58.000000 OptiCommPy-0.5.0/OptiCommPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3866 2023-07-07 20:45:59.052877 OptiCommPy-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3179 2023-07-02 20:15:17.000000 OptiCommPy-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 20:45:58.976885 OptiCommPy-0.5.0/optic/
+-rw-rw-rw-   0        0        0       14 2022-08-27 14:09:58.000000 OptiCommPy-0.5.0/optic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:45:58.981882 OptiCommPy-0.5.0/optic/comm/
+-rw-rw-rw-   0        0        0     1644 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/comm/fec.py
+-rw-rw-rw-   0        0        0    17919 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/comm/metrics.py
+-rw-rw-rw-   0        0        0     5687 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/comm/modulation.py
+-rw-rw-rw-   0        0        0     5703 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/comm/ofdm.py
+-rw-rw-rw-   0        0        0      105 2022-08-27 14:09:58.000000 OptiCommPy-0.5.0/optic/core.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:45:58.986876 OptiCommPy-0.5.0/optic/dsp/
+-rw-rw-rw-   0        0        0     8195 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/dsp/carrierRecovery.py
+-rw-rw-rw-   0        0        0     8874 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/dsp/core.py
+-rw-rw-rw-   0        0        0      892 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/dsp/coreGPU.py
+-rw-rw-rw-   0        0        0    23094 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/dsp/equalization.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:45:59.050876 OptiCommPy-0.5.0/optic/models/
+-rw-rw-rw-   0        0        0    24484 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/models/amplification.py
+-rw-rw-rw-   0        0        0    14687 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/models/channels.py
+-rw-rw-rw-   0        0        0    11705 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/models/devices.py
+-rw-rw-rw-   0        0        0    23028 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/models/modelsGPU.py
+-rw-rw-rw-   0        0        0     6159 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/models/tx.py
+-rw-rw-rw-   0        0        0     9450 2023-07-02 19:21:41.000000 OptiCommPy-0.5.0/optic/plot.py
+-rw-rw-rw-   0        0        0      307 2022-08-27 14:09:58.000000 OptiCommPy-0.5.0/runner
+-rw-rw-rw-   0        0        0       42 2023-07-07 20:45:59.053876 OptiCommPy-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     2376 2023-07-07 20:43:19.000000 OptiCommPy-0.5.0/setup.py
```

### Comparing `OptiCommPy-0.4.0/LICENSE` & `OptiCommPy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OptiCommPy-0.4.0/OptiCommPy.egg-info/PKG-INFO` & `OptiCommPy-0.5.0/OptiCommPy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OptiCommPy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Optical Communications Algorithms with Python
 Home-page: https://github.com/edsonportosilva/OptiCommPy
 Maintainer: Edson Porto da Silva
 Maintainer-email: edsonporto88@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -15,15 +15,15 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OptiCommPy: Fiber Optic Communications with Python
 
-Simulate optical communications systems with Python. This repository is a Python-based framework to simulate systems, subsystems and components of fiber optic communication systems, for educational and research purposes.
+Simulate optical communications systems with Python. This repository is a Python-based framework to simulate systems, subsystems, and components of fiber optic communication systems, for educational and research purposes.
 <p align="center">
 <img class="center" src="https://github.com/edsonportosilva/OptiCommPy/blob/main/figures/eyeDisp.gif" width="400">  <img class="center" src="https://github.com/edsonportosilva/OptiCommPy/blob/main/figures/40GOOK_spectrum.jpg" width="400">
 
 <img src="https://github.com/edsonportosilva/OptiCommPy/blob/main/figures/DSP.jpg" width="800">
 
 </p>
 
@@ -44,19 +44,19 @@
 * Evaluate transmission performance with metrics such as:
   - *Bit-error-rate* (BER).
   - *Symbol-error-rate* (SER).
   - *Error vector magnitude* (EVM).
   - *Mutual information* (MI).
   - *Generalized mutual information* (GMI).  
   - *Normalized generalized mutual information* (NGMI). 
-* Vizualization of the spectrum of electrical/optical signals, signal constellations and eyediagrams.
+* Visualization of the spectrum of electrical/optical signals, signal constellations, and eyediagrams.
 
 ## How can I contribute?
 
-If you want to contribute to this project, just implement the feature you want and send me a pull request. If you want to suggest new features or discuss anything related to OptiCommPy, please get in touch with me (edsonporto88@gmail.com).
+If you want to contribute to this project, implement the feature you want and send me a pull request. If you want to suggest new features or discuss anything related to OptiCommPy, please get in touch with me (edsonporto88@gmail.com).
 
 ## Requirements/Dependencies
 
 - python>=3.2
 - numpy>=1.9.2
 - scipy>=0.15.0
 - matplotlib>=1.4.3
@@ -70,15 +70,15 @@
 
 Using pip:
 
 ```
 pip install OptiCommPy
 ```
 
-Cloning the repository from github:
+Cloning the repository from GitHub:
 
 ```
 $ git clone https://github.com/edsonportosilva/OptiCommPy.git
 $ cd OptiCommPy
 $ python setup.py install
 ```
 or
```

### Comparing `OptiCommPy-0.4.0/PKG-INFO` & `OptiCommPy-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OptiCommPy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Optical Communications Algorithms with Python
 Home-page: https://github.com/edsonportosilva/OptiCommPy
 Maintainer: Edson Porto da Silva
 Maintainer-email: edsonporto88@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -15,15 +15,15 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OptiCommPy: Fiber Optic Communications with Python
 
-Simulate optical communications systems with Python. This repository is a Python-based framework to simulate systems, subsystems and components of fiber optic communication systems, for educational and research purposes.
+Simulate optical communications systems with Python. This repository is a Python-based framework to simulate systems, subsystems, and components of fiber optic communication systems, for educational and research purposes.
 <p align="center">
 <img class="center" src="https://github.com/edsonportosilva/OptiCommPy/blob/main/figures/eyeDisp.gif" width="400">  <img class="center" src="https://github.com/edsonportosilva/OptiCommPy/blob/main/figures/40GOOK_spectrum.jpg" width="400">
 
 <img src="https://github.com/edsonportosilva/OptiCommPy/blob/main/figures/DSP.jpg" width="800">
 
 </p>
 
@@ -44,19 +44,19 @@
 * Evaluate transmission performance with metrics such as:
   - *Bit-error-rate* (BER).
   - *Symbol-error-rate* (SER).
   - *Error vector magnitude* (EVM).
   - *Mutual information* (MI).
   - *Generalized mutual information* (GMI).  
   - *Normalized generalized mutual information* (NGMI). 
-* Vizualization of the spectrum of electrical/optical signals, signal constellations and eyediagrams.
+* Visualization of the spectrum of electrical/optical signals, signal constellations, and eyediagrams.
 
 ## How can I contribute?
 
-If you want to contribute to this project, just implement the feature you want and send me a pull request. If you want to suggest new features or discuss anything related to OptiCommPy, please get in touch with me (edsonporto88@gmail.com).
+If you want to contribute to this project, implement the feature you want and send me a pull request. If you want to suggest new features or discuss anything related to OptiCommPy, please get in touch with me (edsonporto88@gmail.com).
 
 ## Requirements/Dependencies
 
 - python>=3.2
 - numpy>=1.9.2
 - scipy>=0.15.0
 - matplotlib>=1.4.3
@@ -70,15 +70,15 @@
 
 Using pip:
 
 ```
 pip install OptiCommPy
 ```
 
-Cloning the repository from github:
+Cloning the repository from GitHub:
 
 ```
 $ git clone https://github.com/edsonportosilva/OptiCommPy.git
 $ cd OptiCommPy
 $ python setup.py install
 ```
 or
```

### Comparing `OptiCommPy-0.4.0/README.md` & `OptiCommPy-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # OptiCommPy: Fiber Optic Communications with Python
 
-Simulate optical communications systems with Python. This repository is a Python-based framework to simulate systems, subsystems and components of fiber optic communication systems, for educational and research purposes.
+Simulate optical communications systems with Python. This repository is a Python-based framework to simulate systems, subsystems, and components of fiber optic communication systems, for educational and research purposes.
 <p align="center">
 <img class="center" src="https://github.com/edsonportosilva/OptiCommPy/blob/main/figures/eyeDisp.gif" width="400">  <img class="center" src="https://github.com/edsonportosilva/OptiCommPy/blob/main/figures/40GOOK_spectrum.jpg" width="400">
 
 <img src="https://github.com/edsonportosilva/OptiCommPy/blob/main/figures/DSP.jpg" width="800">
 
 </p>
 
@@ -25,19 +25,19 @@
 * Evaluate transmission performance with metrics such as:
   - *Bit-error-rate* (BER).
   - *Symbol-error-rate* (SER).
   - *Error vector magnitude* (EVM).
   - *Mutual information* (MI).
   - *Generalized mutual information* (GMI).  
   - *Normalized generalized mutual information* (NGMI). 
-* Vizualization of the spectrum of electrical/optical signals, signal constellations and eyediagrams.
+* Visualization of the spectrum of electrical/optical signals, signal constellations, and eyediagrams.
 
 ## How can I contribute?
 
-If you want to contribute to this project, just implement the feature you want and send me a pull request. If you want to suggest new features or discuss anything related to OptiCommPy, please get in touch with me (edsonporto88@gmail.com).
+If you want to contribute to this project, implement the feature you want and send me a pull request. If you want to suggest new features or discuss anything related to OptiCommPy, please get in touch with me (edsonporto88@gmail.com).
 
 ## Requirements/Dependencies
 
 - python>=3.2
 - numpy>=1.9.2
 - scipy>=0.15.0
 - matplotlib>=1.4.3
@@ -51,15 +51,15 @@
 
 Using pip:
 
 ```
 pip install OptiCommPy
 ```
 
-Cloning the repository from github:
+Cloning the repository from GitHub:
 
 ```
 $ git clone https://github.com/edsonportosilva/OptiCommPy.git
 $ cd OptiCommPy
 $ python setup.py install
 ```
 or
```

### Comparing `OptiCommPy-0.4.0/optic/plot.py` & `OptiCommPy-0.5.0/optic/plot.py`

 * *Files identical despite different names*

### Comparing `OptiCommPy-0.4.0/setup.py` & `OptiCommPy-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,34 +7,35 @@
 DISTNAME = 'OptiCommPy'
 DESCRIPTION = 'Optical Communications Algorithms with Python'
 LONG_DESCRIPTION = open('README.md', encoding="utf8").read()
 MAINTAINER = 'Edson Porto da Silva'
 MAINTAINER_EMAIL = 'edsonporto88@gmail.com'
 URL = 'https://github.com/edsonportosilva/OptiCommPy'
 LICENSE = 'BSD 3-Clause'
-VERSION = '0.4.0'
+VERSION = '0.5.0'
 
 #This is a list of files to install, and where
 #(relative to the 'root' dir, where setup.py is)
 #You could be more specific.
-files = ["optic/*"]
+files = ["optic/*","optic/comm/*","optic/dsp/*", "optic/models/*", "optic/comm/fecParams/*","optic/models/ampParams/*"]
 
 setup(
     name=DISTNAME,
     maintainer=MAINTAINER,
     maintainer_email=MAINTAINER_EMAIL,
     description=DESCRIPTION,
     license=LICENSE,
     url=URL,
     version=VERSION,
     #Name the folder where your packages live:
     #(If you have other packages (dirs) or modules (py files) then
     #put them into the package directory - they will be found
     #recursively.)
-    packages=['optic'],
+    packages=['optic', 'optic.comm', 'optic.models', 'optic.dsp','optic.models.ampParams','optic.comm.fecParams'],
+    #py_modules = ['plot', 'core', 'comm', 'dsp', 'models'],
     install_requires=[
           'numpy>=1.9.2',
           'scipy>=0.15.0',
           'matplotlib>=3.7.0',
           'sympy',
           'tqdm>=4.64.1',
           'numba>=0.54.1',
```

