# Comparing `tmp/mozdevice-4.1.0.tar.gz` & `tmp/mozdevice-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozdevice-4.1.0.tar", last modified: Mon Jan 16 21:43:24 2023, max compression
+gzip compressed data, was "dist/mozdevice-4.1.1.tar", last modified: Fri Jul  7 16:56:55 2023, max compression
```

## Comparing `mozdevice-4.1.0.tar` & `mozdevice-4.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-01-16 21:43:24.461849 mozdevice-4.1.0/
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      420 2023-01-16 21:43:24.461849 mozdevice-4.1.0/PKG-INFO
-drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-01-16 21:43:24.461849 mozdevice-4.1.0/mozdevice/
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     6920 2023-01-03 17:04:44.000000 mozdevice-4.1.0/mozdevice/__init__.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)   182378 2023-01-06 17:28:12.000000 mozdevice-4.1.0/mozdevice/adb.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      376 2023-01-03 17:04:44.000000 mozdevice-4.1.0/mozdevice/adb_android.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    10343 2023-01-03 17:04:44.000000 mozdevice-4.1.0/mozdevice/remote_process_monitor.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1541 2023-01-03 17:04:44.000000 mozdevice-4.1.0/mozdevice/version_codes.py
-drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-01-16 21:43:24.461849 mozdevice-4.1.0/mozdevice.egg-info/
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      420 2023-01-16 21:43:24.000000 mozdevice-4.1.0/mozdevice.egg-info/PKG-INFO
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      341 2023-01-16 21:43:24.000000 mozdevice-4.1.0/mozdevice.egg-info/SOURCES.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-01-16 21:43:24.000000 mozdevice-4.1.0/mozdevice.egg-info/dependency_links.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-01-16 21:43:24.000000 mozdevice-4.1.0/mozdevice.egg-info/not-zip-safe
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       12 2023-01-16 21:43:24.000000 mozdevice-4.1.0/mozdevice.egg-info/requires.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       10 2023-01-16 21:43:24.000000 mozdevice-4.1.0/mozdevice.egg-info/top_level.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       67 2023-01-16 21:43:24.461849 mozdevice-4.1.0/setup.cfg
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1075 2023-01-16 21:43:01.000000 mozdevice-4.1.0/setup.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-07 16:56:55.000000 mozdevice-4.1.1/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      439 2023-07-07 16:56:55.000000 mozdevice-4.1.1/PKG-INFO
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     6920 2023-03-10 23:28:57.000000 mozdevice-4.1.1/mozdevice/__init__.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)   182366 2023-03-10 23:28:57.000000 mozdevice-4.1.1/mozdevice/adb.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      376 2023-03-10 23:28:57.000000 mozdevice-4.1.1/mozdevice/adb_android.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    10343 2023-03-10 23:28:57.000000 mozdevice-4.1.1/mozdevice/remote_process_monitor.py
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1541 2023-03-10 23:28:57.000000 mozdevice-4.1.1/mozdevice/version_codes.py
+drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      439 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/PKG-INFO
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      377 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       37 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/entry_points.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/not-zip-safe
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       12 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/requires.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       10 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/top_level.txt
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       67 2023-07-07 16:56:55.000000 mozdevice-4.1.1/setup.cfg
+-rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1075 2023-07-07 16:25:07.000000 mozdevice-4.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mozdevice-4.1.0/mozdevice/__init__.py` & `mozdevice-4.1.1/mozdevice/__init__.py`

 * *Files identical despite different names*

### Comparing `mozdevice-4.1.0/mozdevice/adb.py` & `mozdevice-4.1.1/mozdevice/adb.py`

 * *Files 0% similar despite different names*

```diff
@@ -2973,15 +2973,15 @@
         # remove trailing /
         local = os.path.normpath(local)
         remote = posixpath.normpath(remote)
         copy_required = False
         sdcard_remote = None
         if os.path.isfile(local) and self.is_dir(remote):
             # force push to use the correct filename in the remote directory
-            remote = posixpath.join(remote, posixpath.basename(local))
+            remote = posixpath.join(remote, os.path.basename(local))
         elif os.path.isdir(local):
             copy_required = True
             temp_parent = tempfile.mkdtemp()
             remote_name = os.path.basename(remote)
             new_local = os.path.join(temp_parent, remote_name)
             dir_util.copy_tree(local, new_local)
             local = new_local
@@ -3008,15 +3008,15 @@
                 # intermediate location under /data/local/tmp which
                 # should be writable by the shell user, then using
                 # run-as, copy the data into the app's internal
                 # storage.
                 try:
                     with tempfile.NamedTemporaryFile(delete=True) as tmpf:
                         intermediate = posixpath.join(
-                            "/data/local/tmp", posixpath.basename(tmpf.name)
+                            "/data/local/tmp", os.path.basename(tmpf.name)
                         )
                     self.command_output(["push", local, intermediate], timeout=timeout)
                     self.chmod(intermediate, recursive=True, timeout=timeout)
                     parent_dir = posixpath.dirname(remote)
                     if not self.is_dir(parent_dir, timeout=timeout):
                         self.mkdir(parent_dir, parents=True, timeout=timeout)
                     self.cp(intermediate, remote, recursive=True, timeout=timeout)
@@ -3034,15 +3034,15 @@
             # directories which can not be written by "other" by first
             # pushing the source to the sdcard which has no
             # permissions issues, then moving it from the sdcard to
             # the final destination.
             self._logger.info("Falling back to using intermediate /sdcard in push.")
             self.mkdir(posixpath.dirname(remote), parents=True, timeout=timeout)
             with tempfile.NamedTemporaryFile(delete=True) as tmpf:
-                sdcard_remote = posixpath.join("/sdcard", posixpath.basename(tmpf.name))
+                sdcard_remote = posixpath.join("/sdcard", os.path.basename(tmpf.name))
             self.command_output(["push", local, sdcard_remote], timeout=timeout)
             self.cp(sdcard_remote, remote, recursive=True, timeout=timeout)
         except BaseException:
             raise
         finally:
             self._sync(timeout=timeout)
             if copy_required:
@@ -3110,15 +3110,15 @@
                 # from the app's internal storage to a temporary
                 # intermediate location under /data/local/tmp which
                 # should be writable by the shell user, then using
                 # pull, to copy the data off of the device.
                 try:
                     with tempfile.NamedTemporaryFile(delete=True) as tmpf:
                         intermediate = posixpath.join(
-                            "/data/local/tmp", posixpath.basename(tmpf.name)
+                            "/data/local/tmp", os.path.basename(tmpf.name)
                         )
                     # When using run-as <app>, we must first use the
                     # shell to create the intermediate and chmod it
                     # before the app will be able to access it.
                     if self.is_dir(remote, timeout=timeout):
                         self.mkdir(
                             posixpath.join(intermediate, remote_name),
@@ -3467,29 +3467,29 @@
         # already exists and whether they are a directory or file.
         if not self.exists(source, timeout=timeout):
             raise ADBError("cp: can't stat '%s': No such file or directory" % source)
 
         if self.is_file(source, timeout=timeout):
             if self.is_dir(destination, timeout=timeout):
                 # Copy the source file into the destination directory
-                destination = posixpath.join(destination, posixpath.basename(source))
+                destination = posixpath.join(destination, os.path.basename(source))
             self.shell_output("dd if=%s of=%s" % (source, destination), timeout=timeout)
             self.chmod(destination, recursive=recursive, timeout=timeout)
             self._sync(timeout=timeout)
             return
 
         if self.is_file(destination, timeout=timeout):
             raise ADBError("cp: %s: Not a directory" % destination)
 
         if not recursive:
             raise ADBError("cp: omitting directory '%s'" % source)
 
         if self.is_dir(destination, timeout=timeout):
             # Copy the source directory into the destination directory.
-            destination_dir = posixpath.join(destination, posixpath.basename(source))
+            destination_dir = posixpath.join(destination, os.path.basename(source))
         else:
             # Copy the contents of the source directory into the
             # destination directory.
             destination_dir = destination
 
         try:
             # Do not create parent directories since cp does not.
```

### Comparing `mozdevice-4.1.0/mozdevice/remote_process_monitor.py` & `mozdevice-4.1.1/mozdevice/remote_process_monitor.py`

 * *Files identical despite different names*

### Comparing `mozdevice-4.1.0/mozdevice/version_codes.py` & `mozdevice-4.1.1/mozdevice/version_codes.py`

 * *Files identical despite different names*

### Comparing `mozdevice-4.1.0/setup.py` & `mozdevice-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
 from setuptools import setup
 
 PACKAGE_NAME = "mozdevice"
-PACKAGE_VERSION = "4.1.0"
+PACKAGE_VERSION = "4.1.1"
 
 deps = ["mozlog >= 6.0"]
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
     description="Mozilla-authored device management",
```

