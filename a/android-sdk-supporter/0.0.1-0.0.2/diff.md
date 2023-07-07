# Comparing `tmp/android-sdk-supporter-0.0.1.tar.gz` & `tmp/android-sdk-supporter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android-sdk-supporter-0.0.1.tar", last modified: Fri Jul  7 02:05:17 2023, max compression
+gzip compressed data, was "android-sdk-supporter-0.0.2.tar", last modified: Fri Jul  7 02:36:31 2023, max compression
```

## Comparing `android-sdk-supporter-0.0.1.tar` & `android-sdk-supporter-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 02:05:17.860318 android-sdk-supporter-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 02:05:17.860318 android-sdk-supporter-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1945 2023-07-07 02:05:16.000000 android-sdk-supporter-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 02:05:17.857318 android-sdk-supporter-0.0.1/android_sdk_supporter/
--rw-r--r--   0 root         (0) root         (0)       83 2023-07-07 02:05:16.000000 android-sdk-supporter-0.0.1/android_sdk_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-07-07 02:05:16.000000 android-sdk-supporter-0.0.1/android_sdk_supporter/build_tools.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-07-07 02:05:16.000000 android-sdk-supporter-0.0.1/android_sdk_supporter/cmdline_tools.py
--rw-r--r--   0 root         (0) root         (0)     5458 2023-07-07 02:05:16.000000 android-sdk-supporter-0.0.1/android_sdk_supporter/platform_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 02:05:17.859318 android-sdk-supporter-0.0.1/android_sdk_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 02:05:17.000000 android-sdk-supporter-0.0.1/android_sdk_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-07 02:05:17.000000 android-sdk-supporter-0.0.1/android_sdk_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 02:05:17.000000 android-sdk-supporter-0.0.1/android_sdk_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 02:05:17.000000 android-sdk-supporter-0.0.1/android_sdk_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-07 02:05:17.000000 android-sdk-supporter-0.0.1/android_sdk_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 02:05:17.860318 android-sdk-supporter-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      615 2023-07-07 02:05:16.000000 android-sdk-supporter-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 02:36:31.156189 android-sdk-supporter-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 02:36:31.156189 android-sdk-supporter-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-07-07 02:36:05.000000 android-sdk-supporter-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 02:36:31.155189 android-sdk-supporter-0.0.2/android_sdk_supporter/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-07 02:36:05.000000 android-sdk-supporter-0.0.2/android_sdk_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-07-07 02:36:05.000000 android-sdk-supporter-0.0.2/android_sdk_supporter/build_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-07-07 02:36:05.000000 android-sdk-supporter-0.0.2/android_sdk_supporter/cmdline_tools.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-07-07 02:36:05.000000 android-sdk-supporter-0.0.2/android_sdk_supporter/platform_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 02:36:31.156189 android-sdk-supporter-0.0.2/android_sdk_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-07 02:36:30.000000 android-sdk-supporter-0.0.2/android_sdk_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-07 02:36:30.000000 android-sdk-supporter-0.0.2/android_sdk_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 02:36:30.000000 android-sdk-supporter-0.0.2/android_sdk_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 02:36:30.000000 android-sdk-supporter-0.0.2/android_sdk_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-07 02:36:30.000000 android-sdk-supporter-0.0.2/android_sdk_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 02:36:31.156189 android-sdk-supporter-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      615 2023-07-07 02:36:05.000000 android-sdk-supporter-0.0.2/setup.py
```

### Comparing `android-sdk-supporter-0.0.1/PKG-INFO` & `android-sdk-supporter-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-sdk-supporter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Android sdk supporter
 Home-page: https://github.com/automatethem/android-sdk-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `android-sdk-supporter-0.0.1/README.md` & `android-sdk-supporter-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `android-sdk-supporter-0.0.1/android_sdk_supporter/build_tools.py` & `android-sdk-supporter-0.0.2/android_sdk_supporter/platform_tools.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,87 @@
 import os
 import platform
 import subprocess
 import zipfile
 import sys
 import shutil
 
-class BuildTools:
+class PlatformTools:
     def __init__(self, android_sdk_directory=None):
         super().__init__()
         self.android_sdk_directory = android_sdk_directory
+        self.devices = []
 
-        #build-tools
-        if platform.system() == 'Darwin': #맥
-            from_zip = f"{self.android_sdk_directory}/build-tools_r34-rc4-macosx.zip"
-            if not os.path.exists(from_zip):
-                zip_file = zipfile.ZipFile(from_zip)
-                zip_file.extractall(self.android_sdk_directory)
-                zip_file.close()
-                shutil.move(f"{self.android_sdk_directory}/android-UpsideDownCake", f"{self.android_sdk_directory}/build-tools")
-        elif platform.system() == 'Windows': #윈도우
-            from_zip = f"{self.android_sdk_directory}/build-tools_r34-rc4-windows.zip"
-            if not os.path.exists(from_zip):
-                zip_file = zipfile.ZipFile(from_zip)
-                zip_file.extractall(self.android_sdk_directory)
-                zip_file.close()
-                shutil.move(f"{self.android_sdk_directory}/android-UpsideDownCake", f"{self.android_sdk_directory}/build-tools")
-        elif platform.system() == 'Linux': #리눅스 (구글 콜랩)
-            from_zip = f"{self.android_sdk_directory}/build-tools_r34-rc4-linux.zip"
-            if not os.path.exists(from_zip):
-                zip_file = zipfile.ZipFile(from_zip)
-                zip_file.extractall(self.android_sdk_directory)
-                zip_file.close()
-                shutil.move(f"{self.android_sdk_directory}/android-UpsideDownCake", f"{self.android_sdk_directory}/build-tools")
+        if self.android_sdk_directory:
+            #platform-tools
+            platform_tools_directory = f"{self.android_sdk_directory}/platform-tools"
+            if not os.path.exists(platform_tools_directory):
+                if platform.system() == 'Darwin': #맥
+                    from_zip = f"{self.android_sdk_directory}/platform-tools_r34.0.3-darwin.zip"
+                    zip_file = zipfile.ZipFile(from_zip)
+                    zip_file.extractall(self.android_sdk_directory)
+                    zip_file.close()
+                elif platform.system() == 'Windows': #윈도우
+                    from_zip = f"{self.android_sdk_directory}/platform-tools_r34.0.3-windows.zip"
+                    zip_file = zipfile.ZipFile(from_zip)
+                    zip_file.extractall(self.android_sdk_directory)
+                    zip_file.close()
+                elif platform.system() == 'Linux': #리눅스 (구글 콜랩)
+                    from_zip = f"{self.android_sdk_directory}/platform-tools_r34.0.3-linux.zip"
+                    zip_file = zipfile.ZipFile(from_zip)
+                    zip_file.extractall(self.android_sdk_directory)
+                    zip_file.close()
+                
+    '''
+$ adb devices
+List of devices attached
+R95RB00QRCY     offline
+
+
+$ adb devices
+List of devices attached
+R95RB00QRCY     unauthorized
+
+
+$ adb devices
+List of devices attached
+R95RB00QRCY     device    
+    '''
+    def check_devices(self):   
+        if self.android_sdk_directory:
+            cmd = f"{self.android_sdk_directory}/platform-tools/adb"
+        else:
+            cmd = "adb"
+        outputs = subprocess.check_output([cmd, "devices"]).decode('utf-8')
+        devices = []
+        for output in outputs.split("\n")[1:]:
+            output = output.strip()
+            #print(output) #R95RB00QRCY     device
+            if output:
+                device, status = output.split("\t")
+                devices.append({"device": device, "status": status})
+        #print(devices) #[{'device': 'R95RB00QRCY', 'status': 'unauthorized'}]
+        return devices
+    
+    def data_disable(self):
+        if self.android_sdk_directory:
+            adb = f"{self.android_sdk_directory}/platform-tools/adb"
+        else:
+            adb = "adb"
+        cmd = f"{adb} -s {self.devices[0]} shell svc data disable"
+        os.system(cmd)
+
+    def data_enable(self):
+        if self.android_sdk_directory:
+            adb = f"{self.android_sdk_directory}/platform-tools/adb"
+        else:
+            adb = "adb"
+        cmd = f"{adb} -s {self.devices[0]} shell svc data enable"
+        os.system(cmd)
+
+if __name__ == "__main__":
+    android_sdk_directory = os.path.dirname(__file__) + "/android_sdk"
+    platform_tools = PlatformTools(android_sdk_directory)
+
+    devices = platform_tools.check_devices()
+
+    print(devices)
```

### Comparing `android-sdk-supporter-0.0.1/android_sdk_supporter/cmdline_tools.py` & `android-sdk-supporter-0.0.2/android_sdk_supporter/cmdline_tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 import shutil
 
 class CmdlineTools:
     def __init__(self, android_sdk_directory=None):
         super().__init__()
         self.android_sdk_directory = android_sdk_directory
 
-        #cmdline-tools
-        if platform.system() == 'Darwin': #맥
-            from_zip = f"{self.android_sdk_directory}/commandlinetools-mac-9477386_latest.zip"
-            if not os.path.exists(from_zip):
-                zip_file = zipfile.ZipFile(from_zip)
-                zip_file.extractall(self.android_sdk_directory)
-                zip_file.close()
-        elif platform.system() == 'Windows': #윈도우
-            from_zip = f"{self.android_sdk_directory}/commandlinetools-win-9477386_latest.zip"
-            if not os.path.exists(from_zip):
-                zip_file = zipfile.ZipFile(from_zip)
-                zip_file.extractall(self.android_sdk_directory)
-                zip_file.close()
-        elif platform.system() == 'Linux': #리눅스 (구글 콜랩)
-            from_zip = f"{self.android_sdk_directory}/commandlinetools-linux-9477386_latest.zip"
-            if not os.path.exists(from_zip):
-                zip_file = zipfile.ZipFile(from_zip)
-                zip_file.extractall(self.android_sdk_directory)
-                zip_file.close()
+        if self.android_sdk_directory:
+            #cmdline-tools
+            cmdline_tools_directory = f"{self.android_sdk_directory}/cmdline-tools"
+            if not os.path.exists(cmdline_tools_directory):
+                if platform.system() == 'Darwin': #맥
+                    from_zip = f"{self.android_sdk_directory}/commandlinetools-mac-9477386_latest.zip"
+                    zip_file = zipfile.ZipFile(from_zip)
+                    zip_file.extractall(self.android_sdk_directory)
+                    zip_file.close()
+                elif platform.system() == 'Windows': #윈도우
+                    from_zip = f"{self.android_sdk_directory}/commandlinetools-win-9477386_latest.zip"
+                    zip_file = zipfile.ZipFile(from_zip)
+                    zip_file.extractall(self.android_sdk_directory)
+                    zip_file.close()
+                elif platform.system() == 'Linux': #리눅스 (구글 콜랩)
+                    from_zip = f"{self.android_sdk_directory}/commandlinetools-linux-9477386_latest.zip"
+                    zip_file = zipfile.ZipFile(from_zip)
+                    zip_file.extractall(self.android_sdk_directory)
+                    zip_file.close()
+
```

### Comparing `android-sdk-supporter-0.0.1/android_sdk_supporter.egg-info/PKG-INFO` & `android-sdk-supporter-0.0.2/android_sdk_supporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: android-sdk-supporter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Android sdk supporter
 Home-page: https://github.com/automatethem/android-sdk-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `android-sdk-supporter-0.0.1/setup.py` & `android-sdk-supporter-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='android-sdk-supporter',
-	version='0.0.1',
+	version='0.0.2',
 	description='Android sdk supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/android-sdk-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

