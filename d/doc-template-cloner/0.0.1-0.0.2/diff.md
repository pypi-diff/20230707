# Comparing `tmp/doc_template_cloner-0.0.1.tar.gz` & `tmp/doc_template_cloner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml_services/doc_template_cloner/dist/.tmp-rg_rrjml/doc_template_cloner-0.0.1.tar", last modified: Thu Jan 19 16:08:29 2023, max compression
+gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-j8x37w4i/doc_template_cloner-0.0.2.tar", last modified: Thu Jul  6 15:45:55 2023, max compression
```

## Comparing `doc_template_cloner-0.0.1.tar` & `doc_template_cloner-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-01-19 16:08:29.177557 doc_template_cloner-0.0.1/
--rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.1/LICENSE
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-01-19 16:08:29.177287 doc_template_cloner-0.0.1/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.1/README.md
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-01-19 16:08:29.175444 doc_template_cloner-0.0.1/doc_template_cloner/
--rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.1/doc_template_cloner/__init__.py
--rw-r--r--   0 ihor       (501) staff       (20)    11597 2023-01-19 14:38:26.000000 doc_template_cloner-0.0.1/doc_template_cloner/utils.py
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-01-19 16:08:29.176949 doc_template_cloner-0.0.1/doc_template_cloner.egg-info/
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-01-19 16:08:29.000000 doc_template_cloner-0.0.1/doc_template_cloner.egg-info/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      301 2023-01-19 16:08:29.000000 doc_template_cloner-0.0.1/doc_template_cloner.egg-info/SOURCES.txt
--rw-r--r--   0 ihor       (501) staff       (20)        1 2023-01-19 16:08:29.000000 doc_template_cloner-0.0.1/doc_template_cloner.egg-info/dependency_links.txt
--rw-r--r--   0 ihor       (501) staff       (20)        7 2023-01-19 16:08:29.000000 doc_template_cloner-0.0.1/doc_template_cloner.egg-info/requires.txt
--rw-r--r--   0 ihor       (501) staff       (20)       35 2023-01-19 16:08:29.000000 doc_template_cloner-0.0.1/doc_template_cloner.egg-info/top_level.txt
--rw-r--r--   0 ihor       (501) staff       (20)       38 2023-01-19 16:08:29.177644 doc_template_cloner-0.0.1/setup.cfg
--rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-01-19 16:06:42.000000 doc_template_cloner-0.0.1/setup.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-06 15:45:54.998967 doc_template_cloner-0.0.2/
+-rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.2/LICENSE
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-06 15:45:54.998448 doc_template_cloner-0.0.2/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.2/README.md
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-06 15:45:54.994743 doc_template_cloner-0.0.2/doc_template_cloner/
+-rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.2/doc_template_cloner/__init__.py
+-rw-r--r--   0 ihor       (501) staff       (20)    15189 2023-07-05 17:16:54.000000 doc_template_cloner-0.0.2/doc_template_cloner/utils.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-06 15:45:54.997842 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-06 15:45:54.000000 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-06 15:45:54.000000 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/SOURCES.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-06 15:45:54.000000 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/dependency_links.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-06 15:45:54.000000 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/requires.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-06 15:45:54.000000 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/top_level.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-06 15:45:54.999176 doc_template_cloner-0.0.2/setup.cfg
+-rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-06 15:45:41.000000 doc_template_cloner-0.0.2/setup.py
```

### Comparing `doc_template_cloner-0.0.1/LICENSE` & `doc_template_cloner-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doc_template_cloner-0.0.1/PKG-INFO` & `doc_template_cloner-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc_template_cloner
-Version: 0.0.1
+Version: 0.0.2
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.1/doc_template_cloner/utils.py` & `doc_template_cloner-0.0.2/doc_template_cloner/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,22 +8,26 @@
 from matplotlib import pyplot as plt
 
 
 def find_intersected(target_box, boxes, threadhold=0.0):
     """looks for intersected boxes with target_box"""
     matched_boxes=[]
     
-    for box in boxes:
-        area = bops.box_iou(torch.tensor([box], dtype=torch.float), torch.tensor([target_box], dtype=torch.float))
-        area_a = bops.box_area(torch.tensor([box], dtype=torch.float))
-        area_b = bops.box_area(torch.tensor([target_box], dtype=torch.float))
-        res = area/(1+area)*(area_a+area_b)
-        area = res/min([area_a,area_b])
-        if area>threadhold:
-            matched_boxes.append((box,area))
+    try:
+        for box in boxes:
+            area = bops.box_iou(torch.tensor([box], dtype=torch.float), torch.tensor([target_box], dtype=torch.float))
+            area_a = bops.box_area(torch.tensor([box], dtype=torch.float))
+            area_b = bops.box_area(torch.tensor([target_box], dtype=torch.float))
+            res = area/(1+area)*(area_a+area_b)
+            area = res/min([area_a,area_b])
+            if area>threadhold:
+                matched_boxes.append((box,area))
+    except Exception as exception:
+        print(f'Error find_intersected: {exception}')
+        print(target_box, boxes)
     
     matched_boxes = sorted(matched_boxes, key=lambda tup: tup[1])
     
     #if len(matched_boxes)>0:
     #    return matched_boxes[-1][0]
                 
     return matched_boxes
@@ -56,14 +60,15 @@
     if anchor_x>=box[2]:
         relation.append('left')
         
     return relation
 
 
 def relative_box(anchor_point, box, is_relative=True):
+    # Calculates relative coordinates of box with respect to anchor_point.
     if is_relative:
         return [
             box[0]-anchor_point[0],
             box[1]-anchor_point[1],
             box[2]-anchor_point[0],
             box[3]-anchor_point[1]
                 ]
@@ -184,28 +189,28 @@
     _,score,_,point = cv2.minMaxLoc(res)
     
     found_box = None
     
     if score<threshold:
         print('Segment not found')
         plt.imshow(Image.fromarray(static_crop_cv2))
-        raise
+        return None
     
     loc = [point]
     
     if len(loc)==0:
         print('Segment not found')
         plt.imshow(Image.fromarray(static_crop_cv2))
         #cv2.imshow(static_crop_cv2)
-        raise
+        return None
     elif len(loc)>1:
         print('Segment found multiple times')
         print(loc)
         plt.imshow(Image.fromarray(static_crop_cv2))
-        raise
+        return None
     else:    
         #print('Segment found')
         pt = loc[0]
         tupleOfTuples = (pt, (pt[0] + h, pt[1] + w))
         found_box = list(sum(tupleOfTuples, ()))
         
     return found_box
@@ -228,128 +233,197 @@
     result = [max(box1[0],box2[0]),max(box1[1],box2[1]),min(box1[2],box2[2]),min(box1[3],box2[3])]
     
     return result
 
 
 def clone_labels(source_image, 
                  target_image, 
-                 relation_bboxes_ll, 
-                 statis_bboxes_ll, 
-                 variable_one_bboxes_ll, 
-                 variable_many_bboxes_ll):
+                 relation_bboxes_source, 
+                 statis_bboxes_source, 
+                 variable_one_bboxes_source, 
+                 variable_many_bboxes_source,
+                 labeled_boxes_source=None,
+                 threshold=0.85):
     target_image_cv2 = cv2.cvtColor(np.array(target_image), cv2.COLOR_RGB2BGR)
     
     relation_boxes = []
     variable_one_boxes = []
-    static_boxes = []
     variable_many_boxes = []
+    labeled_boxes = []
+    
+    static_boxes_target = clone_static(source_image, 
+                                target_image_cv2, 
+                                statis_bboxes_source,
+                                threshold=threshold)
 
-    for relation_bbox_source in relation_bboxes_ll:
-        relation_boxes_, static_boxes_, variable_one_boxes_, variable_many_boxes_ = clone_relation(relation_bbox_source, 
+    for relation_bbox_source in relation_bboxes_source:
+        relation_boxes_, static_boxes_, variable_one_boxes_, variable_many_boxes_, labeled_boxes_target = clone_relation(relation_bbox_source, 
                            source_image, 
                            target_image_cv2, 
-                           statis_bboxes_ll, 
-                           variable_one_bboxes_ll, 
-                           variable_many_bboxes_ll)
+                           statis_bboxes_source, 
+                           static_boxes_target,
+                           variable_one_bboxes_source, 
+                           variable_many_bboxes_source,
+                           labeled_boxes_source,
+                           threshold)
         
         relation_boxes.extend(relation_boxes_)
-        static_boxes.extend(static_boxes_)
+        #static_boxes_target.extend(static_boxes_)
         variable_many_boxes.extend(variable_many_boxes_)
         variable_one_boxes.extend(variable_one_boxes_)
+        labeled_boxes.extend(labeled_boxes_target)
         
     relation_boxes = merge_boxes(relation_boxes)
-    static_boxes = merge_boxes(static_boxes)
+    #static_boxes_target = merge_boxes(static_boxes_target)
     variable_one_boxes = merge_boxes(variable_one_boxes)
     variable_many_boxes = merge_boxes(variable_many_boxes)
+    labeled_boxes = merge_boxes(labeled_boxes)
     
-    return relation_boxes, static_boxes, variable_one_boxes, variable_many_boxes
+    return relation_boxes, static_boxes_target, variable_one_boxes, variable_many_boxes, labeled_boxes
 
         
 def find_bottom_edge(source_image,target_image_cv2,variable_many_bbox_source,statis_bboxes_ll):
     down_static_anchor_source = find_subboxes_by_axis('y', variable_many_bbox_source, statis_bboxes_ll, threadhold=0.5)
     down_static_anchor_source = [x for x in down_static_anchor_source if variable_many_bbox_source[3]<=x[1]+10]
     if down_static_anchor_source:
         down_static_anchor_source = down_static_anchor_source[0]
     
     if down_static_anchor_source:
         static_crop = source_image.crop(down_static_anchor_source)
         static_crop_cv2 = cv2.cvtColor(np.array(static_crop), cv2.COLOR_RGB2BGR)
         down_static_anchor_target = find_segment(static_crop_cv2, target_image_cv2, threshold = 0.85)
-            
+        
+        if not down_static_anchor_target:
+            return None   
+                  
         return down_static_anchor_target[1]
     else:  
-        return None        
+        return None       
+    
+    
+def clone_static(source_image, 
+                target_image_cv2, 
+                statis_bboxes_ll,
+                threshold=0.85):
+    
+    static_boxes = []
+    
+    #Find relation intersection with statis_bboxes
+    for static_anchor_source in statis_bboxes_ll:
+        #Find static_anchor_target
+        static_crop = source_image.crop(static_anchor_source)
+        static_crop_cv2 = cv2.cvtColor(np.array(static_crop), cv2.COLOR_RGB2BGR)
+        static_anchor_target = find_segment(static_crop_cv2, target_image_cv2, threshold = threshold)
+    
+        if static_anchor_target is None:
+            continue
+    
+        static_boxes.append(static_anchor_target) 
+    
+    return static_boxes
 
 
 def clone_relation(relation_bbox_source, 
                    source_image, 
                    target_image_cv2, 
-                   statis_bboxes_ll, 
-                   variable_one_bboxes_ll,
-                   variable_many_bboxes_ll):
-    
-    relation_boxes = []
-    static_boxes = []
-    variable_many_boxes = []
-    variable_one_boxes=[]
+                   statis_bboxes_source, 
+                   static_boxes_target,
+                   variable_one_bboxes_source,
+                   variable_many_bboxes_source,
+                   labeled_boxes_source=None,
+                   threshold=0.85):
+    
+    relation_boxes_target = []
+    #static_boxes_target = []
+    variable_many_boxes_target = []
+    variable_one_boxes_target=[]
+    labeled_boxes_target=[]
     
     #Find relation intersection with statis_bboxes
-    static_anchor_source = find_intersected(relation_bbox_source, statis_bboxes_ll,0.1)
+    static_anchor_source = find_intersected(relation_bbox_source, statis_bboxes_source,0.1)
     
+    #Shold be no more then one intersection
     if len(static_anchor_source)>1:
         print('Many static_anchor_source')
         raise
     
     #Find static_anchor_target
     static_anchor_source = static_anchor_source[0][0]
     static_crop = source_image.crop(static_anchor_source)
     static_crop_cv2 = cv2.cvtColor(np.array(static_crop), cv2.COLOR_RGB2BGR)
-    static_anchor_target = find_segment(static_crop_cv2, target_image_cv2, threshold = 0.85)
+    static_anchor_target = find_segment(static_crop_cv2, target_image_cv2, threshold = threshold)
     
+    #If not found, return empty lists
     if static_anchor_target is None:
-        return relation_boxes, static_boxes, variable_one_boxes, variable_many_boxes
-    
-    static_boxes.append(static_anchor_target)
+        return relation_boxes_target, [], variable_one_boxes_target, variable_many_boxes_target, labeled_boxes_target
+    #static_boxes_target.append(static_anchor_target)
     
     #Find relation_bbox_target
     relation_bbox_target = relative_box(static_anchor_target,relative_box(static_anchor_source,relation_bbox_source),is_relative=False) 
     
     #Find relation intersection with variable_many_bboxes
-    variable_many_bbox_source = find_intersected(relation_bbox_source, variable_many_bboxes_ll,0.1)
+    variable_many_bbox_source = find_intersected(relation_bbox_source, variable_many_bboxes_source,0.1)
     
     if len(variable_many_bbox_source)>1:
         print('Many variable_many_bbox_source')
         raise
     
+    # apply logic to variable many case
     if variable_many_bbox_source:
         variable_many_bbox_source = variable_many_bbox_source[0][0]
         
         static_in_relation_source = get_intersection(static_anchor_source,relation_bbox_source)
         variable_in_relation_source = get_intersection(variable_many_bbox_source,relation_bbox_source)
         orientation = get_relative_orientation(static_in_relation_source,variable_in_relation_source)
 
         if 'down' in orientation:
             variable_many_bbox_target = relative_box(static_anchor_target,relative_box(static_anchor_source,variable_many_bbox_source),is_relative=False)
             
-            bottom_edge = find_bottom_edge(source_image,target_image_cv2,variable_many_bbox_source,statis_bboxes_ll)
+            bottom_edge = find_bottom_edge(source_image,target_image_cv2,variable_many_bbox_source,statis_bboxes_source)
             
             if bottom_edge is None:
-                bottom_edge = find_bottom_edge(source_image,target_image_cv2,variable_many_bbox_source,variable_one_bboxes_ll)
+                bottom_edge = find_bottom_edge(source_image,target_image_cv2,variable_many_bbox_source,variable_one_bboxes_source)
                 
                 if bottom_edge is None:
                     bottom_edge = variable_many_bbox_target[3] + 100
+                    
+            down_static_anchor_target = find_subboxes_by_axis('y', variable_many_bbox_target, static_boxes_target, threadhold=0.5)
+            down_static_anchor_target = [x for x in down_static_anchor_target if variable_many_bbox_target[3]<=x[1]+10]
+            if down_static_anchor_target:
+                down_static_anchor_target = down_static_anchor_target[0]
+                
+                bottom_edge = min(bottom_edge,down_static_anchor_target[1])
+            
             
             variable_many_bbox_target[3] = bottom_edge
             relation_bbox_target[3] = bottom_edge              
-            variable_many_boxes.append(variable_many_bbox_target)
+            variable_many_boxes_target.append(variable_many_bbox_target)
             
-    relation_boxes.append(relation_bbox_target)
+            if labeled_boxes_source:
+                labeled_boxes = find_intersected(variable_many_bbox_source, labeled_boxes_source,0.1)
+            
+                for labeled_box in labeled_boxes:
+                    labeled_box = labeled_box[0]
+                    labeled_box_target = relative_box(variable_many_bbox_target,relative_box(variable_many_bbox_source,labeled_box),is_relative=False) 
+                    labeled_box_target[3] = bottom_edge       
+                    labeled_boxes_target.append(labeled_box_target)  
+
+            
+    relation_boxes_target.append(relation_bbox_target)
     
-    #Find relation intersection with variable_many_bboxes
-    variable_one_bbox_source = find_intersected(relation_bbox_source, variable_one_bboxes_ll,0.1)
+    #Find relation intersection with variable_one_bboxes_source
+    variable_one_bbox_source = find_intersected(relation_bbox_source, variable_one_bboxes_source,0.1)
     
     for variable_one_bbox in variable_one_bbox_source:
         variable_one_bbox = variable_one_bbox[0]
         variable_one_bbox_target = relative_box(static_anchor_target,relative_box(static_anchor_source,variable_one_bbox),is_relative=False) 
-        variable_one_boxes.append(variable_one_bbox_target)  
+        variable_one_boxes_target.append(variable_one_bbox_target)  
+        
+        if labeled_boxes_source:
+            labeled_boxes = find_intersected(variable_one_bbox, labeled_boxes_source,0.1)
+            
+            for labeled_box in labeled_boxes:
+                labeled_box = labeled_box[0]
+                labeled_box_target = relative_box(variable_one_bbox_target,relative_box(variable_one_bbox,labeled_box),is_relative=False) 
+                labeled_boxes_target.append(labeled_box_target)  
     
-    return relation_boxes, static_boxes, variable_one_boxes, variable_many_boxes
+    return relation_boxes_target, [], variable_one_boxes_target, variable_many_boxes_target, labeled_boxes_target
```

### Comparing `doc_template_cloner-0.0.1/doc_template_cloner.egg-info/PKG-INFO` & `doc_template_cloner-0.0.2/doc_template_cloner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-template-cloner
-Version: 0.0.1
+Version: 0.0.2
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.1/setup.py` & `doc_template_cloner-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 required_packages = [
     #"boto3>=1.20.21,<2.0",
     "pandas",
 ]
 
 setup(
     name="doc_template_cloner",
-    version="0.0.1",
+    version="0.0.2",
     description="Custom lib to clone lebaling from one image to another similar",
     long_description_content_type="text/markdown",
     long_description=read('README.md'),
     packages=find_packages(),
     py_modules=[os.path.splitext(os.path.basename(path))[0] for path in glob("doc_template_cloner/*.py")],
     include_package_data=True,
     author="Ihor Bilyk",
```

