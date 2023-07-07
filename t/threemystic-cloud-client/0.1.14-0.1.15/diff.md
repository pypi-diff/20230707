# Comparing `tmp/threemystic_cloud_client-0.1.14.tar.gz` & `tmp/threemystic_cloud_client-0.1.15.tar.gz`

## Comparing `threemystic_cloud_client-0.1.14.tar` & `threemystic_cloud_client-0.1.15.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cli/actions/token/__init__.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12188 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    21766 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/hatch.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/pyproject.toml
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/token/__init__.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    21814 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/hatch.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cli/actions/token/__init__.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,62 +66,59 @@
     self.__unset_aws_cli_config()
     return self._get_aws_sso_config_profile(*args, **kwargs)
   
   def _get_sso_profile_credentials(self, refresh = False, *args, **kwargs):   
     if(hasattr(self, "_aws_config_profile_credentials") and (not refresh)):
       return self._aws_config_profile_credentials
     
-    cache_key = f'{self.get_common().encryption().hash(hash_method="sha1").generate_hash(data= self._get_aws_sso_config_profile(refresh= refresh)["sso_start_url"])}.json'    
+    cache_key = f'{self.get_common().encryption().hash(hash_method="sha1").generate_hash(data= self._get_aws_sso_config_profile(refresh= refresh)["sso_start_url"])}.json' 
     
-    ssoTokenFile = self.get_aws_user_path().joinpath('sso', 'cache', cache_key)
+    sso_token_file = self.get_aws_user_path().joinpath('sso', 'cache', cache_key)
     
-    if not self.get_common().helper_path().is_file(ssoTokenFile):
+    if not self.get_common().helper_path().is_file(sso_token_file):
       raise self.get_common().exception().exception(
         exception_type = "generic"
       ).type_error(
         logger = self.get_common().get_logger(),
         name = f"NOT FOUND",
-        message = f"Token File not found or not valid file: {ssoTokenFile}"
+        message = f"Token File not found or not valid file: {sso_token_file}"
       )
       
-    with ssoTokenFile.open(mode="r") as sso_cache:
+    with sso_token_file.open(mode="r") as sso_cache:
       self._aws_config_profile_credentials = self.get_common().helper_json().loads(data= sso_cache.read())
 
   def __internal_load_base_configs_ssoprofile(self, *args, **kwargs):
     self._get_sso_profile_credentials()
 
   def _get_session_accesstoken(self, refresh = False, *args, **kwargs):
     if self.session_expired():
       self.ensure_session()
 
     if(hasattr(self, "_aws_config_profile_credentials_accesstoken") and (not refresh)):
       if(not self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._aws_config_profile_credentials_accesstoken) ):
         return self._aws_config_profile_credentials_accesstoken
     
-    self._aws_config_profile_credentials_accesstoken = self._get_sso_profile_credentials()["accessToken"]
-    return self._get_session_accesstoken()
+    self._aws_config_profile_credentials_accesstoken = self._get_sso_profile_credentials().get("accessToken")
+    return self._get_session_accesstoken(refresh= refresh)
   
   def _get_session_expires(self, refresh = False, *args, **kwargs):
     if(hasattr(self, "_aws_config_profile_credentials_expires") and (not refresh)):
       return self._aws_config_profile_credentials_expires
 
-    if(self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._get_sso_profile_credentials()['expiresAt']) ):
+    if(self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._get_sso_profile_credentials(refresh= refresh).get("expiresAt")) ):
       return (self.get_common().helper_type().datetime().get() - self.get_common().helper_type().datetime().time_delta(totalSecondAddTime= 300))
     
     self._aws_config_profile_credentials_expires = self.get_common().helper_type().datetime().convert_utc(
-      dt= (self.get_common().helper_type().datetime().parse_iso(iso_datetime_str= self._get_sso_profile_credentials()['expiresAt']
+      dt= (self.get_common().helper_type().datetime().parse_iso(iso_datetime_str= self._get_sso_profile_credentials().get("expiresAt")
       - self.get_common().helper_type().datetime().time_delta(totalSecondAddTime= 300)))
     )
     return self._get_session_expires()
     
   def _session_expired(self, refresh = False, *args, **kwargs):
 
-    if(self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._get_sso_profile_credentials(refresh= refresh)['expiresAt']) ):
-      return True
-
     return self.get_common().helper_type().datetime().is_token_expired_now(compare_datetime= self._get_session_expires(refresh= refresh))
     
     
   def authenticate_session(self, *args, **kwargs):
     if(self.get_profile()['profile_data']['use_cli_profile']):
       self.__aws_sso_login_profile()
       return
```

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
 
     return self._assume_role(**kwargs)
   
   def session_expired(self, refresh = False, *args, **kwargs):
     return self._session_expired(refresh= refresh, *args, **kwargs)
   
   def ensure_session(self, count = 0, *args, **kwargs):
-    if(not self.session_expired(refresh = False if count == 0 else True)):
+    if(not self.session_expired()):
       return
     
     if count > 5:
       raise self.get_common().exception().exception(
         exception_type = "generic"
       ).type_error(
         logger = self.get_common().get_logger(),
@@ -305,14 +305,17 @@
   def is_authenticating_session(self, *args, **kwargs):
     if(hasattr(self, "_is_authenticating_session")):
       return self._is_authenticating_session
     
     return False
   
   def _set_authenticating_session(self, is_authenticating_session, *args, **kwargs):
+    if not is_authenticating_session:
+      self.session_expired(refresh= True)
+      
     self._is_authenticating_session = is_authenticating_session
     return self.is_authenticating_session()
 
   def _get_organization_client(self, *args, **kwargs):   
     if hasattr(self, "_org_client"):
       return self._org_client
```

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/.gitignore` & `threemystic_cloud_client-0.1.15/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/LICENSE` & `threemystic_cloud_client-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/README.md` & `threemystic_cloud_client-0.1.15/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/hatch.toml` & `threemystic_cloud_client-0.1.15/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/pyproject.toml` & `threemystic_cloud_client-0.1.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.14/PKG-INFO` & `threemystic_cloud_client-0.1.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.14
+Version: 0.1.15
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

