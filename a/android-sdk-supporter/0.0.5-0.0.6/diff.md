# Comparing `tmp/android-sdk-supporter-0.0.5.tar.gz` & `tmp/android-sdk-supporter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android-sdk-supporter-0.0.5.tar", last modified: Fri Jul  7 09:28:45 2023, max compression
+gzip compressed data, was "android-sdk-supporter-0.0.6.tar", last modified: Fri Jul  7 09:31:28 2023, max compression
```

## Comparing `android-sdk-supporter-0.0.5.tar` & `android-sdk-supporter-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:28:45.384491 android-sdk-supporter-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 09:28:45.384491 android-sdk-supporter-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1945 2023-07-07 09:28:44.000000 android-sdk-supporter-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:28:45.383491 android-sdk-supporter-0.0.5/android_sdk_supporter/
--rw-r--r--   0 root         (0) root         (0)       83 2023-07-07 09:28:44.000000 android-sdk-supporter-0.0.5/android_sdk_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-07-07 09:28:44.000000 android-sdk-supporter-0.0.5/android_sdk_supporter/build_tools.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-07-07 09:28:44.000000 android-sdk-supporter-0.0.5/android_sdk_supporter/cmdline_tools.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-07-07 09:28:44.000000 android-sdk-supporter-0.0.5/android_sdk_supporter/platform_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:28:45.383491 android-sdk-supporter-0.0.5/android_sdk_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 09:28:45.000000 android-sdk-supporter-0.0.5/android_sdk_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-07 09:28:45.000000 android-sdk-supporter-0.0.5/android_sdk_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 09:28:45.000000 android-sdk-supporter-0.0.5/android_sdk_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 09:28:45.000000 android-sdk-supporter-0.0.5/android_sdk_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-07 09:28:45.000000 android-sdk-supporter-0.0.5/android_sdk_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 09:28:45.384491 android-sdk-supporter-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      615 2023-07-07 09:28:44.000000 android-sdk-supporter-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:31:28.723812 android-sdk-supporter-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 09:31:28.723812 android-sdk-supporter-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-07-07 09:31:27.000000 android-sdk-supporter-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:31:28.721812 android-sdk-supporter-0.0.6/android_sdk_supporter/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-07 09:31:28.000000 android-sdk-supporter-0.0.6/android_sdk_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-07-07 09:31:28.000000 android-sdk-supporter-0.0.6/android_sdk_supporter/build_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-07-07 09:31:28.000000 android-sdk-supporter-0.0.6/android_sdk_supporter/cmdline_tools.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-07-07 09:31:28.000000 android-sdk-supporter-0.0.6/android_sdk_supporter/platform_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:31:28.722812 android-sdk-supporter-0.0.6/android_sdk_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 09:31:28.000000 android-sdk-supporter-0.0.6/android_sdk_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-07 09:31:28.000000 android-sdk-supporter-0.0.6/android_sdk_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 09:31:28.000000 android-sdk-supporter-0.0.6/android_sdk_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 09:31:28.000000 android-sdk-supporter-0.0.6/android_sdk_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-07 09:31:28.000000 android-sdk-supporter-0.0.6/android_sdk_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 09:31:28.723812 android-sdk-supporter-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      615 2023-07-07 09:31:28.000000 android-sdk-supporter-0.0.6/setup.py
```

### Comparing `android-sdk-supporter-0.0.5/PKG-INFO` & `android-sdk-supporter-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-sdk-supporter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Android sdk supporter
 Home-page: https://github.com/automatethem/android-sdk-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `android-sdk-supporter-0.0.5/README.md` & `android-sdk-supporter-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `android-sdk-supporter-0.0.5/android_sdk_supporter/build_tools.py` & `android-sdk-supporter-0.0.6/android_sdk_supporter/build_tools.py`

 * *Files identical despite different names*

### Comparing `android-sdk-supporter-0.0.5/android_sdk_supporter/cmdline_tools.py` & `android-sdk-supporter-0.0.6/android_sdk_supporter/cmdline_tools.py`

 * *Files identical despite different names*

### Comparing `android-sdk-supporter-0.0.5/android_sdk_supporter/platform_tools.py` & `android-sdk-supporter-0.0.6/android_sdk_supporter/platform_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,27 +67,27 @@
             self.check_devices()
             
         if self.devices:
             if self.android_sdk_directory:
                 adb = f"{self.android_sdk_directory}/platform-tools/adb"
             else:
                 adb = "adb"
-            cmd = f"{adb} -s {self.devices[0]["device"]} shell svc data disable"
+            cmd = f"{adb} -s {self.devices[0]['device']} shell svc data disable"
             os.system(cmd)
 
     def data_enable(self):
         if not self.devices:
             self.check_devices()
         
         if self.devices:        
             if self.android_sdk_directory:
                 adb = f"{self.android_sdk_directory}/platform-tools/adb"
             else:
                 adb = "adb"
-            cmd = f"{adb} -s {self.devices[0]["device"]} shell svc data enable"
+            cmd = f"{adb} -s {self.devices[0]['device']} shell svc data enable"
             os.system(cmd)
 
     def cmd(self, command):
         if self.android_sdk_directory:
             command = f"{self.android_sdk_directory}/platform-tools/{command}"
         os.system(command)
```

### Comparing `android-sdk-supporter-0.0.5/android_sdk_supporter.egg-info/PKG-INFO` & `android-sdk-supporter-0.0.6/android_sdk_supporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-sdk-supporter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Android sdk supporter
 Home-page: https://github.com/automatethem/android-sdk-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `android-sdk-supporter-0.0.5/setup.py` & `android-sdk-supporter-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='android-sdk-supporter',
-	version='0.0.5',
+	version='0.0.6',
 	description='Android sdk supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/android-sdk-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

