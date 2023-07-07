# Comparing `tmp/irene_pro-0.0.86.tar.gz` & `tmp/irene_pro-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.86.tar", last modified: Thu Jul  6 14:05:21 2023, max compression
+gzip compressed data, was "irene_pro-0.0.87.tar", last modified: Thu Jul  6 14:14:46 2023, max compression
```

## Comparing `irene_pro-0.0.86.tar` & `irene_pro-0.0.87.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 14:05:21.738884 irene_pro-0.0.86/
--rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.86/LICENSE
--rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.86/MANIFEST.in
--rw-rw-rw-   0        0        0     1280 2023-07-06 14:05:21.735890 irene_pro-0.0.86/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.86/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 14:05:21.702979 irene_pro-0.0.86/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.86/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     8188 2023-07-06 14:04:14.000000 irene_pro-0.0.86/irene_pro/logics.py
--rw-rw-rw-   0        0        0    35895 2023-07-06 13:53:43.000000 irene_pro-0.0.86/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-06 14:05:21.729908 irene_pro-0.0.86/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1280 2023-07-06 14:05:21.000000 irene_pro-0.0.86/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-06 14:05:21.000000 irene_pro-0.0.86/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 14:05:21.000000 irene_pro-0.0.86/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-06 14:05:21.000000 irene_pro-0.0.86/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 14:05:21.000000 irene_pro-0.0.86/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 14:05:21.739895 irene_pro-0.0.86/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-07-06 14:04:25.000000 irene_pro-0.0.86/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 14:14:46.260631 irene_pro-0.0.87/
+-rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.87/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.87/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-07-06 14:14:46.256529 irene_pro-0.0.87/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.87/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 14:14:46.214571 irene_pro-0.0.87/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.87/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     8188 2023-07-06 14:04:14.000000 irene_pro-0.0.87/irene_pro/logics.py
+-rw-rw-rw-   0        0        0    36055 2023-07-06 14:13:24.000000 irene_pro-0.0.87/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-06 14:14:46.249544 irene_pro-0.0.87/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-07-06 14:14:46.000000 irene_pro-0.0.87/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-06 14:14:46.000000 irene_pro-0.0.87/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 14:14:46.000000 irene_pro-0.0.87/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-06 14:14:46.000000 irene_pro-0.0.87/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 14:14:46.000000 irene_pro-0.0.87/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 14:14:46.261770 irene_pro-0.0.87/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-07-06 14:13:52.000000 irene_pro-0.0.87/setup.py
```

### Comparing `irene_pro-0.0.86/PKG-INFO` & `irene_pro-0.0.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.86
+Version: 0.0.87
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.86/README.md` & `irene_pro-0.0.87/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.86/irene_pro/logics.py` & `irene_pro-0.0.87/irene_pro/logics.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.86/irene_pro/widgets.py` & `irene_pro-0.0.87/irene_pro/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,20 +210,27 @@
         elif "print" in str(self['text']).lower():
             self.config(bg = "#FEE3B8", image = image)
             prev_color = self.cget('bg')
         
         elif "plan" in str(self['text']).lower():
             self.config(bg = "#600", fg = "#fff", image = image)
             prev_color = self.cget('bg')
-
-        if " all" in str(self['text']).lower():
+            
+        elif " all" in str(self['text']).lower():
             self.config(image = image)
         
-        if " id" in str(self['text']).lower():
+        elif " id" in str(self['text']).lower():
             self.config(image = image)
+        else:
+            try:
+                prev_color = self.cget('bg')
+            except Exception:
+                pass
+
+        
         
         self.bind('<Enter>', lambda e: self.config(bg = '#FF78C4'))
         self.bind('<Leave>', lambda e: self.config(bg = prev_color))
     
 
 class Display_image:
     def __init__(self, *args, **kwargs):
```

### Comparing `irene_pro-0.0.86/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.87/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.86
+Version: 0.0.87
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.86/setup.py` & `irene_pro-0.0.87/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3836 270d 0a44 4553 4352   '0.0.86'..DESCR
+00000100: 2027 302e 302e 3837 270d 0a44 4553 4352   '0.0.87'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

