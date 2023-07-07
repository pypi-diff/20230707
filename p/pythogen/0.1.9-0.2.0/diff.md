# Comparing `tmp/pythogen-0.1.9.tar.gz` & `tmp/pythogen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.1.9.tar", max compression
+gzip compressed data, was "pythogen-0.2.0.tar", max compression
```

## Comparing `pythogen-0.1.9.tar` & `pythogen-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-03-21 14:52:33.982397 pythogen-0.1.9/LICENSE
--rw-r--r--   0        0        0     2830 2023-03-21 14:52:33.982397 pythogen-0.1.9/README.md
--rw-r--r--   0        0        0     1381 2023-03-21 14:52:33.986397 pythogen-0.1.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1445 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/entrypoint.py
--rw-r--r--   0        0        0     7247 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/models.py
--rw-r--r--   0        0        0     2363 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3296 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/document.py
--rw-r--r--   0        0        0      601 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3177 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2156 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2461 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1098 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3203 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1834 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/parsers/response.py
--rw-r--r--   0        0        0    15724 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0     9193 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/renderer.py
--rw-r--r--   0        0        0      172 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/settings.py
--rw-r--r--   0        0        0     4759 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/templates/client/httpx-method.j2
--rw-r--r--   0        0        0     1668 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/templates/client/httpx-request-metrics.j2
--rw-r--r--   0        0        0     9165 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/templates/httpx.j2
--rw-r--r--   0        0        0       33 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/templates/init-py.j2
--rw-r--r--   0        0        0      337 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 pythogen-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-07 14:39:08.663445 pythogen-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2097 2023-07-07 14:39:08.663445 pythogen-0.2.0/README.md
+-rw-r--r--   0        0        0     1567 2023-07-07 14:39:08.671445 pythogen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1585 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/entrypoint.py
+-rw-r--r--   0        0        0     7059 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/models.py
+-rw-r--r--   0        0        0     2329 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3307 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      576 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3239 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2132 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2437 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1074 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3512 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1810 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    16508 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0     9844 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/renderer.py
+-rw-r--r--   0        0        0      172 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/settings.py
+-rw-r--r--   0        0        0     5149 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/templates/client/httpx-method.j2
+-rw-r--r--   0        0        0     1668 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/templates/client/httpx-request-metrics.j2
+-rw-r--r--   0        0        0    10825 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/templates/httpx.j2
+-rw-r--r--   0        0        0       33 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/templates/init-py.j2
+-rw-r--r--   0        0        0      337 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/templates/pyproject-toml.j2
+-rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.0/PKG-INFO
```

### Comparing `pythogen-0.1.9/LICENSE` & `pythogen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.9/README.md` & `pythogen-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,91 @@
-<div>
-  <p align="center">
-    <img src="docs/images/logo_long.png" height="auto" width="400px">
-  </p>
-  <br/>
-</div>
+Metadata-Version: 2.1
+Name: pythogen
+Version: 0.2.0
+Summary: Generator of python HTTP-clients from OpenApi specification.
+Home-page: https://github.com/artsmolin/pythogen
+License: MIT
+Keywords: openapi,openapi-generator,swagger,http-client,generator
+Author: Artur Smolin
+Author-email: artursmolin@outlook.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: autoflake (>=2.2.0,<3.0.0)
+Requires-Dist: black (>=23.3.0,<24.0.0)
+Requires-Dist: inflection (>=0.5.1,<0.6.0)
+Requires-Dist: isort (>=5.12.0,<6.0.0)
+Requires-Dist: jinja2 (>=3.1.1,<4.0.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: rich (>=12.2.0,<13.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Project-URL: Repository, https://github.com/artsmolin/pythogen
+Description-Content-Type: text/markdown
 
-Generator of python HTTP-clients from OpenApi specification based on [httpx](https://github.com/projectdiscovery/httpx) and [pydantic](https://github.com/pydantic/pydantic).
+<h2 align="center">Awesome python HTTP-clients from  OpenAPI</h2>
 
 [![Build Status](https://github.com/artsmolin/pythogen/actions/workflows/main.yml/badge.svg)](https://github.com/artsmolin/pythogen/actions)
 [![codecov](https://codecov.io/gh/artsmolin/pythogen/branch/main/graph/badge.svg?token=6JR6NB8Y9Z)](https://codecov.io/gh/artsmolin/pythogen)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-[![Python](https://img.shields.io/pypi/pyversions/pythogen.svg)](https://pypi.python.org/pypi/pythogen/)
+[![downloads](https://pepy.tech/badge/pythogen/month)](https://pepy.tech/project/pythogen)
+[![python](https://img.shields.io/pypi/pyversions/pythogen.svg)](https://pypi.python.org/pypi/pythogen/)
 [![pypi](https://img.shields.io/pypi/v/pythogen.svg)](https://pypi.org/project/pythogen/)
-
 [![license](https://img.shields.io/github/license/artsmolin/pythogen.svg)](https://github.com/artsmolin/pythogen/blob/master/LICENSE)
 
 ---
 
-<p align="center">
-  <img src="docs/images/example.png">
-</p>
-
-## Features
-- [Discriminator](/docs/discriminator.md)
-- [Metrics](/docs/metrics.md)
-- Sync/async clients
+Generator of python HTTP-clients from OpenApi specification based on <i>httpx</i> and <i>pydantic</i>
+> Versions **0.1.*** use pydantic **v1.*** and are no longer supported.
+
+> Versions **0.2.*** use pydantic **v2.***.
 
 ## Examples
-- [**Petstore OpenAPI**](/examples/petstore/openapi.yaml):  [client_sync.py](/examples/petstore/client_sync.py) | [client_async.py](/examples/petstore/client_async.py)
+- [Sync](/examples/petstore/client_sync.py) and [async](/examples/petstore/client_async.py) clients for [Petstore OpenAPI](/examples/petstore/openapi.yaml)
 
 ## Installation
+Pip
 ```shell
 pip install pythogen
 ```
+Docker
+```shell
+docker pull artsmolin/pythogen
+```
 
-## Usage
-### Generate ordinary clients
-- Asynchronous client
-  ```shell
-  pythogen path/to/input/openapi.yaml path/to/output/client.py
-  ```
-- Asynchronous client with integration for metrics
-  ```shell
-  pythogen path/to/input/openapi.yaml path/to/output/client.py --metrics
-  ```
-- Synchronous client
-  ```shell
-  pythogen path/to/input/openapi.yaml path/to/output/client.py --sync
-  ```
-- Synchronous client with integration for metrics
-  ```shell
-  pythogen path/to/input/openapi.yaml path/to/output/client.py --sync --metrics
-  ```
-### Generate client as python-package
+## Generation
+- `path/to/input` — path to the directory with openapi.yaml;
+- `path/to/output` — the path to the directory where the generated client will be saved;
+Pip
+```shell
+pythogen path/to/input/openapi.yaml path/to/output/client.py
+```
+Docker
 ```shell
-pythogen path/to/input/openapi.yaml path/to/package/output --package-version=0.0.1 --package-authors="Rick, Morty"
+docker run \
+-v ./path/to/input:/opt/path/to/input \
+-v ./path/to/output:/opt/path/to/output \
+artsmolin/pythogen \
+path/to/input/openapi.yaml \
+path/to/output/client.py
 ```
-- `--package-version` — required;
-- `--package-authors` — optional;
-- `path/to/package/output` — path to the directory where package will be saved.
-### Usage client
+
+## Usage
 ```python
 from petstore.client_async import Client
 from petstore.client_async import Pet
 from petstore.client_async import EmptyBody
 
 client = Client(base_url="http://your.base.url")
 pets: list[Pet] | EmptyBody = await client.findPetsByStatus(status="available")
 ```
 
-## Development
-- Activate environment
-  ```shell
-  rm -rf .venv || true
-  python3 -m venv .venv
-  source .venv/bin/activate
-  make requirements
-  ```
-- Make changes
-- Execute `make clients-for-tests && make test-clients`
-- Execute `make clients-for-examples`
```

### Comparing `pythogen-0.1.9/pyproject.toml` & `pythogen-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.1.9"
+version = "0.2.0"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
@@ -26,26 +26,37 @@
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Code Generators",
     "Topic :: Utilities",
     "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-typer = "^0.4.1"
+python = "^3.10"
+typer = "^0.9.0"
 pyyaml = "^6.0"
 jinja2 = "^3.1.1"
 rich = "^12.2.0"
 inflection = "^0.5.1"
+black = "^23.3.0"
+autoflake = "^2.2.0"
+isort = "^5.12.0"
+pydantic = "^2.0.2"
 
 [tool.poetry.scripts]
 pythogen = 'pythogen.entrypoint:run'
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 importlib-metadata = "^4.11.4"
 pre-commit = "^2.19.0"
 
+[tool.poetry.group.dev.dependencies]
+httpx = "^0.24.1"
+pydantic = "^2.0.0"
+
 [build-system]
 requires = ["poetry>=1.4.0"]
 build-backend = "poetry.masonry.api"
+
+[tool.black]
+line-length = 120
```

### Comparing `pythogen-0.1.9/pythogen/entrypoint.py` & `pythogen-0.2.0/pythogen/entrypoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     input: str = typer.Argument(..., help="input OpenAPI file path"),
     output: str = typer.Argument(..., help="client output file path"),
     name: str = typer.Option("Client", help="client class name"),
     sync: bool = typer.Option(False, help="sync client"),
     package_version: Optional[str] = typer.Option(None, help="package version"),
     package_authors: Optional[str] = typer.Option(None, help="package authors"),
     metrics: bool = typer.Option(False, help="include metrics integration"),
+    headers: Optional[str] = typer.Option(None, help="required headers"),
 ):
     """
     Generate HTTP clients for python from OpenAPI
     """
     if package_version:
         resp = packager.init_package(
             output_path=output,
@@ -41,14 +42,15 @@
 
     renderer.render_client(
         output_path=output,
         document=document,
         name=name,
         sync=sync,
         metrics=metrics,
+        required_headers=headers.split(",") if headers else None,
     )
 
 
 def run() -> None:
     typer.run(main)
```

### Comparing `pythogen-0.1.9/pythogen/models.py` & `pythogen-0.2.0/pythogen/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 
 from __future__ import annotations
 
 import keyword
 import re
 from dataclasses import dataclass
 from enum import Enum
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Union
 
 
 class HttpMethod(Enum):
     get = 'get'
     put = 'put'
     post = 'post'
     delete = 'delete'
@@ -48,41 +44,41 @@
 
 @dataclass
 class ContactObject:
     """
     https://swagger.io/specification/#contact-object
     """
 
-    name: Optional[str]
-    url: Optional[str]
-    email: Optional[str]
+    name: str | None
+    url: str | None
+    email: str | None
 
 
 @dataclass
 class LicenseObject:
     """
     https://swagger.io/specification/#license-object
     """
 
     name: str
-    url: Optional[str]
+    url: str | None
 
 
 @dataclass
 class InfoObject:
     """
     https://swagger.io/specification/#info-object
     """
 
     title: str
     version: str
-    description: Optional[str] = None
-    termsOfService: Optional[str] = None
-    contact: Optional[ContactObject] = None
-    license: Optional[LicenseObject] = None
+    description: str | None = None
+    termsOfService: str | None = None
+    contact: ContactObject | None = None
+    license: LicenseObject | None = None
 
 
 class Type(Enum):
     string = 'string'
     number = 'number'
     integer = 'integer'
     boolean = 'boolean'
@@ -92,15 +88,15 @@
     # TODO: refactor
     any_of = 'any_of'
 
 
 @dataclass
 class SchemaProperty:
     orig_key: str
-    safety_key: Optional[str]
+    safety_key: str | None
     schema: 'SchemaObject'
 
     @property
     def key(self):
         return self._safe_key()
 
     def _safe_key(self):
@@ -128,52 +124,52 @@
 @dataclass
 class SchemaObject:
     """
     https://swagger.io/specification/#schema-object
     """
 
     id: str
-    title: Optional[str]
-    required: Optional[List[str]]
-    enum: Optional[List[str]]
+    title: str | None
+    required: list[str] | None
+    enum: list[str] | None
     type: Type
-    format: Optional[Format]
-    items: Optional[Union['SchemaObject', List['SchemaObject']]]
-    properties: List[SchemaProperty]
-    description: Optional[str] = None
+    format: Format | None
+    items: 'SchemaObject' | list['SchemaObject'] | None
+    properties: list[SchemaProperty]
+    description: str | None = None
 
     # Технические поля
-    discriminator_base_class_schema: Optional[DiscriminatorBaseClassSchema] = None
+    discriminator_base_class_schema: DiscriminatorBaseClassSchema | None = None
     is_fake: bool = False
 
     @property
-    def required_properties(self) -> List[SchemaProperty]:
+    def required_properties(self) -> list[SchemaProperty]:
         if self.required is None:
             return []
 
         return [p for p in self.properties if p.orig_key in self.required]
 
     @property
-    def optional_properties(self) -> List[SchemaProperty]:
+    def optional_properties(self) -> list[SchemaProperty]:
         if self.required is None:
             return self.properties
 
         return [p for p in self.properties if p.orig_key not in self.required]
 
 
 @dataclass
 class ParameterObject:
     """
     https://swagger.io/specification/#parameter-object
     """
 
     id: str
     orig_key: str
-    safety_key: Optional[str]
-    description: Optional[str]
+    safety_key: str | None
+    description: str | None
     location: ParameterLocation
     required: bool
     schema: SchemaObject
 
     @property
     def key(self):
         return self.safety_key if self.safety_key else self.orig_key
@@ -182,51 +178,51 @@
 @dataclass
 class RequestBodyObject:
     """
     https://swagger.io/specification/#request-body-object
     """
 
     id: str
-    description: Optional[str]
+    description: str | None
     schema: SchemaObject
     required: bool
     is_form_data: bool
     is_multipart_form_data: bool
     are_files_required: bool
 
 
 @dataclass
 class OperationObject:
     """
     https://swagger.io/specification/#operation-object
     """
 
     method: HttpMethod
-    summary: Optional[str]
-    description: Optional[str]
-    operation_id: Optional[str]
-    request_body: Optional[RequestBodyObject]
+    summary: str | None
+    description: str | None
+    operation_id: str | None
+    request_body: RequestBodyObject | None
     responses: ResponsesObject
-    parameters: List[ParameterObject]
+    parameters: list[ParameterObject]
     path_str: str
 
     @property
-    def path_params(self) -> List[ParameterObject]:
+    def path_params(self) -> list[ParameterObject]:
         return [parameter for parameter in self.parameters if parameter.location == ParameterLocation.path]
 
     @property
-    def query_params(self) -> List[ParameterObject]:
+    def query_params(self) -> list[ParameterObject]:
         return [parameter for parameter in self.parameters if parameter.location == ParameterLocation.query]
 
     @property
-    def headers(self) -> List[ParameterObject]:
+    def headers(self) -> list[ParameterObject]:
         return [parameter for parameter in self.parameters if parameter.location == ParameterLocation.header]
 
     @property
-    def fn_name(self) -> Optional[str]:
+    def fn_name(self) -> str | None:
         if self.operation_id is not None:
             return self.operation_id.replace('-', '_')
 
         name = self.path_str.removeprefix('/').replace('-', '_').replace('/', '_').replace('{', '').replace('}', '')
         name = self.method.value + '_' + name
         name = name.lower()
         return name
@@ -234,43 +230,43 @@
 
 @dataclass
 class PathItemObject:
     """
     https://swagger.io/specification/#path-item-object
     """
 
-    summary: Optional[str]
-    description: Optional[str]
-    operations: Dict[HttpMethod, OperationObject]
+    summary: str | None
+    description: str | None
+    operations: dict[HttpMethod, OperationObject]
 
 
 @dataclass
 class ResponseObject:
     id: str
     description: str
-    schema: Optional[SchemaObject]
+    schema: SchemaObject | None
 
 
 @dataclass
 class ResponsesObject:
-    patterned: Dict[str, ResponseObject]
+    patterned: dict[str, ResponseObject]
 
 
 @dataclass
 class Document:
     info: InfoObject
-    paths: Dict[str, PathItemObject]
-    parameters: Dict[str, ParameterObject]
-    schemas: Dict[str, SchemaObject]
+    paths: dict[str, PathItemObject]
+    parameters: dict[str, ParameterObject]
+    schemas: dict[str, SchemaObject]
 
-    discriminator_base_class_schemas: List[DiscriminatorBaseClassSchema]
+    discriminator_base_class_schemas: list[DiscriminatorBaseClassSchema]
 
     @property
-    def sorted_schemas(self) -> List[SchemaObject]:
-        sorted: List[str] = []
+    def sorted_schemas(self) -> list[SchemaObject]:
+        sorted: list[str] = []
         keys = list(self.schemas.keys())
         while keys:
             key = keys.pop()
             if key in sorted:
                 index = sorted.index(key)
             else:
                 sorted.append(key)
```

### Comparing `pythogen-0.1.9/pythogen/packager.py` & `pythogen-0.2.0/pythogen/packager.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Отвечает за всё, что необходимо сделать (сгенерировать файлы
 зависимостей, инициализаций, конфигураций), чтобы сгенерированный
 клиент можно было упаковать в пакет.
 """
 
 import dataclasses
 from pathlib import Path
-from typing import Optional
 
 from jinja2 import Environment
 from jinja2 import FileSystemLoader
 
 from pythogen import settings
 
 
@@ -20,30 +19,30 @@
 
 
 def init_package(
     *,
     output_path: str,
     client_class_name: str,
     package_version: str,
-    package_authors: Optional[str] = None,
+    package_authors: str | None = None,
 ) -> InitPackageResponse:
     package_name = f"{client_class_name.lower().replace('client', '')}_client"
 
     pyproject_path = Path(output_path).joinpath(package_name)
     pyproject_path.mkdir(parents=True, exist_ok=True)
     _create_pyproject_file(pyproject_path, package_name, package_version, package_authors)
 
     sources_path = pyproject_path.joinpath(package_name)
     sources_path.mkdir(parents=True, exist_ok=True)
     _create_init_file(sources_path, package_name)
 
     return InitPackageResponse(client_output_path=str(sources_path.joinpath(f'{package_name}.py')))
 
 
-def _create_pyproject_file(output_dir: Path, package_name: str, version: str, authors: Optional[str] = None) -> None:
+def _create_pyproject_file(output_dir: Path, package_name: str, version: str, authors: str | None = None) -> None:
     env = Environment(
         loader=FileSystemLoader(settings.TEMPLATES_DIR_PATH),
         extensions=['jinja2.ext.loopcontrols'],
     )
     template = env.get_template('pyproject-toml.j2')
 
     pyproject_path = output_dir.joinpath('pyproject.toml')
```

### Comparing `pythogen-0.1.9/pythogen/parsers/document.py` & `pythogen-0.2.0/pythogen/parsers/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from __future__ import annotations
 
 import logging
-from typing import Dict
-from typing import List
 
 import yaml
 
 from pythogen import models
 from pythogen.parsers.inline_schemas_aggregator import InlineSchemasAggregator
 from pythogen.parsers.operations import OperationParser
 from pythogen.parsers.parameters import ParameterParser
@@ -31,15 +29,15 @@
         Путь до OpenAPI-файла, который необходимо спарсить.
     """
     with open(file_path) as file:
         openapi_data = yaml.load(file, yaml.SafeLoader)
 
     # Сюда будут складываться найденные в процессе парсинга базовые классы,
     # в которых определён дискриминатор.
-    discriminator_base_class_schemas: List[models.DiscriminatorBaseClassSchema] = []
+    discriminator_base_class_schemas: list[models.DiscriminatorBaseClassSchema] = []
     inline_schema_aggregator = InlineSchemasAggregator()
 
     ref_resolver = RefResolver(
         openapi_data=openapi_data,
     )
     schema_parser = SchemaParser(
         ref_resolver=ref_resolver,
@@ -51,14 +49,15 @@
         ref_resolver=ref_resolver,
         schema_parser=schema_parser,
         inline_schema_aggregator=inline_schema_aggregator,
     )
     request_body_parser = RequestBodyParser(
         ref_resolver=ref_resolver,
         schema_parser=schema_parser,
+        inline_schema_aggregator=inline_schema_aggregator,
     )
     parameters_parser = ParameterParser(
         ref_resolver=ref_resolver,
         schema_parser=schema_parser,
         openapi_data=openapi_data,
     )
     operation_parser = OperationParser(
@@ -73,15 +72,15 @@
         schema_parser=schema_parser,
         operation_parser=operation_parser,
         openapi_data=openapi_data,
     )
 
     paths = path_parser.parse_collection()
     schemas = schema_parser.parse_collection()
-    all_schemas: Dict[str, models.SchemaObject] = {
+    all_schemas: dict[str, models.SchemaObject] = {
         **schemas,
         **inline_schema_aggregator.get_mapping(),
     }
 
     document = models.Document(
         info=models.InfoObject(
             title=openapi_data['info']['title'],
```

### Comparing `pythogen-0.1.9/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.2.0/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from typing import Dict
-
 from pythogen.models import SchemaObject
 
 
 class InlineSchemasAggregator:
     def __init__(self):
-        self._id_to_schema_mapping: Dict[str, SchemaObject] = {}
+        self._id_to_schema_mapping: dict[str, SchemaObject] = {}
 
     def add(self, schema_id: str, schema_obj: SchemaObject) -> None:
         # if schema_obj.type is Type.object:
         self._id_to_schema_mapping[schema_id] = schema_obj
 
-    def update(self, id_to_schema_mapping: Dict[str, SchemaObject]) -> None:
+    def update(self, id_to_schema_mapping: dict[str, SchemaObject]) -> None:
         self._id_to_schema_mapping.update(id_to_schema_mapping)
 
-    def get_mapping(self) -> Dict[str, SchemaObject]:
+    def get_mapping(self) -> dict[str, SchemaObject]:
         return self._id_to_schema_mapping
```

### Comparing `pythogen-0.1.9/pythogen/parsers/operations.py` & `pythogen-0.2.0/pythogen/parsers/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from typing import Any
-from typing import Dict
 
 from pythogen import models
 from pythogen.parsers.parameters import ParameterParser
 from pythogen.parsers.references import RefResolver
 from pythogen.parsers.request_body import RequestBodyParser
 from pythogen.parsers.response import ResponseParser
 from pythogen.parsers.schemas import SchemaParser
@@ -25,36 +24,38 @@
         self._ref_resolver = ref_resolver
         self._schema_parser = schema_parser
         self._response_parser = response_parser
         self._request_body_parser = request_body_parser
         self._parameters_parser = parameters_parser
 
     def parse_item(
-        self, path_str: str, method: models.HttpMethod, operation_data: Dict[str, Any]
+        self, path_str: str, method: models.HttpMethod, operation_data: dict[str, Any]
     ) -> models.OperationObject:
         """Спарсить спецификацию метода ручки (POST-, GET-, PUT-запроса и т.п.)"""
-        responses: Dict[str, models.ResponseObject] = {}
+        responses: dict[str, models.ResponseObject] = {}
 
         for status_code, response_data in operation_data['responses'].items():
             if status_code == 'default':
                 logger.error('Unable to parse responses, "default" not implemented yet')
                 continue
 
             if response_data.get('$ref', None):
                 resolved_ref = self._ref_resolver.resolve(response_data['$ref'])
                 response_data = resolved_ref.ref_data
                 response_id = resolved_ref.ref_id
             else:
-                response_id = f"{operation_data['summary'].replace(' ', '')}Response{status_code}"
+                response_id = (
+                    f"{operation_data['operationId'].replace('_', ' ').title().replace(' ', '')}Response{status_code}"
+                )
 
             responses[status_code] = self._response_parser.parse_item(response_id, response_data)
 
         request_body_data = operation_data.get('requestBody')
         if request_body_data:
-            request_body = self._request_body_parser.parse_item(request_body_data)
+            request_body = self._request_body_parser.parse_item(request_body_data, operation_data)
         else:
             request_body = None
 
         parameters = []
         for parameter_data in operation_data.get('parameters', []):
             if parameter_data.get('$ref', None):
                 resolved_ref = self._ref_resolver.resolve(parameter_data['$ref'])
```

### Comparing `pythogen-0.1.9/pythogen/parsers/parameters.py` & `pythogen-0.2.0/pythogen/parsers/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import re
 from typing import Any
-from typing import Dict
 
 from pythogen import models
 from pythogen.parsers.references import RefResolver
 from pythogen.parsers.schemas import SchemaParser
 
 
 class ParameterParser:
-    def __init__(self, ref_resolver: RefResolver, schema_parser: SchemaParser, openapi_data: Dict[str, Any]) -> None:
+    def __init__(self, ref_resolver: RefResolver, schema_parser: SchemaParser, openapi_data: dict[str, Any]) -> None:
         self._openapi_data = openapi_data
         self._ref_resolver = ref_resolver
         self._schema_parser = schema_parser
 
-    def parse_collections(self) -> Dict[str, models.ParameterObject]:
+    def parse_collections(self) -> dict[str, models.ParameterObject]:
         parameters = self._openapi_data["components"].get('parameters', {})
         result = {}
         for parameter_id, parameter_data in parameters.items():
             if parameter_data.get('$ref', None):
                 parameter = self.parse_item_from_ref(parameter_id, parameter_data['$ref'])
             else:
                 parameter = self.parse_item(parameter_id, parameter_data)
             result[parameter_id] = parameter
         return result
 
     def parse_item_from_ref(self, id_: str, ref: str) -> models.ParameterObject:
         resolved_ref = self._ref_resolver.resolve(ref)
         return self.parse_item(id_, resolved_ref.ref_data)
 
-    def parse_item(self, id_: str, data: Dict[str, Any]) -> models.ParameterObject:
+    def parse_item(self, id_: str, data: dict[str, Any]) -> models.ParameterObject:
         schema_data = data['schema']
         if schema_data.get('$ref', None):
             resolved_ref = self._ref_resolver.resolve(schema_data['$ref'])
             schema = self._schema_parser.parse_item(resolved_ref.ref_id, resolved_ref.ref_data)
         else:
             schema = self._schema_parser.parse_item(f'<inline+{models.SchemaObject.__name__}>', schema_data)
```

### Comparing `pythogen-0.1.9/pythogen/parsers/paths.py` & `pythogen-0.2.0/pythogen/parsers/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 from typing import Any
-from typing import Dict
 
 from pythogen import models
 from pythogen.parsers.operations import OperationParser
 
 
 if TYPE_CHECKING:
     from parsers import SchemaParser
@@ -43,30 +42,30 @@
     """
 
     def __init__(
         self,
         ref_resolver: RefResolver,
         schema_parser: SchemaParser,
         operation_parser: OperationParser,
-        openapi_data: Dict[str, Any],
+        openapi_data: dict[str, Any],
     ) -> None:
         self._openapi_data = openapi_data
         self._ref_resolver = ref_resolver
         self._schema_parser = schema_parser
         self._operation_parser = operation_parser
 
-    def parse_collection(self) -> Dict[str, models.PathItemObject]:
+    def parse_collection(self) -> dict[str, models.PathItemObject]:
         """Спарсить спецификацию всех ручек из OpenAPI-спеки"""
-        parsed_paths: Dict[str, models.PathItemObject] = {}
+        parsed_paths: dict[str, models.PathItemObject] = {}
         paths = self._openapi_data.get('paths', {})
         for path_str, path_item_data in paths.items():
             parsed_paths[path_str] = self.parse_item(path_str, path_item_data)
         return parsed_paths
 
-    def parse_item(self, path_str: str, path_data: Dict[str, Any]) -> models.PathItemObject:
+    def parse_item(self, path_str: str, path_data: dict[str, Any]) -> models.PathItemObject:
         """Спарсить спецификацию ручки"""
         operations = {}
 
         for method in models.HttpMethod:
             if method.value not in path_data:
                 continue
```

### Comparing `pythogen-0.1.9/pythogen/parsers/references.py` & `pythogen-0.2.0/pythogen/parsers/references.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from dataclasses import dataclass
 from typing import Any
-from typing import Dict
 
 
 @dataclass
 class ResolvedRef:
     ref_data: Any
     ref_id: str
 
 
 class RefResolver:
     """
     Отвечает за получение данных из указанного $ref пути.
     """
 
-    def __init__(self, openapi_data: Dict[str, Any]) -> None:
+    def __init__(self, openapi_data: dict[str, Any]) -> None:
         self._openapi_data = openapi_data
 
     def resolve(self, ref: str) -> ResolvedRef:
         """
         Получить данные из указзаного $ref-пути
 
         Parameters
```

### Comparing `pythogen-0.1.9/pythogen/parsers/request_body.py` & `pythogen-0.2.0/pythogen/parsers/request_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 import logging
 from typing import Any
-from typing import Dict
 
 from pythogen import models
 from pythogen.parsers import constants
+from pythogen.parsers.inline_schemas_aggregator import InlineSchemasAggregator
 from pythogen.parsers.references import RefResolver
 from pythogen.parsers.schemas import SchemaParser
 
 
 logger = logging.getLogger(__name__)
 
 
 class RequestBodyParser:
-    def __init__(self, ref_resolver: RefResolver, schema_parser: SchemaParser) -> None:
+    def __init__(
+        self,
+        ref_resolver: RefResolver,
+        schema_parser: SchemaParser,
+        inline_schema_aggregator: InlineSchemasAggregator,
+    ) -> None:
         self._ref_resolver = ref_resolver
         self._schema_parser = schema_parser
+        self._inline_schema_aggregator = inline_schema_aggregator
 
-    def parse_item(self, request_body_data: Dict[str, Any]) -> models.RequestBodyObject:
+    def parse_item(self, request_body_data: dict[str, Any], operation_data: dict[str, Any]) -> models.RequestBodyObject:
         """Спарсить спецификацию тела ручки"""
         if request_body_data.get('$ref', None):
             resolved_ref = self._ref_resolver.resolve(request_body_data['$ref'])
             data = resolved_ref.ref_data
             id_ = resolved_ref.ref_id
         else:
             data = request_body_data
-            id_ = f'<inline+{models.RequestBodyObject.__name__}>'
+            id_ = f"{operation_data['operationId'].replace('_', ' ').title().replace(' ', '')}RequestBody"
 
         files_required = False
         content = data.get('content')
         if content:
             media_types = list(content.keys())
             if len(media_types) > 1:
                 logger.error(f'Unable to parse request body "{id_}", multiple media types not implemented yet')
             media_type = media_types[0]
             media_type_data = content[media_type]
             schema_data = media_type_data['schema']
             if schema_data.get('$ref', None):
                 resolved_ref = self._ref_resolver.resolve(schema_data['$ref'])
                 schema = self._schema_parser.parse_item(resolved_ref.ref_id, resolved_ref.ref_data)
             else:
-                schema = self._schema_parser.parse_item(f'<inline+{models.SchemaObject.__name__}>', schema_data)
+                schema = self._schema_parser.parse_item(id_, schema_data)
+                self._inline_schema_aggregator.add(id_, schema)
 
             if media_type == constants.MULTIPART_FORM_DATA_TYPE:
                 files_required = self._drop_binary_strings(schema_data)
         else:
             raise Exception(f'Unable to parse request body "{id_}", field "content" must be specified')
 
         type_schema_dict_keys = data.get('content', {}).keys()
```

### Comparing `pythogen-0.1.9/pythogen/parsers/response.py` & `pythogen-0.2.0/pythogen/parsers/response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from typing import Any
-from typing import Dict
 
 from pythogen import models
 from pythogen.parsers.inline_schemas_aggregator import InlineSchemasAggregator
 from pythogen.parsers.references import RefResolver
 from pythogen.parsers.schemas import SchemaParser
 
 
@@ -18,15 +17,15 @@
         schema_parser: SchemaParser,
         inline_schema_aggregator: InlineSchemasAggregator,
     ) -> None:
         self._ref_resolver = ref_resolver
         self._schema_parser = schema_parser
         self._inline_schema_aggregator = inline_schema_aggregator
 
-    def parse_item(self, response_id: str, response_data: Dict[str, Any]) -> models.ResponseObject:
+    def parse_item(self, response_id: str, response_data: dict[str, Any]) -> models.ResponseObject:
         """Спарсить спецификацию ответа ручки"""
         schema = None
 
         content = response_data.get('content')
         if content:
             media_types = list(content.keys())
             if len(media_types) > 1:
```

### Comparing `pythogen-0.1.9/pythogen/parsers/schemas.py` & `pythogen-0.2.0/pythogen/parsers/schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import re
 from collections import defaultdict
 from typing import Any
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Union
 
 from pythogen import models
 from pythogen.parsers.inline_schemas_aggregator import InlineSchemasAggregator
 from pythogen.parsers.references import RefResolver
 
 
 PRIMITIVE_TYPES = ('string', 'number', 'integer', 'boolean')
@@ -39,27 +35,27 @@
         Schema2: ...
     ```
     """
 
     def __init__(
         self,
         ref_resolver: RefResolver,
-        openapi_data: Dict[str, Any],
-        discriminator_base_class_schemas: List[models.DiscriminatorBaseClassSchema],
+        openapi_data: dict[str, Any],
+        discriminator_base_class_schemas: list[models.DiscriminatorBaseClassSchema],
         inline_schema_aggregator: InlineSchemasAggregator,
     ) -> None:
         self._openapi_data = openapi_data
         self._ref_resolver = ref_resolver
         self._discriminator_base_class_schemas = discriminator_base_class_schemas
         self._inline_schema_aggregator = inline_schema_aggregator
 
         self._schema_ids = list(self._openapi_data["components"].get('schemas', {}))
         self._processiong_parsed_schema_id_count: dict[str, int] = defaultdict(int)
 
-    def parse_collection(self) -> Dict[str, models.SchemaObject]:
+    def parse_collection(self) -> dict[str, models.SchemaObject]:
         schemas_data = self._openapi_data["components"].get('schemas', {})
         schemas = {}
         for schema_id, schema_data in schemas_data.items():
             if schema_data.get('$ref', None):
                 resolved_ref = self._ref_resolver.resolve(schema_data['$ref'])
                 schema = self.parse_item(resolved_ref.ref_id, resolved_ref.ref_data)
             else:
@@ -67,15 +63,15 @@
 
             if not schema.is_fake:
                 schemas[schema_id] = schema
 
         return schemas
 
     def parse_item(
-        self, schema_id: str, schema_data: Dict[str, Any], from_depth_level: bool = False
+        self, schema_id: str, schema_data: dict[str, Any], from_depth_level: bool = False
     ) -> models.SchemaObject:
         """Спарсить схему из OpenAPI-спеки
 
         Attributes
         ----------
         schema_id
             Идентификатор схемы (ключ в поле components -> schemas)
@@ -124,69 +120,69 @@
             type=schema_type,
             format=self._parse_format(schema_data),
             items=self._parse_items(schema_id, schema_data),
             properties=self._parse_properties(schema_type, schema_data),
             description=self._get_description(schema_data),
         )
 
-    def _parse_type(self, data: Dict[str, Any]) -> models.Type:
+    def _parse_type(self, data: dict[str, Any]) -> models.Type:
         if data == {}:
             # Парсинг пустой схемы
             # application/json:
             #   schema:
             #     {}
             data_type = models.Type.object
         elif 'allOf' in data:
             data_type = models.Type.object
         elif 'anyOf' in data:
             data_type = models.Type.any_of
         else:
-            raw_data_type: Optional[str] = data.get('type')
+            raw_data_type: str | None = data.get('type')
             try:
                 data_type = models.Type(raw_data_type)
             except ValueError:
                 raise Exception(f'Unable to parse schema "{id}", unknown type "{raw_data_type}" on "{data}"')
         return data_type
 
-    def _parse_format(self, data: Dict[str, Any]) -> Optional[models.Format]:
+    def _parse_format(self, data: dict[str, Any]) -> models.Format | None:
         data_format = data.get('format')
         if data_format:
             try:
                 return models.Format[data_format.replace('-', '_')]
             except Exception:
                 raise Exception(f'Unable to parse schema "{id}", unknown format "{data_format}"')
         return None
 
-    def _get_description(self, data: Dict[str, Any]) -> Optional[str]:
+    def _get_description(self, data: dict[str, Any]) -> str | None:
         description = data.get("description", "")
         if description:
             description = description.replace("\n", "\\n")
             description = description.replace("'", "\\'")
             description = description.replace('"', '\\"')
         return description
 
     def _get_discriminator_base_class_schema(
         self,
-        data: Dict[str, Any],
-    ) -> Optional[models.DiscriminatorBaseClassSchema]:
+        data: dict[str, Any],
+    ) -> models.DiscriminatorBaseClassSchema | None:
         description = data.get("description", "")
         if "__discriminator__" not in description:
             return None
         matches = re.findall(r"(__discriminator__)\((.+)\.(.+)\)", description)
         _, class_name, attr = matches[0]
         return models.DiscriminatorBaseClassSchema(
             name=class_name,
             attr=attr,
         )
 
     def _parse_properties(
         self,
         schema_type: models.Type,
-        data: Dict[str, Any],
-    ) -> List[models.SchemaProperty]:
+        data: dict[str, Any],
+    ) -> list[models.SchemaProperty]:
         data_format = data.get('format')
         if data_format:
             try:
                 data_format = models.Format[data_format.replace('-', '_')]
             except Exception:
                 raise Exception(f'Unable to parse schema "{id}", unknown format "{data_format}"')
 
@@ -303,16 +299,16 @@
                 )
 
         return properties
 
     def _parse_items(
         self,
         parent_schema_id: str,
-        data: Dict[str, Any],
-    ) -> Union[Optional[models.SchemaObject], List[models.SchemaObject]]:
+        data: dict[str, Any],
+    ) -> models.SchemaObject | list[models.SchemaObject] | None:
         items_schema_data = data.get('items')
         if items_schema_data:
             if items_schema_data.get('$ref', None):
                 resolved_ref = self._ref_resolver.resolve(items_schema_data['$ref'])
                 schema = self.parse_item(resolved_ref.ref_id, resolved_ref.ref_data, from_depth_level=True)
                 return schema
             elif items_schema_data.get('anyOf'):
@@ -363,13 +359,32 @@
                     self._inline_schema_aggregator.add(items_schema_id, schema)
                 return schema
 
         if data.get('anyOf'):
             items = []
             for any_ref_item in data['anyOf']:
                 ref = any_ref_item.get('$ref', None)
-                resolved_ref = self._ref_resolver.resolve(ref)
-                ref_schema = self.parse_item(resolved_ref.ref_id, resolved_ref.ref_data, from_depth_level=True)
-                items.append(ref_schema)
+                any_ref_any_type = any_ref_item.get('type')
+                if ref:
+                    resolved_ref = self._ref_resolver.resolve(ref)
+                    ref_schema = self.parse_item(resolved_ref.ref_id, resolved_ref.ref_data, from_depth_level=True)
+                    items.append(ref_schema)
+                elif any_ref_any_type in PRIMITIVE_TYPES:
+                    items.append(
+                        models.SchemaObject(
+                            id='',
+                            type=models.Type(any_ref_any_type),
+                            enum=None,
+                            properties=[],
+                            title=None,
+                            format=None,
+                            items=None,
+                            required=None,
+                        )
+                    )
+                else:
+                    items_schema_id = f'<inline+{models.SchemaObject.__name__}>'
+                    schema = self.parse_item(items_schema_id, items_schema_data)  # type: ignore
+                    self._inline_schema_aggregator.add(items_schema_id, schema)
             return items
 
         return None
```

### Comparing `pythogen-0.1.9/pythogen/renderer.py` & `pythogen-0.2.0/pythogen/renderer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """
 Responsible for rendering/generating client code from data
 that was parsed from an OpenAPI file.
 """
-
-
 import logging
 from dataclasses import dataclass
-from typing import Dict
 from typing import Generic
-from typing import List
-from typing import Tuple
 from typing import TypeVar
 
+import autoflake
+import black
 import inflection
+import isort
 from jinja2 import Environment
 from jinja2 import FileSystemLoader
 
 from pythogen import models
 from pythogen import settings
 
 
 PathStr = TypeVar('PathStr', bound=str)
 
 
 logger = logging.getLogger(__name__)
 
 
-def render_client(*, output_path: str, document: models.Document, name: str, sync: bool, metrics: bool) -> None:
+def render_client(
+    *,
+    output_path: str,
+    document: models.Document,
+    name: str,
+    sync: bool,
+    metrics: bool,
+    required_headers: list[str] | None = None,
+) -> None:
     """Отрисовывает сгенерированный клиент на основе j2-шаблонов
 
     Arguments
     ---------
     output_path
         Пудо до файла, в который запишется сгенерированный клиент
     document
@@ -47,39 +53,53 @@
             'iterresponsemap': iterresponsemap,
         },
     )
 
     prepared_operations = prepare_operations(document)
 
     rendered_client = template.render(
+        document=document,
         name=name,
         version=document.info.version,
         models=document.sorted_schemas,
         get=prepared_operations.get,
         post=prepared_operations.post,
         patch=prepared_operations.patch,
         post_no_body=prepared_operations.post_no_body,
         put=prepared_operations.put,
         delete_no_body=prepared_operations.delete_no_body,
         sync=sync,
         metrics=metrics,
         discriminator_base_class_schemas=document.discriminator_base_class_schemas,
+        required_headers=required_headers,
+    )
+    rendered_client = black.format_str(rendered_client, mode=black.FileMode())
+    rendered_client = isort.code(
+        rendered_client,
+        force_grid_wrap=2,
+        lines_after_imports=2,
+        force_single_line=True,
+        line_length=120,
+    )
+    rendered_client = autoflake.fix_code(
+        rendered_client,
+        remove_all_unused_imports=True,
     )
     with open(output_path, 'w') as output_file:
         output_file.write(rendered_client)
 
 
 @dataclass
 class PreparedOperations(Generic[PathStr]):
-    get: Dict[PathStr, models.OperationObject]
-    post: Dict[PathStr, models.OperationObject]
-    post_no_body: Dict[PathStr, models.OperationObject]
-    put: Dict[PathStr, models.OperationObject]
-    patch: Dict[PathStr, models.OperationObject]
-    delete_no_body: Dict[PathStr, models.OperationObject]
+    get: dict[PathStr, models.OperationObject]
+    post: dict[PathStr, models.OperationObject]
+    post_no_body: dict[PathStr, models.OperationObject]
+    put: dict[PathStr, models.OperationObject]
+    patch: dict[PathStr, models.OperationObject]
+    delete_no_body: dict[PathStr, models.OperationObject]
 
 
 def prepare_operations(document: models.Document) -> PreparedOperations:
     prepared_operations: PreparedOperations = PreparedOperations(
         get={},
         post={},
         post_no_body={},
@@ -102,25 +122,25 @@
                 prepared_operations.delete_no_body[path] = operation
             else:
                 logger.error(f'Unable to parse document, "{method}" operations support not implemented yet')
 
     return prepared_operations
 
 
-def iterresponsemap(responses: models.ResponsesObject) -> List[Tuple[str, str]]:
+def iterresponsemap(responses: models.ResponsesObject) -> list[tuple[str, str]]:
     mapping = []
 
     for code, response in responses.patterned.items():
         if response.schema is None:
             mapper = 'EmptyBody(status_code=response.status_code, text=response.text)'
             mapping.append((code, mapper))
             continue
 
         if response.schema.type == models.Type.object:
-            mapper = f'{classname(response.schema.id)}.parse_obj(response.json())'
+            mapper = f'{classname(response.schema.id)}.model_validate(response.json())'
             mapping.append((code, mapper))
             continue
 
         if response.schema.type == models.Type.any_of and isinstance(response.schema.items, list):
             items_class_names = [classname(items.id) for items in response.schema.items]
             items_class_names_str: str = '[' + ', '.join(items_class_names) + ']'
             mapper = f'self._parse_any_of(response.json(), {items_class_names_str})'
@@ -137,15 +157,15 @@
                 if items is None:
                     mapper = 'EmptyBody(status_code=response.status_code, text=response.text)'
                     mapping.append((code, mapper))
                     continue
 
                 if items.type is models.Type.object:
                     items_class_name = classname(items.id)
-                    mapper = f'[{items_class_name}.parse_obj(item) for item in response.json()]'
+                    mapper = f'[{items_class_name}.model_validate(item) for item in response.json()]'
                     mapping.append((code, mapper))
                     continue
 
                 mapper = f'response.json()'
                 mapping.append((code, mapper))
                 continue
             continue
@@ -186,36 +206,39 @@
 
     types = list(set(types))
 
     if not types:
         return 'None'
 
     elif len(types) == 1:
-        return f'Optional[{types[0]}]'
+        return f'{types[0]} | None'
     else:
-        union_args = ', '.join(types)
-        return f'Union[{union_args}]'
+        return ' | '.join(types)
 
 
-def j2_typerepr(schema: models.SchemaObject) -> str:
+def j2_typerepr(schema: models.SchemaObject, document: models.Document | None = None) -> str:
     """Represent data type on j2 template"""
     primitive_type_mapping = {
         models.Type.integer: 'int',
         models.Type.number: 'float',
         models.Type.boolean: 'bool',
         models.Type.string: 'str',
     }
     format_mapping = {
         models.Format.binary: 'bytes',
         models.Format.uri: 'HttpUrl',
-        models.Format.date: 'date',
-        models.Format.date_time: 'datetime',
+        models.Format.date: 'datetime.date',
+        models.Format.date_time: 'datetime.datetime',
     }
 
-    representation = 'Dict'
+    # TODO: всегда передавать document в функцию
+    if document:
+        schema = document.schemas.get(schema.id, schema)
+
+    representation = 'dict'
 
     if schema.type in primitive_type_mapping:
         if schema.enum:
             representation = f'Literal{schema.enum}'
         elif schema.format in format_mapping:
             representation = format_mapping[schema.format]  # type: ignore
         else:
@@ -230,28 +253,28 @@
             primitive_items = []
             for item in schema.items.items:  # type: ignore
                 if item.id:
                     class_items.append(classname(item.id))
                 else:
                     primitive_items.append(primitive_type_mapping[item.type])
 
-            class_items_str = ', '.join([f'{class_item}' for class_item in class_items])
-            primitives_items_str = ', '.join(primitive_items)
+            class_items_str = ' | '.join([f'{class_item}' for class_item in class_items])
+            primitives_items_str = ' | '.join(primitive_items)
 
             items = []
             if class_items_str:
                 items.append(class_items_str)
             if primitives_items_str:
                 items.append(primitives_items_str)
 
-            items_str = ', '.join(items)
-            representation = f'List[Union[{items_str}]]'
+            items_str = ' | '.join(items)
+            representation = f'list[{items_str}]'
         else:
             item = j2_typerepr(schema.items)  # type: ignore
-            representation = f'List[{item}]'
+            representation = f'list[{item}]'
 
     elif schema.type == models.Type.any_of:
         representation = classname(schema.id)
 
     return representation
```

### Comparing `pythogen-0.1.9/pythogen/templates/client/httpx-method.j2` & `pythogen-0.2.0/pythogen/templates/client/httpx-method.j2`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     {%- if sync %}
     def {{ operation.fn_name }}(
     {%- else %}
     async def {{ operation.fn_name }}(
     {%- endif %}
         self,
         {%- if operation.request_body and operation.request_body.is_multipart_form_data and operation.request_body.are_files_required %}
-        files: Union[Mapping[str, FileTypes], Sequence[Tuple[str, FileTypes]]],
+        files: Mapping[str, FileTypes] | Sequence[tuple[str, FileTypes]],
         {%- endif %}
         {#- path params -#}
         {%- for parameter in operation.path_params %}
         {{ parameter.key }}: {{ typerepr(parameter.schema) }},
         {%- endfor %}
         {#- required query params -#}
         {%- for parameter in operation.query_params -%}
@@ -21,33 +21,34 @@
         {#- required headers -#}
         {%- for parameter in operation.headers -%}
         {%- if parameter.required %}
         {{ varname(parameter.key) }}: {{ typerepr(parameter.schema) }},
         {%- endif %}
         {%- endfor %}
         {%- if operation.request_body %}
-        body: Optional[Union[{{ typerepr(operation.request_body.schema) }}, Dict[str, Any]]] = None,
+        body: {{ typerepr(operation.request_body.schema) }} | dict[str, Any] | None = None,
         {%- endif %}
         {#- optional query params -#}
         {%- for parameter in operation.query_params -%}
         {%- if not parameter.required %}
-        {{ varname(parameter.key) }}: Optional[{{ typerepr(parameter.schema) }}] = None,
+        {{ varname(parameter.key) }}: {{ typerepr(parameter.schema) }} | None = None,
         {%- endif %}
         {%- endfor %}
         {#- optional headers -#}
         {%- for parameter in operation.headers -%}
         {%- if not parameter.required %}
-        {{ varname(parameter.key) }}: Optional[{{ typerepr(parameter.schema) }}] = None,
+        {{ varname(parameter.key) }}: {{ typerepr(parameter.schema) }} | None = None,
         {%- endif %}
         {%- endfor %}
-        auth: Optional[BasicAuth] = None,
-        content: Optional[Union[str, bytes]] = None,
+        auth: BasicAuth | None = None,
+        content: str | bytes | None = None,
         {%- if operation.request_body and operation.request_body.is_multipart_form_data and not operation.request_body.are_files_required %}
-        files: Optional[Union[Mapping[str, FileTypes], Sequence[Tuple[str, FileTypes]]]] = None,
+        files: Mapping[str, FileTypes] | Sequence[tuple[str, FileTypes]] | None = None,
         {%- endif %}
+        headers: dict[str, Any] | None = None,
     ) -> {{ responserepr(operation.responses) }}:
         url = self._get_url(f'{{ path }}')
 
         params = {
             {%- for parameter in operation.query_params %}
             {%- if parameter.required %}
             '{{ parameter.orig_key }}': {{ varname(parameter.key) }},
@@ -82,41 +83,55 @@
             auth_ = auth
         else:
             auth_ = (auth.username, auth.password)
         {% if operation.request_body %}
         if isinstance(body, dict):
             json = body
         elif isinstance(body, {{typerepr(operation.request_body.schema)}}):
-            json = body.dict()
+            json = body.model_dump(by_alias=True)
         else:
             json = None
         {% endif %}
 
         {%- if operation.request_body and operation.request_body.is_form_data %}
         headers_.update({'Content-Type': 'application/x-www-form-urlencoded'})
         {%- elif operation.request_body and operation.request_body.is_multipart_form_data %}
         # Content-Type=multipart/form-data doesn't work, because header MUST contain boundaries
         # let library do it for us
         headers_.pop("Content-Type", None)
         {% endif %}
-
+        if headers:
+            headers_ = headers
 
 {%- with req_body=operation.request_body -%}
 {% include 'client/httpx-request-metrics.j2' %}
-{%- endwith -%}
+{%- endwith %}
+        req = RequestBox(
+            client_name=self.client_name,
+            method="{{ method }}",
+            url=url,
+            params=params,
+            headers=headers_,
+            content=content,
+        )
+
+        resp = ResponseBox(
+            status_code=response.status_code,
+        )
 
         {%- for code, mapper in iterresponsemap(operation.responses) %}
 
         if response.status_code == {{ code }}:
             {% if code | int >= 400 -%}
             method = "{{ method }}"
             if response.content is None:
                 content = None
             else:
                 content = response.content[:500]
 
-            self.log_error(self.client_name, method, url, params, content, headers_)
+            if self.logs_integration:
+                self.logs_integration.log_error(req, resp)
 
             {% endif -%}
             return {{ mapper }}
         {%- endfor %}
     {%endfor %}
```

### Comparing `pythogen-0.1.9/pythogen/templates/client/httpx-request-metrics.j2` & `pythogen-0.2.0/pythogen/templates/client/httpx-request-metrics.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.9/pythogen/templates/httpx.j2` & `pythogen-0.2.0/pythogen/templates/httpx.j2`

 * *Files 21% similar despite different names*

```diff
@@ -9,28 +9,23 @@
 
 # jinja2: lstrip_blocks: "True"
 # mypy: ignore-errors
 
 from __future__ import annotations
 
 import abc
+from dataclasses import dataclass
 
-from datetime import datetime
-from datetime import date
+import datetime
 
 from httpx import Timeout
-try:
-    from typing import Literal
-except ImportError:
-    from typing_extensions import Literal
-from typing import List
-from typing import Tuple
+from typing import Literal
+
 from typing import Any
-from typing import Dict
-from typing import Optional
+
 from typing import Union
 from typing import Callable
 from typing import get_type_hints
 from typing import Mapping
 from typing import Sequence
 from typing import IO
 from typing import cast
@@ -38,34 +33,35 @@
 {%- if metrics %}
 from prometheus_client import Counter
 from prometheus_client import Histogram
 {%- endif %}
 import httpx
 from pydantic import BaseModel
 from pydantic import Field
-from pydantic import root_validator
-from pydantic import validator
+from pydantic import field_validator
+from pydantic import FieldValidationInfo
+from pydantic import ConfigDict
 from pydantic import HttpUrl
+from pydantic import RootModel
 import logging
 from functools import wraps
-from opentracing.ext import tags
 
 
 # backward compatibility for httpx<0.18.2
 try:
     DEFAULT_AUTH = httpx.USE_CLIENT_DEFAULT
 except AttributeError:
     DEFAULT_AUTH = None
 
 {%- if metrics %}
 class BaseMetricsIntegration(abc.ABC):
     def __init__(
         self,
-        client_response_time_histogram: Optional[Histogram] = None,
-        client_non_http_errors_counter: Optional[Counter] = None,
+        client_response_time_histogram: Histogram | None = None,
+        client_non_http_errors_counter: Counter | None = None,
         shadow_path: bool = True,
     ):
         self._client_response_time_histogram = client_response_time_histogram
         self._client_non_http_errors_counter = client_non_http_errors_counter
         self.shadow_path = shadow_path
 
     @abc.abstractmethod
@@ -90,101 +86,164 @@
             client_name=client_name,
             http_method=http_method,
             http_target=http_target,
             http_status_code=response.status_code,
         ).observe(response.elapsed.total_seconds())
 {%- endif %}
 
+
+@dataclass
+class RequestBox:
+    client_name: str
+    method: str
+    url: str
+    params: dict[str, Any]
+    headers: dict[str, Any]
+    content: Any
+
+
+@dataclass
+class ResponseBox:
+    status_code: int
+
+
+class BaseLogsIntegration(abc.ABC):
+    @abc.abstractmethod
+    def log_extra(self, **kwargs: Any) -> dict[str, Any]: ...
+
+    @abc.abstractmethod
+    def log_error(self, req: RequestBox, resp: ResponseBox) -> None: ...
+
+    @abc.abstractmethod
+    def get_log_error_level(self, req: RequestBox, resp: ResponseBox) -> int: ...
+
+
+class DefaultLogsIntegration(BaseLogsIntegration):
+    def log_extra(self, **kwargs: Any) -> dict[str, Any]:
+        return {'props': {'data': kwargs}}
+
+    def log_error(self, req: RequestBox, resp: ResponseBox) -> None:
+        msg = f"request error"
+        msg += f" | client={req.client_name}"
+        msg += f" | method={req.method}"
+        msg += f" | url={req.url}"
+        msg += f" | params={req.params}"
+        msg += f" | content={req.content}"
+        msg += f" | headers={req.headers}"
+
+        level = self.get_log_error_level(req, resp)
+
+        logging.log(
+            level,
+            msg,
+            extra=self.log_extra(
+                client=req.client_name,
+                method=req.method,
+                content=req.content,
+                url=req.url,
+                params=req.params,
+            ),
+        )
+
+    def get_log_error_level(self, req: RequestBox, resp: ResponseBox) -> int:
+        if resp.status_code >= 500:
+            return logging.ERROR
+        elif resp.status_code >= 400:
+            return logging.WARNING
+        elif resp.status_code >= 300:
+            return logging.INFO
+        elif resp.status_code >= 200:
+            return logging.INFO
+        else:
+            return logging.INFO
+
 FileContent = Union[IO[str], IO[bytes], str, bytes]
 FileTypes = Union[
     # file (or text)
     FileContent,
     # (filename, file (or text))
-    Tuple[Optional[str], FileContent],
+    tuple[str | None, FileContent],
     # (filename, file (or text), content_type)
-    Tuple[Optional[str], FileContent, Optional[str]],
+    tuple[str | None, FileContent, str | None],
 ]
 
+
+class RequiredHeaders(Exception):
+    ...
+
+
 class EmptyBody(BaseModel):
     status_code: int
     text: str
 
 {% for schema in discriminator_base_class_schemas %}
 class {{ schema.name }}(BaseModel):
     {{ schema.attr }}: str
 
-    @validator("{{ schema.attr }}", pre=True)
-    def check(cls, v: str) -> str:
+    @field_validator("{{ schema.attr }}", mode='before')
+    def check(cls, v: str, info: FieldValidationInfo) -> str:
         type_hints = get_type_hints(cls)
-        {{ schema.attr }}_values: Tuple[str] = type_hints["{{ schema.attr }}"].__dict__['__args__']
+        {{ schema.attr }}_values: tuple[str] = type_hints["{{ schema.attr }}"].__dict__['__args__']
 
         if v not in {{ schema.attr }}_values:
             raise ValueError(f'invalid {{ schema.attr }} for {cls}')
 
         return v
 {%- endfor %}
 
 
 {%- for model in models %}
 
+{%- if model.type.value == "any_of"  %}
+class {{ classname(model.id) }}(RootModel):
+    root: list[
+    {% set pipe = joiner(" | ") %}
+    {%- for item in model.items %}
+        {{ pipe() }}{{ item.id }}
+    {%- endfor %}
+    ]
+
+    def __iter__(self):
+        return iter(self.root)
+
+    def __getitem__(self, item):
+        return self.root[item]
 
+{%- else %}
 class {{ classname(model.id) }}(BaseModel):
     """
     {{ model.title }}
     """
+    model_config = ConfigDict(
+        populate_by_name=True,  # Addressing by field name, even if there is an alias.
+    )
 
-    {%- if model.type.value == "any_of"  %}
-    __root__: Union[
-    {%- for item in model.items %}
-        '{{ item.id }}',
-    {%- endfor %}
-    ]
-    {%- else %}
-
-    # required ---
+    {% if model.required_properties|length > 0 %}# required ---{% endif %}
     {%- for property in model.required_properties %}
         {%- if property.schema.description %}
-    {{ property.key }}: {{ typerepr(property.schema) }} = Field(description="{{ property.schema.description }}"{%- if property.safety_key %}, alias="{{ property.orig_key }}"{%- endif %})
+    {{ property.key }}: {{ typerepr(property.schema, document) }} = Field(description="{{ property.schema.description }}"{%- if property.safety_key %}, alias="{{ property.orig_key }}"{%- endif %})
         {%- else %}
-    {{ property.key }}: {{ typerepr(property.schema) }}
+    {{ property.key }}: {{ typerepr(property.schema, document) }}
         {%- endif %}
     {%- endfor %}
 
-    # optional ---
+    {% if model.optional_properties|length > 0 %}# optional ---{% endif %}
     {%- for property in model.optional_properties %}
         {%- if property.schema.description %}
-    {{ property.key }}: Optional[{{ typerepr(property.schema) }}] = Field(description="{{ property.schema.description }}"{%- if property.safety_key %}, alias="{{ property.orig_key }}"{%- endif %})
+    {{ property.key }}: {{ typerepr(property.schema, document) }} | None = Field(None, description="{{ property.schema.description }}"{%- if property.safety_key %}, alias="{{ property.orig_key }}"{%- endif %})
         {%- else %}
-    {{ property.key }}: Optional[{{ typerepr(property.schema) }}] = None
+    {{ property.key }}: {{ typerepr(property.schema, document) }} | None = None
         {%- endif %}
     {%- endfor %}
 
     {%- for property in model.required_properties + model.optional_properties if property.safety_key %}
-
-    class Config:
-        # Обращение по имени поля, даже если есть алиас.
-        allow_population_by_field_name = True
-
-    @root_validator
-    def change_name(cls, values):
-        """
-        Каст полей согласно алиасам
-
-        В OpenApi-спеке названия полей могут быть в формате, в котором
-        нельзя создавать имена переменных в python, они заменяются безопасными алиасами
-        """
-        {%- for property in model.required_properties + model.optional_properties if property.safety_key %}
-        values["{{ property.orig_key }}"] = values["{{ property.safety_key }}"]
-        del values["{{ property.safety_key }}"]
-        {% endfor %}
-        return values
     {%- break %}
     {%- endfor %}
+{% endif %}
 
-    {%- endif %}
 {%- endfor %}
 
 
 class BasicAuth(BaseModel):
     username: str
     password: str
 
@@ -192,34 +251,40 @@
 class {{ name }}:
     def __init__(
         self,
         base_url: str,
         timeout: int = 5,
         client_name: str = "{{ name | replace('Client', '') | lower }}",
         {%- if sync %}
-        client: Optional[httpx.Client] = None,
+        client: httpx.Client | None = None,
         {%- else %}
-        client: Optional[httpx.AsyncClient] = None,
+        client: httpx.AsyncClient | None = None,
         {%- endif %}
-        headers: Optional[Dict[str, str]] = None,
+        headers: dict[str, str] | None = None,
         {%- if metrics %}
-        metrics_integration: Optional[BaseMetricsIntegration] = None,
+        metrics_integration: BaseMetricsIntegration | None = None,
         {%- endif %}
+        logs_integration: BaseLogsIntegration | None = DefaultLogsIntegration(),
     ):
         {%- if sync %}
         self.client = client or httpx.Client(timeout=Timeout(timeout))
         {%- else %}
         self.client = client or httpx.AsyncClient(timeout=Timeout(timeout))
         {%- endif %}
         self.base_url = base_url
         self.headers = headers or {}
         {%- if metrics %}
         self.metrics_integration=metrics_integration
         {%- endif %}
+        self.logs_integration = logs_integration
         self.client_name = client_name
+        {% if required_headers %}
+        if set({{ required_headers }}) != set(self.headers):
+            raise RequiredHeaders("Headers {{ required_headers }} is required")
+        {%- endif %}
 
     {#-  get items begin  #}
     {% with items=get.items(), method='get'%}
     {%- include 'client/httpx-method.j2' %}
     {%- endwith %}
     {#-  get items end  #}
     {#-  post items begin  #}
@@ -249,15 +314,15 @@
     async def close(self) -> None:
         await self.client.aclose()
     {%- endif %}
 
     def _get_url(self, path: str) -> str:
         return f'{self.base_url}{path}'
 
-    def log_extra(self, **kwargs: Any) -> Dict[str, Any]:
+    def log_extra(self, **kwargs: Any) -> dict[str, Any]:
         return {'extra': {'props': {'data': kwargs}}}
 
     def log_error(self, client_name: str, method, url: str, params, content, headers) -> None:
         msg = f"request error"
         msg += f" | client={client_name}"
         msg += f" | method={method}"
         msg += f" | url={url}"
@@ -272,21 +337,21 @@
                 method=method,
                 content=content,
                 url=url,
                 params=params,
             ),
         )
 
-    def _parse_any_of(self, item: Dict[str, Any], schema_classes: List[Any]) -> Any:
+    def _parse_any_of(self, item: dict[str, Any], schema_classes: list[Any]) -> Any:
         for schema_class in schema_classes:
             try:
-                return schema_class.parse_obj(item)
+                return schema_class.model_validate(item)
             except:
                 continue
 
         raise Exception("Can't parse \"{item}\"")
 
 
 
 {% for model in models -%}
-{{ classname(model.id) }}.update_forward_refs()
+{{ classname(model.id) }}.model_rebuild()
 {% endfor %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

