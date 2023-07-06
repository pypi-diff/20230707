# Comparing `tmp/dash-auth-external-1.0.1.tar.gz` & `tmp/dash-auth-external-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-auth-external-1.0.1.tar", last modified: Thu Apr  6 20:33:30 2023, max compression
+gzip compressed data, was "dash-auth-external-1.1.0.tar", last modified: Thu Jul  6 22:32:19 2023, max compression
```

## Comparing `dash-auth-external-1.0.1.tar` & `dash-auth-external-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:33:30.725703 dash-auth-external-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-06 20:33:30.725703 dash-auth-external-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:33:30.725703 dash-auth-external-1.0.1/dash_auth_external/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/dash_auth_external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/dash_auth_external/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/dash_auth_external/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/dash_auth_external/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/dash_auth_external/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/dash_auth_external/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:33:30.725703 dash-auth-external-1.0.1/dash_auth_external.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-06 20:33:30.000000 dash-auth-external-1.0.1/dash_auth_external.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-06 20:33:30.000000 dash-auth-external-1.0.1/dash_auth_external.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 20:33:30.000000 dash-auth-external-1.0.1/dash_auth_external.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-06 20:33:30.000000 dash-auth-external-1.0.1/dash_auth_external.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-06 20:33:30.000000 dash-auth-external-1.0.1/dash_auth_external.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-06 20:33:30.729703 dash-auth-external-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:33:30.725703 dash-auth-external-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-06 20:33:19.000000 dash-auth-external-1.0.1/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/dash_auth_external/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/dash_auth_external.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 22:32:19.000000 dash-auth-external-1.1.0/dash_auth_external.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-06 22:32:19.000000 dash-auth-external-1.1.0/dash_auth_external.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:32:19.000000 dash-auth-external-1.1.0/dash_auth_external.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 22:32:19.000000 dash-auth-external-1.1.0/dash_auth_external.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 22:32:19.000000 dash-auth-external-1.1.0/dash_auth_external.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/tests/test_context.py
```

### Comparing `dash-auth-external-1.0.1/LICENSE` & `dash-auth-external-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dash-auth-external-1.0.1/README.md` & `dash-auth-external-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dash-auth-external-1.0.1/dash_auth_external/auth.py` & `dash-auth-external-1.1.0/dash_auth_external/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,24 +61,26 @@
         return token_data.access_token
 
     def __init__(
         self,
         external_auth_url: str,
         external_token_url: str,
         client_id: str,
+        client_secret: str = None,
         with_pkce=True,
         app_url: str = "http://127.0.0.1:8050",
         redirect_suffix: str = "/redirect",
         auth_suffix: str = "/",
         home_suffix="/home",
         _flask_server: Flask = None,
         _token_field_name: str = "access_token",
         _secret_key: str = None,
         auth_request_headers: dict = None,
         token_request_headers: dict = None,
+        token_body_params: dict = None,
         scope: str = None,
         _server_name: str = __name__,
     ):
         """The interface for obtaining access tokens from 3rd party OAuth2 Providers.
 
         Args:
             external_auth_url (str): The authorization endpoint for the OAuth2 Provider.
@@ -86,33 +88,32 @@
             client_id (str): Client ID obtained from OAuth2 provider.
             with_pkce (bool, optional): Use Proof of Key Exchange, reccomended. Enforced by many OAuth2 providers. Defaults to True.
             app_url (str, optional): The url for your dash application Defaults to "http://127.0.0.1:8050".
             redirect_suffix (str, optional): The route that OAuth2 provider will redirect back to. Defaults to "/redirect".
             auth_suffix (str, optional): The route that will trigger the initial redirect to the external OAuth provider. Defaults to "/".
             home_suffix (str, optional): The route your dash application will sit, relative to your url. Defaults to "/home".
             _flask_server (Flask, optional): Flask server to use if additional config required. Defaults to None.
-            _token_field_name (str, optional): The key for the token returned in JSON from the token endpoint. Defaults to "access_token".
             _secret_key (str, optional): Secret key for flask app, normally generated at runtime. Defaults to None.
-            auth_request_headers (dict, optional): Additional params to send to the authorization endpoint. Defaults to None.
+            auth_request_headers (dict, optional): Additional headers to send to the authorization endpoint. Defaults to None.
             token_request_headers (dict, optional): Additional headers to send to the access token endpoint. Defaults to None.
+            token_body_params (dict, optional): Additional body params to send to the access token endpoint. Defaults to None.
             scope (str, optional): Header required by most Oauth2 Providers. Defaults to None.
             _server_name (str, optional): The name of the Flask Server. Defaults to __name__, ignored if _flask_server is not None.
 
 
         Returns:
            DashAuthExternal: Main package class
         """
 
         if auth_request_headers is None:
             auth_request_headers = {}
         if token_request_headers is None:
             token_request_headers = {}
 
         if _flask_server is None:
-
             app = Flask(
                 _server_name, instance_relative_config=False, static_folder="./assets"
             )
         else:
             app = _flask_server
 
         if _secret_key is None:
@@ -132,19 +133,19 @@
             scope=scope,
             auth_request_params=auth_request_headers,
         )
         app = make_access_token_route(
             app,
             external_token_url=external_token_url,
             client_id=client_id,
+            client_secret=client_secret,
             redirect_uri=redirect_uri,
             redirect_suffix=redirect_suffix,
             _home_suffix=home_suffix,
             token_request_headers=token_request_headers,
-            _token_field_name=_token_field_name,
             with_pkce=with_pkce,
         )
 
         self.server = app
         self.home_suffix = home_suffix
         self.redirect_suffix = redirect_suffix
         self.auth_suffix = auth_suffix
@@ -152,15 +153,14 @@
         self.client_id = client_id
         self.external_token_url = external_token_url
         self.token_request_headers = token_request_headers
         self.scope = scope
 
 
 def refresh_token(url: str, token_data: OAuth2Token, headers: dict) -> OAuth2Token:
-
     body = {
         "grant_type": "refresh_token",
         "refresh_token": token_data.refresh_token,
     }
     data = token_request(url, body, headers)
 
     token_data.access_token = data["access_token"]
```

### Comparing `dash-auth-external-1.0.1/dash_auth_external/routes.py` & `dash-auth-external-1.1.0/dash_auth_external/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,53 +62,58 @@
 
         resp = redirect(authorization_url)
         return resp
 
     return app
 
 
-def build_token_body(url: str, redirect_uri: str, client_id: str, with_pkce: bool):
+def build_token_body(
+    url: str, redirect_uri: str, client_id: str, with_pkce: bool, client_secret: str
+):
     query = urllib.parse.urlparse(url).query
     redirect_params = urllib.parse.parse_qs(query)
     code = redirect_params["code"][0]
     state = redirect_params["state"][0]
     body = dict(
         grant_type="authorization_code",
         code=code,
         redirect_uri=redirect_uri,
         client_id=client_id,
         state=state,
     )
 
     if with_pkce:
-
         body["code_verifier"] = session["cv"]
 
+    if client_secret:
+        body["client_secret"] = client_secret
+
     return body
 
 
 def make_access_token_route(
     app: Flask,
     external_token_url: str,
     redirect_suffix: str,
     _home_suffix: str,
     redirect_uri: str,
     client_id: str,
-    _token_field_name: str,
+    client_secret: str,
     with_pkce: bool,
     token_request_headers: dict,
 ):
     @app.route(redirect_suffix, methods=["GET", "POST"])
     def get_token_route():
         url = request.url
         body = build_token_body(
             url=url,
             redirect_uri=redirect_uri,
             with_pkce=with_pkce,
             client_id=client_id,
+            client_secret=client_secret,
         )
 
         response_data = token_request(
             url=external_token_url,
             body=body,
             headers=token_request_headers,
         )
@@ -120,13 +125,9 @@
         return response
 
     return app
 
 
 def token_request(url: str, body: dict, headers: dict):
     r = requests.post(url, data=body, headers=headers)
-
-    if r.status_code != 200:
-        raise requests.RequestException(
-            f"{r.status_code} {r.reason}:The request to the access token endpoint failed."
-        )
+    r.raise_for_status()
     return r.json()
```

### Comparing `dash-auth-external-1.0.1/dash_auth_external.egg-info/SOURCES.txt` & `dash-auth-external-1.1.0/dash_auth_external.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash-auth-external-1.0.1/setup.py` & `dash-auth-external-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 long_description = (
     "Integrate your dashboards with 3rd party APIs and external OAuth providers."
 )
 requires = ["dash >= 2.0.0", "requests >= 1.0.0", "requests-oauthlib >= 0.3.0"]
 
 setup(
     name=NAME,
-    version="1.0.1",
-    description="Integrate Dash with 3rd Parties and external providers",
+    version="1.1.0",
+    description=long_description,
     python_requires=">=3.7",
     author_email="jholcombe@hotmail.co.uk",
     url="https://github.com/jamesholcombe/dash-auth-external",
     keywords=["Dash", "Plotly", "Authentication", "Auth", "External"],
     install_requires=requires,
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `dash-auth-external-1.0.1/tests/test_app.py` & `dash-auth-external-1.1.0/tests/test_app.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,118 +1,95 @@
-"""Module for integation tests, testing full OAuth2 flow, excluding the get_token method
-"""
-
+import pytest
 from dash_auth_external import DashAuthExternal
 from unittest.mock import Mock
 from dash_auth_external.config import FLASK_SESSION_TOKEN_KEY
-from .test_config import EXERNAL_TOKEN_URL, EXTERNAL_AUTH_URL, CLIENT_ID
-from pytest_mock import mocker
+from .test_config import (
+    EXERNAL_TOKEN_URL,
+    EXTERNAL_AUTH_URL,
+    CLIENT_ID,
+    CLIENT_SECRET,
+)
 from requests_oauthlib import OAuth2Session
 
 
-def test_pkce_true(mocker):
+@pytest.mark.parametrize(
+    "with_pkce, with_client_secret",
+    [(True, True), (True, False), (False, True), (False, False)],
+)
+def test_flow(with_pkce, with_client_secret, mocker):
+
     auth = DashAuthExternal(
-        EXTERNAL_AUTH_URL, EXERNAL_TOKEN_URL, CLIENT_ID, with_pkce=True
+        EXTERNAL_AUTH_URL,
+        EXERNAL_TOKEN_URL,
+        CLIENT_ID,
+        with_pkce=with_pkce,
+        client_secret=CLIENT_SECRET if with_client_secret else None,
     )
-    app = auth.server
+    redirect_uri = "http://127.0.0.1:8050" + auth.redirect_suffix
 
-    redirect_uri = "http://localhost:8050"
     session_mock = Mock(
-        OAuth2Session(CLIENT_ID, redirect_uri=redirect_uri, scope=auth.scope)
+        OAuth2Session(
+            CLIENT_ID,
+            redirect_uri=redirect_uri,
+            scope=auth.scope,
+        )
     )
-
+    app = auth.server
     session_mock.authorization_url.return_value = ("https://example.com", "state")
 
     mocker.patch("dash_auth_external.routes.OAuth2Session", return_value=session_mock)
-
-    mocker.patch(
-        "dash_auth_external.routes.make_code_challenge",
-        return_value=("code_challenge", "code_verifier"),
+    token_request_mock = mocker.patch(
+        "dash_auth_external.routes.token_request",
+        return_value={
+            "access_token": "access_token",
+            "refresh_token": "refresh_token",
+            "token_type": "Bearer",
+            "expires_in": "3599",
+        },
     )
+    expected_token_request_body = {
+        "grant_type": "authorization_code",
+        "code": "code",
+        "redirect_uri": redirect_uri,
+        "client_id": CLIENT_ID,
+        "state": "state",
+    }
+    if with_pkce:
+        expected_token_request_body["code_verifier"] = "code_verifier"
+    if with_client_secret:
+        expected_token_request_body["client_secret"] = CLIENT_SECRET
 
-    # mocking the two helper functions called within the view function for the redirect to home suffix.
-
-    with app.test_client() as client:
-
-        response = client.get(auth.auth_suffix)
-        assert response.status_code == 302
-
-        # assert that the authorization_url method was called with the correct arguments
-        session_mock.authorization_url.assert_called_with(
-            EXTERNAL_AUTH_URL,
-            code_challenge="code_challenge",
-            code_challenge_method="S256",
-        )
-
-        # user logs in and is redirected to the redirect_uri, with a code and state
-
-        # mocking the token request in the token route
+    if with_pkce:
         mocker.patch(
-            "dash_auth_external.routes.token_request",
-            return_value={
-                "access_token": "access_token",
-                "refresh_token": "refresh_token",
-                "token_type": "Bearer",
-                "expires_in": "3599",
-            },
+            "dash_auth_external.routes.make_code_challenge",
+            return_value=("code_challenge", "code_verifier"),
         )
 
-        # now we call the token route with the code and state returned from the authorization_url method
-        response = client.get(
-            auth.redirect_suffix, query_string={"code": "code", "state": "state"}
-        )
-        assert response.status_code == 302
-        with client.session_transaction() as session:
-            token_data = session[FLASK_SESSION_TOKEN_KEY]
-            assert token_data["access_token"] == "access_token"
-            assert token_data["refresh_token"] == "refresh_token"
-            assert token_data["token_type"] == "Bearer"
-            assert token_data["expires_in"] == "3599"
-
-
-def test_pkce_false(mocker):
-    auth = DashAuthExternal(
-        EXTERNAL_AUTH_URL, EXERNAL_TOKEN_URL, CLIENT_ID, with_pkce=False
-    )
-    app = auth.server
-
-    redirect_uri = "http://localhost:8050"
-    session_mock = Mock(
-        OAuth2Session(CLIENT_ID, redirect_uri=redirect_uri, scope=auth.scope)
-    )
-
-    session_mock.authorization_url.return_value = ("https://example.com", "state")
-
-    mocker.patch("dash_auth_external.routes.OAuth2Session", return_value=session_mock)
-
     with app.test_client() as client:
-
         response = client.get(auth.auth_suffix)
         assert response.status_code == 302
 
-        # assert that the authorization_url method was called with the correct arguments
-        session_mock.authorization_url.assert_called_with(EXTERNAL_AUTH_URL)
-
-        # user logs in and is redirected to the redirect_uri, with a code and state
+        if with_pkce:
+            session_mock.authorization_url.assert_called_with(
+                EXTERNAL_AUTH_URL,
+                code_challenge="code_challenge",
+                code_challenge_method="S256",
+            )
+        else:
+            session_mock.authorization_url.assert_called_with(EXTERNAL_AUTH_URL)
 
-        # mocking the token request in the token route
-        mocker.patch(
-            "dash_auth_external.routes.token_request",
-            return_value={
-                "access_token": "access_token",
-                "refresh_token": "refresh_token",
-                "token_type": "Bearer",
-                "expires_in": "3599",
-            },
-        )
-
-        # now we call the token route with the code and state returned from the authorization_url method
         response = client.get(
             auth.redirect_suffix, query_string={"code": "code", "state": "state"}
         )
+        token_request_mock.assert_called_with(
+            url=EXERNAL_TOKEN_URL,
+            body=expected_token_request_body,
+            headers={},
+        )
+
         assert response.status_code == 302
         with client.session_transaction() as session:
             token_data = session[FLASK_SESSION_TOKEN_KEY]
             assert token_data["access_token"] == "access_token"
             assert token_data["refresh_token"] == "refresh_token"
             assert token_data["token_type"] == "Bearer"
             assert token_data["expires_in"] == "3599"
```

### Comparing `dash-auth-external-1.0.1/tests/test_auth.py` & `dash-auth-external-1.1.0/tests/test_auth.py`

 * *Files identical despite different names*

