# Comparing `tmp/GSpreadPlus-0.4.4.tar.gz` & `tmp/GSpreadPlus-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GSpreadPlus-0.4.4.tar", last modified: Tue Dec  6 23:07:46 2022, max compression
+gzip compressed data, was "GSpreadPlus-0.4.6.tar", last modified: Fri Jul  7 08:12:31 2023, max compression
```

## Comparing `GSpreadPlus-0.4.4.tar` & `GSpreadPlus-0.4.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2022-12-06 23:07:46.459743 GSpreadPlus-0.4.4/
-drwxrwxrwx   0        0        0        0 2022-12-06 23:07:46.459243 GSpreadPlus-0.4.4/GSpreadPlus/
--rw-rw-rw-   0        0        0       26 2022-05-12 15:31:19.000000 GSpreadPlus-0.4.4/GSpreadPlus/__init__.py
--rw-rw-rw-   0        0        0       47 2022-05-12 15:29:57.000000 GSpreadPlus-0.4.4/GSpreadPlus/errors.py
--rw-rw-rw-   0        0        0    11181 2022-12-06 23:06:08.235416 GSpreadPlus-0.4.4/GSpreadPlus/gspreadplus.py
--rw-rw-rw-   0        0        0     1104 2022-12-06 23:07:46.459743 GSpreadPlus-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       40 2022-04-12 14:24:03.000000 GSpreadPlus-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1304 2022-12-06 23:06:22.267552 GSpreadPlus-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:31.685506 GSpreadPlus-0.4.6/
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:31.684500 GSpreadPlus-0.4.6/GSpreadPlus/
+-rw-rw-rw-   0        0        0       26 2022-05-12 15:31:19.000000 GSpreadPlus-0.4.6/GSpreadPlus/__init__.py
+-rw-rw-rw-   0        0        0       47 2022-05-12 15:29:57.000000 GSpreadPlus-0.4.6/GSpreadPlus/errors.py
+-rw-rw-rw-   0        0        0    13205 2023-07-07 08:09:40.484028 GSpreadPlus-0.4.6/GSpreadPlus/gspreadplus.py
+-rw-rw-rw-   0        0        0     1104 2023-07-07 08:12:31.686506 GSpreadPlus-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2022-04-12 14:24:03.000000 GSpreadPlus-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2023-07-07 08:09:53.494185 GSpreadPlus-0.4.6/setup.py
```

### Comparing `GSpreadPlus-0.4.4/GSpreadPlus/gspreadplus.py` & `GSpreadPlus-0.4.6/GSpreadPlus/gspreadplus.py`

 * *Files 11% similar despite different names*

```diff
@@ -145,63 +145,101 @@
         if header in self.headers:
             index = self.headers.index(header)
         else:
             raise IdentificationError(f"Header with name '{header}' and depth '{self.header_depth}' in {self.orientation} orientation not found\nHeaders starting with: [{self.headers[0]},...")
         return index # Pythonic Indexing
 
     @requirements_exists('*')
-    def commit_new_row(self, values: Union[list,dict], offset:int=0, refresh=True)->list[gspread.cell.Cell]:
+    def commit_new_row(self, values: Union[list,tuple,dict], offset: int = 0, refresh: bool = True)->list[gspread.cell.Cell]:
         '''
         Parameters:
         - values
-            Either a list or dictonary
+            Either a list, tuple or dictonary
             A list would be updated in the given order
             A dict would be updated based on the header of the column that corresponds with the dict key
         - offset
             The number of columns to skip from the left before placing the data
-            For by headers method, these columns will not be checked
+            For by headers method(dict), these columns will not be checked
         - refresh
             The nature of this method defaults this parameter to True
         '''
         if refresh:
             self.refresh_sheet()
         new_row_no = len(self.listed)
         old_commits = set(self.commits.copy())
-        if isinstance(values,list):
+        if isinstance(values,(list, tuple)):
             for i in range(len(values)):
                 self.commits.append(gspread.cell.Cell(row=new_row_no+1,col=i+1+offset,value=values[i]))
         elif isinstance(values,dict):
             headers = self.headers
             assert headers[offset:]!=[], f'Headers Row Empty (offset={offset})'
             for k,v in values.items():
                 if k in headers[offset:]:
                     self.commits.append(gspread.cell.Cell(row=new_row_no+1,col=headers[offset:].index(k)+1,value=v))
                 else:
                     print(f"Dict key <{k}> could not be found in headers...skipping...")
         return [x for x in [i for i in self.commits if self.commits.count(i)>1] if x not in old_commits]
         
+    def commit_new_multiple_rows(self, values: Union[list[list],list[dict]], offset: int = 0, refresh: bool = True)->list[gspread.cell.Cell]:
+        '''
+        Parameters:
+        - values
+            A list of either a list, tuple or dictonary
+            A list would be updated in the given order
+            A dict would be updated based on the header of the column that corresponds with the dict key
+        - offset
+            The number of columns to skip from the left before placing the data
+            For by headers method(dict), these columns will not be checked
+        - refresh
+            The nature of this method defaults this parameter to True
+        '''
+        if refresh:
+            self.refresh_sheet()
+        new_row_no = len(self.listed)
+        old_commits = set(self.commits.copy())
+        internal_offset = 0
+        if isinstance(values[0],(list, tuple)):
+            for item in values:
+                for i in range(len(item)):
+                    # input(str(item)+str(i))
+                    self.commits.append(gspread.cell.Cell(row=new_row_no+internal_offset+1,col=i+1+offset,value=item[i]))
+                internal_offset += 1
+        elif isinstance(values[0],dict):
+            headers = self.headers
+            assert headers[offset:]!=[], f'Headers Row Empty (offset={offset})'
+            for item in values:
+                for k,v in item.items():
+                    if k in headers[offset:]:
+                        self.commits.append(gspread.cell.Cell(row=new_row_no+internal_offset+1,col=headers[offset:].index(k)+1,value=v))
+                    else:
+                        print(f"Dict key <{k}> could not be found in headers...skipping...")
+                internal_offset += 1
+        if refresh:
+            self.refresh_sheet()
+        return [x for x in [i for i in self.commits if self.commits.count(i)>1] if x not in old_commits]
+        
     @requirements_exists('*')
-    def commit_new_column(self, values: Union[list,dict], offset:int=0, refresh=True)->list[gspread.cell.Cell]:
+    def commit_new_column(self, values: Union[list,tuple,dict], offset: int = 0, refresh: bool = True)->list[gspread.cell.Cell]:
         '''
         Parameters:
         - values
-            Either a list or dictonary
+            Either a list, tuple or dictonary
             A list would be updated in the given order
             A dict would be updated based on the header of the column that corresponds with the dict key
         - offset
             The number of columns to skip from the left before placing the data
-            For by headers method, these columns will not be checked
+            For by headers method(dict), these columns will not be checked
         - refresh
             The nature of this method defaults this parameter to True
         '''
         if refresh:
             self.refresh_sheet()
         new_col_no = len(self.listed[0])
         old_commits = set(self.commits.copy())
-        if isinstance(values,list):
+        if isinstance(values,(list, tuple)):
             for i in range(len(values)):
                 self.commits.append(gspread.cell.Cell(row=i+1+offset,col=new_col_no+1,value=values[i]))
         elif isinstance(values,dict):
             headers = self.headers
             assert headers[offset:]!=[], f'Headers Column Empty (offset={offset})'
             for k,v in values.items():
                 if k in headers[offset:]:
```

### Comparing `GSpreadPlus-0.4.4/PKG-INFO` & `GSpreadPlus-0.4.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: GSpreadPlus
-Version: 0.4.4
+Version: 0.4.6
 Summary: Specific Use Cases for Gspread Wrapper
 Home-page: https://github.com/TheReaper62/GSpread-Plus
 Author: FishballNoodles
 Author-email: joelkhorxw@gmail.com
 License: MIT
-Download-URL: https://github.com/TheReaper62/GSpread-Plus/archive/refs/tags/v0.4.4.tar.gz
+Download-URL: https://github.com/TheReaper62/GSpread-Plus/archive/refs/tags/v0.4.6.tar.gz
 Description: Made on top of the orginal gspread Python API Wrapper, this wrapper (wrapper of a wrapper) targets at specific use cases such as returning row after finding column for a value. You'll get it if you use it. Development is open source and you can also request for features by opening an issue in Github.
 Keywords: Google Spreadsheets,Sheets,Sheetsv4,Python 3+,google-spreadsheets,spreadsheets
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GSpreadPlus-0.4.4/setup.py` & `GSpreadPlus-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
     name = 'GSpreadPlus',
     packages = ['GSpreadPlus'],
-    version = '0.4.4',
+    version = '0.4.6',
     license='MIT',
     description = 'Specific Use Cases for Gspread Wrapper',
     author = 'FishballNoodles',
     author_email = 'joelkhorxw@gmail.com',
     url = 'https://github.com/TheReaper62/GSpread-Plus',
-    download_url = 'https://github.com/TheReaper62/GSpread-Plus/archive/refs/tags/v0.4.4.tar.gz',
+    download_url = 'https://github.com/TheReaper62/GSpread-Plus/archive/refs/tags/v0.4.6.tar.gz',
     keywords = ['Google Spreadsheets', 'Sheets', 'Sheetsv4','Python 3+','google-spreadsheets','spreadsheets'],
     install_requires= [
         'oauth2client',
         'gspread'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
```

