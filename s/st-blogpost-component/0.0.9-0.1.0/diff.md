# Comparing `tmp/st_blogpost_component-0.0.9.tar.gz` & `tmp/st_blogpost_component-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_blogpost_component-0.0.9.tar", last modified: Tue Jul  4 21:01:59 2023, max compression
+gzip compressed data, was "st_blogpost_component-0.1.0.tar", last modified: Thu Jul  6 22:27:10 2023, max compression
```

## Comparing `st_blogpost_component-0.0.9.tar` & `st_blogpost_component-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 21:01:59.754145 st_blogpost_component-0.0.9/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1063 2023-07-04 03:12:34.000000 st_blogpost_component-0.0.9/LICENSE
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       57 2023-07-04 04:48:07.000000 st_blogpost_component-0.0.9/MANIFEST.in
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 21:01:59.754145 st_blogpost_component-0.0.9/PKG-INFO
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       38 2023-07-04 21:01:59.754145 st_blogpost_component-0.0.9/setup.cfg
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      628 2023-07-04 21:01:47.000000 st_blogpost_component-0.0.9/setup.py
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 21:01:59.746145 st_blogpost_component-0.0.9/st_blogpost_component/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     4519 2023-07-04 21:01:41.000000 st_blogpost_component-0.0.9/st_blogpost_component/__init__.py
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 21:01:59.746145 st_blogpost_component-0.0.9/st_blogpost_component/frontend/
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 21:01:59.750145 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      691 2023-07-04 21:00:08.000000 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/asset-manifest.json
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   197459 2023-07-04 20:59:50.000000 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/bootstrap.min.css
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2087 2023-07-04 21:00:08.000000 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/index.html
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 21:01:59.746145 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 21:01:59.754145 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   557241 2023-07-04 21:00:08.000000 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2243 2023-07-04 21:00:08.000000 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js.LICENSE.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)  2141256 2023-07-04 21:00:08.000000 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js.map
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2524 2023-07-04 21:00:08.000000 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/main.bbd810e7.chunk.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     7179 2023-07-04 21:00:08.000000 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/main.bbd810e7.chunk.js.map
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1584 2023-07-04 21:00:08.000000 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     8369 2023-07-04 21:00:08.000000 st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 21:01:59.746145 st_blogpost_component-0.0.9/st_blogpost_component.egg-info/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 21:01:59.000000 st_blogpost_component-0.0.9/st_blogpost_component.egg-info/PKG-INFO
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      955 2023-07-04 21:01:59.000000 st_blogpost_component-0.0.9/st_blogpost_component.egg-info/SOURCES.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)        1 2023-07-04 21:01:59.000000 st_blogpost_component-0.0.9/st_blogpost_component.egg-info/dependency_links.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       16 2023-07-04 21:01:59.000000 st_blogpost_component-0.0.9/st_blogpost_component.egg-info/requires.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       22 2023-07-04 21:01:59.000000 st_blogpost_component-0.0.9/st_blogpost_component.egg-info/top_level.txt
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-06 22:27:10.945840 st_blogpost_component-0.1.0/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1063 2023-07-04 03:12:34.000000 st_blogpost_component-0.1.0/LICENSE
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       57 2023-07-04 04:48:07.000000 st_blogpost_component-0.1.0/MANIFEST.in
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-06 22:27:10.945840 st_blogpost_component-0.1.0/PKG-INFO
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       38 2023-07-06 22:27:10.945840 st_blogpost_component-0.1.0/setup.cfg
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      628 2023-07-06 22:24:35.000000 st_blogpost_component-0.1.0/setup.py
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-06 22:27:10.937839 st_blogpost_component-0.1.0/st_blogpost_component/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     3590 2023-07-06 22:24:12.000000 st_blogpost_component-0.1.0/st_blogpost_component/__init__.py
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-06 22:27:10.937839 st_blogpost_component-0.1.0/st_blogpost_component/frontend/
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-06 22:27:10.941839 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      691 2023-07-06 22:24:08.000000 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/asset-manifest.json
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   197459 2023-07-06 22:23:42.000000 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/bootstrap.min.css
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2087 2023-07-06 22:24:08.000000 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/index.html
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-06 22:27:10.937839 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-06 22:27:10.945840 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   557241 2023-07-06 22:24:08.000000 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2243 2023-07-06 22:24:08.000000 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js.LICENSE.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)  2141256 2023-07-06 22:24:08.000000 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js.map
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2541 2023-07-06 22:24:08.000000 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/main.ecb92db9.chunk.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     7255 2023-07-06 22:24:08.000000 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/main.ecb92db9.chunk.js.map
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1584 2023-07-06 22:24:08.000000 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     8369 2023-07-06 22:24:08.000000 st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-06 22:27:10.941839 st_blogpost_component-0.1.0/st_blogpost_component.egg-info/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-06 22:27:10.000000 st_blogpost_component-0.1.0/st_blogpost_component.egg-info/PKG-INFO
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      955 2023-07-06 22:27:10.000000 st_blogpost_component-0.1.0/st_blogpost_component.egg-info/SOURCES.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)        1 2023-07-06 22:27:10.000000 st_blogpost_component-0.1.0/st_blogpost_component.egg-info/dependency_links.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       16 2023-07-06 22:27:10.000000 st_blogpost_component-0.1.0/st_blogpost_component.egg-info/requires.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       22 2023-07-06 22:27:10.000000 st_blogpost_component-0.1.0/st_blogpost_component.egg-info/top_level.txt
```

### Comparing `st_blogpost_component-0.0.9/LICENSE` & `st_blogpost_component-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.9/setup.py` & `st_blogpost_component-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_blogpost_component",
-    version="0.0.9",
+    version="0.1.0",
     author="YM",
     author_email="",
     description="",
     long_description="custom component to display blog post card for personal blog",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/__init__.py` & `st_blogpost_component-0.1.0/st_blogpost_component/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -202,82 +202,24 @@
 00000c90: 2020 2320 4372 6561 7465 2061 6e20 696e    # Create an in
 00000ca0: 7374 616e 6365 206f 6620 6f75 7220 636f  stance of our co
 00000cb0: 6d70 6f6e 656e 7420 7769 7468 2061 2063  mponent with a c
 00000cc0: 6f6e 7374 616e 7420 606e 616d 6560 2061  onstant `name` a
 00000cd0: 7267 2c20 616e 640a 2020 2020 2320 7072  rg, and.    # pr
 00000ce0: 696e 7420 6974 7320 6f75 7470 7574 2076  int its output v
 00000cf0: 616c 7565 0a20 2020 2023 7072 696e 7428  alue.    #print(
-00000d00: 7572 6c29 0a20 2020 200a 2020 2020 7265  url).    .    re
-00000d10: 7370 6f6e 7365 203d 2072 6571 7565 7374  sponse = request
-00000d20: 732e 6765 7428 2268 7474 7073 3a2f 2f70  s.get("https://p
-00000d30: 6572 736f 6e61 6c2d 7369 7465 2d62 6163  ersonal-site-bac
-00000d40: 6b65 6e64 2d70 726f 6475 6374 696f 6e2e  kend-production.
-00000d50: 7570 2e72 6169 6c77 6179 2e61 7070 2f70  up.railway.app/p
-00000d60: 726f 6a65 6374 7322 290a 2020 2020 6966  rojects").    if
-00000d70: 2072 6573 706f 6e73 653a 0a20 2020 2020   response:.     
-00000d80: 2020 2072 6573 706f 6e73 6520 3d20 7265     response = re
-00000d90: 7370 6f6e 7365 2e6a 736f 6e28 290a 2020  sponse.json().  
-00000da0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00000db0: 616e 6765 2830 2c6c 656e 2872 6573 706f  ange(0,len(respo
-00000dc0: 6e73 6529 2c35 293a 0a20 2020 2020 2020  nse),5):.       
-00000dd0: 2020 2020 2063 6f6c 7320 3d20 7374 2e63       cols = st.c
-00000de0: 6f6c 756d 6e73 2835 290a 2020 2020 2020  olumns(5).      
-00000df0: 2020 2020 2020 6966 2069 2025 2035 203d        if i % 5 =
-00000e00: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00000e10: 2020 2020 2077 6974 6820 636f 6c73 5b30       with cols[0
-00000e20: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00000e30: 2020 2020 2020 2078 3120 3d20 626c 6f67         x1 = blog
-00000e40: 5f63 6172 645f 636f 6d70 6f6e 656e 7428  _card_component(
-00000e50: 2a2a 7265 7370 6f6e 7365 5b69 5d29 0a20  **response[i]). 
-00000e60: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
-00000e70: 2b20 3120 3c20 6c65 6e28 7265 7370 6f6e  + 1 < len(respon
-00000e80: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
-00000e90: 2020 2020 2077 6974 6820 636f 6c73 5b31       with cols[1
-00000ea0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00000eb0: 2020 2020 2020 2078 3120 3d20 626c 6f67         x1 = blog
-00000ec0: 5f63 6172 645f 636f 6d70 6f6e 656e 7428  _card_component(
-00000ed0: 2a2a 7265 7370 6f6e 7365 5b69 2b31 5d29  **response[i+1])
-00000ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ef0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00000f00: 2020 6966 2069 202b 2032 203c 206c 656e    if i + 2 < len
-00000f10: 2872 6573 706f 6e73 6529 3a0a 2020 2020  (response):.    
-00000f20: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00000f30: 2063 6f6c 735b 325d 3a0a 2020 2020 2020   cols[2]:.      
-00000f40: 2020 2020 2020 2020 2020 2020 2020 7831                x1
-00000f50: 203d 2062 6c6f 675f 6361 7264 5f63 6f6d   = blog_card_com
-00000f60: 706f 6e65 6e74 282a 2a72 6573 706f 6e73  ponent(**respons
-00000f70: 655b 692b 325d 290a 2020 2020 2020 2020  e[i+2]).        
-00000f80: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00000f90: 2020 2020 2020 2020 2069 6620 6920 2b20           if i + 
-00000fa0: 3320 3c20 6c65 6e28 7265 7370 6f6e 7365  3 < len(response
-00000fb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00000fc0: 2020 2077 6974 6820 636f 6c73 5b33 5d3a     with cols[3]:
-00000fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000fe0: 2020 2020 2078 3120 3d20 626c 6f67 5f63       x1 = blog_c
-00000ff0: 6172 645f 636f 6d70 6f6e 656e 7428 2a2a  ard_component(**
-00001000: 7265 7370 6f6e 7365 5b69 2b33 5d29 0a20  response[i+3]). 
-00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00001030: 6966 2069 202b 2034 203c 206c 656e 2872  if i + 4 < len(r
-00001040: 6573 706f 6e73 6529 3a0a 2020 2020 2020  esponse):.      
-00001050: 2020 2020 2020 2020 2020 7769 7468 2063            with c
-00001060: 6f6c 735b 345d 3a0a 2020 2020 2020 2020  ols[4]:.        
-00001070: 2020 2020 2020 2020 2020 2020 7831 203d              x1 =
-00001080: 2062 6c6f 675f 6361 7264 5f63 6f6d 706f   blog_card_compo
-00001090: 6e65 6e74 282a 2a72 6573 706f 6e73 655b  nent(**response[
-000010a0: 692b 345d 290a 2020 2020 2020 2020 2020  i+4]).          
-000010b0: 2020 2020 2020 2020 2020 0a20 2020 2068            .    h
-000010c0: 6964 655f 7374 7265 616d 6c69 745f 7374  ide_streamlit_st
-000010d0: 796c 6520 3d20 2222 220a 2020 2020 2020  yle = """.      
-000010e0: 2020 2020 2020 3c73 7479 6c65 3e0a 2020        <style>.  
-000010f0: 2020 2020 2020 2020 2020 234d 6169 6e4d            #MainM
-00001100: 656e 7520 7b76 6973 6962 696c 6974 793a  enu {visibility:
-00001110: 2068 6964 6465 6e3b 7d0a 2020 2020 2020   hidden;}.      
-00001120: 2020 2020 2020 666f 6f74 6572 207b 7669        footer {vi
-00001130: 7369 6269 6c69 7479 3a20 6869 6464 656e  sibility: hidden
-00001140: 3b7d 0a20 2020 2020 2020 2020 2020 203c  ;}.            <
-00001150: 2f73 7479 6c65 3e0a 2020 2020 2020 2020  /style>.        
-00001160: 2020 2020 2222 220a 2020 2020 7374 2e6d      """.    st.m
-00001170: 6172 6b64 6f77 6e28 6869 6465 5f73 7472  arkdown(hide_str
-00001180: 6561 6d6c 6974 5f73 7479 6c65 2c20 756e  eamlit_style, un
-00001190: 7361 6665 5f61 6c6c 6f77 5f68 746d 6c3d  safe_allow_html=
-000011a0: 5472 7565 2920 0a                        True) .
+00000d00: 7572 6c29 0a20 2020 2020 2020 2020 2020  url).           
+00000d10: 2020 2020 2020 2020 200a 2020 2020 6869           .    hi
+00000d20: 6465 5f73 7472 6561 6d6c 6974 5f73 7479  de_streamlit_sty
+00000d30: 6c65 203d 2022 2222 0a20 2020 2020 2020  le = """.       
+00000d40: 2020 2020 203c 7374 796c 653e 0a20 2020       <style>.   
+00000d50: 2020 2020 2020 2020 2023 4d61 696e 4d65           #MainMe
+00000d60: 6e75 207b 7669 7369 6269 6c69 7479 3a20  nu {visibility: 
+00000d70: 6869 6464 656e 3b7d 0a20 2020 2020 2020  hidden;}.       
+00000d80: 2020 2020 2066 6f6f 7465 7220 7b76 6973       footer {vis
+00000d90: 6962 696c 6974 793a 2068 6964 6465 6e3b  ibility: hidden;
+00000da0: 7d0a 2020 2020 2020 2020 2020 2020 3c2f  }.            </
+00000db0: 7374 796c 653e 0a20 2020 2020 2020 2020  style>.         
+00000dc0: 2020 2022 2222 0a20 2020 2073 742e 6d61     """.    st.ma
+00000dd0: 726b 646f 776e 2868 6964 655f 7374 7265  rkdown(hide_stre
+00000de0: 616d 6c69 745f 7374 796c 652c 2075 6e73  amlit_style, uns
+00000df0: 6166 655f 616c 6c6f 775f 6874 6d6c 3d54  afe_allow_html=T
+00000e00: 7275 6529 200a                           rue) .
```

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/asset-manifest.json` & `st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/asset-manifest.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.84375%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.ecb92db9.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.ecb92db9.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.ecb92db9.chunk.js.map'}"}*

```diff
@@ -1,17 +1,17 @@
 {
     "entrypoints": [
         "static/js/runtime-main.0f051bbb.js",
         "static/js/2.115577ef.chunk.js",
-        "static/js/main.bbd810e7.chunk.js"
+        "static/js/main.ecb92db9.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.bbd810e7.chunk.js",
-        "main.js.map": "./static/js/main.bbd810e7.chunk.js.map",
+        "main.js": "./static/js/main.ecb92db9.chunk.js",
+        "main.js.map": "./static/js/main.ecb92db9.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.0f051bbb.js",
         "runtime-main.js.map": "./static/js/runtime-main.0f051bbb.js.map",
         "static/js/2.115577ef.chunk.js": "./static/js/2.115577ef.chunk.js",
         "static/js/2.115577ef.chunk.js.LICENSE.txt": "./static/js/2.115577ef.chunk.js.LICENSE.txt",
         "static/js/2.115577ef.chunk.js.map": "./static/js/2.115577ef.chunk.js.map"
     }
 }
```

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/bootstrap.min.css` & `st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/index.html` & `st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,p=t[0],f=t[1],i=t[2],c=0,s=[];c<p.length;c++)l=p[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in f)Object.prototype.hasOwnProperty.call(f,n)&&(e[n]=f[n]);for(a&&a(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,p=1;p<r.length;p++){var f=r[p];0!==o[f]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var p=this.webpackJsonpst_blogpost_component=this.webpackJsonpst_blogpost_component||[],f=p.push.bind(p);p.push=t,p=p.slice();for(var i=0;i<p.length;i++)t(p[i]);var a=f;r()}([])</script><script src="./static/js/2.115577ef.chunk.js"></script><script src="./static/js/main.bbd810e7.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,p=t[0],f=t[1],i=t[2],c=0,s=[];c<p.length;c++)l=p[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in f)Object.prototype.hasOwnProperty.call(f,n)&&(e[n]=f[n]);for(a&&a(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,p=1;p<r.length;p++){var f=r[p];0!==o[f]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var p=this.webpackJsonpst_blogpost_component=this.webpackJsonpst_blogpost_component||[],f=p.push.bind(p);p.push=t,p=p.slice();for(var i=0;i<p.length;i++)t(p[i]);var a=f;r()}([])</script><script src="./static/js/2.115577ef.chunk.js"></script><script src="./static/js/main.ecb92db9.chunk.js"></script></body></html>
```

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js` & `st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js.LICENSE.txt` & `st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js.map` & `st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/main.bbd810e7.chunk.js` & `st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/main.ecb92db9.chunk.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,52 +1,52 @@
 (this.webpackJsonpst_blogpost_component = this.webpackJsonpst_blogpost_component || []).push([
     [0], {
         67: function(e, t, n) {
             "use strict";
             n.r(t);
             var i = n(4),
-                r = n.n(i),
-                s = n(53),
-                o = n.n(s),
+                s = n.n(i),
+                r = n(53),
+                o = n.n(r),
                 a = n(0),
                 c = n(1),
                 h = n(23),
                 l = n(2),
                 d = n(3),
                 u = n(47),
                 p = n(92),
                 b = n(95),
                 j = n(96),
                 g = n(97),
                 f = n(94),
-                O = n(98),
-                w = n(91),
+                w = n(98),
+                O = n(91),
                 m = n(9),
                 W = function() {
                     var e = window;
                     return {
                         innerWidth: e.innerWidth,
                         innerHeight: e.innerHeight
                     }
                 },
-                v = function(e) {
+                _ = function(e) {
                     Object(l.a)(n, e);
                     var t = Object(d.a)(n);
 
                     function n(e) {
                         var i;
                         return Object(a.a)(this, n), (i = t.call(this, e)).state = {
                             url: null,
                             height: 0
                         }, i.render = function() {
                             var e = i.props.args.title,
                                 t = i.props.args.subtitle,
                                 n = i.props.args.description,
-                                r = i.props.args.url,
-                                s = i.props.args.github,
+                                s = i.props.args.url,
+                                r = i.props.args.github,
                                 o = i.props.args.img_path,
                                 a = i.props.args.post,
                                 c = i.props.args.date,
                                 h = {
                                     minWidth: "100",
                                     maxWidth: "100",
                                     transitionDuration: "0.3s",
@@ -69,38 +69,38 @@
                                     }), Object(m.jsxs)(g.a, {
                                         children: [t && Object(m.jsx)(b.a, {
                                             subheader: t
                                         }), n && Object(m.jsx)(f.a, {
                                             variant: "body2",
                                             children: n
                                         })]
-                                    }), Object(m.jsxs)(O.a, {
+                                    }), Object(m.jsxs)(w.a, {
                                         disableSpacing: !0,
-                                        children: [s && Object(m.jsx)(w.a, {
+                                        children: [r && Object(m.jsx)(O.a, {
                                             size: "small",
                                             onClick: function() {
-                                                return window.open(s, "_blank")
+                                                return window.open(r, "_blank")
                                             },
                                             children: "github"
-                                        }), r && Object(m.jsx)(w.a, {
+                                        }), s && Object(m.jsx)(O.a, {
                                             size: "small",
                                             onClick: function() {
-                                                return window.open(r, "_blank")
+                                                return window.open(s, "_blank")
                                             },
                                             children: "link"
-                                        }), a && Object(m.jsx)(w.a, {
+                                        }), a && Object(m.jsx)(O.a, {
                                             size: "small",
                                             onClick: function() {
-                                                return i.setState((function() {
+                                                i.setState((function() {
                                                     return {
                                                         url: a
                                                     }
                                                 }), (function() {
                                                     return u.a.setComponentValue(i.state.url)
-                                                }))
+                                                })), window.open(a, "_blank")
                                             },
                                             children: "Open Article"
                                         })]
                                     })]
                                 })
                             })
                         }, i._handleWindowResize = i._handleWindowResize.bind(Object(h.a)(i)), i
@@ -134,18 +134,18 @@
                                 return {
                                     height: Math.floor(450)
                                 }
                             })), console.log(W()), console.log(this.state.height)
                         }
                     }]), n
                 }(u.b),
-                x = Object(u.c)(v);
-            o.a.render(Object(m.jsx)(r.a.StrictMode, {
-                children: Object(m.jsx)(x, {})
+                v = Object(u.c)(_);
+            o.a.render(Object(m.jsx)(s.a.StrictMode, {
+                children: Object(m.jsx)(v, {})
             }), document.getElementById("root"))
         }
     },
     [
         [67, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.bbd810e7.chunk.js.map
+//# sourceMappingURL=main.ecb92db9.chunk.js.map
```

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/main.bbd810e7.chunk.js.map` & `st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/main.ecb92db9.chunk.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8095238095238095%*

 * *Differences: {"'file'": "'static/js/main.ecb92db9.chunk.js'",*

 * * "'mappings'": "'sRAeMA,EAAgB,WACpB,IAAAC,EAAoCC,OACpC,MAAO,CAAEC,WADSF,EAAVE,WACaC,YADUH,EAAXG,YAEtB,EACMC,EAAa,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GACjB,SAAAA,EAAYK,GAAa,IAADC,EAEwC,OAFxCC,YAAA,KAAAP,IACtBM,EAAAH,EAAAK,KAAA,KAAMH,IAGDI,MAAQ,CAAEC,IAAK,KAAMC,OAAQ,GAAGL,EAgChCM,OAAS,WAGd,IAAMC,EAAQP,EAAKD,MAAMS,KAAY,MAC/BC,EAAWT,EAAKD,MAAMS,KAAe,SACrCE,EAAOV,EAAKD,MAAMS,KAAkB,YACpCG,EAAOX,EAAKD,MAAMS,KAAU,IAC5BI,EAASZ,EAAKD,MAAMS,KAAa,OACjCK,EAAWb, […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.bbd810e7.chunk.js",
-    "mappings": "sRAeMA,EAAgB,WACpB,IAAAC,EAAoCC,OACpC,MAAO,CAAEC,WADSF,EAAVE,WACaC,YADUH,EAAXG,YAEtB,EACMC,EAAa,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GACjB,SAAAA,EAAYK,GAAa,IAADC,EAEwC,OAFxCC,YAAA,KAAAP,IACtBM,EAAAH,EAAAK,KAAA,KAAMH,IAGDI,MAAQ,CAAEC,IAAK,KAAMC,OAAQ,GAAGL,EAgChCM,OAAS,WAGd,IAAMC,EAAQP,EAAKD,MAAMS,KAAY,MAC/BC,EAAWT,EAAKD,MAAMS,KAAe,SACrCE,EAAOV,EAAKD,MAAMS,KAAkB,YACpCG,EAAOX,EAAKD,MAAMS,KAAU,IAC5BI,EAASZ,EAAKD,MAAMS,KAAa,OACjCK,EAAWb,EAAKD,MAAMS,KAAe,SACrCM,EAAOd,EAAKD,MAAMS,KAAW,KAC7BO,EAAOf,EAAKD,MAAMS,KAAW,KAC/BQ,EAAY,CACdC,SAAU,MACVC,SAAU,MACVC,mBAAoB,OACpBd,OAAQL,EAAKG,MAAME,QAGrB,OACEe,cAAA,OAAKC,MAAO,CAAEC,QAAS,UAAWC,SAChCC,eAACC,IAAI,CAACC,QAAQ,WAAWL,MAAOL,EAAUO,SAAA,CACvChB,GAASa,cAACO,IAAU,CAACpB,MAAOA,EAAOqB,UAAWb,IAC9CF,GACCO,cAACS,IAAS,CAACC,UAAU,MAAMzB,OAAO,MAAM0B,IAAKlB,IAG/CW,eAACQ,IAAW,CAAAT,SAAA,CACTd,GAAYW,cAACO,IAAU,CAACC,UAAWnB,IACnCC,GAAQU,cAACa,IAAU,CAACP,QAAQ,QAAOH,SAAEb,OAExCc,eAACU,IAAW,CAACC,gBAAc,EAAAZ,SAAA,CACxBX,GACCQ,cAACgB,IAAM,CACLC,KAAK,QACLC,QAAS,kBAAM/C,OAAOgD,KAAK3B,EAAQ,SAAS,EAACW,SAC9C,WAIFZ,GACCS,cAACgB,IAAM,CAACC,KAAK,QAAQC,QAAS,kBAAM/C,OAAOgD,KAAK5B,EAAM,SAAS,EAACY,SAAC,SAKlET,GACCM,cAACgB,IAAM,CACLC,KAAK,QACLC,QAAS,kBACPtC,EAAKwC,UACH,iBAAO,CAAEpC,IAAKU,EAAM,IACpB,kBAAM2B,IAAUC,kBAAkB1C,EAAKG,MAAMC,IAAI,GAClD,EACFmB,SACF,wBAQb,EAhGEvB,EAAK2C,oBAAsB3C,EAAK2C,oBAAoBC,KAAIC,YAAA7C,IAAMA,CAChE,CA+BC,OA/BA8C,YAAApD,EAAA,EAAAqD,IAAA,oBAAAC,MAGD,WACEzD,OAAO0D,iBAAiB,SAAUC,KAAKP,qBACvCO,KAAKP,qBACP,GAAC,CAAAI,IAAA,uBAAAC,MACD,WACEzD,OAAO4D,oBAAoB,SAAUD,KAAKP,qBAC1CO,KAAKP,qBACP,GAAC,CAAAI,IAAA,sBAAAC,MACD,WACM3D,IAAgBG,WAAa,IAC/B0D,KAAKV,UAAS,iBAAO,CACnBnC,OAAQ+C,KAAKC,MAAM,KACpB,IACQhE,IAAgBG,WAAa,IACtC0D,KAAKV,UAAS,iBAAO,CACnBnC,OAAQ+C,KAAKC,MAAM,KACpB,IACQhE,IAAgBG,WAAa,IACtC0D,KAAKV,UAAS,iBAAO,CACnBnC,OAAQ+C,KAAKC,MAAM,KACpB,IAEDH,KAAKV,UAAS,iBAAO,CACnBnC,OAAQ+C,KAAKC,MAAM,KACpB,IAEHC,QAAQC,IAAIlE,KACZiE,QAAQC,IAAIL,KAAK/C,MAAME,OACzB,KAACX,CAAA,CAnCgB,CAAS8D,KAuGbC,cAAwB/D,GCtHvCgE,IAASpD,OACPc,cAACuC,IAAMC,WAAU,CAAArC,SACfH,cAACyC,EAAQ,MAEXC,SAASC,eAAe,Q",
+    "file": "static/js/main.ecb92db9.chunk.js",
+    "mappings": "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",
     "names": [
         "getWindowSize",
         "_window",
         "window",
         "innerWidth",
         "innerHeight",
         "CardComponent",
@@ -80,12 +80,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "PostCard.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport Card from \"@mui/material/Card\"\nimport CardHeader from \"@mui/material/CardHeader\"\nimport CardMedia from \"@mui/material/CardMedia\"\nimport CardContent from \"@mui/material/CardContent\"\nimport { Typography, CardActions } from \"@mui/material\"\nimport Button from \"@mui/material/Button\"\n\n// the `render()` function is called when component is re-rendered\n\nconst getWindowSize = () => {\n  const { innerWidth, innerHeight } = window\n  return { innerWidth, innerHeight }\n}\nclass CardComponent extends StreamlitComponentBase<any> {\n  constructor(props: any) {\n    super(props)\n    this._handleWindowResize = this._handleWindowResize.bind(this)\n  }\n  public state = { url: null, height: 0 }\n\n  componentDidMount() {\n    window.addEventListener(\"resize\", this._handleWindowResize)\n    this._handleWindowResize()\n  }\n  componentWillUnmount() {\n    window.removeEventListener(\"resize\", this._handleWindowResize)\n    this._handleWindowResize()\n  }\n  _handleWindowResize() {\n    if (getWindowSize().innerWidth < 200) {\n      this.setState(() => ({\n        height: Math.floor(700),\n      }))\n    } else if (getWindowSize().innerWidth < 300) {\n      this.setState(() => ({\n        height: Math.floor(600),\n      }))\n    } else if (getWindowSize().innerWidth < 440) {\n      this.setState(() => ({\n        height: Math.floor(500),\n      }))\n    } else {\n      this.setState(() => ({\n        height: Math.floor(450),\n      }))\n    }\n    console.log(getWindowSize())\n    console.log(this.state.height)\n  }\n\n  public render = (): ReactNode => {\n    // Arguments that are passed to the plugin in Python are accessible\n    // via `this.props.args`\n    const title = this.props.args[\"title\"]\n    const subtitle = this.props.args[\"subtitle\"]\n    const body = this.props.args[\"description\"]\n    const link = this.props.args[\"url\"]\n    const github = this.props.args[\"github\"]\n    const img_link = this.props.args[\"img_path\"]\n    const post = this.props.args[\"post\"]\n    const date = this.props.args[\"date\"]\n    var cardStyle = {\n      minWidth: \"100\",\n      maxWidth: \"100\",\n      transitionDuration: \"0.3s\",\n      height: this.state.height,\n    }\n\n    return (\n      <div style={{ padding: \"0.5rem\" }}>\n        <Card variant=\"outlined\" style={cardStyle}>\n          {title && <CardHeader title={title} subheader={date} />}\n          {img_link && (\n            <CardMedia component=\"img\" height=\"200\" src={img_link} />\n          )}\n\n          <CardContent>\n            {subtitle && <CardHeader subheader={subtitle} />}\n            {body && <Typography variant=\"body2\">{body}</Typography>}\n          </CardContent>\n          <CardActions disableSpacing>\n            {github && (\n              <Button\n                size=\"small\"\n                onClick={() => window.open(github, \"_blank\")}\n              >\n                github\n              </Button>\n            )}\n            {link && (\n              <Button size=\"small\" onClick={() => window.open(link, \"_blank\")}>\n                link\n              </Button>\n            )}\n\n            {post && (\n              <Button\n                size=\"small\"\n                onClick={() =>\n                  this.setState(\n                    () => ({ url: post }),\n                    () => Streamlit.setComponentValue(this.state.url)\n                  )\n                }\n              >\n                Open Article\n              </Button>\n            )}\n          </CardActions>\n        </Card>\n      </div>\n    )\n  }\n}\n\n// connection between component and Streamlit\nexport default withStreamlitConnection(CardComponent)\n",
+        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport Card from \"@mui/material/Card\"\nimport CardHeader from \"@mui/material/CardHeader\"\nimport CardMedia from \"@mui/material/CardMedia\"\nimport CardContent from \"@mui/material/CardContent\"\nimport { Typography, CardActions } from \"@mui/material\"\nimport Button from \"@mui/material/Button\"\n\n// the `render()` function is called when component is re-rendered\n\nconst getWindowSize = () => {\n  const { innerWidth, innerHeight } = window\n  return { innerWidth, innerHeight }\n}\nclass CardComponent extends StreamlitComponentBase<any> {\n  constructor(props: any) {\n    super(props)\n    this._handleWindowResize = this._handleWindowResize.bind(this)\n  }\n  public state = { url: null, height: 0 }\n\n  componentDidMount() {\n    window.addEventListener(\"resize\", this._handleWindowResize)\n    this._handleWindowResize()\n  }\n  componentWillUnmount() {\n    window.removeEventListener(\"resize\", this._handleWindowResize)\n    this._handleWindowResize()\n  }\n  _handleWindowResize() {\n    if (getWindowSize().innerWidth < 200) {\n      this.setState(() => ({\n        height: Math.floor(700),\n      }))\n    } else if (getWindowSize().innerWidth < 300) {\n      this.setState(() => ({\n        height: Math.floor(600),\n      }))\n    } else if (getWindowSize().innerWidth < 440) {\n      this.setState(() => ({\n        height: Math.floor(500),\n      }))\n    } else {\n      this.setState(() => ({\n        height: Math.floor(450),\n      }))\n    }\n    console.log(getWindowSize())\n    console.log(this.state.height)\n  }\n\n  public render = (): ReactNode => {\n    // Arguments that are passed to the plugin in Python are accessible\n    // via `this.props.args`\n    const title = this.props.args[\"title\"]\n    const subtitle = this.props.args[\"subtitle\"]\n    const body = this.props.args[\"description\"]\n    const link = this.props.args[\"url\"]\n    const github = this.props.args[\"github\"]\n    const img_link = this.props.args[\"img_path\"]\n    const post = this.props.args[\"post\"]\n    const date = this.props.args[\"date\"]\n    var cardStyle = {\n      minWidth: \"100\",\n      maxWidth: \"100\",\n      transitionDuration: \"0.3s\",\n      height: this.state.height,\n    }\n\n    return (\n      <div style={{ padding: \"0.5rem\" }}>\n        <Card variant=\"outlined\" style={cardStyle}>\n          {title && <CardHeader title={title} subheader={date} />}\n          {img_link && (\n            <CardMedia component=\"img\" height=\"200\" src={img_link} />\n          )}\n\n          <CardContent>\n            {subtitle && <CardHeader subheader={subtitle} />}\n            {body && <Typography variant=\"body2\">{body}</Typography>}\n          </CardContent>\n          <CardActions disableSpacing>\n            {github && (\n              <Button\n                size=\"small\"\n                onClick={() => window.open(github, \"_blank\")}\n              >\n                github\n              </Button>\n            )}\n            {link && (\n              <Button size=\"small\" onClick={() => window.open(link, \"_blank\")}>\n                link\n              </Button>\n            )}\n\n            {post && (\n              <Button\n                size=\"small\"\n                onClick={() => {\n                  this.setState(\n                    () => ({ url: post }),\n                    () => Streamlit.setComponentValue(this.state.url)\n                  )\n                  window.open(post, \"_blank\")\n                }}\n              >\n                Open Article\n              </Button>\n            )}\n          </CardActions>\n        </Card>\n      </div>\n    )\n  }\n}\n\n// connection between component and Streamlit\nexport default withStreamlitConnection(CardComponent)\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport Postcard from \"./PostCard\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <Postcard />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js` & `st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map` & `st_blogpost_component-0.1.0/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.9/st_blogpost_component.egg-info/SOURCES.txt` & `st_blogpost_component-0.1.0/st_blogpost_component.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 st_blogpost_component.egg-info/top_level.txt
 st_blogpost_component/frontend/build/asset-manifest.json
 st_blogpost_component/frontend/build/bootstrap.min.css
 st_blogpost_component/frontend/build/index.html
 st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js
 st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js.LICENSE.txt
 st_blogpost_component/frontend/build/static/js/2.115577ef.chunk.js.map
-st_blogpost_component/frontend/build/static/js/main.bbd810e7.chunk.js
-st_blogpost_component/frontend/build/static/js/main.bbd810e7.chunk.js.map
+st_blogpost_component/frontend/build/static/js/main.ecb92db9.chunk.js
+st_blogpost_component/frontend/build/static/js/main.ecb92db9.chunk.js.map
 st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
 st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
```

