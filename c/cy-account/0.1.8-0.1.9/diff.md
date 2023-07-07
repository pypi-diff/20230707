# Comparing `tmp/cy_account-0.1.8.tar.gz` & `tmp/cy_account-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cy_account-0.1.8.tar", last modified: Sat Jul  1 16:09:31 2023, max compression
+gzip compressed data, was "cy_account-0.1.9.tar", last modified: Fri Jul  7 12:16:32 2023, max compression
```

## Comparing `cy_account-0.1.8.tar` & `cy_account-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 16:09:31.046296 cy_account-0.1.8/
--rw-rw-rw-   0        0        0      303 2023-07-01 16:09:31.046296 cy_account-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-07-01 03:33:37.000000 cy_account-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 16:09:31.021285 cy_account-0.1.8/cy_account/
--rw-rw-rw-   0        0        0     7438 2023-07-01 16:09:03.000000 cy_account-0.1.8/cy_account/__init__.py
--rw-rw-rw-   0        0        0      389 2023-06-26 16:40:06.000000 cy_account-0.1.8/cy_account/test.py
-drwxrwxrwx   0        0        0        0 2023-07-01 16:09:31.044294 cy_account-0.1.8/cy_account.egg-info/
--rw-rw-rw-   0        0        0      303 2023-07-01 16:09:30.000000 cy_account-0.1.8/cy_account.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-01 16:09:30.000000 cy_account-0.1.8/cy_account.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 16:09:30.000000 cy_account-0.1.8/cy_account.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-01 16:09:30.000000 cy_account-0.1.8/cy_account.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 16:09:30.000000 cy_account-0.1.8/cy_account.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 16:09:31.047288 cy_account-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-07-01 16:09:25.000000 cy_account-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:16:32.026576 cy_account-0.1.9/
+-rw-rw-rw-   0        0        0      303 2023-07-07 12:16:32.025575 cy_account-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-07-01 03:33:37.000000 cy_account-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 12:16:31.999578 cy_account-0.1.9/cy_account/
+-rw-rw-rw-   0        0        0     7527 2023-07-07 12:15:17.000000 cy_account-0.1.9/cy_account/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-07-07 12:15:41.000000 cy_account-0.1.9/cy_account/test.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:16:32.024572 cy_account-0.1.9/cy_account.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-07-07 12:16:31.000000 cy_account-0.1.9/cy_account.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-07 12:16:31.000000 cy_account-0.1.9/cy_account.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 12:16:31.000000 cy_account-0.1.9/cy_account.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-07 12:16:31.000000 cy_account-0.1.9/cy_account.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-07 12:16:31.000000 cy_account-0.1.9/cy_account.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 12:16:32.026576 cy_account-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-07-07 12:16:18.000000 cy_account-0.1.9/setup.py
```

### Comparing `cy_account-0.1.8/cy_account/__init__.py` & `cy_account-0.1.9/cy_account/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,18 +212,19 @@
 
     def get(self, server_name: str, path: str, query: dict = None):
         url = self.__get_url(server_name, path)
 
         response = requests.get(url=url, params=query, headers=self.__get_header())
         return self.__before(response)
 
-    def put(self, server_name: str, path: str, query: dict = None):
+    def put(self, server_name: str, path: str, query: dict = None, body: dict = None):
         url = self.__get_url(server_name, path)
+        body_str = json.dumps(body) if body else None
 
-        response = requests.put(url=url, params=query, headers=self.__get_header())
+        response = requests.put(url=url, params=query, data=body_str, headers=self.__get_header())
         return self.__before(response)
 
     def delete(self, server_name: str, path: str, query: dict = None):
         url = self.__get_url(server_name, path)
 
         response = requests.delete(url=url, params=query, headers=self.__get_header())
         return self.__before(response)
```

### Comparing `cy_account-0.1.8/setup.py` & `cy_account-0.1.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="cy_account",
-    version="0.1.8",
+    version="0.1.9",
     author="luyuan",
     author_email="136735431@qq.com",
     description="edited by myself",
     py_modules=["cy_account"],
     classifiers=["Programming Language :: Python :: 3",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent"],
```

