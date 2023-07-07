# Comparing `tmp/activecampaign_python-1.0.7.tar.gz` & `tmp/activecampaign_python-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activecampaign_python-1.0.7.tar", max compression
+gzip compressed data, was "activecampaign_python-1.0.8.tar", max compression
```

## Comparing `activecampaign_python-1.0.7.tar` & `activecampaign_python-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1065 2023-03-27 20:59:00.982544 activecampaign_python-1.0.7/LICENSE
--rw-r--r--   0        0        0    15391 2023-06-23 13:30:45.288998 activecampaign_python-1.0.7/README.md
--rw-r--r--   0        0        0        0 2023-03-27 20:59:00.982882 activecampaign_python-1.0.7/activecampaign/__init__.py
--rw-r--r--   0        0        0      245 2023-03-27 20:59:00.983020 activecampaign_python-1.0.7/activecampaign/automations.py
--rw-r--r--   0        0        0     2208 2023-06-23 13:30:45.289185 activecampaign_python-1.0.7/activecampaign/client.py
--rw-r--r--   0        0        0     5856 2023-03-27 20:59:00.983212 activecampaign_python-1.0.7/activecampaign/contacts.py
--rw-r--r--   0        0        0     6205 2023-06-23 13:30:45.289308 activecampaign_python-1.0.7/activecampaign/customobjects.py
--rw-r--r--   0        0        0      255 2023-03-27 20:59:00.983313 activecampaign_python-1.0.7/activecampaign/dealActivities.py
--rw-r--r--   0        0        0     4374 2023-03-27 20:59:00.983429 activecampaign_python-1.0.7/activecampaign/deals.py
--rw-r--r--   0        0        0     3782 2023-03-27 20:59:00.983524 activecampaign_python-1.0.7/activecampaign/deepdataintegrations.py
--rw-r--r--   0        0        0      258 2023-03-27 20:59:00.983601 activecampaign_python-1.0.7/activecampaign/emailActivities.py
--rw-r--r--   0        0        0       86 2023-03-27 20:59:00.983691 activecampaign_python-1.0.7/activecampaign/exception.py
--rw-r--r--   0        0        0     1485 2023-03-27 20:59:00.983787 activecampaign_python-1.0.7/activecampaign/lists.py
--rw-r--r--   0        0        0      268 2023-03-27 20:59:00.983875 activecampaign_python-1.0.7/activecampaign/messages.py
--rw-r--r--   0        0        0     1165 2023-03-27 20:59:00.983965 activecampaign_python-1.0.7/activecampaign/notes.py
--rw-r--r--   0        0        0     1099 2023-03-27 20:59:00.984046 activecampaign_python-1.0.7/activecampaign/tags.py
--rw-r--r--   0        0        0     1157 2023-03-27 20:59:00.984140 activecampaign_python-1.0.7/activecampaign/tasks.py
--rw-r--r--   0        0        0     2148 2023-03-27 20:59:00.984242 activecampaign_python-1.0.7/activecampaign/users.py
--rw-r--r--   0        0        0     1380 2023-03-27 20:59:00.984331 activecampaign_python-1.0.7/activecampaign/webhooks.py
--rw-r--r--   0        0        0      415 2023-06-23 13:30:45.290732 activecampaign_python-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    16052 1970-01-01 00:00:00.000000 activecampaign_python-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-27 20:59:00.982544 activecampaign_python-1.0.8/LICENSE
+-rw-r--r--   0        0        0    15391 2023-06-23 13:30:45.288998 activecampaign_python-1.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 20:59:00.982882 activecampaign_python-1.0.8/activecampaign/__init__.py
+-rw-r--r--   0        0        0      245 2023-03-27 20:59:00.983020 activecampaign_python-1.0.8/activecampaign/automations.py
+-rw-r--r--   0        0        0      457 2023-07-07 13:57:13.984494 activecampaign_python-1.0.8/activecampaign/campaigns.py
+-rw-r--r--   0        0        0     2281 2023-07-07 13:57:13.984688 activecampaign_python-1.0.8/activecampaign/client.py
+-rw-r--r--   0        0        0     5856 2023-03-27 20:59:00.983212 activecampaign_python-1.0.8/activecampaign/contacts.py
+-rw-r--r--   0        0        0     6205 2023-06-23 13:30:45.289308 activecampaign_python-1.0.8/activecampaign/customobjects.py
+-rw-r--r--   0        0        0      255 2023-03-27 20:59:00.983313 activecampaign_python-1.0.8/activecampaign/dealActivities.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:59:00.983429 activecampaign_python-1.0.8/activecampaign/deals.py
+-rw-r--r--   0        0        0     3782 2023-03-27 20:59:00.983524 activecampaign_python-1.0.8/activecampaign/deepdataintegrations.py
+-rw-r--r--   0        0        0      258 2023-03-27 20:59:00.983601 activecampaign_python-1.0.8/activecampaign/emailActivities.py
+-rw-r--r--   0        0        0       86 2023-03-27 20:59:00.983691 activecampaign_python-1.0.8/activecampaign/exception.py
+-rw-r--r--   0        0        0     1485 2023-03-27 20:59:00.983787 activecampaign_python-1.0.8/activecampaign/lists.py
+-rw-r--r--   0        0        0      268 2023-03-27 20:59:00.983875 activecampaign_python-1.0.8/activecampaign/messages.py
+-rw-r--r--   0        0        0     1165 2023-03-27 20:59:00.983965 activecampaign_python-1.0.8/activecampaign/notes.py
+-rw-r--r--   0        0        0     1099 2023-03-27 20:59:00.984046 activecampaign_python-1.0.8/activecampaign/tags.py
+-rw-r--r--   0        0        0     1157 2023-03-27 20:59:00.984140 activecampaign_python-1.0.8/activecampaign/tasks.py
+-rw-r--r--   0        0        0     2148 2023-03-27 20:59:00.984242 activecampaign_python-1.0.8/activecampaign/users.py
+-rw-r--r--   0        0        0     1380 2023-03-27 20:59:00.984331 activecampaign_python-1.0.8/activecampaign/webhooks.py
+-rw-r--r--   0        0        0      415 2023-07-07 13:57:23.096302 activecampaign_python-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0    16052 1970-01-01 00:00:00.000000 activecampaign_python-1.0.8/PKG-INFO
```

### Comparing `activecampaign_python-1.0.7/LICENSE` & `activecampaign_python-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/README.md` & `activecampaign_python-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/activecampaign/client.py` & `activecampaign_python-1.0.8/activecampaign/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .users import Users
 from .webhooks import Webhooks
 from .messages import Messages
 from .tags import Tags
 from .emailActivities import EmailActivities
 from .dealActivities import DealActivities
 from .customobjects import CustomObjects
-
+from .campaigns import Campaigns
 
 class Client(object):
     BASE_URL = '{}/api/3'
 
     def __init__(self, url, api_key):
         self.BASE_URL = self.BASE_URL.format(url)
         self.api_key = api_key
@@ -33,14 +33,15 @@
         self.webhooks = Webhooks(self)
         self.messages = Messages(self)
         self.deepdataintegrations = DeepDataIntegrations(self)
         self.tags = Tags(self)
         self.emailActivities = EmailActivities(self)
         self.dealActivities = DealActivities(self)
         self.customobjects = CustomObjects(self)
+        self.campaigns = Campaigns(self)
 
     def _get(self, endpoint, **kwargs):
         return self._request('GET', endpoint, **kwargs)
 
     def _post(self, endpoint, **kwargs):
         return self._request('POST', endpoint, **kwargs)
```

### Comparing `activecampaign_python-1.0.7/activecampaign/contacts.py` & `activecampaign_python-1.0.8/activecampaign/contacts.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/activecampaign/customobjects.py` & `activecampaign_python-1.0.8/activecampaign/customobjects.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/activecampaign/deals.py` & `activecampaign_python-1.0.8/activecampaign/deals.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/activecampaign/deepdataintegrations.py` & `activecampaign_python-1.0.8/activecampaign/deepdataintegrations.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/activecampaign/lists.py` & `activecampaign_python-1.0.8/activecampaign/lists.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/activecampaign/notes.py` & `activecampaign_python-1.0.8/activecampaign/notes.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/activecampaign/tags.py` & `activecampaign_python-1.0.8/activecampaign/tags.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/activecampaign/tasks.py` & `activecampaign_python-1.0.8/activecampaign/tasks.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/activecampaign/users.py` & `activecampaign_python-1.0.8/activecampaign/users.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/activecampaign/webhooks.py` & `activecampaign_python-1.0.8/activecampaign/webhooks.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.7/PKG-INFO` & `activecampaign_python-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activecampaign-python
-Version: 1.0.7
+Version: 1.0.8
 Summary: API wrapper for ActiveCampaign written in Python
 License: MIT
 Author: Miguel Ferrer
 Author-email: ingferrermiguel@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

