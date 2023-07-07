# Comparing `tmp/covdrugsim-0.2.0.tar.gz` & `tmp/covdrugsim-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covdrugsim-0.2.0.tar", max compression
+gzip compressed data, was "covdrugsim-0.3.0.tar", max compression
```

## Comparing `covdrugsim-0.2.0.tar` & `covdrugsim-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1082 2023-07-05 09:33:37.229976 covdrugsim-0.2.0/LICENSE
--rw-r--r--   0        0        0     6643 2023-07-05 09:33:37.229976 covdrugsim-0.2.0/README.md
--rw-r--r--   0        0        0     1956 2023-07-05 09:34:16.390584 covdrugsim-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      733 2023-07-05 09:34:16.390584 covdrugsim-0.2.0/setup.py
--rw-r--r--   0        0        0     1058 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/data/__init__.py
--rw-r--r--   0        0        0      170 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/data/chargesExample.txt
--rw-r--r--   0        0        0     4449 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/data/energyLevellerExample.inp
--rw-r--r--   0        0        0      474 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/datasets.py
--rw-r--r--   0        0        0      241 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/main.py
--rw-r--r--   0        0        0     3839 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/SCbondDist.py
--rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/__init__.py
--rw-r--r--   0        0        0     8141 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/baseID.py
--rw-r--r--   0        0        0     6071 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/bbRMSD.py
--rw-r--r--   0        0        0      331 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/config.py
--rw-r--r--   0        0        0     3084 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/hbondAnalysis.py
--rw-r--r--   0        0        0     3917 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/ligDihedral.py
--rw-r--r--   0        0        0      769 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/mdAnalyse.py
--rw-r--r--   0        0        0     5644 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/prepMTB.py
--rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/admin.py
--rw-r--r--   0        0        0     1377 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/gsub.sh
--rw-r--r--   0        0        0     4421 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/prepGaussian.py
--rw-r--r--   0        0        0     1325 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/settings.py
--rw-r--r--   0        0        0     4914 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/tabulate.py
--rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/unitConv/__init__.py
--rw-r--r--   0        0        0     4241 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/unitConv/unitConv.py
--rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/__init__.py
--rw-r--r--   0        0        0    17951 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
--rw-r--r--   0        0        0    11782 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
--rw-r--r--   0        0        0    13749 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
--rw-r--r--   0        0        0     1134 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/tests/test_covdrugsim.py
--rw-r--r--   0        0        0     7780 1970-01-01 00:00:00.000000 covdrugsim-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-07 07:09:55.192971 covdrugsim-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6643 2023-07-07 07:09:55.192971 covdrugsim-0.3.0/README.md
+-rw-r--r--   0        0        0     1956 2023-07-07 07:10:34.870719 covdrugsim-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      733 2023-07-07 07:10:34.870719 covdrugsim-0.3.0/setup.py
+-rw-r--r--   0        0        0     1410 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/chargesExample.txt
+-rw-r--r--   0        0        0     4449 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/energyLevellerExample.inp
+-rw-r--r--   0        0        0      619 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/exampleXYZs/but2eneE/but2eneE.xyz
+-rw-r--r--   0        0        0      621 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/exampleXYZs/but2eneEd/but2eneEd.xyz
+-rw-r--r--   0        0        0      619 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/exampleXYZs/but2eneZ/but2eneZ.xyz
+-rw-r--r--   0        0        0      866 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/datasets.py
+-rw-r--r--   0        0        0      241 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/main.py
+-rw-r--r--   0        0        0     3839 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/SCbondDist.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/__init__.py
+-rw-r--r--   0        0        0     8141 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/baseID.py
+-rw-r--r--   0        0        0     6071 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/bbRMSD.py
+-rw-r--r--   0        0        0      331 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/config.py
+-rw-r--r--   0        0        0     3084 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/hbondAnalysis.py
+-rw-r--r--   0        0        0     3917 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/ligDihedral.py
+-rw-r--r--   0        0        0      769 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/mdAnalyse.py
+-rw-r--r--   0        0        0     5644 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/prepMTB.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/__init__.py
+-rw-r--r--   0        0        0     1708 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/admin.py
+-rw-r--r--   0        0        0     1324 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/constants.py
+-rw-r--r--   0        0        0     9228 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/genScripts.py
+-rw-r--r--   0        0        0     1605 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/gsub.sh
+-rw-r--r--   0        0        0     4844 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/tabulate.py
+-rw-r--r--   0        0        0     4270 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/unitConv.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/__init__.py
+-rw-r--r--   0        0        0    17951 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
+-rw-r--r--   0        0        0    11782 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
+-rw-r--r--   0        0        0    13749 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
+-rw-r--r--   0        0        0     4017 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/tests/test_covdrugsim.py
+-rw-r--r--   0        0        0     7780 1970-01-01 00:00:00.000000 covdrugsim-0.3.0/PKG-INFO
```

### Comparing `covdrugsim-0.2.0/LICENSE` & `covdrugsim-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/README.md` & `covdrugsim-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/pyproject.toml` & `covdrugsim-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "covdrugsim"
-version = "0.2.0"
+version = "0.3.0"
 description = "Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/covdrugsim"
 repository = "https://github.com/Jon-Ting/covdrugsim"
 documentation = "https://covdrugsim.readthedocs.io/en/latest/"
```

### Comparing `covdrugsim-0.2.0/setup.py` & `covdrugsim-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="covdrugsim",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `covdrugsim-0.2.0/src/covdrugsim/__init__.py` & `covdrugsim-0.3.0/src/covdrugsim/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
   >>> x = 42
   >>> x = x + 1
 
 Use the built-in ``help`` function to view a function's docstring::
 
   >>> import covdrugsim
-  >>> help(covdrugsim.qmcalc.unitConv.unitConv)
+  >>> help(covdrugsim.qmcalc.genScripts)
   ... # docstring: +SKIP
 
 Utilities
 ---------
 test (To be implemented)
     Run CovDrugSim tests.
 __version__
@@ -31,9 +31,15 @@
 """
 # Read version from installed package
 from importlib.metadata import version
 __version__ = version('covdrugsim')
 
 # Populate package namespace
 __all__ = ['mdsim', 'qmcalc']
+from covdrugsim.datasets import genExampleXYZs, getExampleEnergyLevellerInputPath, getExampleChargePath
+from covdrugsim.qmcalc.constants import keywordDict
+from covdrugsim.qmcalc.genScripts import genAllScripts
+from covdrugsim.qmcalc.admin import groupFilesIntoDir
+from covdrugsim.qmcalc.tabulate import writeToExcel
+from covdrugsim.qmcalc.unitConv import energyUnitsConversion, eyringEquation, timeUnitsConversion
+
 from covdrugsim.mdsim import mdAnalyse
-from covdrugsim.qmcalc.unitConv.unitConv import exp_time
```

### Comparing `covdrugsim-0.2.0/src/covdrugsim/data/energyLevellerExample.inp` & `covdrugsim-0.3.0/src/covdrugsim/data/energyLevellerExample.inp`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/src/covdrugsim/mdsim/SCbondDist.py` & `covdrugsim-0.3.0/src/covdrugsim/mdsim/SCbondDist.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/src/covdrugsim/mdsim/baseID.py` & `covdrugsim-0.3.0/src/covdrugsim/mdsim/baseID.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/src/covdrugsim/mdsim/bbRMSD.py` & `covdrugsim-0.3.0/src/covdrugsim/mdsim/bbRMSD.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/src/covdrugsim/mdsim/hbondAnalysis.py` & `covdrugsim-0.3.0/src/covdrugsim/mdsim/hbondAnalysis.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/src/covdrugsim/mdsim/ligDihedral.py` & `covdrugsim-0.3.0/src/covdrugsim/mdsim/ligDihedral.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/src/covdrugsim/mdsim/mdAnalyse.py` & `covdrugsim-0.3.0/src/covdrugsim/mdsim/mdAnalyse.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/src/covdrugsim/mdsim/prepMTB.py` & `covdrugsim-0.3.0/src/covdrugsim/mdsim/prepMTB.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/settings.py` & `covdrugsim-0.3.0/src/covdrugsim/qmcalc/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-keyword_dict = {
+keywordDict = {
     'GOVF': {'type': ' opt int(grid=ultrafine) scf=tight', 'freq': ' freq=noraman', 'mem': int(8000), 'jobfs': int(2400), 'time': '10:00:00'},  # geometry optimization with vibrational frequency calculation
     'TSGOVF': {'type': ' opt=(ts,calcfc,noeigentest,maxcyc=200) int(grid=ultrafine) scf=tight', 'freq': ' freq=noraman', 'mem': int(4000), 'jobfs': int(4000), 'time': '10:00:00'},  # transition state GOVF
 
     'SPEXGO': {'type': '', 'time': '48:00:00', 'vmem': int(10000), 'ncpus': int(16)},  # single-point energy calculation without geometry optimization
     'IRC': {'type': ' irc=(maxpoints=6,stepsize=10,calcfc,maxcyc=200)', 'time': '10:00:00'},  # intrinsic reaction coordinate calculation
     'SPEiS': {'type': ' int(grid=ultrafine) scf=tight', 'freq': '', 'time': '07:00:00', 'mem': int(70000), 'jobfs': int(100000)},  # single-point energy calculation in solvent
     'MO': {'type': ' gfinput iop(6/7=3)', 'time': '10:00:00'},  # print molecular orbitals for Molden display
```

### Comparing `covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/tabulate.py` & `covdrugsim-0.3.0/src/covdrugsim/qmcalc/tabulate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import os
+from os import listdir
 from os.path import isdir
 import re
 
 import pandas as pd
 
 
-def sortHuman(list):
-    """Sort a given list in a more "human" way"""
+def sortHuman(alist):
+    """Sort a given alist in a more 'human' way"""
     convert = lambda text: float(text) if text.isdigit() else text
     alphanum = lambda key: [convert(c) for c in re.split('([-+]?[0-9]*\.?[0-9]*)', key)]
-    list.sort(key=alphanum)
-    return list
+    alist.sort(key=alphanum)
+    return alist
 
 
-def replaceMultiple(main_str, toBeReplaced, new_str):
-    """Replace multiple strings of main_str"""
+def replaceMultiple(mainStr, toBeReplaced, newStr):
+    """Replace multiple strings of mainStr"""
     for elem in toBeReplaced:
-        if elem in main_str:
-            main_str = main_str.replace(elem, new_str)
-    return main_str
+        if elem in mainStr:
+            mainStr = mainStr.replace(elem, newStr)
+    return mainStr
 
 
-def findVal(line_list, target_str):
+def findVal(lineList, targetStr):
     """Find the values of interest from Gaussian output files"""
-    val, isEnergy, isMethod = None, 'Energies' in target_str[0] or 'Enthalpies' in target_str[0], '%chk' in target_str[0]
-    for i, string in enumerate(target_str):
-        for j, line in enumerate(line_list):
+    val, isEnergy, isMethod = None, 'Energies' in targetStr[0] or 'Enthalpies' in targetStr[0], '%chk' in targetStr[0]
+    for i, string in enumerate(targetStr):
+        for j, line in enumerate(lineList):
             if string in line:
                 if isMethod:
-                    value_inc = line_list[j - 2]
-                    val = value_inc.split(' ')[2]; break
+                    valueInc = lineList[j - 2]
+                    val = valueInc.split(' ')[2]; break
                 else:
-                    value_inc = line.split(string)[-1].strip()
+                    valueInc = line.split(string)[-1].strip()
                     if isEnergy:
-                        val = float(value_inc.split('=')[-1].strip().replace(' ', '')); break
+                        val = float(valueInc.split('=')[-1].strip().replace(' ', '')); break
                     else:
-                        if '\\' in value_inc:
-                            val = value_inc.split('\\')[0].split('=')[-1]
+                        if '\\' in valueInc:
+                            val = valueInc.split('\\')[0].split('=')[-1]
                         else:
-                            val = value_inc + line_list[j - 1].split('\\')[0]
+                            val = valueInc + lineList[j - 1].split('\\')[0]
                             val = val.split('=')[-1]
                         try:
                             val = val.replace(' ', '')
                             float(val); break
                         except ValueError:
                             continue
     if val is None:
-        raise Exception('Target string {0} not found!'.format(target_str))
-    # print(target_str, val, line_list[-3])  # For debugging
+        raise Exception('Target string {0} not found!'.format(targetStr))
+    # print(targetStr, val, lineList[-3])  # For debugging
     return val
 
 
-def write_Excel(dir_path):
+def writeToExcel(dir_path):
     """Write a new Excel file tabulating the quantities of interest"""
-    method_list, title_list, molecule_list, conformer_list, NImag_list, Z_list, E_list, H_list, G_list, MP2_list = [], [], [], [], [], [], [], [], [], []
-    var_fill_list = [method_list, NImag_list, Z_list, E_list, H_list, G_list]
-    keyword_list = [['%chk'], ['NI', 'Im'], ['zero-point Energies'], ['HF'], ['thermal Enthalpies'], ['thermal Free Energies']]
+    methodList, titleList, moleculeList, conformerList, NImagList, ZList, EList, HList, GList, MP2List = [], [], [], [], [], [], [], [], [], []
+    varFillList = [methodList, NImagList, ZList, EList, HList, GList]
+    keywordList = [['%chk'], ['NI', 'Im'], ['zero-point Energies'], ['HF'], ['thermal Enthalpies'], ['thermal Free Energies']]
     for j, title in enumerate(groups):
-        conformer_dir = '{0}/{1}'.format(input_dir, title)
+        conformerDir = '{0}/{1}'.format(inputDir, title)
         print("Conformer:", title)
         try:
-            with open('{0}/{1}.out'.format(conformer_dir, title), 'r') as f:
-                line_list = f.readlines()
-                line_list.reverse()
-                for i, var_list in enumerate(var_fill_list):
-                    val = findVal(line_list, keyword_list[i])
-                    var_list.append(val)
-                title_list.append(title)
-                molecule_list.append(replace_multiple(title.split('c')[0].replace('_', ''), ['TR', 'TSS', 'TP'], ''))
-                conformer_list.append('c' + title.split('c')[-1])
+            with open('{0}/{1}.out'.format(conformerDir, title), 'r') as f:
+                lineList = f.readlines()
+                lineList.reverse()
+                for i, varList in enumerate(varFillList):
+                    val = findVal(lineList, keywordList[i])
+                    varList.append(val)
+                titleList.append(title)
+                moleculeList.append(replace_multiple(title.split('c')[0].replace('_', ''), ['TR', 'TSS', 'TP'], ''))
+                conformerList.append('c' + title.split('c')[-1])
         except FileNotFoundError:
-            print("{0}/{1}.out not found!".format(conformer_dir, title))
+            print("{0}/{1}.out not found!".format(conformerDir, title))
             continue
-    data = {'Method': method_list, 'Title': title_list, 'Molecule': molecule_list, 'Conformer': conformer_list, 'NImag': NImag_list,
-           'Z (Hartree)': Z_list, 'E (Hartree)': E_list, 'H (Hartree)': H_list, 'G (Hartree)': G_list}
+    data = {'Method': methodList, 'Title': titleList, 'Molecule': moleculeList, 'Conformer': conformerList, 'NImag': NImagList,
+           'Z (Hartree)': ZList, 'E (Hartree)': EList, 'H (Hartree)': HList, 'G (Hartree)': GList}
     df = pd.DataFrame(data, columns=['Method', 'Title', 'Molecule', 'Conformer', 'NImag', 'Z (Hartree)', 'E (Hartree)', 'H (Hartree)', 'G (Hartree)'])
-    title_list = sortHuman(title_list)
-    sorted_df = df.set_index('Title').reindex(title_list).reset_index()
-    print("# Sorted data frame:\n", sorted_df)
+    titleList = sortHuman(titleList)
+    sortedDF = df.set_index('Title').reindex(titleList).reset_index()
+    print("# Sorted data frame:\n", sortedDF)
 
     print("# Writing to Excel sheet...")
-    # sorted_df.to_excel('{0}/Energies.xlsx'.format(input_dir), sheet_name='Sheet1')
-    writer = pd.ExcelWriter('{0}/Energies.xlsx'.format(input_dir), engine='xlsxwriter')
-    sorted_df.to_excel(writer, startrow=1, sheet_name='Sheet1', index=False)
+    # sortedDF.to_excel('{0}/Energies.xlsx'.format(inputDir), sheet_name='Sheet1')
+    writer = pd.ExcelWriter('{0}/Energies.xlsx'.format(inputDir), engine='xlsxwriter')
+    sortedDF.to_excel(writer, startrow=1, sheet_name='Sheet1', index=False)
     workbook = writer.book
     worksheet = writer.sheets['Sheet1']
-    for i, col in enumerate(sorted_df.columns):
-        column_len = sorted_df[col].astype(str).str.len().max()
+    for i, col in enumerate(sortedDF.columns):
+        column_len = sortedDF[col].astype(str).str.len().max()
         column_len = max(column_len, len(col)) + 2
         worksheet.set_column(i, i, column_len)
     writer.save()
     return workbook
 
 
 if __name__ == "__main__":
 
     # Change this!
-    input_dir = "/User/kahochow/Desktop/Li_mechanism/Li_work/Reactant"
+    inputDir = "/User/kahochow/Desktop/Li_mechanism/Li_work/Reactant"
 
-    groups = [f for f in os.listdir(input_dir) if isdir('{0}/{1}'.format(input_dir, f))]
+    groups = [f for f in listdir(inputDir) if isdir('{0}/{1}'.format(inputDir, f))]
     print("\n# Tabulating values of interest from Gaussian .out files to an Excel sheet...")
-    print("\n# Input directory:\n", input_dir, "\n\n# Groups:\n", groups, "\n")
-    workbook = write_Excel(input_dir)
+    print("\n# Input directory:\n", inputDir, "\n\n# Groups:\n", groups, "\n")
+    workbook = writeToExcel(inputDir)
```

### Comparing `covdrugsim-0.2.0/src/covdrugsim/qmcalc/unitConv/unitConv.py` & `covdrugsim-0.3.0/src/covdrugsim/qmcalc/unitConv.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # (Assumes that the no-recrossing assumption of TST holds perfectly)
 kB = 1.380649 * 10 ** -23  # Boltzmann constant, relates avg relative KE of particles (g) with T [J/K]
 h = 6.62607015 * 10 ** -34  # Planck's constant, relates photon E to its f, quantum of electromagnetic action [Js]
 R = 8.314462618  # Ideal gas constant, equivalent to kB, but expressed in per mole [J/molK]
 cal2J = 4.184
 
 
-def E_unit_conv(E_kcal, E_kJ, verbose=False):
+def energyUnitsConversion(E_kcal, E_kJ, verbose=False):
     """Convert between kcal and kJ.
 
     Parameters
     ----------
     E_kcal : Union[float,bool]
         Energy (kcal).
     E_kJ : Union[float,bool]
@@ -39,15 +39,15 @@
     else:
         raise Exception("Both E_kcal & E_kJ are missing! Provide one.")
     if verbose:
         print("E_kcal =", E_kcal, "kcal/mol, E_kJ =", E_kJ, "kJ/mol")
     return E_kcal, E_kJ
 
 
-def eyring(k, dGbarr, T, verbose=False):
+def eyringEquation(k, dGbarr, T, verbose=False):
     """Calculate off rate or elimination barrier from each other at a specific temperature using Eyring-Polanyi equation.
 
     Parameters
     ----------
     k : Union[float,bool]
         Off rate (s^-1).
     dGbarr : Union[float,bool]
@@ -80,15 +80,15 @@
     dGbarr /= cal2J*1000  # Convert to kcal/mol
     if verbose:
         print("\n--------------------------------------\n\n# Using Eyring-Polanyi equation...")
         print("At T =", T, "K, k =", k, "s^-1, dGbarr =", dGbarr, "kcal/mol")
     return k, dGbarr
 
 
-def exp_time(k, t_half, RT, verbose=False):
+def timeUnitsConversion(k, t_half, RT, verbose=False):
     """Interconvert between off rate (s^-1), half life (s), and residence time (s).
 
     Parameters
     ----------
     k : Union[float,bool]
         Off rate (s^-1).
     t_hald : Union[float,bool]
```

### Comparing `covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py` & `covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py` & `covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py` & `covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.2.0/PKG-INFO` & `covdrugsim-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covdrugsim
-Version: 0.2.0
+Version: 0.3.0
 Summary: Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs.
 Home-page: https://github.com/Jon-Ting/covdrugsim
 License: MIT
 Keywords: covalent,drug,quantum,mechanic,molecular,dynamics,simulation
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
```

