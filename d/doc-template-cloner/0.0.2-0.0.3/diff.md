# Comparing `tmp/doc_template_cloner-0.0.2.tar.gz` & `tmp/doc_template_cloner-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-j8x37w4i/doc_template_cloner-0.0.2.tar", last modified: Thu Jul  6 15:45:55 2023, max compression
+gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-pgvj8w_8/doc_template_cloner-0.0.3.tar", last modified: Fri Jul  7 10:08:08 2023, max compression
```

## Comparing `doc_template_cloner-0.0.2.tar` & `doc_template_cloner-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-06 15:45:54.998967 doc_template_cloner-0.0.2/
--rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.2/LICENSE
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-06 15:45:54.998448 doc_template_cloner-0.0.2/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.2/README.md
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-06 15:45:54.994743 doc_template_cloner-0.0.2/doc_template_cloner/
--rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.2/doc_template_cloner/__init__.py
--rw-r--r--   0 ihor       (501) staff       (20)    15189 2023-07-05 17:16:54.000000 doc_template_cloner-0.0.2/doc_template_cloner/utils.py
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-06 15:45:54.997842 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-06 15:45:54.000000 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-06 15:45:54.000000 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/SOURCES.txt
--rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-06 15:45:54.000000 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/dependency_links.txt
--rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-06 15:45:54.000000 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/requires.txt
--rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-06 15:45:54.000000 doc_template_cloner-0.0.2/doc_template_cloner.egg-info/top_level.txt
--rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-06 15:45:54.999176 doc_template_cloner-0.0.2/setup.cfg
--rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-06 15:45:41.000000 doc_template_cloner-0.0.2/setup.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 10:08:08.940310 doc_template_cloner-0.0.3/
+-rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.3/LICENSE
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 10:08:08.940039 doc_template_cloner-0.0.3/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.3/README.md
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 10:08:08.937770 doc_template_cloner-0.0.3/doc_template_cloner/
+-rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.3/doc_template_cloner/__init__.py
+-rw-r--r--   0 ihor       (501) staff       (20)    15614 2023-07-07 10:07:39.000000 doc_template_cloner-0.0.3/doc_template_cloner/utils.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 10:08:08.939668 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 10:08:08.000000 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-07 10:08:08.000000 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/SOURCES.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-07 10:08:08.000000 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/dependency_links.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-07 10:08:08.000000 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/requires.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-07 10:08:08.000000 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/top_level.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-07 10:08:08.940403 doc_template_cloner-0.0.3/setup.cfg
+-rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-07 10:08:00.000000 doc_template_cloner-0.0.3/setup.py
```

### Comparing `doc_template_cloner-0.0.2/LICENSE` & `doc_template_cloner-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `doc_template_cloner-0.0.2/PKG-INFO` & `doc_template_cloner-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc_template_cloner
-Version: 0.0.2
+Version: 0.0.3
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.2/doc_template_cloner/utils.py` & `doc_template_cloner-0.0.3/doc_template_cloner/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,21 +266,21 @@
                            labeled_boxes_source,
                            threshold)
         
         relation_boxes.extend(relation_boxes_)
         #static_boxes_target.extend(static_boxes_)
         variable_many_boxes.extend(variable_many_boxes_)
         variable_one_boxes.extend(variable_one_boxes_)
-        labeled_boxes.extend(labeled_boxes_target)
+        labeled_boxes.append(labeled_boxes_target)
         
     relation_boxes = merge_boxes(relation_boxes)
     #static_boxes_target = merge_boxes(static_boxes_target)
     variable_one_boxes = merge_boxes(variable_one_boxes)
     variable_many_boxes = merge_boxes(variable_many_boxes)
-    labeled_boxes = merge_boxes(labeled_boxes)
+    #labeled_boxes = merge_boxes(labeled_boxes)
     
     return relation_boxes, static_boxes_target, variable_one_boxes, variable_many_boxes, labeled_boxes
 
         
 def find_bottom_edge(source_image,target_image_cv2,variable_many_bbox_source,statis_bboxes_ll):
     down_static_anchor_source = find_subboxes_by_axis('y', variable_many_bbox_source, statis_bboxes_ll, threadhold=0.5)
     down_static_anchor_source = [x for x in down_static_anchor_source if variable_many_bbox_source[3]<=x[1]+10]
@@ -328,19 +328,21 @@
                    statis_bboxes_source, 
                    static_boxes_target,
                    variable_one_bboxes_source,
                    variable_many_bboxes_source,
                    labeled_boxes_source=None,
                    threshold=0.85):
     
+    """labeled_boxes_source - dict. {'[x0,y0,x1,y1]':'label',...}"""
+    
     relation_boxes_target = []
     #static_boxes_target = []
     variable_many_boxes_target = []
     variable_one_boxes_target=[]
-    labeled_boxes_target=[]
+    labeled_boxes_target={}
     
     #Find relation intersection with statis_bboxes
     static_anchor_source = find_intersected(relation_bbox_source, statis_bboxes_source,0.1)
     
     #Shold be no more then one intersection
     if len(static_anchor_source)>1:
         print('Many static_anchor_source')
@@ -395,35 +397,37 @@
             
             
             variable_many_bbox_target[3] = bottom_edge
             relation_bbox_target[3] = bottom_edge              
             variable_many_boxes_target.append(variable_many_bbox_target)
             
             if labeled_boxes_source:
-                labeled_boxes = find_intersected(variable_many_bbox_source, labeled_boxes_source,0.1)
+                labeled_boxes_source_list = [eval(x) for x in labeled_boxes_source.keys()]
+                intersected_labeled_boxes_list = find_intersected(variable_many_bbox_source, labeled_boxes_source_list,0.1)
             
-                for labeled_box in labeled_boxes:
+                for labeled_box in intersected_labeled_boxes_list:
                     labeled_box = labeled_box[0]
+                    
                     labeled_box_target = relative_box(variable_many_bbox_target,relative_box(variable_many_bbox_source,labeled_box),is_relative=False) 
                     labeled_box_target[3] = bottom_edge       
-                    labeled_boxes_target.append(labeled_box_target)  
-
+                    labeled_boxes_target[str(labeled_box_target)] = labeled_boxes_source[str(labeled_box)]
             
     relation_boxes_target.append(relation_bbox_target)
     
     #Find relation intersection with variable_one_bboxes_source
     variable_one_bbox_source = find_intersected(relation_bbox_source, variable_one_bboxes_source,0.1)
     
     for variable_one_bbox in variable_one_bbox_source:
         variable_one_bbox = variable_one_bbox[0]
         variable_one_bbox_target = relative_box(static_anchor_target,relative_box(static_anchor_source,variable_one_bbox),is_relative=False) 
         variable_one_boxes_target.append(variable_one_bbox_target)  
         
         if labeled_boxes_source:
-            labeled_boxes = find_intersected(variable_one_bbox, labeled_boxes_source,0.1)
+            labeled_boxes_source_list = [eval(x) for x in labeled_boxes_source.keys()]
+            intersected_labeled_boxes_list = find_intersected(variable_one_bbox, labeled_boxes_source_list,0.1)
             
-            for labeled_box in labeled_boxes:
+            for labeled_box in intersected_labeled_boxes_list:
                 labeled_box = labeled_box[0]
                 labeled_box_target = relative_box(variable_one_bbox_target,relative_box(variable_one_bbox,labeled_box),is_relative=False) 
-                labeled_boxes_target.append(labeled_box_target)  
+                labeled_boxes_target[str(labeled_box_target)] = labeled_boxes_source[str(labeled_box)]
     
     return relation_boxes_target, [], variable_one_boxes_target, variable_many_boxes_target, labeled_boxes_target
```

### Comparing `doc_template_cloner-0.0.2/doc_template_cloner.egg-info/PKG-INFO` & `doc_template_cloner-0.0.3/doc_template_cloner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-template-cloner
-Version: 0.0.2
+Version: 0.0.3
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.2/setup.py` & `doc_template_cloner-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 required_packages = [
     #"boto3>=1.20.21,<2.0",
     "pandas",
 ]
 
 setup(
     name="doc_template_cloner",
-    version="0.0.2",
+    version="0.0.3",
     description="Custom lib to clone lebaling from one image to another similar",
     long_description_content_type="text/markdown",
     long_description=read('README.md'),
     packages=find_packages(),
     py_modules=[os.path.splitext(os.path.basename(path))[0] for path in glob("doc_template_cloner/*.py")],
     include_package_data=True,
     author="Ihor Bilyk",
```

