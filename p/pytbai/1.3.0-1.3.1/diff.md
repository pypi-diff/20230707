# Comparing `tmp/pytbai-1.3.0.tar.gz` & `tmp/pytbai-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.3.0.tar", last modified: Fri Jul  7 09:21:40 2023, max compression
+gzip compressed data, was "pytbai-1.3.1.tar", last modified: Fri Jul  7 09:51:09 2023, max compression
```

## Comparing `pytbai-1.3.0.tar` & `pytbai-1.3.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      929 2023-07-07 09:21:38.000000 pytbai-1.3.0/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-07 09:21:38.000000 pytbai-1.3.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-07 09:21:38.000000 pytbai-1.3.0/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-07 09:21:38.000000 pytbai-1.3.0/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 09:21:38.000000 pytbai-1.3.0/Makefile
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 09:21:40.766123 pytbai-1.3.0/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-07 09:21:38.000000 pytbai-1.3.0/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    10691 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2992 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.762123 pytbai-1.3.0/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/utils/pdf.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4524 2023-07-07 09:21:38.000000 pytbai-1.3.0/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/pytbai.egg-info/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 09:21:40.000000 pytbai-1.3.0/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      711 2023-07-07 09:21:40.000000 pytbai-1.3.0/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-07 09:21:40.000000 pytbai-1.3.0/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-07 09:21:40.000000 pytbai-1.3.0/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 09:21:38.000000 pytbai-1.3.0/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-07 09:21:40.766123 pytbai-1.3.0/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1044 2023-07-07 09:21:38.000000 pytbai-1.3.0/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:21:40.766123 pytbai-1.3.0/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2938 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-07 09:21:38.000000 pytbai-1.3.0/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1041 2023-07-07 09:51:08.000000 pytbai-1.3.1/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-07 09:51:08.000000 pytbai-1.3.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-07 09:51:08.000000 pytbai-1.3.1/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      272 2023-07-07 09:51:08.000000 pytbai-1.3.1/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 09:51:08.000000 pytbai-1.3.1/Makefile
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 09:51:09.423006 pytbai-1.3.1/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-07 09:51:08.000000 pytbai-1.3.1/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    10691 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2992 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/templates/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/utils/pdf.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4524 2023-07-07 09:51:08.000000 pytbai-1.3.1/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/pytbai.egg-info/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 09:51:09.000000 pytbai-1.3.1/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      740 2023-07-07 09:51:09.000000 pytbai-1.3.1/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-07 09:51:09.000000 pytbai-1.3.1/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-07 09:51:09.000000 pytbai-1.3.1/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 09:51:08.000000 pytbai-1.3.1/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-07 09:51:09.423006 pytbai-1.3.1/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-07 09:51:08.000000 pytbai-1.3.1/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:08.000000 pytbai-1.3.1/tests/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/tests/certs/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-07 09:51:08.000000 pytbai-1.3.1/tests/certs/cert.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-07 09:51:08.000000 pytbai-1.3.1/tests/certs/cert_for_tests.p12
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-07 09:51:08.000000 pytbai-1.3.1/tests/certs/key.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-07 09:51:08.000000 pytbai-1.3.1/tests/context.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 09:51:09.423006 pytbai-1.3.1/tests/data/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2938 2023-07-07 09:51:08.000000 pytbai-1.3.1/tests/data/tbai_json.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-07 09:51:08.000000 pytbai-1.3.1/tests/test_basic.py
```

### Comparing `pytbai-1.3.0/CHANGELOG.txt` & `pytbai-1.3.1/CHANGELOG.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+1.3.1 (2023-07-07)
+------------------
+
+- package configuration [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+
+
 1.3.0 (2023-07-07)
 ------------------
 
 - include templates in the release [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.3.0/LICENSE` & `pytbai-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/PKG-INFO` & `pytbai-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.3.0/README.md` & `pytbai-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/pytbai/core.py` & `pytbai-1.3.1/pytbai/core.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/pytbai/definitions.py` & `pytbai-1.3.1/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.3.1/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.3.1/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.3.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.3.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/pytbai/utils/pdf.py` & `pytbai-1.3.1/pytbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/pytbai/utils/xml.py` & `pytbai-1.3.1/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/pytbai.egg-info/PKG-INFO` & `pytbai-1.3.1/pytbai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.3.0/pytbai.egg-info/SOURCES.txt` & `pytbai-1.3.1/pytbai.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pytbai/__init__.py
 pytbai/core.py
 pytbai/definitions.py
 pytbai.egg-info/PKG-INFO
 pytbai.egg-info/SOURCES.txt
 pytbai.egg-info/dependency_links.txt
 pytbai.egg-info/top_level.txt
+pytbai/templates/__init__.py
 pytbai/templates/PDF/ticketbai.css
 pytbai/templates/PDF/ticketbai.html
 pytbai/templates/XML/tbai_structure.xml
 pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
 pytbai/templates/XSD/ticketBaiV1-2-1.xsd
 pytbai/utils/__init__.py
 pytbai/utils/crypto.py
```

### Comparing `pytbai-1.3.0/setup.py` & `pytbai-1.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,26 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.3.0",
+    version="1.3.1",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
     author_email="uodriozola@codesyntax.com",
     url="https://github.com/codesyntax/pytbai",
     license=license,
-    packages=find_packages(exclude=("tests", "docs")),
+    packages=find_packages(exclude=("tests",)),
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `pytbai-1.3.0/tests/certs/cert.pem` & `pytbai-1.3.1/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/tests/certs/cert_for_tests.p12` & `pytbai-1.3.1/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/tests/certs/key.pem` & `pytbai-1.3.1/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/tests/data/tbai_json.py` & `pytbai-1.3.1/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.0/tests/test_basic.py` & `pytbai-1.3.1/tests/test_basic.py`

 * *Files identical despite different names*

