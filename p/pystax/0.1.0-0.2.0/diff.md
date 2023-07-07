# Comparing `tmp/pystax-0.1.0.tar.gz` & `tmp/pystax-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystax-0.1.0.tar", last modified: Thu Jul  6 15:33:32 2023, max compression
+gzip compressed data, was "pystax-0.2.0.tar", last modified: Fri Jul  7 18:17:39 2023, max compression
```

## Comparing `pystax-0.1.0.tar` & `pystax-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 15:33:32.026189 pystax-0.1.0/
--rw-rw-rw-   0        0        0      889 2023-07-06 15:33:32.026189 pystax-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-06 15:33:11.000000 pystax-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 15:33:32.010563 pystax-0.1.0/pystax/
--rw-rw-rw-   0        0        0        0 2023-07-05 19:16:55.000000 pystax-0.1.0/pystax/__init__.py
--rw-rw-rw-   0        0        0     2310 2023-07-05 23:12:51.000000 pystax-0.1.0/pystax/checker.py
--rw-rw-rw-   0        0        0      747 2023-07-06 15:32:47.000000 pystax-0.1.0/pystax/test.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:33:32.026189 pystax-0.1.0/pystax.egg-info/
--rw-rw-rw-   0        0        0      889 2023-07-06 15:33:31.000000 pystax-0.1.0/pystax.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-06 15:33:32.000000 pystax-0.1.0/pystax.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 15:33:31.000000 pystax-0.1.0/pystax.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 15:33:32.000000 pystax-0.1.0/pystax.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 15:33:32.026189 pystax-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1468 2023-07-06 15:32:47.000000 pystax-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:17:39.466606 pystax-0.2.0/
+-rw-rw-rw-   0        0        0      889 2023-07-07 18:17:39.461223 pystax-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-07-06 15:41:49.000000 pystax-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 18:17:39.443811 pystax-0.2.0/pystax/
+-rw-rw-rw-   0        0        0        0 2023-07-05 19:16:55.000000 pystax-0.2.0/pystax/__init__.py
+-rw-rw-rw-   0        0        0     2817 2023-07-07 17:54:42.000000 pystax-0.2.0/pystax/checker.py
+-rw-rw-rw-   0        0        0      747 2023-07-06 15:32:47.000000 pystax-0.2.0/pystax/test.py
+drwxrwxrwx   0        0        0        0 2023-07-07 18:17:39.461223 pystax-0.2.0/pystax.egg-info/
+-rw-rw-rw-   0        0        0      889 2023-07-07 18:17:39.000000 pystax-0.2.0/pystax.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-07-07 18:17:39.000000 pystax-0.2.0/pystax.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 18:17:39.000000 pystax-0.2.0/pystax.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 18:17:39.000000 pystax-0.2.0/pystax.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 18:17:39.466606 pystax-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2023-07-07 18:16:29.000000 pystax-0.2.0/setup.py
```

### Comparing `pystax-0.1.0/PKG-INFO` & `pystax-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystax
-Version: 0.1.0
+Version: 0.2.0
 Summary: pystax Python library
 Author: Pritam Dash
 Author-email: pritamdash1997@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pystax-0.1.0/README.md` & `pystax-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 
 - Supports probing domains using both HTTP and HTTPS protocols.
 - Handles various errors such as invalid domains, connection timeouts, and SSL certificate verification failures.
 - Includes special handling for the localhost address (`127.0.0.1` or `"localhost"`).
 
 ## Installation
 
-You can install the Domain Probe library using pip:
+You can install the pystax library using pip:
 
 ```bash
 pip install pystax
```

### Comparing `pystax-0.1.0/pystax/checker.py` & `pystax-0.2.0/pystax/checker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 import socket
 import http.client
 import ssl
+import urllib
 
 
 class DomainProbe:
     def __init__(self):
         self.conn = None
 
-    def probe_domain(self, domain):
+    def probe_domain(self, domain, max_redirects=5):
         try:
             if domain.lower() == "localhost" or domain == "127.0.0.1":
                 return "HTTP", 200
 
             context = ssl.create_default_context()
             context.check_hostname = False
             context.verify_mode = ssl.CERT_NONE
             context.load_default_certs()
 
             self.conn = http.client.HTTPSConnection(domain, timeout=5, context=context)
             self.conn.request("GET", "/")
             response = self.conn.getresponse()
+            if response.status in (301, 302, 303, 307, 308):
+                if max_redirects > 0:
+                    location = response.getheader("Location")
+                    if location:
+                        parsed_url = urllib.parse.urlparse(location)
+                        next_domain = parsed_url.netloc
+                        return self.probe_domain(next_domain, max_redirects=max_redirects - 1)
+                return "Error: Too many redirects"
+
             return "HTTPS", response.status
         except (socket.gaierror, http.client.HTTPException):
             try:
                 self.conn = http.client.HTTPConnection(domain, timeout=5)
                 self.conn.request("GET", "/")
                 response = self.conn.getresponse()
                 return "HTTP", response.status
```

### Comparing `pystax-0.1.0/pystax/test.py` & `pystax-0.2.0/pystax/test.py`

 * *Files identical despite different names*

### Comparing `pystax-0.1.0/pystax.egg-info/PKG-INFO` & `pystax-0.2.0/pystax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystax
-Version: 0.1.0
+Version: 0.2.0
 Summary: pystax Python library
 Author: Pritam Dash
 Author-email: pritamdash1997@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pystax-0.1.0/setup.py` & `pystax-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="pystax",
-    version="0.1.0",
+    version="0.2.0",
     description="pystax Python library",
     long_description="The pystax is a Python library that allows you to probe domains and IP addresses to check their status codes. It helps you verify the accessibility of a domain or IP by performing an HTTP request and retrieving the corresponding status code.,",
     long_description_content_type="text/markdown",
     author="Pritam Dash",
     author_email="pritamdash1997@gmail.com",
     license="MIT",
     classifiers=[
```

