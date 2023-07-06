# Comparing `tmp/threemystic_cloud_client-0.1.8.tar.gz` & `tmp/threemystic_cloud_client-0.1.9.tar.gz`

## Comparing `threemystic_cloud_client-0.1.8.tar` & `threemystic_cloud_client-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cli/actions/test_config/__init__.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cli/actions/token/__init__.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    21260 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/test_config/step_1.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/test_config/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/test_config/base_class/base.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0    13977 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    15338 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/test_config/step_1.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/test_config/base_class/base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/hatch.toml
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cli/actions/test/__init__.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cli/actions/token/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    21260 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/test/step_1.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0    13977 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    15338 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/test/step_1.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/hatch.toml
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.9/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     
     if force_action == "config":
       from threemystic_cloud_client.cli.actions.config import cloud_client_config as user_action
       user_action(cloud_client= self._cloud_client).main(provider= self._client_provider)
       return
 
     if force_action == "test":
-      from threemystic_cloud_client.cli.actions.test_config import cloud_client_test as user_action
+      from threemystic_cloud_client.cli.actions.test import cloud_client_test as user_action
       user_action(cloud_client= self._cloud_client).main(provider= self._client_provider)
       return
 
     if force_action == "token":
       from threemystic_cloud_client.cli.actions.token import cloud_client_token as user_action
       user_action(cloud_client= self._cloud_client).main(provider= self._client_provider)
       return
```

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cli/actions/test_config/__init__.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cli/actions/test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cli/actions/token/__init__.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cli/actions/token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from threemystic_cloud_client.cloud_providers.aws.base_class.base import cloud_client_provider_aws_base as base
+from threemystic_cloud_client.cloud_providers.azure.base_class.base import cloud_client_provider_azure_base as base
 
-
-class cloud_client_aws(base):
+class cloud_client_azure(base):
   def __init__(self, *args, **kwargs):
-    super().__init__(logger_name= "cloud_client_aws", *args, **kwargs)
+    super().__init__(logger_name= "cloud_client_azure", *args, **kwargs)
   
-  # There is not post init when in Config Mode
-  def _post_init(self, *args, **kwargs):
+  def _login(self, *args, **kwargs):
     pass
   
-  def action_test(self, *args, **kwargs):
+  def action_test(self, *args, **kwargs):    
     if not self.is_provider_config_completed():
       print("Provider must be configured first")
       self._setup_another_config()
       return
-    from threemystic_cloud_client.cloud_providers.aws.test_config.step_1 import cloud_client_aws_test_step_1 as test
+    
+    from threemystic_cloud_client.cloud_providers.azure.test.step_1 import cloud_client_azure_test_step_1 as test
     next_step = test(common= self.get_common(), logger= self.get_logger(), *args, **kwargs)
     
     next_step.step()
-
+  
   def action_config(self, *args, **kwargs):     
-    from threemystic_cloud_client.cloud_providers.aws.config.step_1 import cloud_client_aws_config_step_1 as step
+    from threemystic_cloud_client.cloud_providers.azure.config.step_1 import cloud_client_azure_config_step_1 as step
     next_step = step(common= self.get_common(), logger= self.get_logger())
     
     next_step.step()
 
 
-
```

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/test_config/step_1.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/test/step_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,11 +31,11 @@
     if response is None:
       return
 
     if not self.config_profile_name_exists(profile_name= response["profile"].get("formated")):
       print(f"Profile Not Found: {response['profile'].get('formated')}")
       return
 
-    from threemystic_cloud_client.cloud_providers.aws.test_config.step_2 import cloud_client_aws_test_step_2 as nextstep
+    from threemystic_cloud_client.cloud_providers.aws.test.step_2 import cloud_client_aws_test_step_2 as nextstep
     nextstep(init_object = self).step( profile_name= response['profile'].get('formated'))
```

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/test_config/step_2.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/test/step_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from threemystic_cloud_client.cloud_providers.aws.test_config.base_class.base import cloud_client_aws_test_base as base
+from threemystic_cloud_client.cloud_providers.aws.test.base_class.base import cloud_client_aws_test_base as base
 from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
 
 
 class cloud_client_aws_test_step_2(base):
   def __init__(self, *args, **kwargs):
     super().__init__(logger_name= "cloud_client_aws_test2", *args, **kwargs)
```

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/aws/test_config/base_class/base.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from threemystic_cloud_client.cloud_providers.azure.base_class.base import cloud_client_provider_azure_base as base
+from threemystic_cloud_client.cloud_providers.aws.base_class.base import cloud_client_provider_aws_base as base
 
-class cloud_client_azure(base):
+
+class cloud_client_aws(base):
   def __init__(self, *args, **kwargs):
-    super().__init__(logger_name= "cloud_client_azure", *args, **kwargs)
+    super().__init__(logger_name= "cloud_client_aws", *args, **kwargs)
   
-  def _login(self, *args, **kwargs):
+  # There is not post init when in Config Mode
+  def _post_init(self, *args, **kwargs):
     pass
   
-  def action_test(self, *args, **kwargs):    
+  def action_test(self, *args, **kwargs):
     if not self.is_provider_config_completed():
       print("Provider must be configured first")
       self._setup_another_config()
       return
-    
-    from threemystic_cloud_client.cloud_providers.azure.test_config.step_1 import cloud_client_azure_test_step_1 as test
+    from threemystic_cloud_client.cloud_providers.aws.test.step_1 import cloud_client_aws_test_step_1 as test
     next_step = test(common= self.get_common(), logger= self.get_logger(), *args, **kwargs)
     
     next_step.step()
-  
+
   def action_config(self, *args, **kwargs):     
-    from threemystic_cloud_client.cloud_providers.azure.config.step_1 import cloud_client_azure_config_step_1 as step
+    from threemystic_cloud_client.cloud_providers.aws.config.step_1 import cloud_client_aws_config_step_1 as step
     next_step = step(common= self.get_common(), logger= self.get_logger())
     
     next_step.step()
 
 
+
```

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/test_config/step_1.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/test/step_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from threemystic_cloud_client.cloud_providers.azure.test_config.base_class.base import cloud_client_azure_test_base as base
+from threemystic_cloud_client.cloud_providers.azure.test.base_class.base import cloud_client_azure_test_base as base
 from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
 
 
 class cloud_client_azure_test_step_1(base):
   def __init__(self, *args, **kwargs):
     super().__init__(logger_name= "cloud_client_azure_test", *args, **kwargs)
```

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/azure/test_config/base_class/base.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.9/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/.gitignore` & `threemystic_cloud_client-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/LICENSE` & `threemystic_cloud_client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/README.md` & `threemystic_cloud_client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/hatch.toml` & `threemystic_cloud_client-0.1.9/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/pyproject.toml` & `threemystic_cloud_client-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.8/PKG-INFO` & `threemystic_cloud_client-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

