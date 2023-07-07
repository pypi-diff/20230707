# Comparing `tmp/oidcish-0.3.1.tar.gz` & `tmp/oidcish-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidcish-0.3.1.tar", max compression
+gzip compressed data, was "oidcish-1.0.0.tar", max compression
```

## Comparing `oidcish-0.3.1.tar` & `oidcish-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2925 2023-04-05 14:59:26.049048 oidcish-0.3.1/README.md
--rw-r--r--   0        0        0     1069 2023-04-05 14:59:26.049048 oidcish-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      260 2023-03-27 11:20:36.455663 oidcish-0.3.1/src/oidcish/__init__.py
--rw-r--r--   0        0        0     1247 2023-02-22 07:37:52.855116 oidcish-0.3.1/src/oidcish/conn.py
--rw-r--r--   0        0        0     3602 2023-03-27 11:20:36.455663 oidcish-0.3.1/src/oidcish/crypt.py
--rw-r--r--   0        0        0     3781 2023-04-05 12:56:46.261695 oidcish-0.3.1/src/oidcish/flows/base.py
--rw-r--r--   0        0        0    11860 2023-03-27 11:20:36.455663 oidcish-0.3.1/src/oidcish/flows/code.py
--rw-r--r--   0        0        0     6117 2023-04-05 14:59:26.049048 oidcish-0.3.1/src/oidcish/flows/credentials.py
--rw-r--r--   0        0        0     9438 2023-03-27 11:20:36.455663 oidcish-0.3.1/src/oidcish/flows/device.py
--rw-r--r--   0        0        0     2207 2023-04-05 14:59:26.049048 oidcish-0.3.1/src/oidcish/models.py
--rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 oidcish-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2925 2023-04-05 14:59:26.049048 oidcish-1.0.0/README.md
+-rw-r--r--   0        0        0     1077 2023-07-06 11:52:56.051072 oidcish-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      305 2023-07-06 11:52:56.051072 oidcish-1.0.0/src/oidcish/__init__.py
+-rw-r--r--   0        0        0     1207 2023-07-06 11:52:56.051072 oidcish-1.0.0/src/oidcish/conn.py
+-rw-r--r--   0        0        0     3925 2023-07-06 11:52:56.051072 oidcish-1.0.0/src/oidcish/crypt.py
+-rw-r--r--   0        0        0     3891 2023-07-06 11:52:56.051072 oidcish-1.0.0/src/oidcish/flows/base.py
+-rw-r--r--   0        0        0    11917 2023-07-06 11:52:56.051072 oidcish-1.0.0/src/oidcish/flows/code.py
+-rw-r--r--   0        0        0     6139 2023-07-06 11:52:56.051072 oidcish-1.0.0/src/oidcish/flows/credentials.py
+-rw-r--r--   0        0        0     9471 2023-07-06 11:52:56.051072 oidcish-1.0.0/src/oidcish/flows/device.py
+-rw-r--r--   0        0        0     2250 2023-07-06 11:52:56.051072 oidcish-1.0.0/src/oidcish/models.py
+-rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 oidcish-1.0.0/PKG-INFO
```

### Comparing `oidcish-0.3.1/README.md` & `oidcish-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `oidcish-0.3.1/pyproject.toml` & `oidcish-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 [tool.poetry]
 name = "oidcish"
-version = "0.3.1"
+version = "1.0.0"
 description = "Obtain authentication tokens from OIDC providers."
 authors = ["Erik G. Brandt <erik.brandt@shaarpec.com>"]
 readme = "README.md"
 packages = [{include = "oidcish", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pydantic = "^1.10.5"
-httpx = "^0.23.3"
+python = "^3.10"
+pydantic = "^2.0.2"
+httpx = "^0.24.1"
 pkce = "^1.0.3"
-python-dotenv = "^0.21.1"
+python-dotenv = "^1.0.0"
 background = "^0.2.1"
 python-jose = "^3.3.0"
-cryptography = "^38.0.4"
+cryptography = "^41.0.1"
 pendulum = "^2.1.2"
-StrEnum = "^0.4.9"
-beautifulsoup4 = "^4.11.2"
+StrEnum = "^0.4.15"
+beautifulsoup4 = "^4.12.2"
+pydantic-settings = "^2.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
-pylint = "^2.16.2"
-black = "^23.1.0"
-jupyterlab = "^3.6.1"
-jupyterlab-code-formatter = "^1.5.3"
+black = "^23.3.0"
+jupyterlab = "^4.0.2"
+jupyterlab-code-formatter = "^2.2.1"
 isort = "^5.12.0"
-ipython = "^8.10.0"
-jupytext = "^1.14.4"
-pytest = "^7.2.1"
-pytest_check = "^2.1.4"
-Pygments = "^2.14.0"
-devtools = "^0.10.0"
+ipython = "^8.14.0"
+jupytext = "^1.14.7"
+pytest = "^7.4.0"
+pytest_check = "^2.1.5"
+Pygments = "^2.15.1"
+devtools = "^0.11.0"
 respx = "^0.20.1"
-pandas = "^1.5.3"
-pytest-sugar = "^0.9.6"
-pytest-xdist = "^3.2.0"
+pandas = "^2.0.3"
+pytest-sugar = "^0.9.7"
+pytest-xdist = "^3.3.1"
 pytest-icdiff = "^0.6"
 pytest-timeout = "^2.1.0"
+ruff = "^0.0.277"
 
-[tool.pylint.'MESSAGES CONTROL']
-extension-pkg-whitelist = "pydantic"
+[tool.ruff]
+exclude = [".venv", "typings"]
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `oidcish-0.3.1/src/oidcish/conn.py` & `oidcish-1.0.0/src/oidcish/conn.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
         self._set_headers()
         self.wfile.write(
             json.dumps({"signin_recieved": path == "/oauth2/callback"}).encode(("utf8"))
         )
 
     # Silent server.
-    # pylint: disable=redefined-builtin
     def log_message(self, format, *args):
         return
 
 
 class ReuseAddrTCPServer(TCPServer):
     """TCP server which allows reuse of sockets."""
```

### Comparing `oidcish-0.3.1/src/oidcish/crypt.py` & `oidcish-1.0.0/src/oidcish/crypt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Cryptography module."""
 from __future__ import annotations
-from typing import Dict, Mapping, Any
+from typing import Dict, Mapping, Any, MutableMapping
 
 import jose
-import jose.jwk
 import jose.jwt
 import jose.constants
+from jose.jwk import RSAKey
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.primitives import serialization
 
 
 class RsaKeysFactory:
     """Create and handle RSA key pair."""
 
@@ -46,38 +46,40 @@
         """The public RSA key in PEM format."""
         return self._public_key.public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.SubjectPublicKeyInfo,
         ).decode("utf-8")
 
     @property
-    def private(self) -> jose.jwk.RSAKey:
+    def private(self) -> RSAKey | None:  # type: ignore
         """The private RSA key."""
-        return jose.jwk.RSAKey(
-            algorithm=self.algorithm,
-            key=self.private_pem,
-        )
+        if RSAKey:
+            return RSAKey(algorithm=self.algorithm, key=self.private_pem)
+        return None
 
     @property
-    def public(self) -> jose.jwk.RSAKey:
+    def public(self) -> RSAKey | None:  # type: ignore
         """The public RSA key."""
-        return jose.jwk.RSAKey(
-            algorithm=self.algorithm,
-            key=self.public_pem,
-        )
+        if RSAKey:
+            return RSAKey(algorithm=self.algorithm, key=self.public_pem)
+        return None
 
     @property
-    def private_dict(self) -> Dict[str, Any]:
+    def private_dict(self) -> Dict[str, Any] | None:
         """The private RSA key as a dictionary."""
-        return {**self.private.to_dict(), **self.headers}
+        if self.private:
+            return {**self.private.to_dict(), **self.headers}
+        return None
 
     @property
-    def public_dict(self) -> Dict[str, Any]:
+    def public_dict(self) -> Dict[str, Any] | None:
         """The public RSA key as a dictionary."""
-        return {**self.public.to_dict(), **self.headers}
+        if self.public:
+            return {**self.public.to_dict(), **self.headers}
+        return None
 
 
 class Codec:
     """Class that uses a RsaKeysFactory to encode and decode claims."""
 
     def __init__(self, key: RsaKeysFactory) -> None:
         self._key = key
@@ -89,29 +91,33 @@
         algorithm: str = jose.constants.Algorithms.RS256,
         **kwargs,
     ) -> Codec:
         """Create a Codec that uses the given key size and algorithm."""
         key_factory = RsaKeysFactory(key_size=key_size, algorithm=algorithm, **kwargs)
         return cls(key=key_factory)
 
-    def encode(self, claims: Mapping[Any, Any]) -> str:
+    def encode(self, claims: MutableMapping[Any, Any]) -> str | None:
         """Encode claims.
 
         kwargs are used as extra headers.
         """
-        return jose.jwt.encode(
-            claims,
-            key=self._key.private_dict,
-            algorithm=self._key.algorithm,
-            headers=self._key.headers,
-        )
+        if self._key.private_dict:
+            return jose.jwt.encode(
+                claims,
+                key=self._key.private_dict,
+                algorithm=self._key.algorithm,
+                headers=self._key.headers,
+            )
+        return None
 
-    def decode(self, token: str) -> Mapping[Any, Any]:
+    def decode(self, token: str) -> Mapping[Any, Any] | None:
         """Decode the claims in the token."""
-        return jose.jwt.decode(token, key=self._key.public_dict)
+        if self._key.public_dict:
+            return jose.jwt.decode(token, key=self._key.public_dict)
+        return None
 
     @staticmethod
     def get_unverified_claims(token: str) -> Mapping[Any, Any]:
         """Get unverified claims in the token."""
         return jose.jwt.get_unverified_claims(token)
 
     @property
```

### Comparing `oidcish-0.3.1/src/oidcish/flows/base.py` & `oidcish-1.0.0/src/oidcish/flows/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from abc import ABC, abstractmethod
 from enum import Enum, auto
 from typing import List, Optional, final
 
 import httpx
 import jose
 import jose.jwt
-from pydantic import BaseSettings, Field, parse_obj_as
+from pydantic import ConfigDict, Field, TypeAdapter
 from strenum import StrEnum
 
 from oidcish import models
+from pydantic_settings import BaseSettings
 
 
 class Flows(Enum):
     """Supported authentication flows."""
 
     DEVICE = auto()
     CODE = auto()
@@ -28,21 +29,19 @@
 
 class Settings(BaseSettings):
     """Settings for general authentication flow."""
 
     host: str = Field(default=None)
     timeout: float = Field(default=3.0)
 
-    # pylint: disable=too-few-public-methods
-    class Config:
-        """Additional configuration."""
-
-        env_prefix = os.environ.get("OIDCISH_ENV_PREFIX", "oidcish_")
-        env_file = ".env"
-        extra = "ignore"
+    model_config = ConfigDict(  # type: ignore
+        env_prefix=os.environ.get("OIDCISH_ENV_PREFIX", "oidcish_"),
+        env_file=".env",
+        extra="ignore",
+    )
 
 
 class AuthenticationFlow(ABC):
     """Abstract class for authentication flows."""
 
     def __init__(self, settings: Settings) -> None:
         # Set attributes
@@ -55,23 +54,25 @@
 
     @final
     def get_info(self) -> models.Idp:
         """Get discovery document from identity provider."""
         response = self._client.get(".well-known/openid-configuration")
         response.raise_for_status()
 
-        return models.Idp.parse_obj(response.json())
+        return models.Idp.model_validate(response.json())
 
     @final
     def get_jwks(self) -> List[models.Jwks]:
         """Get public JWK set from identity provider."""
         response = self._client.get(self.idp.jwks_uri)
         response.raise_for_status()
 
-        return parse_obj_as(List[models.Jwks], response.json().get("keys"))
+        ta = TypeAdapter(List[models.Jwks])
+
+        return ta.validate_python(response.json().get("keys"))
 
     @final
     @property
     def status(self) -> Status:
         """Access authentication status."""
         return self._status
 
@@ -114,15 +115,19 @@
     @final
     @property
     def id_claims(self) -> Optional[models.Claims]:
         """Id claims corresponding to credentials."""
         if self.credentials is None:
             return None
 
-        return models.Claims.from_token(self.credentials.id_token)
+        return (
+            models.Claims.from_token(self.credentials.id_token)
+            if self.credentials.id_token
+            else None
+        )
 
     @final
     @property
     def access_claims(self) -> Optional[models.Claims]:
         """Access claims corresponding to credentials."""
         if self.credentials is None:
             return None
```

### Comparing `oidcish-0.3.1/src/oidcish/flows/code.py` & `oidcish-1.0.0/src/oidcish/flows/code.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,25 +65,27 @@
     ----------
       **kwargs : Authentication details and other arguments.
 
         Valid authentication arguments are:
           host: str, The IDP host name (OIDCISH_HOST).
           client_id: str, The client ID (OIDCISH_CLIENT_ID).
           client_secret: str, The client secret (OIDCISH_CLIENT_SECRET).
-          redirect_uri: str, Must exactly match one of the allowed redirect URIs for the client
+          redirect_uri: str, Must exactly match one of the allowed redirect URIs for
+          the client
             (OIDCISH_CLIENT_ID, default: http://localhost).
           username: str = The user name (OIDCISH_USERNAME).
           password: str = The user password (OIDCISH_PASSWORD).
           scope: str, A space separated, case-sensitive list of scopes
             (OIDCISH_SCOPE, default: openid profile offline_access).
           audience: str = The access claim was designated for this audience
             (OIDCISH_AUDIENCE).
 
         Valid other arguments are:
-          verbose: boolean, Print more information during the login procedure. (Default = False)
+          verbose: boolean, Print more information during the login procedure.
+            (Default = False)
 
     Examples
     --------
     >>> from oidcish.code import CodeFlow
     >>> auth = DeviceFlow(
             host="https://idp.example.com",
             client_id=...,
@@ -183,24 +185,26 @@
     def __login(self) -> LoginParameters:
         """Login by sending username and password to server.
 
         Return login parameters.
         """
         pre_login_parameters = self.__pre_login()
 
+        rvf = pre_login_parameters.request_verification_token
+
         response = self._client.post(
             pre_login_parameters.login_url,
             headers={"cookie": pre_login_parameters.cookie},
             params={"ReturnUrl": pre_login_parameters.return_url},
             data={
                 "ReturnUrl": pre_login_parameters.return_url,
                 "Username": self.settings.username,
                 "Password": self.settings.password,
                 "button": "login",
-                "__RequestVerificationToken": pre_login_parameters.request_verification_token,
+                "__RequestVerificationToken": rvf,
                 "RememberLogin": "false",
             },
         )
 
         # Follow redirects
         while response.next_request is not None:
             response = self._client.send(response.next_request)
@@ -263,15 +267,15 @@
                 f"Token request: {response.request.method}: {response.request.url} "
                 f"with headers {response.request.headers}."
             )
 
         # Parse credentials
         try:
             response.raise_for_status()
-            credentials = models.Credentials.parse_obj(response.json())
+            credentials = models.Credentials.model_validate(response.json())
         except httpx.HTTPStatusError as exc:
             self._status = CodeStatus.ERROR
             raise httpx.HTTPStatusError(
                 request=exc.request,
                 response=exc.response,
                 message=f"Unexpected response {response.text}.",
             )
@@ -295,25 +299,25 @@
         """Refresh credentials."""
         if self.credentials is None:
             self._status = CodeStatus.UNINITIALIZED
             return
         return
 
     #     data = dict(
-    #         self.settings.dict(),
+    #         self.settings.model_dump(),
     #         grant_type="refresh_token",
     #         refresh_token=self.credentials.refresh_token,
     #     )
     #     data.pop("host")
 
     #     response = self._client.post(self.idp.token_endpoint, data=data)
 
     #     try:
     #         response.raise_for_status()
-    #         credentials = models.Credentials.parse_obj(response.json())
+    #         credentials = models.Credentials.model_validate(response.json())
     #     except httpx.HTTPStatusError as exc:
     #         self._status = DeviceStatus.ERROR
     #         raise httpx.HTTPStatusError(
     #             request=exc.request,
     #             response=exc.response,
     #             message=f"Unexpected response {response.text}.",
     #         )
```

### Comparing `oidcish-0.3.1/src/oidcish/flows/credentials.py` & `oidcish-1.0.0/src/oidcish/flows/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     ERROR = "ERROR: Authentication failed."
     SUCCESS = "SUCCESS: Authentication was successful."
 
 
 class CredentialsFlow(AuthenticationFlow):
     """Authenticate with IDP host using client credentials flow.
 
-    The client on the IDP host must support client credentials flow. Authentication arguments
-    can be provided as keywords, environment variables, or in a file whose path is
-    given with the special `_env_file` argument. The variables in this file are
+    The client on the IDP host must support client credentials flow. Authentication
+    arguments can be provided as keywords, environment variables, or in a file whose
+    path is given with the special `_env_file` argument. The variables in this file are
     prefixed with the value given by the OIDCISH_ENV_PREFIX environment variable
     (default: OIDCISH_).
     \f
     Parameters
     ----------
       **kwargs : Authentication details and other arguments.
 
@@ -89,28 +89,28 @@
                 break
             if pendulum.now(tz="UTC").int_timestamp > self.access_claims.exp:
                 self.refresh()
             time.sleep(poll_rate)
 
     def init(self, poll_rate: float = 1.0) -> None:
         """Initiate sign-in."""
-        data = self.settings.dict()
+        data = self.settings.model_dump()
         data.pop("host")
 
         response = httpx.post(
             self.idp.token_endpoint,
             data=dict(
                 data,
                 grant_type="client_credentials",
             ),
         )
 
         try:
             response.raise_for_status()
-            self._credentials = models.Credentials.parse_obj(response.json())
+            self._credentials = models.Credentials.model_validate(response.json())
         except httpx.HTTPStatusError as exc:
             self._status = CredentialsStatus.ERROR
             raise httpx.HTTPStatusError(
                 request=exc.request,
                 response=exc.response,
                 message=f"Unexpected response {response.text}.",
             )
@@ -142,24 +142,24 @@
     def refresh(self) -> None:
         """Refresh credentials."""
         if self.credentials is None:
             self._status = CredentialsStatus.UNINITIALIZED
             return
 
         data = dict(
-            self.settings.dict(),
+            self.settings.model_dump(),
             grant_type="client_credentials",
         )
         data.pop("host")
 
         response = self._client.post(self.idp.token_endpoint, data=data)
 
         try:
             response.raise_for_status()
-            credentials = models.Credentials.parse_obj(response.json())
+            credentials = models.Credentials.model_validate(response.json())
         except httpx.HTTPStatusError as exc:
             self._status = CredentialsStatus.ERROR
             raise httpx.HTTPStatusError(
                 request=exc.request,
                 response=exc.response,
                 message=f"Unexpected response {response.text}.",
             )
```

### Comparing `oidcish-0.3.1/src/oidcish/flows/device.py` & `oidcish-1.0.0/src/oidcish/flows/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
         # Initiate sign-in procedure
         self.init(poll_rate=poll_rate)
 
     @background.task
     def __signin_once_confirmed(self, verification: DeviceVerification) -> None:
         """Background tasks that signs in once the user confirms the device."""
-        data = self.settings.dict()
+        data = self.settings.model_dump()
         data.pop("host")
 
         start = time.time()
         while (elapsed := time.time() - start) <= verification.expires_in and (
             self.status is not DeviceStatus.ERROR
         ):
             response = httpx.post(
@@ -113,15 +113,15 @@
                     grant_type="urn:ietf:params:oauth:grant-type:device_code",
                     device_code=verification.device_code,
                 ),
             )
 
             try:
                 response.raise_for_status()
-                self._credentials = models.Credentials.parse_obj(response.json())
+                self._credentials = models.Credentials.model_validate(response.json())
             except httpx.HTTPStatusError as exc:
                 if exc.response.status_code == 400:
                     error_msg = exc.response.json().get("error")
                     if error_msg == "authorization_pending":
                         time.sleep(verification.interval)
                     else:
                         self._status = DeviceStatus.ERROR
@@ -169,22 +169,22 @@
                 pendulum.now(tz="UTC").int_timestamp > self.access_claims.exp
             ):
                 self.refresh()
             time.sleep(poll_rate)
 
     def init(self, poll_rate: float = 1.0) -> None:
         """Initiate sign-in."""
-        data = self.settings.dict()
+        data = self.settings.model_dump()
         data.pop("host")
 
         response = self._client.post(self.idp.device_authorization_endpoint, data=data)
 
         try:
             response.raise_for_status()
-            verification = DeviceVerification.parse_obj(response.json())
+            verification = DeviceVerification.model_validate(response.json())
         except httpx.HTTPStatusError as exc:
             self._status = DeviceStatus.ERROR
             raise httpx.HTTPStatusError(
                 request=exc.request,
                 response=exc.response,
                 message=f"Unexpected response {response.text}.",
             )
@@ -217,25 +217,25 @@
     def refresh(self) -> None:
         """Refresh credentials."""
         if self.credentials is None:
             self._status = DeviceStatus.UNINITIALIZED
             return
 
         data = dict(
-            self.settings.dict(),
+            self.settings.model_dump(),
             grant_type="refresh_token",
             refresh_token=self.credentials.refresh_token,
         )
         data.pop("host")
 
         response = self._client.post(self.idp.token_endpoint, data=data)
 
         try:
             response.raise_for_status()
-            credentials = models.Credentials.parse_obj(response.json())
+            credentials = models.Credentials.model_validate(response.json())
         except httpx.HTTPStatusError as exc:
             self._status = DeviceStatus.ERROR
             raise httpx.HTTPStatusError(
                 request=exc.request,
                 response=exc.response,
                 message=f"Unexpected response {response.text}.",
             )
```

### Comparing `oidcish-0.3.1/src/oidcish/models.py` & `oidcish-1.0.0/src/oidcish/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,55 +35,55 @@
     token_endpoint_auth_methods_supported: List[str]
     userinfo_endpoint: str
 
 
 class Credentials(BaseModel):
     """Credentials from IDP server."""
 
-    id_token: Optional[str]
+    id_token: Optional[str] = None
     access_token: str
-    refresh_token: Optional[str]
+    refresh_token: Optional[str] = None
     expires_in: int
     token_type: str
     scope: str
 
 
 class Claims(BaseModel):
     """Set of reserved claims for a token."""
 
     nbf: int
     exp: int
     iss: str
     aud: str
     client_id: str
     sub: str
-    auth_time: Optional[int]
+    auth_time: Optional[int] = None
     idp: str
     jti: str
     iat: int
     role: Union[str, List[str], None] = Field(...)
     scope: Union[str, List[str]] = Field(...)
-    amr: Optional[List[str]]
+    amr: Optional[List[str]] = None
 
     @staticmethod
     def from_token(token: str) -> Optional[Claims]:
         """Convert token to claims object."""
+        claims = None
         try:
-            claims = Claims.parse_obj(jose.jwt.get_unverified_claims(token))
+            claims = Claims.model_validate(jose.jwt.get_unverified_claims(token))
         except ValidationError as exc:
             print(f"Warning: Failed to parse claims:\n{exc}")
-            claims = None
         finally:
             return claims
 
 
 class Jwks(BaseModel):
     """JWKS key."""
 
     kty: str
     use: str
     kid: str
-    x5t: Optional[str]
+    x5t: Optional[str] = None
     e: str
     n: str
-    x5c: Optional[List[str]]
+    x5c: Optional[List[str]] = None
     alg: str
```

### Comparing `oidcish-0.3.1/PKG-INFO` & `oidcish-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: oidcish
-Version: 0.3.1
+Version: 1.0.0
 Summary: Obtain authentication tokens from OIDC providers.
 Author: Erik G. Brandt
 Author-email: erik.brandt@shaarpec.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: StrEnum (>=0.4.9,<0.5.0)
+Requires-Dist: StrEnum (>=0.4.15,<0.5.0)
 Requires-Dist: background (>=0.2.1,<0.3.0)
-Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
-Requires-Dist: cryptography (>=38.0.4,<39.0.0)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: cryptography (>=41.0.1,<42.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pkce (>=1.0.3,<2.0.0)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.1,<3.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # oidcish
 
 - "Oh I Don't Care If Something Happens"
 - "OIDC Is Definitely Cool If Someone Helps"
```

