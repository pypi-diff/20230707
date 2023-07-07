# Comparing `tmp/loadingpy-0.0.0.tar.gz` & `tmp/loadingpy-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadingpy-0.0.0.tar", last modified: Thu Jul  6 15:50:56 2023, max compression
+gzip compressed data, was "loadingpy-0.0.1.tar", last modified: Thu Jul  6 16:05:09 2023, max compression
```

## Comparing `loadingpy-0.0.0.tar` & `loadingpy-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-06 15:50:56.295517 loadingpy-0.0.0/
--rw-r--r--   0 edouard    (501) staff       (20)     1070 2023-07-06 11:00:49.000000 loadingpy-0.0.0/LICENCE
--rw-r--r--   0 edouard    (501) staff       (20)     1939 2023-07-06 15:50:56.295378 loadingpy-0.0.0/PKG-INFO
--rw-r--r--   0 edouard    (501) staff       (20)     1666 2023-07-06 15:50:10.000000 loadingpy-0.0.0/README.md
--rw-r--r--   0 edouard    (501) staff       (20)      385 2023-07-06 11:01:53.000000 loadingpy-0.0.0/pyproject.toml
--rw-r--r--   0 edouard    (501) staff       (20)       38 2023-07-06 15:50:56.295565 loadingpy-0.0.0/setup.cfg
-drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-06 15:50:56.291616 loadingpy-0.0.0/src/
-drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-06 15:50:56.293938 loadingpy-0.0.0/src/loadingpy/
--rw-r--r--   0 edouard    (501) staff       (20)       31 2023-07-06 12:46:20.000000 loadingpy-0.0.0/src/loadingpy/__init__.py
--rw-r--r--   0 edouard    (501) staff       (20)     3388 2023-07-06 12:57:09.000000 loadingpy-0.0.0/src/loadingpy/basic_bar.py
--rw-r--r--   0 edouard    (501) staff       (20)     1500 2023-07-06 11:25:44.000000 loadingpy-0.0.0/src/loadingpy/colored_bar.py
--rw-r--r--   0 edouard    (501) staff       (20)     3944 2023-07-06 12:40:15.000000 loadingpy-0.0.0/src/loadingpy/loading_bar.py
-drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-06 15:50:56.295184 loadingpy-0.0.0/src/loadingpy.egg-info/
--rw-r--r--   0 edouard    (501) staff       (20)     1939 2023-07-06 15:50:56.000000 loadingpy-0.0.0/src/loadingpy.egg-info/PKG-INFO
--rw-r--r--   0 edouard    (501) staff       (20)      291 2023-07-06 15:50:56.000000 loadingpy-0.0.0/src/loadingpy.egg-info/SOURCES.txt
--rw-r--r--   0 edouard    (501) staff       (20)        1 2023-07-06 15:50:56.000000 loadingpy-0.0.0/src/loadingpy.egg-info/dependency_links.txt
--rw-r--r--   0 edouard    (501) staff       (20)       10 2023-07-06 15:50:56.000000 loadingpy-0.0.0/src/loadingpy.egg-info/top_level.txt
+drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-06 16:05:09.809506 loadingpy-0.0.1/
+-rw-r--r--   0 edouard    (501) staff       (20)     1070 2023-07-06 11:00:49.000000 loadingpy-0.0.1/LICENCE
+-rw-r--r--   0 edouard    (501) staff       (20)     1939 2023-07-06 16:05:09.809387 loadingpy-0.0.1/PKG-INFO
+-rw-r--r--   0 edouard    (501) staff       (20)     1666 2023-07-06 15:50:10.000000 loadingpy-0.0.1/README.md
+-rw-r--r--   0 edouard    (501) staff       (20)      385 2023-07-06 16:05:00.000000 loadingpy-0.0.1/pyproject.toml
+-rw-r--r--   0 edouard    (501) staff       (20)       38 2023-07-06 16:05:09.809547 loadingpy-0.0.1/setup.cfg
+drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-06 16:05:09.807838 loadingpy-0.0.1/src/
+drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-06 16:05:09.808688 loadingpy-0.0.1/src/loadingpy/
+-rw-r--r--   0 edouard    (501) staff       (20)       31 2023-07-06 12:46:20.000000 loadingpy-0.0.1/src/loadingpy/__init__.py
+-rw-r--r--   0 edouard    (501) staff       (20)     3329 2023-07-06 16:02:08.000000 loadingpy-0.0.1/src/loadingpy/basic_bar.py
+-rw-r--r--   0 edouard    (501) staff       (20)     1500 2023-07-06 11:25:44.000000 loadingpy-0.0.1/src/loadingpy/colored_bar.py
+-rw-r--r--   0 edouard    (501) staff       (20)     3944 2023-07-06 12:40:15.000000 loadingpy-0.0.1/src/loadingpy/loading_bar.py
+drwxr-xr-x   0 edouard    (501) staff       (20)        0 2023-07-06 16:05:09.809175 loadingpy-0.0.1/src/loadingpy.egg-info/
+-rw-r--r--   0 edouard    (501) staff       (20)     1939 2023-07-06 16:05:09.000000 loadingpy-0.0.1/src/loadingpy.egg-info/PKG-INFO
+-rw-r--r--   0 edouard    (501) staff       (20)      291 2023-07-06 16:05:09.000000 loadingpy-0.0.1/src/loadingpy.egg-info/SOURCES.txt
+-rw-r--r--   0 edouard    (501) staff       (20)        1 2023-07-06 16:05:09.000000 loadingpy-0.0.1/src/loadingpy.egg-info/dependency_links.txt
+-rw-r--r--   0 edouard    (501) staff       (20)       10 2023-07-06 16:05:09.000000 loadingpy-0.0.1/src/loadingpy.egg-info/top_level.txt
```

### Comparing `loadingpy-0.0.0/LICENCE` & `loadingpy-0.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `loadingpy-0.0.0/PKG-INFO` & `loadingpy-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadingpy
-Version: 0.0.0
+Version: 0.0.1
 Summary: fancy progress bar
 Author-email: Edouard Yvinec <edouardyvinec@hotmail.fr>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `loadingpy-0.0.0/README.md` & `loadingpy-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `loadingpy-0.0.0/src/loadingpy/basic_bar.py` & `loadingpy-0.0.1/src/loadingpy/basic_bar.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class ProgressBar:
     def __init__(
         self,
         iterable: Iterable,
         total_steps: int = -1,
         base_str: str = "loop",
     ) -> None:
-        self.iterable = iterable
+        self.iterable = iter(iterable)
         self.total_steps = len(iterable) if total_steps < 0 else total_steps
         self.base_str = base_str
         self.progress_bar_size = self.get_size() - (36 - (21 - len(self.base_str)))
         self.current_progression = 0
         self.suffix_length = 11
         self.start_time = time.time()
 
@@ -85,16 +85,15 @@
         bar = self.build_bar(progression_complete=progression_complete)
         print(
             f"\r{base_string} {bar} {suffix}",
             end="" if not progression_complete else "\n",
         )
         if progression_complete:
             raise StopIteration
-        output = next(iter(self.iterable))
-        # output = self.iterable[self.current_progression]
+        output = next(self.iterable)
         self.current_progression += 1
         return output
 
 
 if __name__ == "__main__":
     a = list(range(15))
     for i in ProgressBar(a):
```

### Comparing `loadingpy-0.0.0/src/loadingpy/colored_bar.py` & `loadingpy-0.0.1/src/loadingpy/colored_bar.py`

 * *Files identical despite different names*

### Comparing `loadingpy-0.0.0/src/loadingpy/loading_bar.py` & `loadingpy-0.0.1/src/loadingpy/loading_bar.py`

 * *Files identical despite different names*

### Comparing `loadingpy-0.0.0/src/loadingpy.egg-info/PKG-INFO` & `loadingpy-0.0.1/src/loadingpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadingpy
-Version: 0.0.0
+Version: 0.0.1
 Summary: fancy progress bar
 Author-email: Edouard Yvinec <edouardyvinec@hotmail.fr>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

