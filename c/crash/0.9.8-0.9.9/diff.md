# Comparing `tmp/crash-0.9.8.tar.gz` & `tmp/crash-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crash-0.9.8.tar", last modified: Tue Jun  3 10:03:41 2014, max compression
+gzip compressed data, was "dist/crash-0.9.9.tar", last modified: Tue Jun  3 13:59:07 2014, max compression
```

## Comparing `crash-0.9.8.tar` & `crash-0.9.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-06-03 10:03:41.000000 crash-0.9.8/
--rw-r--r--   0 philipp    (501) staff       (20)     2088 2014-05-20 08:32:26.000000 crash-0.9.8/DEVELOP.rst
--rw-r--r--   0 philipp    (501) staff       (20)    12029 2014-05-09 07:53:46.000000 crash-0.9.8/LICENSE
--rw-r--r--   0 philipp    (501) staff       (20)       89 2014-05-09 07:53:46.000000 crash-0.9.8/MANIFEST.in
--rw-r--r--   0 philipp    (501) staff       (20)     9726 2014-06-03 10:03:41.000000 crash-0.9.8/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)     3295 2014-05-09 10:20:56.000000 crash-0.9.8/README.rst
--rw-r--r--   0 philipp    (501) staff       (20)       82 2014-06-03 10:03:41.000000 crash-0.9.8/setup.cfg
--rw-r--r--   0 philipp    (501) staff       (20)     3186 2014-05-20 08:32:26.000000 crash-0.9.8/setup.py
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-06-03 10:03:41.000000 crash-0.9.8/src/
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-06-03 10:03:41.000000 crash-0.9.8/src/crash.egg-info/
--rw-r--r--   0 philipp    (501) staff       (20)        1 2014-06-03 10:03:41.000000 crash-0.9.8/src/crash.egg-info/dependency_links.txt
--rw-r--r--   0 philipp    (501) staff       (20)       52 2014-06-03 10:03:41.000000 crash-0.9.8/src/crash.egg-info/entry_points.txt
--rw-r--r--   0 philipp    (501) staff       (20)        6 2014-06-03 10:03:41.000000 crash-0.9.8/src/crash.egg-info/namespace_packages.txt
--rw-r--r--   0 philipp    (501) staff       (20)     9726 2014-06-03 10:03:41.000000 crash-0.9.8/src/crash.egg-info/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)       93 2014-06-03 10:03:41.000000 crash-0.9.8/src/crash.egg-info/requires.txt
--rw-r--r--   0 philipp    (501) staff       (20)      466 2014-06-03 10:03:41.000000 crash-0.9.8/src/crash.egg-info/SOURCES.txt
--rw-r--r--   0 philipp    (501) staff       (20)        6 2014-06-03 10:03:41.000000 crash-0.9.8/src/crash.egg-info/top_level.txt
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-06-03 10:03:41.000000 crash-0.9.8/src/crate/
--rw-r--r--   0 philipp    (501) staff       (20)     1227 2014-05-09 07:53:46.000000 crash-0.9.8/src/crate/__init__.py
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-06-03 10:03:41.000000 crash-0.9.8/src/crate/crash/
--rw-r--r--   0 philipp    (501) staff       (20)     1045 2014-06-03 10:02:03.000000 crash-0.9.8/src/crate/crash/__init__.py
--rw-r--r--   0 philipp    (501) staff       (20)    15793 2014-06-03 09:56:27.000000 crash-0.9.8/src/crate/crash/command.py
--rw-r--r--   0 philipp    (501) staff       (20)     3793 2014-06-03 08:32:53.000000 crash-0.9.8/src/crate/crash/crash.txt
--rw-r--r--   0 philipp    (501) staff       (20)    31487 2014-05-20 09:22:54.000000 crash-0.9.8/src/crate/crash/tabulate.py
--rw-r--r--   0 philipp    (501) staff       (20)     4657 2014-06-03 09:56:27.000000 crash-0.9.8/src/crate/crash/test_command.py
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-06-03 13:59:07.000000 crash-0.9.9/
+-rw-r--r--   0 philipp    (501) staff       (20)     2088 2014-05-20 08:32:26.000000 crash-0.9.9/DEVELOP.rst
+-rw-r--r--   0 philipp    (501) staff       (20)    12029 2014-05-09 07:53:46.000000 crash-0.9.9/LICENSE
+-rw-r--r--   0 philipp    (501) staff       (20)       89 2014-05-09 07:53:46.000000 crash-0.9.9/MANIFEST.in
+-rw-r--r--   0 philipp    (501) staff       (20)     9726 2014-06-03 13:59:07.000000 crash-0.9.9/PKG-INFO
+-rw-r--r--   0 philipp    (501) staff       (20)     3295 2014-05-09 10:20:56.000000 crash-0.9.9/README.rst
+-rw-r--r--   0 philipp    (501) staff       (20)       82 2014-06-03 13:59:07.000000 crash-0.9.9/setup.cfg
+-rw-r--r--   0 philipp    (501) staff       (20)     3186 2014-05-20 08:32:26.000000 crash-0.9.9/setup.py
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-06-03 13:59:07.000000 crash-0.9.9/src/
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-06-03 13:59:07.000000 crash-0.9.9/src/crash.egg-info/
+-rw-r--r--   0 philipp    (501) staff       (20)        1 2014-06-03 13:59:07.000000 crash-0.9.9/src/crash.egg-info/dependency_links.txt
+-rw-r--r--   0 philipp    (501) staff       (20)       52 2014-06-03 13:59:07.000000 crash-0.9.9/src/crash.egg-info/entry_points.txt
+-rw-r--r--   0 philipp    (501) staff       (20)        6 2014-06-03 13:59:07.000000 crash-0.9.9/src/crash.egg-info/namespace_packages.txt
+-rw-r--r--   0 philipp    (501) staff       (20)     9726 2014-06-03 13:59:07.000000 crash-0.9.9/src/crash.egg-info/PKG-INFO
+-rw-r--r--   0 philipp    (501) staff       (20)       93 2014-06-03 13:59:07.000000 crash-0.9.9/src/crash.egg-info/requires.txt
+-rw-r--r--   0 philipp    (501) staff       (20)      466 2014-06-03 13:59:07.000000 crash-0.9.9/src/crash.egg-info/SOURCES.txt
+-rw-r--r--   0 philipp    (501) staff       (20)        6 2014-06-03 13:59:07.000000 crash-0.9.9/src/crash.egg-info/top_level.txt
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-06-03 13:59:07.000000 crash-0.9.9/src/crate/
+-rw-r--r--   0 philipp    (501) staff       (20)     1227 2014-05-09 07:53:46.000000 crash-0.9.9/src/crate/__init__.py
+drwxr-xr-x   0 philipp    (501) staff       (20)        0 2014-06-03 13:59:07.000000 crash-0.9.9/src/crate/crash/
+-rw-r--r--   0 philipp    (501) staff       (20)     1045 2014-06-03 13:58:13.000000 crash-0.9.9/src/crate/crash/__init__.py
+-rw-r--r--   0 philipp    (501) staff       (20)    15806 2014-06-03 13:57:26.000000 crash-0.9.9/src/crate/crash/command.py
+-rw-r--r--   0 philipp    (501) staff       (20)     3793 2014-06-03 08:32:53.000000 crash-0.9.9/src/crate/crash/crash.txt
+-rw-r--r--   0 philipp    (501) staff       (20)    31487 2014-06-03 13:34:22.000000 crash-0.9.9/src/crate/crash/tabulate.py
+-rw-r--r--   0 philipp    (501) staff       (20)     5262 2014-06-03 13:57:26.000000 crash-0.9.9/src/crate/crash/test_command.py
```

### Comparing `crash-0.9.8/DEVELOP.rst` & `crash-0.9.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `crash-0.9.8/LICENSE` & `crash-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crash-0.9.8/PKG-INFO` & `crash-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: crash
-Version: 0.9.8
+Version: 0.9.9
 Summary: The Crate Data Shell
 Home-page: https://github.com/crate/crash
 Author: CRATE Technology GmbH
 Author-email: office@crate.io
 License: Apache License 2.0
 Description: .. image:: https://cdn.crate.io/web/1.0.0/img/logo-solid.png
            :width: 155px
```

### Comparing `crash-0.9.8/README.rst` & `crash-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `crash-0.9.8/setup.py` & `crash-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `crash-0.9.8/src/crash.egg-info/PKG-INFO` & `crash-0.9.9/src/crash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: crash
-Version: 0.9.8
+Version: 0.9.9
 Summary: The Crate Data Shell
 Home-page: https://github.com/crate/crash
 Author: CRATE Technology GmbH
 Author-email: office@crate.io
 License: Apache License 2.0
 Description: .. image:: https://cdn.crate.io/web/1.0.0/img/logo-solid.png
            :width: 155px
```

### Comparing `crash-0.9.8/src/crate/__init__.py` & `crash-0.9.9/src/crate/__init__.py`

 * *Files identical despite different names*

### Comparing `crash-0.9.8/src/crate/crash/__init__.py` & `crash-0.9.9/src/crate/crash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
 
-__version__ = '0.9.8'
+__version__ = '0.9.9'
```

### Comparing `crash-0.9.8/src/crate/crash/command.py` & `crash-0.9.9/src/crate/crash/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                 print(e)
         return False
 
     def pprint(self, rows, cols=None):
         if cols is None:
             cols = self.cols()
         rows = [list(map(self._transform_field, row)) for row in rows]
-        print(tabulate(rows, headers=cols, tablefmt=crate_fmt))
+        print(tabulate(rows, headers=cols, tablefmt=crate_fmt, floatfmt=""))
 
     def _transform_field(self, field):
         """transform field for displaying"""
         if field is None:
             return self.NULL
         elif isinstance(field, bool):
             return "TRUE" if field else "FALSE"
```

### Comparing `crash-0.9.8/src/crate/crash/crash.txt` & `crash-0.9.9/src/crate/crash/crash.txt`

 * *Files identical despite different names*

### Comparing `crash-0.9.8/src/crate/crash/tabulate.py` & `crash-0.9.9/src/crate/crash/tabulate.py`

 * *Files identical despite different names*

### Comparing `crash-0.9.8/src/crate/crash/test_command.py` & `crash-0.9.9/src/crate/crash/test_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,7 +120,22 @@
                               '+--------------------+',
                               '| ["Arthur", "Ford"] |',
                               '+--------------------+\n'])
         command = CrateCmd()
         with patch('sys.stdout', new_callable=StringIO) as output:
             command.pprint([[names]], ['names'])
             self.assertEqual(expected, output.getvalue())
+
+
+
+    def test_rendering_float(self):
+        """Test rendering an array"""
+        expected = "\n".join(['+---------------+',
+                              '|        number |',
+                              '+---------------+',
+                              '|  3.1415926535 |',
+                              '| 42.0          |',
+                              '+---------------+\n'])
+        command = CrateCmd()
+        with patch('sys.stdout', new_callable=StringIO) as output:
+            command.pprint([[3.1415926535], [42.0]], ['number'])
+            self.assertEqual(expected, output.getvalue())
```

