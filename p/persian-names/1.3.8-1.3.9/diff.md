# Comparing `tmp/persian-names-1.3.8.tar.gz` & `tmp/persian-names-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persian-names-1.3.8.tar", last modified: Sat May 27 20:31:35 2023, max compression
+gzip compressed data, was "persian-names-1.3.9.tar", last modified: Fri Jul  7 15:04:39 2023, max compression
```

## Comparing `persian-names-1.3.8.tar` & `persian-names-1.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-05-27 20:31:35.372847 persian-names-1.3.8/
--rw-r--r--   0 arman      (501) staff       (20)     1068 2022-11-15 18:36:04.000000 persian-names-1.3.8/LICENSE
--rw-r--r--   0 arman      (501) staff       (20)     4006 2023-05-27 20:31:35.372724 persian-names-1.3.8/PKG-INFO
--rw-r--r--   0 arman      (501) staff       (20)     2700 2023-03-06 21:55:33.000000 persian-names-1.3.8/README.md
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-05-27 20:31:35.370750 persian-names-1.3.8/persian_names/
--rw-r--r--   0 arman      (501) staff       (20)       28 2022-11-21 18:59:10.000000 persian-names-1.3.8/persian_names/__init__.py
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-05-27 20:31:35.372429 persian-names-1.3.8/persian_names/data/
--rw-r--r--   0 arman      (501) staff       (20)     2239 2023-04-07 21:05:49.000000 persian-names-1.3.8/persian_names/data/female_en.txt
--rw-r--r--   0 arman      (501) staff       (20)     3380 2023-04-07 21:06:05.000000 persian-names-1.3.8/persian_names/data/female_fa.txt
--rw-r--r--   0 arman      (501) staff       (20)     2089 2023-05-27 20:27:16.000000 persian-names-1.3.8/persian_names/data/male_en.txt
--rw-r--r--   0 arman      (501) staff       (20)     3133 2023-05-27 20:27:47.000000 persian-names-1.3.8/persian_names/data/male_fa.txt
--rw-r--r--   0 arman      (501) staff       (20)        0 2023-03-06 21:07:00.000000 persian-names-1.3.8/persian_names/p.py
--rw-r--r--   0 arman      (501) staff       (20)     7834 2023-05-27 20:28:55.000000 persian-names-1.3.8/persian_names/persian_names.py
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-05-27 20:31:35.371350 persian-names-1.3.8/persian_names.egg-info/
--rw-r--r--   0 arman      (501) staff       (20)     4006 2023-05-27 20:31:35.000000 persian-names-1.3.8/persian_names.egg-info/PKG-INFO
--rw-r--r--   0 arman      (501) staff       (20)      378 2023-05-27 20:31:35.000000 persian-names-1.3.8/persian_names.egg-info/SOURCES.txt
--rw-r--r--   0 arman      (501) staff       (20)        1 2023-05-27 20:31:35.000000 persian-names-1.3.8/persian_names.egg-info/dependency_links.txt
--rw-r--r--   0 arman      (501) staff       (20)       14 2023-05-27 20:31:35.000000 persian-names-1.3.8/persian_names.egg-info/top_level.txt
--rw-r--r--   0 arman      (501) staff       (20)       38 2023-05-27 20:31:35.372960 persian-names-1.3.8/setup.cfg
--rw-r--r--   0 arman      (501) staff       (20)     1722 2023-05-27 20:30:06.000000 persian-names-1.3.8/setup.py
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-07-07 15:04:39.902627 persian-names-1.3.9/
+-rw-r--r--   0 arman      (501) staff       (20)     1068 2022-11-15 18:36:04.000000 persian-names-1.3.9/LICENSE
+-rw-r--r--   0 arman      (501) staff       (20)     4006 2023-07-07 15:04:39.902495 persian-names-1.3.9/PKG-INFO
+-rw-r--r--   0 arman      (501) staff       (20)     2700 2023-07-07 15:00:41.000000 persian-names-1.3.9/README.md
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-07-07 15:04:39.900170 persian-names-1.3.9/persian_names/
+-rw-r--r--   0 arman      (501) staff       (20)       28 2022-11-21 18:59:10.000000 persian-names-1.3.9/persian_names/__init__.py
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-07-07 15:04:39.902199 persian-names-1.3.9/persian_names/data/
+-rw-r--r--   0 arman      (501) staff       (20)     2239 2023-04-07 21:05:49.000000 persian-names-1.3.9/persian_names/data/female_en.txt
+-rw-r--r--   0 arman      (501) staff       (20)     3380 2023-04-07 21:06:05.000000 persian-names-1.3.9/persian_names/data/female_fa.txt
+-rw-r--r--   0 arman      (501) staff       (20)     2129 2023-07-07 14:55:54.000000 persian-names-1.3.9/persian_names/data/male_en.txt
+-rw-r--r--   0 arman      (501) staff       (20)     3188 2023-07-07 14:56:11.000000 persian-names-1.3.9/persian_names/data/male_fa.txt
+-rw-r--r--   0 arman      (501) staff       (20)        0 2023-03-06 21:07:00.000000 persian-names-1.3.9/persian_names/p.py
+-rw-r--r--   0 arman      (501) staff       (20)     7882 2023-07-07 15:03:18.000000 persian-names-1.3.9/persian_names/persian_names.py
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-07-07 15:04:39.900787 persian-names-1.3.9/persian_names.egg-info/
+-rw-r--r--   0 arman      (501) staff       (20)     4006 2023-07-07 15:04:39.000000 persian-names-1.3.9/persian_names.egg-info/PKG-INFO
+-rw-r--r--   0 arman      (501) staff       (20)      378 2023-07-07 15:04:39.000000 persian-names-1.3.9/persian_names.egg-info/SOURCES.txt
+-rw-r--r--   0 arman      (501) staff       (20)        1 2023-07-07 15:04:39.000000 persian-names-1.3.9/persian_names.egg-info/dependency_links.txt
+-rw-r--r--   0 arman      (501) staff       (20)       14 2023-07-07 15:04:39.000000 persian-names-1.3.9/persian_names.egg-info/top_level.txt
+-rw-r--r--   0 arman      (501) staff       (20)       38 2023-07-07 15:04:39.902745 persian-names-1.3.9/setup.cfg
+-rw-r--r--   0 arman      (501) staff       (20)     1722 2023-07-07 14:57:16.000000 persian-names-1.3.9/setup.py
```

### Comparing `persian-names-1.3.8/LICENSE` & `persian-names-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `persian-names-1.3.8/PKG-INFO` & `persian-names-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-names
-Version: 1.3.8
+Version: 1.3.9
 Summary: A Python library for generating random Persian (Farsi) names.
 Home-page: https://github.com/armanyazdi/persian-names
 Author: Arman Yazdi
 License: MIT
 Project-URL: Source, https://github.com/armanyazdi/persian-names
 Project-URL: Documentation, https://pypi.org/project/persian-names
 Keywords: persian names,farsi names,iranian names,name generator
```

### Comparing `persian-names-1.3.8/README.md` & `persian-names-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `persian-names-1.3.8/persian_names/data/female_en.txt` & `persian-names-1.3.9/persian_names/data/female_en.txt`

 * *Files identical despite different names*

### Comparing `persian-names-1.3.8/persian_names/data/female_fa.txt` & `persian-names-1.3.9/persian_names/data/female_fa.txt`

 * *Files identical despite different names*

### Comparing `persian-names-1.3.8/persian_names/data/male_en.txt` & `persian-names-1.3.9/persian_names/data/male_en.txt`

 * *Files 13% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 Samyar
 Shantia
 Shervin
 Abdolreza
 Abed
 Abolfazl
 Adel
+Adib
 Afshar
 Afshin
 Ahmadreza
 Alborz
 Ali
 Aliakbar
 Aliasghar
@@ -180,14 +181,15 @@
 Khashayar
 Kian
 Kiarash
 Kourosh
 Kousha
 Mahan
 Mahdi
+Mahmoudreza
 Majid
 Manouchehr
 Masoud
 Matin
 Mazaher
 Mazdak
 Maziar
@@ -208,14 +210,15 @@
 Mohammadamin
 Mohammadhassan
 Mohammadhossein
 Mohammadjavad
 Mohammadmahdi
 Mohammadreza
 Mohammadsadegh
+Moharram
 Mohsen
 Mojtaba
 Mokhtar
 Morad
 Morteza
 Moshfegh
 Moslem
@@ -238,16 +241,18 @@
 Pouria
 Pouya
 Rahmat
 Rambod
 Ramin
 Ramtin
 Rashid
+Rasoul
 Rostam
 Rouzbeh
+Saadat
 Saber
 Sadegh
 Sajjad
 Salar
 Salman
 Saman
 Sasan
```

### Comparing `persian-names-1.3.8/persian_names/data/male_fa.txt` & `persian-names-1.3.9/persian_names/data/male_fa.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 مهیار
 آرام
 آزاد
 ابوالفضل
 اتابک
 احسان
 احمدرضا
+ادیب
 اردشیر
 اردلان
 ارسلان
 اروند
 ارژنگ
 اسدالله
 اصغر
@@ -124,23 +125,25 @@
 دانیال
 ذاکر
 رامبد
 رامتین
 رامین
 رحمت
 رستم
+رسول
 رشید
 روزبه
 زبیر
 ساسان
 سالار
 سامان
 سبحان
 سجاد
 سروش
+سعادت
 سلمان
 سهراب
 سهیل
 سپهر
 سیامک
 سیاوش
 سینا
@@ -199,23 +202,25 @@
 قلی
 مازیار
 ماهان
 مبین
 متین
 مجتبی
 مجید
+محرم
 محسن
 محمدامین
 محمدجواد
 محمدحسن
 محمدحسین
 محمدرضا
 محمدصادق
 محمدعلی
 محمدمهدی
+محمودرضا
 مختار
 مراد
 مرتضی
 مزدک
 مسعود
 مسلم
 مشفق
```

### Comparing `persian-names-1.3.8/persian_names/persian_names.py` & `persian-names-1.3.9/persian_names/persian_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,29 +71,30 @@
         'nejad', '',
         'bayat', '',
         'yekta' '',
         'sabet' '',
         'azad', '',
         'zare', '',
         'moghaddam', '',
-        'roshan', '',
+        'tabar', '',
     ]
     more_suffixes = [
         'pour', 'i',
         'zadeh', 'i',
         'far', 'i',
         'fard', 'i',
         'khani', 'i',
         'vand', 'i',
         'lou', 'i',
         'nia', 'i',
         'zehi', 'i',
         'nejad', 'i',
         'beigi', 'i',
         'zare', 'i',
+        'tabar', 'i',
     ]
     arabic_names = []
     illegal_names = []
 
     f = open(path + '/data/' + files[0], 'r', encoding='utf8')
     names = f.read().split('\n')
     f.close()
@@ -217,29 +218,30 @@
         ' نژاد', '',
         ' بیات', '',
         ' یکتا', '',
         ' ثابت', '',
         ' آزاد', '',
         ' زارع', '',
         ' مقدم', '',
-        ' روشن', '',
+        ' تبار', '',
     ]
     more_suffixes = [
         ' پور', 'ی',
         ' زاده', 'ی',
         ' فر', 'ی',
         ' فرد', 'ی',
         ' خانی', 'ی',
         ' وند', 'ی',
         ' لو', 'ی',
         ' نیا', 'ی',
         ' زهی', 'ی',
         ' نژاد', 'ی',
         ' بیگی', 'ی',
         ' زارع', 'ی',
+        ' تبار', 'ی',
     ]
     arabic_names = []
     illegal_names = []
 
     f = open(path + '/data/' + files[2], 'r', encoding='utf8')
     names = f.read().split('\n')
     f.close()
```

### Comparing `persian-names-1.3.8/persian_names.egg-info/PKG-INFO` & `persian-names-1.3.9/persian_names.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-names
-Version: 1.3.8
+Version: 1.3.9
 Summary: A Python library for generating random Persian (Farsi) names.
 Home-page: https://github.com/armanyazdi/persian-names
 Author: Arman Yazdi
 License: MIT
 Project-URL: Source, https://github.com/armanyazdi/persian-names
 Project-URL: Documentation, https://pypi.org/project/persian-names
 Keywords: persian names,farsi names,iranian names,name generator
```

### Comparing `persian-names-1.3.8/setup.py` & `persian-names-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('./README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='persian-names',
-    version='1.3.8',
+    version='1.3.9',
     packages=['persian_names'],
     include_package_data=True,
     data_files=[('', [
         'persian_names/data/female_en.txt',
         'persian_names/data/female_fa.txt',
         'persian_names/data/male_en.txt',
         'persian_names/data/male_fa.txt'
```

