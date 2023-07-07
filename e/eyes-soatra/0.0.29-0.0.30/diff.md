# Comparing `tmp/eyes_soatra-0.0.29.tar.gz` & `tmp/eyes_soatra-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.29.tar", last modified: Fri Jun  9 08:20:35 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.30.tar", last modified: Fri Jul  7 03:15:14 2023, max compression
```

## Comparing `eyes_soatra-0.0.29.tar` & `eyes_soatra-0.0.30.tar`

### file list

```diff
@@ -1,55 +1,65 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.596090 eyes_soatra-0.0.29/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.29/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      835 2023-06-09 08:20:35.595957 eyes_soatra-0.0.29/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      330 2023-06-02 06:41:30.000000 eyes_soatra-0.0.29/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.590731 eyes_soatra-0.0.29/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.29/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.591702 eyes_soatra-0.0.29/eyes_soatra/constant/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.29/eyes_soatra/constant/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.591835 eyes_soatra-0.0.29/eyes_soatra/constant/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.592318 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/end.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.592775 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/end.py
--rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/period.py
--rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/start.py
--rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/period.py
--rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/start.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.593136 eyes_soatra-0.0.29/eyes_soatra/constant/depends/view/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/view/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/view/no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.29/eyes_soatra/constant/depends/view/not_found.py
--rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.29/eyes_soatra/constant/labels.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.593350 eyes_soatra-0.0.29/eyes_soatra/constant/libs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.29/eyes_soatra/constant/libs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      387 2023-06-09 08:18:33.000000 eyes_soatra-0.0.29/eyes_soatra/constant/libs/requests.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.593569 eyes_soatra-0.0.29/eyes_soatra/constant/user/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.29/eyes_soatra/constant/user/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.29/eyes_soatra/constant/user/user_agents.py
--rw-r--r--   0 soatra     (501) staff       (20)      844 2023-06-07 03:44:07.000000 eyes_soatra-0.0.29/eyes_soatra/constant/vars.py
--rw-r--r--   0 soatra     (501) staff       (20)      107 2023-05-23 06:52:23.000000 eyes_soatra-0.0.29/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.594724 eyes_soatra-0.0.29/eyes_soatra/funcs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)    20149 2023-06-07 04:28:32.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/time_app.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.595255 eyes_soatra-0.0.29/eyes_soatra/funcs/utils/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/utils/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/utils/dict.py
--rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/utils/list.py
--rw-r--r--   0 soatra     (501) staff       (20)     2538 2023-06-02 06:33:58.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/utils/string.py
--rw-r--r--   0 soatra     (501) staff       (20)    14065 2023-06-07 04:33:46.000000 eyes_soatra-0.0.29/eyes_soatra/funcs/view_page.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.591345 eyes_soatra-0.0.29/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      835 2023-06-09 08:20:35.000000 eyes_soatra-0.0.29/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)     1363 2023-06-09 08:20:35.000000 eyes_soatra-0.0.29/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-06-09 08:20:35.000000 eyes_soatra-0.0.29/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       34 2023-06-09 08:20:35.000000 eyes_soatra-0.0.29/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-06-09 08:20:35.000000 eyes_soatra-0.0.29/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-06-09 08:20:35.596137 eyes_soatra-0.0.29/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1122 2023-06-09 08:20:33.000000 eyes_soatra-0.0.29/setup.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-09 08:20:35.595744 eyes_soatra-0.0.29/test/
--rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.29/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.29/test/test1.py
--rw-r--r--   0 soatra     (501) staff       (20)      241 2023-06-07 04:03:02.000000 eyes_soatra-0.0.29/test/test2.py
--rw-r--r--   0 soatra     (501) staff       (20)      210 2023-06-07 04:38:58.000000 eyes_soatra-0.0.29/test/test3.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.505958 eyes_soatra-0.0.30/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.30/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      835 2023-07-07 03:15:14.505799 eyes_soatra-0.0.30/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      330 2023-06-02 06:41:30.000000 eyes_soatra-0.0.30/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.492421 eyes_soatra-0.0.30/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.30/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.494502 eyes_soatra-0.0.30/eyes_soatra/constant/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.30/eyes_soatra/constant/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.494876 eyes_soatra-0.0.30/eyes_soatra/constant/area/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-06-14 00:49:26.000000 eyes_soatra-0.0.30/eyes_soatra/constant/area/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)    19032 2023-06-14 01:12:10.000000 eyes_soatra-0.0.30/eyes_soatra/constant/area/id.py
+-rw-r--r--   0 soatra     (501) staff       (20)      233 2023-06-14 03:16:23.000000 eyes_soatra-0.0.30/eyes_soatra/constant/classes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.495378 eyes_soatra-0.0.30/eyes_soatra/constant/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.496192 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/end.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.497130 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/end.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/start.py
+-rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.497768 eyes_soatra-0.0.30/eyes_soatra/constant/depends/view/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/view/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/view/no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/view/not_found.py
+-rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.30/eyes_soatra/constant/labels.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.498168 eyes_soatra-0.0.30/eyes_soatra/constant/libs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.30/eyes_soatra/constant/libs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      387 2023-06-09 08:18:33.000000 eyes_soatra-0.0.30/eyes_soatra/constant/libs/requests.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.498539 eyes_soatra-0.0.30/eyes_soatra/constant/user/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.30/eyes_soatra/constant/user/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.30/eyes_soatra/constant/user/user_agents.py
+-rw-r--r--   0 soatra     (501) staff       (20)      844 2023-06-07 03:44:07.000000 eyes_soatra-0.0.30/eyes_soatra/constant/vars.py
+-rw-r--r--   0 soatra     (501) staff       (20)      174 2023-06-14 04:10:56.000000 eyes_soatra-0.0.30/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.501652 eyes_soatra-0.0.30/eyes_soatra/funcs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.502010 eyes_soatra-0.0.30/eyes_soatra/funcs/listener/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-06-14 00:49:35.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/listener/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9251 2023-06-14 07:16:46.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/listener/watch_changes.py
+-rw-r--r--   0 soatra     (501) staff       (20)    20149 2023-06-09 08:49:06.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/time_app.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.504278 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      602 2023-06-14 06:18:06.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/console.py
+-rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/dict.py
+-rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/list.py
+-rw-r--r--   0 soatra     (501) staff       (20)       82 2023-06-14 03:20:51.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/number.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2624 2023-06-14 04:22:54.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/string.py
+-rw-r--r--   0 soatra     (501) staff       (20)       99 2023-06-14 06:54:22.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/time.py
+-rw-r--r--   0 soatra     (501) staff       (20)    14223 2023-07-07 03:11:17.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/view_page.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.493447 eyes_soatra-0.0.30/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      835 2023-07-07 03:15:14.000000 eyes_soatra-0.0.30/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)     1644 2023-07-07 03:15:14.000000 eyes_soatra-0.0.30/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-07-07 03:15:14.000000 eyes_soatra-0.0.30/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       34 2023-07-07 03:15:14.000000 eyes_soatra-0.0.30/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-07-07 03:15:14.000000 eyes_soatra-0.0.30/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-07-07 03:15:14.506008 eyes_soatra-0.0.30/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1122 2023-07-07 03:14:34.000000 eyes_soatra-0.0.30/setup.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1123 2023-06-02 02:26:19.000000 eyes_soatra-0.0.30/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.505450 eyes_soatra-0.0.30/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.30/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.30/test/test1.py
+-rw-r--r--   0 soatra     (501) staff       (20)      794 2023-07-07 03:11:42.000000 eyes_soatra-0.0.30/test/test2.py
```

### Comparing `eyes_soatra-0.0.29/PKG-INFO` & `eyes_soatra-0.0.30/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes_soatra
-Version: 0.0.29
+Version: 0.0.30
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/end.py` & `eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/end.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/period.py` & `eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/period.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.29/eyes_soatra/constant/depends/app_date/formats/start.py` & `eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/start.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.29/eyes_soatra/constant/depends/view/not_found.py` & `eyes_soatra-0.0.30/eyes_soatra/constant/depends/view/not_found.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.29/eyes_soatra/constant/user/user_agents.py` & `eyes_soatra-0.0.30/eyes_soatra/constant/user/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.29/eyes_soatra/constant/vars.py` & `eyes_soatra-0.0.30/eyes_soatra/constant/vars.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.29/eyes_soatra/funcs/time_app.py` & `eyes_soatra-0.0.30/eyes_soatra/funcs/time_app.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.29/eyes_soatra/funcs/utils/string.py` & `eyes_soatra-0.0.30/eyes_soatra/funcs/utils/string.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,8 +108,10 @@
     path = remove_slash(path)
     
     if not '/' in path:
         return True
 
     return False
 
-
+def clean_url(url):
+    if url:
+        return __re.sub(r'\s+', '', remove_slash(url))
```

### Comparing `eyes_soatra-0.0.29/eyes_soatra/funcs/view_page.py` & `eyes_soatra-0.0.30/eyes_soatra/funcs/view_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!python3
 from eyes_soatra.constant.depends.view.no_data import depends as __depends_no_data
 from eyes_soatra.constant.depends.view.not_found import depends as __depends_404
 from eyes_soatra.constant.user.user_agents import User_Agents as __User_Agents
 from eyes_soatra.constant.libs.requests import requests as __requests
-from eyes_soatra.constant.vars import header_xpaths as __header_xpaths_all
 from eyes_soatra.constant.vars import remove_tags as __remove_tags
 from eyes_soatra.funcs.utils.string import strip_space as __strip_space
 from eyes_soatra.funcs.utils.string import back_home as __back_home
 from eyes_soatra.funcs.utils.string import protocol as __protocol
 from eyes_soatra.funcs.utils.string import join_path as __join_path
 from eyes_soatra.funcs.utils.string import get_domain as __get_domain
 from eyes_soatra.funcs.utils.string import raw_url as __raw_url
@@ -18,24 +17,37 @@
 
 import jellyfish as __jellyfish
 import random as __random
 import time as __time
 import re as __re
 
 # private global variables
-__separator = '\||-|:'
+__separator = '\||-|:|。'
 __header_min_length = 3
 __paragraph_min_length = 7
 __content_min_length = 1
 __container = 'self::div or self::span or self::table'
 __header_xpaths = [
     '//title',
     '//h1[self::*//text() and last()=1]',
     '//h2[self::*//text() and last()=1]'
 ]
+__header_xpaths_all = [
+    '//title',
+    '//h1',
+    '//h2',
+    '//h3',
+    '//h4',
+    '//h5',
+    '//h6',
+    '//p',
+
+    '//div',
+    '//span',
+]
 __paragraph_xpaths = [
     '//p[@class="no_data"]',
     '//h1[self::*//text()]/following-sibling::p[1]',
     '//h1[self::*//text()]/following-sibling::*//p[1]',
     f'//*[({__container}) and self::*//h1[self::*//text()] and self::*/*[last()=1]]/following-sibling::*[1][{__container}]//p[1]'
 ]
 __content_xpaths = [
@@ -305,15 +317,16 @@
                     'error': f'Server error responses: {status_code}',
                     'redirected': redirected,
                     'url': current_url,
                     'status': status_code,
                     'tried': tried,
                 }
 
-            html = __html.fromstring(response.content)
+            text = __re.sub('(<\?.*\?>)', '', response.text + response.content.decode())
+            html = __html.fromstring(text)
             __etree.strip_elements(html, *__remove_tags)
             
             if allow_redirects:
                 meta_refresh = html.xpath("//meta[translate(@http-equiv,'REFSH','refsh')='refresh']/@content")
                 
                 if len(meta_refresh):
                     if tried < tries_forward:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eyes_soatra-0.0.29/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.30/eyes_soatra.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes-soatra
-Version: 0.0.29
+Version: 0.0.30
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.29/eyes_soatra.egg-info/SOURCES.txt` & `eyes_soatra-0.0.30/eyes_soatra.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 LICENSE
 README.md
 setup.py
+start.py
 eyes_soatra/__init__.py
 eyes_soatra/eyes.py
 eyes_soatra.egg-info/PKG-INFO
 eyes_soatra.egg-info/SOURCES.txt
 eyes_soatra.egg-info/dependency_links.txt
 eyes_soatra.egg-info/requires.txt
 eyes_soatra.egg-info/top_level.txt
 eyes_soatra/constant/__init__.py
+eyes_soatra/constant/classes.py
 eyes_soatra/constant/labels.py
 eyes_soatra/constant/vars.py
+eyes_soatra/constant/area/__init__.py
+eyes_soatra/constant/area/id.py
 eyes_soatra/constant/depends/__init__.py
 eyes_soatra/constant/depends/app_date/__init__.py
 eyes_soatra/constant/depends/app_date/end.py
 eyes_soatra/constant/depends/app_date/period.py
 eyes_soatra/constant/depends/app_date/start.py
 eyes_soatra/constant/depends/app_date/formats/__init__.py
 eyes_soatra/constant/depends/app_date/formats/end.py
@@ -26,15 +30,19 @@
 eyes_soatra/constant/libs/__init__.py
 eyes_soatra/constant/libs/requests.py
 eyes_soatra/constant/user/__init__.py
 eyes_soatra/constant/user/user_agents.py
 eyes_soatra/funcs/__init__.py
 eyes_soatra/funcs/time_app.py
 eyes_soatra/funcs/view_page.py
+eyes_soatra/funcs/listener/__init__.py
+eyes_soatra/funcs/listener/watch_changes.py
 eyes_soatra/funcs/utils/__init__.py
+eyes_soatra/funcs/utils/console.py
 eyes_soatra/funcs/utils/dict.py
 eyes_soatra/funcs/utils/list.py
+eyes_soatra/funcs/utils/number.py
 eyes_soatra/funcs/utils/string.py
+eyes_soatra/funcs/utils/time.py
 test/test.py
 test/test1.py
-test/test2.py
-test/test3.py
+test/test2.py
```

### Comparing `eyes_soatra-0.0.29/setup.py` & `eyes_soatra-0.0.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.29'
+VERSION = '0.0.30'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

### Comparing `eyes_soatra-0.0.29/test/test.py` & `eyes_soatra-0.0.30/test/test.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.29/test/test1.py` & `eyes_soatra-0.0.30/test/test1.py`

 * *Files identical despite different names*

