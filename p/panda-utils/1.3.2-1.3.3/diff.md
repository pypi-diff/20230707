# Comparing `tmp/panda_utils-1.3.2.tar.gz` & `tmp/panda_utils-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.3.2.tar", last modified: Fri Jul  7 08:00:07 2023, max compression
+gzip compressed data, was "panda_utils-1.3.3.tar", last modified: Fri Jul  7 09:35:41 2023, max compression
```

## Comparing `panda_utils-1.3.2.tar` & `panda_utils-1.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 08:00:07.457566 panda_utils-1.3.2/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1080 2022-08-12 11:48:21.000000 panda_utils-1.3.2/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    21141 2023-07-07 08:00:07.457566 panda_utils-1.3.2/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    20411 2023-07-07 07:56:07.000000 panda_utils-1.3.2/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.3.2/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 08:00:07.454233 panda_utils-1.3.2/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3.2/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.3.2/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 08:00:07.457566 panda_utils-1.3.2/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.3.2/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3713 2023-07-06 06:40:24.000000 panda_utils-1.3.2/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      256 2023-06-13 10:12:15.000000 panda_utils-1.3.2/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.3.2/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    11709 2023-07-07 07:59:14.000000 panda_utils-1.3.2/panda_utils/assetpipeline/models.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.3.2/panda_utils/assetpipeline/textures.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 08:00:07.457566 panda_utils-1.3.2/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.3.2/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.3.2/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.3.2/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 08:00:07.457566 panda_utils-1.3.2/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.3.2/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5179 2023-06-14 17:29:22.000000 panda_utils-1.3.2/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.3.2/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 08:00:07.457566 panda_utils-1.3.2/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3.2/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.3.2/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.3.2/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.3.2/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.3.2/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.3.2/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2483 2023-07-06 07:51:52.000000 panda_utils-1.3.2/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 08:00:07.454233 panda_utils-1.3.2/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    21141 2023-07-07 08:00:07.000000 panda_utils-1.3.2/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      916 2023-07-07 08:00:07.000000 panda_utils-1.3.2/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-07 08:00:07.000000 panda_utils-1.3.2/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-07 08:00:07.000000 panda_utils-1.3.2/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-07 08:00:07.000000 panda_utils-1.3.2/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-07 07:54:22.000000 panda_utils-1.3.2/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.3.2/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-07 08:00:07.457566 panda_utils-1.3.2/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 09:35:41.230776 panda_utils-1.3.3/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.3.3/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    22167 2023-07-07 09:35:41.230776 panda_utils-1.3.3/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    21437 2023-07-07 09:35:29.000000 panda_utils-1.3.3/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.3.3/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 09:35:41.227443 panda_utils-1.3.3/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3.3/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.3.3/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 09:35:41.230776 panda_utils-1.3.3/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.3.3/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3884 2023-07-07 08:54:01.000000 panda_utils-1.3.3/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      256 2023-06-13 10:12:15.000000 panda_utils-1.3.3/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.3.3/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    13121 2023-07-07 09:32:01.000000 panda_utils-1.3.3/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.3.3/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 09:35:41.230776 panda_utils-1.3.3/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.3.3/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.3.3/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.3.3/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 09:35:41.230776 panda_utils-1.3.3/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.3.3/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5608 2023-07-07 09:32:40.000000 panda_utils-1.3.3/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.3.3/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 09:35:41.230776 panda_utils-1.3.3/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3.3/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.3.3/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.3.3/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.3.3/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.3.3/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.3.3/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2483 2023-07-06 07:51:52.000000 panda_utils-1.3.3/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-07 09:35:41.230776 panda_utils-1.3.3/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    22167 2023-07-07 09:35:41.000000 panda_utils-1.3.3/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      916 2023-07-07 09:35:41.000000 panda_utils-1.3.3/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-07 09:35:41.000000 panda_utils-1.3.3/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-07 09:35:41.000000 panda_utils-1.3.3/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-07 09:35:41.000000 panda_utils-1.3.3/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-07 08:59:42.000000 panda_utils-1.3.3/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.3.3/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-07 09:35:41.230776 panda_utils-1.3.3/setup.cfg
```

### Comparing `panda_utils-1.3.2/LICENSE` & `panda_utils-1.3.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Toontown: Event Horizon
+Copyright (c) 2022-2023 Toontown: Event Horizon
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `panda_utils-1.3.2/PKG-INFO` & `panda_utils-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda_utils
-Version: 1.3.2
+Version: 1.3.3
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: imagery
 Provides-Extra: autopath
 Provides-Extra: runnable
 Provides-Extra: pipeline
 Provides-Extra: everything
 License-File: LICENSE
 
-# Panda3D Utils v1.3.2
+# Panda3D Utils v1.3.3
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -179,33 +179,39 @@
 In that case, the step will take the arguments from a YAML file named `model-config.yml`
 in the asset input directory. It is parsed as follows:
 
 * First, the yaml field with the name = the step name is taken from the file.
 * If that field is not present, or the file is not present, the step has
   no effect.
 * If the field is a dictionary, it will be applied as keyword arguments.
-* If the field is a list, the step will be applied once for each dictionary
-  inside of it in the proper order.
+* If the field is a string, it will be applied as the only positional argument.
+  *New in version 1.3.3.*
+* If the field is a list, the step will be applied once for each item
+  inside of it in the proper order. This is not recursive.
 
 This sounds confusing, so here's an example of such a config file:
 
 ```yaml
 transform:
   - scale: 10
   - rotate: 0,0,180
 collide:
   flags: keep,descend
   method: polyset
   group_name: optimized
+random_action: group2
 ```
 
 When a `transform[]` action is encountered, two transform steps will be called
 in order, first the node will be rescaled, and then it will be rotated.
 When a `collide[]` action is encountered, it will be called once with the given
-arguments. If a different `[]` action is encountered, it will not run.
+arguments.
+When a `random_action[]` action is encountered, it will be called once with the
+argument `group2`.
+If a different `[]` action is encountered, it will not run.
 This method is used for easy interaction with Makefiles (if the input folder 
 is set as the makefile dependency, changing this file will cause the task
 building a given asset to be rerun).
 
 The pipeline will normally hide all outputs unless the environmental variable
 `PANDA_UTILS_LOGGING`  is not empty.
 
@@ -221,27 +227,27 @@
 
 **Changelog**
 * 1.2 - now joins all models into the same blend file, instead of making
   separate blend files per model
 * 1.1 - initial implementation
 
 **Examples**
-`preblend`
+* `preblend`
 
 ### BlendRename
 
 This step will rename the BLEND models into their proper name. It is required
 if the input files are in BLEND format, but not required if the Blend files are
 generated through Preblend. This step takes no arguments.
 
 **Changelog**
 * 1.1 - initial implementation
 
 **Examples**
-`blendrename`
+* `blendrename`
 
 ### Blend2Bam
 
 This step will use Blend2Bam to convert the BLEND moodels into an intermediate
 BAM model. It should happen after `preblend` or `blendrename`. This model
 is usually not suitable for ingame use and requires further processing through
 `bam2egg`. This step requires installing Blender on the machine. It is tested
@@ -298,15 +304,15 @@
 `find()` while loading this model.
 
 This step takes no parameters.
 
 **Changelog**
 * 1.3 - initial implementation
 
-*Examples**
+**Examples**
 * `model_parent`
 
 ### Group rename
 This step renames all collections with the given name into a different name.
 
 This step uses keyword arguments, which means it can only be run through `[]`.
 Setting a name to `__delete__` will delete the node. For example:
@@ -316,15 +322,15 @@
   hands.003: hands
   useless-node: __delete__
 ```
 
 **Changelog**
 * 1.3 - initial implementation
 
-*Examples**
+**Examples**
 * `group_rename[]`
 
 ### Group remove
 This step removes all collections with the given name. Unlike group rename,
 allows using fnmatch syntax to find the collections.
 
 Accepts one argument equal to the fnmatch pattern that is removed. Can be
@@ -335,15 +341,15 @@
   hands.003: hands
   useless-node: __delete__
 ```
 
 **Changelog**
 * 1.3 - initial implementation
 
-*Examples**
+**Examples**
 * `group_remove[]`
 * `group_remove:*useless*`
 
 ### Optchar
 This step runs `egg-optchar`, setting the exposed joints and the flagged nodes.
 Note that changing the dart is currently not supported.
 
@@ -409,14 +415,42 @@
 
 **Examples**
 * `collide`
 * `collide:keep,descend:tube`
 * `collide:descend:polyset:optimized_geom`
 * `collide[]`
 
+### Remove Materials
+
+This step removes all materials and UV maps from the models. This is needed
+to export certain actors, and things like toon heads. You should not use
+this step unless you know what you're doing. It accepts no parameters.
+
+Note that applying this step before `palettize` will not have any effect.
+
+**Changelog**
+* 1.3.3 - initial implementation
+
+**Examples**
+* `rmmat`
+
+### Transparent
+
+This step makes all textures in the model semitransparent by adding
+`<Scalar> alpha { dual }` to all of them. You should not use this unless you
+get transparency-related rendering issues. It accepts no parameters.
+
+Note that applying this step before `palettize` will not have any effect.
+
+**Changelog**
+* 1.3.3 - initial implementation
+
+**Examples**
+* `transparent`
+
 ### Downscale
 
 This step is used to resize one texture or all PNG textures in the folder
 to a given size. Installing `Pillow` is required for this step (provided
 by the `imagery` extra).
 
 This step accepts up to four arguments.
```

### Comparing `panda_utils-1.3.2/README.md` & `panda_utils-1.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Panda3D Utils v1.3.2
+# Panda3D Utils v1.3.3
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -160,33 +160,39 @@
 In that case, the step will take the arguments from a YAML file named `model-config.yml`
 in the asset input directory. It is parsed as follows:
 
 * First, the yaml field with the name = the step name is taken from the file.
 * If that field is not present, or the file is not present, the step has
   no effect.
 * If the field is a dictionary, it will be applied as keyword arguments.
-* If the field is a list, the step will be applied once for each dictionary
-  inside of it in the proper order.
+* If the field is a string, it will be applied as the only positional argument.
+  *New in version 1.3.3.*
+* If the field is a list, the step will be applied once for each item
+  inside of it in the proper order. This is not recursive.
 
 This sounds confusing, so here's an example of such a config file:
 
 ```yaml
 transform:
   - scale: 10
   - rotate: 0,0,180
 collide:
   flags: keep,descend
   method: polyset
   group_name: optimized
+random_action: group2
 ```
 
 When a `transform[]` action is encountered, two transform steps will be called
 in order, first the node will be rescaled, and then it will be rotated.
 When a `collide[]` action is encountered, it will be called once with the given
-arguments. If a different `[]` action is encountered, it will not run.
+arguments.
+When a `random_action[]` action is encountered, it will be called once with the
+argument `group2`.
+If a different `[]` action is encountered, it will not run.
 This method is used for easy interaction with Makefiles (if the input folder 
 is set as the makefile dependency, changing this file will cause the task
 building a given asset to be rerun).
 
 The pipeline will normally hide all outputs unless the environmental variable
 `PANDA_UTILS_LOGGING`  is not empty.
 
@@ -202,27 +208,27 @@
 
 **Changelog**
 * 1.2 - now joins all models into the same blend file, instead of making
   separate blend files per model
 * 1.1 - initial implementation
 
 **Examples**
-`preblend`
+* `preblend`
 
 ### BlendRename
 
 This step will rename the BLEND models into their proper name. It is required
 if the input files are in BLEND format, but not required if the Blend files are
 generated through Preblend. This step takes no arguments.
 
 **Changelog**
 * 1.1 - initial implementation
 
 **Examples**
-`blendrename`
+* `blendrename`
 
 ### Blend2Bam
 
 This step will use Blend2Bam to convert the BLEND moodels into an intermediate
 BAM model. It should happen after `preblend` or `blendrename`. This model
 is usually not suitable for ingame use and requires further processing through
 `bam2egg`. This step requires installing Blender on the machine. It is tested
@@ -279,15 +285,15 @@
 `find()` while loading this model.
 
 This step takes no parameters.
 
 **Changelog**
 * 1.3 - initial implementation
 
-*Examples**
+**Examples**
 * `model_parent`
 
 ### Group rename
 This step renames all collections with the given name into a different name.
 
 This step uses keyword arguments, which means it can only be run through `[]`.
 Setting a name to `__delete__` will delete the node. For example:
@@ -297,15 +303,15 @@
   hands.003: hands
   useless-node: __delete__
 ```
 
 **Changelog**
 * 1.3 - initial implementation
 
-*Examples**
+**Examples**
 * `group_rename[]`
 
 ### Group remove
 This step removes all collections with the given name. Unlike group rename,
 allows using fnmatch syntax to find the collections.
 
 Accepts one argument equal to the fnmatch pattern that is removed. Can be
@@ -316,15 +322,15 @@
   hands.003: hands
   useless-node: __delete__
 ```
 
 **Changelog**
 * 1.3 - initial implementation
 
-*Examples**
+**Examples**
 * `group_remove[]`
 * `group_remove:*useless*`
 
 ### Optchar
 This step runs `egg-optchar`, setting the exposed joints and the flagged nodes.
 Note that changing the dart is currently not supported.
 
@@ -390,14 +396,42 @@
 
 **Examples**
 * `collide`
 * `collide:keep,descend:tube`
 * `collide:descend:polyset:optimized_geom`
 * `collide[]`
 
+### Remove Materials
+
+This step removes all materials and UV maps from the models. This is needed
+to export certain actors, and things like toon heads. You should not use
+this step unless you know what you're doing. It accepts no parameters.
+
+Note that applying this step before `palettize` will not have any effect.
+
+**Changelog**
+* 1.3.3 - initial implementation
+
+**Examples**
+* `rmmat`
+
+### Transparent
+
+This step makes all textures in the model semitransparent by adding
+`<Scalar> alpha { dual }` to all of them. You should not use this unless you
+get transparency-related rendering issues. It accepts no parameters.
+
+Note that applying this step before `palettize` will not have any effect.
+
+**Changelog**
+* 1.3.3 - initial implementation
+
+**Examples**
+* `transparent`
+
 ### Downscale
 
 This step is used to resize one texture or all PNG textures in the folder
 to a given size. Installing `Pillow` is required for this step (provided
 by the `imagery` extra).
 
 This step accepts up to four arguments.
```

### Comparing `panda_utils-1.3.2/panda_utils/__main__.py` & `panda_utils-1.3.3/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.3.3/panda_utils/assetpipeline/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,21 +41,27 @@
         with open(YAML_CONFIG_FILENAME) as f:
             data = yaml.safe_load(f)
 
         if name not in data:
             return
 
         args = data[name]
+        if isinstance(args, list):
+            for kwargs in args:
+                self.run_action(action, kwargs)
+        else:
+            self.run_action(action, args)
+
+    def run_action(self, action, args):
         if isinstance(args, dict):
             action(self, **args)
-        elif isinstance(args, list):
-            for kwargs in args:
-                action(self, **kwargs)
+        elif isinstance(args, str):
+            action(self, args)
         else:
-            logger.warning("%s: Invalid configured arguments: %s (expected list or dict)", self.name, type(args))
+            logger.warning("%s: Invalid configured arguments: %s (expected dict, or str)", self.name, type(args))
 
 
 def main(enable_logging=False):
     if enable_logging:
         console = logging.StreamHandler()
         console.setLevel(logging.INFO)
         formatter = logging.Formatter("%(name)-12s: %(levelname)-8s %(message)s")
```

### Comparing `panda_utils-1.3.2/panda_utils/assetpipeline/models.py` & `panda_utils-1.3.3/panda_utils/assetpipeline/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,34 @@
                     nodeset.add(node)
         eggtree.remove_nodes(nodeset)
 
         with open(file, "w") as f:
             f.write(str(eggtree))
 
 
+def action_transparent(ctx):
+    for file in ctx.files:
+        if file.endswith(".egg"):
+            logger.info("%s: Adding transparency to: %s", ctx.name, file)
+            with open(file) as f:
+                data = f.readlines()
+
+            eggtree = eggparse.egg_tokenize(data)
+            new_node = eggparse.EggLeaf("Scalar", "alpha", "dual")
+            for tex in eggtree.findall("Texture"):
+                for child in tex.children:
+                    if child.equals(new_node):
+                        break
+                else:
+                    tex.add_child(new_node)
+
+            with open(file, "w") as f:
+                f.write(str(eggtree))
+
+
 def action_model_parent(ctx):
     for file in ctx.files:
         if not file.endswith(".egg"):
             continue
 
         with open(file) as f:
             eggtree = eggparse.egg_tokenize(f.readlines())
@@ -158,14 +178,36 @@
                     options.append(str(value))
             if options:
                 translated_file_name = f"translated-{file}"
                 util.run_panda(ctx.putil_ctx, "egg-trans", *options, "-o", translated_file_name, file)
                 os.replace(translated_file_name, file)
 
 
+def action_rmmat(ctx):
+    for file in ctx.files:
+        if file.endswith(".egg"):
+            logger.info("%s: Removing materials from: %s", ctx.name, file)
+            with open(file) as f:
+                data = f.readlines()
+
+            eggtree = eggparse.egg_tokenize(data)
+            nodes_for_removal = (
+                eggtree.findall("Material")
+                + eggtree.findall("MRef")
+                + [scalar for scalar in eggtree.findall("Scalar") if scalar.node_name == "uv-name"]
+            )
+            eggtree.remove_nodes(set(nodes_for_removal))
+
+            for uv in eggtree.findall("UV"):
+                uv.node_name = None
+
+            with open(file, "w") as f:
+                f.write(str(eggtree))
+
+
 def action_collide(ctx, flags="keep,descend", method="sphere", group_name=None, bitmask=None):
     group_name = group_name or ctx.model_name
     method = method.capitalize()
     flags = flags.replace(",", " ")
     for file in ctx.files:
         if file.endswith(".egg"):
             logger.info("%s: Adding collisions to %s: flags=%s method=%s", ctx.name, file, flags, method)
@@ -190,16 +232,16 @@
                 # when the egg file is read. So we have to delete every object that's not a polygon.
                 # https://github.com/panda3d/panda3d/issues/1515
                 nodes = groups[0].findall("Line") + groups[0].findall("Patch") + groups[0].findall("PointLight")
                 if nodes:
                     logger.warning("Found non-polygon objects while generating collisions, removing...")
                     groups[0].remove_nodes(set(nodes))
 
-            with open(file, "w") as f:
-                f.write(str(eggtree))
+                with open(file, "w") as f:
+                    f.write(str(eggtree))
 
 
 def action_palettize(ctx, palette_size="1024", flags=""):
     palette_size = int(palette_size)
     if palette_size & (palette_size - 1):
         raise ValueError("The palette size must be a power of two!")
```

### Comparing `panda_utils-1.3.2/panda_utils/assetpipeline/textures.py` & `panda_utils-1.3.3/panda_utils/assetpipeline/textures.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/panda_utils/blender/import_model.py` & `panda_utils-1.3.3/panda_utils/blender/import_model.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/panda_utils/eggtree/eggparse.py` & `panda_utils-1.3.3/panda_utils/eggtree/eggparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,18 @@
     def remove_nodes(self, nodeset):
         pass
 
     @abc.abstractmethod
     def get_child(self, index):
         pass
 
+    # We can't use __eq__ because it breaks set()
+    def equals(self, other):
+        return False
+
 
 class EggString(EggNode):
     def __init__(self, value):
         self.value = value
 
     def __repr__(self):
         return self.value
@@ -60,21 +64,30 @@
 
     def remove_nodes(self, nodeset):
         pass
 
     def get_child(self, index):
         return None
 
+    def equals(self, other):
+        return isinstance(other, EggString) and other.value == self.value
+
 
 class EggLeaf(EggNode):
     def __init__(self, node_type, node_name, node_value):
         self.node_type = node_type
         self.node_name = (node_name or "").strip()
         self.node_value = node_value
 
+    def equals(self, other):
+        return (
+            isinstance(other, EggLeaf) and other.node_name == self.node_name and other.node_value == self.node_value
+            and other.node_type == self.node_type
+        )
+
     def __repr__(self):
         if self.node_name:
             return f"<{self.node_type}> {self.node_name.strip()} {{ {self.node_value.strip()} }}"
         return f"<{self.node_type}> {{ {self.node_value.strip()} }}"
 
     def findall(self, node_type):
         if self.node_type == node_type:
```

### Comparing `panda_utils-1.3.2/panda_utils/eggtree/operations.py` & `panda_utils-1.3.3/panda_utils/eggtree/operations.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/panda_utils/tools/animconvert.py` & `panda_utils-1.3.3/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/panda_utils/tools/convert.py` & `panda_utils-1.3.3/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/panda_utils/tools/downscale.py` & `panda_utils-1.3.3/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/panda_utils/tools/palettize.py` & `panda_utils-1.3.3/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/panda_utils/tools/toontown.py` & `panda_utils-1.3.3/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/panda_utils/util.py` & `panda_utils-1.3.3/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.3.3/panda_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-utils
-Version: 1.3.2
+Version: 1.3.3
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: imagery
 Provides-Extra: autopath
 Provides-Extra: runnable
 Provides-Extra: pipeline
 Provides-Extra: everything
 License-File: LICENSE
 
-# Panda3D Utils v1.3.2
+# Panda3D Utils v1.3.3
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -179,33 +179,39 @@
 In that case, the step will take the arguments from a YAML file named `model-config.yml`
 in the asset input directory. It is parsed as follows:
 
 * First, the yaml field with the name = the step name is taken from the file.
 * If that field is not present, or the file is not present, the step has
   no effect.
 * If the field is a dictionary, it will be applied as keyword arguments.
-* If the field is a list, the step will be applied once for each dictionary
-  inside of it in the proper order.
+* If the field is a string, it will be applied as the only positional argument.
+  *New in version 1.3.3.*
+* If the field is a list, the step will be applied once for each item
+  inside of it in the proper order. This is not recursive.
 
 This sounds confusing, so here's an example of such a config file:
 
 ```yaml
 transform:
   - scale: 10
   - rotate: 0,0,180
 collide:
   flags: keep,descend
   method: polyset
   group_name: optimized
+random_action: group2
 ```
 
 When a `transform[]` action is encountered, two transform steps will be called
 in order, first the node will be rescaled, and then it will be rotated.
 When a `collide[]` action is encountered, it will be called once with the given
-arguments. If a different `[]` action is encountered, it will not run.
+arguments.
+When a `random_action[]` action is encountered, it will be called once with the
+argument `group2`.
+If a different `[]` action is encountered, it will not run.
 This method is used for easy interaction with Makefiles (if the input folder 
 is set as the makefile dependency, changing this file will cause the task
 building a given asset to be rerun).
 
 The pipeline will normally hide all outputs unless the environmental variable
 `PANDA_UTILS_LOGGING`  is not empty.
 
@@ -221,27 +227,27 @@
 
 **Changelog**
 * 1.2 - now joins all models into the same blend file, instead of making
   separate blend files per model
 * 1.1 - initial implementation
 
 **Examples**
-`preblend`
+* `preblend`
 
 ### BlendRename
 
 This step will rename the BLEND models into their proper name. It is required
 if the input files are in BLEND format, but not required if the Blend files are
 generated through Preblend. This step takes no arguments.
 
 **Changelog**
 * 1.1 - initial implementation
 
 **Examples**
-`blendrename`
+* `blendrename`
 
 ### Blend2Bam
 
 This step will use Blend2Bam to convert the BLEND moodels into an intermediate
 BAM model. It should happen after `preblend` or `blendrename`. This model
 is usually not suitable for ingame use and requires further processing through
 `bam2egg`. This step requires installing Blender on the machine. It is tested
@@ -298,15 +304,15 @@
 `find()` while loading this model.
 
 This step takes no parameters.
 
 **Changelog**
 * 1.3 - initial implementation
 
-*Examples**
+**Examples**
 * `model_parent`
 
 ### Group rename
 This step renames all collections with the given name into a different name.
 
 This step uses keyword arguments, which means it can only be run through `[]`.
 Setting a name to `__delete__` will delete the node. For example:
@@ -316,15 +322,15 @@
   hands.003: hands
   useless-node: __delete__
 ```
 
 **Changelog**
 * 1.3 - initial implementation
 
-*Examples**
+**Examples**
 * `group_rename[]`
 
 ### Group remove
 This step removes all collections with the given name. Unlike group rename,
 allows using fnmatch syntax to find the collections.
 
 Accepts one argument equal to the fnmatch pattern that is removed. Can be
@@ -335,15 +341,15 @@
   hands.003: hands
   useless-node: __delete__
 ```
 
 **Changelog**
 * 1.3 - initial implementation
 
-*Examples**
+**Examples**
 * `group_remove[]`
 * `group_remove:*useless*`
 
 ### Optchar
 This step runs `egg-optchar`, setting the exposed joints and the flagged nodes.
 Note that changing the dart is currently not supported.
 
@@ -409,14 +415,42 @@
 
 **Examples**
 * `collide`
 * `collide:keep,descend:tube`
 * `collide:descend:polyset:optimized_geom`
 * `collide[]`
 
+### Remove Materials
+
+This step removes all materials and UV maps from the models. This is needed
+to export certain actors, and things like toon heads. You should not use
+this step unless you know what you're doing. It accepts no parameters.
+
+Note that applying this step before `palettize` will not have any effect.
+
+**Changelog**
+* 1.3.3 - initial implementation
+
+**Examples**
+* `rmmat`
+
+### Transparent
+
+This step makes all textures in the model semitransparent by adding
+`<Scalar> alpha { dual }` to all of them. You should not use this unless you
+get transparency-related rendering issues. It accepts no parameters.
+
+Note that applying this step before `palettize` will not have any effect.
+
+**Changelog**
+* 1.3.3 - initial implementation
+
+**Examples**
+* `transparent`
+
 ### Downscale
 
 This step is used to resize one texture or all PNG textures in the folder
 to a given size. Installing `Pillow` is required for this step (provided
 by the `imagery` extra).
 
 This step accepts up to four arguments.
```

### Comparing `panda_utils-1.3.2/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.3.3/panda_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3.2/pyproject.toml` & `panda_utils-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.3.2"
+version = "1.3.3"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

