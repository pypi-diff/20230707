# Comparing `tmp/django_google_fonts-0.0.1.tar.gz` & `tmp/django_google_fonts-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_fonts-0.0.1.tar", last modified: Wed Jun 21 04:45:32 2023, max compression
+gzip compressed data, was "django_google_fonts-0.0.3.tar", last modified: Fri Jul  7 18:46:29 2023, max compression
```

## Comparing `django_google_fonts-0.0.1.tar` & `django_google_fonts-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:45:32.416842 django_google_fonts-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-21 04:45:20.000000 django_google_fonts-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-21 04:45:32.416842 django_google_fonts-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-21 04:45:20.000000 django_google_fonts-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:45:32.416842 django_google_fonts-0.0.1/django_google_fonts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 04:45:20.000000 django_google_fonts-0.0.1/django_google_fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-21 04:45:20.000000 django_google_fonts-0.0.1/django_google_fonts/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:45:32.416842 django_google_fonts-0.0.1/django_google_fonts/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 04:45:20.000000 django_google_fonts-0.0.1/django_google_fonts/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-21 04:45:20.000000 django_google_fonts-0.0.1/django_google_fonts/templatetags/google_fonts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-21 04:45:20.000000 django_google_fonts-0.0.1/django_google_fonts/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:45:32.416842 django_google_fonts-0.0.1/django_google_fonts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-21 04:45:32.000000 django_google_fonts-0.0.1/django_google_fonts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-21 04:45:32.000000 django_google_fonts-0.0.1/django_google_fonts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 04:45:32.000000 django_google_fonts-0.0.1/django_google_fonts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 04:45:32.000000 django_google_fonts-0.0.1/django_google_fonts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 04:45:32.000000 django_google_fonts-0.0.1/django_google_fonts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 04:45:20.000000 django_google_fonts-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 04:45:32.416842 django_google_fonts-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:46:29.635193 django_google_fonts-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-07 18:46:15.000000 django_google_fonts-0.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-07 18:46:29.631193 django_google_fonts-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-07 18:46:15.000000 django_google_fonts-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:46:29.631193 django_google_fonts-0.0.3/django_google_fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:46:15.000000 django_google_fonts-0.0.3/django_google_fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-07 18:46:15.000000 django_google_fonts-0.0.3/django_google_fonts/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:46:29.631193 django_google_fonts-0.0.3/django_google_fonts/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:46:15.000000 django_google_fonts-0.0.3/django_google_fonts/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-07 18:46:15.000000 django_google_fonts-0.0.3/django_google_fonts/templatetags/google_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-07 18:46:15.000000 django_google_fonts-0.0.3/django_google_fonts/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:46:29.631193 django_google_fonts-0.0.3/django_google_fonts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-07 18:46:29.000000 django_google_fonts-0.0.3/django_google_fonts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-07 18:46:29.000000 django_google_fonts-0.0.3/django_google_fonts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:46:29.000000 django_google_fonts-0.0.3/django_google_fonts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 18:46:29.000000 django_google_fonts-0.0.3/django_google_fonts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 18:46:29.000000 django_google_fonts-0.0.3/django_google_fonts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-07 18:46:15.000000 django_google_fonts-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:46:29.635193 django_google_fonts-0.0.3/setup.cfg
```

### Comparing `django_google_fonts-0.0.1/LICENSE.md` & `django_google_fonts-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_google_fonts-0.0.1/PKG-INFO` & `django_google_fonts-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,9 @@
-Metadata-Version: 2.1
-Name: django_google_fonts
-Version: 0.0.1
-Summary: Easy to install and offline Google fonts in Django projects
-Author-email: Andy McKay <andy@mckay.pub>
-Project-URL: Homepage, https://github.com/andymckay/django-google-fonts
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 `django-google-fonts` lets you use Google fonts in Django easily, by downloading, rewriting and caching the font and CSS files locally. 
-
+README.md
 This means that you can have all the benefits of using Google Fonts, but with added privacy, security and speed for your users, because all the requests for the fonts will be on your domain and not hitting Google servers.
 
 When the server restarts it will check if any fonts are missing locally and load them if they are. So there is no impact or performance considerations. After that initial download of the fonts, `django-google-fonts` does not need to make any more requests to Google servers, working totally offline from the Google servers.
 
 ### Installing
 
 ```bash
@@ -24,27 +11,27 @@
 ```
 
 Then add to your Django settings file:
 
 ```python
 INSTALLED_APPS = [
     ...
-    `django_google_fonts`
+    'django_google_fonts'
 ]
 ```
 
 ### Using
 
 Tell Django which fonts you'd like:
 
 ```python
 GOOGLE_FONTS = ["Kablammo", "Roboto"]
 ```
 
-When Django starts it will grab the fonts from Google and store them in the `GOOGLE_FONTS_DEST`. It will rewrite the CSS that Google Fonts provides, so all you have to do is load the font like normal. For example:
+When Django starts it will grab the fonts from Google and store them in your `STATICFILES_DIRS` directory. It will rewrite the CSS that Google Fonts provides, so all you have to do is load the font like normal. For example:
 
 ```html
 <link rel="stylesheet" href="{% static 'fonts/pathwayextreme.css' %}">
 <style>
     body {
         font-family: 'Pathway Extreme';
     }
@@ -54,27 +41,49 @@
 There is also a `font` tag that will return the raw CSS:
 
 ```html
     {% load google_fonts %}
     {% font_css "Pathway Extreme" %}
 ```
 
+Custom font weights are available by specifying the font weights in the URL. The easy way to do this is visit a font page, for example [Robot](https://fonts.google.com/specimen/Roboto) and then selecting the weights and styles you'd like. Then click on `Selected Families` and copy the font definition in.
+
+For example Google will suggest embedding the font using this URL:
+
+```html
+<link rel="preconnect" href="https://fonts.googleapis.com">
+<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
+<link href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,700;0,900;1,700&display=swap" rel="stylesheet">
+```
+
+Roboto with italic in weights 100, 700, 900. To use this in Django you would specify:
+
+```python
+GOOGLE_FONTS = ["Roboto:ital,wght@0,100;0,700;1,700"]
+```
+
+And you would reference it in a stylesheet:
+
+```html
+<link rel="stylesheet" href="{% static 'fonts/roboto:ital,wght@0,100;0,700;1,700.css' %}">
+```
+
 #### Optional settings
 
 By default `django-google-fonts` will store fonts in the first directory specified in `STATICFILES_DIRS`. That might not be where you want, so you can set a `GOOGLE_FONTS_DIR` setting if you'd like it be somewhere else:
 
 ```python
-GOOGLE_FONT_DIR = BASE_DIR / "fonts"
+GOOGLE_FONTS_DIR = BASE_DIR / "fonts"
 STATICFILES_DIRS = [BASE_DIR / "static", BASE_DIR / "fonts"]
 ```
 
 The CSS file contains the path to the font and `django-google-fonts` tries to calculate what the path to the font should be by using the value of `STATIC_URL`. If that's wrong and you need it be something else, you can set that value:
 
 ```python
-GOOGLE_FONT_URL = "my-exotic-static/url/to-the-fonts"
+GOOGLE_FONTS_URL = "my-exotic-static/url/to-the-fonts"
 ```
 
 ### Names
 
 Google fonts normally have title cased names, with capitalized first names [^1]. For example `Pathway Extreme`. Google normalises this too: `pathwayextreme` and this is used in file names. So in the case of `Pathway Extreme`
 
 |Where|Name|
```

#### html2text {}

```diff
@@ -1,43 +1,48 @@
-Metadata-Version: 2.1 Name: django_google_fonts Version: 0.0.1 Summary: Easy to
-install and offline Google fonts in Django projects Author-email: Andy McKay
-mckay.pub> Project-URL: Homepage, https://github.com/andymckay/django-google-
-fonts Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE.md `django-google-fonts` lets you use Google fonts in Django easily, by
-downloading, rewriting and caching the font and CSS files locally. This means
-that you can have all the benefits of using Google Fonts, but with added
-privacy, security and speed for your users, because all the requests for the
-fonts will be on your domain and not hitting Google servers. When the server
-restarts it will check if any fonts are missing locally and load them if they
-are. So there is no impact or performance considerations. After that initial
-download of the fonts, `django-google-fonts` does not need to make any more
-requests to Google servers, working totally offline from the Google servers.
-### Installing ```bash pip install django-google-fonts ``` Then add to your
-Django settings file: ```python INSTALLED_APPS = [ ... `django_google_fonts` ]
-``` ### Using Tell Django which fonts you'd like: ```python GOOGLE_FONTS =
-["Kablammo", "Roboto"] ``` When Django starts it will grab the fonts from
-Google and store them in the `GOOGLE_FONTS_DEST`. It will rewrite the CSS that
-Google Fonts provides, so all you have to do is load the font like normal. For
-example: ```html
+`django-google-fonts` lets you use Google fonts in Django easily, by
+downloading, rewriting and caching the font and CSS files locally. README.md
+This means that you can have all the benefits of using Google Fonts, but with
+added privacy, security and speed for your users, because all the requests for
+the fonts will be on your domain and not hitting Google servers. When the
+server restarts it will check if any fonts are missing locally and load them if
+they are. So there is no impact or performance considerations. After that
+initial download of the fonts, `django-google-fonts` does not need to make any
+more requests to Google servers, working totally offline from the Google
+servers. ### Installing ```bash pip install django-google-fonts ``` Then add to
+your Django settings file: ```python INSTALLED_APPS = [ ...
+'django_google_fonts' ] ``` ### Using Tell Django which fonts you'd like:
+```python GOOGLE_FONTS = ["Kablammo", "Roboto"] ``` When Django starts it will
+grab the fonts from Google and store them in your `STATICFILES_DIRS` directory.
+It will rewrite the CSS that Google Fonts provides, so all you have to do is
+load the font like normal. For example: ```html
  ``` There is also a `font` tag that will return the raw CSS: ```html {% load
-google_fonts %} {% font_css "Pathway Extreme" %} ``` #### Optional settings By
-default `django-google-fonts` will store fonts in the first directory specified
-in `STATICFILES_DIRS`. That might not be where you want, so you can set a
-`GOOGLE_FONTS_DIR` setting if you'd like it be somewhere else: ```python
-GOOGLE_FONT_DIR = BASE_DIR / "fonts" STATICFILES_DIRS = [BASE_DIR / "static",
-BASE_DIR / "fonts"] ``` The CSS file contains the path to the font and `django-
-google-fonts` tries to calculate what the path to the font should be by using
-the value of `STATIC_URL`. If that's wrong and you need it be something else,
-you can set that value: ```python GOOGLE_FONT_URL = "my-exotic-static/url/to-
-the-fonts" ``` ### Names Google fonts normally have title cased names, with
-capitalized first names [^1]. For example `Pathway Extreme`. Google normalises
-this too: `pathwayextreme` and this is used in file names. So in the case of
-`Pathway Extreme` |Where|Name| |-|-| |Settings file|`Pathway Extreme`| |Font
-tag|`Pathway Extreme`| |Static tag|`pathwayextreme`| [^1]: Font's like `IBM
-Plex Sans` have more capital letters than just the first letter. If you are
-unsure you can get at the fonts programatically, for example: ```python >>>
-from django.apps import apps >>> for font in apps.get_app_config
-("django_google_fonts").fonts: ... print(font.name, font.slug, font.dest) ...
-Kablammo kablammo /Users/a/c/examplefonts/static/fonts/kablammo Roboto roboto /
-Users/a/c/examplefonts/static/fonts/roboto ```
+google_fonts %} {% font_css "Pathway Extreme" %} ``` Custom font weights are
+available by specifying the font weights in the URL. The easy way to do this is
+visit a font page, for example [Robot](https://fonts.google.com/specimen/
+Roboto) and then selecting the weights and styles you'd like. Then click on
+`Selected Families` and copy the font definition in. For example Google will
+suggest embedding the font using this URL: ```html
+
+
+ ``` Roboto with italic in weights 100, 700, 900. To use this in Django you
+would specify: ```python GOOGLE_FONTS = ["Roboto:ital,wght@0,100;0,700;1,700"]
+``` And you would reference it in a stylesheet: ```html
+ ``` #### Optional settings By default `django-google-fonts` will store fonts
+in the first directory specified in `STATICFILES_DIRS`. That might not be where
+you want, so you can set a `GOOGLE_FONTS_DIR` setting if you'd like it be
+somewhere else: ```python GOOGLE_FONTS_DIR = BASE_DIR / "fonts"
+STATICFILES_DIRS = [BASE_DIR / "static", BASE_DIR / "fonts"] ``` The CSS file
+contains the path to the font and `django-google-fonts` tries to calculate what
+the path to the font should be by using the value of `STATIC_URL`. If that's
+wrong and you need it be something else, you can set that value: ```python
+GOOGLE_FONTS_URL = "my-exotic-static/url/to-the-fonts" ``` ### Names Google
+fonts normally have title cased names, with capitalized first names [^1]. For
+example `Pathway Extreme`. Google normalises this too: `pathwayextreme` and
+this is used in file names. So in the case of `Pathway Extreme` |Where|Name| |-
+|-| |Settings file|`Pathway Extreme`| |Font tag|`Pathway Extreme`| |Static
+tag|`pathwayextreme`| [^1]: Font's like `IBM Plex Sans` have more capital
+letters than just the first letter. If you are unsure you can get at the fonts
+programatically, for example: ```python >>> from django.apps import apps >>>
+for font in apps.get_app_config("django_google_fonts").fonts: ... print
+(font.name, font.slug, font.dest) ... Kablammo kablammo /Users/a/c/
+examplefonts/static/fonts/kablammo Roboto roboto /Users/a/c/examplefonts/
+static/fonts/roboto ```
```

### Comparing `django_google_fonts-0.0.1/django_google_fonts/apps.py` & `django_google_fonts-0.0.3/django_google_fonts/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Google Fonts produces a different CSS based on the user agent, using the Chrome user agent seems to give us a nice CSS compatible with browsers.
 # But in case you can override this by setting the GOOGLE_FONTS_USER_AGENT setting.
 user_agent = getattr(
     settings,
     "GOOGLE_FONTS_USER_AGENT",
     "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
 )
-css_url = "https://fonts.googleapis.com/css"
+css_url = "https://fonts.googleapis.com/css2"
 css_prefix = "https://fonts.gstatic.com/s/"
 log_prefix = "django_google_fonts"
 # Requests timeout in seconds.
 timeout = 10
 fonts = []
```

### Comparing `django_google_fonts-0.0.1/django_google_fonts/templatetags/google_fonts.py` & `django_google_fonts-0.0.3/django_google_fonts/templatetags/google_fonts.py`

 * *Files identical despite different names*

### Comparing `django_google_fonts-0.0.1/django_google_fonts/tests.py` & `django_google_fonts-0.0.3/django_google_fonts/tests.py`

 * *Files identical despite different names*

### Comparing `django_google_fonts-0.0.1/django_google_fonts.egg-info/PKG-INFO` & `django_google_fonts-0.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: django-google-fonts
-Version: 0.0.1
+Name: django_google_fonts
+Version: 0.0.3
 Summary: Easy to install and offline Google fonts in Django projects
 Author-email: Andy McKay <andy@mckay.pub>
 Project-URL: Homepage, https://github.com/andymckay/django-google-fonts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 `django-google-fonts` lets you use Google fonts in Django easily, by downloading, rewriting and caching the font and CSS files locally. 
-
+README.md
 This means that you can have all the benefits of using Google Fonts, but with added privacy, security and speed for your users, because all the requests for the fonts will be on your domain and not hitting Google servers.
 
 When the server restarts it will check if any fonts are missing locally and load them if they are. So there is no impact or performance considerations. After that initial download of the fonts, `django-google-fonts` does not need to make any more requests to Google servers, working totally offline from the Google servers.
 
 ### Installing
 
 ```bash
@@ -24,27 +24,27 @@
 ```
 
 Then add to your Django settings file:
 
 ```python
 INSTALLED_APPS = [
     ...
-    `django_google_fonts`
+    'django_google_fonts'
 ]
 ```
 
 ### Using
 
 Tell Django which fonts you'd like:
 
 ```python
 GOOGLE_FONTS = ["Kablammo", "Roboto"]
 ```
 
-When Django starts it will grab the fonts from Google and store them in the `GOOGLE_FONTS_DEST`. It will rewrite the CSS that Google Fonts provides, so all you have to do is load the font like normal. For example:
+When Django starts it will grab the fonts from Google and store them in your `STATICFILES_DIRS` directory. It will rewrite the CSS that Google Fonts provides, so all you have to do is load the font like normal. For example:
 
 ```html
 <link rel="stylesheet" href="{% static 'fonts/pathwayextreme.css' %}">
 <style>
     body {
         font-family: 'Pathway Extreme';
     }
@@ -54,27 +54,49 @@
 There is also a `font` tag that will return the raw CSS:
 
 ```html
     {% load google_fonts %}
     {% font_css "Pathway Extreme" %}
 ```
 
+Custom font weights are available by specifying the font weights in the URL. The easy way to do this is visit a font page, for example [Robot](https://fonts.google.com/specimen/Roboto) and then selecting the weights and styles you'd like. Then click on `Selected Families` and copy the font definition in.
+
+For example Google will suggest embedding the font using this URL:
+
+```html
+<link rel="preconnect" href="https://fonts.googleapis.com">
+<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
+<link href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,700;0,900;1,700&display=swap" rel="stylesheet">
+```
+
+Roboto with italic in weights 100, 700, 900. To use this in Django you would specify:
+
+```python
+GOOGLE_FONTS = ["Roboto:ital,wght@0,100;0,700;1,700"]
+```
+
+And you would reference it in a stylesheet:
+
+```html
+<link rel="stylesheet" href="{% static 'fonts/roboto:ital,wght@0,100;0,700;1,700.css' %}">
+```
+
 #### Optional settings
 
 By default `django-google-fonts` will store fonts in the first directory specified in `STATICFILES_DIRS`. That might not be where you want, so you can set a `GOOGLE_FONTS_DIR` setting if you'd like it be somewhere else:
 
 ```python
-GOOGLE_FONT_DIR = BASE_DIR / "fonts"
+GOOGLE_FONTS_DIR = BASE_DIR / "fonts"
 STATICFILES_DIRS = [BASE_DIR / "static", BASE_DIR / "fonts"]
 ```
 
 The CSS file contains the path to the font and `django-google-fonts` tries to calculate what the path to the font should be by using the value of `STATIC_URL`. If that's wrong and you need it be something else, you can set that value:
 
 ```python
-GOOGLE_FONT_URL = "my-exotic-static/url/to-the-fonts"
+GOOGLE_FONTS_URL = "my-exotic-static/url/to-the-fonts"
 ```
 
 ### Names
 
 Google fonts normally have title cased names, with capitalized first names [^1]. For example `Pathway Extreme`. Google normalises this too: `pathwayextreme` and this is used in file names. So in the case of `Pathway Extreme`
 
 |Where|Name|
```

#### html2text {}

```diff
@@ -1,43 +1,54 @@
-Metadata-Version: 2.1 Name: django-google-fonts Version: 0.0.1 Summary: Easy to
+Metadata-Version: 2.1 Name: django_google_fonts Version: 0.0.3 Summary: Easy to
 install and offline Google fonts in Django projects Author-email: Andy McKay
 mckay.pub> Project-URL: Homepage, https://github.com/andymckay/django-google-
 fonts Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE.md `django-google-fonts` lets you use Google fonts in Django easily, by
-downloading, rewriting and caching the font and CSS files locally. This means
-that you can have all the benefits of using Google Fonts, but with added
-privacy, security and speed for your users, because all the requests for the
-fonts will be on your domain and not hitting Google servers. When the server
-restarts it will check if any fonts are missing locally and load them if they
-are. So there is no impact or performance considerations. After that initial
-download of the fonts, `django-google-fonts` does not need to make any more
-requests to Google servers, working totally offline from the Google servers.
-### Installing ```bash pip install django-google-fonts ``` Then add to your
-Django settings file: ```python INSTALLED_APPS = [ ... `django_google_fonts` ]
-``` ### Using Tell Django which fonts you'd like: ```python GOOGLE_FONTS =
-["Kablammo", "Roboto"] ``` When Django starts it will grab the fonts from
-Google and store them in the `GOOGLE_FONTS_DEST`. It will rewrite the CSS that
-Google Fonts provides, so all you have to do is load the font like normal. For
-example: ```html
+downloading, rewriting and caching the font and CSS files locally. README.md
+This means that you can have all the benefits of using Google Fonts, but with
+added privacy, security and speed for your users, because all the requests for
+the fonts will be on your domain and not hitting Google servers. When the
+server restarts it will check if any fonts are missing locally and load them if
+they are. So there is no impact or performance considerations. After that
+initial download of the fonts, `django-google-fonts` does not need to make any
+more requests to Google servers, working totally offline from the Google
+servers. ### Installing ```bash pip install django-google-fonts ``` Then add to
+your Django settings file: ```python INSTALLED_APPS = [ ...
+'django_google_fonts' ] ``` ### Using Tell Django which fonts you'd like:
+```python GOOGLE_FONTS = ["Kablammo", "Roboto"] ``` When Django starts it will
+grab the fonts from Google and store them in your `STATICFILES_DIRS` directory.
+It will rewrite the CSS that Google Fonts provides, so all you have to do is
+load the font like normal. For example: ```html
  ``` There is also a `font` tag that will return the raw CSS: ```html {% load
-google_fonts %} {% font_css "Pathway Extreme" %} ``` #### Optional settings By
-default `django-google-fonts` will store fonts in the first directory specified
-in `STATICFILES_DIRS`. That might not be where you want, so you can set a
-`GOOGLE_FONTS_DIR` setting if you'd like it be somewhere else: ```python
-GOOGLE_FONT_DIR = BASE_DIR / "fonts" STATICFILES_DIRS = [BASE_DIR / "static",
-BASE_DIR / "fonts"] ``` The CSS file contains the path to the font and `django-
-google-fonts` tries to calculate what the path to the font should be by using
-the value of `STATIC_URL`. If that's wrong and you need it be something else,
-you can set that value: ```python GOOGLE_FONT_URL = "my-exotic-static/url/to-
-the-fonts" ``` ### Names Google fonts normally have title cased names, with
-capitalized first names [^1]. For example `Pathway Extreme`. Google normalises
-this too: `pathwayextreme` and this is used in file names. So in the case of
-`Pathway Extreme` |Where|Name| |-|-| |Settings file|`Pathway Extreme`| |Font
-tag|`Pathway Extreme`| |Static tag|`pathwayextreme`| [^1]: Font's like `IBM
-Plex Sans` have more capital letters than just the first letter. If you are
-unsure you can get at the fonts programatically, for example: ```python >>>
-from django.apps import apps >>> for font in apps.get_app_config
-("django_google_fonts").fonts: ... print(font.name, font.slug, font.dest) ...
-Kablammo kablammo /Users/a/c/examplefonts/static/fonts/kablammo Roboto roboto /
-Users/a/c/examplefonts/static/fonts/roboto ```
+google_fonts %} {% font_css "Pathway Extreme" %} ``` Custom font weights are
+available by specifying the font weights in the URL. The easy way to do this is
+visit a font page, for example [Robot](https://fonts.google.com/specimen/
+Roboto) and then selecting the weights and styles you'd like. Then click on
+`Selected Families` and copy the font definition in. For example Google will
+suggest embedding the font using this URL: ```html
+
+
+ ``` Roboto with italic in weights 100, 700, 900. To use this in Django you
+would specify: ```python GOOGLE_FONTS = ["Roboto:ital,wght@0,100;0,700;1,700"]
+``` And you would reference it in a stylesheet: ```html
+ ``` #### Optional settings By default `django-google-fonts` will store fonts
+in the first directory specified in `STATICFILES_DIRS`. That might not be where
+you want, so you can set a `GOOGLE_FONTS_DIR` setting if you'd like it be
+somewhere else: ```python GOOGLE_FONTS_DIR = BASE_DIR / "fonts"
+STATICFILES_DIRS = [BASE_DIR / "static", BASE_DIR / "fonts"] ``` The CSS file
+contains the path to the font and `django-google-fonts` tries to calculate what
+the path to the font should be by using the value of `STATIC_URL`. If that's
+wrong and you need it be something else, you can set that value: ```python
+GOOGLE_FONTS_URL = "my-exotic-static/url/to-the-fonts" ``` ### Names Google
+fonts normally have title cased names, with capitalized first names [^1]. For
+example `Pathway Extreme`. Google normalises this too: `pathwayextreme` and
+this is used in file names. So in the case of `Pathway Extreme` |Where|Name| |-
+|-| |Settings file|`Pathway Extreme`| |Font tag|`Pathway Extreme`| |Static
+tag|`pathwayextreme`| [^1]: Font's like `IBM Plex Sans` have more capital
+letters than just the first letter. If you are unsure you can get at the fonts
+programatically, for example: ```python >>> from django.apps import apps >>>
+for font in apps.get_app_config("django_google_fonts").fonts: ... print
+(font.name, font.slug, font.dest) ... Kablammo kablammo /Users/a/c/
+examplefonts/static/fonts/kablammo Roboto roboto /Users/a/c/examplefonts/
+static/fonts/roboto ```
```

### Comparing `django_google_fonts-0.0.1/pyproject.toml` & `django_google_fonts-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 profile = "black"
 
 [tool.black]
 line-length = 100
 
 [project]
 name = "django_google_fonts"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
   { name="Andy McKay", email="andy@mckay.pub" },
 ]
 dependencies = [
     'requests >= 2.31.0',
     'tinycss2 >= 1.2.1',
 ]
```

