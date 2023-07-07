# Comparing `tmp/AshCrypt-1.2.4.tar.gz` & `tmp/AshCrypt-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.2.4.tar", last modified: Wed Jul  5 14:20:46 2023, max compression
+gzip compressed data, was "AshCrypt-1.2.6.tar", last modified: Fri Jul  7 13:15:31 2023, max compression
```

## Comparing `AshCrypt-1.2.4.tar` & `AshCrypt-1.2.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.150701 AshCrypt-1.2.4/
-drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.083189 AshCrypt-1.2.4/AshCrypt/
--rw-rw-rw-   0        0        0     4985 2023-07-02 19:28:38.000000 AshCrypt-1.2.4/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0    35061 2023-07-05 14:19:33.000000 AshCrypt-1.2.4/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     6654 2023-07-01 17:13:11.000000 AshCrypt-1.2.4/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0     8450 2023-07-03 21:05:38.000000 AshCrypt-1.2.4/AshCrypt/Database.py
--rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.2.4/AshCrypt/FileCrypt.py
--rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.2.4/AshCrypt/README.md
--rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.2.4/AshCrypt/TextCrypt.py
--rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.2.4/AshCrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.124449 AshCrypt-1.2.4/AshCrypt/__pycache__/
--rw-rw-rw-   0        0        0     6336 2023-07-03 12:24:42.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/Ash.cpython-39.pyc
--rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
--rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/Database.cpython-39.pyc
--rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1263 2023-07-01 02:23:01.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/qr.cpython-39.pyc
--rw-rw-rw-   0        0        0     1045 2023-06-30 15:01:03.000000 AshCrypt-1.2.4/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.135519 AshCrypt-1.2.4/AshCrypt/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.2.4/AshCrypt/unittests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.144769 AshCrypt-1.2.4/AshCrypt/unittests/__pycache__/
--rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.2.4/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.2.4/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
--rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.2.4/AshCrypt/unittests/unittestAsh.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.099172 AshCrypt-1.2.4/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    19466 2023-07-05 14:20:45.000000 AshCrypt-1.2.4/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-07-05 14:20:45.000000 AshCrypt-1.2.4/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 14:20:45.000000 AshCrypt-1.2.4/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-05 14:20:45.000000 AshCrypt-1.2.4/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-05 14:20:45.000000 AshCrypt-1.2.4/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.2.4/LICENSE
--rw-rw-rw-   0        0        0    19466 2023-07-05 14:20:46.148800 AshCrypt-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    21853 2023-07-02 19:31:35.000000 AshCrypt-1.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-05 14:20:46.150701 AshCrypt-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-07-02 21:38:12.000000 AshCrypt-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:15:31.013840 AshCrypt-1.2.6/
+drwxrwxrwx   0        0        0        0 2023-07-07 13:15:30.940812 AshCrypt-1.2.6/AshCrypt/
+-rw-rw-rw-   0        0        0     4985 2023-07-02 19:28:38.000000 AshCrypt-1.2.6/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    35051 2023-07-07 13:12:01.000000 AshCrypt-1.2.6/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     6654 2023-07-01 17:13:11.000000 AshCrypt-1.2.6/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0     8450 2023-07-03 21:05:38.000000 AshCrypt-1.2.6/AshCrypt/Database.py
+-rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.2.6/AshCrypt/FileCrypt.py
+-rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.2.6/AshCrypt/README.md
+-rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.2.6/AshCrypt/TextCrypt.py
+-rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.2.6/AshCrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:15:30.988718 AshCrypt-1.2.6/AshCrypt/__pycache__/
+-rw-rw-rw-   0        0        0     6336 2023-07-03 12:24:42.000000 AshCrypt-1.2.6/AshCrypt/__pycache__/Ash.cpython-39.pyc
+-rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.2.6/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.2.6/AshCrypt/__pycache__/Database.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.2.6/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.2.6/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.2.6/AshCrypt/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      779 2023-07-07 12:45:40.000000 AshCrypt-1.2.6/AshCrypt/__pycache__/qr.cpython-39.pyc
+-rw-rw-rw-   0        0        0      536 2023-07-07 12:45:35.000000 AshCrypt-1.2.6/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:15:30.999895 AshCrypt-1.2.6/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.2.6/AshCrypt/unittests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:15:31.008376 AshCrypt-1.2.6/AshCrypt/unittests/__pycache__/
+-rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.2.6/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.2.6/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.2.6/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:15:30.960456 AshCrypt-1.2.6/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    19466 2023-07-07 13:15:30.000000 AshCrypt-1.2.6/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-07-07 13:15:30.000000 AshCrypt-1.2.6/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:15:30.000000 AshCrypt-1.2.6/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-07 13:15:30.000000 AshCrypt-1.2.6/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 13:15:30.000000 AshCrypt-1.2.6/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0    19466 2023-07-07 13:15:31.012349 AshCrypt-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    21853 2023-07-02 19:31:35.000000 AshCrypt-1.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:15:31.013840 AshCrypt-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-07 13:14:48.000000 AshCrypt-1.2.6/setup.py
```

### Comparing `AshCrypt-1.2.4/AshCrypt/Ash.py` & `AshCrypt-1.2.6/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.2.6/AshCrypt/AshCryptGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,21 +39,22 @@
 
 '''--------------------------------------DATABASE FRAME STARTED------------------------------------------------'''
 
 
 databaseFrame = tk.Frame(master=object,height=800, width=500)
 databaseFrame.place(rely=0, relx=0)
 
-console_label = tk.Label(master=databaseFrame, text='DATABASE OUTPUT CONSOLE', font='Terminal 15 bold')
+console_label = tk.Label(master=databaseFrame, text='DATABASE OUTPUT CONSOLE', font='terminal 15 bold')
 console_label.place( relx=0.09,rely=0.04)
 
 
-db_display_text = tk.ScrolledText(width=36 , height=30, font='Terminal 10',wrap='word')
-db_display_text.insert(tk.END,'Waiting to fetch..')
+db_display_text = tk.Text(width=38 , height=19, font='arial 13',wrap='word')
 db_display_text.place(relx=0.015 ,rely=0.105)
+db_display_text.insert(tk.END,'Waiting to fetch..')
+
 
 def show_all_content():
     global db_enable_blocker, main_db_name_var, usable_real_path, main_db_conn,db_display_text,keys_db_conn
     if db_enable_blocker != 0:
         db_display_text.delete('1.0', tk.END)
         db_display_text.insert(tk.END, f"Check 'output.json' in the chosen path : {usable_real_path}\n")
         json_path = os.path.join(usable_real_path, 'output.json')
@@ -831,17 +832,17 @@
 
 def genMainKey():
     keyGenVar.set(AF.CryptFile.genkey())
 
 
 keyGenVar = tk.StringVar(value='')
 keyGenEntry = tk.Entry(master=frameFile2 ,
-                        font='arial 15 ',
+                        font='arial 12',
                         textvariable=keyGenVar,
-                        width=18).place(relx=0.1 ,rely=0.69)
+                        width=23).place(relx=0.1 ,rely=0.69)
 
 keyButton = tk.Button(master=frameFile2 ,
                       text='GENERATE',
                       command=genMainKey,
                       bootstyle='success outline').place(relx=0.671, rely=0.7)
```

### Comparing `AshCrypt-1.2.4/AshCrypt/CliCrypt.py` & `AshCrypt-1.2.6/AshCrypt/CliCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/Database.py` & `AshCrypt-1.2.6/AshCrypt/Database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/FileCrypt.py` & `AshCrypt-1.2.6/AshCrypt/FileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/README.md` & `AshCrypt-1.2.6/AshCrypt/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/TextCrypt.py` & `AshCrypt-1.2.6/AshCrypt/TextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/__pycache__/Ash.cpython-39.pyc` & `AshCrypt-1.2.6/AshCrypt/__pycache__/Ash.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc` & `AshCrypt-1.2.6/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/__pycache__/Database.cpython-39.pyc` & `AshCrypt-1.2.6/AshCrypt/__pycache__/Database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc` & `AshCrypt-1.2.6/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc` & `AshCrypt-1.2.6/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc` & `AshCrypt-1.2.6/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt/unittests/unittestAsh.py` & `AshCrypt-1.2.6/AshCrypt/unittests/unittestAsh.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.2.6/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.2.4
+Version: 1.2.6
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.2.4/AshCrypt.egg-info/SOURCES.txt` & `AshCrypt-1.2.6/AshCrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/LICENSE` & `AshCrypt-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/PKG-INFO` & `AshCrypt-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.2.4
+Version: 1.2.6
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.2.4/README.md` & `AshCrypt-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.4/setup.py` & `AshCrypt-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.2.4',
+    version='1.2.6',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

