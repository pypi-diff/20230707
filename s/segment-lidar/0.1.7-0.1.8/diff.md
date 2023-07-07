# Comparing `tmp/segment-lidar-0.1.7.tar.gz` & `tmp/segment-lidar-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\segment-lidar-0.1.7.tar", last modified: Fri Jul  7 10:41:24 2023, max compression
+gzip compressed data, was "segment-lidar-0.1.8.tar", last modified: Fri Jul  7 19:15:12 2023, max compression
```

## Comparing `segment-lidar-0.1.7.tar` & `segment-lidar-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 10:41:24.780911 segment-lidar-0.1.7/
--rw-rw-rw-   0        0        0     1608 2023-06-30 18:32:20.000000 segment-lidar-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     6680 2023-07-07 10:41:24.759548 segment-lidar-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6138 2023-07-07 10:40:00.000000 segment-lidar-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 10:41:24.151334 segment-lidar-0.1.7/segment_lidar/
--rw-rw-rw-   0        0        0        0 2023-06-30 18:32:20.000000 segment-lidar-0.1.7/segment_lidar/__init__.py
--rw-rw-rw-   0        0        0    19042 2023-07-07 10:20:38.000000 segment-lidar-0.1.7/segment_lidar/samlidar.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:41:24.654560 segment-lidar-0.1.7/segment_lidar.egg-info/
--rw-rw-rw-   0        0        0     6680 2023-07-07 10:41:22.000000 segment-lidar-0.1.7/segment_lidar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-07 10:41:22.000000 segment-lidar-0.1.7/segment_lidar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 10:41:22.000000 segment-lidar-0.1.7/segment_lidar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-07-07 10:41:22.000000 segment-lidar-0.1.7/segment_lidar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 10:41:22.000000 segment-lidar-0.1.7/segment_lidar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 10:41:24.780911 segment-lidar-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-07-07 10:22:26.000000 segment-lidar-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:15:12.907227 segment-lidar-0.1.8/
+-rw-rw-rw-   0        0        0     1608 2023-07-07 11:54:01.000000 segment-lidar-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     6680 2023-07-07 19:15:12.906228 segment-lidar-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6138 2023-07-07 11:54:01.000000 segment-lidar-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 19:15:12.849763 segment-lidar-0.1.8/segment_lidar/
+-rw-rw-rw-   0        0        0        0 2023-07-07 11:54:01.000000 segment-lidar-0.1.8/segment_lidar/__init__.py
+-rw-rw-rw-   0        0        0    19617 2023-07-07 19:10:03.000000 segment-lidar-0.1.8/segment_lidar/samlidar.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:15:12.899288 segment-lidar-0.1.8/segment_lidar.egg-info/
+-rw-rw-rw-   0        0        0     6680 2023-07-07 19:15:12.000000 segment-lidar-0.1.8/segment_lidar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-07 19:15:12.000000 segment-lidar-0.1.8/segment_lidar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 19:15:12.000000 segment-lidar-0.1.8/segment_lidar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-07-07 19:15:12.000000 segment-lidar-0.1.8/segment_lidar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 19:15:12.000000 segment-lidar-0.1.8/segment_lidar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 19:15:12.908231 segment-lidar-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-07-07 19:11:27.000000 segment-lidar-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:15:12.902230 segment-lidar-0.1.8/tests/
+-rw-rw-rw-   0        0        0      382 2023-07-07 13:38:17.000000 segment-lidar-0.1.8/tests/test.py
```

### Comparing `segment-lidar-0.1.7/LICENSE` & `segment-lidar-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-lidar-0.1.7/PKG-INFO` & `segment-lidar-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-lidar
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
 Home-page: https://github.com/Yarroudh/segment-lidar
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `segment-lidar-0.1.7/README.md` & `segment-lidar-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `segment-lidar-0.1.7/segment_lidar/samlidar.py` & `segment-lidar-0.1.8/segment_lidar/samlidar.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,33 +37,31 @@
     :param resolution: The resolution of the image in units per pixel.
     :type resolution: float
     :return: An image array representing the point cloud, where each pixel contains the RGB color values
              of the corresponding point in the cloud.
     :rtype: ndarray
     :raises ValueError: If the shape of the points array is not valid or if any parameter is invalid.
     """
+    if points.shape[1] == 3:
+        colors = np.array([255, 255, 255])
+    else:
+        colors = points[:, -3:]
+
+    x = (points[:, 0] - minx) / resolution
+    y = (maxy - points[:, 1]) / resolution
+    pixel_x = np.floor(x).astype(int)
+    pixel_y = np.floor(y).astype(int)
+
     width = int((maxx - minx) / resolution) + 1
     height = int((maxy - miny) / resolution) + 1
 
     image = np.zeros((height, width, 3), dtype=np.uint8)
-    for point in points:
-        if points.shape[1] == 3:
-            x, y, *_ = point
-            r, g, b = (255, 255, 255)
-            pixel_x = int((x - minx) / resolution)
-            pixel_y = int((maxy - y) / resolution)
-            image[pixel_y, pixel_x] = [r, g, b]
-        else:
-            x, y, *_ = point
-            r, g, b = point[-3:]
-            pixel_x = int((x - minx) / resolution)
-            pixel_y = int((maxy - y) / resolution)
-            image[pixel_y, pixel_x] = [r, g, b]
-    return image
+    image[pixel_y, pixel_x] = colors
 
+    return image
 
 
 def image_to_cloud(points: np.ndarray, minx: float, maxy: float, image: np.ndarray, resolution: float) -> List[int]:
     """
     Converts an image to a point cloud with segment IDs.
 
     :param points: An array of points representing the cloud, where each row represents a point.
@@ -76,28 +74,35 @@
              in the input image that the corresponding point belongs to.
     :rtype: List[int]
     """
     segment_ids = []
     unique_values = {}
     image = np.asarray(image)
 
-    for point in points:
-        x, y, *_ = point
-        pixel_x = int((x - minx) / resolution)
-        pixel_y = int((maxy - y) / resolution)
-        if not (0 <= pixel_x < image.shape[1]) or not (0 <= pixel_y < image.shape[0]):
-            segment_ids.append(-1)
-            continue
-        rgb = image[pixel_y, pixel_x]
+    # Calculate pixel coordinates for all points
+    x = (points[:, 0] - minx) / resolution
+    y = (maxy - points[:, 1]) / resolution
+    pixel_x = np.floor(x).astype(int)
+    pixel_y = np.floor(y).astype(int)
+
+    # Mask points outside image bounds
+    out_of_bounds = (pixel_x < 0) | (pixel_x >= image.shape[1]) | (pixel_y < 0) | (pixel_y >= image.shape[0])
+    segment_ids.extend([-1] * np.sum(out_of_bounds))
+
+    # Extract RGB values for valid points
+    valid_points = ~out_of_bounds
+    rgb = image[pixel_y[valid_points], pixel_x[valid_points]]
+
+    # Map RGB values to unique segment IDs
+    for rgb_val in rgb:
+        if rgb_val not in unique_values:
+            unique_values[rgb_val] = len(unique_values)
 
-        if rgb not in unique_values:
-            unique_values[rgb] = len(unique_values)
+        segment_ids.append(unique_values[rgb_val])
 
-        id = unique_values[rgb]
-        segment_ids.append(id)
     return segment_ids
 
 
 class mask:
     def __init__(self, crop_n_layers: int = 1, crop_n_points_downscale_factor: int = 1, min_mask_region_area: int = 200, points_per_side: int = 5, pred_iou_thresh: float = 0.90, stability_score_thresh: float = 0.92):
         """
         Initializes an instance of the mask class.
@@ -144,15 +149,15 @@
         self.algorithm = algorithm
         self.model_type = model_type
         self.ckpt_path = ckpt_path
         self.resolution = resolution
         self.device = torch.device('cuda:0') if device == 'cuda:0' and torch.cuda.is_available() else torch.device('cpu')
         self.mask = mask()
 
-        if sam_kwargs:
+        if sam_kwargs or algorithm == 'segment-anything':
             self.mask_generator = SamAutomaticMaskGenerator(
                 model=sam_model_registry[model_type](checkpoint=ckpt_path).to(device=self.device),
                 crop_n_layers=self.mask.crop_n_layers,
                 crop_n_points_downscale_factor=self.mask.crop_n_points_downscale_factor,
                 min_mask_region_area=self.mask.min_mask_region_area,
                 points_per_side=self.mask.points_per_side,
                 pred_iou_thresh=self.mask.pred_iou_thresh,
@@ -322,22 +327,36 @@
             image_rgb = src.read()
 
         print(f'- Applying {self.algorithm} to raster image...')
         if self.algorithm == 'segment-anything':
             sam = sam_model_registry[self.model_type](checkpoint=self.ckpt_path)
             sam.to(self.device)
 
-            image_rgb = image_rgb.reshape((image_rgb.shape[1], image_rgb.shape[2], image_rgb.shape[0]))
+            image_rgb = image_rgb.transpose(1, 2, 0)
             result = self.mask_generator.generate(image_rgb)
             mask_annotator = sv.MaskAnnotator()
             detections = sv.Detections.from_sam(result)
-            segmented_image = mask_annotator.annotate(image_rgb, detections)
+            num_masks, height, width = detections.mask.shape
+            segmented_image = np.zeros((height, width), dtype=np.uint8)
+            for i in range(num_masks):
+                mask = detections.mask[i]
+                segmented_image[mask] = i
 
-            cv2.imwrite(labels_path, segmented_image)
             print(f'- Saving segmented image...')
+            with rasterio.open(
+                labels_path,
+                'w',
+                driver='GTiff',
+                width=segmented_image.shape[1],
+                height=segmented_image.shape[0],
+                count=1,
+                dtype=segmented_image.dtype
+            ) as dst:
+                dst.write(segmented_image, 1)
+
 
         elif self.algorithm == 'segment-geospatial':
             if text_prompt is not None:
                 print(f'- Generating labels using text prompt...')
                 sam = LangSAM()
                 sam.predict(image=image_path, text_prompt=text_prompt, box_threshold=0.24, text_threshold=0.3, output=labels_path)
                 print(f'- Saving segmented image...')
@@ -386,15 +405,15 @@
             print(lines[-1])
             exit()
 
         print(f'Writing the segmented point cloud to {save_path}...')
 
         header = laspy.LasHeader(point_format=3, version="1.3")
         lidar = laspy.LasData(header=header)
-        
+
         if ground is not None:
             indices = np.concatenate((non_ground, ground))
             lidar.xyz = points[indices]
             segment_ids = np.append(segment_ids, np.full(len(ground), -1))
             lidar.add_extra_dim(laspy.ExtraBytesParams(name="segment_id", type=np.int32))
             lidar.segment_id = segment_ids
         else:
```

### Comparing `segment-lidar-0.1.7/segment_lidar.egg-info/PKG-INFO` & `segment-lidar-0.1.8/segment_lidar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-lidar
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.
 Home-page: https://github.com/Yarroudh/segment-lidar
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `segment-lidar-0.1.7/setup.py` & `segment-lidar-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         except ImportError:
             subprocess.call(['pip', 'install', 'git+https://github.com/jianboqi/CSF.git'])
         from samgeo import SamGeo
         from samgeo.text_sam import LangSAM
 
 setup(
     name="segment-lidar",
-    version='0.1.7',
+    version='0.1.8',
     description="A package for segmenting LiDAR data using Segment-Anything Model (SAM) from Meta AI Research.",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license='BSD 3-Clause "New" or "Revised" License',
     author='Anass Yarroudh',
     author_email='ayarroudh@uliege.be',
     url='https://github.com/Yarroudh/segment-lidar',
```

