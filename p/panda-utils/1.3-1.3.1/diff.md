# Comparing `tmp/panda_utils-1.3.tar.gz` & `tmp/panda_utils-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.3.tar", last modified: Wed Jun 14 19:27:38 2023, max compression
+gzip compressed data, was "panda_utils-1.3.1.tar", last modified: Thu Jul  6 09:07:56 2023, max compression
```

## Comparing `panda_utils-1.3.tar` & `panda_utils-1.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.510842 panda_utils-1.3/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1080 2022-08-12 11:48:21.000000 panda_utils-1.3/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    20931 2023-06-14 19:27:38.510842 panda_utils-1.3/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    20203 2023-06-14 19:27:28.000000 panda_utils-1.3/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.3/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.467509 panda_utils-1.3/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.3/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.510842 panda_utils-1.3/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.3/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3715 2023-06-13 13:14:07.000000 panda_utils-1.3/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      256 2023-06-13 10:12:15.000000 panda_utils-1.3/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.3/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    10820 2023-06-14 19:20:04.000000 panda_utils-1.3/panda_utils/assetpipeline/models.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.3/panda_utils/assetpipeline/textures.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.510842 panda_utils-1.3/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.3/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.3/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.3/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.510842 panda_utils-1.3/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.3/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5179 2023-06-14 17:29:22.000000 panda_utils-1.3/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.3/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.510842 panda_utils-1.3/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.3/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.3/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.3/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.3/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.3/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2482 2023-06-12 19:50:06.000000 panda_utils-1.3/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-14 19:27:38.470842 panda_utils-1.3/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    20931 2023-06-14 19:27:38.000000 panda_utils-1.3/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      916 2023-06-14 19:27:38.000000 panda_utils-1.3/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-06-14 19:27:38.000000 panda_utils-1.3/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-06-14 19:27:38.000000 panda_utils-1.3/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-06-14 19:27:38.000000 panda_utils-1.3/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1021 2023-06-14 19:20:10.000000 panda_utils-1.3/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.3/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-06-14 19:27:38.510842 panda_utils-1.3/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-06 09:07:56.981162 panda_utils-1.3.1/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1080 2022-08-12 11:48:21.000000 panda_utils-1.3.1/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    20933 2023-07-06 09:07:56.981162 panda_utils-1.3.1/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    20203 2023-06-14 19:27:28.000000 panda_utils-1.3.1/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.3.1/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-06 09:07:56.977828 panda_utils-1.3.1/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3.1/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.3.1/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-06 09:07:56.981162 panda_utils-1.3.1/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.3.1/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3713 2023-07-06 06:40:24.000000 panda_utils-1.3.1/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      256 2023-06-13 10:12:15.000000 panda_utils-1.3.1/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.3.1/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    11400 2023-07-06 09:04:12.000000 panda_utils-1.3.1/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.3.1/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-06 09:07:56.981162 panda_utils-1.3.1/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.3.1/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.3.1/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.3.1/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-06 09:07:56.981162 panda_utils-1.3.1/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.3.1/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5179 2023-06-14 17:29:22.000000 panda_utils-1.3.1/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.3.1/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-06 09:07:56.981162 panda_utils-1.3.1/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.3.1/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.3.1/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.3.1/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.3.1/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.3.1/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.3.1/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2483 2023-07-06 07:51:52.000000 panda_utils-1.3.1/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-06 09:07:56.977828 panda_utils-1.3.1/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    20933 2023-07-06 09:07:56.000000 panda_utils-1.3.1/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      916 2023-07-06 09:07:56.000000 panda_utils-1.3.1/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-06 09:07:56.000000 panda_utils-1.3.1/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-06 09:07:56.000000 panda_utils-1.3.1/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-06 09:07:56.000000 panda_utils-1.3.1/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-06 09:07:18.000000 panda_utils-1.3.1/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.3.1/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-06 09:07:56.981162 panda_utils-1.3.1/setup.cfg
```

### Comparing `panda_utils-1.3/LICENSE` & `panda_utils-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/PKG-INFO` & `panda_utils-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda_utils
-Version: 1.3
+Version: 1.3.1
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.3/README.md` & `panda_utils-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/__main__.py` & `panda_utils-1.3.1/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.3.1/panda_utils/assetpipeline/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.intermediate_path = f"{OUTPUT_PARENT}/{output_phase}/models/{output_folder}/{self.model_name}"
         self.output_model_rel = f"{output_phase}/models/{output_folder}"
         self.output_model = os.path.abspath(os.path.dirname(self.intermediate_path))
         self.output_texture = os.path.abspath(f"{OUTPUT_PARENT}/{output_phase}/maps")
 
     @property
     def files(self):
-        return os.listdir()
+        return sorted(os.listdir())
 
     def run_action_through_config(self, action, name):
         if YAML_CONFIG_FILENAME not in self.files:
             return
 
         with open(YAML_CONFIG_FILENAME) as f:
             data = yaml.safe_load(f)
@@ -51,15 +51,15 @@
             for kwargs in args:
                 action(self, **kwargs)
         else:
             logger.warning("%s: Invalid configured arguments: %s (expected list or dict)", self.name, type(args))
 
 
 def main(enable_logging=False):
-    if False and enable_logging:
+    if enable_logging:
         console = logging.StreamHandler()
         console.setLevel(logging.INFO)
         formatter = logging.Formatter("%(name)-12s: %(levelname)-8s %(message)s")
         console.setFormatter(formatter)
         global_logger = logging.getLogger("")
         global_logger.setLevel(logging.INFO)
         global_logger.addHandler(console)
@@ -103,8 +103,8 @@
             if use_config:
                 ctx.run_action_through_config(action, method_name)
             else:
                 action(ctx, *args)
 
 
 if __name__ == "__main__":
-    main(os.getenv("PANDA_UTILS_LOGGING") != "")
+    main(bool(os.getenv("PANDA_UTILS_LOGGING")))
```

### Comparing `panda_utils-1.3/panda_utils/assetpipeline/models.py` & `panda_utils-1.3.1/panda_utils/assetpipeline/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 stdout=subprocess.DEVNULL,
                 cwd=ctx.cwd,
             )
 
             logger.info("%s: Converting to bam: %s", ctx.name, file)
             bam_filename = file[:-5] + "bam"
             res = subprocess.run(["blend2bam", "--no-srgb", file, bam_filename],
-                                 stdout=subprocess.DEVNULL, stderr=subprocess.PIPE)
+                                 stdout=subprocess.DEVNULL, stderr=subprocess.PIPE, cwd=ctx.cwd)
             err = res.stderr.decode("utf-8")
             if err and "KeyError: 'nodes'" in err:
                 logger.error("%s: Blender output an empty model, aborting.", ctx.name)
                 ctx.valid = False
             elif err:
                 logger.error("%s: Blender failed", ctx.name)
                 print(err)
@@ -176,14 +176,22 @@
             eggtree = eggparse.egg_tokenize(data)
             groups = [group for group in eggtree.findall("Group") if group.node_name == group_name]
             if len(groups) == 1:
                 logger.info("Found the named group!")
                 new_node = eggparse.EggLeaf("Collide", group_name, f"{method} {flags}")
                 groups[0].children.children.insert(0, new_node)
 
+                # Fun fact: Setting <Collide> polyset if the group has non-poly objects will cause a segfault
+                # when the egg file is read. So we have to delete every object that's not a polygon.
+                if method == "Polyset":
+                    nodes = groups[0].findall("Line") + groups[0].findall("Patch") + groups[0].findall("PointLight")
+                    if nodes:
+                        logger.warning("Found non-polygon objects while generating collisions, removing...")
+                        groups[0].remove_nodes(set(nodes))
+
             with open(file, "w") as f:
                 f.write(str(eggtree))
 
 
 def action_palettize(ctx, palette_size="1024", flags=""):
     palette_size = int(palette_size)
     if palette_size & (palette_size - 1):
```

### Comparing `panda_utils-1.3/panda_utils/assetpipeline/textures.py` & `panda_utils-1.3.1/panda_utils/assetpipeline/textures.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/blender/import_model.py` & `panda_utils-1.3.1/panda_utils/blender/import_model.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/eggtree/eggparse.py` & `panda_utils-1.3.1/panda_utils/eggtree/eggparse.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/eggtree/operations.py` & `panda_utils-1.3.1/panda_utils/eggtree/operations.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/tools/animconvert.py` & `panda_utils-1.3.1/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/tools/convert.py` & `panda_utils-1.3.1/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/tools/downscale.py` & `panda_utils-1.3.1/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/tools/palettize.py` & `panda_utils-1.3.1/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/tools/toontown.py` & `panda_utils-1.3.1/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/panda_utils/util.py` & `panda_utils-1.3.1/panda_utils/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     path = f"{init_path}/{base_path}"
     if not os.path.exists(path):
         return []
 
     return [file for file in os.listdir(path) if os.path.isfile(f"{path}/{file}")]
 
 
-def run_panda(ctx: Context, command: str, *args: str, timeout: int = 2, debug: bool = False) -> str:
+def run_panda(ctx: Context, command: str, *args: str, timeout: int = 10, debug: bool = False) -> str:
     process = subprocess.Popen(
         [f"{ctx.panda_path}/{command}", *args], stdout=subprocess.DEVNULL, stderr=subprocess.PIPE
     )
     out = process.communicate(timeout=timeout)
     bts = out[1] if isinstance(out, tuple) else out
     out_str = bts.decode("utf-8")
     if process.returncode or debug:
```

### Comparing `panda_utils-1.3/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.3.1/panda_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-utils
-Version: 1.3
+Version: 1.3.1
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.3/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.3.1/panda_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_utils-1.3/pyproject.toml` & `panda_utils-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.3"
+version = "1.3.1"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

