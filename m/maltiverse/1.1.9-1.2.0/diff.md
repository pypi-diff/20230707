# Comparing `tmp/maltiverse-1.1.9.tar.gz` & `tmp/maltiverse-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maltiverse-1.1.9.tar", last modified: Fri Mar 17 11:26:19 2023, max compression
+gzip compressed data, was "maltiverse-1.2.0.tar", last modified: Fri Jul  7 09:04:55 2023, max compression
```

## Comparing `maltiverse-1.1.9.tar` & `maltiverse-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 jlopez    (1000) jlopez    (1000)        0 2023-03-17 11:26:19.258275 maltiverse-1.1.9/
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)     1067 2023-03-17 09:54:08.000000 maltiverse-1.1.9/LICENSE
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)    13903 2023-03-17 11:26:19.258275 maltiverse-1.1.9/PKG-INFO
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)    11819 2023-03-17 09:54:08.000000 maltiverse-1.1.9/README.md
-drwxr-xr-x   0 jlopez    (1000) jlopez    (1000)        0 2023-03-17 11:26:19.258275 maltiverse-1.1.9/maltiverse/
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)       61 2023-03-17 09:54:08.000000 maltiverse-1.1.9/maltiverse/__init__.py
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)     9949 2023-03-17 09:54:08.000000 maltiverse-1.1.9/maltiverse/maltiverse.py
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)     7734 2023-03-17 09:54:08.000000 maltiverse-1.1.9/maltiverse/test_maltiverse.py
-drwxr-xr-x   0 jlopez    (1000) jlopez    (1000)        0 2023-03-17 11:26:19.258275 maltiverse-1.1.9/maltiverse.egg-info/
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)    13903 2023-03-17 11:26:19.000000 maltiverse-1.1.9/maltiverse.egg-info/PKG-INFO
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)      279 2023-03-17 11:26:19.000000 maltiverse-1.1.9/maltiverse.egg-info/SOURCES.txt
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)        1 2023-03-17 11:26:19.000000 maltiverse-1.1.9/maltiverse.egg-info/dependency_links.txt
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)       15 2023-03-17 11:26:19.000000 maltiverse-1.1.9/maltiverse.egg-info/requires.txt
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)       11 2023-03-17 11:26:19.000000 maltiverse-1.1.9/maltiverse.egg-info/top_level.txt
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)      978 2023-03-17 11:25:55.000000 maltiverse-1.1.9/pyproject.toml
--rw-r--r--   0 jlopez    (1000) jlopez    (1000)       38 2023-03-17 11:26:19.258275 maltiverse-1.1.9/setup.cfg
+drwxr-xr-x   0 jlopez    (1000) jlopez    (1000)        0 2023-07-07 09:04:55.503188 maltiverse-1.2.0/
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)     1067 2023-03-17 09:54:08.000000 maltiverse-1.2.0/LICENSE
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)    14171 2023-07-07 09:04:55.503188 maltiverse-1.2.0/PKG-INFO
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)    11819 2023-03-17 09:54:08.000000 maltiverse-1.2.0/README.md
+drwxr-xr-x   0 jlopez    (1000) jlopez    (1000)        0 2023-07-07 09:04:55.503188 maltiverse-1.2.0/maltiverse/
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)       61 2023-03-17 09:54:08.000000 maltiverse-1.2.0/maltiverse/__init__.py
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)     8892 2023-07-07 09:00:45.000000 maltiverse-1.2.0/maltiverse/maltiverse.py
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)     7722 2023-07-07 09:00:45.000000 maltiverse-1.2.0/maltiverse/test_maltiverse.py
+drwxr-xr-x   0 jlopez    (1000) jlopez    (1000)        0 2023-07-07 09:04:55.503188 maltiverse-1.2.0/maltiverse.egg-info/
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)    14171 2023-07-07 09:04:55.000000 maltiverse-1.2.0/maltiverse.egg-info/PKG-INFO
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)      288 2023-07-07 09:04:55.000000 maltiverse-1.2.0/maltiverse.egg-info/SOURCES.txt
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)        1 2023-07-07 09:04:55.000000 maltiverse-1.2.0/maltiverse.egg-info/dependency_links.txt
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)       15 2023-07-07 09:04:55.000000 maltiverse-1.2.0/maltiverse.egg-info/requires.txt
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)       11 2023-07-07 09:04:55.000000 maltiverse-1.2.0/maltiverse.egg-info/top_level.txt
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)     1031 2023-07-07 09:01:33.000000 maltiverse-1.2.0/pyproject.toml
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)       38 2023-07-07 09:04:55.503188 maltiverse-1.2.0/setup.cfg
+-rw-r--r--   0 jlopez    (1000) jlopez    (1000)     1168 2023-07-07 09:00:45.000000 maltiverse-1.2.0/setup.py
```

### Comparing `maltiverse-1.1.9/LICENSE` & `maltiverse-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maltiverse-1.1.9/PKG-INFO` & `maltiverse-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: maltiverse
-Version: 1.1.9
+Version: 1.2.0
 Summary: Wrapper for the Maltiverse API
-Author-email: Antonio Gomez <antonio.gomez@maltiverse.com>, Jorge Lopez <jorge.lopez@maltiverse.com>
+Home-page: https://github.com/maltiverse/maltiverse-python
+Download-URL: https://github.com/maltiverse/python-maltiverse/archive/master.zip
+Author: Antonio Gomez
+Author-email: Antonio Gomez <antonio.gomez@maltiverse.com>, Jorge Lopez <jorge.lopez@maltiverse.com>, Developers <dev@maltiverse.com>
 License: MIT License
         
         Copyright (c) 2017 maltiverse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -23,14 +26,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/maltiverse/python-maltiverse
 Project-URL: Bug Tracker, https://github.com/maltiverse/python-maltiverse/issues
+Keywords: maltiverse,API,threat intelligence,IoC,blacklist,search engine
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `maltiverse-1.1.9/README.md` & `maltiverse-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `maltiverse-1.1.9/maltiverse/maltiverse.py` & `maltiverse-1.2.0/maltiverse/maltiverse.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,18 @@
         self.endpoint = endpoint
         self.auth_token = auth_token
         self.sub = None
         self.team_name = None
         self.team_researcher = None
         self.admin = None
 
+        self._default_headers = {"Accept": "application/json"}
+        if self.auth_token:
+            self._default_headers.update({"Authorization": f"Bearer {self.auth_token}"})
+
     def prepare_put_payload(self, params):
         """Auxiliar method to perform PUT requests to the platform"""
         if self.team_researcher and not self.admin:
             # Adding required information to push info being a researcher.
             if "blacklist" in params:
                 # Is not allowed to specify dates
                 if "creation_time" in params:
@@ -51,23 +55,22 @@
                         params["blacklist"][i].pop("first_seen", None)
                     if "last_seen" in params["blacklist"][i]:
                         params["blacklist"][i].pop("last_seen", None)
 
         return json.dumps(params)
 
     def login(self, email, password):
-        r = requests.post(
+        r_json = requests.post(
             self.endpoint + "/auth/login",
             data=json.dumps({"email": email, "password": password}),
             headers={
                 "Content-Type": "application/json",
                 "Accept": "application/json",
             },
-        )
-        r_json = json.loads(r.text)
+        ).json()
 
         if "status" in r_json and r_json["status"] == "success":
             if r_json["auth_token"]:
                 self.auth_token = str(r_json["auth_token"])
                 decoded_payload = jwt.decode(
                     self.auth_token, options={"verify_signature": False}
                 )
@@ -77,172 +80,133 @@
                 self.admin = decoded_payload["admin"]
                 return True
 
         raise Exception("Login Failed")
 
     def ip_get(self, ip_addr):
         """Requests an IP address"""
-        headers = {
-            "Accept": "application/json",
-        }
-        if self.auth_token:
-            headers["Authorization"] = "Bearer " + self.auth_token
-        r = requests.get(self.endpoint + "/ip/" + ip_addr, headers=headers)
-        return json.loads(r.text)
+        return requests.get(
+            f"{self.endpoint}/ip/{ip_addr}", headers=self._default_headers
+        ).json()
 
     def ip_put(self, ip_dict):
-        """Inserts a new Ip address observable. If it exists, the document is merged and stored. Requires authentication as admin"""
-        r = requests.put(
-            self.endpoint + "/ip/" + ip_dict["ip_addr"],
+        """Inserts a new Ip address observable.
+
+        If it exists, the document is merged and stored.
+        Requires authentication as admin
+        """
+        return requests.put(
+            f"{self.endpoint}/ip/{ip_dict['ip_addr']}",
             data=self.prepare_put_payload(ip_dict),
-            headers={
-                "Accept": "application/json",
-                "Content-Type": "application/json",
-                "Authorization": "Bearer " + self.auth_token,
-            },
-        )
-        return json.loads(r.text)
+            headers=dict(self._default_headers, **{"Content-Type": "application/json"}),
+        ).json()
 
     def ip_delete(self, ip_addr):
         """Deletes Ip address observable. Requires authentication as admin"""
-        r = requests.delete(
-            self.endpoint + "/ip/" + ip_addr,
-            headers={
-                "Accept": "application/json",
-                "Authorization": "Bearer " + self.auth_token,
-            },
-        )
-        return json.loads(r.text)
+        return requests.delete(
+            f"{self.endpoint}/ip/{ip_addr}", headers=self._default_headers
+        ).json()
 
     def hostname_get(self, hostname):
         """Requests a hostname"""
-        headers = {
-            "Accept": "application/json",
-        }
-        if self.auth_token:
-            headers["Authorization"] = "Bearer " + self.auth_token
-        r = requests.get(self.endpoint + "/hostname/" + hostname, headers=headers)
-        return json.loads(r.text)
+        return requests.get(
+            f"{self.endpoint}/hostname/{hostname}", headers=self._default_headers
+        ).json()
 
     def hostname_put(self, hostname_dict):
         """Inserts a new hostname observable. If it exists, the document is merged and stored. Requires authentication as admin"""
-        r = requests.put(
-            self.endpoint + "/hostname/" + hostname_dict["hostname"],
+        return requests.put(
+            f"{self.endpoint}/hostname/{hostname_dict['hostname']}",
             data=self.prepare_put_payload(hostname_dict),
-            headers={
-                "Accept": "application/json",
-                "Content-Type": "application/json",
-                "Authorization": "Bearer " + self.auth_token,
-            },
-        )
-        return json.loads(r.text)
+            headers=dict(self._default_headers, **{"Content-Type": "application/json"}),
+        ).json()
 
     def hostname_delete(self, hostname):
         """Deletes hostname observable. Requires authentication as admin"""
-        r = requests.delete(
-            self.endpoint + "/hostname/" + hostname,
-            headers={
-                "Accept": "application/json",
-                "Authorization": "Bearer " + self.auth_token,
-            },
-        )
-        return json.loads(r.text)
+        return requests.delete(
+            f"{self.endpoint}/hostname/{hostname}", headers=self._default_headers
+        ).json()
 
     def url_get(self, url):
         """Requests a url"""
         urlchecksum = hashlib.sha256(url.encode("utf-8")).hexdigest()
-        headers = {
-            "Accept": "application/json",
-        }
-        if self.auth_token:
-            headers["Authorization"] = "Bearer " + self.auth_token
-        r = requests.get(self.endpoint + "/url/" + urlchecksum, headers=headers)
-        return json.loads(r.text)
+        return requests.get(
+            f"{self.endpoint}/url/{urlchecksum}", headers=self._default_headers
+        ).json()
 
     def url_get_by_checksum(self, urlchecksum):
         """Requests a url by its sha256 checksum"""
-        headers = {
-            "Accept": "application/json",
-        }
-        if self.auth_token:
-            headers["Authorization"] = "Bearer " + self.auth_token
-        r = requests.get(self.endpoint + "/url/" + urlchecksum, headers=headers)
-        return json.loads(r.text)
+        return requests.get(
+            f"{self.endpoint}/url/{urlchecksum}", headers=self._default_headers
+        ).json()
 
     def url_put(self, url_dict):
         """Inserts a new url observable. If it exists, the document is merged and stored. Requires authentication as admin"""
         urlchecksum = hashlib.sha256(url_dict["url"].encode("utf-8")).hexdigest()
-        r = requests.put(
-            self.endpoint + "/url/" + urlchecksum,
+        return requests.put(
+            f"{self.endpoint}/url/{urlchecksum}",
             data=self.prepare_put_payload(url_dict),
-            headers={
-                "Accept": "application/json",
-                "Content-Type": "application/json",
-                "Authorization": "Bearer " + self.auth_token,
-            },
-        )
-        return json.loads(r.text)
+            headers=dict(self._default_headers, **{"Content-Type": "application/json"}),
+        ).json()
 
     def url_delete(self, url):
         """Deletes url observable. Requires authentication as admin"""
         urlchecksum = hashlib.sha256(url.encode("utf-8")).hexdigest()
-        r = requests.delete(
-            self.endpoint + "/url/" + urlchecksum,
-            headers={
-                "Accept": "application/json",
-                "Authorization": "Bearer " + self.auth_token,
-            },
-        )
-        return json.loads(r.text)
+        return requests.delete(
+            f"{self.endpoint}/url/{urlchecksum}",
+            headers=self._default_headers,
+        ).json()
 
-    def sample_get(self, sha256):
+    def sample_get(self, sample, algorithm="sha256"):
         """Requests a sample"""
-        headers = {
-            "Accept": "application/json",
+        mapping = {
+            "sha256": self.sample_get_by_sha256,
+            "md5": self.sample_get_by_md5,
+            "sha1": self.sample_get_by_sha1,
+            "sha512": self.sample_get_by_sha512,
         }
-        if self.auth_token:
-            headers["Authorization"] = "Bearer " + self.auth_token
-        r = requests.get(self.endpoint + "/sample/" + sha256, headers=headers)
-        return json.loads(r.text)
+        return mapping.get(algorithm, mapping.get("sha256"))()
+
+    def sample_get_by_md5(self, md5):
+        """Requests a sample by MD5"""
+        return requests.get(
+            f"{self.endpoint}/sample/md5/{md5}", headers=self._default_headers
+        ).json()
+
+    def sample_get_by_sha1(self, sha1):
+        """Requests a sample by SHA1"""
+        return requests.get(
+            f"{self.endpoint}/sample/sha1/{sha1}", headers=self._default_headers
+        ).json()
+
+    def sample_get_by_sha256(self, sha256):
+        """Requests a sample by SHA256"""
+        return requests.get(
+            f"{self.endpoint}/sample/{sha256}", headers=self._default_headers
+        ).json()
+
+    def sample_get_by_sha512(self, sha512):
+        """Requests a sample by SHA512"""
+        return requests.get(
+            f"{self.endpoint}/sample/sha512/{sha512}", headers=self._default_headers
+        ).json()
 
     def sample_put(self, sample_dict):
         """Inserts a new sample observable. If it exists, the document is merged and stored. Requires authentication as admin"""
-        r = requests.put(
-            self.endpoint + "/sample/" + sample_dict["sha256"],
+        return requests.put(
+            f"{self.endpoint}/sample/{sample_dict['sha256']}",
             data=self.prepare_put_payload(sample_dict),
-            headers={
-                "Accept": "application/json",
-                "Content-Type": "application/json",
-                "Authorization": "Bearer " + self.auth_token,
-            },
-        )
-        return json.loads(r.text)
+            headers=dict(self._default_headers, **{"Content-Type": "application/json"}),
+        ).json()
 
     def sample_delete(self, sha256):
         """Deletes sample observable. Requires authentication as admin"""
-        r = requests.delete(
-            self.endpoint + "/sample/" + sha256,
-            headers={
-                "Accept": "application/json",
-                "Authorization": "Bearer " + self.auth_token,
-            },
-        )
-        return json.loads(r.text)
-
-    def sample_get_by_md5(self, md5):
-        """Requests a sample by MD5"""
-        headers = {
-            "Accept": "application/json",
-        }
-        if self.auth_token:
-            headers["Authorization"] = "Bearer " + self.auth_token
-        r = requests.get(
-            self.endpoint + '/search?query=md5:"' + md5 + '"', headers=headers
-        )
-        return json.loads(r.text)
+        return requests.delete(
+            f"{self.endpoint}/sample/{sha256}", headers=self._default_headers
+        ).json()
 
     def search(
         self,
         query,
         fr=None,
         size=None,
         sort=None,
@@ -274,10 +238,11 @@
             params["format"] = format
 
         headers = {
             "Accept": "application/json",
         }
         if self.auth_token:
             headers["Authorization"] = "Bearer " + self.auth_token
-        r = requests.get(self.endpoint + "/search", params=params, headers=headers)
 
-        return json.loads(r.text)
+        return requests.get(
+            self.endpoint + "/search", params=params, headers=headers
+        ).json()
```

### Comparing `maltiverse-1.1.9/maltiverse/test_maltiverse.py` & `maltiverse-1.2.0/maltiverse/test_maltiverse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 
 import unittest
-import json
 from maltiverse import Maltiverse
 import time
 
 
 class TestMaltiverse(unittest.TestCase):
     """Test for Maltiverse class"""
```

### Comparing `maltiverse-1.1.9/maltiverse.egg-info/PKG-INFO` & `maltiverse-1.2.0/maltiverse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: maltiverse
-Version: 1.1.9
+Version: 1.2.0
 Summary: Wrapper for the Maltiverse API
-Author-email: Antonio Gomez <antonio.gomez@maltiverse.com>, Jorge Lopez <jorge.lopez@maltiverse.com>
+Home-page: https://github.com/maltiverse/maltiverse-python
+Download-URL: https://github.com/maltiverse/python-maltiverse/archive/master.zip
+Author: Antonio Gomez
+Author-email: Antonio Gomez <antonio.gomez@maltiverse.com>, Jorge Lopez <jorge.lopez@maltiverse.com>, Developers <dev@maltiverse.com>
 License: MIT License
         
         Copyright (c) 2017 maltiverse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -23,14 +26,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/maltiverse/python-maltiverse
 Project-URL: Bug Tracker, https://github.com/maltiverse/python-maltiverse/issues
+Keywords: maltiverse,API,threat intelligence,IoC,blacklist,search engine
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `maltiverse-1.1.9/pyproject.toml` & `maltiverse-1.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 name = "maltiverse"
-version = "1.1.9"
+version = "1.2.0"
 authors = [
   { name="Antonio Gomez", email="antonio.gomez@maltiverse.com" },
   { name="Jorge Lopez", email="jorge.lopez@maltiverse.com" },
+  { name="Developers", email="dev@maltiverse.com" },
 ]
 description = "Wrapper for the Maltiverse API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

