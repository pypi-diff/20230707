# Comparing `tmp/hadder-1.9.tar.gz` & `tmp/hadder-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hadder-1.9.tar", last modified: Tue Jul  4 01:45:18 2023, max compression
+gzip compressed data, was "hadder-2.0.tar", last modified: Fri Jul  7 08:53:04 2023, max compression
```

## Comparing `hadder-1.9.tar` & `hadder-2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-07-04 01:45:18.299478 hadder-1.9/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)    11357 2023-06-27 09:36:35.000000 hadder-1.9/LICENSE
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     3199 2023-07-04 01:45:18.299478 hadder-1.9/PKG-INFO
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     2901 2023-06-27 09:36:35.000000 hadder-1.9/README.md
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-07-04 01:45:18.295478 hadder-1.9/hadder/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     8549 2023-06-27 09:36:35.000000 hadder-1.9/hadder/__init__.py
--rw-rw-r--   0 dechin    (1001) dechin    (1001)      893 2023-06-27 09:36:35.000000 hadder-1.9/hadder/__main__.py
--rw-rw-r--   0 dechin    (1001) dechin    (1001)    40338 2023-06-27 09:36:35.000000 hadder-1.9/hadder/constants.py
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     6059 2023-07-04 01:44:26.000000 hadder-1.9/hadder/parsers.py
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-07-04 01:45:18.299478 hadder-1.9/hadder.egg-info/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     3199 2023-07-04 01:45:18.000000 hadder-1.9/hadder.egg-info/PKG-INFO
--rw-rw-r--   0 dechin    (1001) dechin    (1001)      251 2023-07-04 01:45:18.000000 hadder-1.9/hadder.egg-info/SOURCES.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        1 2023-07-04 01:45:18.000000 hadder-1.9/hadder.egg-info/dependency_links.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)       20 2023-07-04 01:45:18.000000 hadder-1.9/hadder.egg-info/requires.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        7 2023-07-04 01:45:18.000000 hadder-1.9/hadder.egg-info/top_level.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)       38 2023-07-04 01:45:18.299478 hadder-1.9/setup.cfg
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     1488 2023-07-04 01:44:41.000000 hadder-1.9/setup.py
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-07-07 08:53:04.385965 hadder-2.0/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)    11357 2023-06-27 09:36:35.000000 hadder-2.0/LICENSE
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     3226 2023-07-07 08:53:04.385965 hadder-2.0/PKG-INFO
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     2928 2023-07-04 01:48:55.000000 hadder-2.0/README.md
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-07-07 08:53:04.385965 hadder-2.0/hadder/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     8549 2023-06-27 09:36:35.000000 hadder-2.0/hadder/__init__.py
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)      893 2023-06-27 09:36:35.000000 hadder-2.0/hadder/__main__.py
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)    40338 2023-06-27 09:36:35.000000 hadder-2.0/hadder/constants.py
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     6394 2023-07-07 08:52:25.000000 hadder-2.0/hadder/parsers.py
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-07-07 08:53:04.385965 hadder-2.0/hadder.egg-info/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     3226 2023-07-07 08:53:04.000000 hadder-2.0/hadder.egg-info/PKG-INFO
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)      251 2023-07-07 08:53:04.000000 hadder-2.0/hadder.egg-info/SOURCES.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)        1 2023-07-07 08:53:04.000000 hadder-2.0/hadder.egg-info/dependency_links.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)       20 2023-07-07 08:53:04.000000 hadder-2.0/hadder.egg-info/requires.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)        7 2023-07-07 08:53:04.000000 hadder-2.0/hadder.egg-info/top_level.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)       38 2023-07-07 08:53:04.385965 hadder-2.0/setup.cfg
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     1488 2023-07-06 01:06:46.000000 hadder-2.0/setup.py
```

### Comparing `hadder-1.9/LICENSE` & `hadder-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hadder-1.9/PKG-INFO` & `hadder-2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hadder
-Version: 1.9
+Version: 2.0
 Summary: Hydrogen adder for pdb protein files
 Home-page: https://gitee.com/dechin/hadder
 Author: Dechin CHEN
 Author-email: dechin.phy@gmail.com
 License: Apache 2.0 Licence
 Platform: any
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 很多蛋白质数据库往往会采用去掉氢原子的方式来存储各种pdb蛋白质结构文件，
 这就要求我们在实际构建力场的过程中手动去补齐氢原子，
 本开源工具就可以实现这样的功能。
 
 # 安装与使用
 本软件支持pip一键安装与更新：
 ```bash
-$ python3 -m pip install hadder --upgrade
+$ python3 -m pip install hadder --upgrade -i https://pypi.org/simple
 ```
 支持在python中调用API接口，来完成蛋白质补氢：
 ```python
 from hadder import AddHydrogen
 AddHydrogen('input.pdb', 'output.pdb')
 ```
 如果成功运行，会在终端窗口上打印如下文字：
```

### Comparing `hadder-1.9/README.md` & `hadder-2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 很多蛋白质数据库往往会采用去掉氢原子的方式来存储各种pdb蛋白质结构文件，
 这就要求我们在实际构建力场的过程中手动去补齐氢原子，
 本开源工具就可以实现这样的功能。
 
 # 安装与使用
 本软件支持pip一键安装与更新：
 ```bash
-$ python3 -m pip install hadder --upgrade
+$ python3 -m pip install hadder --upgrade -i https://pypi.org/simple
 ```
 支持在python中调用API接口，来完成蛋白质补氢：
 ```python
 from hadder import AddHydrogen
 AddHydrogen('input.pdb', 'output.pdb')
 ```
 如果成功运行，会在终端窗口上打印如下文字：
```

### Comparing `hadder-1.9/hadder/__init__.py` & `hadder-2.0/hadder/__init__.py`

 * *Files identical despite different names*

### Comparing `hadder-1.9/hadder/__main__.py` & `hadder-2.0/hadder/__main__.py`

 * *Files identical despite different names*

### Comparing `hadder-1.9/hadder/constants.py` & `hadder-2.0/hadder/constants.py`

 * *Files identical despite different names*

### Comparing `hadder-1.9/hadder/parsers.py` & `hadder-2.0/hadder/parsers.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 from .constants import atom14_order_dict
 
 
 atom_order = {atom_type: i for i, atom_type in enumerate(atom_types)}
 atom_type_num = len(atom_types)  # := 37.
 
 
-def read_pdb(pdb_name, ignoreh=False):
+def read_pdb(pdb_name, ignoreh=False, prefix=None):
     """Read a pdb file and return atom information with numpy array format.
     Args:
         pdb_name(str): The pdb file name, absolute path is suggested.
+        ignoreh(bool): Decide to load hydrogen atoms from pdb or not.
+        prefix(str): If multi results exists in a residue, we need to choose one via given prefix.
     Returns:
         atom_names(list): 1-dimension list contain all atom names in each residue.
         res_names(list): 1-dimension list of all residue names.
         res_ids(numpy.int32): Unique id for each residue names.
         crds(list): The list format of coordinates.
         res_pointer(numpy.int32): The pointer where the residue starts.
         flatten_atoms(numpy.str_): The flatten atom names.
@@ -46,42 +48,47 @@
     init_res_ids = []
     crds = []
     crd_group = []
     res_pointer = []
     flatten_atoms = []
     flatten_crds = []
     for index, line in enumerate(lines):
-        if 'END' in line or 'TER' in line:
+        if line.startswith('END') or line.startswith('TER'):
             atom_names.append(atom_group)
             crds.append(crd_group)
             break
         if not line.startswith('ATOM'):
             continue
         atom_name = line[12:16].strip()
         if ignoreh and atom_name.startswith('H'):
             continue
-        res_name = line[17:20].strip()
+        res_name = line[16:20].strip()
         res_id = int(line[22:26].strip())
         crd = [float(line[30:38]),
                float(line[38:46]),
                float(line[46:54])]
         pointer = int(line[6:11].strip()) - 1
+
+        if prefix is not None:
+            if len(res_name) == 4 and not res_name.startswith(prefix):
+                continue
+            elif len(res_name) == 4:
+                res_name = res_name[1:]
+
         flatten_atoms.append(atom_name)
         flatten_crds.append(crd)
         init_res_names.append(res_name)
         init_res_ids.append(res_id)
         if res_ids == []:
             res_ids.append(res_id)
             res_names.append(res_name)
             atom_group.append(atom_name)
             crd_group.append(crd)
             res_pointer.append(0)
-            atom_pos = np.zeros((14, 3))
         elif res_id != res_ids[-1]:
-            atom_pos = np.zeros((14, 3))
             atom_names.append(atom_group)
             crds.append(crd_group)
             atom_group = []
             crd_group = []
             res_ids.append(res_id)
             res_names.append(res_name)
             atom_group.append(atom_name)
@@ -130,15 +137,15 @@
     """
     success = 1
     with open(pdb_name, 'w') as pdb:
         # pdb.write('REMARK    1 Generated By MindSponge (Molecule)\n')
         pdb.write('MODEL     1\n')
         for i, c in enumerate(crd[0]):
             pdb.write('ATOM'.ljust(6))
-            pdb.write('{}'.format(i + 1).rjust(5))
+            pdb.write('{}'.format((i + 1) % 100000).rjust(5))
             if len(atom_names[i]) < 4:
                 pdb.write('  ')
                 pdb.write(atom_names[i].ljust(3))
             else:
                 pdb.write(' ')
                 pdb.write(atom_names[i].ljust(4))
             pdb.write(res_names[i].rjust(4))
```

### Comparing `hadder-1.9/hadder.egg-info/PKG-INFO` & `hadder-2.0/hadder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hadder
-Version: 1.9
+Version: 2.0
 Summary: Hydrogen adder for pdb protein files
 Home-page: https://gitee.com/dechin/hadder
 Author: Dechin CHEN
 Author-email: dechin.phy@gmail.com
 License: Apache 2.0 Licence
 Platform: any
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 很多蛋白质数据库往往会采用去掉氢原子的方式来存储各种pdb蛋白质结构文件，
 这就要求我们在实际构建力场的过程中手动去补齐氢原子，
 本开源工具就可以实现这样的功能。
 
 # 安装与使用
 本软件支持pip一键安装与更新：
 ```bash
-$ python3 -m pip install hadder --upgrade
+$ python3 -m pip install hadder --upgrade -i https://pypi.org/simple
 ```
 支持在python中调用API接口，来完成蛋白质补氢：
 ```python
 from hadder import AddHydrogen
 AddHydrogen('input.pdb', 'output.pdb')
 ```
 如果成功运行，会在终端窗口上打印如下文字：
```

### Comparing `hadder-1.9/setup.py` & `hadder-2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="hadder",
-    version="1.9",
+    version="2.0",
     description="Hydrogen adder for pdb protein files",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="Apache 2.0 Licence",
 
     url="https://gitee.com/dechin/hadder",
     author="Dechin CHEN",
```

