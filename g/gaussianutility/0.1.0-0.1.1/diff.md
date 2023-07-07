# Comparing `tmp/gaussianutility-0.1.0.tar.gz` & `tmp/gaussianutility-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussianutility-0.1.0.tar", last modified: Fri Jun 30 20:26:49 2023, max compression
+gzip compressed data, was "gaussianutility-0.1.1.tar", last modified: Fri Jul  7 17:26:50 2023, max compression
```

## Comparing `gaussianutility-0.1.0.tar` & `gaussianutility-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,41 @@
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-06-30 20:26:49.482905 gaussianutility-0.1.0/
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1799 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/.gitignore
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1068 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/LICENSE
--rw-r--r--   0 sungil    (1000) sungil    (1000)      486 2023-06-30 20:26:49.482905 gaussianutility-0.1.0/PKG-INFO
--rw-r--r--   0 sungil    (1000) sungil    (1000)       17 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/README.md
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-06-30 20:26:49.462907 gaussianutility-0.1.0/gaussianutility/
--rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/gaussianutility/__init__.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2595 2023-06-28 20:50:29.000000 gaussianutility-0.1.0/gaussianutility/com2vasp.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1202 2023-06-28 20:49:34.000000 gaussianutility-0.1.0/gaussianutility/com2xyz.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2194 2023-06-28 21:08:12.000000 gaussianutility-0.1.0/gaussianutility/freezeLayer.py
--rwxr-xr-x   0 sungil    (1000) sungil    (1000)     6042 2023-06-28 21:02:43.000000 gaussianutility-0.1.0/gaussianutility/gibbsTemp.py
--rwxr-xr-x   0 sungil    (1000) sungil    (1000)     1494 2023-06-28 20:56:01.000000 gaussianutility-0.1.0/gaussianutility/out2com.py
--rwxr-xr-x   0 sungil    (1000) sungil    (1000)     1578 2023-06-28 20:56:05.000000 gaussianutility-0.1.0/gaussianutility/out2xyz.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2146 2023-06-28 20:39:44.000000 gaussianutility-0.1.0/gaussianutility/printE.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     7563 2023-06-28 20:33:50.000000 gaussianutility-0.1.0/gaussianutility/sortInput.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)    10666 2023-06-28 21:15:40.000000 gaussianutility-0.1.0/gaussianutility/spectrum.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     9331 2023-06-28 19:07:39.000000 gaussianutility-0.1.0/gaussianutility/utilities.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2794 2023-06-28 20:36:17.000000 gaussianutility-0.1.0/gaussianutility/vasp2com.py
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-06-30 20:26:49.462907 gaussianutility-0.1.0/gaussianutility.egg-info/
--rw-r--r--   0 sungil    (1000) sungil    (1000)      486 2023-06-30 20:26:49.000000 gaussianutility-0.1.0/gaussianutility.egg-info/PKG-INFO
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1338 2023-06-30 20:26:49.000000 gaussianutility-0.1.0/gaussianutility.egg-info/SOURCES.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2023-06-30 20:26:49.000000 gaussianutility-0.1.0/gaussianutility.egg-info/dependency_links.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)      428 2023-06-30 20:26:49.000000 gaussianutility-0.1.0/gaussianutility.egg-info/entry_points.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)      103 2023-06-30 20:26:49.000000 gaussianutility-0.1.0/gaussianutility.egg-info/requires.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)       16 2023-06-30 20:26:49.000000 gaussianutility-0.1.0/gaussianutility.egg-info/top_level.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)      472 2023-06-30 20:26:43.000000 gaussianutility-0.1.0/pyproject.toml
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-06-30 20:26:49.462907 gaussianutility-0.1.0/recyclebin/
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2872 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/com2vasp.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1460 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/command.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     4400 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/extract_geom.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)      799 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/freezeLayer.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)      482 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/freezeLow.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2487 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/freeze_low.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)      742 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/genFeat.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)      585 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/inputSort.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     5148 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/old_xgeom.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)      864 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/pathFeature.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1952 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/path_feature.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     4332 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/removed_from_utils.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)    11512 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/utils.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)      962 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/recyclebin/xgeom.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)       38 2023-06-30 20:26:49.482905 gaussianutility-0.1.0/setup.cfg
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1622 2023-06-30 20:18:42.000000 gaussianutility-0.1.0/setup.py
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-06-30 20:26:49.472906 gaussianutility-0.1.0/test/
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1187 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/3trimerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  2499899 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/3trimerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1596 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/4tetramerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  6317153 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/4tetramerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1929 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/5pentamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)   702306 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/5pentamerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2335 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/6hexamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  4029103 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/6hexamerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2676 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/7heptamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  4193531 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/7heptamerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     3082 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/8octamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000) 10170069 2023-06-28 19:04:07.000000 gaussianutility-0.1.0/test/8octamerPrism.SiAl.out
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-07 17:26:50.662551 gaussianutility-0.1.1/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1799 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/.gitignore
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1068 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/LICENSE
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     5038 2023-07-07 17:26:50.652551 gaussianutility-0.1.1/PKG-INFO
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     4570 2023-07-07 16:22:21.000000 gaussianutility-0.1.1/README.md
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-07 17:26:50.632552 gaussianutility-0.1.1/gaussianutility/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/gaussianutility/__init__.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2595 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/com2vasp.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1202 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/com2xyz.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2194 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/freezeLayer.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     6161 2023-07-03 20:31:32.000000 gaussianutility-0.1.1/gaussianutility/gibbsTemp.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1494 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/out2com.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1578 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/out2xyz.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2146 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/printE.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     7563 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/sortInput.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)    10666 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/spectrum.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     9331 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/utilities.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2794 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/vasp2com.py
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-07 17:26:50.642552 gaussianutility-0.1.1/gaussianutility.egg-info/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     5038 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/PKG-INFO
+-rw-r--r--   0 sungil    (1000) sungil    (1000)      995 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/SOURCES.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/dependency_links.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)      428 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/entry_points.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)      103 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/requires.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)       16 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/top_level.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)      472 2023-07-07 17:22:57.000000 gaussianutility-0.1.1/pyproject.toml
+-rw-r--r--   0 sungil    (1000) sungil    (1000)       38 2023-07-07 17:26:50.662551 gaussianutility-0.1.1/setup.cfg
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1622 2023-07-07 17:22:57.000000 gaussianutility-0.1.1/setup.py
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-07 17:26:50.652551 gaussianutility-0.1.1/test/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1187 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/3trimerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  2499899 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/3trimerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1596 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/4tetramerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  6317153 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/4tetramerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1929 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/5pentamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)   702306 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/5pentamerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2335 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/6hexamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  4029103 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/6hexamerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2676 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/7heptamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  4193531 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/7heptamerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     3082 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/8octamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000) 10170069 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/8octamerPrism.SiAl.out
```

### Comparing `gaussianutility-0.1.0/.gitignore` & `gaussianutility-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/LICENSE` & `gaussianutility-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility/com2vasp.py` & `gaussianutility-0.1.1/gaussianutility/com2vasp.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility/com2xyz.py` & `gaussianutility-0.1.1/gaussianutility/com2xyz.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility/freezeLayer.py` & `gaussianutility-0.1.1/gaussianutility/freezeLayer.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility/gibbsTemp.py` & `gaussianutility-0.1.1/gaussianutility/gibbsTemp.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,48 +9,52 @@
 h = 6.62607015e-34 # Js
 Rgas = 8.3144626 # J/mol/K
 Na = 6.02214076e23
 
 # Calculate contributions from translational, rotational, vibrational, and eletronic motions
 # The equations are sourced from "Thermochemistry in Gaussian" written by Joseph W. Ochterski (2000)
 # https://gaussian.com/wp-content/uploads/dl/thermo.pdf
-
-# Function to calculate all conbtibutions
-def Contributions(temp,mass,press,vibTemp,multiplicity): # temp is a single float value
+def Contributions(temp, mass, press, vibTemp, multiplicity, rho_r, theta_r):
     ## Translational part
     qt = m.pow(2*m.pi*mass*kB*temp/h**2, 3/2) * kB*temp/press
     St = Rgas*(m.log(qt)+1+3/2)
     Et = 3/2*Rgas*temp
 
     ## Rotational part
-    Sr, Er = 0, 0
-    if 'rho_r' in globals():
-        if 'theta_rx' in globals():    
-            qr = m.pi**(1/2)/rho_r*m.sqrt((temp**3/(theta_rx*theta_ry*theta_rz)))
-        else: qr = m.pi**(1/2)/rho_r*m.sqrt((temp/(theta_r)))
-        Sr += Rgas*(m.log(qr)+3/2)
+    if len(theta_r) > 1:    
+        qr = m.pi**(1/2)/rho_r*m.sqrt((temp**3/np.prod(theta_r)))
+    elif len(theta_r) == 1:
+        qr = m.pi**(1/2)/rho_r*m.sqrt((temp/(theta_r[0])))
+        
+    if 'qr' in locals():
+        Sr = Rgas*(m.log(qr)+3/2)
         Er = 3/2*Rgas*temp
+    else:
+        Sr = 0
+        Er = 0
 
     ## Vibrational part
     summ1 = 0 # for entropy contribution
     summ2 = 0 # for energy contribution
+
     for val in vibTemp:
         summ1 += val/temp/(m.exp(val/temp) - 1) - m.log(1-m.exp(-val/temp))
         summ2 += val*(1/2 + 1/(m.exp(val/temp)-1))
+
     Sv, Ev = Rgas*np.array([summ1, summ2])
 
     ## Electronic part
     Se = Rgas * m.log(multiplicity)
     Ee = 0
     
     Stot = St + Sr + Sv + Se
     Etot = Et + Er + Ev + Ee
     
     return Stot, Etot # return total entropy correction and energy correction
-
+    
 def main():
     # Print error/help messages that looks like argparse functionality
     if len(sys.argv) == 1:
         print("usage: gibbsTemp [-h] file_name temp1 [temp2 [step_number]]")
         print("gibbsTemp: error: the following arguments are required: file_name temp1")
         sys.exit()
 
@@ -96,19 +100,23 @@
         if idx >= beginIdx-1 and idx < endIdx-3:
             thermochem.append(line)
 
     # Extract required informations from the thermochemistry output
     for idx, line in enumerate(thermochem):
         if "Pressure" in line:
             press = float(line.split()[4])*101325 # Pa
-        if "Molecular mass" in line: mass = float(line.split()[2])*1.6605391e-27 # kg
-        if "Rotational symmetry number" in line: rho_r = float(line.split()[3]) 
-        if "Rotational temperature" in line: 
-            if len(line.split()) < 5: theta_r = float(line.split()[3])         
-            else: theta_rx, theta_ry, theta_rz = np.float64(np.array(line.split()[3:6]))
+        if "Molecular mass" in line:
+            mass = float(line.split()[2])*1.6605391e-27 # kg
+        if "Rotational symmetry number" in line:\
+            rho_r = float(line.split()[3]) 
+        if "Rotational temperatures" in line: 
+            if len(line.split()) < 5: 
+                theta_r = np.array([float(line.split()[3])])
+            else:
+                theta_r = np.float64(np.array(line.split()[3:6]))
         if "Vibrational temperature" in line:
             vibTempBeginIdx = idx
         if "Zero-point correction" in line: 
             zpCorr = float(line.split()[2])*2625.4996394799e3 # J/mol
             vibTempEndIdx = idx
         if "Sum of electronic and zero-point Energies" in line:
             ElectE = float(line.split()[6])*2625.4996394799e3 - zpCorr # J/mol
@@ -119,26 +127,31 @@
             try: vibTemp.append(float(elem))
             except: ValueError
     vibTemp = np.array(vibTemp)
 
     # Arrays of entropy and energy corrections in the given temperature (range)
     StotArr=[]
     EtotArr=[]
+    
+    if 'rho_r' not in locals():
+        rho_r = []
+        theta_r = []
 
     for temp in temperature:
-        Stot, Etot = Contributions(temp,mass,press,vibTemp,multiplicity)
+        Stot, Etot = Contributions(temp, mass, press, vibTemp, multiplicity, rho_r, theta_r)
         StotArr.append(Stot)
         EtotArr.append(Etot)
 
     StotArr = np.array(StotArr)
     EtotArr = np.array(EtotArr)
-
+    
     Hcorr = EtotArr + kB*temperature*Na # Thermal corrections to Enthalpy
     Gcorr = Hcorr - temperature * StotArr # Thermal corrections to Free energy
     Gibbs = (ElectE + Gcorr) / 2625.4996394799e3 # Final Gibbs free energy in Hartree
 
     temperature = np.ndarray.tolist(np.round(temperature,decimals=6))
     Gibbs = np.ndarray.tolist(np.round(Gibbs,decimals=6))
 
     print("Temperature [K]: " + str(temperature).strip('[]'))
     print("Gibbs free energy [Hartree]: " + str(Gibbs).strip('[]'))
 
+
```

### Comparing `gaussianutility-0.1.0/gaussianutility/out2com.py` & `gaussianutility-0.1.1/gaussianutility/out2com.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility/out2xyz.py` & `gaussianutility-0.1.1/gaussianutility/out2xyz.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility/printE.py` & `gaussianutility-0.1.1/gaussianutility/printE.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility/sortInput.py` & `gaussianutility-0.1.1/gaussianutility/sortInput.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility/spectrum.py` & `gaussianutility-0.1.1/gaussianutility/spectrum.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility/utilities.py` & `gaussianutility-0.1.1/gaussianutility/utilities.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility/vasp2com.py` & `gaussianutility-0.1.1/gaussianutility/vasp2com.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/gaussianutility.egg-info/SOURCES.txt` & `gaussianutility-0.1.1/gaussianutility.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -17,28 +17,14 @@
 gaussianutility/vasp2com.py
 gaussianutility.egg-info/PKG-INFO
 gaussianutility.egg-info/SOURCES.txt
 gaussianutility.egg-info/dependency_links.txt
 gaussianutility.egg-info/entry_points.txt
 gaussianutility.egg-info/requires.txt
 gaussianutility.egg-info/top_level.txt
-recyclebin/com2vasp.py
-recyclebin/command.py
-recyclebin/extract_geom.py
-recyclebin/freezeLayer.py
-recyclebin/freezeLow.py
-recyclebin/freeze_low.py
-recyclebin/genFeat.py
-recyclebin/inputSort.py
-recyclebin/old_xgeom.py
-recyclebin/pathFeature.py
-recyclebin/path_feature.py
-recyclebin/removed_from_utils.py
-recyclebin/utils.py
-recyclebin/xgeom.py
 test/3trimerPrism.SiAl.geom.com
 test/3trimerPrism.SiAl.out
 test/4tetramerPrism.SiAl.geom.com
 test/4tetramerPrism.SiAl.out
 test/5pentamerPrism.SiAl.geom.com
 test/5pentamerPrism.SiAl.out
 test/6hexamerPrism.SiAl.geom.com
```

### Comparing `gaussianutility-0.1.0/setup.py` & `gaussianutility-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gaussianutility",
-    version="0.1.0",
+    version="0.1.1",
     author="Sungil Hong",
     author_email="suh33@pitt.edu",
     description="Useful utilities to use Gaussian09/16 software",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={'console_scripts': [
                   'com2vasp = gaussianutility.com2vasp:main',
@@ -27,14 +27,14 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"],
     python_requires='>=3.6',
     install_requires=['numpy>=1.17.2',
-                      'pandas>=1.3.0',
+                      'pandas>=1.1.0',
                       'periodictable>=1.6.1',
                       'ase',
                       'argparse>=1.1',
                       'matplotlib>=3.5.3',
                       'mendeleev>=0.12.0']
 )
```

### Comparing `gaussianutility-0.1.0/test/3trimerPrism.SiAl.geom.com` & `gaussianutility-0.1.1/test/3trimerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/3trimerPrism.SiAl.out` & `gaussianutility-0.1.1/test/3trimerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/4tetramerPrism.SiAl.geom.com` & `gaussianutility-0.1.1/test/4tetramerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/4tetramerPrism.SiAl.out` & `gaussianutility-0.1.1/test/4tetramerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/5pentamerPrism.SiAl.geom.com` & `gaussianutility-0.1.1/test/5pentamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/5pentamerPrism.SiAl.out` & `gaussianutility-0.1.1/test/5pentamerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/6hexamerPrism.SiAl.geom.com` & `gaussianutility-0.1.1/test/6hexamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/6hexamerPrism.SiAl.out` & `gaussianutility-0.1.1/test/6hexamerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/7heptamerPrism.SiAl.geom.com` & `gaussianutility-0.1.1/test/7heptamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/7heptamerPrism.SiAl.out` & `gaussianutility-0.1.1/test/7heptamerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/8octamerPrism.SiAl.geom.com` & `gaussianutility-0.1.1/test/8octamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.0/test/8octamerPrism.SiAl.out` & `gaussianutility-0.1.1/test/8octamerPrism.SiAl.out`

 * *Files identical despite different names*

