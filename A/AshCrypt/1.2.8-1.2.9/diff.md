# Comparing `tmp/AshCrypt-1.2.8.tar.gz` & `tmp/AshCrypt-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.2.8.tar", last modified: Fri Jul  7 13:43:14 2023, max compression
+gzip compressed data, was "AshCrypt-1.2.9.tar", last modified: Fri Jul  7 13:53:11 2023, max compression
```

## Comparing `AshCrypt-1.2.8.tar` & `AshCrypt-1.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:43:14.743599 AshCrypt-1.2.8/
-drwxrwxrwx   0        0        0        0 2023-07-07 13:43:14.681606 AshCrypt-1.2.8/AshCrypt/
--rw-rw-rw-   0        0        0     4985 2023-07-02 19:28:38.000000 AshCrypt-1.2.8/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0    35332 2023-07-07 13:42:21.000000 AshCrypt-1.2.8/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     6654 2023-07-01 17:13:11.000000 AshCrypt-1.2.8/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0     8450 2023-07-03 21:05:38.000000 AshCrypt-1.2.8/AshCrypt/Database.py
--rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.2.8/AshCrypt/FileCrypt.py
--rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.2.8/AshCrypt/README.md
--rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.2.8/AshCrypt/TextCrypt.py
--rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.2.8/AshCrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:43:14.718168 AshCrypt-1.2.8/AshCrypt/__pycache__/
--rw-rw-rw-   0        0        0     6336 2023-07-03 12:24:42.000000 AshCrypt-1.2.8/AshCrypt/__pycache__/Ash.cpython-39.pyc
--rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.2.8/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
--rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.2.8/AshCrypt/__pycache__/Database.cpython-39.pyc
--rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.2.8/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.2.8/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.2.8/AshCrypt/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      779 2023-07-07 12:45:40.000000 AshCrypt-1.2.8/AshCrypt/__pycache__/qr.cpython-39.pyc
--rw-rw-rw-   0        0        0      536 2023-07-07 12:45:35.000000 AshCrypt-1.2.8/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:43:14.726547 AshCrypt-1.2.8/AshCrypt/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.2.8/AshCrypt/unittests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:43:14.737155 AshCrypt-1.2.8/AshCrypt/unittests/__pycache__/
--rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.2.8/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.2.8/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
--rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.2.8/AshCrypt/unittests/unittestAsh.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:43:14.699081 AshCrypt-1.2.8/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    19466 2023-07-07 13:43:14.000000 AshCrypt-1.2.8/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-07-07 13:43:14.000000 AshCrypt-1.2.8/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:43:14.000000 AshCrypt-1.2.8/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-07 13:43:14.000000 AshCrypt-1.2.8/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 13:43:14.000000 AshCrypt-1.2.8/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.2.8/LICENSE
--rw-rw-rw-   0        0        0    19466 2023-07-07 13:43:14.741549 AshCrypt-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    21853 2023-07-02 19:31:35.000000 AshCrypt-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 13:43:14.744574 AshCrypt-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-07-07 13:35:14.000000 AshCrypt-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:53:11.503172 AshCrypt-1.2.9/
+drwxrwxrwx   0        0        0        0 2023-07-07 13:53:11.446828 AshCrypt-1.2.9/AshCrypt/
+-rw-rw-rw-   0        0        0     4985 2023-07-02 19:28:38.000000 AshCrypt-1.2.9/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    35550 2023-07-07 13:47:49.000000 AshCrypt-1.2.9/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     6654 2023-07-01 17:13:11.000000 AshCrypt-1.2.9/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0     8450 2023-07-03 21:05:38.000000 AshCrypt-1.2.9/AshCrypt/Database.py
+-rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.2.9/AshCrypt/FileCrypt.py
+-rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.2.9/AshCrypt/README.md
+-rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.2.9/AshCrypt/TextCrypt.py
+-rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.2.9/AshCrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:53:11.482877 AshCrypt-1.2.9/AshCrypt/__pycache__/
+-rw-rw-rw-   0        0        0     6336 2023-07-03 12:24:42.000000 AshCrypt-1.2.9/AshCrypt/__pycache__/Ash.cpython-39.pyc
+-rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.2.9/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.2.9/AshCrypt/__pycache__/Database.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.2.9/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.2.9/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.2.9/AshCrypt/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      779 2023-07-07 12:45:40.000000 AshCrypt-1.2.9/AshCrypt/__pycache__/qr.cpython-39.pyc
+-rw-rw-rw-   0        0        0      536 2023-07-07 12:45:35.000000 AshCrypt-1.2.9/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:53:11.490668 AshCrypt-1.2.9/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.2.9/AshCrypt/unittests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:53:11.499006 AshCrypt-1.2.9/AshCrypt/unittests/__pycache__/
+-rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.2.9/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.2.9/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.2.9/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:53:11.462873 AshCrypt-1.2.9/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    19466 2023-07-07 13:53:10.000000 AshCrypt-1.2.9/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-07-07 13:53:10.000000 AshCrypt-1.2.9/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:53:10.000000 AshCrypt-1.2.9/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-07 13:53:10.000000 AshCrypt-1.2.9/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 13:53:10.000000 AshCrypt-1.2.9/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0    19466 2023-07-07 13:53:11.502128 AshCrypt-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    21853 2023-07-02 19:31:35.000000 AshCrypt-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:53:11.503172 AshCrypt-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-07 13:52:53.000000 AshCrypt-1.2.9/setup.py
```

### Comparing `AshCrypt-1.2.8/AshCrypt/Ash.py` & `AshCrypt-1.2.9/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.2.9/AshCrypt/AshCryptGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -631,21 +631,25 @@
 
 filepathlabel = tk.Label(master=frameFile1 ,
                       text='FILE PATH',
                       font='Calibre 20 bold' ,
                       )
 filepathlabel.place(relx=0.335,rely=0.10)
 
-
-resultvarfile = tk.StringVar(value='                  ..........')
-resultLabelfile =  tk.Label(master= frameFile1,
-                         textvariable=resultvarfile,
-                         font='terminal 13 bold').place(
-                                                       rely= 0.55 ,
-                                                       )
+import platform
+if platform.system() == 'Windows':
+    resultvarfile = tk.StringVar(value='                  ..........')
+    resultLabelfile =  tk.Label(master= frameFile1,
+                             textvariable=resultvarfile,
+                             font='terminal 13 bold').place(rely= 0.55)
+else:
+    resultvarfile = tk.StringVar(value='                     ..........')
+    resultLabelfile = tk.Label(master=frameFile1,
+                               textvariable=resultvarfile,
+                               font='terminal 13 bold').place(rely=0.55)
 
 
 def encFile():
     global fileaccessSemo ,add_enc_to_db ,main_db_conn,mainkey
     if 1 :
         if keySelectionFlag.get() != 0:
             filename = filenameStringVar.get().strip()
```

### Comparing `AshCrypt-1.2.8/AshCrypt/CliCrypt.py` & `AshCrypt-1.2.9/AshCrypt/CliCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/Database.py` & `AshCrypt-1.2.9/AshCrypt/Database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/FileCrypt.py` & `AshCrypt-1.2.9/AshCrypt/FileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/README.md` & `AshCrypt-1.2.9/AshCrypt/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/TextCrypt.py` & `AshCrypt-1.2.9/AshCrypt/TextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/__pycache__/Ash.cpython-39.pyc` & `AshCrypt-1.2.9/AshCrypt/__pycache__/Ash.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc` & `AshCrypt-1.2.9/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/__pycache__/Database.cpython-39.pyc` & `AshCrypt-1.2.9/AshCrypt/__pycache__/Database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc` & `AshCrypt-1.2.9/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc` & `AshCrypt-1.2.9/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/__pycache__/qr.cpython-39.pyc` & `AshCrypt-1.2.9/AshCrypt/__pycache__/qr.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/qr.py` & `AshCrypt-1.2.9/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc` & `AshCrypt-1.2.9/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt/unittests/unittestAsh.py` & `AshCrypt-1.2.9/AshCrypt/unittests/unittestAsh.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.2.9/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.2.8
+Version: 1.2.9
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.2.8/AshCrypt.egg-info/SOURCES.txt` & `AshCrypt-1.2.9/AshCrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/LICENSE` & `AshCrypt-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/PKG-INFO` & `AshCrypt-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.2.8
+Version: 1.2.9
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.2.8/README.md` & `AshCrypt-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.8/setup.py` & `AshCrypt-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.2.8',
+    version='1.2.9',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

