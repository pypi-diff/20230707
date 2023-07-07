# Comparing `tmp/doc_template_cloner-0.0.3.tar.gz` & `tmp/doc_template_cloner-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-pgvj8w_8/doc_template_cloner-0.0.3.tar", last modified: Fri Jul  7 10:08:08 2023, max compression
+gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml-services/doc_template_cloner/dist/.tmp-zrpu4n4u/doc_template_cloner-0.0.4.tar", last modified: Fri Jul  7 11:04:53 2023, max compression
```

## Comparing `doc_template_cloner-0.0.3.tar` & `doc_template_cloner-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 10:08:08.940310 doc_template_cloner-0.0.3/
--rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.3/LICENSE
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 10:08:08.940039 doc_template_cloner-0.0.3/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.3/README.md
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 10:08:08.937770 doc_template_cloner-0.0.3/doc_template_cloner/
--rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.3/doc_template_cloner/__init__.py
--rw-r--r--   0 ihor       (501) staff       (20)    15614 2023-07-07 10:07:39.000000 doc_template_cloner-0.0.3/doc_template_cloner/utils.py
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 10:08:08.939668 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/
--rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 10:08:08.000000 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-07 10:08:08.000000 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/SOURCES.txt
--rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-07 10:08:08.000000 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/dependency_links.txt
--rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-07 10:08:08.000000 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/requires.txt
--rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-07 10:08:08.000000 doc_template_cloner-0.0.3/doc_template_cloner.egg-info/top_level.txt
--rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-07 10:08:08.940403 doc_template_cloner-0.0.3/setup.cfg
--rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-07 10:08:00.000000 doc_template_cloner-0.0.3/setup.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:04:53.595920 doc_template_cloner-0.0.4/
+-rw-r--r--   0 ihor       (501) staff       (20)    11357 2023-01-18 10:30:40.000000 doc_template_cloner-0.0.4/LICENSE
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:04:53.595642 doc_template_cloner-0.0.4/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      108 2023-01-17 12:49:21.000000 doc_template_cloner-0.0.4/README.md
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:04:53.592594 doc_template_cloner-0.0.4/doc_template_cloner/
+-rw-r--r--   0 ihor       (501) staff       (20)       21 2023-01-18 12:52:53.000000 doc_template_cloner-0.0.4/doc_template_cloner/__init__.py
+-rw-r--r--   0 ihor       (501) staff       (20)    15702 2023-07-07 11:03:56.000000 doc_template_cloner-0.0.4/doc_template_cloner/utils.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2023-07-07 11:04:53.595255 doc_template_cloner-0.0.4/doc_template_cloner.egg-info/
+-rw-r--r--   0 ihor       (501) staff       (20)      957 2023-07-07 11:04:53.000000 doc_template_cloner-0.0.4/doc_template_cloner.egg-info/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      301 2023-07-07 11:04:53.000000 doc_template_cloner-0.0.4/doc_template_cloner.egg-info/SOURCES.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        1 2023-07-07 11:04:53.000000 doc_template_cloner-0.0.4/doc_template_cloner.egg-info/dependency_links.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        7 2023-07-07 11:04:53.000000 doc_template_cloner-0.0.4/doc_template_cloner.egg-info/requires.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       35 2023-07-07 11:04:53.000000 doc_template_cloner-0.0.4/doc_template_cloner.egg-info/top_level.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       38 2023-07-07 11:04:53.596079 doc_template_cloner-0.0.4/setup.cfg
+-rw-r--r--   0 ihor       (501) staff       (20)     1490 2023-07-07 11:04:47.000000 doc_template_cloner-0.0.4/setup.py
```

### Comparing `doc_template_cloner-0.0.3/LICENSE` & `doc_template_cloner-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `doc_template_cloner-0.0.3/PKG-INFO` & `doc_template_cloner-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc_template_cloner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.3/doc_template_cloner/utils.py` & `doc_template_cloner-0.0.4/doc_template_cloner/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,24 +251,26 @@
     labeled_boxes = []
     
     static_boxes_target = clone_static(source_image, 
                                 target_image_cv2, 
                                 statis_bboxes_source,
                                 threshold=threshold)
 
+    print('Clonning relation')
     for relation_bbox_source in relation_bboxes_source:
         relation_boxes_, static_boxes_, variable_one_boxes_, variable_many_boxes_, labeled_boxes_target = clone_relation(relation_bbox_source, 
                            source_image, 
                            target_image_cv2, 
                            statis_bboxes_source, 
                            static_boxes_target,
                            variable_one_bboxes_source, 
                            variable_many_bboxes_source,
                            labeled_boxes_source,
                            threshold)
+        print(relation_bbox_source,labeled_boxes_source)
         
         relation_boxes.extend(relation_boxes_)
         #static_boxes_target.extend(static_boxes_)
         variable_many_boxes.extend(variable_many_boxes_)
         variable_one_boxes.extend(variable_one_boxes_)
         labeled_boxes.append(labeled_boxes_target)
```

### Comparing `doc_template_cloner-0.0.3/doc_template_cloner.egg-info/PKG-INFO` & `doc_template_cloner-0.0.4/doc_template_cloner.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-template-cloner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Custom lib to clone lebaling from one image to another similar
 Home-page: https://github.com/bilykigor/doc_template_cloner
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Custom lib to clone lebaling from one image to another similar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `doc_template_cloner-0.0.3/setup.py` & `doc_template_cloner-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 required_packages = [
     #"boto3>=1.20.21,<2.0",
     "pandas",
 ]
 
 setup(
     name="doc_template_cloner",
-    version="0.0.3",
+    version="0.0.4",
     description="Custom lib to clone lebaling from one image to another similar",
     long_description_content_type="text/markdown",
     long_description=read('README.md'),
     packages=find_packages(),
     py_modules=[os.path.splitext(os.path.basename(path))[0] for path in glob("doc_template_cloner/*.py")],
     include_package_data=True,
     author="Ihor Bilyk",
```

