# Comparing `tmp/openapi_pydantic-0.2.2.tar.gz` & `tmp/openapi_pydantic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_pydantic-0.2.2.tar", max compression
+gzip compressed data, was "openapi_pydantic-0.3.0.tar", max compression
```

## Comparing `openapi_pydantic-0.2.2.tar` & `openapi_pydantic-0.3.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0     1896 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/LICENSE
--rw-r--r--   0        0        0     8376 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/README.md
--rw-r--r--   0        0        0     1366 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/__init__.py
--rw-r--r--   0        0        0       26 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/py.typed
--rw-r--r--   0        0        0     5464 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/util.py
--rw-r--r--   0        0        0     1419 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/__init__.py
--rw-r--r--   0        0        0      447 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/parser.py
--rw-r--r--   0        0        0     1603 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/README.md
--rw-r--r--   0        0        0     1941 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/__init__.py
--rw-r--r--   0        0        0      747 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/callback.py
--rw-r--r--   0        0        0     5491 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/components.py
--rw-r--r--   0        0        0      865 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/contact.py
--rw-r--r--   0        0        0      215 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/datatype.py
--rw-r--r--   0        0        0     1282 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/discriminator.py
--rw-r--r--   0        0        0     3141 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/encoding.py
--rw-r--r--   0        0        0     1554 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/example.py
--rw-r--r--   0        0        0      731 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/external_documentation.py
--rw-r--r--   0        0        0     1073 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/header.py
--rw-r--r--   0        0        0     1982 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/info.py
--rw-r--r--   0        0        0      645 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/license.py
--rw-r--r--   0        0        0     2958 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/link.py
--rw-r--r--   0        0        0     2980 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/media_type.py
--rw-r--r--   0        0        0     2125 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/oauth_flow.py
--rw-r--r--   0        0        0      835 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/oauth_flows.py
--rw-r--r--   0        0        0     2684 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/open_api.py
--rw-r--r--   0        0        0     6422 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/operation.py
--rw-r--r--   0        0        0     8047 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/parameter.py
--rw-r--r--   0        0        0     4930 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/path_item.py
--rw-r--r--   0        0        0     1017 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/paths.py
--rw-r--r--   0        0        0      894 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/reference.py
--rw-r--r--   0        0        0     3209 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/request_body.py
--rw-r--r--   0        0        0     3719 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/response.py
--rw-r--r--   0        0        0     2050 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/responses.py
--rw-r--r--   0        0        0    22285 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/schema.py
--rw-r--r--   0        0        0     1325 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/security_requirement.py
--rw-r--r--   0        0        0     3545 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/security_scheme.py
--rw-r--r--   0        0        0     1889 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/server.py
--rw-r--r--   0        0        0     1071 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/server_variable.py
--rw-r--r--   0        0        0      887 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/tag.py
--rw-r--r--   0        0        0     5464 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/util.py
--rw-r--r--   0        0        0     1850 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/xml.py
--rw-r--r--   0        0        0     1663 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/README.md
--rw-r--r--   0        0        0     1941 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/__init__.py
--rw-r--r--   0        0        0      806 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/callback.py
--rw-r--r--   0        0        0     5650 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/components.py
--rw-r--r--   0        0        0      861 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/contact.py
--rw-r--r--   0        0        0      238 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/datatype.py
--rw-r--r--   0        0        0     1282 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/discriminator.py
--rw-r--r--   0        0        0     3573 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/encoding.py
--rw-r--r--   0        0        0     1633 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/example.py
--rw-r--r--   0        0        0      729 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/external_documentation.py
--rw-r--r--   0        0        0     1076 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/header.py
--rw-r--r--   0        0        0     2112 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/info.py
--rw-r--r--   0        0        0     1028 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/license.py
--rw-r--r--   0        0        0     3038 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/link.py
--rw-r--r--   0        0        0     3060 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/media_type.py
--rw-r--r--   0        0        0     2306 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/oauth_flow.py
--rw-r--r--   0        0        0      835 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/oauth_flows.py
--rw-r--r--   0        0        0     3522 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/open_api.py
--rw-r--r--   0        0        0     6704 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/operation.py
--rw-r--r--   0        0        0     8049 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/parameter.py
--rw-r--r--   0        0        0     5010 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/path_item.py
--rw-r--r--   0        0        0     1040 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/paths.py
--rw-r--r--   0        0        0     1463 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/reference.py
--rw-r--r--   0        0        0     3209 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/request_body.py
--rw-r--r--   0        0        0     3545 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/response.py
--rw-r--r--   0        0        0     2048 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/responses.py
--rw-r--r--   0        0        0    38873 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/schema.py
--rw-r--r--   0        0        0     1434 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/security_requirement.py
--rw-r--r--   0        0        0     3932 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/security_scheme.py
--rw-r--r--   0        0        0     1890 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/server.py
--rw-r--r--   0        0        0     1069 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/server_variable.py
--rw-r--r--   0        0        0      887 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/tag.py
--rw-r--r--   0        0        0     1962 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/xml.py
--rw-r--r--   0        0        0     1222 2023-05-21 22:51:37.982565 openapi_pydantic-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     9245 1970-01-01 00:00:00.000000 openapi_pydantic-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1896 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9803 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/README.md
+-rw-r--r--   0        0        0     1417 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/__init__.py
+-rw-r--r--   0        0        0     3180 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/compat.py
+-rw-r--r--   0        0        0       26 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/py.typed
+-rw-r--r--   0        0        0     6860 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/util.py
+-rw-r--r--   0        0        0     1474 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/__init__.py
+-rw-r--r--   0        0        0      849 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/parser.py
+-rw-r--r--   0        0        0     1659 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/README.md
+-rw-r--r--   0        0        0     2297 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/__init__.py
+-rw-r--r--   0        0        0      747 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/callback.py
+-rw-r--r--   0        0        0     4770 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/components.py
+-rw-r--r--   0        0        0     1026 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/contact.py
+-rw-r--r--   0        0        0      283 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/datatype.py
+-rw-r--r--   0        0        0     1419 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/discriminator.py
+-rw-r--r--   0        0        0     3242 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/encoding.py
+-rw-r--r--   0        0        0     1667 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/example.py
+-rw-r--r--   0        0        0      934 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/external_documentation.py
+-rw-r--r--   0        0        0     1836 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/header.py
+-rw-r--r--   0        0        0     2023 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/info.py
+-rw-r--r--   0        0        0      818 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/license.py
+-rw-r--r--   0        0        0     3083 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/link.py
+-rw-r--r--   0        0        0     2940 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/media_type.py
+-rw-r--r--   0        0        0     2058 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/oauth_flow.py
+-rw-r--r--   0        0        0     1008 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/oauth_flows.py
+-rw-r--r--   0        0        0     2857 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/open_api.py
+-rw-r--r--   0        0        0     6103 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/operation.py
+-rw-r--r--   0        0        0     7683 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/parameter.py
+-rw-r--r--   0        0        0     4554 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/path_item.py
+-rw-r--r--   0        0        0     1017 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/paths.py
+-rw-r--r--   0        0        0     1118 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/reference.py
+-rw-r--r--   0        0        0     2836 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/request_body.py
+-rw-r--r--   0        0        0     3198 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/response.py
+-rw-r--r--   0        0        0     2050 2023-07-07 18:59:06.714754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/responses.py
+-rw-r--r--   0        0        0    21668 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/schema.py
+-rw-r--r--   0        0        0     1325 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/security_requirement.py
+-rw-r--r--   0        0        0     3529 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/security_scheme.py
+-rw-r--r--   0        0        0     1906 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/server.py
+-rw-r--r--   0        0        0     1244 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/server_variable.py
+-rw-r--r--   0        0        0     1142 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/tag.py
+-rw-r--r--   0        0        0     7712 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/util.py
+-rw-r--r--   0        0        0     2047 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/xml.py
+-rw-r--r--   0        0        0     1719 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/README.md
+-rw-r--r--   0        0        0     2297 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/callback.py
+-rw-r--r--   0        0        0     4929 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/components.py
+-rw-r--r--   0        0        0     1022 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/contact.py
+-rw-r--r--   0        0        0      238 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/datatype.py
+-rw-r--r--   0        0        0     1419 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/discriminator.py
+-rw-r--r--   0        0        0     3674 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/encoding.py
+-rw-r--r--   0        0        0     1769 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/example.py
+-rw-r--r--   0        0        0      932 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/external_documentation.py
+-rw-r--r--   0        0        0     1835 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/header.py
+-rw-r--r--   0        0        0     2141 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/info.py
+-rw-r--r--   0        0        0     1189 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/license.py
+-rw-r--r--   0        0        0     3163 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/link.py
+-rw-r--r--   0        0        0     3008 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/media_type.py
+-rw-r--r--   0        0        0     2239 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/oauth_flow.py
+-rw-r--r--   0        0        0     1008 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/oauth_flows.py
+-rw-r--r--   0        0        0     3695 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/open_api.py
+-rw-r--r--   0        0        0     6385 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/operation.py
+-rw-r--r--   0        0        0     7685 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/parameter.py
+-rw-r--r--   0        0        0     4634 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/path_item.py
+-rw-r--r--   0        0        0     1040 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/paths.py
+-rw-r--r--   0        0        0     1687 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/reference.py
+-rw-r--r--   0        0        0     2836 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/request_body.py
+-rw-r--r--   0        0        0     3187 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/response.py
+-rw-r--r--   0        0        0     2048 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/responses.py
+-rw-r--r--   0        0        0    38287 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/schema.py
+-rw-r--r--   0        0        0     1434 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/security_requirement.py
+-rw-r--r--   0        0        0     3916 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/security_scheme.py
+-rw-r--r--   0        0        0     1907 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/server.py
+-rw-r--r--   0        0        0     1242 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/server_variable.py
+-rw-r--r--   0        0        0     1142 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/tag.py
+-rw-r--r--   0        0        0     2123 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/xml.py
+-rw-r--r--   0        0        0     1221 2023-07-07 18:59:06.718754 openapi_pydantic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10663 1970-01-01 00:00:00.000000 openapi_pydantic-0.3.0/PKG-INFO
```

### Comparing `openapi_pydantic-0.2.2/LICENSE` & `openapi_pydantic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.2/README.md` & `openapi_pydantic-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # openapi-pydantic
 
 [![PyPI](https://img.shields.io/pypi/v/openapi-pydantic)](https://pypi.org/project/openapi-pydantic/)
 [![PyPI - License](https://img.shields.io/pypi/l/openapi-pydantic)](https://github.com/mike-oakley/openapi-pydantic/blob/main/LICENSE)
 
-OpenAPI schema implemented in [Pydantic](https://github.com/samuelcolvin/pydantic).
+OpenAPI schema implemented in [Pydantic](https://github.com/samuelcolvin/pydantic). Both Pydantic 1.8+ and 2.x are supported.
 
 The naming of the classes follows the schema in 
 [OpenAPI specification](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.1.0.md#schema).
 
+> This library is forked from [OpenAPI Schema Pydantic](https://github.com/kuimono/openapi-schema-pydantic)  (at version [1.2.4](https://github.com/kuimono/openapi-schema-pydantic/releases/tag/v1.2.4)) which is no longer actively maintained.
+
 ## Installation
 
 `pip install openapi-pydantic`
 
 ## Try me
 
 ```python
@@ -31,15 +33,16 @@
                         description="pong"
                     )
                 }
             )
         )
     },
 )
-print(open_api.json(by_alias=True, exclude_none=True, indent=2))
+# Note: for Pydantic 1.x, replace `model_dump_json` with `json`
+print(open_api.model_dump_json(by_alias=True, exclude_none=True, indent=2))
 ```
 
 Result:
 
 ```json
 {
   "openapi": "3.1.0",
@@ -65,73 +68,77 @@
     }
   }
 }
 ```
 
 ## Take advantage of Pydantic
 
-Pydantic is a great tool, allow you to use object / dict / mixed data for for input.
+Pydantic is a great tool. It allows you to use object / dict / mixed data for input.
 
 The following examples give the same OpenAPI result as above:
 
 ```python
 from openapi_pydantic import parse_obj, OpenAPI, PathItem, Response
 
 # Construct OpenAPI from dict, inferring the correct schema version
 open_api = parse_obj({
+    "openapi": "3.1.0",
     "info": {"title": "My own API", "version": "v0.0.1"},
     "paths": {
         "/ping": {
             "get": {"responses": {"200": {"description": "pong"}}}
         }
     },
 })
 
 
 # Construct OpenAPI v3.1.0 schema from dict
-open_api = OpenAPI.parse_obj({
+# Note: for Pydantic 1.x, replace `model_validate` with `parse_obj`
+open_api = OpenAPI.model_validate({
     "info": {"title": "My own API", "version": "v0.0.1"},
     "paths": {
         "/ping": {
             "get": {"responses": {"200": {"description": "pong"}}}
         }
     },
 })
 
 # Construct OpenAPI with mix of dict/object
-open_api = OpenAPI.parse_obj({
+# Note: for Pydantic 1.x, replace `model_validate` with `parse_obj`
+open_api = OpenAPI.model_validate({
     "info": {"title": "My own API", "version": "v0.0.1"},
     "paths": {
         "/ping": PathItem(
             get={"responses": {"200": Response(description="pong")}}
         )
     },
 })
 ```
 
 ## Use Pydantic classes as schema
 
 - The [Schema Object](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md#schemaObject)
-  in OpenAPI has definitions and tweaks in JSON Schema, which is hard to comprehend and define a good data class
-- Pydantic already has a good way to [create JSON schema](https://pydantic-docs.helpmanual.io/usage/schema/),
-  let's not re-invent the wheel
-  
+  in OpenAPI has definitions and tweaks in JSON Schema, which are hard to comprehend and define a good data class
+- Pydantic already has a good way to [create JSON schema](https://pydantic-docs.helpmanual.io/usage/schema/).
+  Let's not reinvent the wheel.
+
 The approach to deal with this:
 
 1. Use `PydanticSchema` objects to represent the `Schema` in `OpenAPI` object
 2. Invoke `construct_open_api_with_schema_class` to resolve the JSON schemas and references
 
 ```python
 from pydantic import BaseModel, Field
 
 from openapi_pydantic import OpenAPI
 from openapi_pydantic.util import PydanticSchema, construct_open_api_with_schema_class
 
 def construct_base_open_api() -> OpenAPI:
-    return OpenAPI.parse_obj({
+    # Note: for Pydantic 1.x, replace `model_validate` with `parse_obj`
+    return OpenAPI.model_validate({
         "info": {"title": "My own API", "version": "v0.0.1"},
         "paths": {
             "/ping": {
                 "post": {
                     "requestBody": {"content": {"application/json": {
                         "schema": PydanticSchema(schema_class=PingRequest)
                     }}},
@@ -156,15 +163,16 @@
     resp_foo: str = Field(description="foo value of the response")
     resp_bar: str = Field(description="bar value of the response")
 
 open_api = construct_base_open_api()
 open_api = construct_open_api_with_schema_class(open_api)
 
 # print the result openapi.json
-print(open_api.json(by_alias=True, exclude_none=True, indent=2))
+# Note: for Pydantic 1.x, replace `model_dump_json` with `json`
+print(open_api.model_dump_json(by_alias=True, exclude_none=True, indent=2))
 ```
 
 Result:
 
 ```json
 {
   "openapi": "3.1.0",
@@ -253,29 +261,32 @@
     }
   }
 }
 ```
 
 ## Notes
 
-### Use of OpenAPI.json() / OpenAPI.dict()
+### Use of OpenAPI.model_dump() / OpenAPI.model_dump_json() / OpenAPI.json() / OpenAPI.dict()
 
-When using `OpenAPI.json()` / `OpenAPI.dict()` function,
-arguments `by_alias=True, exclude_none=True` has to be in place.
-Otherwise the result json will not fit the OpenAPI standard.
+When using `OpenAPI.model_dump()` / `OpenAPI.model_dump_json()` / `OpenAPI.json()` / `OpenAPI.dict()` functions,
+the arguments `by_alias=True, exclude_none=True` have to be in place.
+Otherwise the resulting json will not fit the OpenAPI standard.
 
 ```python
-# OK
+# OK (Pydantic 2)
+open_api.model_dump_json(by_alias=True, exclude_none=True, indent=2)
+# OK (Pydantic 1)
 open_api.json(by_alias=True, exclude_none=True, indent=2)
 
 # Not good
+open_api.model_dump_json(indent=2)
 open_api.json(indent=2)
 ```
 
-More info about field alias:
+More info about field aliases:
 
 | OpenAPI version | Field alias info |
 | --------------- | ---------------- |
 | 3.1.0 | [here](https://github.com/mike-oakley/openapi-pydantic/blob/main/openapi_pydantic/v3/v3_1_0/README.md#alias) |
 | 3.0.3 | [here](https://github.com/mike-oakley/openapi-pydantic/blob/main/openapi_pydantic/v3/v3_0_3/README.md#alias) |
 
 ### Non-pydantic schema types
@@ -287,21 +298,25 @@
 | --------------- | ----------------------------- |
 | 3.1.0 | [here](https://github.com/mike-oakley/openapi-pydantic/blob/main/openapi_pydantic/v3/v3_1_0/README.md#non-pydantic-schema-types) |
 | 3.0.3 | [here](https://github.com/mike-oakley/openapi-pydantic/blob/main/openapi_pydantic/v3/v3_0_3/README.md#non-pydantic-schema-types) |
 
 ### Use OpenAPI 3.0.3 instead of 3.1.0
 
 Some UI renderings (e.g. Swagger) still do not support OpenAPI 3.1.0.
-It is allowed to use the old 3.0.3 version by importing from different paths:
+The old 3.0.3 version is available by importing from different paths:
 
 ```python
 from openapi_pydantic.v3.v3_0_3 import OpenAPI, ...
 from openapi_pydantic.v3.v3_0_3.util import PydanticSchema, construct_open_api_with_schema_class
 ```
 
+### Pydantic version compatibility
+
+Compatibility with both major versions of Pydantic (1.8+ and 2.*) is mostly achieved using a module called `compat.py`. It detects the installed version of Pydantic and exports version-specific symbols for use by the rest of the package. It also provides all symbols necessary for type checking. The `compat.py` module is not intended to be imported by other packages, but other packages may find it helpful as an example of how to span major versions of Pydantic.
+
 ## Credits
 
 This library is based from the original implementation by Kuimono of [OpenAPI Schema Pydantic](https://github.com/kuimono/openapi-schema-pydantic) which is no longer actively maintained.
 
 ## License
 
 [MIT License](https://github.com/mike-oakley/openapi-pydantic/blob/main/LICENSE)
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/__init__.py` & `openapi_pydantic-0.3.0/openapi_pydantic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,9 +29,10 @@
 from .v3 import Schema as Schema
 from .v3 import SecurityRequirement as SecurityRequirement
 from .v3 import SecurityScheme as SecurityScheme
 from .v3 import Server as Server
 from .v3 import ServerVariable as ServerVariable
 from .v3 import Tag as Tag
 from .v3 import parse_obj as parse_obj
+from .v3 import schema_validate as schema_validate
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/__init__.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,7 +27,8 @@
 from .v3_1_0 import Responses as Responses
 from .v3_1_0 import Schema as Schema
 from .v3_1_0 import SecurityRequirement as SecurityRequirement
 from .v3_1_0 import SecurityScheme as SecurityScheme
 from .v3_1_0 import Server as Server
 from .v3_1_0 import ServerVariable as ServerVariable
 from .v3_1_0 import Tag as Tag
+from .v3_1_0 import schema_validate as schema_validate
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/README.md` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 | SecurityScheme | security_scheme_in | in |
 | Schema | schema_format | format |
 | Schema | schema_not | not |
 
 > <a name="header_param_in"></a>The "in" field in Header object is actually a constant (`{"in": "header"}`).
 
 > For convenience of object creation, the classes mentioned in above
-> has configured `allow_population_by_field_name=True`.
+> have configured `allow_population_by_field_name=True` (Pydantic V1) or `populate_by_name=True` (Pydantic V2).
 >
 > Reference: [Pydantic's Model Config](https://pydantic-docs.helpmanual.io/usage/model_config/)
 
 ## Non-pydantic schema types
 
 Due to the constriants of python typing structure (not able to handle dynamic field names),
 the following schema classes are actually just a typing of `Dict`:
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/__init__.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """
-OpenAPI v3.0.3 schema types, created according to the specification:
-https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md
+OpenAPI v3.1.0 schema types, created according to the specification:
+https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.1.0.md
 
 The type orders are according to the contents of the specification:
-https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md#table-of-contents
+https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.1.0.md#table-of-contents
 """
 
+from typing import TYPE_CHECKING
+
+from openapi_pydantic.compat import PYDANTIC_V2
+
 from .callback import Callback as Callback
 from .components import Components as Components
 from .contact import Contact as Contact
 from .datatype import DataType as DataType
 from .discriminator import Discriminator as Discriminator
 from .encoding import Encoding as Encoding
 from .example import Example as Example
@@ -28,18 +32,28 @@
 from .path_item import PathItem as PathItem
 from .paths import Paths as Paths
 from .reference import Reference as Reference
 from .request_body import RequestBody as RequestBody
 from .response import Response as Response
 from .responses import Responses as Responses
 from .schema import Schema as Schema
+from .schema import schema_validate as schema_validate
 from .security_requirement import SecurityRequirement as SecurityRequirement
 from .security_scheme import SecurityScheme as SecurityScheme
 from .server import Server as Server
 from .server_variable import ServerVariable as ServerVariable
 from .tag import Tag as Tag
 from .xml import XML as XML
 
-# resolve forward references
-Encoding.update_forward_refs(Header=Header)
-Schema.update_forward_refs()
-Operation.update_forward_refs(PathItem=PathItem)
+if TYPE_CHECKING:
+    pass
+elif PYDANTIC_V2:
+    # resolve forward references
+    Encoding.model_rebuild()
+    OpenAPI.model_rebuild()
+    Components.model_rebuild()
+    Operation.model_rebuild()
+else:
+    # resolve forward references
+    Encoding.update_forward_refs(Header=Header)
+    Schema.update_forward_refs()
+    Operation.update_forward_refs(PathItem=PathItem)
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/callback.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/components.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,99 @@
 from typing import Dict, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .callback import Callback
 from .example import Example
 from .header import Header
 from .link import Link
 from .parameter import Parameter
 from .reference import Reference
 from .request_body import RequestBody
 from .response import Response
 from .schema import Schema
 from .security_scheme import SecurityScheme
 
+_examples = [
+    {
+        "schemas": {
+            "GeneralError": {
+                "type": "object",
+                "properties": {
+                    "code": {"type": "integer", "format": "int32"},
+                    "message": {"type": "string"},
+                },
+            },
+            "Category": {
+                "type": "object",
+                "properties": {
+                    "id": {"type": "integer", "format": "int64"},
+                    "name": {"type": "string"},
+                },
+            },
+            "Tag": {
+                "type": "object",
+                "properties": {
+                    "id": {"type": "integer", "format": "int64"},
+                    "name": {"type": "string"},
+                },
+            },
+        },
+        "parameters": {
+            "skipParam": {
+                "name": "skip",
+                "in": "query",
+                "description": "number of items to skip",
+                "required": True,
+                "schema": {"type": "integer", "format": "int32"},
+            },
+            "limitParam": {
+                "name": "limit",
+                "in": "query",
+                "description": "max records to return",
+                "required": True,
+                "schema": {"type": "integer", "format": "int32"},
+            },
+        },
+        "responses": {
+            "NotFound": {"description": "Entity not found."},
+            "IllegalInput": {"description": "Illegal input for operation."},
+            "GeneralError": {
+                "description": "General Error",
+                "content": {
+                    "application/json": {
+                        "schema": {"$ref": "#/components/schemas/GeneralError"}
+                    }
+                },
+            },
+        },
+        "securitySchemes": {
+            "api_key": {
+                "type": "apiKey",
+                "name": "api_key",
+                "in": "header",
+            },
+            "petstore_auth": {
+                "type": "oauth2",
+                "flows": {
+                    "implicit": {
+                        "authorizationUrl": "http://example.org/api/oauth/dialog",
+                        "scopes": {
+                            "write:pets": "modify pets in your account",
+                            "read:pets": "read your pets",
+                        },
+                    }
+                },
+            },
+        },
+    }
+]
+
 
 class Components(BaseModel):
     """
     Holds a set of reusable objects for different aspects of the OAS.
     All objects defined within the components object will have no effect on the API
     unless they are explicitly referenced from properties outside the components object.
     """
@@ -44,87 +121,18 @@
 
     links: Optional[Dict[str, Union[Link, Reference]]] = None
     """An object to hold reusable [Link Objects](#linkObject)."""
 
     callbacks: Optional[Dict[str, Union[Callback, Reference]]] = None
     """An object to hold reusable [Callback Objects](#callbackObject)."""
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "schemas": {
-                        "GeneralError": {
-                            "type": "object",
-                            "properties": {
-                                "code": {"type": "integer", "format": "int32"},
-                                "message": {"type": "string"},
-                            },
-                        },
-                        "Category": {
-                            "type": "object",
-                            "properties": {
-                                "id": {"type": "integer", "format": "int64"},
-                                "name": {"type": "string"},
-                            },
-                        },
-                        "Tag": {
-                            "type": "object",
-                            "properties": {
-                                "id": {"type": "integer", "format": "int64"},
-                                "name": {"type": "string"},
-                            },
-                        },
-                    },
-                    "parameters": {
-                        "skipParam": {
-                            "name": "skip",
-                            "in": "query",
-                            "description": "number of items to skip",
-                            "required": True,
-                            "schema": {"type": "integer", "format": "int32"},
-                        },
-                        "limitParam": {
-                            "name": "limit",
-                            "in": "query",
-                            "description": "max records to return",
-                            "required": True,
-                            "schema": {"type": "integer", "format": "int32"},
-                        },
-                    },
-                    "responses": {
-                        "NotFound": {"description": "Entity not found."},
-                        "IllegalInput": {"description": "Illegal input for operation."},
-                        "GeneralError": {
-                            "description": "General Error",
-                            "content": {
-                                "application/json": {
-                                    "schema": {
-                                        "$ref": "#/components/schemas/GeneralError"
-                                    }
-                                }
-                            },
-                        },
-                    },
-                    "securitySchemes": {
-                        "api_key": {
-                            "type": "apiKey",
-                            "name": "api_key",
-                            "in": "header",
-                        },
-                        "petstore_auth": {
-                            "type": "oauth2",
-                            "flows": {
-                                "implicit": {
-                                    "authorizationUrl": "http://example.org/api/oauth/dialog",
-                                    "scopes": {
-                                        "write:pets": "modify pets in your account",
-                                        "read:pets": "read your pets",
-                                    },
-                                }
-                            },
-                        },
-                    },
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/contact.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/contact.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {
+        "name": "API Support",
+        "url": "http://www.example.com/support",
+        "email": "support@example.com",
+    }
+]
 
 
 class Contact(BaseModel):
     """
     Contact information for the exposed API.
     """
 
@@ -21,18 +31,18 @@
 
     email: Optional[str] = None
     """
     The email address of the contact person/organization.
     MUST be in the format of an email address.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "name": "API Support",
-                    "url": "http://www.example.com/support",
-                    "email": "support@example.com",
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/discriminator.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/discriminator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {
+        "propertyName": "petType",
+        "mapping": {
+            "dog": "#/components/schemas/Dog",
+            "monster": "https://gigantic-server.com/schemas/Monster/schema.json",
+        },
+    }
+]
 
 
 class Discriminator(BaseModel):
     """
     When request bodies or response payloads may be one of a number of different
     schemas, a `discriminator` object can be used to aid in serialization,
     deserialization, and validation.
@@ -23,20 +35,18 @@
     """
 
     mapping: Optional[Dict[str, str]] = None
     """
     An object to hold mappings between payload values and schema names or references.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "propertyName": "petType",
-                    "mapping": {
-                        "dog": "#/components/schemas/Dog",
-                        "monster": "https://gigantic-server.com/schemas/Monster/schema.json",
-                    },
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/encoding.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/encoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .reference import Reference
 
 if TYPE_CHECKING:
     from .header import Header
 
+_examples = [
+    {
+        "contentType": "image/png, image/jpeg",
+        "headers": {
+            "X-Rate-Limit-Limit": {
+                "description": "The number of allowed requests in the "
+                "current period",
+                "schema": {"type": "integer"},
+            }
+        },
+    }
+]
+
 
 class Encoding(BaseModel):
     """A single encoding definition applied to a single schema property."""
 
     contentType: Optional[str] = None
     """
     The Content-Type for encoding a specific property.
@@ -62,23 +77,18 @@
     as defined by [RFC3986](https://tools.ietf.org/html/rfc3986#section-2.2)
     `:/?#[]@!$&'()*+,;=` to be included without percent-encoding.
     The default value is `false`.
     This property SHALL be ignored if the request body media type is not 
     `application/x-www-form-urlencoded`.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "contentType": "image/png, image/jpeg",
-                    "headers": {
-                        "X-Rate-Limit-Limit": {
-                            "description": "The number of allowed requests in the "
-                            "current period",
-                            "schema": {"type": "integer"},
-                        }
-                    },
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/example.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 from typing import Any, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {"summary": "A foo example", "value": {"foo": "bar"}},
+    {
+        "summary": "This is an example in XML",
+        "externalValue": "http://example.org/examples/address-example.xml",
+    },
+    {
+        "summary": "This is a text example",
+        "externalValue": "http://foo.bar/examples/address-example.txt",
+    },
+]
 
 
 class Example(BaseModel):
     summary: Optional[str] = None
     """
     Short description for the example.
     """
@@ -29,22 +43,18 @@
     A URL that points to the literal example.
     This provides the capability to reference examples that cannot easily be included 
     in JSON or YAML documents.
     
     The `value` field and `externalValue` field are mutually exclusive.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {"summary": "A foo example", "value": {"foo": "bar"}},
-                {
-                    "summary": "This is an example in XML",
-                    "externalValue": "http://example.org/examples/address-example.xml",
-                },
-                {
-                    "summary": "This is a text example",
-                    "externalValue": "http://foo.bar/examples/address-example.txt",
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/external_documentation.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/external_documentation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [{"description": "Find more info here", "url": "https://example.com"}]
 
 
 class ExternalDocumentation(BaseModel):
     """Allows referencing an external resource for extended documentation."""
 
     description: Optional[str] = None
     """
@@ -15,14 +19,18 @@
 
     url: str
     """
     **REQUIRED**. The URL for the target documentation.
     Value MUST be in the format of a URL.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {"description": "Find more info here", "url": "https://example.com"}
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/header.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/server_variable.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,42 @@
-from pydantic import Extra, Field
+from typing import List, Optional
 
-from .parameter import Parameter, ParameterLocation
+from pydantic import BaseModel
 
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
-class Header(Parameter):
+
+class ServerVariable(BaseModel):
+    """An object representing a Server Variable for server URL template substitution."""
+
+    enum: Optional[List[str]] = None
+    """
+    An enumeration of string values to be used if the substitution options are from a 
+    limited set. The array SHOULD NOT be empty.
+    """
+
+    default: str
+    """
+    **REQUIRED**. The default value to use for substitution,
+    which SHALL be sent if an alternate value is _not_ supplied.
+    Note this behavior is different than the [Schema Object's](#schemaObject) treatment 
+    of default values, because in those cases parameter values are optional.
+    If the [`enum`](#serverVariableEnum) is defined, the value MUST exist in the enum's 
+    values.
     """
-    The Header Object follows the structure of the [Parameter Object](#parameterObject)
-    with the following changes:
-
-    1. `name` MUST NOT be specified, it is given in the corresponding `headers` map.
-    2. `in` MUST NOT be specified, it is implicitly in `header`.
-    3. All traits that are affected by the location MUST be applicable to a location of
-    `header` (for example, [`style`](#parameterStyle)).
-    """
-
-    name: str = Field(default="", const=True)
-    param_in: ParameterLocation = Field(
-        default=ParameterLocation.HEADER, const=True, alias="in"
-    )
-
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {
-                    "description": "The number of allowed requests in the current "
-                    "period",
-                    "schema": {"type": "integer"},
-                }
-            ]
-        }
+
+    description: Optional[str] = None
+    """
+    An optional description for the server variable.
+    [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text 
+    representation.
+    """
+
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/info.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,34 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .contact import Contact
 from .license import License
 
+_examples = [
+    {
+        "title": "Sample Pet Store App",
+        "description": "This is a sample server for a pet store.",
+        "termsOfService": "http://example.com/terms/",
+        "contact": {
+            "name": "API Support",
+            "url": "http://www.example.com/support",
+            "email": "support@example.com",
+        },
+        "license": {
+            "name": "Apache 2.0",
+            "url": "https://www.apache.org/licenses/LICENSE-2.0.html",
+        },
+        "version": "1.0.1",
+    }
+]
+
 
 class Info(BaseModel):
     """
     The object provides metadata about the API.
     The metadata MAY be used by the clients if needed,
     and MAY be presented in editing or documentation generation tools for convenience.
     """
@@ -44,28 +64,18 @@
     version: str
     """
     **REQUIRED**. The version of the OpenAPI document
     (which is distinct from the [OpenAPI Specification version](#oasVersion) or the API 
     implementation version).
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "title": "Sample Pet Store App",
-                    "description": "This is a sample server for a pet store.",
-                    "termsOfService": "http://example.com/terms/",
-                    "contact": {
-                        "name": "API Support",
-                        "url": "http://www.example.com/support",
-                        "email": "support@example.com",
-                    },
-                    "license": {
-                        "name": "Apache 2.0",
-                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html",
-                    },
-                    "version": "1.0.1",
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/license.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/license.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {
+        "name": "Apache 2.0",
+        "url": "https://www.apache.org/licenses/LICENSE-2.0.html",
+    }
+]
 
 
 class License(BaseModel):
     """
     License information for the exposed API.
     """
 
@@ -15,17 +24,18 @@
 
     url: Optional[str] = None
     """
     A URL to the license used for the API.
     MUST be in the format of a URL.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "name": "Apache 2.0",
-                    "url": "https://www.apache.org/licenses/LICENSE-2.0.html",
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/link.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/link.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 from typing import Any, Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .server import Server
 
+_examples = [
+    {
+        "operationId": "getUserAddressByUUID",
+        "parameters": {"userUuid": "$response.body#/uuid"},
+    },
+    {
+        "operationRef": "#/paths/~12.0~1repositories~1{username}/get",
+        "parameters": {"username": "$response.body#/username"},
+    },
+]
+
 
 class Link(BaseModel):
     """
     The `Link object` represents a possible design-time link for a response.
     The presence of a link does not guarantee the caller's ability to successfully
     invoke it, rather it provides a known relationship and traversal mechanism between
     responses and other operations.
@@ -64,21 +77,18 @@
     """
 
     server: Optional[Server] = None
     """
     A server object to be used by the target operation.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "operationId": "getUserAddressByUUID",
-                    "parameters": {"userUuid": "$response.body#/uuid"},
-                },
-                {
-                    "operationRef": "#/paths/~12.0~1repositories~1{username}/get",
-                    "parameters": {"username": "$response.body#/username"},
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/media_type.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/media_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,46 @@
 from typing import Any, Dict, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .encoding import Encoding
 from .example import Example
 from .reference import Reference
 from .schema import Schema
 
+_examples = [
+    {
+        "schema": {"$ref": "#/components/schemas/Pet"},
+        "examples": {
+            "cat": {
+                "summary": "An example of a cat",
+                "value": {
+                    "name": "Fluffy",
+                    "petType": "Cat",
+                    "color": "White",
+                    "gender": "male",
+                    "breed": "Persian",
+                },
+            },
+            "dog": {
+                "summary": "An example of a dog with a cat's name",
+                "value": {
+                    "name": "Puma",
+                    "petType": "Dog",
+                    "color": "Black",
+                    "gender": "Female",
+                    "breed": "Mixed",
+                },
+            },
+        },
+    }
+]
+
 
 class MediaType(BaseModel):
     """Each Media Type Object provides schema and examples for the media type
     identified by its key."""
 
     media_type_schema: Optional[Union[Reference, Schema]] = Field(
         default=None, alias="schema"
@@ -47,39 +77,20 @@
     """
     A map between a property name and its encoding information.
     The key, being the property name, MUST exist in the schema as a property.
     The encoding object SHALL only apply to `requestBody` objects
     when the media type is `multipart` or `application/x-www-form-urlencoded`.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {
-                    "schema": {"$ref": "#/components/schemas/Pet"},
-                    "examples": {
-                        "cat": {
-                            "summary": "An example of a cat",
-                            "value": {
-                                "name": "Fluffy",
-                                "petType": "Cat",
-                                "color": "White",
-                                "gender": "male",
-                                "breed": "Persian",
-                            },
-                        },
-                        "dog": {
-                            "summary": "An example of a dog with a cat's name",
-                            "value": {
-                                "name": "Puma",
-                                "petType": "Dog",
-                                "color": "Black",
-                                "gender": "Female",
-                                "breed": "Mixed",
-                            },
-                        },
-                    },
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/oauth_flow.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/oauth_flow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,39 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {
+        "authorizationUrl": "https://example.com/api/oauth/dialog",
+        "scopes": {
+            "write:pets": "modify pets in your account",
+            "read:pets": "read your pets",
+        },
+    },
+    {
+        "authorizationUrl": "https://example.com/api/oauth/dialog",
+        "tokenUrl": "https://example.com/api/oauth/token",
+        "scopes": {
+            "write:pets": "modify pets in your account",
+            "read:pets": "read your pets",
+        },
+    },
+    {
+        "authorizationUrl": "/api/oauth/dialog",
+        "tokenUrl": "/api/oauth/token",
+        "refreshUrl": "/api/oauth/token",
+        "scopes": {
+            "write:pets": "modify pets in your account",
+            "read:pets": "read your pets",
+        },
+    },
+]
 
 
 class OAuthFlow(BaseModel):
     """
     Configuration details for a supported OAuth Flow
     """
 
@@ -30,37 +59,18 @@
     scopes: Dict[str, str]
     """
     **REQUIRED**. The available scopes for the OAuth2 security scheme.
     A map between the scope name and a short description for it.
     The map MAY be empty.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "authorizationUrl": "https://example.com/api/oauth/dialog",
-                    "scopes": {
-                        "write:pets": "modify pets in your account",
-                        "read:pets": "read your pets",
-                    },
-                },
-                {
-                    "authorizationUrl": "https://example.com/api/oauth/dialog",
-                    "tokenUrl": "https://example.com/api/oauth/token",
-                    "scopes": {
-                        "write:pets": "modify pets in your account",
-                        "read:pets": "read your pets",
-                    },
-                },
-                {
-                    "authorizationUrl": "/api/oauth/dialog",
-                    "tokenUrl": "/api/oauth/token",
-                    "refreshUrl": "/api/oauth/token",
-                    "scopes": {
-                        "write:pets": "modify pets in your account",
-                        "read:pets": "read your pets",
-                    },
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/oauth_flows.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/oauth_flows.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .oauth_flow import OAuthFlow
 
 
 class OAuthFlows(BaseModel):
     """
     Allows configuration of the supported OAuth Flows.
@@ -30,9 +32,16 @@
     authorizationCode: Optional[OAuthFlow] = None
     """
     Configuration for the OAuth Authorization Code flow.
     
     Previously called `accessCode` in OpenAPI 2.0.
     """
 
-    class Config:
-        extra = Extra.allow
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/open_api.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/open_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import List, Literal, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .components import Components
 from .external_documentation import ExternalDocumentation
 from .info import Info
 from .paths import Paths
 from .security_requirement import SecurityRequirement
 from .server import Server
@@ -67,9 +69,16 @@
     """
 
     externalDocs: Optional[ExternalDocumentation] = None
     """
     Additional external documentation.
     """
 
-    class Config:
-        extra = Extra.allow
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/operation.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/operation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,70 @@
 from typing import Dict, List, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .callback import Callback
 from .external_documentation import ExternalDocumentation
 from .parameter import Parameter
 from .reference import Reference
 from .request_body import RequestBody
 from .responses import Responses
 from .security_requirement import SecurityRequirement
 from .server import Server
 
+_examples = [
+    {
+        "tags": ["pet"],
+        "summary": "Updates a pet in the store with form data",
+        "operationId": "updatePetWithForm",
+        "parameters": [
+            {
+                "name": "petId",
+                "in": "path",
+                "description": "ID of pet that needs to be updated",
+                "required": True,
+                "schema": {"type": "string"},
+            }
+        ],
+        "requestBody": {
+            "content": {
+                "application/x-www-form-urlencoded": {
+                    "schema": {
+                        "type": "object",
+                        "properties": {
+                            "name": {
+                                "description": "Updated name of the pet",
+                                "type": "string",
+                            },
+                            "status": {
+                                "description": "Updated status of the pet",
+                                "type": "string",
+                            },
+                        },
+                        "required": ["status"],
+                    }
+                }
+            }
+        },
+        "responses": {
+            "200": {
+                "description": "Pet updated.",
+                "content": {"application/json": {}, "application/xml": {}},
+            },
+            "405": {
+                "description": "Method Not Allowed",
+                "content": {"application/json": {}, "application/xml": {}},
+            },
+        },
+        "security": [{"petstore_auth": ["write:pets", "read:pets"]}],
+    }
+]
+
 
 class Operation(BaseModel):
     """Describes a single API operation on a path."""
 
     tags: Optional[List[str]] = None
     """
     A list of tags for API documentation control.
@@ -106,58 +156,18 @@
     servers: Optional[List[Server]] = None
     """
     An alternative `server` array to service this operation.
     If an alternative `server` object is specified at the Path Item Object or Root 
     level, it will be overridden by this value.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "tags": ["pet"],
-                    "summary": "Updates a pet in the store with form data",
-                    "operationId": "updatePetWithForm",
-                    "parameters": [
-                        {
-                            "name": "petId",
-                            "in": "path",
-                            "description": "ID of pet that needs to be updated",
-                            "required": True,
-                            "schema": {"type": "string"},
-                        }
-                    ],
-                    "requestBody": {
-                        "content": {
-                            "application/x-www-form-urlencoded": {
-                                "schema": {
-                                    "type": "object",
-                                    "properties": {
-                                        "name": {
-                                            "description": "Updated name of the pet",
-                                            "type": "string",
-                                        },
-                                        "status": {
-                                            "description": "Updated status of the pet",
-                                            "type": "string",
-                                        },
-                                    },
-                                    "required": ["status"],
-                                }
-                            }
-                        }
-                    },
-                    "responses": {
-                        "200": {
-                            "description": "Pet updated.",
-                            "content": {"application/json": {}, "application/xml": {}},
-                        },
-                        "405": {
-                            "description": "Method Not Allowed",
-                            "content": {"application/json": {}, "application/xml": {}},
-                        },
-                    },
-                    "security": [{"petstore_auth": ["write:pets", "read:pets"]}],
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/parameter.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,74 @@
 import enum
 from typing import Any, Dict, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .example import Example
 from .media_type import MediaType
 from .reference import Reference
 from .schema import Schema
 
+_examples = [
+    {
+        "name": "token",
+        "in": "header",
+        "description": "token to be passed as a header",
+        "required": True,
+        "schema": {
+            "type": "array",
+            "items": {"type": "integer", "format": "int64"},
+        },
+        "style": "simple",
+    },
+    {
+        "name": "username",
+        "in": "path",
+        "description": "username to fetch",
+        "required": True,
+        "schema": {"type": "string"},
+    },
+    {
+        "name": "id",
+        "in": "query",
+        "description": "ID of the object to fetch",
+        "required": False,
+        "schema": {"type": "array", "items": {"type": "string"}},
+        "style": "form",
+        "explode": True,
+    },
+    {
+        "in": "query",
+        "name": "freeForm",
+        "schema": {
+            "type": "object",
+            "additionalProperties": {"type": "integer"},
+        },
+        "style": "form",
+    },
+    {
+        "in": "query",
+        "name": "coordinates",
+        "content": {
+            "application/json": {
+                "schema": {
+                    "type": "object",
+                    "required": ["lat", "long"],
+                    "properties": {
+                        "lat": {"type": "number"},
+                        "long": {"type": "number"},
+                    },
+                }
+            }
+        },
+    },
+]
+
 
 class ParameterLocation(str, enum.Enum):
     """The location of a given parameter."""
 
     QUERY = "query"
     HEADER = "header"
     PATH = "path"
@@ -156,66 +213,20 @@
     content: Optional[Dict[str, MediaType]] = None
     """
     A map containing the representations for the parameter.
     The key is the media type and the value describes it.
     The map MUST only contain one entry.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {
-                    "name": "token",
-                    "in": "header",
-                    "description": "token to be passed as a header",
-                    "required": True,
-                    "schema": {
-                        "type": "array",
-                        "items": {"type": "integer", "format": "int64"},
-                    },
-                    "style": "simple",
-                },
-                {
-                    "name": "username",
-                    "in": "path",
-                    "description": "username to fetch",
-                    "required": True,
-                    "schema": {"type": "string"},
-                },
-                {
-                    "name": "id",
-                    "in": "query",
-                    "description": "ID of the object to fetch",
-                    "required": False,
-                    "schema": {"type": "array", "items": {"type": "string"}},
-                    "style": "form",
-                    "explode": True,
-                },
-                {
-                    "in": "query",
-                    "name": "freeForm",
-                    "schema": {
-                        "type": "object",
-                        "additionalProperties": {"type": "integer"},
-                    },
-                    "style": "form",
-                },
-                {
-                    "in": "query",
-                    "name": "coordinates",
-                    "content": {
-                        "application/json": {
-                            "schema": {
-                                "type": "object",
-                                "required": ["lat", "long"],
-                                "properties": {
-                                    "lat": {"type": "number"},
-                                    "long": {"type": "number"},
-                                },
-                            }
-                        }
-                    },
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/path_item.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/path_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,59 @@
 from typing import List, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .operation import Operation
 from .parameter import Parameter
 from .reference import Reference
 from .server import Server
 
+_examples = [
+    {
+        "get": {
+            "description": "Returns pets based on ID",
+            "summary": "Find pets by ID",
+            "operationId": "getPetsById",
+            "responses": {
+                "200": {
+                    "description": "pet response",
+                    "content": {
+                        "*/*": {
+                            "schema": {
+                                "type": "array",
+                                "items": {"$ref": "#/components/schemas/Pet"},
+                            }
+                        }
+                    },
+                },
+                "default": {
+                    "description": "error payload",
+                    "content": {
+                        "text/html": {
+                            "schema": {"$ref": "#/components/schemas/ErrorModel"}
+                        }
+                    },
+                },
+            },
+        },
+        "parameters": [
+            {
+                "name": "id",
+                "in": "path",
+                "description": "ID of pet to use",
+                "required": True,
+                "schema": {"type": "array", "items": {"type": "string"}},
+                "style": "simple",
+            }
+        ],
+    }
+]
+
 
 class PathItem(BaseModel):
     """
     Describes the operations available on a single path.
     A Path Item MAY be empty, due to [ACL constraints](#securityFiltering).
     The path itself is still exposed to the documentation viewer
     but they will not know which operations and parameters are available.
@@ -90,56 +133,20 @@
     removed there. The list MUST NOT include duplicated parameters.
     A unique parameter is defined by a combination of a [name](#parameterName) and 
     [location](#parameterIn). The list can use the [Reference Object](#referenceObject) 
     to link to parameters that are defined at the
     [OpenAPI Object's components/parameters](#componentsParameters).
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {
-                    "get": {
-                        "description": "Returns pets based on ID",
-                        "summary": "Find pets by ID",
-                        "operationId": "getPetsById",
-                        "responses": {
-                            "200": {
-                                "description": "pet response",
-                                "content": {
-                                    "*/*": {
-                                        "schema": {
-                                            "type": "array",
-                                            "items": {
-                                                "$ref": "#/components/schemas/Pet"
-                                            },
-                                        }
-                                    }
-                                },
-                            },
-                            "default": {
-                                "description": "error payload",
-                                "content": {
-                                    "text/html": {
-                                        "schema": {
-                                            "$ref": "#/components/schemas/ErrorModel"
-                                        }
-                                    }
-                                },
-                            },
-                        },
-                    },
-                    "parameters": [
-                        {
-                            "name": "id",
-                            "in": "path",
-                            "description": "ID of pet to use",
-                            "required": True,
-                            "schema": {"type": "array", "items": {"type": "string"}},
-                            "style": "simple",
-                        }
-                    ],
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/paths.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/request_body.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/request_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,63 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .media_type import MediaType
 
+_examples = [
+    {
+        "description": "user to add to the system",
+        "content": {
+            "application/json": {
+                "schema": {"$ref": "#/components/schemas/User"},
+                "examples": {
+                    "user": {
+                        "summary": "User Example",
+                        "externalValue": "http://foo.bar/examples/user-example.json",
+                    }
+                },
+            },
+            "application/xml": {
+                "schema": {"$ref": "#/components/schemas/User"},
+                "examples": {
+                    "user": {
+                        "summary": "User example in XML",
+                        "externalValue": "http://foo.bar/examples/user-example.xml",
+                    }
+                },
+            },
+            "text/plain": {
+                "examples": {
+                    "user": {
+                        "summary": "User example in Plain text",
+                        "externalValue": "http://foo.bar/examples/user-example.txt",
+                    }
+                }
+            },
+            "*/*": {
+                "examples": {
+                    "user": {
+                        "summary": "User example in other format",
+                        "externalValue": "http://foo.bar/examples/user-example.whatever",
+                    }
+                }
+            },
+        },
+    },
+    {
+        "description": "user to add to the system",
+        "content": {
+            "text/plain": {"schema": {"type": "array", "items": {"type": "string"}}}
+        },
+    },
+]
+
 
 class RequestBody(BaseModel):
     """Describes a single request body."""
 
     description: Optional[str] = None
     """
     A brief description of the request body.
@@ -28,60 +78,18 @@
     """
 
     required: bool = False
     """
     Determines if the request body is required in the request. Defaults to `false`.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "description": "user to add to the system",
-                    "content": {
-                        "application/json": {
-                            "schema": {"$ref": "#/components/schemas/User"},
-                            "examples": {
-                                "user": {
-                                    "summary": "User Example",
-                                    "externalValue": "http://foo.bar/examples/user-example.json",
-                                }
-                            },
-                        },
-                        "application/xml": {
-                            "schema": {"$ref": "#/components/schemas/User"},
-                            "examples": {
-                                "user": {
-                                    "summary": "User example in XML",
-                                    "externalValue": "http://foo.bar/examples/user-example.xml",
-                                }
-                            },
-                        },
-                        "text/plain": {
-                            "examples": {
-                                "user": {
-                                    "summary": "User example in Plain text",
-                                    "externalValue": "http://foo.bar/examples/user-example.txt",
-                                }
-                            }
-                        },
-                        "*/*": {
-                            "examples": {
-                                "user": {
-                                    "summary": "User example in other format",
-                                    "externalValue": "http://foo.bar/examples/user-example.whatever",
-                                }
-                            }
-                        },
-                    },
-                },
-                {
-                    "description": "user to add to the system",
-                    "content": {
-                        "text/plain": {
-                            "schema": {"type": "array", "items": {"type": "string"}}
-                        }
-                    },
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/response.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,57 @@
 from typing import Dict, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .header import Header
 from .link import Link
 from .media_type import MediaType
 from .reference import Reference
 
+_examples = [
+    {
+        "description": "A complex object array response",
+        "content": {
+            "application/json": {
+                "schema": {
+                    "type": "array",
+                    "items": {"$ref": "#/components/schemas/VeryComplexType"},
+                }
+            }
+        },
+    },
+    {
+        "description": "A simple string response",
+        "content": {"text/plain": {"schema": {"type": "string"}}},
+    },
+    {
+        "description": "A simple string response",
+        "content": {"text/plain": {"schema": {"type": "string", "example": "whoa!"}}},
+        "headers": {
+            "X-Rate-Limit-Limit": {
+                "description": ("The number of allowed requests in the current period"),
+                "schema": {"type": "integer"},
+            },
+            "X-Rate-Limit-Remaining": {
+                "description": (
+                    "The number of remaining requests in the current period"
+                ),
+                "schema": {"type": "integer"},
+            },
+            "X-Rate-Limit-Reset": {
+                "description": ("The number of seconds left in the current period"),
+                "schema": {"type": "integer"},
+            },
+        },
+    },
+    {"description": "object created"},
+]
+
 
 class Response(BaseModel):
     """
     Describes a single response from an API Operation, including design-time,
     static `links` to operations based on the response.
     """
 
@@ -43,59 +84,18 @@
     """
     A map of operations links that can be followed from the response.
     The key of the map is a short name for the link,
     following the naming constraints of the names for 
     [Component Objects](#componentsObject).
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "description": "A complex object array response",
-                    "content": {
-                        "application/json": {
-                            "schema": {
-                                "type": "array",
-                                "items": {
-                                    "$ref": "#/components/schemas/VeryComplexType"
-                                },
-                            }
-                        }
-                    },
-                },
-                {
-                    "description": "A simple string response",
-                    "content": {"text/plain": {"schema": {"type": "string"}}},
-                },
-                {
-                    "description": "A simple string response",
-                    "content": {
-                        "text/plain": {"schema": {"type": "string", "example": "whoa!"}}
-                    },
-                    "headers": {
-                        "X-Rate-Limit-Limit": {
-                            "description": (
-                                "The number of allowed requests in the "
-                                "current period"
-                            ),
-                            "schema": {"type": "integer"},
-                        },
-                        "X-Rate-Limit-Remaining": {
-                            "description": (
-                                "The number of remaining requests in the "
-                                "current period"
-                            ),
-                            "schema": {"type": "integer"},
-                        },
-                        "X-Rate-Limit-Reset": {
-                            "description": (
-                                "The number of seconds left in the current period"
-                            ),
-                            "schema": {"type": "integer"},
-                        },
-                    },
-                },
-                {"description": "object created"},
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/responses.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/schema.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,117 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra, min_length_arg
 
 from .datatype import DataType
 from .discriminator import Discriminator
 from .external_documentation import ExternalDocumentation
 from .reference import Reference
 from .xml import XML
 
+_examples = [
+    {"type": "string", "format": "email"},
+    {
+        "type": "object",
+        "required": ["name"],
+        "properties": {
+            "name": {"type": "string"},
+            "address": {"$ref": "#/components/schemas/Address"},
+            "age": {"type": "integer", "format": "int32", "minimum": 0},
+        },
+    },
+    {"type": "object", "additionalProperties": {"type": "string"}},
+    {
+        "type": "object",
+        "additionalProperties": {"$ref": "#/components/schemas/ComplexModel"},
+    },
+    {
+        "type": "object",
+        "properties": {
+            "id": {"type": "integer", "format": "int64"},
+            "name": {"type": "string"},
+        },
+        "required": ["name"],
+        "example": {"name": "Puma", "id": 1},
+    },
+    {
+        "type": "object",
+        "required": ["message", "code"],
+        "properties": {
+            "message": {"type": "string"},
+            "code": {"type": "integer", "minimum": 100, "maximum": 600},
+        },
+    },
+    {
+        "allOf": [
+            {"$ref": "#/components/schemas/ErrorModel"},
+            {
+                "type": "object",
+                "required": ["rootCause"],
+                "properties": {"rootCause": {"type": "string"}},
+            },
+        ]
+    },
+    {
+        "type": "object",
+        "discriminator": {"propertyName": "petType"},
+        "properties": {
+            "name": {"type": "string"},
+            "petType": {"type": "string"},
+        },
+        "required": ["name", "petType"],
+    },
+    {
+        "description": "A representation of a cat. "
+        "Note that `Cat` will be used as the discriminator value.",
+        "allOf": [
+            {"$ref": "#/components/schemas/Pet"},
+            {
+                "type": "object",
+                "properties": {
+                    "huntingSkill": {
+                        "type": "string",
+                        "description": "The measured skill for hunting",
+                        "default": "lazy",
+                        "enum": [
+                            "clueless",
+                            "lazy",
+                            "adventurous",
+                            "aggressive",
+                        ],
+                    }
+                },
+                "required": ["huntingSkill"],
+            },
+        ],
+    },
+    {
+        "description": "A representation of a dog. "
+        "Note that `Dog` will be used as the discriminator value.",
+        "allOf": [
+            {"$ref": "#/components/schemas/Pet"},
+            {
+                "type": "object",
+                "properties": {
+                    "packSize": {
+                        "type": "integer",
+                        "format": "int32",
+                        "description": ("the size of the pack the dog is from"),
+                        "default": 0,
+                        "minimum": 0,
+                    }
+                },
+                "required": ["packSize"],
+            },
+        ],
+    },
+]
+
 
 class Schema(BaseModel):
     """
     The Schema Object allows the definition of input and output data types.
     These types can be objects, but also primitives and arrays.
     This object is an extended subset of the [JSON Schema Specification Wright Draft 00](https://json-schema.org/).
 
@@ -179,25 +279,25 @@
     An object instance is valid against "minProperties" if its number of
     properties is greater than, or equal to, the value of this keyword.
     
     If this keyword is not present, it may be considered present with a
     value of 0.
     """
 
-    required: Optional[List[str]] = Field(default=None, min_items=1)
+    required: Optional[List[str]] = Field(default=None, **min_length_arg(1))
     """
     The value of this keyword MUST be an array.  This array MUST have at
     least one element.  Elements of this array MUST be strings, and MUST
     be unique.
     
     An object instance is valid against this keyword if its property set
     contains all elements in this keyword's array value.
     """
 
-    enum: Optional[List[Any]] = Field(default=None, min_items=1)
+    enum: Optional[List[Any]] = Field(default=None, **min_length_arg(1))
     """
     The value of this keyword MUST be an array.  This array SHOULD have
     at least one element.  Elements in the array SHOULD be unique.
     
     Elements in the array MAY be of any type, including null.
     
     An instance validates successfully against this keyword if its value
@@ -478,113 +578,38 @@
 
     deprecated: Optional[bool] = None
     """ 
     Specifies that a schema is deprecated and SHOULD be transitioned out of usage.
     Default value is `false`.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {"type": "string", "format": "email"},
-                {
-                    "type": "object",
-                    "required": ["name"],
-                    "properties": {
-                        "name": {"type": "string"},
-                        "address": {"$ref": "#/components/schemas/Address"},
-                        "age": {"type": "integer", "format": "int32", "minimum": 0},
-                    },
-                },
-                {"type": "object", "additionalProperties": {"type": "string"}},
-                {
-                    "type": "object",
-                    "additionalProperties": {
-                        "$ref": "#/components/schemas/ComplexModel"
-                    },
-                },
-                {
-                    "type": "object",
-                    "properties": {
-                        "id": {"type": "integer", "format": "int64"},
-                        "name": {"type": "string"},
-                    },
-                    "required": ["name"],
-                    "example": {"name": "Puma", "id": 1},
-                },
-                {
-                    "type": "object",
-                    "required": ["message", "code"],
-                    "properties": {
-                        "message": {"type": "string"},
-                        "code": {"type": "integer", "minimum": 100, "maximum": 600},
-                    },
-                },
-                {
-                    "allOf": [
-                        {"$ref": "#/components/schemas/ErrorModel"},
-                        {
-                            "type": "object",
-                            "required": ["rootCause"],
-                            "properties": {"rootCause": {"type": "string"}},
-                        },
-                    ]
-                },
-                {
-                    "type": "object",
-                    "discriminator": {"propertyName": "petType"},
-                    "properties": {
-                        "name": {"type": "string"},
-                        "petType": {"type": "string"},
-                    },
-                    "required": ["name", "petType"],
-                },
-                {
-                    "description": "A representation of a cat. "
-                    "Note that `Cat` will be used as the discriminator value.",
-                    "allOf": [
-                        {"$ref": "#/components/schemas/Pet"},
-                        {
-                            "type": "object",
-                            "properties": {
-                                "huntingSkill": {
-                                    "type": "string",
-                                    "description": "The measured skill for hunting",
-                                    "default": "lazy",
-                                    "enum": [
-                                        "clueless",
-                                        "lazy",
-                                        "adventurous",
-                                        "aggressive",
-                                    ],
-                                }
-                            },
-                            "required": ["huntingSkill"],
-                        },
-                    ],
-                },
-                {
-                    "description": "A representation of a dog. "
-                    "Note that `Dog` will be used as the discriminator value.",
-                    "allOf": [
-                        {"$ref": "#/components/schemas/Pet"},
-                        {
-                            "type": "object",
-                            "properties": {
-                                "packSize": {
-                                    "type": "integer",
-                                    "format": "int32",
-                                    "description": (
-                                        "the size of the pack the dog is from"
-                                    ),
-                                    "default": 0,
-                                    "minimum": 0,
-                                }
-                            },
-                            "required": ["packSize"],
-                        },
-                    ],
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
+
+
+if TYPE_CHECKING:
+
+    def schema_validate(
+        obj: Any,
+        *,
+        strict: bool | None = None,
+        from_attributes: bool | None = None,
+        context: dict[str, Any] | None = None
+    ) -> Schema:
+        ...
+
+elif PYDANTIC_V2:
+    schema_validate = Schema.model_validate
+
+else:
+    schema_validate = Schema.parse_obj
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/security_requirement.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/security_scheme.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/security_scheme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,41 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .oauth_flows import OAuthFlows
 
+_examples = [
+    {"type": "http", "scheme": "basic"},
+    {"type": "apiKey", "name": "api_key", "in": "header"},
+    {"type": "http", "scheme": "bearer", "bearerFormat": "JWT"},
+    {
+        "type": "oauth2",
+        "flows": {
+            "implicit": {
+                "authorizationUrl": "https://example.com/api/oauth/dialog",
+                "scopes": {
+                    "write:pets": "modify pets in your account",
+                    "read:pets": "read your pets",
+                },
+            }
+        },
+    },
+    {
+        "type": "openIdConnect",
+        "openIdConnectUrl": "https://example.com/openIdConnect",
+    },
+    {
+        "type": "openIdConnect",
+        "openIdConnectUrl": "openIdConnect",
+    },  # #5: allow relative path
+]
+
 
 class SecurityScheme(BaseModel):
     """
     Defines a security scheme that can be used by the operations.
     Supported schemes are HTTP authentication,
     an API key (either as a header, a cookie parameter or as a query parameter),
     OAuth2's common flows (implicit, password, client credentials and authorization
@@ -65,37 +93,20 @@
 
     openIdConnectUrl: Optional[str] = None
     """
     **REQUIRED** for `openIdConnect`. OpenId Connect URL to discover OAuth2 
     configuration values. This MUST be in the form of a URL.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {"type": "http", "scheme": "basic"},
-                {"type": "apiKey", "name": "api_key", "in": "header"},
-                {"type": "http", "scheme": "bearer", "bearerFormat": "JWT"},
-                {
-                    "type": "oauth2",
-                    "flows": {
-                        "implicit": {
-                            "authorizationUrl": "https://example.com/api/oauth/dialog",
-                            "scopes": {
-                                "write:pets": "modify pets in your account",
-                                "read:pets": "read your pets",
-                            },
-                        }
-                    },
-                },
-                {
-                    "type": "openIdConnect",
-                    "openIdConnectUrl": "https://example.com/openIdConnect",
-                },
-                {
-                    "type": "openIdConnect",
-                    "openIdConnectUrl": "openIdConnect",
-                },  # #5: allow relative path
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/server.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .server_variable import ServerVariable
 
+_examples = [
+    {
+        "url": "https://development.gigantic-server.com/v1",
+        "description": "Development server",
+    },
+    {
+        "url": "https://{username}.gigantic-server.com:{port}/{basePath}",
+        "description": "The production API server",
+        "variables": {
+            "username": {
+                "default": "demo",
+                "description": "this value is assigned by the service "
+                "provider, in this example `gigantic-server.com`",
+            },
+            "port": {"enum": ["8443", "443"], "default": "8443"},
+            "basePath": {"default": "v2"},
+        },
+    },
+]
+
 
 class Server(BaseModel):
     """An object representing a Server."""
 
     url: str
     """
     **REQUIRED**. A URL to the target host.
@@ -28,30 +50,18 @@
     variables: Optional[Dict[str, ServerVariable]] = None
     """
     A map between a variable name and its value.
     
     The value is used for substitution in the server's URL template.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "url": "https://development.gigantic-server.com/v1",
-                    "description": "Development server",
-                },
-                {
-                    "url": "https://{username}.gigantic-server.com:{port}/{basePath}",
-                    "description": "The production API server",
-                    "variables": {
-                        "username": {
-                            "default": "demo",
-                            "description": "this value is assigned by the service"
-                            "provider, in this example `gigantic-server.com`",
-                        },
-                        "port": {"enum": ["8443", "443"], "default": "8443"},
-                        "basePath": {"default": "v2"},
-                    },
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/server_variable.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/server_variable.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import List, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 
 class ServerVariable(BaseModel):
     """An object representing a Server Variable for server URL template substitution."""
 
     enum: Optional[List[str]] = None
     """
@@ -25,9 +27,16 @@
     description: Optional[str] = None
     """
     An optional description for the server variable.
     [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text 
     representation.
     """
 
-    class Config:
-        extra = Extra.allow
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/tag.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/tag.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .external_documentation import ExternalDocumentation
 
+_examples = [{"name": "pet", "description": "Pets operations"}]
+
 
 class Tag(BaseModel):
     """
     Adds metadata to a single tag that is used by the
     [Operation Object](#operationObject).
     It is not mandatory to have a Tag Object per tag defined in the Operation Object
     instances.
@@ -26,10 +30,18 @@
     """
 
     externalDocs: Optional[ExternalDocumentation] = None
     """
     Additional external documentation for this tag.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {"examples": [{"name": "pet", "description": "Pets operations"}]}
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_0_3/xml.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/xml.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {"namespace": "http://example.com/schema/sample", "prefix": "sample"},
+    {"name": "aliens", "wrapped": True},
+]
 
 
 class XML(BaseModel):
     """
     A metadata object that allows for more fine-tuned XML model definitions.
 
     When using arrays, XML element names are *not* inferred (for singular/plural forms)
@@ -44,15 +51,18 @@
     Signifies whether the array is wrapped (for example, 
     `<books><book/><book/></books>`) or unwrapped (`<book/><book/>`).
     Default value is `false`.
     The definition takes effect only when defined alongside `type` being `array` 
     (outside the `items`).
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {"namespace": "http://example.com/schema/sample", "prefix": "sample"},
-                {"name": "aliens", "wrapped": True},
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/README.md` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 | Schema | schema_not | not |
 | Schema | schema_if | if |
 | Schema | schema_else | else |
 
 > <a name="header_param_in"></a>The "in" field in Header object is actually a constant (`{"in": "header"}`).
 
 > For convenience of object creation, the classes mentioned in above
-> has configured `allow_population_by_field_name=True`.
+> have configured `allow_population_by_field_name=True` (Pydantic V1) or `populate_by_name=True` (Pydantic V2).
 >
 > Reference: [Pydantic's Model Config](https://pydantic-docs.helpmanual.io/usage/model_config/)
 
 ## Non-pydantic schema types
 
 Due to the constriants of python typing structure (not able to handle dynamic field names),
 the following schema classes are actually just a typing of `Dict`:
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/callback.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/components.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,100 @@
 from typing import Dict, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .callback import Callback
 from .example import Example
 from .header import Header
 from .link import Link
 from .parameter import Parameter
 from .path_item import PathItem
 from .reference import Reference
 from .request_body import RequestBody
 from .response import Response
 from .schema import Schema
 from .security_scheme import SecurityScheme
 
+_examples = [
+    {
+        "schemas": {
+            "GeneralError": {
+                "type": "object",
+                "properties": {
+                    "code": {"type": "integer", "format": "int32"},
+                    "message": {"type": "string"},
+                },
+            },
+            "Category": {
+                "type": "object",
+                "properties": {
+                    "id": {"type": "integer", "format": "int64"},
+                    "name": {"type": "string"},
+                },
+            },
+            "Tag": {
+                "type": "object",
+                "properties": {
+                    "id": {"type": "integer", "format": "int64"},
+                    "name": {"type": "string"},
+                },
+            },
+        },
+        "parameters": {
+            "skipParam": {
+                "name": "skip",
+                "in": "query",
+                "description": "number of items to skip",
+                "required": True,
+                "schema": {"type": "integer", "format": "int32"},
+            },
+            "limitParam": {
+                "name": "limit",
+                "in": "query",
+                "description": "max records to return",
+                "required": True,
+                "schema": {"type": "integer", "format": "int32"},
+            },
+        },
+        "responses": {
+            "NotFound": {"description": "Entity not found."},
+            "IllegalInput": {"description": "Illegal input for operation."},
+            "GeneralError": {
+                "description": "General Error",
+                "content": {
+                    "application/json": {
+                        "schema": {"$ref": "#/components/schemas/GeneralError"}
+                    }
+                },
+            },
+        },
+        "securitySchemes": {
+            "api_key": {
+                "type": "apiKey",
+                "name": "api_key",
+                "in": "header",
+            },
+            "petstore_auth": {
+                "type": "oauth2",
+                "flows": {
+                    "implicit": {
+                        "authorizationUrl": "http://example.org/api/oauth/dialog",
+                        "scopes": {
+                            "write:pets": "modify pets in your account",
+                            "read:pets": "read your pets",
+                        },
+                    }
+                },
+            },
+        },
+    }
+]
+
 
 class Components(BaseModel):
     """
     Holds a set of reusable objects for different aspects of the OAS.
     All objects defined within the components object will have no effect on the API
     unless they are explicitly referenced from properties outside the components object.
     """
@@ -48,87 +125,18 @@
 
     callbacks: Optional[Dict[str, Union[Callback, Reference]]] = None
     """An object to hold reusable [Callback Objects](#callbackObject)."""
 
     pathItems: Optional[Dict[str, Union[PathItem, Reference]]] = None
     """An object to hold reusable [Path Item Object](#pathItemObject)."""
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "schemas": {
-                        "GeneralError": {
-                            "type": "object",
-                            "properties": {
-                                "code": {"type": "integer", "format": "int32"},
-                                "message": {"type": "string"},
-                            },
-                        },
-                        "Category": {
-                            "type": "object",
-                            "properties": {
-                                "id": {"type": "integer", "format": "int64"},
-                                "name": {"type": "string"},
-                            },
-                        },
-                        "Tag": {
-                            "type": "object",
-                            "properties": {
-                                "id": {"type": "integer", "format": "int64"},
-                                "name": {"type": "string"},
-                            },
-                        },
-                    },
-                    "parameters": {
-                        "skipParam": {
-                            "name": "skip",
-                            "in": "query",
-                            "description": "number of items to skip",
-                            "required": True,
-                            "schema": {"type": "integer", "format": "int32"},
-                        },
-                        "limitParam": {
-                            "name": "limit",
-                            "in": "query",
-                            "description": "max records to return",
-                            "required": True,
-                            "schema": {"type": "integer", "format": "int32"},
-                        },
-                    },
-                    "responses": {
-                        "NotFound": {"description": "Entity not found."},
-                        "IllegalInput": {"description": "Illegal input for operation."},
-                        "GeneralError": {
-                            "description": "General Error",
-                            "content": {
-                                "application/json": {
-                                    "schema": {
-                                        "$ref": "#/components/schemas/GeneralError"
-                                    }
-                                }
-                            },
-                        },
-                    },
-                    "securitySchemes": {
-                        "api_key": {
-                            "type": "apiKey",
-                            "name": "api_key",
-                            "in": "header",
-                        },
-                        "petstore_auth": {
-                            "type": "oauth2",
-                            "flows": {
-                                "implicit": {
-                                    "authorizationUrl": "http://example.org/api/oauth/dialog",
-                                    "scopes": {
-                                        "write:pets": "modify pets in your account",
-                                        "read:pets": "read your pets",
-                                    },
-                                }
-                            },
-                        },
-                    },
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/contact.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/contact.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {
+        "name": "API Support",
+        "url": "http://www.example.com/support",
+        "email": "support@example.com",
+    }
+]
 
 
 class Contact(BaseModel):
     """
     Contact information for the exposed API.
     """
 
@@ -21,18 +31,18 @@
 
     email: Optional[str] = None
     """
     The email address of the contact person/organization.
     MUST be in the form of an email address.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "name": "API Support",
-                    "url": "http://www.example.com/support",
-                    "email": "support@example.com",
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/discriminator.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/discriminator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {
+        "propertyName": "petType",
+        "mapping": {
+            "dog": "#/components/schemas/Dog",
+            "monster": "https://gigantic-server.com/schemas/Monster/schema.json",
+        },
+    }
+]
 
 
 class Discriminator(BaseModel):
     """
     When request bodies or response payloads may be one of a number of different
     schemas, a `discriminator` object can be used to aid in serialization,
     deserialization, and validation.
@@ -23,20 +35,18 @@
     """
 
     mapping: Optional[Dict[str, str]] = None
     """
     An object to hold mappings between payload values and schema names or references.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "propertyName": "petType",
-                    "mapping": {
-                        "dog": "#/components/schemas/Dog",
-                        "monster": "https://gigantic-server.com/schemas/Monster/schema.json",
-                    },
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/encoding.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/encoding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .reference import Reference
 
 if TYPE_CHECKING:
     from .header import Header
 
+_examples = [
+    {
+        "contentType": "image/png, image/jpeg",
+        "headers": {
+            "X-Rate-Limit-Limit": {
+                "description": "The number of allowed requests in the "
+                "current period",
+                "schema": {"type": "integer"},
+            }
+        },
+    }
+]
+
 
 class Encoding(BaseModel):
     """A single encoding definition applied to a single schema property."""
 
     contentType: Optional[str] = None
     """
     The Content-Type for encoding a specific property.
@@ -69,23 +84,18 @@
     This property SHALL be ignored if the request body media type
     is not `application/x-www-form-urlencoded` or `multipart/form-data`.
     If a value is explicitly defined,
     then the value of [`contentType`](#encodingContentType) (implicit or explicit) 
     SHALL be ignored.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "contentType": "image/png, image/jpeg",
-                    "headers": {
-                        "X-Rate-Limit-Limit": {
-                            "description": "The number of allowed requests in the "
-                            "current period",
-                            "schema": {"type": "integer"},
-                        }
-                    },
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/example.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/example.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 from typing import Any, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {
+        "summary": "A foo example",
+        "value": {"foo": "bar"},
+    },
+    {
+        "summary": "This is an example in XML",
+        "externalValue": "http://example.org/examples/address-example.xml",
+    },
+    {
+        "summary": "This is a text example",
+        "externalValue": "http://foo.bar/examples/address-example.txt",
+    },
+]
 
 
 class Example(BaseModel):
     summary: Optional[str] = None
     """
     Short description for the example.
     """
@@ -30,22 +47,18 @@
     This provides the capability to reference examples that cannot easily be included 
     in JSON or YAML documents.
     
     The `value` field and `externalValue` field are mutually exclusive.
     See the rules for resolving [Relative References](#relativeReferencesURI).
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {"summary": "A foo example", "value": {"foo": "bar"}},
-                {
-                    "summary": "This is an example in XML",
-                    "externalValue": "http://example.org/examples/address-example.xml",
-                },
-                {
-                    "summary": "This is a text example",
-                    "externalValue": "http://foo.bar/examples/address-example.txt",
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/external_documentation.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/external_documentation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [{"description": "Find more info here", "url": "https://example.com"}]
 
 
 class ExternalDocumentation(BaseModel):
     """Allows referencing an external resource for extended documentation."""
 
     description: Optional[str] = None
     """
@@ -15,14 +19,18 @@
 
     url: str
     """
     **REQUIRED**. The URL for the target documentation.
     Value MUST be in the form of a URL.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {"description": "Find more info here", "url": "https://example.com"}
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/info.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/info.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .contact import Contact
 from .license import License
 
+_examples = [
+    {
+        "title": "Sample Pet Store App",
+        "summary": "A pet store manager.",
+        "description": "This is a sample server for a pet store.",
+        "termsOfService": "http://example.com/terms/",
+        "contact": {
+            "name": "API Support",
+            "url": "http://www.example.com/support",
+            "email": "support@example.com",
+        },
+        "license": {
+            "name": "Apache 2.0",
+            "url": "https://www.apache.org/licenses/LICENSE-2.0.html",
+        },
+        "version": "1.0.1",
+    }
+]
+
 
 class Info(BaseModel):
     """
     The object provides metadata about the API.
     The metadata MAY be used by the clients if needed,
     and MAY be presented in editing or documentation generation tools for convenience.
     """
@@ -49,29 +70,18 @@
     version: str
     """
     **REQUIRED**. The version of the OpenAPI document
     (which is distinct from the [OpenAPI Specification version](#oasVersion) or the API 
     implementation version).
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "title": "Sample Pet Store App",
-                    "summary": "A pet store manager.",
-                    "description": "This is a sample server for a pet store.",
-                    "termsOfService": "http://example.com/terms/",
-                    "contact": {
-                        "name": "API Support",
-                        "url": "http://www.example.com/support",
-                        "email": "support@example.com",
-                    },
-                    "license": {
-                        "name": "Apache 2.0",
-                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html",
-                    },
-                    "version": "1.0.1",
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/license.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/license.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {"name": "Apache 2.0", "identifier": "Apache-2.0"},
+    {
+        "name": "Apache 2.0",
+        "url": "https://www.apache.org/licenses/LICENSE-2.0.html",
+    },
+]
 
 
 class License(BaseModel):
     """
     License information for the exposed API.
     """
 
@@ -23,18 +33,18 @@
     url: Optional[str] = None
     """
     A URL to the license used for the API.
     This MUST be in the form of a URL.
     The `url` field is mutually exclusive of the `identifier` field.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {"name": "Apache 2.0", "identifier": "Apache-2.0"},
-                {
-                    "name": "Apache 2.0",
-                    "url": "https://www.apache.org/licenses/LICENSE-2.0.html",
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/link.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/link.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 from typing import Any, Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .server import Server
 
+_examples = [
+    {
+        "operationId": "getUserAddressByUUID",
+        "parameters": {"userUuid": "$response.body#/uuid"},
+    },
+    {
+        "operationRef": "#/paths/~12.0~1repositories~1{username}/get",
+        "parameters": {"username": "$response.body#/username"},
+    },
+]
+
 
 class Link(BaseModel):
     """
     The `Link object` represents a possible design-time link for a response.
     The presence of a link does not guarantee the caller's ability to successfully
     invoke it, rather it provides a known relationship and traversal mechanism between
     responses and other operations.
@@ -65,21 +78,18 @@
     """
 
     server: Optional[Server] = None
     """
     A server object to be used by the target operation.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "operationId": "getUserAddressByUUID",
-                    "parameters": {"userUuid": "$response.body#/uuid"},
-                },
-                {
-                    "operationRef": "#/paths/~12.0~1repositories~1{username}/get",
-                    "parameters": {"username": "$response.body#/username"},
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/media_type.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/media_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,47 @@
 from typing import Any, Dict, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .encoding import Encoding
 from .example import Example
 from .reference import Reference
 from .schema import Schema
 
+_examples = [
+    {
+        "schema": {"$ref": "#/components/schemas/Pet"},
+        "examples": {
+            "cat": {
+                "summary": "An example of a cat",
+                "value": {
+                    "name": "Fluffy",
+                    "petType": "Cat",
+                    "color": "White",
+                    "gender": "male",
+                    "breed": "Persian",
+                },
+            },
+            "dog": {
+                "summary": "An example of a dog with a cat's name",
+                "value": {
+                    "name": "Puma",
+                    "petType": "Dog",
+                    "color": "Black",
+                    "gender": "Female",
+                    "breed": "Mixed",
+                },
+            },
+            "frog": {"$ref": "#/components/examples/frog-example"},
+        },
+    }
+]
+
 
 class MediaType(BaseModel):
     """Each Media Type Object provides schema and examples for the media type
     identified by its key."""
 
     media_type_schema: Optional[Union[Reference, Schema]] = Field(
         default=None, alias="schema"
@@ -47,40 +78,20 @@
     """
     A map between a property name and its encoding information.
     The key, being the property name, MUST exist in the schema as a property.
     The encoding object SHALL only apply to `requestBody` objects
     when the media type is `multipart` or `application/x-www-form-urlencoded`.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {
-                    "schema": {"$ref": "#/components/schemas/Pet"},
-                    "examples": {
-                        "cat": {
-                            "summary": "An example of a cat",
-                            "value": {
-                                "name": "Fluffy",
-                                "petType": "Cat",
-                                "color": "White",
-                                "gender": "male",
-                                "breed": "Persian",
-                            },
-                        },
-                        "dog": {
-                            "summary": "An example of a dog with a cat's name",
-                            "value": {
-                                "name": "Puma",
-                                "petType": "Dog",
-                                "color": "Black",
-                                "gender": "Female",
-                                "breed": "Mixed",
-                            },
-                        },
-                        "frog": {"$ref": "#/components/examples/frog-example"},
-                    },
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/oauth_flow.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/oauth_flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,39 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {
+        "authorizationUrl": "https://example.com/api/oauth/dialog",
+        "scopes": {
+            "write:pets": "modify pets in your account",
+            "read:pets": "read your pets",
+        },
+    },
+    {
+        "authorizationUrl": "https://example.com/api/oauth/dialog",
+        "tokenUrl": "https://example.com/api/oauth/token",
+        "scopes": {
+            "write:pets": "modify pets in your account",
+            "read:pets": "read your pets",
+        },
+    },
+    {
+        "authorizationUrl": "/api/oauth/dialog",
+        "tokenUrl": "/api/oauth/token",
+        "refreshUrl": "/api/oauth/token",
+        "scopes": {
+            "write:pets": "modify pets in your account",
+            "read:pets": "read your pets",
+        },
+    },
+]
 
 
 class OAuthFlow(BaseModel):
     """
     Configuration details for a supported OAuth Flow
     """
 
@@ -34,37 +63,18 @@
     scopes: Optional[Dict[str, str]] = None
     """
     **REQUIRED** for `oauth2`. The available scopes for the OAuth2 security scheme.
     A map between the scope name and a short description for it.
     The map MAY be empty.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "authorizationUrl": "https://example.com/api/oauth/dialog",
-                    "scopes": {
-                        "write:pets": "modify pets in your account",
-                        "read:pets": "read your pets",
-                    },
-                },
-                {
-                    "authorizationUrl": "https://example.com/api/oauth/dialog",
-                    "tokenUrl": "https://example.com/api/oauth/token",
-                    "scopes": {
-                        "write:pets": "modify pets in your account",
-                        "read:pets": "read your pets",
-                    },
-                },
-                {
-                    "authorizationUrl": "/api/oauth/dialog",
-                    "tokenUrl": "/api/oauth/token",
-                    "refreshUrl": "/api/oauth/token",
-                    "scopes": {
-                        "write:pets": "modify pets in your account",
-                        "read:pets": "read your pets",
-                    },
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/oauth_flows.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/oauth_flows.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .oauth_flow import OAuthFlow
 
 
 class OAuthFlows(BaseModel):
     """
     Allows configuration of the supported OAuth Flows.
@@ -30,9 +32,16 @@
     authorizationCode: Optional[OAuthFlow] = None
     """
     Configuration for the OAuth Authorization Code flow.
     
     Previously called `accessCode` in OpenAPI 2.0.
     """
 
-    class Config:
-        extra = Extra.allow
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/open_api.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/open_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Dict, List, Literal, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .components import Components
 from .external_documentation import ExternalDocumentation
 from .info import Info
 from .path_item import PathItem
 from .paths import Paths
 from .reference import Reference
@@ -87,9 +89,16 @@
     """
 
     externalDocs: Optional[ExternalDocumentation] = None
     """
     Additional external documentation.
     """
 
-    class Config:
-        extra = Extra.allow
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/operation.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,70 @@
 from typing import Dict, List, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .callback import Callback
 from .external_documentation import ExternalDocumentation
 from .parameter import Parameter
 from .reference import Reference
 from .request_body import RequestBody
 from .responses import Responses
 from .security_requirement import SecurityRequirement
 from .server import Server
 
+_examples = [
+    {
+        "tags": ["pet"],
+        "summary": "Updates a pet in the store with form data",
+        "operationId": "updatePetWithForm",
+        "parameters": [
+            {
+                "name": "petId",
+                "in": "path",
+                "description": "ID of pet that needs to be updated",
+                "required": True,
+                "schema": {"type": "string"},
+            }
+        ],
+        "requestBody": {
+            "content": {
+                "application/x-www-form-urlencoded": {
+                    "schema": {
+                        "type": "object",
+                        "properties": {
+                            "name": {
+                                "description": "Updated name of the pet",
+                                "type": "string",
+                            },
+                            "status": {
+                                "description": "Updated status of the pet",
+                                "type": "string",
+                            },
+                        },
+                        "required": ["status"],
+                    }
+                }
+            }
+        },
+        "responses": {
+            "200": {
+                "description": "Pet updated.",
+                "content": {"application/json": {}, "application/xml": {}},
+            },
+            "405": {
+                "description": "Method Not Allowed",
+                "content": {"application/json": {}, "application/xml": {}},
+            },
+        },
+        "security": [{"petstore_auth": ["write:pets", "read:pets"]}],
+    }
+]
+
 
 class Operation(BaseModel):
     """Describes a single API operation on a path."""
 
     tags: Optional[List[str]] = None
     """
     A list of tags for API documentation control.
@@ -109,58 +159,18 @@
     servers: Optional[List[Server]] = None
     """
     An alternative `server` array to service this operation.
     If an alternative `server` object is specified at the Path Item Object or Root 
     level, it will be overridden by this value.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "tags": ["pet"],
-                    "summary": "Updates a pet in the store with form data",
-                    "operationId": "updatePetWithForm",
-                    "parameters": [
-                        {
-                            "name": "petId",
-                            "in": "path",
-                            "description": "ID of pet that needs to be updated",
-                            "required": True,
-                            "schema": {"type": "string"},
-                        }
-                    ],
-                    "requestBody": {
-                        "content": {
-                            "application/x-www-form-urlencoded": {
-                                "schema": {
-                                    "type": "object",
-                                    "properties": {
-                                        "name": {
-                                            "description": "Updated name of the pet",
-                                            "type": "string",
-                                        },
-                                        "status": {
-                                            "description": "Updated status of the pet",
-                                            "type": "string",
-                                        },
-                                    },
-                                    "required": ["status"],
-                                }
-                            }
-                        }
-                    },
-                    "responses": {
-                        "200": {
-                            "description": "Pet updated.",
-                            "content": {"application/json": {}, "application/xml": {}},
-                        },
-                        "405": {
-                            "description": "Method Not Allowed",
-                            "content": {"application/json": {}, "application/xml": {}},
-                        },
-                    },
-                    "security": [{"petstore_auth": ["write:pets", "read:pets"]}],
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/parameter.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,74 @@
 import enum
 from typing import Any, Dict, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .example import Example
 from .media_type import MediaType
 from .reference import Reference
 from .schema import Schema
 
+_examples = [
+    {
+        "name": "token",
+        "in": "header",
+        "description": "token to be passed as a header",
+        "required": True,
+        "schema": {
+            "type": "array",
+            "items": {"type": "integer", "format": "int64"},
+        },
+        "style": "simple",
+    },
+    {
+        "name": "username",
+        "in": "path",
+        "description": "username to fetch",
+        "required": True,
+        "schema": {"type": "string"},
+    },
+    {
+        "name": "id",
+        "in": "query",
+        "description": "ID of the object to fetch",
+        "required": False,
+        "schema": {"type": "array", "items": {"type": "string"}},
+        "style": "form",
+        "explode": True,
+    },
+    {
+        "in": "query",
+        "name": "freeForm",
+        "schema": {
+            "type": "object",
+            "additionalProperties": {"type": "integer"},
+        },
+        "style": "form",
+    },
+    {
+        "in": "query",
+        "name": "coordinates",
+        "content": {
+            "application/json": {
+                "schema": {
+                    "type": "object",
+                    "required": ["lat", "long"],
+                    "properties": {
+                        "lat": {"type": "number"},
+                        "long": {"type": "number"},
+                    },
+                }
+            }
+        },
+    },
+]
+
 
 class ParameterLocation(str, enum.Enum):
     """The location of a given parameter."""
 
     QUERY = "query"
     HEADER = "header"
     PATH = "path"
@@ -157,66 +214,20 @@
     content: Optional[Dict[str, MediaType]] = None
     """
     A map containing the representations for the parameter.
     The key is the media type and the value describes it.
     The map MUST only contain one entry.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {
-                    "name": "token",
-                    "in": "header",
-                    "description": "token to be passed as a header",
-                    "required": True,
-                    "schema": {
-                        "type": "array",
-                        "items": {"type": "integer", "format": "int64"},
-                    },
-                    "style": "simple",
-                },
-                {
-                    "name": "username",
-                    "in": "path",
-                    "description": "username to fetch",
-                    "required": True,
-                    "schema": {"type": "string"},
-                },
-                {
-                    "name": "id",
-                    "in": "query",
-                    "description": "ID of the object to fetch",
-                    "required": False,
-                    "schema": {"type": "array", "items": {"type": "string"}},
-                    "style": "form",
-                    "explode": True,
-                },
-                {
-                    "in": "query",
-                    "name": "freeForm",
-                    "schema": {
-                        "type": "object",
-                        "additionalProperties": {"type": "integer"},
-                    },
-                    "style": "form",
-                },
-                {
-                    "in": "query",
-                    "name": "coordinates",
-                    "content": {
-                        "application/json": {
-                            "schema": {
-                                "type": "object",
-                                "required": ["lat", "long"],
-                                "properties": {
-                                    "lat": {"type": "number"},
-                                    "long": {"type": "number"},
-                                },
-                            }
-                        }
-                    },
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/path_item.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/path_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,59 @@
 from typing import List, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .operation import Operation
 from .parameter import Parameter
 from .reference import Reference
 from .server import Server
 
+_examples = [
+    {
+        "get": {
+            "description": "Returns pets based on ID",
+            "summary": "Find pets by ID",
+            "operationId": "getPetsById",
+            "responses": {
+                "200": {
+                    "description": "pet response",
+                    "content": {
+                        "*/*": {
+                            "schema": {
+                                "type": "array",
+                                "items": {"$ref": "#/components/schemas/Pet"},
+                            }
+                        }
+                    },
+                },
+                "default": {
+                    "description": "error payload",
+                    "content": {
+                        "text/html": {
+                            "schema": {"$ref": "#/components/schemas/ErrorModel"}
+                        }
+                    },
+                },
+            },
+        },
+        "parameters": [
+            {
+                "name": "id",
+                "in": "path",
+                "description": "ID of pet to use",
+                "required": True,
+                "schema": {"type": "array", "items": {"type": "string"}},
+                "style": "simple",
+            }
+        ],
+    }
+]
+
 
 class PathItem(BaseModel):
     """
     Describes the operations available on a single path.
     A Path Item MAY be empty, due to [ACL constraints](#securityFiltering).
     The path itself is still exposed to the documentation viewer
     but they will not know which operations and parameters are available.
@@ -91,56 +134,20 @@
     removed there. The list MUST NOT include duplicated parameters.
     A unique parameter is defined by a combination of a [name](#parameterName) and 
     [location](#parameterIn). The list can use the [Reference Object](#referenceObject) 
     to link to parameters that are defined at the 
     [OpenAPI Object's components/parameters](#componentsParameters).
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {
-                    "get": {
-                        "description": "Returns pets based on ID",
-                        "summary": "Find pets by ID",
-                        "operationId": "getPetsById",
-                        "responses": {
-                            "200": {
-                                "description": "pet response",
-                                "content": {
-                                    "*/*": {
-                                        "schema": {
-                                            "type": "array",
-                                            "items": {
-                                                "$ref": "#/components/schemas/Pet"
-                                            },
-                                        }
-                                    }
-                                },
-                            },
-                            "default": {
-                                "description": "error payload",
-                                "content": {
-                                    "text/html": {
-                                        "schema": {
-                                            "$ref": "#/components/schemas/ErrorModel"
-                                        }
-                                    }
-                                },
-                            },
-                        },
-                    },
-                    "parameters": [
-                        {
-                            "name": "id",
-                            "in": "path",
-                            "description": "ID of pet to use",
-                            "required": True,
-                            "schema": {"type": "array", "items": {"type": "string"}},
-                            "style": "simple",
-                        }
-                    ],
-                }
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/paths.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/reference.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/reference.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {"$ref": "#/components/schemas/Pet"},
+    {"$ref": "Pet.json"},
+    {"$ref": "definitions.json#/Pet"},
+]
 
 
 class Reference(BaseModel):
     """
     A simple object to allow referencing other components in the OpenAPI document.
 
     The `$ref` string value contains a URI [RFC3986](https://tools.ietf.org/html/rfc3986),
@@ -28,17 +36,20 @@
     A description which by default SHOULD override that of the referenced component.
     [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text 
     representation.
     If the referenced object-type does not allow a `description` field, then this field 
     has no effect.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {"$ref": "#/components/schemas/Pet"},
-                {"$ref": "Pet.json"},
-                {"$ref": "definitions.json#/Pet"},
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/request_body.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/request_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,63 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .media_type import MediaType
 
+_examples = [
+    {
+        "description": "user to add to the system",
+        "content": {
+            "application/json": {
+                "schema": {"$ref": "#/components/schemas/User"},
+                "examples": {
+                    "user": {
+                        "summary": "User Example",
+                        "externalValue": "http://foo.bar/examples/user-example.json",
+                    }
+                },
+            },
+            "application/xml": {
+                "schema": {"$ref": "#/components/schemas/User"},
+                "examples": {
+                    "user": {
+                        "summary": "User example in XML",
+                        "externalValue": "http://foo.bar/examples/user-example.xml",
+                    }
+                },
+            },
+            "text/plain": {
+                "examples": {
+                    "user": {
+                        "summary": "User example in Plain text",
+                        "externalValue": "http://foo.bar/examples/user-example.txt",
+                    }
+                }
+            },
+            "*/*": {
+                "examples": {
+                    "user": {
+                        "summary": "User example in other format",
+                        "externalValue": "http://foo.bar/examples/user-example.whatever",
+                    }
+                }
+            },
+        },
+    },
+    {
+        "description": "user to add to the system",
+        "content": {
+            "text/plain": {"schema": {"type": "array", "items": {"type": "string"}}}
+        },
+    },
+]
+
 
 class RequestBody(BaseModel):
     """Describes a single request body."""
 
     description: Optional[str] = None
     """
     A brief description of the request body.
@@ -28,60 +78,18 @@
     """
 
     required: bool = False
     """
     Determines if the request body is required in the request. Defaults to `false`.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "description": "user to add to the system",
-                    "content": {
-                        "application/json": {
-                            "schema": {"$ref": "#/components/schemas/User"},
-                            "examples": {
-                                "user": {
-                                    "summary": "User Example",
-                                    "externalValue": "http://foo.bar/examples/user-example.json",
-                                }
-                            },
-                        },
-                        "application/xml": {
-                            "schema": {"$ref": "#/components/schemas/User"},
-                            "examples": {
-                                "user": {
-                                    "summary": "User example in XML",
-                                    "externalValue": "http://foo.bar/examples/user-example.xml",
-                                }
-                            },
-                        },
-                        "text/plain": {
-                            "examples": {
-                                "user": {
-                                    "summary": "User example in Plain text",
-                                    "externalValue": "http://foo.bar/examples/user-example.txt",
-                                }
-                            }
-                        },
-                        "*/*": {
-                            "examples": {
-                                "user": {
-                                    "summary": "User example in other format",
-                                    "externalValue": "http://foo.bar/examples/user-example.whatever",
-                                }
-                            }
-                        },
-                    },
-                },
-                {
-                    "description": "user to add to the system",
-                    "content": {
-                        "text/plain": {
-                            "schema": {"type": "array", "items": {"type": "string"}}
-                        }
-                    },
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/response.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,57 @@
 from typing import Dict, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .header import Header
 from .link import Link
 from .media_type import MediaType
 from .reference import Reference
 
+_examples = [
+    {
+        "description": "A complex object array response",
+        "content": {
+            "application/json": {
+                "schema": {
+                    "type": "array",
+                    "items": {"$ref": "#/components/schemas/VeryComplexType"},
+                }
+            }
+        },
+    },
+    {
+        "description": "A simple string response",
+        "content": {"text/plain": {"schema": {"type": "string"}}},
+    },
+    {
+        "description": "A simple string response",
+        "content": {"text/plain": {"schema": {"type": "string", "example": "whoa!"}}},
+        "headers": {
+            "X-Rate-Limit-Limit": {
+                "description": "The number of allowed requests in the "
+                "current period",
+                "schema": {"type": "integer"},
+            },
+            "X-Rate-Limit-Remaining": {
+                "description": "The number of remaining requests in the "
+                "current period",
+                "schema": {"type": "integer"},
+            },
+            "X-Rate-Limit-Reset": {
+                "description": "The number of seconds left in the current period",
+                "schema": {"type": "integer"},
+            },
+        },
+    },
+    {"description": "object created"},
+]
+
 
 class Response(BaseModel):
     """
     Describes a single response from an API Operation, including design-time,
     static `links` to operations based on the response.
     """
 
@@ -42,54 +83,18 @@
     links: Optional[Dict[str, Union[Link, Reference]]] = None
     """
     A map of operations links that can be followed from the response.
     The key of the map is a short name for the link, following the naming constraints 
     of the names for [Component Objects](#componentsObject).
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "description": "A complex object array response",
-                    "content": {
-                        "application/json": {
-                            "schema": {
-                                "type": "array",
-                                "items": {
-                                    "$ref": "#/components/schemas/VeryComplexType"
-                                },
-                            }
-                        }
-                    },
-                },
-                {
-                    "description": "A simple string response",
-                    "content": {"text/plain": {"schema": {"type": "string"}}},
-                },
-                {
-                    "description": "A simple string response",
-                    "content": {
-                        "text/plain": {"schema": {"type": "string", "example": "whoa!"}}
-                    },
-                    "headers": {
-                        "X-Rate-Limit-Limit": {
-                            "description": "The number of allowed requests in the "
-                            "current period",
-                            "schema": {"type": "integer"},
-                        },
-                        "X-Rate-Limit-Remaining": {
-                            "description": "The number of remaining requests in the "
-                            "current period",
-                            "schema": {"type": "integer"},
-                        },
-                        "X-Rate-Limit-Reset": {
-                            "description": "The number of seconds left in the current "
-                            "period",
-                            "schema": {"type": "integer"},
-                        },
-                    },
-                },
-                {"description": "object created"},
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/responses.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/schema.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,117 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra, min_length_arg
 
 from .datatype import DataType
 from .discriminator import Discriminator
 from .external_documentation import ExternalDocumentation
 from .reference import Reference
 from .xml import XML
 
+_examples = [
+    {"type": "string", "format": "email"},
+    {
+        "type": "object",
+        "required": ["name"],
+        "properties": {
+            "name": {"type": "string"},
+            "address": {"$ref": "#/components/schemas/Address"},
+            "age": {"type": "integer", "format": "int32", "minimum": 0},
+        },
+    },
+    {"type": "object", "additionalProperties": {"type": "string"}},
+    {
+        "type": "object",
+        "additionalProperties": {"$ref": "#/components/schemas/ComplexModel"},
+    },
+    {
+        "type": "object",
+        "properties": {
+            "id": {"type": "integer", "format": "int64"},
+            "name": {"type": "string"},
+        },
+        "required": ["name"],
+        "example": {"name": "Puma", "id": 1},
+    },
+    {
+        "type": "object",
+        "required": ["message", "code"],
+        "properties": {
+            "message": {"type": "string"},
+            "code": {"type": "integer", "minimum": 100, "maximum": 600},
+        },
+    },
+    {
+        "allOf": [
+            {"$ref": "#/components/schemas/ErrorModel"},
+            {
+                "type": "object",
+                "required": ["rootCause"],
+                "properties": {"rootCause": {"type": "string"}},
+            },
+        ]
+    },
+    {
+        "type": "object",
+        "discriminator": {"propertyName": "petType"},
+        "properties": {
+            "name": {"type": "string"},
+            "petType": {"type": "string"},
+        },
+        "required": ["name", "petType"],
+    },
+    {
+        "description": "A representation of a cat. "
+        "Note that `Cat` will be used as the discriminator value.",
+        "allOf": [
+            {"$ref": "#/components/schemas/Pet"},
+            {
+                "type": "object",
+                "properties": {
+                    "huntingSkill": {
+                        "type": "string",
+                        "description": "The measured skill for hunting",
+                        "default": "lazy",
+                        "enum": [
+                            "clueless",
+                            "lazy",
+                            "adventurous",
+                            "aggressive",
+                        ],
+                    }
+                },
+                "required": ["huntingSkill"],
+            },
+        ],
+    },
+    {
+        "description": "A representation of a dog. "
+        "Note that `Dog` will be used as the discriminator value.",
+        "allOf": [
+            {"$ref": "#/components/schemas/Pet"},
+            {
+                "type": "object",
+                "properties": {
+                    "packSize": {
+                        "type": "integer",
+                        "format": "int32",
+                        "description": "the size of the pack the dog is from",
+                        "default": 0,
+                        "minimum": 0,
+                    }
+                },
+                "required": ["packSize"],
+            },
+        ],
+    },
+]
+
 
 class Schema(BaseModel):
     """
     The Schema Object allows the definition of input and output data types.
     These types can be objects, but also primitives and arrays.
     This object is a superset of
     the [JSON Schema Specification Draft 2020-12](https://tools.ietf.org/html/draft-bhutton-json-schema-00).
@@ -373,15 +473,15 @@
     "boolean", "object", "array", "number", or "string"), or "integer"
     which matches any number with a zero fractional part.
     
     An instance validates if and only if the instance is in any of the
     sets listed for this keyword.
     """
 
-    enum: Optional[List[Any]] = Field(default=None, min_items=1)
+    enum: Optional[List[Any]] = Field(default=None, **min_length_arg(1))
     """
     The value of this keyword MUST be an array.  This array SHOULD have
     at least one element.  Elements in the array SHOULD be unique.
     
     An instance validates successfully against this keyword if its value
     is equal to one of the elements in this keyword's array value.
     
@@ -835,112 +935,38 @@
     
     Deprecated: The example property has been deprecated in favor of the JSON Schema 
     examples keyword.
     Use of example is discouraged, and later versions of this specification may remove 
     it.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {"type": "string", "format": "email"},
-                {
-                    "type": "object",
-                    "required": ["name"],
-                    "properties": {
-                        "name": {"type": "string"},
-                        "address": {"$ref": "#/components/schemas/Address"},
-                        "age": {"type": "integer", "format": "int32", "minimum": 0},
-                    },
-                },
-                {"type": "object", "additionalProperties": {"type": "string"}},
-                {
-                    "type": "object",
-                    "additionalProperties": {
-                        "$ref": "#/components/schemas/ComplexModel"
-                    },
-                },
-                {
-                    "type": "object",
-                    "properties": {
-                        "id": {"type": "integer", "format": "int64"},
-                        "name": {"type": "string"},
-                    },
-                    "required": ["name"],
-                    "example": {"name": "Puma", "id": 1},
-                },
-                {
-                    "type": "object",
-                    "required": ["message", "code"],
-                    "properties": {
-                        "message": {"type": "string"},
-                        "code": {"type": "integer", "minimum": 100, "maximum": 600},
-                    },
-                },
-                {
-                    "allOf": [
-                        {"$ref": "#/components/schemas/ErrorModel"},
-                        {
-                            "type": "object",
-                            "required": ["rootCause"],
-                            "properties": {"rootCause": {"type": "string"}},
-                        },
-                    ]
-                },
-                {
-                    "type": "object",
-                    "discriminator": {"propertyName": "petType"},
-                    "properties": {
-                        "name": {"type": "string"},
-                        "petType": {"type": "string"},
-                    },
-                    "required": ["name", "petType"],
-                },
-                {
-                    "description": "A representation of a cat. "
-                    "Note that `Cat` will be used as the discriminator value.",
-                    "allOf": [
-                        {"$ref": "#/components/schemas/Pet"},
-                        {
-                            "type": "object",
-                            "properties": {
-                                "huntingSkill": {
-                                    "type": "string",
-                                    "description": "The measured skill for hunting",
-                                    "default": "lazy",
-                                    "enum": [
-                                        "clueless",
-                                        "lazy",
-                                        "adventurous",
-                                        "aggressive",
-                                    ],
-                                }
-                            },
-                            "required": ["huntingSkill"],
-                        },
-                    ],
-                },
-                {
-                    "description": "A representation of a dog. "
-                    "Note that `Dog` will be used as the discriminator value.",
-                    "allOf": [
-                        {"$ref": "#/components/schemas/Pet"},
-                        {
-                            "type": "object",
-                            "properties": {
-                                "packSize": {
-                                    "type": "integer",
-                                    "format": "int32",
-                                    "description": "the size of the pack the dog is "
-                                    "from",
-                                    "default": 0,
-                                    "minimum": 0,
-                                }
-                            },
-                            "required": ["packSize"],
-                        },
-                    ],
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
+
+
+if TYPE_CHECKING:
+
+    def schema_validate(
+        obj: Any,
+        *,
+        strict: bool | None = None,
+        from_attributes: bool | None = None,
+        context: dict[str, Any] | None = None
+    ) -> Schema:
+        ...
+
+elif PYDANTIC_V2:
+    schema_validate = Schema.model_validate
+
+else:
+    schema_validate = Schema.parse_obj
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/security_requirement.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/security_scheme.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/security_scheme.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,41 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .oauth_flows import OAuthFlows
 
+_examples = [
+    {"type": "http", "scheme": "basic"},
+    {"type": "apiKey", "name": "api_key", "in": "header"},
+    {"type": "http", "scheme": "bearer", "bearerFormat": "JWT"},
+    {
+        "type": "oauth2",
+        "flows": {
+            "implicit": {
+                "authorizationUrl": "https://example.com/api/oauth/dialog",
+                "scopes": {
+                    "write:pets": "modify pets in your account",
+                    "read:pets": "read your pets",
+                },
+            }
+        },
+    },
+    {
+        "type": "openIdConnect",
+        "openIdConnectUrl": "https://example.com/openIdConnect",
+    },
+    {
+        "type": "openIdConnect",
+        "openIdConnectUrl": "openIdConnect",
+    },  # issue #5: allow relative path
+]
+
 
 class SecurityScheme(BaseModel):
     """
     Defines a security scheme that can be used by the operations.
 
     Supported schemes are HTTP authentication,
     an API key (either as a header, a cookie parameter or as a query parameter),
@@ -72,37 +100,20 @@
     openIdConnectUrl: Optional[str] = None
     """
     **REQUIRED** for `openIdConnect`. OpenId Connect URL to discover OAuth2 
     configuration values. This MUST be in the form of a URL. The OpenID Connect 
     standard requires the use of TLS.
     """
 
-    class Config:
-        extra = Extra.allow
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {"type": "http", "scheme": "basic"},
-                {"type": "apiKey", "name": "api_key", "in": "header"},
-                {"type": "http", "scheme": "bearer", "bearerFormat": "JWT"},
-                {
-                    "type": "oauth2",
-                    "flows": {
-                        "implicit": {
-                            "authorizationUrl": "https://example.com/api/oauth/dialog",
-                            "scopes": {
-                                "write:pets": "modify pets in your account",
-                                "read:pets": "read your pets",
-                            },
-                        }
-                    },
-                },
-                {
-                    "type": "openIdConnect",
-                    "openIdConnectUrl": "https://example.com/openIdConnect",
-                },
-                {
-                    "type": "openIdConnect",
-                    "openIdConnectUrl": "openIdConnect",
-                },  # issue #5: allow relative path
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            populate_by_name=True,
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            allow_population_by_field_name = True
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/server.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_0_3/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .server_variable import ServerVariable
 
+_examples = [
+    {
+        "url": "https://development.gigantic-server.com/v1",
+        "description": "Development server",
+    },
+    {
+        "url": "https://{username}.gigantic-server.com:{port}/{basePath}",
+        "description": "The production API server",
+        "variables": {
+            "username": {
+                "default": "demo",
+                "description": "this value is assigned by the service"
+                "provider, in this example `gigantic-server.com`",
+            },
+            "port": {"enum": ["8443", "443"], "default": "8443"},
+            "basePath": {"default": "v2"},
+        },
+    },
+]
+
 
 class Server(BaseModel):
     """An object representing a Server."""
 
     url: str
     """
     **REQUIRED**. A URL to the target host.
@@ -28,30 +50,18 @@
     variables: Optional[Dict[str, ServerVariable]] = None
     """
     A map between a variable name and its value.
     
     The value is used for substitution in the server's URL template.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {
-                    "url": "https://development.gigantic-server.com/v1",
-                    "description": "Development server",
-                },
-                {
-                    "url": "https://{username}.gigantic-server.com:{port}/{basePath}",
-                    "description": "The production API server",
-                    "variables": {
-                        "username": {
-                            "default": "demo",
-                            "description": "this value is assigned by the service "
-                            "provider, in this example `gigantic-server.com`",
-                        },
-                        "port": {"enum": ["8443", "443"], "default": "8443"},
-                        "basePath": {"default": "v2"},
-                    },
-                },
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/tag.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/tag.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
 
 from .external_documentation import ExternalDocumentation
 
+_examples = [{"name": "pet", "description": "Pets operations"}]
+
 
 class Tag(BaseModel):
     """
     Adds metadata to a single tag that is used by the
     [Operation Object](#operationObject).
     It is not mandatory to have a Tag Object per tag defined in the Operation Object
     instances.
@@ -26,10 +30,18 @@
     """
 
     externalDocs: Optional[ExternalDocumentation] = None
     """
     Additional external documentation for this tag.
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {"examples": [{"name": "pet", "description": "Pets operations"}]}
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/openapi_pydantic/v3/v3_1_0/xml.py` & `openapi_pydantic-0.3.0/openapi_pydantic/v3/v3_1_0/xml.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
+
+from openapi_pydantic.compat import PYDANTIC_V2, ConfigDict, Extra
+
+_examples = [
+    {"name": "animal"},
+    {"attribute": True},
+    {"wrapped": True},
+    {"namespace": "http://example.com/schema/sample", "prefix": "sample"},
+    {"name": "aliens", "wrapped": True},
+]
 
 
 class XML(BaseModel):
     """
     A metadata object that allows for more fine-tuned XML model definitions.
 
     When using arrays, XML element names are *not* inferred (for singular/plural forms)
@@ -45,18 +55,18 @@
     Signifies whether the array is wrapped 
     (for example, `<books><book/><book/></books>`) or unwrapped (`<book/><book/>`).
     Default value is `false`.
     The definition takes effect only when defined alongside `type` being `array` 
     (outside the `items`).
     """
 
-    class Config:
-        extra = Extra.allow
-        schema_extra = {
-            "examples": [
-                {"name": "animal"},
-                {"attribute": True},
-                {"wrapped": True},
-                {"namespace": "http://example.com/schema/sample", "prefix": "sample"},
-                {"name": "aliens", "wrapped": True},
-            ]
-        }
+    if PYDANTIC_V2:
+        model_config = ConfigDict(
+            extra="allow",
+            json_schema_extra={"examples": _examples},
+        )
+
+    else:
+
+        class Config:
+            extra = Extra.allow
+            schema_extra = {"examples": _examples}
```

### Comparing `openapi_pydantic-0.2.2/pyproject.toml` & `openapi_pydantic-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-pydantic"
-version = "0.2.2"
+version = "0.3.0"
 description = "Pydantic OpenAPI schema implementation"
 authors = ["Mike Oakley <mike-oakley@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/mike-oakley/openapi-pydantic"
 license = "MIT"
 keywords = [
   "openapi",
@@ -19,15 +19,15 @@
   "Operating System :: OS Independent",
   "Framework :: Pydantic",
 ]
 include = ["openapi_pydantic/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "^1.8.2"
+pydantic = ">=1.8"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
```

### Comparing `openapi_pydantic-0.2.2/PKG-INFO` & `openapi_pydantic-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic
-Version: 0.2.2
+Version: 0.3.0
 Summary: Pydantic OpenAPI schema implementation
 Home-page: https://github.com/mike-oakley/openapi-pydantic
 License: MIT
 Keywords: openapi,schema,parser,pydantic,validation
 Author: Mike Oakley
 Author-email: mike-oakley@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -12,28 +12,30 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: pydantic (>=1.8)
 Project-URL: Repository, https://github.com/mike-oakley/openapi-pydantic
 Description-Content-Type: text/markdown
 
 # openapi-pydantic
 
 [![PyPI](https://img.shields.io/pypi/v/openapi-pydantic)](https://pypi.org/project/openapi-pydantic/)
 [![PyPI - License](https://img.shields.io/pypi/l/openapi-pydantic)](https://github.com/mike-oakley/openapi-pydantic/blob/main/LICENSE)
 
-OpenAPI schema implemented in [Pydantic](https://github.com/samuelcolvin/pydantic).
+OpenAPI schema implemented in [Pydantic](https://github.com/samuelcolvin/pydantic). Both Pydantic 1.8+ and 2.x are supported.
 
 The naming of the classes follows the schema in 
 [OpenAPI specification](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.1.0.md#schema).
 
+> This library is forked from [OpenAPI Schema Pydantic](https://github.com/kuimono/openapi-schema-pydantic)  (at version [1.2.4](https://github.com/kuimono/openapi-schema-pydantic/releases/tag/v1.2.4)) which is no longer actively maintained.
+
 ## Installation
 
 `pip install openapi-pydantic`
 
 ## Try me
 
 ```python
@@ -53,15 +55,16 @@
                         description="pong"
                     )
                 }
             )
         )
     },
 )
-print(open_api.json(by_alias=True, exclude_none=True, indent=2))
+# Note: for Pydantic 1.x, replace `model_dump_json` with `json`
+print(open_api.model_dump_json(by_alias=True, exclude_none=True, indent=2))
 ```
 
 Result:
 
 ```json
 {
   "openapi": "3.1.0",
@@ -87,73 +90,77 @@
     }
   }
 }
 ```
 
 ## Take advantage of Pydantic
 
-Pydantic is a great tool, allow you to use object / dict / mixed data for for input.
+Pydantic is a great tool. It allows you to use object / dict / mixed data for input.
 
 The following examples give the same OpenAPI result as above:
 
 ```python
 from openapi_pydantic import parse_obj, OpenAPI, PathItem, Response
 
 # Construct OpenAPI from dict, inferring the correct schema version
 open_api = parse_obj({
+    "openapi": "3.1.0",
     "info": {"title": "My own API", "version": "v0.0.1"},
     "paths": {
         "/ping": {
             "get": {"responses": {"200": {"description": "pong"}}}
         }
     },
 })
 
 
 # Construct OpenAPI v3.1.0 schema from dict
-open_api = OpenAPI.parse_obj({
+# Note: for Pydantic 1.x, replace `model_validate` with `parse_obj`
+open_api = OpenAPI.model_validate({
     "info": {"title": "My own API", "version": "v0.0.1"},
     "paths": {
         "/ping": {
             "get": {"responses": {"200": {"description": "pong"}}}
         }
     },
 })
 
 # Construct OpenAPI with mix of dict/object
-open_api = OpenAPI.parse_obj({
+# Note: for Pydantic 1.x, replace `model_validate` with `parse_obj`
+open_api = OpenAPI.model_validate({
     "info": {"title": "My own API", "version": "v0.0.1"},
     "paths": {
         "/ping": PathItem(
             get={"responses": {"200": Response(description="pong")}}
         )
     },
 })
 ```
 
 ## Use Pydantic classes as schema
 
 - The [Schema Object](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md#schemaObject)
-  in OpenAPI has definitions and tweaks in JSON Schema, which is hard to comprehend and define a good data class
-- Pydantic already has a good way to [create JSON schema](https://pydantic-docs.helpmanual.io/usage/schema/),
-  let's not re-invent the wheel
-  
+  in OpenAPI has definitions and tweaks in JSON Schema, which are hard to comprehend and define a good data class
+- Pydantic already has a good way to [create JSON schema](https://pydantic-docs.helpmanual.io/usage/schema/).
+  Let's not reinvent the wheel.
+
 The approach to deal with this:
 
 1. Use `PydanticSchema` objects to represent the `Schema` in `OpenAPI` object
 2. Invoke `construct_open_api_with_schema_class` to resolve the JSON schemas and references
 
 ```python
 from pydantic import BaseModel, Field
 
 from openapi_pydantic import OpenAPI
 from openapi_pydantic.util import PydanticSchema, construct_open_api_with_schema_class
 
 def construct_base_open_api() -> OpenAPI:
-    return OpenAPI.parse_obj({
+    # Note: for Pydantic 1.x, replace `model_validate` with `parse_obj`
+    return OpenAPI.model_validate({
         "info": {"title": "My own API", "version": "v0.0.1"},
         "paths": {
             "/ping": {
                 "post": {
                     "requestBody": {"content": {"application/json": {
                         "schema": PydanticSchema(schema_class=PingRequest)
                     }}},
@@ -178,15 +185,16 @@
     resp_foo: str = Field(description="foo value of the response")
     resp_bar: str = Field(description="bar value of the response")
 
 open_api = construct_base_open_api()
 open_api = construct_open_api_with_schema_class(open_api)
 
 # print the result openapi.json
-print(open_api.json(by_alias=True, exclude_none=True, indent=2))
+# Note: for Pydantic 1.x, replace `model_dump_json` with `json`
+print(open_api.model_dump_json(by_alias=True, exclude_none=True, indent=2))
 ```
 
 Result:
 
 ```json
 {
   "openapi": "3.1.0",
@@ -275,29 +283,32 @@
     }
   }
 }
 ```
 
 ## Notes
 
-### Use of OpenAPI.json() / OpenAPI.dict()
+### Use of OpenAPI.model_dump() / OpenAPI.model_dump_json() / OpenAPI.json() / OpenAPI.dict()
 
-When using `OpenAPI.json()` / `OpenAPI.dict()` function,
-arguments `by_alias=True, exclude_none=True` has to be in place.
-Otherwise the result json will not fit the OpenAPI standard.
+When using `OpenAPI.model_dump()` / `OpenAPI.model_dump_json()` / `OpenAPI.json()` / `OpenAPI.dict()` functions,
+the arguments `by_alias=True, exclude_none=True` have to be in place.
+Otherwise the resulting json will not fit the OpenAPI standard.
 
 ```python
-# OK
+# OK (Pydantic 2)
+open_api.model_dump_json(by_alias=True, exclude_none=True, indent=2)
+# OK (Pydantic 1)
 open_api.json(by_alias=True, exclude_none=True, indent=2)
 
 # Not good
+open_api.model_dump_json(indent=2)
 open_api.json(indent=2)
 ```
 
-More info about field alias:
+More info about field aliases:
 
 | OpenAPI version | Field alias info |
 | --------------- | ---------------- |
 | 3.1.0 | [here](https://github.com/mike-oakley/openapi-pydantic/blob/main/openapi_pydantic/v3/v3_1_0/README.md#alias) |
 | 3.0.3 | [here](https://github.com/mike-oakley/openapi-pydantic/blob/main/openapi_pydantic/v3/v3_0_3/README.md#alias) |
 
 ### Non-pydantic schema types
@@ -309,21 +320,25 @@
 | --------------- | ----------------------------- |
 | 3.1.0 | [here](https://github.com/mike-oakley/openapi-pydantic/blob/main/openapi_pydantic/v3/v3_1_0/README.md#non-pydantic-schema-types) |
 | 3.0.3 | [here](https://github.com/mike-oakley/openapi-pydantic/blob/main/openapi_pydantic/v3/v3_0_3/README.md#non-pydantic-schema-types) |
 
 ### Use OpenAPI 3.0.3 instead of 3.1.0
 
 Some UI renderings (e.g. Swagger) still do not support OpenAPI 3.1.0.
-It is allowed to use the old 3.0.3 version by importing from different paths:
+The old 3.0.3 version is available by importing from different paths:
 
 ```python
 from openapi_pydantic.v3.v3_0_3 import OpenAPI, ...
 from openapi_pydantic.v3.v3_0_3.util import PydanticSchema, construct_open_api_with_schema_class
 ```
 
+### Pydantic version compatibility
+
+Compatibility with both major versions of Pydantic (1.8+ and 2.*) is mostly achieved using a module called `compat.py`. It detects the installed version of Pydantic and exports version-specific symbols for use by the rest of the package. It also provides all symbols necessary for type checking. The `compat.py` module is not intended to be imported by other packages, but other packages may find it helpful as an example of how to span major versions of Pydantic.
+
 ## Credits
 
 This library is based from the original implementation by Kuimono of [OpenAPI Schema Pydantic](https://github.com/kuimono/openapi-schema-pydantic) which is no longer actively maintained.
 
 ## License
 
 [MIT License](https://github.com/mike-oakley/openapi-pydantic/blob/main/LICENSE)
```

