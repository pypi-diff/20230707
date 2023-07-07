# Comparing `tmp/pantherdb-1.2.3.tar.gz` & `tmp/pantherdb-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pantherdb-1.2.3.tar", last modified: Fri Jun 30 09:28:09 2023, max compression
+gzip compressed data, was "pantherdb-1.2.4.tar", last modified: Fri Jul  7 08:59:55 2023, max compression
```

## Comparing `pantherdb-1.2.3.tar` & `pantherdb-1.2.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:28:09.869982 pantherdb-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-30 09:28:09.869982 pantherdb-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-30 09:27:54.000000 pantherdb-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:28:09.865982 pantherdb-1.2.3/pantherdb/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 09:27:54.000000 pantherdb-1.2.3/pantherdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-30 09:27:54.000000 pantherdb-1.2.3/pantherdb/pantherdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:28:09.869982 pantherdb-1.2.3/pantherdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-30 09:28:09.000000 pantherdb-1.2.3/pantherdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-30 09:28:09.000000 pantherdb-1.2.3/pantherdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:28:09.000000 pantherdb-1.2.3/pantherdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 09:28:09.000000 pantherdb-1.2.3/pantherdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 09:28:09.000000 pantherdb-1.2.3/pantherdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:28:09.869982 pantherdb-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-30 09:27:54.000000 pantherdb-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:59:55.904312 pantherdb-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-07 08:59:55.904312 pantherdb-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-07 08:59:42.000000 pantherdb-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:59:55.904312 pantherdb-1.2.4/pantherdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 08:59:42.000000 pantherdb-1.2.4/pantherdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-07-07 08:59:42.000000 pantherdb-1.2.4/pantherdb/pantherdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:59:55.904312 pantherdb-1.2.4/pantherdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-07 08:59:55.000000 pantherdb-1.2.4/pantherdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-07 08:59:55.000000 pantherdb-1.2.4/pantherdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:59:55.000000 pantherdb-1.2.4/pantherdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 08:59:55.000000 pantherdb-1.2.4/pantherdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 08:59:55.000000 pantherdb-1.2.4/pantherdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:59:55.904312 pantherdb-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-07 08:59:42.000000 pantherdb-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:59:55.904312 pantherdb-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-07-07 08:59:42.000000 pantherdb-1.2.4/tests/test_normal.py
```

### Comparing `pantherdb-1.2.3/PKG-INFO` & `pantherdb-1.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pantherdb
-Version: 1.2.3
+Version: 1.2.4
 Summary: is a Simple, FileBase and Document Oriented database
 Home-page: https://github.com/alirn76/pantherdb
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ## Introduction
 
 PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
 
 ### Features:
```

### Comparing `pantherdb-1.2.3/README.md` & `pantherdb-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pantherdb-1.2.3/pantherdb/pantherdb.py` & `pantherdb-1.2.4/pantherdb/pantherdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,19 @@
     __return_dict: bool
     __content: dict
 
     def __init__(self, db_name: str | None = None, return_dict: bool = False, secret_key: bytes | None = None):
         self.__return_dict = return_dict
         self.__secret_key = secret_key
         self.__fernet = Fernet(self.__secret_key) if self.__secret_key else None
+        self.__content = {}
+
         if db_name:
+            if not db_name.endswith('pdb'):
+                db_name = f'{db_name}.pdb'
             self.db_name = db_name
         if not os.path.exists(self.db_name):
             open(self.db_name, 'w').close()
 
     def __str__(self) -> str:
         self._refresh()
         db = ',\n'.join(f'    {k}: {len(v)} documents' for k, v in self.content.items())
@@ -36,15 +40,15 @@
         return self.__content
 
     @property
     def return_dict(self) -> bool:
         return self.__return_dict
 
     @property
-    def secret_key(self) -> bytes:
+    def secret_key(self) -> bytes | None:
         return self.__secret_key
 
     def _write(self) -> None:
         content = json.dumps(self.content)
 
         if self.secret_key:
             content = self.__fernet.encrypt(content)
@@ -87,19 +91,22 @@
 
     def __init__(self, db_name: str, collection_name: str, return_dict: bool, secret_key: bytes):
         super().__init__(db_name=db_name, return_dict=return_dict, secret_key=secret_key)
         self.__collection_name = collection_name
 
     def __str__(self) -> str:
         self._refresh()
-        documents = self.content[self.collection_name]
-        if not documents:
-            return f'{self.__class__.__name__}(\n    collection_name: {self.collection_name}\n)'
 
-        result = '\n'.join(f'    {k}: {type(v).__name__}' for k, v in documents[0].items())
+        if self.collection_name not in self.content:
+            result = ''
+        elif documents := self.content[self.collection_name]:
+            result = ''
+        else:
+            result = '\n'.join(f'    {k}: {type(v).__name__}' for k, v in documents[0].items())
+
         return f'{self.__class__.__name__}(\n    collection_name: {self.collection_name}\n\n{result}\n)'
 
     @property
     def collection_name(self) -> str:
         return self.__collection_name
 
     def __check_is_panther_document(self) -> None:
@@ -120,15 +127,16 @@
 
     def _write_collection(self, documents: list) -> None:
         self.content[self.collection_name] = documents
         self._write()
 
     def _drop_collection(self) -> None:
         self._refresh()
-        del self.content[self.collection_name]
+        if self.collection_name in self.content:
+            del self.content[self.collection_name]
         self._write()
 
     def _get_collection(self) -> list[dict]:
         """return documents"""
         self._refresh()
         return self.content.get(self.collection_name, [])
 
@@ -237,14 +245,15 @@
     def update(self, **kwargs) -> None:
         self.__check_is_panther_document()
         documents = self._get_collection()
         for d in documents:
             if d.get('_id') == self._id:  # NOQA: Unresolved References
                 for k, v in kwargs.items():
                     d[k] = v
+                    setattr(self, k, v)
                 self._write_collection(documents)
 
     def update_one(self, condition: dict, **kwargs) -> bool:
         documents = self._get_collection()
         result = False
 
         if not condition:
@@ -325,14 +334,15 @@
             error = f'Invalid Collection Field: "{item}"'
             raise PantherDBException(error)
 
     def __setattr__(self, key, value):
         if key not in [
             '_PantherDB__return_dict',
             '_PantherDB__secret_key',
+            '_PantherDB__content',
             '_PantherDB__fernet',
             '_PantherCollection__collection_name',
             '_PantherDocument__data'
         ]:
             try:
                 object.__getattribute__(self, key)
             except AttributeError:
@@ -352,11 +362,12 @@
     def save(self) -> None:
         """Pop & Insert New Document"""
         documents = self._get_collection()
         for i, d in enumerate(documents):
             if d['_id'] == self.id:
                 documents.pop(i)
                 documents.insert(i, self.data)
-        super()._write_collection(documents=documents)
+                break
+        self._write_collection(documents)
 
     def json(self) -> str:
         return json.dumps(self.data).decode()
```

### Comparing `pantherdb-1.2.3/pantherdb.egg-info/PKG-INFO` & `pantherdb-1.2.4/pantherdb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pantherdb
-Version: 1.2.3
+Version: 1.2.4
 Summary: is a Simple, FileBase and Document Oriented database
 Home-page: https://github.com/alirn76/pantherdb
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ## Introduction
 
 PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
 
 ### Features:
```

### Comparing `pantherdb-1.2.3/setup.py` & `pantherdb-1.2.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 
 VERSION = pantherdb_version()
 DESCRIPTION = open('README.md').read()
 
 setup(
     name='pantherdb',
     version=VERSION,
-    python_requires='>=3.11',
+    python_requires='>=3.10',
     author='Ali RajabNezhad',
     author_email='alirn76@yahoo.com',
     url='https://github.com/alirn76/pantherdb',
     description='is a Simple, FileBase and Document Oriented database',
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     include_package_data=True,
     license='MIT',
     classifiers=[
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     install_requires=[
-        'orjson>=3.8.6',
-        'cryptography>=39.0.2',
+        'orjson~=3.8',
+        'cryptography~=39.0',
     ],
 )
```

