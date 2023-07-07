# Comparing `tmp/segment-lidar-0.1.6.tar.gz` & `tmp/segment-lidar-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\segment-lidar-0.1.6.tar", last modified: Fri Jun 30 18:35:57 2023, max compression
+gzip compressed data, was "dist\segment-lidar-0.1.7.tar", last modified: Fri Jul  7 10:41:24 2023, max compression
```

## Comparing `segment-lidar-0.1.6.tar` & `segment-lidar-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 18:35:57.456594 segment-lidar-0.1.6/
--rw-rw-rw-   0        0        0     1608 2023-06-30 18:32:20.000000 segment-lidar-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     6286 2023-06-30 18:35:57.455596 segment-lidar-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5744 2023-06-30 18:32:20.000000 segment-lidar-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 18:35:57.415704 segment-lidar-0.1.6/segment_lidar/
--rw-rw-rw-   0        0        0        0 2023-06-30 18:32:20.000000 segment-lidar-0.1.6/segment_lidar/__init__.py
--rw-rw-rw-   0        0        0    19012 2023-06-30 18:33:58.000000 segment-lidar-0.1.6/segment_lidar/samlidar.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:35:57.453628 segment-lidar-0.1.6/segment_lidar.egg-info/
--rw-rw-rw-   0        0        0     6286 2023-06-30 18:35:56.000000 segment-lidar-0.1.6/segment_lidar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-30 18:35:56.000000 segment-lidar-0.1.6/segment_lidar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 18:35:56.000000 segment-lidar-0.1.6/segment_lidar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-06-30 18:35:56.000000 segment-lidar-0.1.6/segment_lidar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 18:35:56.000000 segment-lidar-0.1.6/segment_lidar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 18:35:57.456594 segment-lidar-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-06-30 18:33:17.000000 segment-lidar-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:41:24.780911 segment-lidar-0.1.7/
+-rw-rw-rw-   0        0        0     1608 2023-06-30 18:32:20.000000 segment-lidar-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     6680 2023-07-07 10:41:24.759548 segment-lidar-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6138 2023-07-07 10:40:00.000000 segment-lidar-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 10:41:24.151334 segment-lidar-0.1.7/segment_lidar/
+-rw-rw-rw-   0        0        0        0 2023-06-30 18:32:20.000000 segment-lidar-0.1.7/segment_lidar/__init__.py
+-rw-rw-rw-   0        0        0    19042 2023-07-07 10:20:38.000000 segment-lidar-0.1.7/segment_lidar/samlidar.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:41:24.654560 segment-lidar-0.1.7/segment_lidar.egg-info/
+-rw-rw-rw-   0        0        0     6680 2023-07-07 10:41:22.000000 segment-lidar-0.1.7/segment_lidar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-07 10:41:22.000000 segment-lidar-0.1.7/segment_lidar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:41:22.000000 segment-lidar-0.1.7/segment_lidar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-07-07 10:41:22.000000 segment-lidar-0.1.7/segment_lidar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 10:41:22.000000 segment-lidar-0.1.7/segment_lidar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 10:41:24.780911 segment-lidar-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-07-07 10:22:26.000000 segment-lidar-0.1.7/setup.py
```

### Comparing `segment-lidar-0.1.6/LICENSE` & `segment-lidar-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-lidar-0.1.6/PKG-INFO` & `segment-lidar-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-lidar
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
 Home-page: https://github.com/Yarroudh/segment-lidar
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -15,15 +15,15 @@
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 [![read - documentation](https://img.shields.io/static/v1?label=read&message=documentation&color=orange)](https://yarroudh.gitbook.io/segment-lidar/)
 
-*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI.*
+*Python package for segmenting aerial LiDAR data using Segment-Anything Model (SAM) from Meta AI.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
 ![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/089a603b-697e-4483-af1e-3687a79adcc1)
 
 ## Installation
 
@@ -50,14 +50,27 @@
 If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](https://yarroudh.gitbook.io/segment-lidar/). The documentation is an essential resource that will help you understand the features of the package, as well as provide guidance on how to use it effectively.
 
 ## Basic tutorial
 
 A basic tutorial is available [here](https://yarroudh.gitbook.io/segment-lidar/tutorial/basic-usage).
 You can also refer to API for more information about different parameters.
 
+### Without ground filtering
+
+```python
+from segment_lidar import samlidar
+
+model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
+points = model.read("pointcloud.las")
+labels, *_ = model.segment(points=points, image_path="raster.tif", labels_path="labeled.tif")
+model.write(points=points, segment_ids=labels, save_path="segmented.las")
+```
+
+### With ground filtering
+
 ```python
 from segment_lidar import samlidar
 
 model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
 points = model.read("pointcloud.las")
 cloud, non_ground, ground = model.csf(points)
 labels, *_ = model.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
```

### Comparing `segment-lidar-0.1.6/README.md` & `segment-lidar-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 [![read - documentation](https://img.shields.io/static/v1?label=read&message=documentation&color=orange)](https://yarroudh.gitbook.io/segment-lidar/)
 
-*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI.*
+*Python package for segmenting aerial LiDAR data using Segment-Anything Model (SAM) from Meta AI.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
 ![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/089a603b-697e-4483-af1e-3687a79adcc1)
 
 ## Installation
 
@@ -36,14 +36,27 @@
 If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](https://yarroudh.gitbook.io/segment-lidar/). The documentation is an essential resource that will help you understand the features of the package, as well as provide guidance on how to use it effectively.
 
 ## Basic tutorial
 
 A basic tutorial is available [here](https://yarroudh.gitbook.io/segment-lidar/tutorial/basic-usage).
 You can also refer to API for more information about different parameters.
 
+### Without ground filtering
+
+```python
+from segment_lidar import samlidar
+
+model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
+points = model.read("pointcloud.las")
+labels, *_ = model.segment(points=points, image_path="raster.tif", labels_path="labeled.tif")
+model.write(points=points, segment_ids=labels, save_path="segmented.las")
+```
+
+### With ground filtering
+
 ```python
 from segment_lidar import samlidar
 
 model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
 points = model.read("pointcloud.las")
 cloud, non_ground, ground = model.csf(points)
 labels, *_ = model.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
```

### Comparing `segment-lidar-0.1.6/segment_lidar/samlidar.py` & `segment-lidar-0.1.7/segment_lidar/samlidar.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
             }
         else:
             self.sam_kwargs = None
 
         self.sam_geo = SamGeo(
             model_type=self.model_type,
             checkpoint=self.ckpt_path,
+            device=self.device,
             sam_kwargs=self.sam_kwargs
         )
 
         os.environ['KMP_DUPLICATE_LIB_OK'] = 'True'
 
 
 
@@ -393,15 +394,15 @@
         if ground is not None:
             indices = np.concatenate((non_ground, ground))
             lidar.xyz = points[indices]
             segment_ids = np.append(segment_ids, np.full(len(ground), -1))
             lidar.add_extra_dim(laspy.ExtraBytesParams(name="segment_id", type=np.int32))
             lidar.segment_id = segment_ids
         else:
-            lidar.points = points
+            lidar.xyz = points
             lidar.add_extra_dim(laspy.ExtraBytesParams(name="segment_id", type=np.int32))
             lidar.segment_id = segment_ids
 
         lidar.write(save_path)
 
         end = time.time()
         print(f'Writing is completed in {end - start:.2f} seconds.\n')
```

### Comparing `segment-lidar-0.1.6/segment_lidar.egg-info/PKG-INFO` & `segment-lidar-0.1.7/segment_lidar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-lidar
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
 Home-page: https://github.com/Yarroudh/segment-lidar
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -15,15 +15,15 @@
 <img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>
 
 # segment-lidar
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/Yarroudh/ZRect3D/blob/main/LICENSE)
 [![Geomatics Unit of ULiege - Development](https://img.shields.io/badge/Geomatics_Unit_of_ULiege-Development-2ea44f)](http://geomatics.ulg.ac.be/)
 [![read - documentation](https://img.shields.io/static/v1?label=read&message=documentation&color=orange)](https://yarroudh.gitbook.io/segment-lidar/)
 
-*Python package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI.*
+*Python package for segmenting aerial LiDAR data using Segment-Anything Model (SAM) from Meta AI.*
 
 This package is specifically designed for **unsupervised instance segmentation** of **aerial LiDAR data**. It brings together the power of the **Segment-Anything Model (SAM)** developed by [Meta Research](https://github.com/facebookresearch) and the **segment-geospatial** package from [Open Geospatial Solutions](https://github.com/opengeos). Whether you're a researcher, developer, or a geospatial enthusiast, segment-lidar opens up new possibilities for automatic processing of aerial LiDAR data and enables further applications. We encourage you to explore our code, contribute to its development and leverage its capabilities for your segmentation tasks.
 
 ![results](https://github.com/Yarroudh/segment-lidar/assets/72500344/089a603b-697e-4483-af1e-3687a79adcc1)
 
 ## Installation
 
@@ -50,14 +50,27 @@
 If you are using `segment-lidar`, we highly recommend that you take the time to read the [documentation](https://yarroudh.gitbook.io/segment-lidar/). The documentation is an essential resource that will help you understand the features of the package, as well as provide guidance on how to use it effectively.
 
 ## Basic tutorial
 
 A basic tutorial is available [here](https://yarroudh.gitbook.io/segment-lidar/tutorial/basic-usage).
 You can also refer to API for more information about different parameters.
 
+### Without ground filtering
+
+```python
+from segment_lidar import samlidar
+
+model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
+points = model.read("pointcloud.las")
+labels, *_ = model.segment(points=points, image_path="raster.tif", labels_path="labeled.tif")
+model.write(points=points, segment_ids=labels, save_path="segmented.las")
+```
+
+### With ground filtering
+
 ```python
 from segment_lidar import samlidar
 
 model = samlidar.SamLidar(ckpt_path="sam_vit_h_4b8939.pth")
 points = model.read("pointcloud.las")
 cloud, non_ground, ground = model.csf(points)
 labels, *_ = model.segment(points=cloud, image_path="raster.tif", labels_path="labeled.tif")
```

### Comparing `segment-lidar-0.1.6/setup.py` & `segment-lidar-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         except ImportError:
             subprocess.call(['pip', 'install', 'git+https://github.com/jianboqi/CSF.git'])
         from samgeo import SamGeo
         from samgeo.text_sam import LangSAM
 
 setup(
     name="segment-lidar",
-    version='0.1.6',
+    version='0.1.7',
     description="A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license='BSD 3-Clause "New" or "Revised" License',
     author='Anass Yarroudh',
     author_email='ayarroudh@uliege.be',
     url='https://github.com/Yarroudh/segment-lidar',
```

