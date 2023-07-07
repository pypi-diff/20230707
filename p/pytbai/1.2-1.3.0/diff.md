# Comparing `tmp/pytbai-1.2.tar.gz` & `tmp/pytbai-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.2.tar", last modified: Wed Jul  5 14:47:48 2023, max compression
+gzip compressed data, was "pytbai-1.3.0.tar", last modified: Fri Jul  7 09:21:40 2023, max compression
```

## Comparing `pytbai-1.2.tar` & `pytbai-1.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.088391 pytbai-1.2/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      806 2023-07-05 14:47:46.000000 pytbai-1.2/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-05 14:47:46.000000 pytbai-1.2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-05 14:47:46.000000 pytbai-1.2/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      271 2023-07-05 14:47:46.000000 pytbai-1.2/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-05 14:47:46.000000 pytbai-1.2/Makefile
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3640 2023-07-05 14:47:48.088391 pytbai-1.2/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-05 14:47:46.000000 pytbai-1.2/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.084391 pytbai-1.2/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    10691 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2992 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.080391 pytbai-1.2/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.084391 pytbai-1.2/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.084391 pytbai-1.2/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.084391 pytbai-1.2/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.088391 pytbai-1.2/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/utils/pdf.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4524 2023-07-05 14:47:46.000000 pytbai-1.2/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.084391 pytbai-1.2/pytbai.egg-info/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3640 2023-07-05 14:47:48.000000 pytbai-1.2/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      711 2023-07-05 14:47:48.000000 pytbai-1.2/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-05 14:47:48.000000 pytbai-1.2/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-05 14:47:48.000000 pytbai-1.2/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-05 14:47:46.000000 pytbai-1.2/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-05 14:47:48.088391 pytbai-1.2/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1042 2023-07-05 14:47:46.000000 pytbai-1.2/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.088391 pytbai-1.2/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:46.000000 pytbai-1.2/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.088391 pytbai-1.2/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-05 14:47:46.000000 pytbai-1.2/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-05 14:47:46.000000 pytbai-1.2/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-05 14:47:46.000000 pytbai-1.2/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-05 14:47:46.000000 pytbai-1.2/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-05 14:47:48.088391 pytbai-1.2/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2938 2023-07-05 14:47:46.000000 pytbai-1.2/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-05 14:47:46.000000 pytbai-1.2/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      929 2023-07-07 09:21:38.000000 pytbai-1.3.0/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-07 09:21:38.000000 pytbai-1.3.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-07 09:21:38.000000 pytbai-1.3.0/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-07 09:21:38.000000 pytbai-1.3.0/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 09:21:38.000000 pytbai-1.3.0/Makefile
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 09:21:40.766123 pytbai-1.3.0/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-07 09:21:38.000000 pytbai-1.3.0/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    10691 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2992 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.762123 pytbai-1.3.0/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/utils/pdf.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4524 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai.egg-info/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 09:21:40.000000 pytbai-1.3.0/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      711 2023-07-07 09:21:40.000000 pytbai-1.3.0/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-07 09:21:40.000000 pytbai-1.3.0/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-07 09:21:40.000000 pytbai-1.3.0/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 09:21:38.000000 pytbai-1.3.0/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-07 09:21:40.766123 pytbai-1.3.0/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1044 2023-07-07 09:21:38.000000 pytbai-1.3.0/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/tests/certs/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/certs/cert.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/certs/cert_for_tests.p12
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/certs/key.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/context.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/tests/data/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2938 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/data/tbai_json.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/test_basic.py
```

### Comparing `pytbai-1.2/CHANGELOG.txt` & `pytbai-1.3.0/CHANGELOG.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+1.3.0 (2023-07-07)
+------------------
+
+- include templates in the release [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+
+
 1.2 (2023-07-05)
 ----------------
 
 - include pem files for testing purpose [Urtzi Odriozola <uodriozola@codesyntax.com>]
 
 - update README [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.2/LICENSE` & `pytbai-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/PKG-INFO` & `pytbai-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.2
+Version: 1.3.0
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.2/README.md` & `pytbai-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/pytbai/core.py` & `pytbai-1.3.0/pytbai/core.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/pytbai/definitions.py` & `pytbai-1.3.0/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.3.0/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.3.0/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.3.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.3.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/pytbai/utils/pdf.py` & `pytbai-1.3.0/pytbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/pytbai/utils/xml.py` & `pytbai-1.3.0/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/pytbai.egg-info/PKG-INFO` & `pytbai-1.3.0/pytbai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.2
+Version: 1.3.0
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.2/pytbai.egg-info/SOURCES.txt` & `pytbai-1.3.0/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/setup.py` & `pytbai-1.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.2",
+    version="1.3.0",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.2/tests/certs/cert.pem` & `pytbai-1.3.0/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/tests/certs/cert_for_tests.p12` & `pytbai-1.3.0/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/tests/certs/key.pem` & `pytbai-1.3.0/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/tests/data/tbai_json.py` & `pytbai-1.3.0/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.2/tests/test_basic.py` & `pytbai-1.3.0/tests/test_basic.py`

 * *Files identical despite different names*

