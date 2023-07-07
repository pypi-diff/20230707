# Comparing `tmp/threemystic_cloud_client-0.1.15.tar.gz` & `tmp/threemystic_cloud_client-0.1.16.tar.gz`

## Comparing `threemystic_cloud_client-0.1.15.tar` & `threemystic_cloud_client-0.1.16.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/token/__init__.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    21814 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/hatch.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/pyproject.toml
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cli/actions/token/__init__.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12196 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    21814 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/hatch.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/pyproject.toml
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.16/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cli/actions/token/__init__.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cli/actions/token/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,23 @@
           "--account": {
             "default": None, 
             "type": str,
             "dest": "token_account",
             "help": "The AWS Account ID to generate access token information for",
             "action": 'store'
           }
+        },
+        {
+          "--profile": {
+            "default": None, 
+            "type": str,
+            "dest": "token_profile",
+            "help": "The 3Mystic profile to use.",
+            "action": 'store'
+          }
         }
       ])
     )
 
 
     processed_info = self._process_options.process_opts(
       parser = parser
```

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-from threemystic_cloud_client.cloud_providers.aws.action_test.base_class.base import cloud_client_aws_test_base as base
+from threemystic_cloud_client.cloud_providers.aws.config.base_class.base import cloud_client_aws_config_base as base
 from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
+from threemystic_cloud_client.cloud_providers.aws.config.step_2 import cloud_client_aws_config_step_2 as nextstep
 
 
-class cloud_client_aws_test_step_1(base):
+class cloud_client_aws_config_step_1(base):
   def __init__(self, *args, **kwargs):
-    super().__init__(logger_name= "cloud_client_aws_test", *args, **kwargs)
+    super().__init__(logger_name= "cloud_client_aws_config_step_1", *args, **kwargs)
     
 
   def step(self, *args, **kwargs):
-    if not super().step( *args, **kwargs):
-      return
     
+    if not super().step(force_cli_installed_prompt= True):
+      return
     
     response = self.get_common().generate_data().generate(
       generate_data_config = {
-        "profile": {
-            "validation": lambda item: self.config_profile_name_exists( profile_name= item),
+        "type": {
+            "validation": lambda item: self.get_common().helper_type().bool().is_bool(check_value= item),
             "messages":{
-              "validation": f"Please enter a valid existing Cloud Client Profile",
+              "validation": f"Valid options for Yes are: {self.get_common().helper_type().bool().is_true_values()}",
             },
-            "conversion": lambda item: self.get_common().helper_type().string().set_case(string_value= self.get_common().helper_type().string().trim(string_value= item), case= "lower"),
-            "desc": f"What Cloud Client Profile to load",
+            "conversion": lambda item: self.get_common().helper_type().bool().is_true(check_value= item),
+            "desc": f"New Configuration\nValid optiond for yes: {self.get_common().helper_type().bool().is_true_values()}",
+            "default": True,
             "handler": generate_data_handlers.get_handler(handler= "base"),
-            "optional": True,
-            "default": self.get_default_profile_name()
+            "optional": True
         }
       }
     )
 
     if response is None:
       return
 
-    if not self.config_profile_name_exists(profile_name= response["profile"].get("formated")):
-      print(f"Profile Not Found: {response['profile'].get('formated')}")
-      return
-
-    from threemystic_cloud_client.cloud_providers.aws.action_test.step_2 import cloud_client_aws_test_step_2 as nextstep
-    nextstep(init_object = self).step( profile_name= response['profile'].get('formated'))
+    self.update_provider_config_completed(status= "step1")
+    nextstep(init_object = self).step(is_new_config= response["type"].get("formated") == True)
```

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,32 +64,36 @@
     
     self._aws_config_profile = self.__get_aws_cli_config()[f"profile {self.get_profile()['profile_data']['sso_profile_name']}"]
     self.__unset_aws_cli_config()
     return self._get_aws_sso_config_profile(*args, **kwargs)
   
   def _get_sso_profile_credentials(self, refresh = False, *args, **kwargs):   
     if(hasattr(self, "_aws_config_profile_credentials") and (not refresh)):
-      return self._aws_config_profile_credentials
+      if len(self._aws_config_profile_credentials) > 0:
+        return self._aws_config_profile_credentials
     
     cache_key = f'{self.get_common().encryption().hash(hash_method="sha1").generate_hash(data= self._get_aws_sso_config_profile(refresh= refresh)["sso_start_url"])}.json' 
     
     sso_token_file = self.get_aws_user_path().joinpath('sso', 'cache', cache_key)
     
+    self._aws_config_profile_credentials = {}
     if not self.get_common().helper_path().is_file(sso_token_file):
       raise self.get_common().exception().exception(
         exception_type = "generic"
       ).type_error(
         logger = self.get_common().get_logger(),
         name = f"NOT FOUND",
         message = f"Token File not found or not valid file: {sso_token_file}"
       )
-      
+    
     with sso_token_file.open(mode="r") as sso_cache:
       self._aws_config_profile_credentials = self.get_common().helper_json().loads(data= sso_cache.read())
 
+    return self._get_sso_profile_credentials()
+  
   def __internal_load_base_configs_ssoprofile(self, *args, **kwargs):
     self._get_sso_profile_credentials()
 
   def _get_session_accesstoken(self, refresh = False, *args, **kwargs):
     if self.session_expired():
       self.ensure_session()
 
@@ -101,20 +105,21 @@
     return self._get_session_accesstoken(refresh= refresh)
   
   def _get_session_expires(self, refresh = False, *args, **kwargs):
     if(hasattr(self, "_aws_config_profile_credentials_expires") and (not refresh)):
       return self._aws_config_profile_credentials_expires
 
     if(self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._get_sso_profile_credentials(refresh= refresh).get("expiresAt")) ):
-      return (self.get_common().helper_type().datetime().get() - self.get_common().helper_type().datetime().time_delta(totalSecondAddTime= 300))
+      return (self.get_common().helper_type().datetime().get() - self.get_common().helper_type().datetime().time_delta(seconds= 300))
     
-    self._aws_config_profile_credentials_expires = self.get_common().helper_type().datetime().convert_utc(
-      dt= (self.get_common().helper_type().datetime().parse_iso(iso_datetime_str= self._get_sso_profile_credentials().get("expiresAt")
-      - self.get_common().helper_type().datetime().time_delta(totalSecondAddTime= 300)))
+    self._aws_config_profile_credentials_expires = (self.get_common().helper_type().datetime().convert_utc(
+      dt= self.get_common().helper_type().datetime().parse_iso(iso_datetime_str= self._get_sso_profile_credentials().get("expiresAt")))
+      - self.get_common().helper_type().datetime().time_delta(seconds= 300)
     )
+
     return self._get_session_expires()
     
   def _session_expired(self, refresh = False, *args, **kwargs):
 
     return self.get_common().helper_type().datetime().is_token_expired_now(compare_datetime= self._get_session_expires(refresh= refresh))
```

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.16/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/.gitignore` & `threemystic_cloud_client-0.1.16/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/LICENSE` & `threemystic_cloud_client-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/README.md` & `threemystic_cloud_client-0.1.16/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/hatch.toml` & `threemystic_cloud_client-0.1.16/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.15/pyproject.toml` & `threemystic_cloud_client-0.1.16/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.5",
+  "threemystic-common >= 0.1.6",
   "polling2 >= 0.5.0",
   "typing-extensions >= 4.4.0",
   "pyopenssl >= 22.1.0",
   "PyJWT >= 2.7.0",
   "cryptography >= 41.0.1",
   "boto3 >= 1.26.151",
   "botocore >= 1.29.151",
```

### Comparing `threemystic_cloud_client-0.1.15/PKG-INFO` & `threemystic_cloud_client-0.1.16/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.15
+Version: 0.1.16
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 Requires-Dist: boto3>=1.26.151
 Requires-Dist: botocore>=1.29.151
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: cryptography>=41.0.1
 Requires-Dist: polling2>=0.5.0
 Requires-Dist: pyjwt>=2.7.0
 Requires-Dist: pyopenssl>=22.1.0
-Requires-Dist: threemystic-common>=0.1.5
+Requires-Dist: threemystic-common>=0.1.6
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_client
 A tool to help uniform the connection to the cloud providers.
 Currently supports AWS/Azure
```

