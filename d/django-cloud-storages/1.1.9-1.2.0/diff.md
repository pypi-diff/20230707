# Comparing `tmp/django_cloud_storages-1.1.9.tar.gz` & `tmp/django_cloud_storages-1.2.0.tar.gz`

## Comparing `django_cloud_storages-1.1.9.tar` & `django_cloud_storages-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/.readthedocs.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/cloud_storages/__init__.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/cloud_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/cloud_storages/backends/__init__.py
--rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/cloud_storages/backends/appwrite.py
--rw-r--r--   0        0        0    10516 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/cloud_storages/backends/dropbox.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/LICENSE
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/README.md
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/cloud_storages/__init__.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/cloud_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/cloud_storages/backends/__init__.py
+-rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/cloud_storages/backends/appwrite.py
+-rw-r--r--   0        0        0    10543 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/cloud_storages/backends/dropbox.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/README.md
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.0/PKG-INFO
```

### Comparing `django_cloud_storages-1.1.9/.readthedocs.yaml` & `django_cloud_storages-1.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.9/cloud_storages/utils.py` & `django_cloud_storages-1.2.0/cloud_storages/utils.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.9/cloud_storages/backends/appwrite.py` & `django_cloud_storages-1.2.0/cloud_storages/backends/appwrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,16 @@
             self._save(path[0], content)
         return path[0]
     def _save(self, path, content):
         folder, filename = self.extract_folder_and_filename(path)
         content.open()
         the_file = InputFile.from_bytes(bytes=content.read(), filename=content.name)
         result = self.storage.create_file(bucket_id=folder, file_id=filename, file=the_file)
-        content.close()
+        content.seek(0)
+        # content.close()
         return path
     
     def _id_validation(self, name):
         name = re.sub(r"^\W+|^_+", "", name) # Remove special characters at beginning
         name = re.sub(r"[^a-zA-Z0-9-._]*", "", name)
         return name
```

### Comparing `django_cloud_storages-1.1.9/cloud_storages/backends/dropbox.py` & `django_cloud_storages-1.2.0/cloud_storages/backends/dropbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,16 @@
     def _save(self, name, content):
         full_name = self._full_path(name)
         content.open()
         if content.size <= self.CHUNK_SIZE:
             self.dbx.files_upload(content.read(), full_name, mode=WriteMode(self.write_mode))
         else:
             self._chunked_upload(content, full_name)
-        content.close()
+        content.seek(0)
+        # content.close()
         return name
 
     def get_available_name(self, name, content, max_length=None):
         """
         Return a filename that's free on the target storage system and
         available for new content to be written to.
         """
```

### Comparing `django_cloud_storages-1.1.9/.gitignore` & `django_cloud_storages-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.9/LICENSE` & `django_cloud_storages-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.9/README.md` & `django_cloud_storages-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.9/pyproject.toml` & `django_cloud_storages-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.9/PKG-INFO` & `django_cloud_storages-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloud-storages
-Version: 1.1.9
+Version: 1.2.0
 Summary: Cloud file storages for django.
 Project-URL: Homepage, https://pypi.org/project/django-cloud-storages
 Project-URL: Source code, https://github.com/Samiddha99/django-cloud-storages
 Project-URL: Documentation, https://django-cloud-storages.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/Samiddha99/django-cloud-storages/issues
 Author-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
 Maintainer-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
```

