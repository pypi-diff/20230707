# Comparing `tmp/vfsfusepy-0.1.0.tar.gz` & `tmp/vfsfusepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfsfusepy-0.1.0.tar", last modified: Tue Jul  4 10:40:19 2023, max compression
+gzip compressed data, was "vfsfusepy-0.1.1.tar", last modified: Fri Jul  7 07:36:55 2023, max compression
```

## Comparing `vfsfusepy-0.1.0.tar` & `vfsfusepy-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 wangzhao (10250) wangzhao (10250)        0 2023-07-04 10:40:19.430962 vfsfusepy-0.1.0/
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)     1066 2023-07-03 10:51:54.000000 vfsfusepy-0.1.0/LICENSE
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)     3100 2023-07-04 10:40:19.430962 vfsfusepy-0.1.0/PKG-INFO
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)     2437 2023-07-04 07:50:08.000000 vfsfusepy-0.1.0/README.md
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)       94 2023-07-04 06:13:00.000000 vfsfusepy-0.1.0/pyproject.toml
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)       33 2023-07-04 05:34:10.000000 vfsfusepy-0.1.0/requirements.txt
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)      823 2023-07-04 10:40:19.458963 vfsfusepy-0.1.0/setup.cfg
-drwxrwxr-x   0 wangzhao (10250) wangzhao (10250)        0 2023-07-04 10:40:19.430962 vfsfusepy-0.1.0/vfsfusepy/
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)       33 2023-07-04 06:13:00.000000 vfsfusepy-0.1.0/vfsfusepy/__init__.py
--rwxrwxr-x   0 wangzhao (10250) wangzhao (10250)     3605 2023-07-04 06:18:24.000000 vfsfusepy-0.1.0/vfsfusepy/__main__.py
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)       22 2023-07-04 06:13:00.000000 vfsfusepy-0.1.0/vfsfusepy/version.py
-drwxrwxr-x   0 wangzhao (10250) wangzhao (10250)        0 2023-07-04 10:40:19.430962 vfsfusepy-0.1.0/vfsfusepy.egg-info/
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)     3100 2023-07-04 10:40:19.000000 vfsfusepy-0.1.0/vfsfusepy.egg-info/PKG-INFO
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)      324 2023-07-04 10:40:19.000000 vfsfusepy-0.1.0/vfsfusepy.egg-info/SOURCES.txt
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)        1 2023-07-04 10:40:19.000000 vfsfusepy-0.1.0/vfsfusepy.egg-info/dependency_links.txt
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)       53 2023-07-04 10:40:19.000000 vfsfusepy-0.1.0/vfsfusepy.egg-info/entry_points.txt
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)       33 2023-07-04 10:40:19.000000 vfsfusepy-0.1.0/vfsfusepy.egg-info/requires.txt
--rw-rw-r--   0 wangzhao (10250) wangzhao (10250)       10 2023-07-04 10:40:19.000000 vfsfusepy-0.1.0/vfsfusepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:36:55.885024 vfsfusepy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 07:36:41.000000 vfsfusepy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-07 07:36:55.885024 vfsfusepy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-07 07:36:41.000000 vfsfusepy-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-07 07:36:41.000000 vfsfusepy-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 07:36:41.000000 vfsfusepy-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-07 07:36:55.889024 vfsfusepy-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:36:55.885024 vfsfusepy-0.1.1/vfsfusepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 07:36:41.000000 vfsfusepy-0.1.1/vfsfusepy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4116 2023-07-07 07:36:41.000000 vfsfusepy-0.1.1/vfsfusepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 07:36:43.000000 vfsfusepy-0.1.1/vfsfusepy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:36:55.885024 vfsfusepy-0.1.1/vfsfusepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-07 07:36:55.000000 vfsfusepy-0.1.1/vfsfusepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-07 07:36:55.000000 vfsfusepy-0.1.1/vfsfusepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:36:55.000000 vfsfusepy-0.1.1/vfsfusepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-07 07:36:55.000000 vfsfusepy-0.1.1/vfsfusepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 07:36:55.000000 vfsfusepy-0.1.1/vfsfusepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 07:36:55.000000 vfsfusepy-0.1.1/vfsfusepy.egg-info/top_level.txt
```

### Comparing `vfsfusepy-0.1.0/LICENSE` & `vfsfusepy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.1.0/README.md` & `vfsfusepy-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 ## Requirements
 
 - Python 3.7 or later
 
 ## Installation
 
+### From PyPI
+
+```bash
+pip install vfsfusepy
+```
+
 ### From Source
 
 1. Clone the repository:
 
 ```bash
 git clone https://github.com/nero19960329/VFS-FUSE.git
 ```
@@ -30,15 +36,17 @@
 ```
 
 ## Usage
 
 To use VFS-FUSE, you need to specify the directory of the Git repository and the mount point of the file system:
 
 ```bash
-python vfsfusepy/__main__.py /path/to/git_dir /path/to/mount_point
+vfs-fuse /path/to/git_dir /path/to/mount_point  # if installed from PyPI
+
+python vfsfusepy/__main__.py /path/to/git_dir /path/to/mount_point  # if installed from source
 ```
 
 Where:
 
 - `git_dir` is the directory of the Git repository that will be used to store and manage file versions.
 - `mount_point` is the directory where the VFS-FUSE file system will be mounted.
 
@@ -46,18 +54,19 @@
 
 ## Example
 
 Here is an example of how to use VFS-FUSE:
 
 ```bash
 # Mount the file system
-python vfsfusepy/__main__.py /data/vfs-root /data/vfs-mount
+mkdir /data/vfs-root
+mkdir /data/vfs-mount
+vfs-fuse /data/vfs-root /data/vfs-mount
 
 # Go to the mount point
-mkdir /data/vfs-mount
 cd /data/vfs-mount
 
 # Create a new file
 echo "Hello, World!" > test.txt
 
 # View the file
 cat test.txt
@@ -65,15 +74,15 @@
 # Remove the file
 rm test.txt
 
 # View the commit history
 git log
 ```
 
-In this example, when you write to test.txt, the file system automatically commits the changes to the Git repository located at /data/vfs-root. You can then use standard Git commands to view the commit history and checkout previous versions of the file.
+In this example, when you write to test.txt, the file system automatically commits the changes to the Git repository located at `/data/vfs-root`. You can then use standard Git commands to view the commit history and checkout previous versions of the file.
 
 ## FAQ
 
 ### Why not use Git directly?
 
 `VFS-FUSE` offers automatic git commits for all file changes, creating a real-time version control system. It simplifies the use of git, allowing operations via a standard file system interface. Essentially, it's git made easy for everyday file operations.
 
@@ -81,10 +90,17 @@
 
 You need to install the FUSE library. On Ubuntu, you can install it with the following command:
 
 ```bash
 sudo apt-get update && sudo apt-get install fuse
 ```
 
+## Contributing
+We welcome contributions to this repository! If you would like to contribute code, please take a moment to read our [contribution guidelines](https://github.com/nero19960329/VFS-FUSE/blob/main/CONTRIBUTING.md).
+
+By following these guidelines, you can ensure that your contributions are in line with our coding standards and testing procedures.
+
+We appreciate your interest and look forward to your contributions!
+
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `vfsfusepy-0.1.0/setup.cfg` & `vfsfusepy-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.1.0/vfsfusepy/__main__.py` & `vfsfusepy-0.1.1/vfsfusepy/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         return [".", ".."] + os.listdir(f"{self.repo.working_dir}{path}")
 
     def create(self, path: str, mode: int) -> int:
         file_path = os.path.join(self.repo.working_dir, path.lstrip("/"))
         try:
             fd = os.open(file_path, os.O_WRONLY | os.O_CREAT, mode)
             os.close(fd)
+            if path.lstrip("/").startswith(".git"):
+                return 0
             self.repo.git.add(file_path)
             self.repo.git.commit("-m", f"create file {path}")
             return 0
         except Exception as e:
             logger.error(f"Failed to create file: {file_path}. Error: {str(e)}")
             raise FuseOSError(errno.EACCES) from e
 
@@ -52,37 +54,49 @@
             with open(f"{self.repo.working_dir}{path}", "rb") as f:
                 f.seek(offset)
                 return f.read(size)
         except FileNotFoundError as e:
             raise FuseOSError(errno.ENOENT) from e
 
     def write(self, path: str, data: bytes, offset: int, fh: int) -> int:
+        if path.lstrip("/").startswith(".git"):
+            os.lseek(fh, offset, os.SEEK_SET)
+            return os.write(fh, data)
+
         file_path = os.path.join(self.repo.working_dir, path.lstrip("/"))
         try:
             with open(file_path, "wb") as f:
                 f.seek(offset)
                 f.write(data)
             self.repo.git.add(file_path)
             self.repo.git.commit("-m", f"update file {path}")
             return len(data)
         except Exception as e:
             logger.error(f"Failed to write file: {file_path}. Error: {str(e)}")
             raise FuseOSError(errno.EACCES) from e
 
     def truncate(self, path: str, length: int, fh: Optional[int] = None) -> None:
+        if path.lstrip("/").startswith(".git"):
+            full_path = os.path.join(self.repo.working_dir, path.lstrip("/"))
+            with open(full_path, "r+") as f:
+                f.truncate(length)
+            return
+
         try:
             with open(f"{self.repo.working_dir}{path}", "rb+") as f:
                 f.truncate(length)
         except FileNotFoundError as e:
             raise FuseOSError(errno.ENOENT) from e
 
     def unlink(self, path: str) -> None:
         file_path = os.path.join(self.repo.working_dir, path.lstrip("/"))
         try:
             os.unlink(file_path)
+            if path.lstrip("/").startswith(".git"):
+                return
             self.repo.git.rm(file_path)
             self.repo.git.commit("-m", f"remove file {path}")
         except Exception as e:
             logger.error(f"Failed to remove file: {file_path}. Error: {str(e)}")
             raise FuseOSError(errno.EACCES) from e
```

