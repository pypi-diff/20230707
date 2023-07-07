# Comparing `tmp/kikyo-sz-0.1.4.tar.gz` & `tmp/kikyo-sz-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kikyo-sz-0.1.4.tar", last modified: Mon Jul  3 03:17:37 2023, max compression
+gzip compressed data, was "kikyo-sz-0.2.tar", last modified: Fri Jul  7 08:07:17 2023, max compression
```

## Comparing `kikyo-sz-0.1.4.tar` & `kikyo-sz-0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/
--rw-r--r--   0 jadbin     (501) staff       (20)     1063 2021-03-30 06:22:21.000000 kikyo-sz-0.1.4/LICENSE
--rw-r--r--   0 jadbin     (501) staff       (20)      141 2023-03-14 08:19:45.000000 kikyo-sz-0.1.4/MANIFEST.in
--rw-r--r--   0 jadbin     (501) staff       (20)      484 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)       36 2023-03-14 08:10:35.000000 kikyo-sz-0.1.4/README.rst
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz/
--rw-r--r--   0 jadbin     (501) staff       (20)       22 2023-07-03 03:17:12.000000 kikyo-sz-0.1.4/kikyo_sz/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      132 2023-03-16 01:40:07.000000 kikyo-sz-0.1.4/kikyo_sz/config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2288 2023-07-03 03:15:05.000000 kikyo-sz-0.1.4/kikyo_sz/oss.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/
--rw-r--r--   0 jadbin     (501) staff       (20)      484 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)      386 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/SOURCES.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/dependency_links.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       43 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/entry_points.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2023-03-14 08:18:27.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/not-zip-safe
--rw-r--r--   0 jadbin     (501) staff       (20)       45 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/requires.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        9 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/top_level.txt
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/requirements/
--rw-r--r--   0 jadbin     (501) staff       (20)       18 2021-03-30 06:22:21.000000 kikyo-sz-0.1.4/requirements/test.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/setup.cfg
--rw-r--r--   0 jadbin     (501) staff       (20)     1948 2023-03-16 08:38:31.000000 kikyo-sz-0.1.4/setup.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/tests/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-03-30 06:22:21.000000 kikyo-sz-0.1.4/tests/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      538 2023-03-16 01:32:54.000000 kikyo-sz-0.1.4/tests/test_filesys_oss.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-07 08:07:17.828357 kikyo-sz-0.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1063 2023-07-07 08:06:22.000000 kikyo-sz-0.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      141 2023-07-07 08:06:22.000000 kikyo-sz-0.2/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      521 2023-07-07 08:07:17.823046 kikyo-sz-0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-07-07 08:06:22.000000 kikyo-sz-0.2/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-07 08:07:17.033040 kikyo-sz-0.2/kikyo_sz/
+-rwxrwxrwx   0 root         (0) root         (0)       20 2023-07-07 08:07:06.000000 kikyo-sz-0.2/kikyo_sz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      132 2023-07-07 08:06:22.000000 kikyo-sz-0.2/kikyo_sz/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     2288 2023-07-07 08:06:22.000000 kikyo-sz-0.2/kikyo_sz/oss.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-07 08:07:17.393851 kikyo-sz-0.2/kikyo_sz.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      521 2023-07-07 08:07:16.000000 kikyo-sz-0.2/kikyo_sz.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      386 2023-07-07 08:07:16.000000 kikyo-sz-0.2/kikyo_sz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-07 08:07:16.000000 kikyo-sz-0.2/kikyo_sz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       44 2023-07-07 08:07:16.000000 kikyo-sz-0.2/kikyo_sz.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-07 08:07:16.000000 kikyo-sz-0.2/kikyo_sz.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-07-07 08:07:16.000000 kikyo-sz-0.2/kikyo_sz.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-07-07 08:07:16.000000 kikyo-sz-0.2/kikyo_sz.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-07 08:07:17.492849 kikyo-sz-0.2/requirements/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-07-07 08:06:22.000000 kikyo-sz-0.2/requirements/test.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-07 08:07:17.829360 kikyo-sz-0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1948 2023-07-07 08:06:55.000000 kikyo-sz-0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-07 08:07:17.721360 kikyo-sz-0.2/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-07 08:06:22.000000 kikyo-sz-0.2/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      538 2023-07-07 08:06:22.000000 kikyo-sz-0.2/tests/test_filesys_oss.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kikyo-sz-0.1.4/LICENSE` & `kikyo-sz-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kikyo-sz-0.1.4/kikyo_sz/oss.py` & `kikyo-sz-0.2/kikyo_sz/oss.py`

 * *Files identical despite different names*

### Comparing `kikyo-sz-0.1.4/setup.py` & `kikyo-sz-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         errno = pytest.main(['tests'])
         sys.exit(errno)
 
 
 tests_require = read_requirements('test.txt')
 install_requires = [
-    'kikyo>=0.12.3,<0.13',
+    'kikyo>=0.13.6,<0.14',
     'requests-toolbelt>=0.9.1',
 ]
 
 
 def main():
     if sys.version_info < (3, 6):
         raise RuntimeError('The minimal supported Python version is 3.6')
```

### Comparing `kikyo-sz-0.1.4/tests/test_filesys_oss.py` & `kikyo-sz-0.2/tests/test_filesys_oss.py`

 * *Files identical despite different names*

