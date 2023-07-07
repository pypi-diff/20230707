# Comparing `tmp/pysigsci-3.8.0-py2.py3-none-any.whl.zip` & `tmp/pysigsci-3.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 27606 bytes, number of entries: 14
--rw-r--r--  2.0 unx       65 b- defN 20-May-26 20:28 pysigsci/__init__.py
+Zip file size: 27612 bytes, number of entries: 14
+-rw-r--r--  2.0 unx       65 b- defN 20-May-28 18:35 pysigsci/__init__.py
 -rw-r--r--  2.0 unx       62 b- defN 19-Jan-16 02:48 pysigsci/powerrules/__init__.py
 -rw-r--r--  2.0 unx     8996 b- defN 19-Jan-16 02:48 pysigsci/powerrules/powerrules.py
 -rw-r--r--  2.0 unx      199 b- defN 19-Sep-04 18:52 pysigsci/releases/__init__.py
 -rw-r--r--  2.0 unx     1038 b- defN 19-Sep-04 18:52 pysigsci/releases/releases.py
 -rw-r--r--  2.0 unx      848 b- defN 20-May-26 20:22 pysigsci/sigsciapi/__init__.py
--rw-r--r--  2.0 unx    52792 b- defN 20-May-22 17:22 pysigsci/sigsciapi/sigsciapi.py
--rwxr-xr-x  2.0 unx    13076 b- defN 20-May-01 19:25 pysigsci-3.8.0.data/scripts/pysigsci
--rwxr-xr-x  2.0 unx     9059 b- defN 20-Feb-27 20:27 pysigsci-3.8.0.data/scripts/pysigscia
--rw-r--r--  2.0 unx    35147 b- defN 20-May-26 20:30 pysigsci-3.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1975 b- defN 20-May-26 20:30 pysigsci-3.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 20-May-26 20:30 pysigsci-3.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 20-May-26 20:30 pysigsci-3.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1177 b- defN 20-May-26 20:30 pysigsci-3.8.0.dist-info/RECORD
-14 files, 124553 bytes uncompressed, 25640 bytes compressed:  79.4%
+-rw-r--r--  2.0 unx    52819 b- defN 20-May-28 18:32 pysigsci/sigsciapi/sigsciapi.py
+-rwxr-xr-x  2.0 unx    13076 b- defN 20-May-01 19:25 pysigsci-3.9.0.data/scripts/pysigsci
+-rwxr-xr-x  2.0 unx     9059 b- defN 20-Feb-27 20:27 pysigsci-3.9.0.data/scripts/pysigscia
+-rw-r--r--  2.0 unx    35147 b- defN 20-May-28 18:36 pysigsci-3.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1975 b- defN 20-May-28 18:36 pysigsci-3.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 20-May-28 18:36 pysigsci-3.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 20-May-28 18:36 pysigsci-3.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1177 b- defN 20-May-28 18:36 pysigsci-3.9.0.dist-info/RECORD
+14 files, 124580 bytes uncompressed, 25646 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -15,29 +15,29 @@
 
 Filename: pysigsci/sigsciapi/__init__.py
 Comment: 
 
 Filename: pysigsci/sigsciapi/sigsciapi.py
 Comment: 
 
-Filename: pysigsci-3.8.0.data/scripts/pysigsci
+Filename: pysigsci-3.9.0.data/scripts/pysigsci
 Comment: 
 
-Filename: pysigsci-3.8.0.data/scripts/pysigscia
+Filename: pysigsci-3.9.0.data/scripts/pysigscia
 Comment: 
 
-Filename: pysigsci-3.8.0.dist-info/LICENSE
+Filename: pysigsci-3.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: pysigsci-3.8.0.dist-info/METADATA
+Filename: pysigsci-3.9.0.dist-info/METADATA
 Comment: 
 
-Filename: pysigsci-3.8.0.dist-info/WHEEL
+Filename: pysigsci-3.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: pysigsci-3.8.0.dist-info/top_level.txt
+Filename: pysigsci-3.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pysigsci-3.8.0.dist-info/RECORD
+Filename: pysigsci-3.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pysigsci/__init__.py

```diff
@@ -1,3 +1,3 @@
 """The version string for this application"""
 
-VERSION = "3.8.0"
+VERSION = "3.9.0"
```

## pysigsci/sigsciapi/sigsciapi.py

```diff
@@ -11,14 +11,15 @@
     Class for Signal Sciences API
     """
     base_url = "https://dashboard.signalsciences.net/api/"
     api_version = "v0"
     bearer_token = None
     api_user = None
     api_token = None
+    headers = dict()
     cookies = None
     corp = None
     site = None
 
     # endpoints
     ep_auth = "/auth"
     ep_auth_logout = ep_auth + "/logout"
@@ -37,15 +38,15 @@
 
     def _make_request(self,
                       endpoint,
                       params=None,
                       data=None,
                       json=None,
                       method="GET"):
-        headers = dict()
+        headers = self.headers
         cookies = None
 
         if endpoint != self.ep_auth and self.bearer_token is not None:
             headers["Authorization"] = "Bearer {}".format(self.bearer_token['token'])
         elif endpoint != self.ep_auth:
             headers["X-Api-User"] = self.api_user
             headers['X-Api-Token'] = self.api_token
```

## Comparing `pysigsci-3.8.0.data/scripts/pysigsci` & `pysigsci-3.9.0.data/scripts/pysigsci`

 * *Files identical despite different names*

## Comparing `pysigsci-3.8.0.data/scripts/pysigscia` & `pysigsci-3.9.0.data/scripts/pysigscia`

 * *Files identical despite different names*

## Comparing `pysigsci-3.8.0.dist-info/LICENSE` & `pysigsci-3.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pysigsci-3.8.0.dist-info/METADATA` & `pysigsci-3.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigsci
-Version: 3.8.0
+Version: 3.9.0
 Summary: A python wrapper for the Signal Sciences API - https://docs.signalsciences.net/api/
 Home-page: https://github.com/foospidy/pysigsci
 Author: foospidy
 Author-email: UNKNOWN
 License: MIT
 Download-URL: https://github.com/foospidy/pysigsci
 Keywords: wrapper library signal sciences sigsci pysigsci api cli
```

## Comparing `pysigsci-3.8.0.dist-info/RECORD` & `pysigsci-3.9.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-pysigsci/__init__.py,sha256=wTO9YQGrN5JbXIVw7hb7YJecwVmuGpd2lsUlhb-4isA,65
+pysigsci/__init__.py,sha256=aFl8h2WxZfb-G55945MRtLegblOXFlHAH6TZvcYilTc,65
 pysigsci/powerrules/__init__.py,sha256=bigDnXBnIieSQ_8Wp-7nHqsB6v42l3FXRCzXQG6iXc0,62
 pysigsci/powerrules/powerrules.py,sha256=adCc9i3UAeEId09ndBNzkzD4rR-Ox-PA2THmGE4_r7o,8996
 pysigsci/releases/__init__.py,sha256=nAjfh0S064z-3-r5oViiHZuADQJKN8jNC4FsUElOrus,199
 pysigsci/releases/releases.py,sha256=VuKbnH1d_0JZ1Na69uCaWCa0h85TmxMooNJ-8s31UXI,1038
 pysigsci/sigsciapi/__init__.py,sha256=QH1zOQ3IMDje_-aCpirW6JHHPtjmhW5o__Ia800AZN0,848
-pysigsci/sigsciapi/sigsciapi.py,sha256=Dj1Ts1EUxGruIu6ZzzJAjR4_wgYfyOoTX4AzE3KudMI,52792
-pysigsci-3.8.0.data/scripts/pysigsci,sha256=sbyLqawwegYxsjft2vbXBlBU2oRgzG9DCs1Tac1vkzA,13076
-pysigsci-3.8.0.data/scripts/pysigscia,sha256=MFfaFCVMutgRK_EItHMfu5hRycilqIvI1fX0GluIXKc,9059
-pysigsci-3.8.0.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
-pysigsci-3.8.0.dist-info/METADATA,sha256=1YHEqKrkE_zmyFaTu-IyG7g5X8Yoau4nb2RQKnfRAGI,1975
-pysigsci-3.8.0.dist-info/WHEEL,sha256=_wJFdOYk7i3xxT8ElOkUJvOdOvfNGbR9g-bf6UQT6sU,110
-pysigsci-3.8.0.dist-info/top_level.txt,sha256=LP_vBhm7qge-_nVktRem2mYuGd5aT_yrUXWRqnVpEuQ,9
-pysigsci-3.8.0.dist-info/RECORD,,
+pysigsci/sigsciapi/sigsciapi.py,sha256=qNMuWi8vuslNTvq9j2yn8OGq4F5JMqxKRPAy__p-SW0,52819
+pysigsci-3.9.0.data/scripts/pysigsci,sha256=sbyLqawwegYxsjft2vbXBlBU2oRgzG9DCs1Tac1vkzA,13076
+pysigsci-3.9.0.data/scripts/pysigscia,sha256=MFfaFCVMutgRK_EItHMfu5hRycilqIvI1fX0GluIXKc,9059
+pysigsci-3.9.0.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
+pysigsci-3.9.0.dist-info/METADATA,sha256=CDLVMFUbOf1x1as8jxZLr8ciMd29y7Y_L_ojEvwhyEs,1975
+pysigsci-3.9.0.dist-info/WHEEL,sha256=_wJFdOYk7i3xxT8ElOkUJvOdOvfNGbR9g-bf6UQT6sU,110
+pysigsci-3.9.0.dist-info/top_level.txt,sha256=LP_vBhm7qge-_nVktRem2mYuGd5aT_yrUXWRqnVpEuQ,9
+pysigsci-3.9.0.dist-info/RECORD,,
```

