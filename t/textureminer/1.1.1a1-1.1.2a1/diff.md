# Comparing `tmp/textureminer-1.1.1a1.tar.gz` & `tmp/textureminer-1.1.2a1.tar.gz`

## Comparing `textureminer-1.1.1a1.tar` & `textureminer-1.1.2a1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/CHANGELOG.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/requirements.txt
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/.vscode/tasks.json
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/src/textureminer/__init__.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/src/textureminer/__main__.py
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/src/textureminer/bedrock.py
--rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/src/textureminer/common.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/src/textureminer/java.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/src/textureminer/texts.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/LICENSE
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/pyproject.toml
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 textureminer-1.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/CHANGELOG.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/requirements.txt
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/.vscode/tasks.json
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/src/textureminer/__init__.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/src/textureminer/__main__.py
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/src/textureminer/bedrock.py
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/src/textureminer/common.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/src/textureminer/java.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/src/textureminer/texts.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/LICENSE
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/pyproject.toml
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 textureminer-1.1.2a1/PKG-INFO
```

### Comparing `textureminer-1.1.1a1/src/textureminer/__main__.py` & `textureminer-1.1.2a1/src/textureminer/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,30 +21,31 @@
         **kwargs: keyword arguments that will be passed to the get_textures function of the specified edition
 
     Returns:
         string: path of the final textures
     """
 
     if edition == EditionType.JAVA:
-        tabbed_print(texts.EDITION_USING_X.format(edition=edition.value))
+        tabbed_print(
+            texts.EDITION_USING_X.format(edition=edition.value.capitalize()))
         return java.get_textures(*args, **kwargs)
 
     if edition == EditionType.BEDROCK:
-        tabbed_print(texts.EDITION_USING_X.format(edition=edition.value))
+        tabbed_print(
+            texts.EDITION_USING_X.format(edition=edition.value.capitalize()))
         return bedrock.get_textures(*args, **kwargs)
     return None
 
 
 def cli():
     """CLI entrypoint.
 
     Returns:
         str: path to the output directory
     """
-    args = sys.argv[1:]
 
     if len(args) > 0 and args[0].lower() in [
             '--help',
             '-h'
             'help',
     ]:
         print(texts.COMMAND_SYNTAX)
@@ -93,8 +94,9 @@
 
     tabbed_print(texts.INVALID_COMBINATION)
     tabbed_print(texts.EDITION_USING_DEFAULT)
     return get_textures(version_or_type=DEFAULT_VERSION,
                         edition=DEFAULT_EDITION)
 
 
+args = sys.argv[1:]
 cli()
```

### Comparing `textureminer-1.1.1a1/src/textureminer/bedrock.py` & `textureminer-1.1.2a1/src/textureminer/bedrock.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,40 +67,44 @@
 
     tabbed_print(texts.FILE_DOWNLOADING)
 
     repo_dir = f'{TEMP_PATH}/bedrock-samples/'
 
     rm_if_exists(repo_dir)
 
-    clone_command = ['git', 'clone', REPO_URL, repo_dir]
+    command_1 = f'git clone --filter=blob:none --sparse {REPO_URL} {repo_dir}'
+    command_2 = 'git config core.sparsecheckout true && echo "resource_pack" >> .git/info/sparse-checkout && git sparse-checkout init --cone && git sparse-checkout set resource_pack'
 
     try:
-        subprocess.run(clone_command,
+        subprocess.run(command_1,
                        check=True,
                        stdout=subprocess.DEVNULL,
                        stderr=subprocess.STDOUT)
+        subprocess.run(command_2,
+                       check=True,
+                       stdout=subprocess.DEVNULL,
+                       stderr=subprocess.STDOUT,
+                       cwd=repo_dir,
+                       shell=True)
+
     except subprocess.CalledProcessError as err:
         print(
             texts.ERROR_COMMAND_FAILED.format(error_code=err.returncode,
                                               error_msg=err.stderr))
 
     return repo_dir
 
 
 def update_tags(repo_dir: str):
     """Updates the tags of the repository.
 
     Args:
         repo_dir (str): directory of the repository
     """
-    subprocess.run(
-        'git fetch --tags',
-        check=False,
-        cwd=repo_dir,
-    )
+    subprocess.run('git fetch --tags', check=False, cwd=repo_dir)
 
 
 def change_repo_version(repo_dir: str, version: str, fetch_tags: bool = True):
     """Changes the version of the repository.
 
     Args:
         repo_dir (str): directory of the repository
```

### Comparing `textureminer-1.1.1a1/src/textureminer/common.py` & `textureminer-1.1.2a1/src/textureminer/common.py`

 * *Files identical despite different names*

### Comparing `textureminer-1.1.1a1/src/textureminer/java.py` & `textureminer-1.1.2a1/src/textureminer/java.py`

 * *Files identical despite different names*

### Comparing `textureminer-1.1.1a1/src/textureminer/texts.py` & `textureminer-1.1.2a1/src/textureminer/texts.py`

 * *Files identical despite different names*

### Comparing `textureminer-1.1.1a1/.gitignore` & `textureminer-1.1.2a1/.gitignore`

 * *Files identical despite different names*

### Comparing `textureminer-1.1.1a1/LICENSE` & `textureminer-1.1.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `textureminer-1.1.1a1/README.md` & `textureminer-1.1.2a1/README.md`

 * *Files identical despite different names*

### Comparing `textureminer-1.1.1a1/pyproject.toml` & `textureminer-1.1.2a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "textureminer"
-version = "1.1.1-alpha.1"
+version = "1.1.2-alpha.1"
 authors = [
   { name="4MBL" },
 ]
 description = "Script that allows you to extract and scale Minecraft's item and block textures."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.11"
```

### Comparing `textureminer-1.1.1a1/PKG-INFO` & `textureminer-1.1.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textureminer
-Version: 1.1.1a1
+Version: 1.1.2a1
 Summary: Script that allows you to extract and scale Minecraft's item and block textures.
 Project-URL: Homepage, https://github.com/4MBL/texture-miner
 Project-URL: Bug Tracker, https://github.com/4MBL/texture-miner/issues
 Author: 4MBL
 License: MIT License
         
         Copyright (c) 2023 4MBL
```

