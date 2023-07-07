# Comparing `tmp/threemystic_cloud_client-0.1.18.tar.gz` & `tmp/threemystic_cloud_client-0.1.19.tar.gz`

## Comparing `threemystic_cloud_client-0.1.18.tar` & `threemystic_cloud_client-0.1.19.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cli/actions/token/__init__.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    21819 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/hatch.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/pyproject.toml
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.18/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/token/__init__.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    21814 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/hatch.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/pyproject.toml
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.19/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,19 @@
     if not hasattr(self, "_client"):
       self._client = {}
 
     if self._client.get(provider) is not None:
       return
 
     if provider == "azure":
-      self.__set_provider_azure(provider= provider)
+      self.__set_provider_azure(provider= provider, *args, **kwargs)
       return
     
     if provider == "aws":
-      self.__set_provider_aws(provider= provider)
+      self.__set_provider_aws(provider= provider, *args, **kwargs)
       return  
        
     raise self.get_common().exception().exception(
       exception_type = "argument"
     ).not_implemented(
       logger = self.get_common().get_logger(),
       name = "provider",
```

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cli/actions/token/__init__.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cli/actions/token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,12 +21,18 @@
 
   def action_config(self, *args, **kwargs):     
     from threemystic_cloud_client.cloud_providers.aws.config.step_1 import cloud_client_aws_config_step_1 as step
     next_step = step(common= self.get_common(), logger= self.get_logger())
     
     next_step.step()
 
+  def action_token(self, *args, **kwargs):     
+    from threemystic_cloud_client.cloud_providers.aws.action_token.step_1 import cloud_client_aws_token_step_1 as step
+    next_step = step(common= self.get_common(), logger= self.get_logger())
+    
+    next_step.step()
+
```

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     if account is None or (self.get_common().helper_type().general().is_type(obj= account, type_check= str) and self.get_common().helper_type().string().is_null_or_whitespace(string_value= account)):
       account = self.get_default_account()
 
     return f'{self.get_account_id(account= account)}_{role}'
 
   def _get_assumed_role_credentials(self, *args, **kwargs):
-    if(not hasattr(self, "_assumed_role_credentials")):
+    if(hasattr(self, "_assumed_role_credentials")):
       return self._assumed_role_credentials
     
     self._assumed_role_credentials = {}
     return self._get_assumed_role_credentials()
     
   def get_profile(self, *args, **kwargs):
     if(not hasattr(self, "_profile")):
@@ -262,15 +262,15 @@
     
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
```

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     self._process_cli_args()
     
   def _process_cli_args(self, *args, **kwargs):
     process_options = base_process_options(common= self.get_common())
     token_parser_args = {   }
     self._arg_parser = process_options.get_parser(
       parser_init_kwargs = {
-        "prog": "3mystic_cloud_client -p azure --token",
+        "prog": "3mystic_cloud_client --token -p azure",
         "formatter_class": argparse.RawDescriptionHelpFormatter,
         "description": textwrap.dedent('''\
         Requires additional settings.
           --tenant is required
           --resource is required
 
           To learn more please see: https://learn.microsoft.com/en-us/cli/azure/account?view=azure-cli-latest#az-account-get-access-token
```

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.19/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/.gitignore` & `threemystic_cloud_client-0.1.19/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/LICENSE` & `threemystic_cloud_client-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/README.md` & `threemystic_cloud_client-0.1.19/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/hatch.toml` & `threemystic_cloud_client-0.1.19/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/pyproject.toml` & `threemystic_cloud_client-0.1.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.18/PKG-INFO` & `threemystic_cloud_client-0.1.19/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.18
+Version: 0.1.19
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

