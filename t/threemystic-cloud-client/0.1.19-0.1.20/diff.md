# Comparing `tmp/threemystic_cloud_client-0.1.19.tar.gz` & `tmp/threemystic_cloud_client-0.1.20.tar.gz`

## Comparing `threemystic_cloud_client-0.1.19.tar` & `threemystic_cloud_client-0.1.20.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/token/__init__.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    21814 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/hatch.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/pyproject.toml
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cli/actions/token/__init__.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12270 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    22018 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/hatch.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.20/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/token/__init__.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cli/actions/token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,38 +228,42 @@
     return self.make_account(Id = self._get_aws_sso_config_profile()["sso_account_id"])
   
   def __get_sso_boto_session(self):
     return boto3.Session(
       profile_name = self.get_profile()['profile_data']['sso_profile_name']
     )
   
-  def _assume_role(self, account = None, region = None, role = None, force_refresh= False, *args, **kwargs):
+  def _assume_role(self, account = None, region = None, role = None, refresh= False, *args, **kwargs):
         
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= role):
       role = self.get_default_rolename()
     
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= region):
-        region = self.get_default_region()
+      region = self.get_default_region()
 
     if account is None or (self.get_common().helper_type().general().is_type(obj= account, type_check= str) and self.get_common().helper_type().string().is_null_or_whitespace(string_value= account)):
-        account = self.get_default_account()
-    
-    if not force_refresh and self._get_assumed_role_credentials().get(self._get_assumed_role_credentials_key(account= account, role= role)) is not None:
-        experation = self._get_assumed_role_credentials()[self._get_assumed_role_credentials_key(account= account, role= role)]["Credentials"]["Expiration"]
-        if self.get_common().helper_type().general().is_type(obj= experation, type_check= str):
-            experation = self.get_common().helper_type().datetime().parse_iso(iso_datetime_str=experation)
+      account = self.get_default_account()
+
+    if not refresh and self._get_assumed_role_credentials().get(self._get_assumed_role_credentials_key(account= account, role= role)) is not None:
+      experation = self._get_assumed_role_credentials()[self._get_assumed_role_credentials_key(account= account, role= role)]["Credentials"]["Expiration"]
+      if self.get_common().helper_type().general().is_type(obj= experation, type_check= str):
+        experation = self.get_common().helper_type().datetime().parse_iso(iso_datetime_str=experation)
 
-            if not self.get_common().helper_type().datetime().is_token_expired_now(compare_datetime= experation):
-                return self._get_assumed_role_credentials()[self._get_assumed_role_credentials_key(account= account, role= role)]["Credentials"]
+        if not self.get_common().helper_type().datetime().is_token_expired_now(compare_datetime= experation):
+          return self._get_assumed_role_credentials()[self._get_assumed_role_credentials_key(account= account, role= role)]["Credentials"]
     
     self._get_assumed_role_credentials()[self._get_assumed_role_credentials_key(account= account, role= role)] = self.__get_sso_boto_session().client('sso').get_role_credentials(
       roleName=role,
       accountId=self.get_account_id(account= account),
       accessToken=self._get_session_accesstoken()
     )
+
+    return self._assume_role(
+      account = account, region = region, role = role, *args, **kwargs
+    )
                 
   
   def get_main_account_id(self, *args, **kwargs):
     return self.get_account_id(account= self.get_default_account())
 
   def get_organization_account_id(self, *args, **kwargs):
     return self.get_account_id(account= self.get_default_account())
```

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,21 @@
       role = self.get_default_rolename()
 
     if account is None or (self.get_common().helper_type().general().is_type(obj= account, type_check= str) and self.get_common().helper_type().string().is_null_or_whitespace(string_value= account)):
       account = self.get_default_account()
 
     return f'{self.get_account_id(account= account)}_{role}'
 
-  def _get_assumed_role_credentials(self, *args, **kwargs):
+  def _get_assumed_role_credentials(self, unset = False, *args, **kwargs):
     if(hasattr(self, "_assumed_role_credentials")):
+      if unset:
+        current = self._assumed_role_credentials
+        delattr(self, "_assumed_role_credentials")
+        return current
+      
       return self._assumed_role_credentials
     
     self._assumed_role_credentials = {}
     return self._get_assumed_role_credentials()
     
   def get_profile(self, *args, **kwargs):
     if(not hasattr(self, "_profile")):
@@ -262,15 +267,15 @@
     
     self._organization_account = self.make_account(Id = self.get_organization_account_id())
     return self.get_organization_account()
 
   def assume_role(self, *args, **kwargs):
     self.ensure_session()
     if kwargs.get("account") is not None and self.get_common().helper_type().general().is_type(obj= kwargs["account"], type_check= str):
-      kwargs["account"] = self.make_account(Id= kwargs["account"])     
+      kwargs["account"] = self.make_account(Id= kwargs["account"]) 
 
     return self._assume_role(**kwargs)
   
   def session_expired(self, refresh = False, *args, **kwargs):
     return self._session_expired(refresh= refresh, *args, **kwargs)
   
   def ensure_session(self, count = 0, *args, **kwargs):
@@ -306,27 +311,28 @@
     if(hasattr(self, "_is_authenticating_session")):
       return self._is_authenticating_session
     
     return False
   
   def _set_authenticating_session(self, is_authenticating_session, *args, **kwargs):
     if not is_authenticating_session:
+      self._get_assumed_role_credentials(unset= True)
       self.session_expired(refresh= True)
       
     self._is_authenticating_session = is_authenticating_session
     return self.is_authenticating_session()
 
   def _get_organization_client(self, *args, **kwargs):   
     if hasattr(self, "_org_client"):
       return self._org_client
     
     self._org_client = self.get_boto_client(
       client= 'organizations', 
       account=self.get_organization_account(),
-      role = None, 
+      role = None,
       region = None
     )
     return self._get_organization_client()
 
   
   def get_boto_config(self, region= None, max_attempts = 10, read_timeout = 900, connect_timeout = 10, max_pool_connections = 20,   *argv, **kwargs):
     config = botocore_config_config(
@@ -409,15 +415,15 @@
 
     session = self.__get_boto_session(
       account=account, role = role, region = region, profile = profile
     )     
 
     credentials = botocore_credentials.RefreshableCredentials.create_from_metadata(
       metadata=self._convert_assume_role_credentials_boto_session(self.assume_role(account=account, role=role)),
-      refresh_using=lambda: self._convert_assume_role_credentials_boto_session(self.assume_role(account=account, role=role, force_refresh= True)),
+      refresh_using=lambda: self._convert_assume_role_credentials_boto_session(self.assume_role(account=account, role=role, refresh= True)),
       method="sts-assume-role",
     )
 
     session._credentials = credentials 
     session.set_config_variable("region", region)
       
     self._get_created_boto_sessions()[cache_key] = boto_session(botocore_session= session)
```

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.20/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/.gitignore` & `threemystic_cloud_client-0.1.20/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/LICENSE` & `threemystic_cloud_client-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/README.md` & `threemystic_cloud_client-0.1.20/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/hatch.toml` & `threemystic_cloud_client-0.1.20/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/pyproject.toml` & `threemystic_cloud_client-0.1.20/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.19/PKG-INFO` & `threemystic_cloud_client-0.1.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.19
+Version: 0.1.20
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

