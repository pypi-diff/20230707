# Comparing `tmp/mastsel-0.1.tar.gz` & `tmp/mastsel-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastsel-0.1.tar", last modified: Thu Apr  6 16:10:17 2023, max compression
+gzip compressed data, was "mastsel-1.1.tar", last modified: Fri Jul  7 08:51:38 2023, max compression
```

## Comparing `mastsel-0.1.tar` & `mastsel-1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-06 16:10:17.482845 mastsel-0.1/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-06 16:10:17.479512 mastsel-0.1/.github/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-06 16:10:17.479512 mastsel-0.1/.github/workflows/
--rw-r--r--   0 simon     (1000) simon     (1000)      923 2023-03-28 07:09:22.000000 mastsel-0.1/.github/workflows/publish.yml
--rw-r--r--   0 simon     (1000) simon     (1000)     1819 2023-03-28 07:09:22.000000 mastsel-0.1/.gitignore
--rw-r--r--   0 simon     (1000) simon     (1000)     1064 2023-03-31 16:17:21.000000 mastsel-0.1/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)       25 2023-04-06 16:06:53.000000 mastsel-0.1/MANIFEST.in
--rw-r--r--   0 simon     (1000) simon     (1000)     1448 2023-04-06 16:10:17.482845 mastsel-0.1/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     1110 2023-03-28 07:09:22.000000 mastsel-0.1/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-06 16:10:17.479512 mastsel-0.1/mastsel/
--rw-r--r--   0 simon     (1000) simon     (1000)      402 2023-03-28 07:09:22.000000 mastsel-0.1/mastsel/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      155 2023-04-06 16:10:17.000000 mastsel-0.1/mastsel/_version.py
--rw-r--r--   0 simon     (1000) simon     (1000)      971 2023-01-18 11:49:49.000000 mastsel-0.1/mastsel/ini_to_yaml.py
--rw-r--r--   0 simon     (1000) simon     (1000)    20442 2023-04-06 15:56:12.000000 mastsel-0.1/mastsel/mavisFormulas.py
--rw-r--r--   0 simon     (1000) simon     (1000)    42007 2023-04-06 15:56:12.000000 mastsel-0.1/mastsel/mavisLO.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6165 2023-01-18 11:49:49.000000 mastsel-0.1/mastsel/mavisParams.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6033 2023-01-18 11:49:49.000000 mastsel-0.1/mastsel/mavisParamsOld.py
--rw-r--r--   0 simon     (1000) simon     (1000)    13216 2023-01-18 11:49:49.000000 mastsel-0.1/mastsel/mavisPsf.py
--rw-r--r--   0 simon     (1000) simon     (1000)     7956 2023-03-28 07:09:22.000000 mastsel-0.1/mastsel/mavisUtilities.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-06 16:10:17.479512 mastsel-0.1/mastsel.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     1448 2023-04-06 16:10:17.000000 mastsel-0.1/mastsel.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      657 2023-04-06 16:10:17.000000 mastsel-0.1/mastsel.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-04-06 16:10:17.000000 mastsel-0.1/mastsel.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       56 2023-04-06 16:10:17.000000 mastsel-0.1/mastsel.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        8 2023-04-06 16:10:17.000000 mastsel-0.1/mastsel.egg-info/top_level.txt
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-06 16:10:17.482845 mastsel-0.1/notebooks/
--rw-r--r--   0 simon     (1000) simon     (1000)     3063 2023-01-18 11:49:49.000000 mastsel-0.1/notebooks/MAVIS-CONVOLUTION-TEST.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)     9842 2023-01-18 11:49:49.000000 mastsel-0.1/notebooks/MAVIS-CONVOLUTION.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)    10266 2023-03-28 07:09:22.000000 mastsel-0.1/notebooks/MAVIS.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)    10100 2023-01-18 11:49:49.000000 mastsel-0.1/notebooks/MAVIS2.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)     3929 2023-01-18 11:49:49.000000 mastsel-0.1/notebooks/MAVIS3.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)     7064 2023-01-18 11:49:49.000000 mastsel-0.1/notebooks/MAVIS_INT_REC.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)     3896 2023-01-18 11:49:49.000000 mastsel-0.1/notebooks/MAVIS_MAIN.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)      711 2023-04-06 15:56:12.000000 mastsel-0.1/pyproject.toml
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-04-06 16:10:17.482845 mastsel-0.1/setup.cfg
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-06 16:10:17.482845 mastsel-0.1/tests/
--rw-r--r--   0 simon     (1000) simon     (1000)     8749 2023-01-18 11:49:49.000000 mastsel-0.1/tests/allTests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.713973 mastsel-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 08:51:22.000000 mastsel-1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-07 08:51:22.000000 mastsel-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 08:51:22.000000 mastsel-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 08:51:22.000000 mastsel-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-07 08:51:38.709973 mastsel-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-07 08:51:22.000000 mastsel-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/mastsel/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/ini_to_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisFormulas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45142 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisParams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisParamsOld.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisPsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisUtilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/mastsel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS-CONVOLUTION-TEST.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS-CONVOLUTION.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS_INT_REC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS_MAIN.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-07 08:51:22.000000 mastsel-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:51:38.713973 mastsel-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-07 08:51:22.000000 mastsel-1.1/tests/allTests.py
```

### Comparing `mastsel-0.1/.github/workflows/publish.yml` & `mastsel-1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/.gitignore` & `mastsel-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/LICENSE` & `mastsel-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/PKG-INFO` & `mastsel-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastsel
-Version: 0.1
+Version: 1.1
 Summary: Asterism Selection for MAVIS instrument
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/MASTSEL
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
```

### Comparing `mastsel-0.1/README.md` & `mastsel-1.1/README.md`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/mastsel/ini_to_yaml.py` & `mastsel-1.1/mastsel/ini_to_yaml.py`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/mastsel/mavisFormulas.py` & `mastsel-1.1/mastsel/mavisFormulas.py`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/mastsel/mavisLO.py` & `mastsel-1.1/mastsel/mavisLO.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,225 +13,167 @@
 import multiprocessing as mp
 from configparser import ConfigParser
 import yaml
 import os
 
 
 class MavisLO(object):
+    
+    def check_section_key(self, primary):
+        if self.configType == 'ini':
+            return self.config.has_section(primary)
+        elif self.configType == 'yml':
+            return primary in self.my_yaml_dict.keys()
+    
+    def check_config_key(self, primary, secondary):
+        if self.configType == 'ini':
+            return self.config.has_option(primary, secondary)
+        elif self.configType == 'yml':
+            if primary in self.my_yaml_dict.keys():
+                return secondary in self.my_yaml_dict[primary].keys()
+            else:
+                return False
+
+    def get_config_value(self, primary, secondary):
+        if self.configType == 'ini':
+            return eval(self.config[primary][secondary])
+        elif self.configType == 'yml':
+            return self.my_yaml_dict[primary][secondary]
 
     def __init__(self, path, parametersFile, verbose=False):
 
-        self.verbose=verbose
+        self.verbose = verbose
+        self.plot4debug = False
+        self.displayEquation = False
 
         filename_ini = os.path.join(path, parametersFile + '.ini')
         filename_yml = os.path.join(path, parametersFile + '.yml')
 
+        self.error = False
         if os.path.exists(filename_yml):
+            self.configType = 'yml'
             with open(filename_yml) as f:
                 self.my_yaml_dict = yaml.safe_load(f)
-                
-            self.TelescopeDiameter      = self.my_yaml_dict['telescope']['TelescopeDiameter']
-            self.ZenithAngle            = self.my_yaml_dict['telescope']['ZenithAngle']
-            self.TechnicalFoV           = self.my_yaml_dict['telescope']['TechnicalFoV']
-            self.ObscurationRatio       = self.my_yaml_dict['telescope']['ObscurationRatio']
-            if 'windPsdFile' in self.my_yaml_dict['telescope'].keys():
-                windPsdFile = self.my_yaml_dict['telescope']['windPsdFile']
-                self.psd_freq, self.psd_tip_wind, self.psd_tilt_wind = self.loadWindPsd(windPsdFile)
-            else:
-                print('No windPsdFile file is set.')
-                self.psd_freq = np.asarray(np.linspace(0.5, 250.0, 500))
-                self.psd_tip_wind = np.zeros((500))
-                self.psd_tilt_wind = np.zeros((500))
-
-            self.AtmosphereWavelength   = self.my_yaml_dict['atmosphere']['Wavelength']
-            self.L0                     = self.my_yaml_dict['atmosphere']['L0']
-            self.Cn2Weights             = self.my_yaml_dict['atmosphere']['Cn2Weights']
-            self.Cn2Heights             = self.my_yaml_dict['atmosphere']['Cn2Heights']
-
-            SensingWavelength_LO = self.my_yaml_dict['sources_LO']['Wavelength']
-            if isinstance(SensingWavelength_LO, list):
-                self.SensingWavelength_LO = SensingWavelength_LO[0]
-            else:
-                self.SensingWavelength_LO = SensingWavelength_LO
-
-            self.NumberLenslets         = self.my_yaml_dict['sensor_LO']['NumberLenslets']
-
-            self.N_sa_tot_LO            = self.NumberLenslets[0]**2
-            if self.NumberLenslets[0] > 2:
-                self.N_sa_tot_LO        = int ( np.floor( self.N_sa_tot_LO * np.pi/4.0 * (1.0 - self.ObscurationRatio**2) ) )
-
-            self.PixelScale_LO          = self.my_yaml_dict['sensor_LO']['PixelScale']
-            self.WindowRadiusWCoG_LO    = self.my_yaml_dict['sensor_LO']['WindowRadiusWCoG']
-            self.sigmaRON_LO            = self.my_yaml_dict['sensor_LO']['SigmaRON']
-            if self.sigmaRON_LO == 0:
-                self.sigmaRON_LO = 1e-6
-            self.ExcessNoiseFactor_LO   = self.my_yaml_dict['sensor_LO']['ExcessNoiseFactor']
-            self.Dark_LO                = self.my_yaml_dict['sensor_LO']['Dark']
-            self.skyBackground_LO       = self.my_yaml_dict['sensor_LO']['SkyBackground']
-            self.ThresholdWCoG_LO       = self.my_yaml_dict['sensor_LO']['ThresholdWCoG']
-            self.NewValueThrPix_LO      = self.my_yaml_dict['sensor_LO']['NewValueThrPix']
-
-            if 'noNoise' in self.my_yaml_dict['sensor_LO'].keys():
-                self.noNoise = self.my_yaml_dict['sensor_LO']['noNoise']
-            else:
-                self.noNoise = False
+        elif os.path.exists(filename_ini):
+            self.configType = 'ini'
+            self.config = ConfigParser()
+            self.config.optionxform = str
+            self.config.read(filename_ini)
+        else:
+            print('%%%%%%%% ERROR %%%%%%%%')
+            print('The .ini or .yml file does not exist\n')
+            self.error = True
+            return
+        
+        self.TelescopeDiameter      = self.get_config_value('telescope','TelescopeDiameter')  
+        self.ZenithAngle            = self.get_config_value('telescope','ZenithAngle')  
+        self.TechnicalFoV           = self.get_config_value('telescope','TechnicalFoV')  
+        self.ObscurationRatio       = self.get_config_value('telescope','ObscurationRatio')   
+        
+        if self.check_config_key('telescope','windPsdFile'):        
+            windPsdFile = self.get_config_value('telescope','windPsdFile')
+            self.psd_freq, self.psd_tip_wind, self.psd_tilt_wind = self.loadWindPsd(windPsdFile)
+        else:
+            print('No windPsdFile file is set.')
+            self.psd_freq = np.asarray(np.linspace(0.5, 250.0, 500))
+            self.psd_tip_wind = np.zeros((500))
+            self.psd_tilt_wind = np.zeros((500))
+
+        self.AtmosphereWavelength   = self.get_config_value('atmosphere','Wavelength')
+        self.L0                     = self.get_config_value('atmosphere','L0')
+        self.Cn2Weights             = self.get_config_value('atmosphere','Cn2Weights')
+        self.Cn2Heights             = self.get_config_value('atmosphere','Cn2Heights')
+       
+        if np.min(self.Cn2Heights) == 0:
+            self.Cn2Heights[np.argmin(self.Cn2Heights)] = 1e-6
+
+        SensingWavelength_LO = self.get_config_value('sources_LO','Wavelength')
+        if isinstance(SensingWavelength_LO, list):
+            self.SensingWavelength_LO = SensingWavelength_LO[0]
+        else:
+            self.SensingWavelength_LO = SensingWavelength_LO
 
-            self.DmHeights              = self.my_yaml_dict['DM']['DmHeights']
+        self.NumberLenslets         = self.get_config_value('sensor_LO','NumberLenslets')
 
-            self.SensorFrameRate_LO     = self.my_yaml_dict['RTC']['SensorFrameRate_LO']
-            self.loopDelaySteps_LO      = self.my_yaml_dict['RTC']['LoopDelaySteps_LO']
+        self.N_sa_tot_LO            = self.NumberLenslets[0]**2
+        if self.NumberLenslets[0] > 2:
+            self.N_sa_tot_LO        = int ( np.floor( self.N_sa_tot_LO * np.pi/4.0 * (1.0 - self.ObscurationRatio**2) ) )
+
+        self.PixelScale_LO          = self.get_config_value('sensor_LO','PixelScale')
+        self.WindowRadiusWCoG_LO    = self.get_config_value('sensor_LO','WindowRadiusWCoG')
+        self.sigmaRON_LO            = self.get_config_value('sensor_LO','SigmaRON')
+        if self.sigmaRON_LO == 0:
+            self.sigmaRON_LO = 1e-6
+        self.ExcessNoiseFactor_LO   = self.get_config_value('sensor_LO','ExcessNoiseFactor')
+        self.Dark_LO                = self.get_config_value('sensor_LO','Dark')
+        self.skyBackground_LO       = self.get_config_value('sensor_LO','SkyBackground')
+        self.ThresholdWCoG_LO       = self.get_config_value('sensor_LO','ThresholdWCoG')
+        self.NewValueThrPix_LO      = self.get_config_value('sensor_LO','NewValueThrPix')
 
-            defaultCompute = 'GPU'
-            defaultIntegralDiscretization1 = 1000
-            defaultIntegralDiscretization2 = 4000
-            self.computationPlatform =defaultCompute
-            self.integralDiscretization1 = defaultIntegralDiscretization1
-            self.integralDiscretization2 = defaultIntegralDiscretization2
-
-            if 'COMPUTATION' in self.my_yaml_dict.keys():
-                if self.my_yaml_dict['COMPUTATION']['platform']:
-                    self.computationPlatform    = self.my_yaml_dict['COMPUTATION']['platform']
-                if self.my_yaml_dict['COMPUTATION']['integralDiscretization1']:
-                    self.integralDiscretization1 = self.my_yaml_dict['COMPUTATION']['integralDiscretization1']
-                if self.my_yaml_dict['COMPUTATION']['integralDiscretization2']:
-                    self.integralDiscretization2 = self.my_yaml_dict['COMPUTATION']['integralDiscretization2']
+        
+        if self.check_config_key('sensor_LO','noNoise'):
+            self.noNoise = self.get_config_value('sensor_LO','noNoise')
+        else:
+            self.noNoise = False
 
-            if 'r0_Value' in self.my_yaml_dict['atmosphere'].keys() and 'Seeing' in self.my_yaml_dict['atmosphere'].keys():
-                print('%%%%%%%% ATTENTION %%%%%%%%')
-                print('You must provide r0_Value or Seeing value, not both, ')
-                print('Seeing parameter will be used, r0_Value will be discarded!\n')
+        self.DmHeights              = self.get_config_value('DM','DmHeights')
 
-            if 'Seeing' in self.my_yaml_dict['atmosphere'].keys():
-                self.Seeing = self.my_yaml_dict['atmosphere']['Seeing']
-                self.r0_Value = 0.976*self.AtmosphereWavelength/self.Seeing*206264.8 # old: 0.15
-            else:
-                self.r0_Value = self.my_yaml_dict['atmosphere']['r0_Value']
+        self.SensorFrameRate_LO     = self.get_config_value('RTC','SensorFrameRate_LO')
+        self.loopDelaySteps_LO      = self.get_config_value('RTC','LoopDelaySteps_LO')
+        self.LoopGain_LO            = self.get_config_value('RTC','LoopGain_LO')
+
+        defaultCompute = 'GPU'
+        defaultIntegralDiscretization1 = 1000
+        defaultIntegralDiscretization2 = 4000
+        self.computationPlatform =defaultCompute
+        self.integralDiscretization1 = defaultIntegralDiscretization1
+        self.integralDiscretization2 = defaultIntegralDiscretization2
+        
+        if self.check_section_key('COMPUTATION'):
+            if self.check_config_key('COMPUTATION','platform'):
+                self.computationPlatform    = self.get_config_value('COMPUTATION','platform')
+            if self.check_config_key('COMPUTATION','integralDiscretization1'):
+                self.integralDiscretization1 = self.get_config_value('COMPUTATION','integralDiscretization1')
+            if self.check_config_key('COMPUTATION','integralDiscretization2'):
+                self.integralDiscretization2 = self.get_config_value('COMPUTATION','integralDiscretization2')
+
+        if self.check_config_key('atmosphere','r0_Value') and self.check_config_key('atmosphere','Seeing'):
+            print('%%%%%%%% ATTENTION %%%%%%%%')
+            print('You must provide r0_Value or Seeing value, not both, ')
+            print('Seeing parameter will be used, r0_Value will be discarded!\n')
+
+        if self.check_config_key('atmosphere','Seeing'):
+            self.Seeing = self.get_config_value('atmosphere','Seeing')
+            self.r0_Value = 0.976*self.AtmosphereWavelength/self.Seeing*206264.8 # old: 0.15
+        else:
+            self.r0_Value = self.get_config_value('atmosphere','r0_Value')
 
-            testWindspeedIsValid = False
-            if 'testWindspeed' in self.my_yaml_dict['atmosphere'].keys():
-                testWindspeed = self.my_yaml_dict['atmosphere']['testWindspeed']
-                try:
-                    testWindspeed = float(testWindspeed)
-                    if testWindspeed > 0:
-                        testWindspeedIsValid = True
-                    else:
-                        testWindspeedIsValid = False
-                except:
+        testWindspeedIsValid = False
+        if self.check_config_key('atmosphere','testWindspeed'):
+            testWindspeed = self.get_config_value('atmosphere','testWindspeed')
+            try:
+                testWindspeed = float(testWindspeed)
+                if testWindspeed > 0:
+                    testWindspeedIsValid = True
+                else:
                     testWindspeedIsValid = False
+            except:
+                testWindspeedIsValid = False
 
-            if 'WindSpeed' in self.my_yaml_dict['atmosphere'].keys() and 'testWindspeed' in self.my_yaml_dict['atmosphere'].keys():
-                if testWindspeedIsValid:
-                    print('%%%%%%%% ATTENTION %%%%%%%%')
-                    print('You must provide WindSpeed or testWindspeed value, not both, ')
-                    print('testWindspeed parameter will be used, WindSpeed will be discarded!\n')
-
+        if self.check_config_key('atmosphere','WindSpeed') and self.check_config_key('atmosphere','testWindspeed'):
             if testWindspeedIsValid:
-                self.WindSpeed = self.my_yaml_dict['atmosphere']['testWindspeed']
-            else:
-                self.wSpeed = self.my_yaml_dict['atmosphere']['WindSpeed']
-                self.WindSpeed = (np.dot( np.power(np.asarray(self.wSpeed), 5.0/3.0), np.asarray(self.Cn2Weights) ) / np.sum( np.asarray(self.Cn2Weights) ) ) ** (3.0/5.0)
-
-        else:
-            parser = ConfigParser()
-            parser.read( os.path.join(path, parametersFile + '.ini') )
-            #
-            # SETTING PARAMETERS READ FROM FILE       
-            #
-            self.TelescopeDiameter      = eval(parser.get('telescope', 'TelescopeDiameter'))
-            self.ZenithAngle            = eval(parser.get('telescope', 'ZenithAngle'))
-            self.TechnicalFoV           = eval(parser.get('telescope', 'TechnicalFoV'))
-            self.ObscurationRatio       = eval(parser.get('telescope', 'ObscurationRatio'))
-            if parser.has_option('telescope', 'windPsdFile'):
-                windPsdFile = eval(parser.get('telescope', 'windPsdFile'))
-                self.psd_freq, self.psd_tip_wind, self.psd_tilt_wind = self.loadWindPsd(windPsdFile)
-            else:
-                print('No windPsdFile file is set.')
-                self.psd_freq = np.asarray(np.linspace(0.5, 250.0, 500))
-                self.psd_tip_wind = np.zeros((500))
-                self.psd_tilt_wind = np.zeros((500))
-
-            self.AtmosphereWavelength   = eval(parser.get('atmosphere', 'Wavelength'))
-            self.L0                     = eval(parser.get('atmosphere', 'L0'))
-            self.Cn2Weights             = eval(parser.get('atmosphere', 'Cn2Weights'))
-            self.Cn2Heights             = eval(parser.get('atmosphere', 'Cn2Heights'))
-
-            SensingWavelength_LO = eval(parser.get('sources_LO', 'Wavelength'))
-            if isinstance(SensingWavelength_LO, list):
-                self.SensingWavelength_LO = SensingWavelength_LO[0]
-            else:
-                self.SensingWavelength_LO = SensingWavelength_LO
-
-            self.NumberLenslets         = eval(parser.get('sensor_LO', 'NumberLenslets'))
-
-            self.N_sa_tot_LO            = self.NumberLenslets[0]**2
-            if self.NumberLenslets[0] > 2:
-                self.N_sa_tot_LO        = int ( np.floor( self.N_sa_tot_LO * np.pi/4.0 * (1.0 - self.ObscurationRatio**2) ) )
-
-            self.PixelScale_LO          = eval(parser.get('sensor_LO', 'PixelScale'))
-            self.WindowRadiusWCoG_LO    = eval(parser.get('sensor_LO', 'WindowRadiusWCoG'))
-            self.sigmaRON_LO            = eval(parser.get('sensor_LO', 'SigmaRON'))
-            if self.sigmaRON_LO == 0:
-                self.sigmaRON_LO = 1e-6
-            self.ExcessNoiseFactor_LO   = eval(parser.get('sensor_LO', 'ExcessNoiseFactor'))
-            self.Dark_LO                = eval(parser.get('sensor_LO', 'Dark'))
-            self.skyBackground_LO       = eval(parser.get('sensor_LO', 'SkyBackground'))
-            self.ThresholdWCoG_LO       = eval(parser.get('sensor_LO', 'ThresholdWCoG'))
-            self.NewValueThrPix_LO      = eval(parser.get('sensor_LO', 'NewValueThrPix'))
-
-            if parser.has_option('sensor_LO', 'noNoise'):
-                self.noNoise = eval(parser.get('sensor_LO', 'noNoise'))
-            else:
-                self.noNoise = False
-
-            self.DmHeights              = eval(parser.get('DM', 'DmHeights'))
-
-            self.SensorFrameRate_LO     = eval(parser.get('RTC', 'SensorFrameRate_LO'))
-            self.loopDelaySteps_LO      = eval(parser.get('RTC', 'LoopDelaySteps_LO'))
-
-            defaultCompute = 'GPU'
-            defaultIntegralDiscretization1 = 1000
-            defaultIntegralDiscretization2 = 4000
-            self.computationPlatform    = eval(parser.get('COMPUTATION', 'platform', fallback='defaultCompute'))
-            self.integralDiscretization1 = eval(parser.get('COMPUTATION', 'integralDiscretization1', fallback='defaultIntegralDiscretization1'))
-            self.integralDiscretization2 = eval(parser.get('COMPUTATION', 'integralDiscretization2', fallback='defaultIntegralDiscretization2'))
-
-            if parser.has_option('atmosphere', 'r0_Value') and parser.has_option('atmosphere', 'Seeing'):
                 print('%%%%%%%% ATTENTION %%%%%%%%')
-                print('You must provide r0_Value or Seeing value, not both, ')
-                print('Seeing parameter will be used, r0_Value will be discarded!\n')
+                print('You must provide WindSpeed or testWindspeed value, not both, ')
+                print('testWindspeed parameter will be used, WindSpeed will be discarded!\n')
 
-            if parser.has_option('atmosphere', 'Seeing'):
-                self.Seeing = eval(parser.get('atmosphere', 'Seeing'))
-                self.r0_Value = 0.976*self.AtmosphereWavelength/self.Seeing*206264.8 # old: 0.15
-            else:
-                self.r0_Value = eval(parser.get('atmosphere', 'r0_Value'))
-
-            testWindspeedIsValid = False
-            if parser.has_option('atmosphere', 'testWindspeed'):
-                testWindspeed = parser.get('atmosphere', 'testWindspeed')
-                try:
-                    testWindspeed = float(testWindspeed)
-                    if testWindspeed > 0:
-                        testWindspeedIsValid = True
-                    else:
-                        testWindspeedIsValid = False
-                except:
-                    testWindspeedIsValid = False
-
-            if parser.has_option('atmosphere', 'WindSpeed') and parser.has_option('atmosphere', 'testWindspeed'):
-                if testWindspeedIsValid:
-                    print('%%%%%%%% ATTENTION %%%%%%%%')
-                    print('You must provide WindSpeed or testWindspeed value, not both, ')
-                    print('testWindspeed parameter will be used, WindSpeed will be discarded!\n')
-
-            if testWindspeedIsValid:
-                self.WindSpeed = eval(parser.get('atmosphere', 'testWindspeed'))
-            else:
-                self.wSpeed = eval(parser.get('atmosphere', 'WindSpeed'))
-                self.WindSpeed = (np.dot( np.power(np.asarray(self.wSpeed), 5.0/3.0), np.asarray(self.Cn2Weights) ) / np.sum( np.asarray(self.Cn2Weights) ) ) ** (3.0/5.0)   
+        if testWindspeedIsValid:
+            self.WindSpeed = self.get_config_value('atmosphere','testWindspeed')
+        else:
+            self.wSpeed = self.get_config_value('atmosphere','WindSpeed')
+            self.WindSpeed = (np.dot( np.power(np.asarray(self.wSpeed), 5.0/3.0), np.asarray(self.Cn2Weights) ) / np.sum( np.asarray(self.Cn2Weights) ) ) ** (3.0/5.0)
 
         #
         # END OF SETTING PARAMETERS READ FROM FILE       
         #
         
         airmass = 1/np.cos(self.ZenithAngle*np.pi/180)
         self.r0_Value = self.r0_Value * airmass**(-3.0/5.0)
@@ -275,63 +217,142 @@
     # specialized formulas, mostly substituting parameter with mavisParametrs.py values
     def specializedIM(self, alib=cpulib):
         apIM = self.MavisFormulas['interactionMatrixNGS']
         apIM = subsParamsByName(apIM, {'D':self.TelescopeDiameter, 'r_FoV':self.TechnicalFoV*arcsecsToRadians/2.0, 'H_DM':max(self.DmHeights)})
         xx, yy = sp.symbols('x_1 y_1', real=True)
         apIM = subsParamsByName(apIM, {'x_NGS':xx, 'y_NGS':yy})
         apIM_func = sp.lambdify((xx, yy), apIM, modules=alib)
+        if self.displayEquation:
+            print('mavisLO.specializedIM')
+            print('    apIM')
+            try:
+                display(apIM)
+            except:
+                print('    no apIM')
+            print('    apIM_func')
+            try:
+                display(apIM_func)
+            except:
+                print('    no apIM_func')
         return apIM, apIM_func
 
     
     def specializedMeanVarFormulas(self, kind):
         dd0 = {'t':self.ThresholdWCoG_LO, 'nu':self.NewValueThrPix_LO, 'sigma_RON':self.sigmaRON_LO}
         dd1 = {'b':self.Dark_LO/self.SensorFrameRate_LO}
         dd2 = {'F':self.ExcessNoiseFactor_LO}
         expr0, exprK, integral = self.MavisFormulas[kind+"0"], self.MavisFormulas[kind+"1"], self.MavisFormulas[kind+"2"]
         expr0 = subsParamsByName( expr0, {**dd0, **dd1} )
         exprK = subsParamsByName( exprK, {**dd1} )
         integral = subsParamsByName( integral,  {**dd0, **dd1, **dd2} )
+        if self.displayEquation:
+            print('mavisLO.specializedMeanVarFormulas')
+            print('    expr0')
+            try:
+                display(expr0)
+            except:
+                print('    no expr0')
+            print('    exprK')
+            try:
+                display(exprK)
+            except:
+                print('    no exprK')
+            print('    integral')
+            try:
+                display(integral)
+            except:
+                print('    no integral')
         aFunction = exprK * integral.function
         return aFunction, expr0
 
     def specializedGMeanVarFormulas(self, kind):
         dd0 = {'t':self.ThresholdWCoG_LO, 'nu':self.NewValueThrPix_LO, 'sigma_RON':self.sigmaRON_LO}
         dd1 = {'b':self.Dark_LO/self.SensorFrameRate_LO}
         dd2 = {'F':self.ExcessNoiseFactor_LO}
         expr0 = self.MavisFormulas[kind]
         expr0 = subsParamsByName( expr0, {**dd0, **dd1, **dd2} )
+        if self.displayEquation:
+            print('mavisLO.specializedGMeanVarFormulas')
+            print('    expr0')
+            try:
+                display(expr0)
+            except:
+                print('    no expr0')
         return expr0
 
     def specializedTurbFuncs(self):
         aTurbPSDTip = subsParamsByName(self.MavisFormulas['turbPSDTip'], {'V':self.WindSpeed, 'R':self.TelescopeDiameter/2.0, 'r_0':self.r0_Value, 'L_0':self.L0, 'k_y_min':0.0001, 'k_y_max':100})
         aTurbPSDTilt = subsParamsByName(self.MavisFormulas['turbPSDTilt'], {'V':self.WindSpeed, 'R':self.TelescopeDiameter/2.0, 'r_0':self.r0_Value, 'L_0':self.L0, 'k_y_min':0.0001, 'k_y_max':100})
+        if self.displayEquation:
+            print('mavisLO.specializedTurbFuncs')
+            print('    aTurbPSDTip')
+            try:
+                display(aTurbPSDTip)
+            except:
+                print('    no aTurbPSDTip')
+            print('    aTurbPSDTilt')
+            try:
+                display(aTurbPSDTilt)
+            except:
+                print('    no aTurbPSDTilt')
         return aTurbPSDTip, aTurbPSDTilt
 
     
     def specializedC_coefficient(self):
         ffC = self.MavisFormulas['noisePropagationCoefficient'].rhs
         self.fCValue1 = subsParamsByName(ffC, {'D':self.TelescopeDiameter, 'N_sa_tot':self.N_sa_tot_LO })
+        if self.displayEquation:
+            print('mavisLO.specializedC_coefficient')
+            print('    self.fCValue1')
+            try:
+                display(self.fCValue1)
+            except:
+                print('    no self.fCValue1')
         return self.fCValue1
 
     
     def specializedNoiseFuncs(self):
         dict1 = {'d':self.loopDelaySteps_LO, 'f_loop':self.SensorFrameRate_LO}
         self.fTipS_LO1 = subsParamsByName(self.MavisFormulas['completeIntegralTipLO'], dict1 ).function
         self.fTiltS_LO1 = subsParamsByName(self.MavisFormulas['completeIntegralTiltLO'], dict1).function
 #        self.fTipS_LO1 = sp.simplify(subsParamsByName(self.MavisFormulas['completeIntegralTipLO'], dict1 ).function)
 #        self.fTiltS_LO1 = sp.simplify(subsParamsByName(self.MavisFormulas['completeIntegralTiltLO'], dict1).function)
+        if self.displayEquation:
+            print('mavisLO.specializedNoiseFuncs')
+            print('    self.fTipS_LO1')
+            try:
+                display(self.fTipS_LO1)
+            except:
+                print('    no self.fTipS_LO1')
+            print('    self.fTiltS_LO1')
+            try:
+                display(self.fTiltS_LO1)
+            except:
+                print('    no self.fTiltS_LO1')
         return self.fTipS_LO1, self.fTiltS_LO1
 
     
     def specializedWindFuncs(self):
         dict1 = {'d':self.loopDelaySteps_LO, 'f_loop':self.SensorFrameRate_LO}
         self.fTipS1 = subsParamsByName(self.MavisFormulas['completeIntegralTip'], dict1).function
         self.fTiltS1 = subsParamsByName(self.MavisFormulas['completeIntegralTilt'], dict1).function
 #        self.fTipS1 = sp.simplify(subsParamsByName(self.MavisFormulas['completeIntegralTip'], dict1).function)
 #        self.fTiltS1 = sp.simplify(subsParamsByName(self.MavisFormulas['completeIntegralTilt'], dict1).function)
+        if self.displayEquation:
+            print('mavisLO.specializedWindFuncs')
+            print('    self.fTipS1')
+            try:
+                display(self.fTipS1)
+            except:
+                print('    no self.fTipS1')
+            print('    self.fTiltS1')
+            try:
+                display(self.fTiltS1)
+            except:
+                print('    no self.fTiltS1')
         return self.fTipS1, self.fTiltS1
     
     
     def buildSpecializedCovFunctions(self):
         covValue_integrationLimits = (sp.symbols('f', positive=True), 1e-3, 10.0)
         p = sp.symbols('p', real=False)
         cov_expr={}
@@ -421,39 +442,61 @@
         return mu_ktr_array, var_ktr_array, sigma_ktr_array
 
         
     def computeBias(self, aNGS_flux, aNGS_SR_LO, aNGS_FWHM_mas):
         gridSpanArcsec= self.mediumPixelScale*self.largeGridSize/1000
         gridSpanRad = gridSpanArcsec/radiansToArcsecs
         
+        # diffraction limited FWHM - full aperture
         diffNGS_FWHM_mas = self.SensingWavelength_LO/(self.TelescopeDiameter)*radiansToArcsecs*1000
-        
-        peakValue = aNGS_flux/self.SensorFrameRate_LO*aNGS_SR_LO*4.0*np.log(2)/(np.pi*(diffNGS_FWHM_mas*2.0/self.mediumPixelScale)**2)
-        if self.verbose:
-            print('mavisLO.computeBias, peakValue',peakValue)
-        peakValueNoFlux = aNGS_SR_LO*4.0*np.log(2)/(np.pi*(diffNGS_FWHM_mas*2.0/self.mediumPixelScale)**2)
-
-#        peakValue = peakValue/(40**self.TelescopeDiameter/2)
-#        peakValueNoFlux = aNGS_SR_LO*4.0*np.log(2)/(np.pi*(self.SensingWavelength_LO/(self.TelescopeDiameter/2)*radiansToArcsecs*1000/self.mediumPixelScale)**2)
-
+        # diffraction limited FWHM - one sub-aperture
+        subapNGS_FWHM_mas = self.SensingWavelength_LO/(self.TelescopeDiameter/self.NumberLenslets[0])*radiansToArcsecs*1000
+        # increment of FWHM given by the partial correction
+        FWHM_coeff = np.sqrt(np.abs(aNGS_FWHM_mas**2 - diffNGS_FWHM_mas**2 ))
+        # estimated FWHM on a sub-aperture 
+        aNGS_FWHM_mas_mod = np.sqrt( FWHM_coeff**2 + subapNGS_FWHM_mas**2 )
+        asigma = aNGS_FWHM_mas_mod/sigmaToFWHM/self.mediumPixelScale
+            
         xCoords=np.asarray(np.linspace(-self.largeGridSize/2.0+0.5, self.largeGridSize/2.0-0.5, self.largeGridSize), dtype=np.float32)
         yCoords=np.asarray(np.linspace(-self.largeGridSize/2.0+0.5, self.largeGridSize/2.0-0.5, self.largeGridSize), dtype=np.float32)
         xGrid, yGrid = np.meshgrid( xCoords, yCoords, sparse=False, copy=True)
         
-        FWHM_coeff = np.sqrt(np.abs(aNGS_FWHM_mas**2 - diffNGS_FWHM_mas**2 ))
-        
-        subapNGS_FWHM_mas = self.SensingWavelength_LO/(self.TelescopeDiameter/self.NumberLenslets[0])*radiansToArcsecs*1000
-        
-        aNGS_FWHM_mas_mod = np.sqrt( FWHM_coeff**2 + subapNGS_FWHM_mas**2 )
-        asigma = aNGS_FWHM_mas_mod/sigmaToFWHM/self.mediumPixelScale
-        g2d = peakValue * simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
-
-#        asigma = aNGS_FWHM_mas/sigmaToFWHM/self.mediumPixelScale
-#        asigma *= 40.0
-#        g2d = peakValue * simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
+        loD = self.SensingWavelength_LO/self.TelescopeDiameter*radiansToArcsecs*1000
+       
+        if aNGS_FWHM_mas >= 2*diffNGS_FWHM_mas:
+            if self.verbose:
+                print('mavisLO.computeBias, FWHM (',aNGS_FWHM_mas,') is larger than 2 times the diffraction.')
+            # if correction is low we consider that there is a seeing limited like PSF
+            g2d = simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
+            g2d = g2d * aNGS_flux/self.SensorFrameRate_LO * 1 / np.sum(g2d)
+            peakValue = np.max(g2d)
+        elif aNGS_FWHM_mas >= 1.25*diffNGS_FWHM_mas and aNGS_FWHM_mas < 2*diffNGS_FWHM_mas:
+            if self.verbose:
+                print('mavisLO.computeBias, FWHM (',aNGS_FWHM_mas,') is less than 2 times the diffraction, but more than 1.25 times diffraction.')
+            # if correction is "medium" we consider that there is a comination of diffration limited and seeing limited like PSF
+            r0_SensingWavelength_LO = self.r0_Value * (self.SensingWavelength_LO/self.AtmosphereWavelength)**(6/5)
+            seeing = 0.976*self.AtmosphereWavelength/r0_SensingWavelength_LO*206264.8 # * np.sqrt(1-2.183*(r0_SensingWavelength_LO/self.L0)*0.356)
+            seeing = np.sqrt( seeing**2 + subapNGS_FWHM_mas**2 )
+            asigma_seeing = seeing/sigmaToFWHM/self.mediumPixelScale
+            g2d_seeing = simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
+            g2d_seeing = g2d_seeing * (1-aNGS_SR_LO) * aNGS_flux/self.SensorFrameRate_LO * 1 / np.sum(g2d_seeing)
+            peakValue = aNGS_flux/self.SensorFrameRate_LO*aNGS_SR_LO*4.0*np.log(2)/(np.pi*(diffNGS_FWHM_mas/self.mediumPixelScale)**2)
+            g2d = peakValue * simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
+            g2d = g2d + g2d_seeing
+            peakValue = np.max(g2d)
+        else:
+            if self.verbose:
+                print('mavisLO.computeBias, FWHM (',aNGS_FWHM_mas,') is less than 1.25 times the diffraction.')
+            # if correction is high we consider that there is a diffraction limited core
+            # in the center of the PSF and wings given by the fitting error
+            peakValue = aNGS_flux/self.SensorFrameRate_LO*aNGS_SR_LO*4.0*np.log(2)/(np.pi*(diffNGS_FWHM_mas/self.mediumPixelScale)**2)
+            g2d = peakValue * simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
+            
+        if self.verbose:
+            print('mavisLO.computeBias, peakValue',peakValue)
 
         g2d = intRebin(g2d, self.mediumShape) * self.downsample_factor**2
         I_k_data = peakValue * simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
         I_k_prime_data = peakValue * simple2Dgaussian( xGrid, yGrid, self.p_offset, 0, asigma)
         back = self.skyBackground_LO/self.SensorFrameRate_LO
         I_k_data = intRebin(I_k_data, self.mediumShape) * self.downsample_factor**2
         I_k_prime_data = intRebin(I_k_prime_data,self.mediumShape) * self.downsample_factor**2
@@ -511,75 +554,144 @@
 
         
     def computeNoiseResidual(self, fmin, fmax, freq_samples, varX, bias, alib):
         npoints = 99
         Cfloat = self.fCValue.evalf()
         psd_tip_wind, psd_tilt_wind = self.computeWindPSDs(fmin, fmax, freq_samples)
         psd_freq = np.asarray(np.linspace(fmin, fmax, freq_samples))
+        
+        if self.plot4debug:
+            fig, ax1 = plt.subplots(1,1)
+            im = ax1.plot(psd_freq,psd_tip_wind) 
+            im = ax1.plot(psd_freq,psd_tilt_wind) 
+            ax1.set_xscale('log')
+            ax1.set_yscale('log')
+            ax1.set_title('Turbulence PSD', color='black')
+            ax1.set_xlabel('frequency [Hz]')
+            ax1.set_ylabel('Power')
+        
         df = psd_freq[1]-psd_freq[0]
         Df = psd_freq[-1]-psd_freq[0]
         sigma2Noise =  varX / bias**2 * Cfloat / (Df / df)
         # must wait till this moment to substitute the noise level
         self.fTipS1 = subsParamsByName(self.fTipS_LO, {'phi^noise_Tip': sigma2Noise})
         self.fTiltS1 = subsParamsByName( self.fTiltS_LO, {'phi^noise_Tilt': sigma2Noise})    
         self.fTipS_lambda1 = lambdifyByName( self.fTipS1, ['g^Tip_0', 'f', 'phi^wind_Tip'], alib)
         self.fTiltS_lambda1 = lambdifyByName( self.fTiltS1, ['g^Tilt_0', 'f', 'phi^wind_Tilt'], alib)
+        if self.displayEquation:
+            print('computeNoiseResidual')
+            try:
+                display(self.fTipS1)
+            except:
+                print('    no self.fTipS1')
+            try:
+                display(self.fTiltS1)
+            except:
+                print('    no self.fTiltS1')
         if alib==gpulib and gpuEnabled:
             xp = cp
             psd_freq = cp.asarray(psd_freq)
             psd_tip_wind = cp.asarray(psd_tip_wind)
             psd_tilt_wind = cp.asarray(psd_tilt_wind)        
         else:
             xp = np
-        g0g = xp.asarray( xp.linspace(0.01, 0.99, npoints) )
+        if self.LoopGain_LO == 'optimize':
+            # add small values of gain to have a good optimization
+            # when the noise level is high.
+            g0 = (0.00000001,0.0000001,0.000001,0.00001,0.0001,0.001)
+            g0g = xp.concatenate((xp.asarray( g0),xp.linspace(0.01, 0.99, npoints)))
+        else:
+            # if gain is set no optimization is done and bias is not compensated
+            g0 = (bias*self.LoopGain_LO,bias*self.LoopGain_LO)
+            g0g = xp.asarray(g0)
+            
         e1 = psd_freq.reshape((1,psd_freq.shape[0]))
         e2 = psd_tip_wind.reshape((1,psd_tip_wind.shape[0]))
         e3 = psd_tilt_wind.reshape((1,psd_tilt_wind.shape[0]))
         e4 = g0g.reshape((g0g.shape[0], 1))
         psd_freq_ext, psd_tip_wind_ext, psd_tilt_wind_ext, g0g_ext = xp.broadcast_arrays(e1, e2, e3, e4)
+               
+        if self.plot4debug:
+            fig, ax2 = plt.subplots(1,1)
+            for x in range(g0g.shape[0]):
+                im = ax2.plot(psd_freq.get(),(self.fTipS_lambda1( g0g_ext, psd_freq_ext, psd_tip_wind_ext).get())[x,:]) 
+            ax2.set_xscale('log')
+            ax2.set_yscale('log')
+            ax2.set_title('residual PSD', color='black')
+            ax2.set_xlabel('frequency [Hz]')
+            ax2.set_ylabel('Power')
+        
         resultTip = xp.absolute((xp.sum(self.fTipS_lambda1( g0g_ext, psd_freq_ext, psd_tip_wind_ext), axis=(1)) ) )
         resultTilt = xp.absolute((xp.sum(self.fTiltS_lambda1( g0g_ext, psd_freq_ext, psd_tilt_wind_ext), axis=(1)) ) )
         minTipIdx = xp.where(resultTip == xp.amin(resultTip)) #    print(minTipIdx[0], resultTip[minTipIdx[0][0]])
         minTiltIdx = xp.where(resultTilt == xp.amin(resultTilt)) #    print(minTiltIdx[0], resultTilt[minTiltIdx[0][0]])
+        if self.verbose:
+            print('         best tip gain (noise)',g0g[minTipIdx[0][0]])
+            print('         best tilt gain (noise)',g0g[minTiltIdx[0][0]])
         if alib==gpulib and gpuEnabled:
             return cp.asnumpy(resultTip[minTipIdx[0][0]]), cp.asnumpy(resultTilt[minTiltIdx[0][0]])
         else:
             return (resultTip[minTipIdx[0][0]], resultTilt[minTiltIdx[0][0]])
 
         
     def computeWindResidual(self, psd_freq, psd_tip_wind0, psd_tilt_wind0, var1x, bias, alib):
         npoints = 99
         Cfloat = self.fCValue.evalf()
         df = psd_freq[1]-psd_freq[0]
         Df = psd_freq[-1]-psd_freq[0]
         psd_tip_wind = psd_tip_wind0 * df
         psd_tilt_wind = psd_tilt_wind0 * df
+        
+        if self.plot4debug:
+            fig, ax1 = plt.subplots(1,1)
+            im = ax1.plot(psd_freq,psd_tip_wind) 
+            im = ax1.plot(psd_freq,psd_tilt_wind) 
+            ax1.set_xscale('log')
+            ax1.set_yscale('log')
+            ax1.set_title('wind shake PSD', color='black')
+            ax1.set_xlabel('frequency [Hz]')
+            ax1.set_ylabel('Power')
+               
         sigma2Noise = var1x / bias**2 * Cfloat / (Df / df)
         self.fTipS1 = subsParamsByName(self.fTipS, {'phi^noise_Tip': sigma2Noise})
         self.fTiltS1 = subsParamsByName( self.fTiltS, {'phi^noise_Tilt': sigma2Noise})
         self.fTipS_lambda1 = lambdifyByName( self.fTipS1, ['g^Tip_0', 'g^Tip_1', 'f', 'phi^wind_Tip'], alib)
         self.fTiltS_lambda1 = lambdifyByName( self.fTiltS1, ['g^Tilt_0', 'g^Tilt_1', 'f', 'phi^wind_Tilt'], alib)
         if alib==gpulib and gpuEnabled:
             xp = cp
             psd_freq = cp.asarray(psd_freq)
             psd_tip_wind = cp.asarray(psd_tip_wind)
             psd_tilt_wind = cp.asarray(psd_tilt_wind)        
         else:
             xp = np
-        g0g, g1g = xp.meshgrid(xp.linspace(0.01,0.99,npoints), xp.linspace(0.01,0.99,npoints)) 
+        
+        if self.LoopGain_LO == 'optimize':
+            # add small values of gain to have a good optimization
+            # when the noise level is high.
+            g0 = (0.00000001,0.0000001,0.000001,0.00001,0.0001,0.001)
+            g0g = xp.concatenate((xp.asarray( g0),xp.linspace(0.01, 0.99, npoints)))
+        else:
+            # if gain is set no optimization is done and bias is not compensated
+            g0 = (bias*self.LoopGain_LO,bias*self.LoopGain_LO)
+            g0g = xp.asarray(g0)
+        g0g, g1g = xp.meshgrid( g0g,g0g )
+        
         e1 = psd_freq.reshape((1,1,psd_freq.shape[0]))
         e2 = psd_tip_wind.reshape((1,1,psd_tip_wind.shape[0]))
         e3 = psd_tilt_wind.reshape((1,1,psd_tilt_wind.shape[0]))
         e4 = g0g.reshape((g0g.shape[0],g0g.shape[1],1))
         e5 = g1g.reshape((g1g.shape[0],g1g.shape[1],1))
         psd_freq_ext, psd_tip_wind_ext, psd_tilt_wind_ext, g0g_ext, g1g_ext  = xp.broadcast_arrays(e1, e2, e3, e4, e5)
         resultTip = xp.absolute((xp.sum(self.fTipS_lambda1( g0g_ext, g1g_ext, psd_freq_ext, psd_tip_wind_ext), axis=(2)) ) )
         resultTilt = xp.absolute((xp.sum(self.fTiltS_lambda1( g0g_ext, g1g_ext, psd_freq_ext, psd_tilt_wind_ext), axis=(2)) ) )
         minTipIdx = xp.where(resultTip == xp.amin(resultTip))
         minTiltIdx = xp.where(resultTilt == xp.amin(resultTilt))
+        if self.verbose:
+            print('         best tip gain (wind)',g0g[minTipIdx[0][0],minTipIdx[1][0]])
+            print('         best tilt gain (wind)',g0g[minTiltIdx[0][0],minTiltIdx[1][0]])
         if alib==gpulib and gpuEnabled:
             return cp.asnumpy(resultTip[minTipIdx[0][0], minTipIdx[1][0]]), cp.asnumpy(resultTilt[minTiltIdx[0][0], minTiltIdx[1][0]])
         else:
             return (resultTip[minTipIdx[0][0], minTipIdx[1][0]], resultTilt[minTiltIdx[0][0], minTiltIdx[1][0]])
 
         
     def covValue(self, ii,jj, pp, hh):
@@ -696,37 +808,44 @@
     def computeTotalResidualMatrix(self, aCartPointingCoords, aCartNGSCoords, aNGS_flux, aNGS_SR_LO, aNGS_FWHM_mas):
         nPointings = aCartPointingCoords.shape[0]
         maxFluxIndex = np.where(aNGS_flux==np.amax(aNGS_flux))
         nNaturalGS = aCartNGSCoords.shape[0]
         C1 = np.zeros((2,2))
         Cnn = np.zeros((2*nNaturalGS,2*nNaturalGS))
 
-
         if self.verbose:
             print('mavisLO.computeTotalResidualMatrix')
-            print('             aNGS_flux',aNGS_flux)
-            print('             self.N_sa_tot_LO',self.N_sa_tot_LO)
+            print('         aNGS_flux',aNGS_flux)
+            print('         self.N_sa_tot_LO',self.N_sa_tot_LO)
+            
         for starIndex in range(nNaturalGS):
             bias, amu, avar = self.computeBias(aNGS_flux[starIndex], aNGS_SR_LO[starIndex], aNGS_FWHM_mas[starIndex]) # one scalar, two tuples of 2
             if self.verbose:
-                print('             bias',bias)
-                print('             amu',amu)
-                print('             avar',avar)
+                print('         bias',bias)
+                print('         amu',amu)
+                print('         avar',avar)
 
             var1x = avar[0] * self.PixelScale_LO**2
             nr = self.computeNoiseResidual(0.25, 250.0, 1000, var1x, bias, self.platformlib )
+            # TODO: this second computation must be embedded in the previous one.
             wr = self.computeWindResidual(self.psd_freq, self.psd_tip_wind, self.psd_tilt_wind, var1x, bias, self.platformlib )
+            if self.verbose:
+                print('         noise residual:     ',nr)
+                print('         wind-shake residual:',wr)
             Cnn[2*starIndex,2*starIndex] = nr[0]
             Cnn[2*starIndex+1,2*starIndex+1] = nr[1]
             if starIndex == maxFluxIndex[0][0]:
                 C1[0,0] = wr[0]
                 C1[1,1] = wr[1]
 
         # C1 and Cnn do not depend on aCartPointingCoords[i]
         Ctot = self.multiCMatAssemble(aCartPointingCoords, aCartNGSCoords, Cnn, C1)
+        if self.verbose:
+            print('         Ctot:')
+            print(Ctot)
         return Ctot.reshape((nPointings,2,2))
 
 
     def ellipsesFromCovMats(self, Ctot):
         theta = sp.symbols('theta')
         sigma_1 = sp.symbols('sigma^2_1')
         sigma_2 = sp.symbols('sigma^2_2')
```

### Comparing `mastsel-0.1/mastsel/mavisParams.py` & `mastsel-1.1/mastsel/mavisParams.py`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/mastsel/mavisParamsOld.py` & `mastsel-1.1/mastsel/mavisParamsOld.py`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/mastsel/mavisPsf.py` & `mastsel-1.1/mastsel/mavisPsf.py`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/mastsel/mavisUtilities.py` & `mastsel-1.1/mastsel/mavisUtilities.py`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/mastsel.egg-info/PKG-INFO` & `mastsel-1.1/mastsel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastsel
-Version: 0.1
+Version: 1.1
 Summary: Asterism Selection for MAVIS instrument
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/MASTSEL
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
```

### Comparing `mastsel-0.1/mastsel.egg-info/SOURCES.txt` & `mastsel-1.1/mastsel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/notebooks/MAVIS-CONVOLUTION-TEST.ipynb` & `mastsel-1.1/notebooks/MAVIS-CONVOLUTION-TEST.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/notebooks/MAVIS-CONVOLUTION.ipynb` & `mastsel-1.1/notebooks/MAVIS-CONVOLUTION.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/notebooks/MAVIS.ipynb` & `mastsel-1.1/notebooks/MAVIS.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/notebooks/MAVIS2.ipynb` & `mastsel-1.1/notebooks/MAVIS2.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/notebooks/MAVIS3.ipynb` & `mastsel-1.1/notebooks/MAVIS3.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/notebooks/MAVIS_INT_REC.ipynb` & `mastsel-1.1/notebooks/MAVIS_INT_REC.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/notebooks/MAVIS_MAIN.ipynb` & `mastsel-1.1/notebooks/MAVIS_MAIN.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/pyproject.toml` & `mastsel-1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mastsel-0.1/tests/allTests.py` & `mastsel-1.1/tests/allTests.py`

 * *Files identical despite different names*

