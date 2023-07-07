# Comparing `tmp/flet_timer-0.0.6.tar.gz` & `tmp/flet_timer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_timer-0.0.6.tar", last modified: Thu Jul  6 16:12:39 2023, max compression
+gzip compressed data, was "flet_timer-0.0.8.tar", last modified: Thu Jul  6 16:43:54 2023, max compression
```

## Comparing `flet_timer-0.0.6.tar` & `flet_timer-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:12:39.536335 flet_timer-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-06 16:12:31.000000 flet_timer-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 16:12:39.536335 flet_timer-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 16:12:31.000000 flet_timer-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:12:39.532335 flet_timer-0.0.6/flet_timer/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 16:12:31.000000 flet_timer-0.0.6/flet_timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-06 16:12:31.000000 flet_timer-0.0.6/flet_timer/flet_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:12:39.536335 flet_timer-0.0.6/flet_timer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 16:12:39.000000 flet_timer-0.0.6/flet_timer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-06 16:12:39.000000 flet_timer-0.0.6/flet_timer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:12:39.000000 flet_timer-0.0.6/flet_timer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:12:39.000000 flet_timer-0.0.6/flet_timer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 16:12:39.000000 flet_timer-0.0.6/flet_timer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 16:12:39.000000 flet_timer-0.0.6/flet_timer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:12:39.536335 flet_timer-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-06 16:12:31.000000 flet_timer-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:43:54.516300 flet_timer-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-06 16:43:45.000000 flet_timer-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 16:43:54.516300 flet_timer-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-06 16:43:45.000000 flet_timer-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:43:54.516300 flet_timer-0.0.8/flet_timer/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 16:43:45.000000 flet_timer-0.0.8/flet_timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-06 16:43:45.000000 flet_timer-0.0.8/flet_timer/flet_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:43:54.516300 flet_timer-0.0.8/flet_timer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 16:43:54.000000 flet_timer-0.0.8/flet_timer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-06 16:43:54.000000 flet_timer-0.0.8/flet_timer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:43:54.000000 flet_timer-0.0.8/flet_timer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:43:54.000000 flet_timer-0.0.8/flet_timer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 16:43:54.000000 flet_timer-0.0.8/flet_timer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 16:43:54.000000 flet_timer-0.0.8/flet_timer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:43:54.516300 flet_timer-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-06 16:43:45.000000 flet_timer-0.0.8/setup.py
```

### Comparing `flet_timer-0.0.6/LICENSE` & `flet_timer-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_timer-0.0.6/flet_timer/flet_timer.py` & `flet_timer-0.0.8/flet_timer/flet_timer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import threading
 
 import flet as ft
 from interval_timer import IntervalTimer
 
 
 class Timer(ft.UserControl):
-    def __init__(self, name, interval_s, callback, *args, **kwargs):
+    def __init__(self, name="Timer", interval_s=1, callback=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
-
         self.name = name
         self.interval_s = interval_s
         self.callback = callback
         self.active = False
         self.th = threading.Thread(target=self.tick, daemon=True)
-
-        print(f"Timer {self.name} created")
+        if callback is None:
+            self.callback = lambda: print(f"Timer {self.name} ticked")
 
     def did_mount(self):
         self.start()
         self.th.start()
 
     def start(self):
         self.active = True
@@ -35,11 +34,9 @@
             except Exception as e:
                 print(e)
 
     def build(self):
         return ft.Container(padding=0, margin=0)
 
     def will_unmount(self):
-        print(f"Disposing timer {self.name}")
         self.stop()
-        # self.th.join()
         super().will_unmount()
```

### Comparing `flet_timer-0.0.6/setup.py` & `flet_timer-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,10 +15,10 @@
     install_requires=requirements,
     license="MIT license",
     include_package_data=True,
     keywords='flet_timer',
     name='flet_timer',
     packages=find_packages(include=['flet_timer', 'flet_timer.*']),
     url='https://github.com/panos-stavrianos/flet_timer',
-    version='0.0.6',
+    version='0.0.8',
     zip_safe=False,
 )
```

