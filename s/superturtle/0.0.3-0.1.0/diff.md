# Comparing `tmp/superturtle-0.0.3.tar.gz` & `tmp/superturtle-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superturtle-0.0.3.tar", max compression
+gzip compressed data, was "superturtle-0.1.0.tar", max compression
```

## Comparing `superturtle-0.0.3.tar` & `superturtle-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      354 2022-02-25 13:29:49.565158 superturtle-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       22 2022-02-18 15:24:39.342386 superturtle-0.0.3/superturtle/__init__.py
--rw-r--r--   0        0        0    14157 2022-02-25 13:28:41.154951 superturtle-0.0.3/superturtle/animation.py
--rw-r--r--   0        0        0     5186 2022-02-18 15:03:22.417356 superturtle-0.0.3/superturtle/easing.py
--rw-r--r--   0        0        0       76 2022-02-15 19:01:58.964204 superturtle-0.0.3/superturtle/fancy_drawing.py
--rw-r--r--   0        0        0      496 2022-02-18 11:46:34.191351 superturtle-0.0.3/superturtle/image.py
--rw-r--r--   0        0        0     3526 2022-02-15 19:40:45.669077 superturtle-0.0.3/superturtle/movement.py
--rw-r--r--   0        0        0     5364 2022-02-15 20:03:09.750216 superturtle-0.0.3/superturtle/stroke.py
--rw-r--r--   0        0        0     1558 2022-02-15 19:01:58.973426 superturtle-0.0.3/superturtle/test.py
--rw-r--r--   0        0        0      535 2022-02-25 13:31:02.499064 superturtle-0.0.3/setup.py
--rw-r--r--   0        0        0      330 2022-02-25 13:31:02.499301 superturtle-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1322 2023-05-30 12:15:15.132008 superturtle-0.1.0/README.md
+-rw-r--r--   0        0        0      459 2023-07-07 18:40:36.420182 superturtle-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-30 12:15:15.159236 superturtle-0.1.0/superturtle/__init__.py
+-rw-r--r--   0        0        0    14157 2023-05-30 12:15:15.160769 superturtle-0.1.0/superturtle/animation.py
+-rw-r--r--   0        0        0     5186 2023-05-30 12:15:15.161962 superturtle-0.1.0/superturtle/easing.py
+-rw-r--r--   0        0        0       76 2022-02-15 19:01:58.964204 superturtle-0.1.0/superturtle/fancy_drawing.py
+-rw-r--r--   0        0        0      496 2023-05-30 12:15:15.163141 superturtle-0.1.0/superturtle/image.py
+-rw-r--r--   0        0        0     3548 2023-05-30 12:15:15.164690 superturtle-0.1.0/superturtle/movement.py
+-rw-r--r--   0        0        0     5371 2023-05-30 12:15:15.165869 superturtle-0.1.0/superturtle/stroke.py
+-rw-r--r--   0        0        0     1558 2022-02-15 19:01:58.973426 superturtle-0.1.0/superturtle/test.py
+-rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 superturtle-0.1.0/PKG-INFO
```

### Comparing `superturtle-0.0.3/superturtle/animation.py` & `superturtle-0.1.0/superturtle/animation.py`

 * *Files identical despite different names*

### Comparing `superturtle-0.0.3/superturtle/easing.py` & `superturtle-0.1.0/superturtle/easing.py`

 * *Files identical despite different names*

### Comparing `superturtle-0.0.3/superturtle/movement.py` & `superturtle-0.1.0/superturtle/movement.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class restore_state_when_finished:
     """
     A context manager which records the turtle's position and heading
     at the beginning and restores them at the end of the code block.
     For example::
 
         from turtle import forward, right
-        from helpers import restore_state_when_finished
+        from superturtle.movement import restore_state_when_finished
         for angle in range(0, 360, 15):
             with restore_state_when_finished():
                 right(angle)
                 forward(100)
     """
 
     def __enter__(self):
@@ -86,16 +86,16 @@
         pendown()
 
 class no_delay:
     """A context manager which causes drawing code to run instantly.
 
        For example::
 
-           from movement import fly, no_delay
         from turtle import forward, right
+        from superturtle.movement import fly, no_delay
         fly(-150, 150)
         with no_delay():
             for i in range(720):
                 forward(300)
                 right(71)
         input()
     """
```

### Comparing `superturtle-0.0.3/superturtle/stroke.py` & `superturtle-0.1.0/superturtle/stroke.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         colors (list): (Optional) A sequence of color names (any valid inputs to 
             turtle.setcolor). By default, uses a rainbow.
 
     ::
 
         from turtle import forward
         from superturtle.stroke import rainbow
-        with rainbow(["black", "grey", "white"]):
+        with rainbow(colors=["black", "grey", "white"]):
             forward(60)
     """
 
     default_colors = ['red', 'orange', 'yellow', 'green', 'blue', 'purple']
     
     def __init__(self, spacing=10, colors=None):
         self.spacing = spacing
```

### Comparing `superturtle-0.0.3/superturtle/test.py` & `superturtle-0.1.0/superturtle/test.py`

 * *Files identical despite different names*

