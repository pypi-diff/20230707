# Comparing `tmp/django_oauth_usp-1.2.1.tar.gz` & `tmp/django_oauth_usp-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oauth_usp-1.2.1.tar", max compression
+gzip compressed data, was "django_oauth_usp-1.2.2.tar", max compression
```

## Comparing `django_oauth_usp-1.2.1.tar` & `django_oauth_usp-1.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1068 2023-07-03 19:42:21.440019 django_oauth_usp-1.2.1/LICENSE
--rw-r--r--   0        0        0     1780 2023-07-03 19:42:21.440019 django_oauth_usp-1.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/__init__.py
--rw-r--r--   0        0        0      402 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/admin.py
--rw-r--r--   0        0        0      108 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/apps.py
--rw-r--r--   0        0        0     3122 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/managers.py
--rw-r--r--   0        0        0      555 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/middleware.py
--rw-r--r--   0        0        0     2557 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/migrations/__init__.py
--rw-r--r--   0        0        0     2288 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/models.py
--rw-r--r--   0        0        0     1395 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/oauth.py
--rw-r--r--   0        0        0      180 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/templates/main.html
--rw-r--r--   0        0        0      624 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/templates/user.html
--rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/__init__.py
--rw-r--r--   0        0        0     1076 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/faker.py
--rw-r--r--   0        0        0     1985 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/mock.py
--rw-r--r--   0        0        0      346 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_admin.py
--rw-r--r--   0        0        0      324 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_manager.py
--rw-r--r--   0        0        0     2964 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_models.py
--rw-r--r--   0        0        0     1224 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_transform.py
--rw-r--r--   0        0        0     4535 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_views.py
--rw-r--r--   0        0        0     1440 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_oauth.py
--rw-r--r--   0        0        0      912 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_user_middleware.py
--rw-r--r--   0        0        0      764 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/transform.py
--rw-r--r--   0        0        0      361 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/urls.py
--rw-r--r--   0        0        0     2720 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/accounts/views.py
--rw-r--r--   0        0        0     2316 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/settings.py
--rw-r--r--   0        0        0      115 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/django_oauth_usp/urls.py
--rw-r--r--   0        0        0      965 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 django_oauth_usp-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-03 19:42:21.440019 django_oauth_usp-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2176 2023-07-07 17:12:51.138203 django_oauth_usp-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/__init__.py
+-rw-r--r--   0        0        0      402 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/admin.py
+-rw-r--r--   0        0        0      108 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/apps.py
+-rw-r--r--   0        0        0     3122 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/managers.py
+-rw-r--r--   0        0        0      555 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/middleware.py
+-rw-r--r--   0        0        0     2557 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/migrations/__init__.py
+-rw-r--r--   0        0        0     3045 2023-07-06 18:38:36.763707 django_oauth_usp-1.2.2/django_oauth_usp/accounts/models.py
+-rw-r--r--   0        0        0     1395 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/oauth.py
+-rw-r--r--   0        0        0      180 2023-07-06 12:36:32.208583 django_oauth_usp-1.2.2/django_oauth_usp/accounts/templates/account_main.html
+-rw-r--r--   0        0        0      632 2023-07-06 12:36:32.208583 django_oauth_usp-1.2.2/django_oauth_usp/accounts/templates/user.html
+-rw-r--r--   0        0        0        0 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/__init__.py
+-rw-r--r--   0        0        0     1076 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/faker.py
+-rw-r--r--   0        0        0     1985 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/mock.py
+-rw-r--r--   0        0        0      346 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_accounts_admin.py
+-rw-r--r--   0        0        0      324 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_accounts_manager.py
+-rw-r--r--   0        0        0     5126 2023-07-06 18:38:36.763707 django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_accounts_models.py
+-rw-r--r--   0        0        0     1224 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_accounts_transform.py
+-rw-r--r--   0        0        0     4543 2023-07-06 12:36:32.208583 django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_accounts_views.py
+-rw-r--r--   0        0        0     1440 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_oauth.py
+-rw-r--r--   0        0        0      912 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_user_middleware.py
+-rw-r--r--   0        0        0      764 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/transform.py
+-rw-r--r--   0        0        0      361 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/urls.py
+-rw-r--r--   0        0        0     2720 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/accounts/views.py
+-rw-r--r--   0        0        0     2316 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/settings.py
+-rw-r--r--   0        0        0      115 2023-07-03 19:42:21.443353 django_oauth_usp-1.2.2/django_oauth_usp/urls.py
+-rw-r--r--   0        0        0      965 2023-07-07 17:16:36.474022 django_oauth_usp-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 django_oauth_usp-1.2.2/PKG-INFO
```

### Comparing `django_oauth_usp-1.2.1/LICENSE` & `django_oauth_usp-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/README.md` & `django_oauth_usp-1.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,106 @@
-================
-Django OAuth USP
-================
+# Django OAuth USP
+
 
 Este pacote permite que usuários façam login utilizando a senha única USP.
 
 Além da autenticação OAuth este pacote também possui migrations para o armazenamento dos
 usuários no banco de dados.
 
 É recomendado que a estas migrations sejam rodadas antes de qualquer outra migration, devido
 a dificuldade de alteração do model User depois de realizada a primeira migration:
-`Using a custom user model when starting a project`__
-
-__ https://docs.djangoproject.com/en/3.1/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project
 
-Quick start
------------
+*[Using a custom user model when starting a project](https://docs.djangoproject.com/en/4.2/topics/auth/customizing/)*
 
-1. Adicione "django_oauth_usp" em INSTALLED_APPS no arquivo settings.py::
+## Como usar
 
+1. Adicione "django_oauth_usp" em INSTALLED_APPS no arquivo settings.py
+    ```
     INSTALLED_APPS = [
         ...
         'django_oauth_usp.accounts',
     ]
+    ```
 
-2. Adicone o Middleware OAuthUspMiddleware::
+2. Adicone o Middleware OAuthUspMiddleware
 
+    ```
     MIDDLEWARE = [
         ...
         'django_oauth_usp.accounts.middleware.OAuthUspMiddleware',
     ]
+    ```
 
-3. No arquivo settings.py, informe o Model que será utilizado para armazenar os usuários::
+3. No arquivo settings.py, informe o Model que será utilizado para armazenar os usuários
 
+        ```
         AUTH_USER_MODEL= 'accounts.UserModel'
+        ```
 
 4. Defina os parâmetro para OAuth::
 
+    ```
     OAUTH_CALLBACK_ID = 'callback_id_da_aplicação'
 
     AUTHLIB_OAUTH_CLIENTS = {
         'usp': {
             'client_id': 'meu_client_id',
             'client_secret': 'meu_secret_key'
         }
     }
-
+    
     #Rota utilizada para a view accounts_authorize
     REDIRECT_URI = '/auth/authorize'
 
     #Lista com o código das unidades que poderão ter acesso.
     ALLOWED_UNIDADES = [12, 13, 14]
+    ```
+
 5. Rode as migrations::
 
+    ```
     python manage.py migrate
+    ```
 
 6. Adicione rotas para as views accounts_login e accounts_authorize::
 
+    ```
     urlpatterns = [
         path('login', accounts_login, name='login'),
         path('authorize', accounts_authorize, name='authorize'),
     ]
+    ```
+## Dados do usuário
 
-
+Os model UserModel provê os seguintes dados do usuário
+* Nome completo
+```
+user.get_full_name()
+```
+* Primeiro nome()
+```
+user.get_short_name()
+```
+* Email
+```
+user.email_user()
+```
+* Telefone
+```
+user.get_phone()
+```
+* É servidor
+```
+user.is_servidor()
+```
+* Função
+```
+user.get_funcao()
+```
+* Vínculo
+```
+user.get_vinculo()
+```
+* Setor
+```
+user.get_setor()
+```
```

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/managers.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/managers.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/middleware.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/middleware.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/migrations/0001_initial.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/models.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -59,11 +59,34 @@
         bind = self.get_bind()
         for item in bind:
             codigo_unidade = item["codigoUnidade"]
             if str(codigo_unidade) in self.ALLOWED_UNIDADES:
                 return True
 
         return False
+    
+    def prepare_json_string(self, json_string: str):
+        prepared = json_string.replace("'", '"')
+        prepared = prepared.replace('None', '"None"')
+        return prepared
 
     def get_bind(self):
-        bind = self.bind.replace("'", '"')
+        bind = self.prepare_json_string(self.bind)
         return json.loads(bind)
+
+    def get_funcao(self):
+        bind = self.get_bind()
+        funcao = [item.get("tipoFuncao") for item in bind if item["tipoVinculo"] == "SERVIDOR"][0]
+        if funcao:
+            return funcao
+        return None
+
+    def get_vinculo(self):
+        bind = self.get_bind()
+        return [item.get("tipoVinculo") for item in bind]
+
+    def get_setor(self):
+        bind = self.get_bind()
+        setor = [item.get("nomeAbreviadoSetor") for item in bind if item["tipoVinculo"] == "SERVIDOR"][0]
+        if setor:
+            return setor
+        return None
```

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/oauth.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/oauth.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/templates/user.html` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/templates/user.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'main.html' %}
+{% extends 'account_main.html' %}
 
 {% block content %}
 
     <ul>
         <li>
             Nome: {{ user.name }}
         </li>
```

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/faker.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/faker.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/mock.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/mock.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_transform.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_accounts_transform.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_accounts_views.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_accounts_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     def test_authentication_required(self):
         client = Client()
         resp = client.get(r('accounts:user_detail'))
         self.assertEqual(302, resp.status_code)
 
     def test_template(self):
-        self.assertTemplateUsed(self.resp, 'main.html')
+        self.assertTemplateUsed(self.resp, 'account_main.html')
         self.assertTemplateUsed(self.resp, 'user.html')
 
     def test_context_has_user(self):
         context = self.resp.context
         self.assertEqual(self.user, context.get('user'))
 
     def test_template_has_user_data(self):
```

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_oauth.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/tests/test_user_middleware.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/tests/test_user_middleware.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/transform.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/transform.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/accounts/views.py` & `django_oauth_usp-1.2.2/django_oauth_usp/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/django_oauth_usp/settings.py` & `django_oauth_usp-1.2.2/django_oauth_usp/settings.py`

 * *Files identical despite different names*

### Comparing `django_oauth_usp-1.2.1/pyproject.toml` & `django_oauth_usp-1.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-oauth-usp"
-version = "1.2.1"
+version = "1.2.2"
 description = ""
 authors = ["Marcelo Schneider <schenider.fei@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_oauth_usp"}]
 
 classifiers = [
```

### Comparing `django_oauth_usp-1.2.1/PKG-INFO` & `django_oauth_usp-1.2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oauth-usp
-Version: 1.2.1
+Version: 1.2.2
 Summary: 
 License: MIT
 Author: Marcelo Schneider
 Author-email: schenider.fei@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,72 +18,113 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: authlib (>=1.2.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-================
-Django OAuth USP
-================
+# Django OAuth USP
+
 
 Este pacote permite que usuários façam login utilizando a senha única USP.
 
 Além da autenticação OAuth este pacote também possui migrations para o armazenamento dos
 usuários no banco de dados.
 
 É recomendado que a estas migrations sejam rodadas antes de qualquer outra migration, devido
 a dificuldade de alteração do model User depois de realizada a primeira migration:
-`Using a custom user model when starting a project`__
-
-__ https://docs.djangoproject.com/en/3.1/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project
 
-Quick start
------------
+*[Using a custom user model when starting a project](https://docs.djangoproject.com/en/4.2/topics/auth/customizing/)*
 
-1. Adicione "django_oauth_usp" em INSTALLED_APPS no arquivo settings.py::
+## Como usar
 
+1. Adicione "django_oauth_usp" em INSTALLED_APPS no arquivo settings.py
+    ```
     INSTALLED_APPS = [
         ...
         'django_oauth_usp.accounts',
     ]
+    ```
 
-2. Adicone o Middleware OAuthUspMiddleware::
+2. Adicone o Middleware OAuthUspMiddleware
 
+    ```
     MIDDLEWARE = [
         ...
         'django_oauth_usp.accounts.middleware.OAuthUspMiddleware',
     ]
+    ```
 
-3. No arquivo settings.py, informe o Model que será utilizado para armazenar os usuários::
+3. No arquivo settings.py, informe o Model que será utilizado para armazenar os usuários
 
+        ```
         AUTH_USER_MODEL= 'accounts.UserModel'
+        ```
 
 4. Defina os parâmetro para OAuth::
 
+    ```
     OAUTH_CALLBACK_ID = 'callback_id_da_aplicação'
 
     AUTHLIB_OAUTH_CLIENTS = {
         'usp': {
             'client_id': 'meu_client_id',
             'client_secret': 'meu_secret_key'
         }
     }
-
+    
     #Rota utilizada para a view accounts_authorize
     REDIRECT_URI = '/auth/authorize'
 
     #Lista com o código das unidades que poderão ter acesso.
     ALLOWED_UNIDADES = [12, 13, 14]
+    ```
+
 5. Rode as migrations::
 
+    ```
     python manage.py migrate
+    ```
 
 6. Adicione rotas para as views accounts_login e accounts_authorize::
 
+    ```
     urlpatterns = [
         path('login', accounts_login, name='login'),
         path('authorize', accounts_authorize, name='authorize'),
     ]
+    ```
+## Dados do usuário
 
-
-
+Os model UserModel provê os seguintes dados do usuário
+* Nome completo
+```
+user.get_full_name()
+```
+* Primeiro nome()
+```
+user.get_short_name()
+```
+* Email
+```
+user.email_user()
+```
+* Telefone
+```
+user.get_phone()
+```
+* É servidor
+```
+user.is_servidor()
+```
+* Função
+```
+user.get_funcao()
+```
+* Vínculo
+```
+user.get_vinculo()
+```
+* Setor
+```
+user.get_setor()
+```
```

