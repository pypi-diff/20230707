# Comparing `tmp/revChatGPT-6.7.6.tar.gz` & `tmp/revChatGPT-6.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.7.6.tar", last modified: Sun Jul  2 09:36:31 2023, max compression
+gzip compressed data, was "revChatGPT-6.7.7.tar", last modified: Fri Jul  7 14:52:28 2023, max compression
```

## Comparing `revChatGPT-6.7.6.tar` & `revChatGPT-6.7.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 09:36:31.292034 revChatGPT-6.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    60775 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:28.878790 revChatGPT-6.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-07 14:52:28.878790 revChatGPT-6.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-07 14:52:28.000000 revChatGPT-6.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 14:52:28.878790 revChatGPT-6.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:28.870789 revChatGPT-6.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:28.874790 revChatGPT-6.7.7/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    60820 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:28.874790 revChatGPT-6.7.7/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:28.874790 revChatGPT-6.7.7/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-07 14:52:28.000000 revChatGPT-6.7.7/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-07 14:52:28.000000 revChatGPT-6.7.7/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:52:28.000000 revChatGPT-6.7.7/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-07 14:52:28.000000 revChatGPT-6.7.7/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 14:52:28.000000 revChatGPT-6.7.7/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:28.874790 revChatGPT-6.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 14:51:58.000000 revChatGPT-6.7.7/tests/test_recipient.py
```

### Comparing `revChatGPT-6.7.6/LICENSE` & `revChatGPT-6.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.6/PKG-INFO` & `revChatGPT-6.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.6
+Version: 6.7.7
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.6/README.md` & `revChatGPT-6.7.7/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.6/setup.py` & `revChatGPT-6.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.6/src/revChatGPT/V1.py` & `revChatGPT-6.7.7/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,17 +163,18 @@
 
     Challenge details:
         game_type: str - Audio or Image
         instructions: str - Instructions for the captcha
         URLs: list[str] - URLs of the images or audio files
     """
     resp = requests.get(
-        (CAPTCHA_URL + "start?download_images=true")
-        if download_images
-        else CAPTCHA_URL + "start",
+        "https://arkose-token.tms.im/"
+        # (CAPTCHA_URL + "start?download_images=true")
+        # if download_images
+        # else CAPTCHA_URL + "start",
     )
     resp_json: dict = resp.json()
     if resp.status_code == 200:
         return resp_json.get("token")
     if resp.status_code != 511:
         raise Exception(resp_json.get("error", "Unknown error"))
```

### Comparing `revChatGPT-6.7.6/src/revChatGPT/V3.py` & `revChatGPT-6.7.7/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.6/src/revChatGPT/__init__.py` & `revChatGPT-6.7.7/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.6/src/revChatGPT/__main__.py` & `revChatGPT-6.7.7/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.6/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.7.7/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.6/src/revChatGPT/typings.py` & `revChatGPT-6.7.7/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.6/src/revChatGPT/utils.py` & `revChatGPT-6.7.7/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.6/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.7.7/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.6
+Version: 6.7.7
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.6/tests/test_recipient.py` & `revChatGPT-6.7.7/tests/test_recipient.py`

 * *Files identical despite different names*

