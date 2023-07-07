# Comparing `tmp/AshCrypt-1.3.2.tar.gz` & `tmp/AshCrypt-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.3.2.tar", last modified: Fri Jul  7 14:01:41 2023, max compression
+gzip compressed data, was "AshCrypt-1.3.3.tar", last modified: Fri Jul  7 14:06:15 2023, max compression
```

## Comparing `AshCrypt-1.3.2.tar` & `AshCrypt-1.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 14:01:41.654806 AshCrypt-1.3.2/
-drwxrwxrwx   0        0        0        0 2023-07-07 14:01:41.596340 AshCrypt-1.3.2/AshCrypt/
--rw-rw-rw-   0        0        0     4985 2023-07-02 19:28:38.000000 AshCrypt-1.3.2/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0    37325 2023-07-07 14:01:18.000000 AshCrypt-1.3.2/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     6654 2023-07-01 17:13:11.000000 AshCrypt-1.3.2/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0     8450 2023-07-03 21:05:38.000000 AshCrypt-1.3.2/AshCrypt/Database.py
--rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.3.2/AshCrypt/FileCrypt.py
--rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.3.2/AshCrypt/README.md
--rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.3.2/AshCrypt/TextCrypt.py
--rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.3.2/AshCrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:01:41.634363 AshCrypt-1.3.2/AshCrypt/__pycache__/
--rw-rw-rw-   0        0        0     6336 2023-07-03 12:24:42.000000 AshCrypt-1.3.2/AshCrypt/__pycache__/Ash.cpython-39.pyc
--rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.3.2/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
--rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.3.2/AshCrypt/__pycache__/Database.cpython-39.pyc
--rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.3.2/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.3.2/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.3.2/AshCrypt/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      779 2023-07-07 12:45:40.000000 AshCrypt-1.3.2/AshCrypt/__pycache__/qr.cpython-39.pyc
--rw-rw-rw-   0        0        0      536 2023-07-07 12:45:35.000000 AshCrypt-1.3.2/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:01:41.641122 AshCrypt-1.3.2/AshCrypt/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.3.2/AshCrypt/unittests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:01:41.649586 AshCrypt-1.3.2/AshCrypt/unittests/__pycache__/
--rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.3.2/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.3.2/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
--rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.3.2/AshCrypt/unittests/unittestAsh.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:01:41.613264 AshCrypt-1.3.2/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    19466 2023-07-07 14:01:41.000000 AshCrypt-1.3.2/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-07-07 14:01:41.000000 AshCrypt-1.3.2/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 14:01:41.000000 AshCrypt-1.3.2/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-07 14:01:41.000000 AshCrypt-1.3.2/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 14:01:41.000000 AshCrypt-1.3.2/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.3.2/LICENSE
--rw-rw-rw-   0        0        0    19466 2023-07-07 14:01:41.653831 AshCrypt-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    21853 2023-07-02 19:31:35.000000 AshCrypt-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 14:01:41.656157 AshCrypt-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-07-07 14:01:35.000000 AshCrypt-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.587549 AshCrypt-1.3.3/
+drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.523386 AshCrypt-1.3.3/AshCrypt/
+-rw-rw-rw-   0        0        0     4985 2023-07-02 19:28:38.000000 AshCrypt-1.3.3/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    37331 2023-07-07 14:05:56.000000 AshCrypt-1.3.3/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     6654 2023-07-01 17:13:11.000000 AshCrypt-1.3.3/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0     8450 2023-07-03 21:05:38.000000 AshCrypt-1.3.3/AshCrypt/Database.py
+-rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.3.3/AshCrypt/FileCrypt.py
+-rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.3.3/AshCrypt/README.md
+-rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.3.3/AshCrypt/TextCrypt.py
+-rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.3.3/AshCrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.565834 AshCrypt-1.3.3/AshCrypt/__pycache__/
+-rw-rw-rw-   0        0        0     6336 2023-07-03 12:24:42.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/Ash.cpython-39.pyc
+-rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/Database.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      779 2023-07-07 12:45:40.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/qr.cpython-39.pyc
+-rw-rw-rw-   0        0        0      536 2023-07-07 12:45:35.000000 AshCrypt-1.3.3/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.573752 AshCrypt-1.3.3/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.3.3/AshCrypt/unittests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.581571 AshCrypt-1.3.3/AshCrypt/unittests/__pycache__/
+-rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.3.3/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.3.3/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.3.3/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.544791 AshCrypt-1.3.3/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    19466 2023-07-07 14:06:15.000000 AshCrypt-1.3.3/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-07-07 14:06:15.000000 AshCrypt-1.3.3/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:06:15.000000 AshCrypt-1.3.3/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-07 14:06:15.000000 AshCrypt-1.3.3/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 14:06:15.000000 AshCrypt-1.3.3/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0    19466 2023-07-07 14:06:15.585649 AshCrypt-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    21853 2023-07-02 19:31:35.000000 AshCrypt-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 14:06:15.587549 AshCrypt-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-07 14:05:56.000000 AshCrypt-1.3.3/setup.py
```

### Comparing `AshCrypt-1.3.2/AshCrypt/Ash.py` & `AshCrypt-1.3.3/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.3.3/AshCrypt/AshCryptGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,15 +656,15 @@
             filename = filenameStringVar.get().strip()
             key = mainkey
             target = AF.CryptFile(filename, key)
             a = target.encrypt()
             if a == 1:
                 filename = filename + '.crypt'
                 filenameStringVar.set(filename)
-                resultvarfile.set('    Encrypted Successfully / added .crypt')
+                resultvarfile.set('      Encrypted Successfully / added .crypt')
                 if encfiletoolbuttvar.get() == 1:
                     with open(filename,'rb') as f:
                         file_content = f.read()
                     try:
                         main_db_conn.insert(filename,file_content, outputKeyref.get().strip())
                     except:
                         db_display_text.delete('1.0', tk.END)
@@ -707,15 +707,15 @@
             filename =filenameStringVar.get().strip()
             key = mainkey
             target = AF.CryptFile(filename, key)
             a = target.decrypt()
             if a == 1:
                 filename = os.path.splitext(filename)[0]
                 filenameStringVar.set(filename)
-                resultvarfile.set('   Decrypted Successfully + removed .crypt')
+                resultvarfile.set('     Decrypted Successfully + removed .crypt')
                 if decfiletoolbuttvar.get() == 1:
                     with open(filename,'rb') as f:
                         file_content = f.read()
                     try:
                         main_db_conn.insert(filename,file_content, outputKeyref.get().strip())
                     except:
                         db_display_text.delete('1.0', tk.END)
@@ -753,14 +753,15 @@
 
 
 
 
 
 
 
+
 encryptionfilebutton = tk.Button(master=frameFile1 ,text='ENCRYPT FILE', command=encFile, bootstyle='warning outline').place(relx=0.25, rely=0.73)
 decryptionfilebutton = tk.Button(master=frameFile1 , text='DECRYPT FILE', command=decfile,bootstyle='warning outline').place(relx=0.55,rely=0.73)
 
 filenameStringVar = tk.StringVar(value='')
 
 filenametext = tk.Entry(master=frameFile1 ,
                         width=31,
```

### Comparing `AshCrypt-1.3.2/AshCrypt/CliCrypt.py` & `AshCrypt-1.3.3/AshCrypt/CliCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/Database.py` & `AshCrypt-1.3.3/AshCrypt/Database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/FileCrypt.py` & `AshCrypt-1.3.3/AshCrypt/FileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/README.md` & `AshCrypt-1.3.3/AshCrypt/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/TextCrypt.py` & `AshCrypt-1.3.3/AshCrypt/TextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/__pycache__/Ash.cpython-39.pyc` & `AshCrypt-1.3.3/AshCrypt/__pycache__/Ash.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc` & `AshCrypt-1.3.3/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/__pycache__/Database.cpython-39.pyc` & `AshCrypt-1.3.3/AshCrypt/__pycache__/Database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc` & `AshCrypt-1.3.3/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc` & `AshCrypt-1.3.3/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/__pycache__/qr.cpython-39.pyc` & `AshCrypt-1.3.3/AshCrypt/__pycache__/qr.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/qr.py` & `AshCrypt-1.3.3/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc` & `AshCrypt-1.3.3/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt/unittests/unittestAsh.py` & `AshCrypt-1.3.3/AshCrypt/unittests/unittestAsh.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.3.3/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.3.2
+Version: 1.3.3
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.3.2/AshCrypt.egg-info/SOURCES.txt` & `AshCrypt-1.3.3/AshCrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/LICENSE` & `AshCrypt-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/PKG-INFO` & `AshCrypt-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.3.2
+Version: 1.3.3
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.3.2/README.md` & `AshCrypt-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.2/setup.py` & `AshCrypt-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.3.2',
+    version='1.3.3',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

