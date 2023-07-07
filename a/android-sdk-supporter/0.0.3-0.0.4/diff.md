# Comparing `tmp/android-sdk-supporter-0.0.3.tar.gz` & `tmp/android-sdk-supporter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android-sdk-supporter-0.0.3.tar", last modified: Fri Jul  7 03:12:47 2023, max compression
+gzip compressed data, was "android-sdk-supporter-0.0.4.tar", last modified: Fri Jul  7 03:15:31 2023, max compression
```

## Comparing `android-sdk-supporter-0.0.3.tar` & `android-sdk-supporter-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 03:12:47.215618 android-sdk-supporter-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 03:12:47.215618 android-sdk-supporter-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1945 2023-07-07 03:12:46.000000 android-sdk-supporter-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 03:12:47.214618 android-sdk-supporter-0.0.3/android_sdk_supporter/
--rw-r--r--   0 root         (0) root         (0)       83 2023-07-07 03:12:46.000000 android-sdk-supporter-0.0.3/android_sdk_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-07-07 03:12:46.000000 android-sdk-supporter-0.0.3/android_sdk_supporter/build_tools.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-07-07 03:12:46.000000 android-sdk-supporter-0.0.3/android_sdk_supporter/cmdline_tools.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-07-07 03:12:46.000000 android-sdk-supporter-0.0.3/android_sdk_supporter/platform_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 03:12:47.215618 android-sdk-supporter-0.0.3/android_sdk_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 03:12:46.000000 android-sdk-supporter-0.0.3/android_sdk_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-07 03:12:47.000000 android-sdk-supporter-0.0.3/android_sdk_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 03:12:46.000000 android-sdk-supporter-0.0.3/android_sdk_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 03:12:46.000000 android-sdk-supporter-0.0.3/android_sdk_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-07 03:12:46.000000 android-sdk-supporter-0.0.3/android_sdk_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 03:12:47.215618 android-sdk-supporter-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      615 2023-07-07 03:12:46.000000 android-sdk-supporter-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 03:15:31.721465 android-sdk-supporter-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 03:15:31.721465 android-sdk-supporter-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 03:15:31.719465 android-sdk-supporter-0.0.4/android_sdk_supporter/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/android_sdk_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/android_sdk_supporter/build_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/android_sdk_supporter/cmdline_tools.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/android_sdk_supporter/platform_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 03:15:31.720465 android-sdk-supporter-0.0.4/android_sdk_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/android_sdk_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/android_sdk_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/android_sdk_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/android_sdk_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/android_sdk_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 03:15:31.721465 android-sdk-supporter-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      615 2023-07-07 03:15:31.000000 android-sdk-supporter-0.0.4/setup.py
```

### Comparing `android-sdk-supporter-0.0.3/PKG-INFO` & `android-sdk-supporter-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-sdk-supporter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Android sdk supporter
 Home-page: https://github.com/automatethem/android-sdk-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `android-sdk-supporter-0.0.3/README.md` & `android-sdk-supporter-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `android-sdk-supporter-0.0.3/android_sdk_supporter/build_tools.py` & `android-sdk-supporter-0.0.4/android_sdk_supporter/build_tools.py`

 * *Files identical despite different names*

### Comparing `android-sdk-supporter-0.0.3/android_sdk_supporter/cmdline_tools.py` & `android-sdk-supporter-0.0.4/android_sdk_supporter/cmdline_tools.py`

 * *Files identical despite different names*

### Comparing `android-sdk-supporter-0.0.3/android_sdk_supporter/platform_tools.py` & `android-sdk-supporter-0.0.4/android_sdk_supporter/platform_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if self.android_sdk_directory:
             adb = f"{self.android_sdk_directory}/platform-tools/adb"
         else:
             adb = "adb"
         cmd = f"{adb} -s {self.devices[0]} shell svc data enable"
         os.system(cmd)
 
-    def cmd(self, command):
+    def cmd(self, command):
         if self.android_sdk_directory:
             command = f"{self.android_sdk_directory}/platform-tools/{command}"
         os.system(command)
         
 if __name__ == "__main__":
     android_sdk_directory = os.path.dirname(__file__) + "/android_sdk"
     platform_tools = PlatformTools(android_sdk_directory)
```

### Comparing `android-sdk-supporter-0.0.3/android_sdk_supporter.egg-info/PKG-INFO` & `android-sdk-supporter-0.0.4/android_sdk_supporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-sdk-supporter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Android sdk supporter
 Home-page: https://github.com/automatethem/android-sdk-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `android-sdk-supporter-0.0.3/setup.py` & `android-sdk-supporter-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='android-sdk-supporter',
-	version='0.0.3',
+	version='0.0.4',
 	description='Android sdk supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/android-sdk-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

