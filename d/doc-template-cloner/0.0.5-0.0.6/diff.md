# Comparing `tmp/doc_template_cloner-0.0.5.tar.gz` & `tmp/doc_template_cloner-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-8b2njtl8/doc_template_cloner-0.0.5.tar", last modified: Fri Jul  7 11:17:38 2023, max compression
+gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-rztfnmpu/doc_template_cloner-0.0.6.tar", last modified: Fri Jul  7 11:27:21 2023, max compression
```

## Comparing `doc_template_cloner-0.0.5.tar` & `doc_template_cloner-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:17:38.959798 doc_template_cloner-0.0.5/
--rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.5/LICENSE
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:17:38.959435 doc_template_cloner-0.0.5/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.5/README.md
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:17:38.956912 doc_template_cloner-0.0.5/doc_template_cloner/
--rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.5/doc_template_cloner/__init__.py
--rw-r--r--   0 ihor       (501) staff       (20)    15708 2023-07-07 11:17:23.000000 doc_template_cloner-0.0.5/doc_template_cloner/utils.py
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:17:38.958995 doc_template_cloner-0.0.5/doc_template_cloner.egg-info/
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:17:38.000000 doc_template_cloner-0.0.5/doc_template_cloner.egg-info/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-07 11:17:38.000000 doc_template_cloner-0.0.5/doc_template_cloner.egg-info/SOURCES.txt
--rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-07 11:17:38.000000 doc_template_cloner-0.0.5/doc_template_cloner.egg-info/dependency_links.txt
--rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-07 11:17:38.000000 doc_template_cloner-0.0.5/doc_template_cloner.egg-info/requires.txt
--rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-07 11:17:38.000000 doc_template_cloner-0.0.5/doc_template_cloner.egg-info/top_level.txt
--rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-07 11:17:38.959908 doc_template_cloner-0.0.5/setup.cfg
--rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-07 11:17:32.000000 doc_template_cloner-0.0.5/setup.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:27:21.358814 doc_template_cloner-0.0.6/
+-rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.6/LICENSE
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:27:21.358248 doc_template_cloner-0.0.6/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.6/README.md
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:27:21.355713 doc_template_cloner-0.0.6/doc_template_cloner/
+-rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.6/doc_template_cloner/__init__.py
+-rw-r--r--   0 ihor       (501) staff       (20)    16089 2023-07-07 11:27:01.000000 doc_template_cloner-0.0.6/doc_template_cloner/utils.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:27:21.357729 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:27:21.000000 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-07 11:27:21.000000 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/SOURCES.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-07 11:27:21.000000 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/dependency_links.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-07 11:27:21.000000 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/requires.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-07 11:27:21.000000 doc_template_cloner-0.0.6/doc_template_cloner.egg-info/top_level.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-07 11:27:21.358947 doc_template_cloner-0.0.6/setup.cfg
+-rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-07 11:27:15.000000 doc_template_cloner-0.0.6/setup.py
```

### Comparing `doc_template_cloner-0.0.5/LICENSE` & `doc_template_cloner-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `doc_template_cloner-0.0.5/PKG-INFO` & `doc_template_cloner-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc_template_cloner
-Version: 0.0.5
+Version: 0.0.6
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.5/doc_template_cloner/utils.py` & `doc_template_cloner-0.0.6/doc_template_cloner/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,15 +344,15 @@
     
     #Find relation intersection with statis_bboxes
     static_anchor_source = find_intersected(relation_bbox_source, statis_bboxes_source,0.1)
     
     #Shold be no more then one intersection
     if len(static_anchor_source)>1:
         print('Many static_anchor_source')
-        raise
+        return None
     
     #Find static_anchor_target
     static_anchor_source = static_anchor_source[0][0]
     static_crop = source_image.crop(static_anchor_source)
     static_crop_cv2 = cv2.cvtColor(np.array(static_crop), cv2.COLOR_RGB2BGR)
     static_anchor_target = find_segment(static_crop_cv2, target_image_cv2, threshold = threshold)
     
@@ -361,75 +361,78 @@
         return relation_boxes_target, [], variable_one_boxes_target, variable_many_boxes_target, labeled_boxes_target
     #static_boxes_target.append(static_anchor_target)
     
     #Find relation_bbox_target
     relation_bbox_target = relative_box(static_anchor_target,relative_box(static_anchor_source,relation_bbox_source),is_relative=False) 
     
     #Find relation intersection with variable_many_bboxes
-    variable_many_bbox_source = find_intersected(relation_bbox_source, variable_many_bboxes_source,0.1)
-    
-    if len(variable_many_bbox_source)>1:
-        print('Many variable_many_bbox_source')
-        raise
-    
-    # apply logic to variable many case
-    if variable_many_bbox_source:
-        variable_many_bbox_source = variable_many_bbox_source[0][0]
+    if variable_many_bboxes_source:
+        variable_many_bbox_source = find_intersected(relation_bbox_source, variable_many_bboxes_source,0.1)
+        
+        if len(variable_many_bbox_source)>1:
+            print('Many variable_many_bbox_source')
+            return None
         
-        static_in_relation_source = get_intersection(static_anchor_source,relation_bbox_source)
-        variable_in_relation_source = get_intersection(variable_many_bbox_source,relation_bbox_source)
-        orientation = get_relative_orientation(static_in_relation_source,variable_in_relation_source)
+        # apply logic to variable many case
+        if variable_many_bbox_source:
+            variable_many_bbox_source = variable_many_bbox_source[0][0]
+            
+            static_in_relation_source = get_intersection(static_anchor_source,relation_bbox_source)
+            variable_in_relation_source = get_intersection(variable_many_bbox_source,relation_bbox_source)
+            orientation = get_relative_orientation(static_in_relation_source,variable_in_relation_source)
 
-        if 'down' in orientation:
-            variable_many_bbox_target = relative_box(static_anchor_target,relative_box(static_anchor_source,variable_many_bbox_source),is_relative=False)
-            
-            bottom_edge = find_bottom_edge(source_image,target_image_cv2,variable_many_bbox_source,statis_bboxes_source)
-            
-            if bottom_edge is None:
-                bottom_edge = find_bottom_edge(source_image,target_image_cv2,variable_many_bbox_source,variable_one_bboxes_source)
+            if 'down' in orientation:
+                variable_many_bbox_target = relative_box(static_anchor_target,relative_box(static_anchor_source,variable_many_bbox_source),is_relative=False)
+                
+                bottom_edge = find_bottom_edge(source_image,target_image_cv2,variable_many_bbox_source,statis_bboxes_source)
                 
                 if bottom_edge is None:
-                    bottom_edge = variable_many_bbox_target[3] + 100
+                    bottom_edge = find_bottom_edge(source_image,target_image_cv2,variable_many_bbox_source,variable_one_bboxes_source)
                     
-            down_static_anchor_target = find_subboxes_by_axis('y', variable_many_bbox_target, static_boxes_target, threadhold=0.5)
-            down_static_anchor_target = [x for x in down_static_anchor_target if variable_many_bbox_target[3]<=x[1]+10]
-            if down_static_anchor_target:
-                down_static_anchor_target = down_static_anchor_target[0]
-                
-                bottom_edge = min(bottom_edge,down_static_anchor_target[1])
-            
-            
-            variable_many_bbox_target[3] = bottom_edge
-            relation_bbox_target[3] = bottom_edge              
-            variable_many_boxes_target.append(variable_many_bbox_target)
-            
-            if labeled_boxes_source:
-                labeled_boxes_source_list = [eval(x) for x in labeled_boxes_source.keys()]
-                intersected_labeled_boxes_list = find_intersected(variable_many_bbox_source, labeled_boxes_source_list,0.1)
-            
-                for labeled_box in intersected_labeled_boxes_list:
-                    labeled_box = labeled_box[0]
+                    if bottom_edge is None:
+                        bottom_edge = variable_many_bbox_target[3] + 100
+                        
+                down_static_anchor_target = find_subboxes_by_axis('y', variable_many_bbox_target, static_boxes_target, threadhold=0.5)
+                down_static_anchor_target = [x for x in down_static_anchor_target if variable_many_bbox_target[3]<=x[1]+10]
+                if down_static_anchor_target:
+                    down_static_anchor_target = down_static_anchor_target[0]
                     
-                    labeled_box_target = relative_box(variable_many_bbox_target,relative_box(variable_many_bbox_source,labeled_box),is_relative=False) 
-                    labeled_box_target[3] = bottom_edge       
-                    labeled_boxes_target[str(labeled_box_target)] = labeled_boxes_source[str(labeled_box)]
+                    bottom_edge = min(bottom_edge,down_static_anchor_target[1])
+                
+                
+                variable_many_bbox_target[3] = bottom_edge
+                relation_bbox_target[3] = bottom_edge              
+                variable_many_boxes_target.append(variable_many_bbox_target)
+                
+                if labeled_boxes_source:
+                    labeled_boxes_source_list = [eval(x) for x in labeled_boxes_source.keys()]
+                    intersected_labeled_boxes_list = find_intersected(variable_many_bbox_source, labeled_boxes_source_list,0.1)
+                
+                    for labeled_box in intersected_labeled_boxes_list:
+                        labeled_box = labeled_box[0]
+                        
+                        labeled_box_target = relative_box(variable_many_bbox_target,relative_box(variable_many_bbox_source,labeled_box),is_relative=False) 
+                        labeled_box_target[3] = bottom_edge       
+                        labeled_boxes_target[str(labeled_box_target)] = labeled_boxes_source[str(labeled_box)]
             
     relation_boxes_target.append(relation_bbox_target)
     
     #Find relation intersection with variable_one_bboxes_source
     variable_one_bbox_source = find_intersected(relation_bbox_source, variable_one_bboxes_source,0.1)
     
+    print('variable_one_bbox_source:',variable_one_bbox_source)
     for variable_one_bbox in variable_one_bbox_source:
         variable_one_bbox = variable_one_bbox[0]
         variable_one_bbox_target = relative_box(static_anchor_target,relative_box(static_anchor_source,variable_one_bbox),is_relative=False) 
         variable_one_boxes_target.append(variable_one_bbox_target)  
         
         if labeled_boxes_source:
             labeled_boxes_source_list = [eval(x) for x in labeled_boxes_source.keys()]
             intersected_labeled_boxes_list = find_intersected(variable_one_bbox, labeled_boxes_source_list,0.1)
             
+            print('intersected_labeled_boxes_list:', intersected_labeled_boxes_list)
             for labeled_box in intersected_labeled_boxes_list:
                 labeled_box = labeled_box[0]
                 labeled_box_target = relative_box(variable_one_bbox_target,relative_box(variable_one_bbox,labeled_box),is_relative=False) 
                 labeled_boxes_target[str(labeled_box_target)] = labeled_boxes_source[str(labeled_box)]
     
     return relation_boxes_target, [], variable_one_boxes_target, variable_many_boxes_target, labeled_boxes_target
```

### Comparing `doc_template_cloner-0.0.5/doc_template_cloner.egg-info/PKG-INFO` & `doc_template_cloner-0.0.6/doc_template_cloner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-template-cloner
-Version: 0.0.5
+Version: 0.0.6
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.5/setup.py` & `doc_template_cloner-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 required_packages = [
     #"boto3>=1.20.21,<2.0",
     "pandas",
 ]
 
 setup(
     name="doc_template_cloner",
-    version="0.0.5",
+    version="0.0.6",
     description="Custom lib to clone lebaling from one image to another similar",
     long_description_content_type="text/markdown",
     long_description=read('README.md'),
     packages=find_packages(),
     py_modules=[os.path.splitext(os.path.basename(path))[0] for path in glob("doc_template_cloner/*.py")],
     include_package_data=True,
     author="Ihor Bilyk",
```

