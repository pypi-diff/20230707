# Comparing `tmp/django-lazy-srcset-0.2.1.tar.gz` & `tmp/django-lazy-srcset-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lazy-srcset-0.2.1.tar", last modified: Fri Jun 30 12:30:30 2023, max compression
+gzip compressed data, was "django-lazy-srcset-0.2.2.tar", last modified: Thu Jul  6 22:44:29 2023, max compression
```

## Comparing `django-lazy-srcset-0.2.1.tar` & `django-lazy-srcset-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.835195 django-lazy-srcset-0.2.1/
--rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-0.2.1/LICENSE
--rw-r--r--   0 quantra    (501) staff       (20)       73 2023-06-29 00:05:50.000000 django-lazy-srcset-0.2.1/MANIFEST.in
--rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-06-30 12:30:30.835304 django-lazy-srcset-0.2.1/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     5492 2023-06-27 20:50:37.000000 django-lazy-srcset-0.2.1/README.rst
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.830690 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/
--rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-06-30 12:30:30.000000 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)      576 2023-06-30 12:30:30.000000 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/SOURCES.txt
--rw-r--r--   0 quantra    (501) staff       (20)       40 2023-06-30 12:30:30.000000 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/dependency_links.txt
--rw-r--r--   0 quantra    (501) staff       (20)       35 2023-06-30 12:30:30.000000 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/requires.txt
--rw-r--r--   0 quantra    (501) staff       (20)       20 2023-06-30 12:30:30.000000 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/top_level.txt
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.832149 django-lazy-srcset-0.2.1/lazy_srcset/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.1/lazy_srcset/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-0.2.1/lazy_srcset/apps.py
--rw-r--r--   0 quantra    (501) staff       (20)     1237 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.1/lazy_srcset/conf.py
--rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.1/lazy_srcset/imagegenerators.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.832940 django-lazy-srcset-0.2.1/lazy_srcset/management/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:58.000000 django-lazy-srcset-0.2.1/lazy_srcset/management/__init__.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.833974 django-lazy-srcset-0.2.1/lazy_srcset/management/commands/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:50.000000 django-lazy-srcset-0.2.1/lazy_srcset/management/commands/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)     3299 2023-06-29 00:03:00.000000 django-lazy-srcset-0.2.1/lazy_srcset/management/commands/imagekit_cleanup.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.834933 django-lazy-srcset-0.2.1/lazy_srcset/templatetags/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.1/lazy_srcset/templatetags/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)     8879 2023-06-27 16:04:10.000000 django-lazy-srcset-0.2.1/lazy_srcset/templatetags/lazy_srcset.py
--rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-0.2.1/pyproject.toml
--rw-r--r--   0 quantra    (501) staff       (20)     1917 2023-06-30 12:30:30.839863 django-lazy-srcset-0.2.1/setup.cfg
--rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-0.2.1/setup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.530314 django-lazy-srcset-0.2.2/
+-rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-0.2.2/LICENSE
+-rw-r--r--   0 quantra    (501) staff       (20)       73 2023-06-29 00:05:50.000000 django-lazy-srcset-0.2.2/MANIFEST.in
+-rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-07-06 22:44:29.530437 django-lazy-srcset-0.2.2/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     5492 2023-06-27 20:50:37.000000 django-lazy-srcset-0.2.2/README.rst
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.524296 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/
+-rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-07-06 22:44:29.000000 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)      576 2023-07-06 22:44:29.000000 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/SOURCES.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       40 2023-07-06 22:44:29.000000 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/dependency_links.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       35 2023-07-06 22:44:29.000000 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/requires.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       20 2023-07-06 22:44:29.000000 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/top_level.txt
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.526626 django-lazy-srcset-0.2.2/lazy_srcset/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.2/lazy_srcset/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-0.2.2/lazy_srcset/apps.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1237 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.2/lazy_srcset/conf.py
+-rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.2/lazy_srcset/imagegenerators.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.527402 django-lazy-srcset-0.2.2/lazy_srcset/management/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:58.000000 django-lazy-srcset-0.2.2/lazy_srcset/management/__init__.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.528478 django-lazy-srcset-0.2.2/lazy_srcset/management/commands/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:50.000000 django-lazy-srcset-0.2.2/lazy_srcset/management/commands/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)     3299 2023-06-29 00:03:00.000000 django-lazy-srcset-0.2.2/lazy_srcset/management/commands/imagekit_cleanup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.530098 django-lazy-srcset-0.2.2/lazy_srcset/templatetags/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.2/lazy_srcset/templatetags/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)     8925 2023-07-06 19:45:37.000000 django-lazy-srcset-0.2.2/lazy_srcset/templatetags/lazy_srcset.py
+-rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-0.2.2/pyproject.toml
+-rw-r--r--   0 quantra    (501) staff       (20)     1917 2023-07-06 22:44:29.537313 django-lazy-srcset-0.2.2/setup.cfg
+-rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-0.2.2/setup.py
```

### Comparing `django-lazy-srcset-0.2.1/LICENSE` & `django-lazy-srcset-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.1/PKG-INFO` & `django-lazy-srcset-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lazy-srcset
-Version: 0.2.1
+Version: 0.2.2
 Summary: Lazy srcset and image generation for Django. Minimum effort required. No database required.
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Source, https://github.com/Quantra/django-lazy-srcset
 Keywords: django,django-lazy-srcset,django lazy srcset,django srcset,django responsive images,django responsive
 Classifier: Environment :: Web Environment
```

### Comparing `django-lazy-srcset-0.2.1/README.rst` & `django-lazy-srcset-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/PKG-INFO` & `django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lazy-srcset
-Version: 0.2.1
+Version: 0.2.2
 Summary: Lazy srcset and image generation for Django. Minimum effort required. No database required.
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Source, https://github.com/Quantra/django-lazy-srcset
 Keywords: django,django-lazy-srcset,django lazy srcset,django srcset,django responsive images,django responsive
 Classifier: Environment :: Web Environment
```

### Comparing `django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/SOURCES.txt` & `django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.1/lazy_srcset/conf.py` & `django-lazy-srcset-0.2.2/lazy_srcset/conf.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.1/lazy_srcset/imagegenerators.py` & `django-lazy-srcset-0.2.2/lazy_srcset/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.1/lazy_srcset/management/commands/imagekit_cleanup.py` & `django-lazy-srcset-0.2.2/lazy_srcset/management/commands/imagekit_cleanup.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.1/lazy_srcset/templatetags/lazy_srcset.py` & `django-lazy-srcset-0.2.2/lazy_srcset/templatetags/lazy_srcset.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,26 +149,26 @@
         image = ImageFile(open(finders.find(image), "rb"))
         image.url = url
 
     # If the image is an SVG return now with src="whatever.svg" and width and height if possible. SVG is lazy king!
     if Path(image.name).suffix.lower() == ".svg":
         return svg_srcset(image)
 
-    # Get the conf from the first arg or default
+    # Get the conf from the config kwarg or default
     try:
         conf = settings.LAZY_SRCSET[kwargs.pop("config")]
     except KeyError:
         conf = settings.LAZY_SRCSET["default"]
 
     # Get the max_width from kwargs or conf.
     max_width = get_from_kwargs_or_conf("max_width", kwargs, conf)
 
     # Set the maximum width image in our srcset.
     if max_width is None or max_width > image.width:
-        # Clamp max_width to image.width or use image.width if max_width is None.
+        # Limit max_width to image.width or use image.width if max_width is None.
         max_width = image.width
 
     # Get the format and quality from kwargs or conf and wrap up together with source in generator_kwargs.
     # These will be used for every image generation.
     generator_kwargs = {
         "source": image,
         "output_format": conf.get("format"),
@@ -184,16 +184,16 @@
     # Generate the max_width image via imagekit.
     generator = generator_registry.get(
         generator_id, width=max_width, **generator_kwargs
     )
     generator_image = ImageCacheFile(generator)
 
     # Set the max_width image as our src and include it in the srcset.
-    src = generator_image.url
-    srcset = [FORMAT_STRINGS["srcset_entry"] % (generator_image.url, max_width)]
+    src_value = generator_image.url
+    srcset_values = [FORMAT_STRINGS["srcset_entry"] % (generator_image.url, max_width)]
 
     # Set the width and height from the max_width image.
     width, height = generator_image.width, generator_image.height
 
     # If we have kwargs we can set the sizes otherwise try and get them from args.
     sizes_dict = (
         {int(k): int(v) for k, v in kwargs.items()}
@@ -218,22 +218,22 @@
         # Generate the image via imagekit.
         generator = generator_registry.get(
             generator_id, width=target_width, **generator_kwargs
         )
         generator_image = ImageCacheFile(generator)
 
         # Add an entry for this image to the srcset.
-        srcset.append(
+        srcset_values.append(
             FORMAT_STRINGS["srcset_entry"] % (generator_image.url, target_width)
         )
 
     # Create the attrs list for imminent stringification.
     attrs = [
-        FORMAT_STRINGS["src"] % src,
-        FORMAT_STRINGS["srcset"] % ", ".join(srcset),
-        FORMAT_STRINGS["sizes"] % ", ".join(sizes),
+        FORMAT_STRINGS["src"] % src_value,
+        FORMAT_STRINGS["srcset"] % ", ".join(srcset_values),
+        FORMAT_STRINGS["sizes"] % ", ".join(reversed(sizes)),
         FORMAT_STRINGS["width"] % width,
         FORMAT_STRINGS["height"] % height,
     ]
 
     # Stringify!
     return mark_safe(" ".join(attrs))
```

### Comparing `django-lazy-srcset-0.2.1/setup.cfg` & `django-lazy-srcset-0.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-lazy-srcset
-version = 0.2.1
+version = 0.2.2
 description = Lazy srcset and image generation for Django. Minimum effort required. No database required.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers =
```

