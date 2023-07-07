# Comparing `tmp/pytbai-1.3.3.tar.gz` & `tmp/pytbai-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.3.3.tar", last modified: Fri Jul  7 10:10:09 2023, max compression
+gzip compressed data, was "pytbai-1.3.4.tar", last modified: Fri Jul  7 10:30:28 2023, max compression
```

## Comparing `pytbai-1.3.3.tar` & `pytbai-1.3.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.237161 pytbai-1.3.3/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1301 2023-07-07 10:10:08.000000 pytbai-1.3.3/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-07 10:10:08.000000 pytbai-1.3.3/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-07 10:10:08.000000 pytbai-1.3.3/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-07 10:10:08.000000 pytbai-1.3.3/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 10:10:08.000000 pytbai-1.3.3/Makefile
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 10:10:09.237161 pytbai-1.3.3/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-07 10:10:08.000000 pytbai-1.3.3/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.233162 pytbai-1.3.3/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    10691 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2992 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.233162 pytbai-1.3.3/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.233162 pytbai-1.3.3/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/templates/PDF/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.233162 pytbai-1.3.3/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/templates/XML/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.233162 pytbai-1.3.3/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/templates/XSD/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/templates/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.233162 pytbai-1.3.3/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/utils/pdf.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4524 2023-07-07 10:10:08.000000 pytbai-1.3.3/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.233162 pytbai-1.3.3/pytbai.egg-info/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 10:10:09.000000 pytbai-1.3.3/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-07 10:10:09.000000 pytbai-1.3.3/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-07 10:10:09.000000 pytbai-1.3.3/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-07 10:10:09.000000 pytbai-1.3.3/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 10:10:08.000000 pytbai-1.3.3/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-07 10:10:09.237161 pytbai-1.3.3/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-07 10:10:08.000000 pytbai-1.3.3/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.233162 pytbai-1.3.3/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:08.000000 pytbai-1.3.3/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.233162 pytbai-1.3.3/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-07 10:10:08.000000 pytbai-1.3.3/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-07 10:10:08.000000 pytbai-1.3.3/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-07 10:10:08.000000 pytbai-1.3.3/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-07 10:10:08.000000 pytbai-1.3.3/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:10:09.233162 pytbai-1.3.3/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2938 2023-07-07 10:10:08.000000 pytbai-1.3.3/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-07 10:10:08.000000 pytbai-1.3.3/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.599691 pytbai-1.3.4/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1412 2023-07-07 10:30:27.000000 pytbai-1.3.4/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-07 10:30:27.000000 pytbai-1.3.4/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-07 10:30:27.000000 pytbai-1.3.4/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-07 10:30:27.000000 pytbai-1.3.4/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 10:30:27.000000 pytbai-1.3.4/Makefile
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 10:30:28.599691 pytbai-1.3.4/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-07 10:30:27.000000 pytbai-1.3.4/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.595691 pytbai-1.3.4/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    10498 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2992 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.595691 pytbai-1.3.4/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.599691 pytbai-1.3.4/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/templates/PDF/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.599691 pytbai-1.3.4/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/templates/XML/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.599691 pytbai-1.3.4/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/templates/XSD/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/templates/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.599691 pytbai-1.3.4/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/utils/pdf.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4524 2023-07-07 10:30:27.000000 pytbai-1.3.4/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.595691 pytbai-1.3.4/pytbai.egg-info/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 10:30:28.000000 pytbai-1.3.4/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-07 10:30:28.000000 pytbai-1.3.4/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-07 10:30:28.000000 pytbai-1.3.4/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-07 10:30:28.000000 pytbai-1.3.4/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 10:30:27.000000 pytbai-1.3.4/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-07 10:30:28.599691 pytbai-1.3.4/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-07 10:30:27.000000 pytbai-1.3.4/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.599691 pytbai-1.3.4/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:27.000000 pytbai-1.3.4/tests/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.599691 pytbai-1.3.4/tests/certs/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-07 10:30:27.000000 pytbai-1.3.4/tests/certs/cert.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-07 10:30:27.000000 pytbai-1.3.4/tests/certs/cert_for_tests.p12
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-07 10:30:27.000000 pytbai-1.3.4/tests/certs/key.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-07 10:30:27.000000 pytbai-1.3.4/tests/context.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 10:30:28.599691 pytbai-1.3.4/tests/data/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2938 2023-07-07 10:30:27.000000 pytbai-1.3.4/tests/data/tbai_json.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-07 10:30:27.000000 pytbai-1.3.4/tests/test_basic.py
```

### Comparing `pytbai-1.3.3/CHANGELOG.txt` & `pytbai-1.3.4/CHANGELOG.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+1.3.4 (2023-07-07)
+------------------
+
+- fix invoice get_dict [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+
+
 1.3.3 (2023-07-07)
 ------------------
 
 - xml/xsd/html/css files missing [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.3.3/LICENSE` & `pytbai-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/PKG-INFO` & `pytbai-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.3.3
+Version: 1.3.4
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.3.3/README.md` & `pytbai-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/pytbai/core.py` & `pytbai-1.3.4/pytbai/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -243,20 +243,15 @@
     def delete_lines(self, lines):
         curr_lines = self.lines
         for line in lines:
             curr_lines.remove(line)
         self.lines = curr_lines
 
     def get_dict(self):
-        invoice_json = self.__dict__
-        lines_json = []
-        for line in invoice_json["lines"]:
-            lines_json.append(line.get_dict())
-        invoice_json["lines"] = lines_json
-        return invoice_json
+        return self.__dict__
 
 
 class Software:
     def __init__(
         self,
         license,
         dev_entity,
```

### Comparing `pytbai-1.3.3/pytbai/definitions.py` & `pytbai-1.3.4/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.3.4/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.3.4/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.3.4/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.3.4/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/pytbai/utils/pdf.py` & `pytbai-1.3.4/pytbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/pytbai/utils/xml.py` & `pytbai-1.3.4/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/pytbai.egg-info/PKG-INFO` & `pytbai-1.3.4/pytbai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.3.3
+Version: 1.3.4
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.3.3/pytbai.egg-info/SOURCES.txt` & `pytbai-1.3.4/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/setup.py` & `pytbai-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.3.3",
+    version="1.3.4",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.3.3/tests/certs/cert.pem` & `pytbai-1.3.4/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/tests/certs/cert_for_tests.p12` & `pytbai-1.3.4/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/tests/certs/key.pem` & `pytbai-1.3.4/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/tests/data/tbai_json.py` & `pytbai-1.3.4/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.3/tests/test_basic.py` & `pytbai-1.3.4/tests/test_basic.py`

 * *Files identical despite different names*

