# Comparing `tmp/findmyfile-0.3.0.tar.gz` & `tmp/findmyfile-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyfile-0.3.0.tar", last modified: Sun Jun 25 02:19:32 2023, max compression
+gzip compressed data, was "findmyfile-0.3.1.tar", last modified: Thu Jul  6 23:02:12 2023, max compression
```

## Comparing `findmyfile-0.3.0.tar` & `findmyfile-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 02:19:32.556000 findmyfile-0.3.0/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1061 2023-06-24 01:20:32.000000 findmyfile-0.3.0/LICENCE.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      687 2023-06-25 02:19:32.536000 findmyfile-0.3.0/PKG-INFO
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     4316 2023-06-25 02:18:06.000000 findmyfile-0.3.0/README.md
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 02:19:31.915000 findmyfile-0.3.0/findmyfile/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 10:58:56.000000 findmyfile-0.3.0/findmyfile/__init__.py
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       64 2023-06-24 10:59:26.000000 findmyfile-0.3.0/findmyfile/__main__.py
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     9362 2023-06-25 02:06:09.000000 findmyfile-0.3.0/findmyfile/main.py
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 02:19:32.464000 findmyfile-0.3.0/findmyfile.egg-info/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      687 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/PKG-INFO
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      301 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/SOURCES.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        1 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/dependency_links.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       45 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/entry_points.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       53 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/requires.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       11 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/top_level.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       38 2023-06-25 02:19:32.553000 findmyfile-0.3.0/setup.cfg
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1714 2023-06-25 02:07:41.000000 findmyfile-0.3.0/setup.py
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-07-06 23:02:12.760000 findmyfile-0.3.1/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1061 2023-06-24 01:20:32.000000 findmyfile-0.3.1/LICENCE.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      687 2023-07-06 23:02:12.739000 findmyfile-0.3.1/PKG-INFO
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     4316 2023-06-25 02:18:06.000000 findmyfile-0.3.1/README.md
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-07-06 23:02:12.187000 findmyfile-0.3.1/findmyfile/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 10:58:56.000000 findmyfile-0.3.1/findmyfile/__init__.py
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       64 2023-06-24 10:59:26.000000 findmyfile-0.3.1/findmyfile/__main__.py
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)    10100 2023-07-06 23:02:08.000000 findmyfile-0.3.1/findmyfile/main.py
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-07-06 23:02:12.685000 findmyfile-0.3.1/findmyfile.egg-info/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      687 2023-07-06 23:02:11.000000 findmyfile-0.3.1/findmyfile.egg-info/PKG-INFO
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      301 2023-07-06 23:02:11.000000 findmyfile-0.3.1/findmyfile.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        1 2023-07-06 23:02:11.000000 findmyfile-0.3.1/findmyfile.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       45 2023-07-06 23:02:11.000000 findmyfile-0.3.1/findmyfile.egg-info/entry_points.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       53 2023-07-06 23:02:11.000000 findmyfile-0.3.1/findmyfile.egg-info/requires.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       11 2023-07-06 23:02:11.000000 findmyfile-0.3.1/findmyfile.egg-info/top_level.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       38 2023-07-06 23:02:12.756000 findmyfile-0.3.1/setup.cfg
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1714 2023-07-06 23:02:01.000000 findmyfile-0.3.1/setup.py
```

### Comparing `findmyfile-0.3.0/LICENCE.txt` & `findmyfile-0.3.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `findmyfile-0.3.0/PKG-INFO` & `findmyfile-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyfile
-Version: 0.3.0
+Version: 0.3.1
 Summary: This package allows you to search a directory for documents that match keywords
 Home-page: https://github.com/Sanjin84/findmyfile
 Download-URL: https://github.com/Sanjin84/findmyfile/archive/refs/tags/v_01.tar.gz
 Author: Sanjin Dedic
 Author-email: sanjindedic8@gmail.com
 License: MIT
 Keywords: file search,find file,search directory
```

### Comparing `findmyfile-0.3.0/README.md` & `findmyfile-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `findmyfile-0.3.0/findmyfile/main.py` & `findmyfile-0.3.1/findmyfile/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,14 @@
     def __init__(self, path, extension=".txt"):
         self.path = path
         self.name = os.path.basename(self.path)
         self.extension = extension
         self.readable = True
         self.data = ""
 
-    @classmethod
-    def create(cls, path, extension):
-        return cls(path, extension)
-
     def print(self, chars=100):
         """Prints the file data."""
         print("------------------------------------------------")
         print(self.data[:chars])
         print("------------------------------------------------")
 
     def search_all(self, *keywords):
@@ -60,15 +56,16 @@
         try:
             data = ''
             prs = Presentation(self.path)
             values = [shape.text for slide in prs.slides for shape in slide.shapes if hasattr(
                 shape, "text")]
             data = ' '.join(values)
             self.data = data
-        except:
+        except Exception as e:
+            print(f"Failed to read PptxFile: {self.path}. Error: {e}")
             self.readable = False
 
 
 class DocxFile(File):
     """
     The DocxFile class represents a Word (.docx) file. It inherits from the File class and
     overrides the read() method to read Word files.
@@ -78,15 +75,16 @@
         """Reads the Word file and extracts the text."""
         try:
             data = ''
             doc = Document(self.path)
             for para in doc.paragraphs:
                 data += '\n' + para.text
             self.data = data
-        except:
+        except Exception as e:
+            print(f"Failed to read Docx file: {self.path}. Error: {e}")
             self.readable = False
 
 
 class XlsxFile(File):
     """
     The XlsxFile class represents an Excel (.xlsx) file. It inherits from the File class and
     overrides the read() method to read Excel files.
@@ -114,29 +112,46 @@
         try:
             with open(self.path, 'r', encoding="utf8") as f:
                 self.data = f.read()
         except:
             self.readable = False
 
 
+class PyFile(File):
+    """
+    The PyFile class represents a Python (.py) file. It inherits from the File class and
+    overrides the read() method to read Python files.
+    """
+
+    def read(self):
+        """Reads the Python file and stores the data as a string."""
+        try:
+            with open(self.path, 'r', encoding="utf8") as f:
+                self.data = f.read()
+        except Exception as e:
+            print(f"Failed to read PyFile: {self.path}. Error: {e}")
+            self.readable = False
+
+
 class PdfFile(File):
     """
     The PdfFile class represents a PDF (.pdf) file. It inherits from the File class and
     overrides the read() method to read PDF files.
     """
 
     def read(self):
         """Reads the PDF file and extracts the text."""
         try:
             doc = fitz.open(self.path)
             text = ""
             for page in doc:
                 text += page.get_text()
             self.data = text
-        except:
+        except Exception as e:
+            print(f"Failed to read PdfFile: {self.path}. Error: {e}")
             self.readable = False
 
 
 class ProgressBar():
     """
     This class represents a progress bar. It is used to display the progress of a search task.
     A progress bar is created every time a search task is started and it represents the loading
@@ -182,15 +197,15 @@
     def count_files(self):
         """
         Counts the total number of supported files in the given path.
         """
         file_count = 0
         for root, dirs, files in os.walk(self.path, topdown=False):
             for file in files:
-                if file.endswith((".pptx", ".docx", ".xlsx", ".pdf", ".txt")):
+                if file.endswith((".pptx", ".docx", ".xlsx", ".pdf", ".txt", ".py")):
                     file_count += 1
         return file_count
 
     def add_file_data(self):
         """
         Adds file data to the database by creating appropriate file objects for each file type.
         """
@@ -199,15 +214,16 @@
             total_files, prefix='Loading Files:', suffix='Complete', length=50)
         loaded_files = 0
 
         readers = {'pptx': PptxFile,
                    'docx': DocxFile,
                    'xlsx': XlsxFile,
                    'pdf': PdfFile,
-                   'txt': TxtFile
+                   'txt': TxtFile,
+                   'py': PyFile
                    }
 
         for root, dirs, files in os.walk(self.path, topdown=False):
             for file in files:
                 ext = os.path.splitext(file)[-1].lstrip('.')
                 if ext in readers:
                     # creates a file object
```

### Comparing `findmyfile-0.3.0/findmyfile.egg-info/PKG-INFO` & `findmyfile-0.3.1/findmyfile.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyfile
-Version: 0.3.0
+Version: 0.3.1
 Summary: This package allows you to search a directory for documents that match keywords
 Home-page: https://github.com/Sanjin84/findmyfile
 Download-URL: https://github.com/Sanjin84/findmyfile/archive/refs/tags/v_01.tar.gz
 Author: Sanjin Dedic
 Author-email: sanjindedic8@gmail.com
 License: MIT
 Keywords: file search,find file,search directory
```

### Comparing `findmyfile-0.3.0/setup.py` & `findmyfile-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='findmyfile',         # How you named your package folder (MyLib)
     packages=find_packages(),   # Chose the same as "name"
-    version='0.3.0',      # Start with a small number and increase it with every change you make
+    version='0.3.1',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='This package allows you to search a directory for documents that match keywords',
     author='Sanjin Dedic',                   # Type in your name
     author_email='sanjindedic8@gmail.com',      # Type in your E-Mail
     # Provide either the link to your github or to your website
```

