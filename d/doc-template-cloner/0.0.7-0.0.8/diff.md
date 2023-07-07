# Comparing `tmp/doc_template_cloner-0.0.7.tar.gz` & `tmp/doc_template_cloner-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-6mb5mzwz/doc_template_cloner-0.0.7.tar", last modified: Fri Jul  7 11:46:05 2023, max compression
+gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-kyfz_ayi/doc_template_cloner-0.0.8.tar", last modified: Fri Jul  7 13:27:32 2023, max compression
```

## Comparing `doc_template_cloner-0.0.7.tar` & `doc_template_cloner-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:46:05.057556 doc_template_cloner-0.0.7/
--rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.7/LICENSE
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:46:05.057272 doc_template_cloner-0.0.7/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.7/README.md
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:46:05.054996 doc_template_cloner-0.0.7/doc_template_cloner/
--rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.7/doc_template_cloner/__init__.py
--rw-r--r--   0 ihor       (501) staff       (20)    16089 2023-07-07 11:27:01.000000 doc_template_cloner-0.0.7/doc_template_cloner/utils.py
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:46:05.056754 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:46:05.000000 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-07 11:46:05.000000 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/SOURCES.txt
--rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-07 11:46:05.000000 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/dependency_links.txt
--rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-07 11:46:05.000000 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/requires.txt
--rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-07 11:46:05.000000 doc_template_cloner-0.0.7/doc_template_cloner.egg-info/top_level.txt
--rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-07 11:46:05.057648 doc_template_cloner-0.0.7/setup.cfg
--rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-07 11:45:59.000000 doc_template_cloner-0.0.7/setup.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 13:27:32.876094 doc_template_cloner-0.0.8/
+-rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.8/LICENSE
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 13:27:32.875834 doc_template_cloner-0.0.8/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.8/README.md
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 13:27:32.873700 doc_template_cloner-0.0.8/doc_template_cloner/
+-rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.8/doc_template_cloner/__init__.py
+-rw-r--r--   0 ihor       (501) staff       (20)    16257 2023-07-07 13:26:30.000000 doc_template_cloner-0.0.8/doc_template_cloner/utils.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 13:27:32.875473 doc_template_cloner-0.0.8/doc_template_cloner.egg-info/
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 13:27:32.000000 doc_template_cloner-0.0.8/doc_template_cloner.egg-info/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-07 13:27:32.000000 doc_template_cloner-0.0.8/doc_template_cloner.egg-info/SOURCES.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-07 13:27:32.000000 doc_template_cloner-0.0.8/doc_template_cloner.egg-info/dependency_links.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-07 13:27:32.000000 doc_template_cloner-0.0.8/doc_template_cloner.egg-info/requires.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-07 13:27:32.000000 doc_template_cloner-0.0.8/doc_template_cloner.egg-info/top_level.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-07 13:27:32.876182 doc_template_cloner-0.0.8/setup.cfg
+-rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-07 13:27:26.000000 doc_template_cloner-0.0.8/setup.py
```

### Comparing `doc_template_cloner-0.0.7/LICENSE` & `doc_template_cloner-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `doc_template_cloner-0.0.7/PKG-INFO` & `doc_template_cloner-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc_template_cloner
-Version: 0.0.7
+Version: 0.0.8
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.7/doc_template_cloner/utils.py` & `doc_template_cloner-0.0.8/doc_template_cloner/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,16 @@
         
         if len(variable_many_bbox_source)>1:
             print('Many variable_many_bbox_source')
             return None
         
         # apply logic to variable many case
         if variable_many_bbox_source:
+            print('variable_many_bbox_source:',variable_many_bbox_source)
+
             variable_many_bbox_source = variable_many_bbox_source[0][0]
             
             static_in_relation_source = get_intersection(static_anchor_source,relation_bbox_source)
             variable_in_relation_source = get_intersection(variable_many_bbox_source,relation_bbox_source)
             orientation = get_relative_orientation(static_in_relation_source,variable_in_relation_source)
 
             if 'down' in orientation:
@@ -415,24 +417,25 @@
                         labeled_boxes_target[str(labeled_box_target)] = labeled_boxes_source[str(labeled_box)]
             
     relation_boxes_target.append(relation_bbox_target)
     
     #Find relation intersection with variable_one_bboxes_source
     variable_one_bbox_source = find_intersected(relation_bbox_source, variable_one_bboxes_source,0.1)
     
-    print('variable_one_bbox_source:',variable_one_bbox_source)
-    for variable_one_bbox in variable_one_bbox_source:
-        variable_one_bbox = variable_one_bbox[0]
-        variable_one_bbox_target = relative_box(static_anchor_target,relative_box(static_anchor_source,variable_one_bbox),is_relative=False) 
-        variable_one_boxes_target.append(variable_one_bbox_target)  
-        
-        if labeled_boxes_source:
-            labeled_boxes_source_list = [eval(x) for x in labeled_boxes_source.keys()]
-            intersected_labeled_boxes_list = find_intersected(variable_one_bbox, labeled_boxes_source_list,0.1)
+    if variable_one_bbox_source:
+        print('variable_one_bbox_source:',variable_one_bbox_source)
+        for variable_one_bbox in variable_one_bbox_source:
+            variable_one_bbox = variable_one_bbox[0]
+            variable_one_bbox_target = relative_box(static_anchor_target,relative_box(static_anchor_source,variable_one_bbox),is_relative=False) 
+            variable_one_boxes_target.append(variable_one_bbox_target)  
             
-            print('intersected_labeled_boxes_list:', intersected_labeled_boxes_list)
-            for labeled_box in intersected_labeled_boxes_list:
-                labeled_box = labeled_box[0]
-                labeled_box_target = relative_box(variable_one_bbox_target,relative_box(variable_one_bbox,labeled_box),is_relative=False) 
-                labeled_boxes_target[str(labeled_box_target)] = labeled_boxes_source[str(labeled_box)]
+            if labeled_boxes_source:
+                labeled_boxes_source_list = [eval(x) for x in labeled_boxes_source.keys()]
+                intersected_labeled_boxes_list = find_intersected(variable_one_bbox, labeled_boxes_source_list,0.1)
+                
+                print('intersected_labeled_boxes_list:', intersected_labeled_boxes_list)
+                for labeled_box in intersected_labeled_boxes_list:
+                    labeled_box = labeled_box[0]
+                    labeled_box_target = relative_box(variable_one_bbox_target,relative_box(variable_one_bbox,labeled_box),is_relative=False) 
+                    labeled_boxes_target[str(labeled_box_target)] = labeled_boxes_source[str(labeled_box)]
     
     return relation_boxes_target, [], variable_one_boxes_target, variable_many_boxes_target, labeled_boxes_target
```

### Comparing `doc_template_cloner-0.0.7/doc_template_cloner.egg-info/PKG-INFO` & `doc_template_cloner-0.0.8/doc_template_cloner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-template-cloner
-Version: 0.0.7
+Version: 0.0.8
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.7/setup.py` & `doc_template_cloner-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 required_packages = [
     #"boto3>=1.20.21,<2.0",
     "pandas",
 ]
 
 setup(
     name="doc_template_cloner",
-    version="0.0.7",
+    version="0.0.8",
     description="Custom lib to clone lebaling from one image to another similar",
     long_description_content_type="text/markdown",
     long_description=read('README.md'),
     packages=find_packages(),
     py_modules=[os.path.splitext(os.path.basename(path))[0] for path in glob("doc_template_cloner/*.py")],
     include_package_data=True,
     author="Ihor Bilyk",
```

