# Comparing `tmp/seg_mask_modifs-1.0.2.tar.gz` & `tmp/seg_mask_modifs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seg_mask_modifs-1.0.2.tar", last modified: Sun Jun  5 10:44:24 2022, max compression
+gzip compressed data, was "seg_mask_modifs-1.2.0.tar", last modified: Fri Jul  7 09:02:44 2023, max compression
```

## Comparing `seg_mask_modifs-1.0.2.tar` & `seg_mask_modifs-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxr-x   0 vardan    (1000) vardan    (1000)        0 2022-06-05 10:44:24.765649 seg_mask_modifs-1.0.2/
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     1071 2022-02-11 05:19:38.000000 seg_mask_modifs-1.0.2/LICENSE
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     5577 2022-06-05 10:44:24.765649 seg_mask_modifs-1.0.2/PKG-INFO
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     4949 2022-03-03 14:18:03.000000 seg_mask_modifs-1.0.2/README.md
--rw-rw-r--   0 vardan    (1000) vardan    (1000)      103 2022-02-11 05:19:38.000000 seg_mask_modifs-1.0.2/pyproject.toml
-drwxrwxr-x   0 vardan    (1000) vardan    (1000)        0 2022-06-05 10:44:24.765649 seg_mask_modifs-1.0.2/seg_mask_modifs/
--rw-rw-r--   0 vardan    (1000) vardan    (1000)        0 2022-02-11 05:19:38.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/__init__.py
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     2693 2022-02-11 05:19:38.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/download_models.py
--rw-rw-r--   0 vardan    (1000) vardan    (1000)      953 2022-06-03 06:13:25.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/gen.py
--rw-rw-r--   0 vardan    (1000) vardan    (1000)    11340 2022-06-03 11:10:17.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/mask_generator.py
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     7144 2022-03-03 14:11:08.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/mask_modifier.py
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     2294 2022-02-11 05:19:38.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/mask_utils.py
-drwxrwxr-x   0 vardan    (1000) vardan    (1000)        0 2022-06-05 10:44:24.765649 seg_mask_modifs-1.0.2/seg_mask_modifs/model_utils/
--rw-rw-r--   0 vardan    (1000) vardan    (1000)        0 2022-06-03 10:07:59.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/model_utils/__init__.py
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     1707 2022-06-03 11:03:49.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/model_utils/labels.py
--rw-rw-r--   0 vardan    (1000) vardan    (1000)    10889 2022-06-03 11:09:30.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/model_utils/model_celebmask.py
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     3618 2022-06-03 10:04:34.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/model_utils/resnet.py
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     1009 2022-06-03 11:10:39.000000 seg_mask_modifs-1.0.2/seg_mask_modifs/print_labels.py
-drwxrwxr-x   0 vardan    (1000) vardan    (1000)        0 2022-06-05 10:44:24.765649 seg_mask_modifs-1.0.2/seg_mask_modifs.egg-info/
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     5577 2022-06-05 10:44:24.000000 seg_mask_modifs-1.0.2/seg_mask_modifs.egg-info/PKG-INFO
--rw-rw-r--   0 vardan    (1000) vardan    (1000)      623 2022-06-05 10:44:24.000000 seg_mask_modifs-1.0.2/seg_mask_modifs.egg-info/SOURCES.txt
--rw-rw-r--   0 vardan    (1000) vardan    (1000)        1 2022-06-05 10:44:24.000000 seg_mask_modifs-1.0.2/seg_mask_modifs.egg-info/dependency_links.txt
--rw-rw-r--   0 vardan    (1000) vardan    (1000)       88 2022-06-05 10:44:24.000000 seg_mask_modifs-1.0.2/seg_mask_modifs.egg-info/requires.txt
--rw-rw-r--   0 vardan    (1000) vardan    (1000)       16 2022-06-05 10:44:24.000000 seg_mask_modifs-1.0.2/seg_mask_modifs.egg-info/top_level.txt
--rw-rw-r--   0 vardan    (1000) vardan    (1000)       70 2022-06-05 10:44:24.765649 seg_mask_modifs-1.0.2/setup.cfg
--rw-rw-r--   0 vardan    (1000) vardan    (1000)     1121 2022-06-05 10:44:10.000000 seg_mask_modifs-1.0.2/setup.py
+drwxrwxr-x   0 vardan    (1000) vardan    (1000)        0 2023-07-07 09:02:44.643413 seg_mask_modifs-1.2.0/
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     1071 2023-04-21 14:30:03.000000 seg_mask_modifs-1.2.0/LICENSE
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     5332 2023-07-07 09:02:44.643413 seg_mask_modifs-1.2.0/PKG-INFO
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     4704 2023-04-21 15:10:07.000000 seg_mask_modifs-1.2.0/README.md
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)      103 2023-04-21 14:30:03.000000 seg_mask_modifs-1.2.0/pyproject.toml
+drwxrwxr-x   0 vardan    (1000) vardan    (1000)        0 2023-07-07 09:02:44.643413 seg_mask_modifs-1.2.0/seg_mask_modifs/
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)        0 2023-04-21 14:30:03.000000 seg_mask_modifs-1.2.0/seg_mask_modifs/__init__.py
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     3994 2023-04-21 15:12:31.000000 seg_mask_modifs-1.2.0/seg_mask_modifs/download_models.py
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)    16418 2023-04-21 15:12:31.000000 seg_mask_modifs-1.2.0/seg_mask_modifs/mask_generator.py
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     7144 2023-04-21 14:30:03.000000 seg_mask_modifs-1.2.0/seg_mask_modifs/mask_modifier.py
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     5661 2023-04-21 15:12:31.000000 seg_mask_modifs-1.2.0/seg_mask_modifs/mask_utils.py
+drwxrwxr-x   0 vardan    (1000) vardan    (1000)        0 2023-07-07 09:02:44.643413 seg_mask_modifs-1.2.0/seg_mask_modifs/model_utils/
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)        0 2023-04-21 14:30:03.000000 seg_mask_modifs-1.2.0/seg_mask_modifs/model_utils/__init__.py
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     1707 2023-04-21 14:30:03.000000 seg_mask_modifs-1.2.0/seg_mask_modifs/model_utils/labels.py
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)    10889 2023-04-21 14:30:03.000000 seg_mask_modifs-1.2.0/seg_mask_modifs/model_utils/model_celebmask.py
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     3618 2023-04-21 14:30:03.000000 seg_mask_modifs-1.2.0/seg_mask_modifs/model_utils/resnet.py
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     1138 2023-04-21 15:12:31.000000 seg_mask_modifs-1.2.0/seg_mask_modifs/print_labels.py
+drwxrwxr-x   0 vardan    (1000) vardan    (1000)        0 2023-07-07 09:02:44.643413 seg_mask_modifs-1.2.0/seg_mask_modifs.egg-info/
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     5332 2023-07-07 09:02:44.000000 seg_mask_modifs-1.2.0/seg_mask_modifs.egg-info/PKG-INFO
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)      600 2023-07-07 09:02:44.000000 seg_mask_modifs-1.2.0/seg_mask_modifs.egg-info/SOURCES.txt
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)        1 2023-07-07 09:02:44.000000 seg_mask_modifs-1.2.0/seg_mask_modifs.egg-info/dependency_links.txt
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)       88 2023-07-07 09:02:44.000000 seg_mask_modifs-1.2.0/seg_mask_modifs.egg-info/requires.txt
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)       16 2023-07-07 09:02:44.000000 seg_mask_modifs-1.2.0/seg_mask_modifs.egg-info/top_level.txt
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)       70 2023-07-07 09:02:44.643413 seg_mask_modifs-1.2.0/setup.cfg
+-rw-rw-r--   0 vardan    (1000) vardan    (1000)     1121 2023-07-07 09:01:52.000000 seg_mask_modifs-1.2.0/setup.py
```

### Comparing `seg_mask_modifs-1.0.2/LICENSE` & `seg_mask_modifs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seg_mask_modifs-1.0.2/PKG-INFO` & `seg_mask_modifs-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: seg_mask_modifs
-Version: 1.0.2
+Version: 1.2.0
 Summary: A package for easy generation of mask of different labels using multiple models and applying different operations on that.
 Home-page: https://github.com/vardanagarwal/seg_mask_modifs
 Author: Vardan Agarwal
 Author-email: vardanagarwal16@gmail.com
 Project-URL: Bug Tracker, https://github.com/vardanagarwal/seg_mask_modifs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # seg_mask_modifs
 
-[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fvardanagarwal%2Fmask_modifs&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
-
 ## Description
 A package for easy generation of binary semantic mask of different labels using multiple models easily. Moreover, supports operations on the mask created for image editing.
 
 #### Curent models and labels supported:
 - Deeplabv3 with pascal labels
 - Maskrcnn with coco labels
 - Bisnet with face labels
```

### Comparing `seg_mask_modifs-1.0.2/README.md` & `seg_mask_modifs-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # seg_mask_modifs
 
-[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fvardanagarwal%2Fmask_modifs&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
-
 ## Description
 A package for easy generation of binary semantic mask of different labels using multiple models easily. Moreover, supports operations on the mask created for image editing.
 
 #### Curent models and labels supported:
 - Deeplabv3 with pascal labels
 - Maskrcnn with coco labels
 - Bisnet with face labels
```

### Comparing `seg_mask_modifs-1.0.2/seg_mask_modifs/mask_modifier.py` & `seg_mask_modifs-1.2.0/seg_mask_modifs/mask_modifier.py`

 * *Files identical despite different names*

### Comparing `seg_mask_modifs-1.0.2/seg_mask_modifs/model_utils/labels.py` & `seg_mask_modifs-1.2.0/seg_mask_modifs/model_utils/labels.py`

 * *Files identical despite different names*

### Comparing `seg_mask_modifs-1.0.2/seg_mask_modifs/model_utils/model_celebmask.py` & `seg_mask_modifs-1.2.0/seg_mask_modifs/model_utils/model_celebmask.py`

 * *Files identical despite different names*

### Comparing `seg_mask_modifs-1.0.2/seg_mask_modifs/model_utils/resnet.py` & `seg_mask_modifs-1.2.0/seg_mask_modifs/model_utils/resnet.py`

 * *Files identical despite different names*

### Comparing `seg_mask_modifs-1.0.2/seg_mask_modifs/print_labels.py` & `seg_mask_modifs-1.2.0/seg_mask_modifs/print_labels.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,21 @@
     Returns: list of labels"""
 
     labels = data['face_labels'][1:]
     print(', '.join(labels))
 
     return labels
 
+def sam():
+    """ Print sam labels
+
+    Returns: list of labels. Empty dictionary as it is a zero shot model"""
+
+    return []
+
 
 def all():
     """ Print labels of all models"""
 
     print('MaskRCNN labels')
     maskrcnn_coco()
```

### Comparing `seg_mask_modifs-1.0.2/seg_mask_modifs.egg-info/PKG-INFO` & `seg_mask_modifs-1.2.0/seg_mask_modifs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: seg-mask-modifs
-Version: 1.0.2
+Version: 1.2.0
 Summary: A package for easy generation of mask of different labels using multiple models and applying different operations on that.
 Home-page: https://github.com/vardanagarwal/seg_mask_modifs
 Author: Vardan Agarwal
 Author-email: vardanagarwal16@gmail.com
 Project-URL: Bug Tracker, https://github.com/vardanagarwal/seg_mask_modifs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # seg_mask_modifs
 
-[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fvardanagarwal%2Fmask_modifs&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
-
 ## Description
 A package for easy generation of binary semantic mask of different labels using multiple models easily. Moreover, supports operations on the mask created for image editing.
 
 #### Curent models and labels supported:
 - Deeplabv3 with pascal labels
 - Maskrcnn with coco labels
 - Bisnet with face labels
```

### Comparing `seg_mask_modifs-1.0.2/seg_mask_modifs.egg-info/SOURCES.txt` & `seg_mask_modifs-1.2.0/seg_mask_modifs.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 seg_mask_modifs/__init__.py
 seg_mask_modifs/download_models.py
-seg_mask_modifs/gen.py
 seg_mask_modifs/mask_generator.py
 seg_mask_modifs/mask_modifier.py
 seg_mask_modifs/mask_utils.py
 seg_mask_modifs/print_labels.py
 seg_mask_modifs.egg-info/PKG-INFO
 seg_mask_modifs.egg-info/SOURCES.txt
 seg_mask_modifs.egg-info/dependency_links.txt
```

### Comparing `seg_mask_modifs-1.0.2/setup.py` & `seg_mask_modifs-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seg_mask_modifs",
-    version="1.0.2",
+    version="1.2.0",
     author="Vardan Agarwal",
     author_email="vardanagarwal16@gmail.com",
     description="A package for easy generation of mask of different labels using multiple models"
                 " and applying different operations on that.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vardanagarwal/seg_mask_modifs",
```

