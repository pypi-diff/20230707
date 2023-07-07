# Comparing `tmp/pait-1.0.0a6.tar.gz` & `tmp/pait-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pait-1.0.0a6.tar", max compression
+gzip compressed data, was "pait-1.0.0a7.tar", max compression
```

## Comparing `pait-1.0.0a6.tar` & `pait-1.0.0a7.tar`

### file list

```diff
@@ -1,183 +1,162 @@
--rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 pait-1.0.0a6/LICENSE
--rw-r--r--   0        0        0     5244 2023-05-10 15:19:11.464788 pait-1.0.0a6/README.md
--rw-r--r--   0        0        0       37 2023-05-24 03:47:38.134524 pait-1.0.0a6/pait/__init__.py
--rw-r--r--   0        0        0       31 2023-07-03 06:00:19.859163 pait-1.0.0a6/pait/__version__.py
--rw-r--r--   0        0        0      216 2023-07-03 05:59:15.586022 pait-1.0.0a6/pait/app/__init__.py
--rw-r--r--   0        0        0     5528 2023-05-23 09:37:37.084528 pait-1.0.0a6/pait/app/any/__init__.py
--rw-r--r--   0        0        0      535 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/any/plugin/__init__.py
--rw-r--r--   0        0        0      460 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/any/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0      425 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/any/plugin/cache_response.py
--rw-r--r--   0        0        0      405 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/any/plugin/check_json_resp.py
--rw-r--r--   0        0        0      373 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/any/plugin/mock_response.py
--rw-r--r--   0        0        0      424 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/any/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-17 11:47:59.744123 pait-1.0.0a6/pait/app/any/security/__init__.py
--rw-r--r--   0        0        0      342 2023-02-08 03:58:49.610123 pait-1.0.0a6/pait/app/any/security/api_key.py
--rw-r--r--   0        0        0      653 2023-02-10 15:24:31.281635 pait-1.0.0a6/pait/app/any/security/http.py
--rw-r--r--   0        0        0      660 2023-02-08 03:43:07.655826 pait-1.0.0a6/pait/app/any/security/oauth2.py
--rw-r--r--   0        0        0     1328 2023-01-18 19:31:20.014191 pait-1.0.0a6/pait/app/any/util.py
--rw-r--r--   0        0        0      562 2023-02-15 10:04:32.538762 pait-1.0.0a6/pait/app/auto_load_app.py
--rw-r--r--   0        0        0      121 2023-01-09 15:13:50.000000 pait-1.0.0a6/pait/app/base/__init__.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a6/pait/app/base/adapter/__init__.py
--rw-r--r--   0        0        0     2427 2023-04-08 08:28:39.674480 pait-1.0.0a6/pait/app/base/adapter/request.py
--rw-r--r--   0        0        0     1806 2023-05-10 15:19:11.476786 pait-1.0.0a6/pait/app/base/app_helper.py
--rw-r--r--   0        0        0        0 2023-02-10 10:23:08.836059 pait-1.0.0a6/pait/app/base/security/__init__.py
--rw-r--r--   0        0        0     1636 2023-05-24 16:45:31.309997 pait-1.0.0a6/pait/app/base/security/api_key.py
--rw-r--r--   0        0        0      656 2023-06-20 03:10:53.261639 pait-1.0.0a6/pait/app/base/security/base.py
--rw-r--r--   0        0        0     7130 2023-05-24 16:53:10.775208 pait-1.0.0a6/pait/app/base/security/http.py
--rw-r--r--   0        0        0     4978 2023-05-24 16:53:10.759208 pait-1.0.0a6/pait/app/base/security/oauth2.py
--rw-r--r--   0        0        0      794 2023-05-16 11:28:00.165083 pait-1.0.0a6/pait/app/base/security/util.py
--rw-r--r--   0        0        0      649 2023-05-10 15:19:11.476786 pait-1.0.0a6/pait/app/base/simple_route.py
--rw-r--r--   0        0        0    13846 2023-05-23 07:58:06.372833 pait-1.0.0a6/pait/app/base/test_helper.py
--rw-r--r--   0        0        0      332 2023-07-03 05:59:15.586022 pait-1.0.0a6/pait/app/flask/__init__.py
--rw-r--r--   0        0        0      719 2023-03-21 10:06:14.408062 pait-1.0.0a6/pait/app/flask/_app_helper.py
--rw-r--r--   0        0        0      394 2023-03-21 10:06:14.408062 pait-1.0.0a6/pait/app/flask/_attribute.py
--rw-r--r--   0        0        0      792 2023-05-10 15:19:11.476786 pait-1.0.0a6/pait/app/flask/_exception.py
--rw-r--r--   0        0        0     3495 2023-05-10 15:19:11.476786 pait-1.0.0a6/pait/app/flask/_load_app.py
--rw-r--r--   0        0        0      269 2022-01-10 09:58:31.000000 pait-1.0.0a6/pait/app/flask/_pait.py
--rw-r--r--   0        0        0     1775 2023-05-10 15:19:11.476786 pait-1.0.0a6/pait/app/flask/_simple_route.py
--rw-r--r--   0        0        0     1900 2023-05-10 15:19:11.476786 pait-1.0.0a6/pait/app/flask/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a6/pait/app/flask/adapter/__init__.py
--rw-r--r--   0        0        0     1689 2023-04-08 08:28:39.674480 pait-1.0.0a6/pait/app/flask/adapter/request.py
--rw-r--r--   0        0        0     1070 2023-05-10 15:19:11.476786 pait-1.0.0a6/pait/app/flask/adapter/response.py
--rw-r--r--   0        0        0      784 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/flask/plugin/__init__.py
--rw-r--r--   0        0        0      117 2023-02-06 11:24:42.996357 pait-1.0.0a6/pait/app/flask/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0      138 2023-05-23 09:37:36.512526 pait-1.0.0a6/pait/app/flask/plugin/cache_response.py
--rw-r--r--   0        0        0      556 2023-05-10 15:19:11.476786 pait-1.0.0a6/pait/app/flask/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1208 2023-05-23 03:11:41.942069 pait-1.0.0a6/pait/app/flask/plugin/mock_response.py
--rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/flask/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a6/pait/app/flask/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/flask/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/flask/security/http.py
--rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/flask/security/oauth2.py
--rw-r--r--   0        0        0      321 2023-05-10 15:19:11.476786 pait-1.0.0a6/pait/app/flask/security/util.py
--rw-r--r--   0        0        0      332 2023-07-03 05:59:15.586022 pait-1.0.0a6/pait/app/sanic/__init__.py
--rw-r--r--   0        0        0      938 2023-03-21 10:06:14.408062 pait-1.0.0a6/pait/app/sanic/_app_helper.py
--rw-r--r--   0        0        0      403 2023-03-21 10:06:14.412062 pait-1.0.0a6/pait/app/sanic/_attribute.py
--rw-r--r--   0        0        0      319 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/sanic/_exception.py
--rw-r--r--   0        0        0     3902 2023-05-19 10:54:00.027470 pait-1.0.0a6/pait/app/sanic/_load_app.py
--rw-r--r--   0        0        0      374 2023-05-09 02:55:20.341357 pait-1.0.0a6/pait/app/sanic/_pait.py
--rw-r--r--   0        0        0     1749 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/sanic/_simple_route.py
--rw-r--r--   0        0        0     2172 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/sanic/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a6/pait/app/sanic/adapter/__init__.py
--rw-r--r--   0        0        0     2067 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/sanic/adapter/request.py
--rw-r--r--   0        0        0     1102 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/sanic/adapter/response.py
--rw-r--r--   0        0        0      716 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/sanic/plugin/__init__.py
--rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/sanic/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0      138 2023-05-23 09:37:36.508526 pait-1.0.0a6/pait/app/sanic/plugin/cache_response.py
--rw-r--r--   0        0        0      934 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/sanic/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1432 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/sanic/plugin/mock_response.py
--rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/sanic/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a6/pait/app/sanic/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/sanic/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/sanic/security/http.py
--rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/sanic/security/oauth2.py
--rw-r--r--   0        0        0      321 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/sanic/security/util.py
--rw-r--r--   0        0        0      336 2023-07-03 05:59:15.586022 pait-1.0.0a6/pait/app/starlette/__init__.py
--rw-r--r--   0        0        0      651 2023-03-21 10:06:14.412062 pait-1.0.0a6/pait/app/starlette/_app_helper.py
--rw-r--r--   0        0        0      430 2023-03-21 10:06:14.412062 pait-1.0.0a6/pait/app/starlette/_attribute.py
--rw-r--r--   0        0        0      319 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/starlette/_exception.py
--rw-r--r--   0        0        0     3877 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/starlette/_load_app.py
--rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a6/pait/app/starlette/_pait.py
--rw-r--r--   0        0        0      996 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/starlette/_simple_route.py
--rw-r--r--   0        0        0     2021 2023-06-02 02:45:03.967509 pait-1.0.0a6/pait/app/starlette/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a6/pait/app/starlette/adapter/__init__.py
--rw-r--r--   0        0        0     2718 2023-04-08 08:28:39.674480 pait-1.0.0a6/pait/app/starlette/adapter/request.py
--rw-r--r--   0        0        0     1065 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/starlette/adapter/response.py
--rw-r--r--   0        0        0      800 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/starlette/plugin/__init__.py
--rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/starlette/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0      138 2023-05-23 09:37:36.560526 pait-1.0.0a6/pait/app/starlette/plugin/cache_response.py
--rw-r--r--   0        0        0      785 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/starlette/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1626 2023-02-16 07:49:53.639890 pait-1.0.0a6/pait/app/starlette/plugin/mock_response.py
--rw-r--r--   0        0        0      702 2023-02-07 03:41:51.356781 pait-1.0.0a6/pait/app/starlette/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a6/pait/app/starlette/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/starlette/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/starlette/security/http.py
--rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/starlette/security/oauth2.py
--rw-r--r--   0        0        0      325 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/starlette/security/util.py
--rw-r--r--   0        0        0      334 2023-07-03 05:59:15.586022 pait-1.0.0a6/pait/app/tornado/__init__.py
--rw-r--r--   0        0        0     1002 2023-03-21 10:06:14.412062 pait-1.0.0a6/pait/app/tornado/_app_helper.py
--rw-r--r--   0        0        0      424 2023-03-21 10:06:14.412062 pait-1.0.0a6/pait/app/tornado/_attribute.py
--rw-r--r--   0        0        0      298 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/tornado/_exception.py
--rw-r--r--   0        0        0     2559 2023-05-19 10:54:00.027470 pait-1.0.0a6/pait/app/tornado/_load_app.py
--rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a6/pait/app/tornado/_pait.py
--rw-r--r--   0        0        0     2839 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/tornado/_simple_route.py
--rw-r--r--   0        0        0     4664 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/tornado/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a6/pait/app/tornado/adapter/__init__.py
--rw-r--r--   0        0        0     2244 2023-04-08 08:28:39.674480 pait-1.0.0a6/pait/app/tornado/adapter/request.py
--rw-r--r--   0        0        0     1130 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/tornado/adapter/response.py
--rw-r--r--   0        0        0      792 2023-02-07 03:41:51.360782 pait-1.0.0a6/pait/app/tornado/plugin/__init__.py
--rw-r--r--   0        0        0      574 2023-02-07 03:41:51.360782 pait-1.0.0a6/pait/app/tornado/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0     1411 2023-05-23 09:37:36.612527 pait-1.0.0a6/pait/app/tornado/plugin/cache_response.py
--rw-r--r--   0        0        0     1211 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/tornado/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1237 2023-02-07 03:41:51.360782 pait-1.0.0a6/pait/app/tornado/plugin/mock_response.py
--rw-r--r--   0        0        0     1247 2023-02-07 03:41:51.360782 pait-1.0.0a6/pait/app/tornado/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-02-03 19:54:29.188502 pait-1.0.0a6/pait/app/tornado/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/tornado/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/tornado/security/http.py
--rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a6/pait/app/tornado/security/oauth2.py
--rw-r--r--   0        0        0      323 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/app/tornado/security/util.py
--rw-r--r--   0        0        0    18186 2023-05-23 08:13:27.664682 pait-1.0.0a6/pait/core.py
--rw-r--r--   0        0        0     1645 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/data.py
--rw-r--r--   0        0        0      688 2023-01-11 17:12:40.000000 pait-1.0.0a6/pait/exceptions.py
--rw-r--r--   0        0        0        0 2022-04-03 14:03:33.000000 pait-1.0.0a6/pait/extra/__init__.py
--rw-r--r--   0        0        0     7254 2023-05-19 10:54:00.027470 pait-1.0.0a6/pait/extra/config.py
--rw-r--r--   0        0        0      729 2023-05-21 10:48:05.570392 pait-1.0.0a6/pait/extra/util.py
--rw-r--r--   0        0        0    11023 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/field.py
--rw-r--r--   0        0        0     1261 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/g.py
--rw-r--r--   0        0        0      508 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/grpc/__init__.py
--rw-r--r--   0        0        0     4623 2023-05-21 09:27:09.618683 pait-1.0.0a6/pait/grpc/base_gateway.py
--rw-r--r--   0        0        0      511 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/grpc/desc_template.py
--rw-r--r--   0        0        0    13491 2023-05-23 09:37:37.496529 pait-1.0.0a6/pait/grpc/gateway.py
--rw-r--r--   0        0        0    10338 2023-05-23 08:36:43.286298 pait-1.0.0a6/pait/grpc/inspect.py
--rw-r--r--   0        0        0        0 2023-03-24 09:24:42.276250 pait-1.0.0a6/pait/grpc/plugin/__init__.py
--rw-r--r--   0        0        0       31 2023-03-24 09:24:42.276250 pait-1.0.0a6/pait/grpc/plugin/__main__.py
--rw-r--r--   0        0        0     1762 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/grpc/plugin/code_gen.py
--rw-r--r--   0        0        0     1322 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/grpc/plugin/config.py
--rw-r--r--   0        0        0    20548 2023-05-10 15:19:11.480786 pait-1.0.0a6/pait/grpc/plugin/field_desc_proto_to_route_code.py
--rw-r--r--   0        0        0     3248 2023-05-21 10:37:23.919357 pait-1.0.0a6/pait/grpc/plugin/gateway.py
--rwxr-xr-x   0        0        0      266 2023-03-24 09:24:42.276250 pait-1.0.0a6/pait/grpc/plugin/main.py
--rw-r--r--   0        0        0     1120 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/grpc/plugin/model.py
--rw-r--r--   0        0        0        0 2023-03-24 09:24:42.276250 pait-1.0.0a6/pait/grpc/proto/__init__.py
--rw-r--r--   0        0        0     4193 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/grpc/proto/api.proto
--rw-r--r--   0        0        0     5030 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/grpc/proto/api_pb2.py
--rw-r--r--   0        0        0    11716 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/grpc/proto/api_pb2.pyi
--rw-r--r--   0        0        0      146 2023-04-11 03:13:45.778998 pait-1.0.0a6/pait/grpc/proto/api_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-10 09:17:38.116710 pait-1.0.0a6/pait/grpc/proto/api_pb2_grpc.pyi
--rw-r--r--   0        0        0      436 2023-03-24 09:24:42.276250 pait-1.0.0a6/pait/grpc/types.py
--rw-r--r--   0        0        0     5420 2023-05-23 09:37:37.100528 pait-1.0.0a6/pait/grpc/util.py
--rw-r--r--   0        0        0      559 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/model/__init__.py
--rw-r--r--   0        0        0     3305 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/model/config.py
--rw-r--r--   0        0        0     1606 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/model/context.py
--rw-r--r--   0        0        0     9443 2023-05-23 09:37:37.408529 pait-1.0.0a6/pait/model/core.py
--rw-r--r--   0        0        0     6051 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/model/response.py
--rw-r--r--   0        0        0      908 2023-05-28 10:00:37.748027 pait-1.0.0a6/pait/model/status.py
--rw-r--r--   0        0        0     1400 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/model/tag.py
--rw-r--r--   0        0        0     1166 2022-09-26 15:06:36.000000 pait-1.0.0a6/pait/model/template.py
--rw-r--r--   0        0        0        0 2022-01-21 03:47:13.000000 pait-1.0.0a6/pait/openapi/__init__.py
--rw-r--r--   0        0        0     9701 2023-06-18 05:44:11.012681 pait-1.0.0a6/pait/openapi/doc_route.py
--rw-r--r--   0        0        0    12159 2023-05-28 10:02:29.009525 pait-1.0.0a6/pait/openapi/openapi.py
--rw-r--r--   0        0        0      105 2023-02-07 03:41:51.360782 pait-1.0.0a6/pait/param_handle/__init__.py
--rw-r--r--   0        0        0     6319 2023-06-12 07:13:53.829457 pait-1.0.0a6/pait/param_handle/_async.py
--rw-r--r--   0        0        0     5262 2023-06-12 07:13:53.829457 pait-1.0.0a6/pait/param_handle/_sync.py
--rw-r--r--   0        0        0    12598 2023-06-12 07:13:53.829457 pait-1.0.0a6/pait/param_handle/base.py
--rw-r--r--   0        0        0       87 2023-02-07 03:41:51.360782 pait-1.0.0a6/pait/plugin/__init__.py
--rw-r--r--   0        0        0     2298 2023-02-07 03:41:51.360782 pait-1.0.0a6/pait/plugin/at_most_one_of.py
--rw-r--r--   0        0        0     2599 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0     3592 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/plugin/base.py
--rw-r--r--   0        0        0     8867 2023-05-23 09:45:50.401974 pait-1.0.0a6/pait/plugin/cache_response.py
--rw-r--r--   0        0        0     2228 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/plugin/check_json_resp.py
--rw-r--r--   0        0        0     5145 2023-05-23 09:37:37.272529 pait-1.0.0a6/pait/plugin/mock_response.py
--rw-r--r--   0        0        0     3312 2023-02-07 03:41:51.360782 pait-1.0.0a6/pait/plugin/required.py
--rw-r--r--   0        0        0     2109 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/plugin/unified_response.py
--rw-r--r--   0        0        0     1283 2023-06-12 07:13:53.829457 pait-1.0.0a6/pait/types.py
--rw-r--r--   0        0        0      524 2023-02-14 09:33:41.434168 pait-1.0.0a6/pait/util/__init__.py
--rw-r--r--   0        0        0     2185 2023-06-12 07:13:53.829457 pait-1.0.0a6/pait/util/_func_sig.py
--rw-r--r--   0        0        0     2607 2023-01-12 10:30:13.000000 pait-1.0.0a6/pait/util/_gen_tip.py
--rw-r--r--   0        0        0     1907 2022-04-10 08:10:06.000000 pait-1.0.0a6/pait/util/_lazy_property.py
--rw-r--r--   0        0        0      957 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/util/_pydantic_util.py
--rw-r--r--   0        0        0     4211 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/util/_types.py
--rw-r--r--   0        0        0    13534 2023-05-30 08:34:59.099755 pait-1.0.0a6/pait/util/_util.py
--rw-r--r--   0        0        0      869 2023-05-10 15:19:11.484786 pait-1.0.0a6/pait/util/encoder.py
--rw-r--r--   0        0        0     3527 2023-07-03 06:00:19.855163 pait-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     7405 1970-01-01 00:00:00.000000 pait-1.0.0a6/setup.py
--rw-r--r--   0        0        0     6801 1970-01-01 00:00:00.000000 pait-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 pait-1.0.0a7/LICENSE
+-rw-r--r--   0        0        0     5244 2023-05-10 15:19:11.464788 pait-1.0.0a7/README.md
+-rw-r--r--   0        0        0       37 2023-05-24 03:47:38.134524 pait-1.0.0a7/pait/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-07 10:53:38.002595 pait-1.0.0a7/pait/__version__.py
+-rw-r--r--   0        0        0      216 2023-07-03 05:59:15.586022 pait-1.0.0a7/pait/app/__init__.py
+-rw-r--r--   0        0        0     5528 2023-05-23 09:37:37.084528 pait-1.0.0a7/pait/app/any/__init__.py
+-rw-r--r--   0        0        0      535 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/any/plugin/__init__.py
+-rw-r--r--   0        0        0      460 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/any/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      425 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/any/plugin/cache_response.py
+-rw-r--r--   0        0        0      405 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/any/plugin/check_json_resp.py
+-rw-r--r--   0        0        0      373 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/any/plugin/mock_response.py
+-rw-r--r--   0        0        0      424 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/any/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-17 11:47:59.744123 pait-1.0.0a7/pait/app/any/security/__init__.py
+-rw-r--r--   0        0        0      342 2023-02-08 03:58:49.610123 pait-1.0.0a7/pait/app/any/security/api_key.py
+-rw-r--r--   0        0        0      653 2023-02-10 15:24:31.281635 pait-1.0.0a7/pait/app/any/security/http.py
+-rw-r--r--   0        0        0      660 2023-02-08 03:43:07.655826 pait-1.0.0a7/pait/app/any/security/oauth2.py
+-rw-r--r--   0        0        0     1510 2023-07-03 16:22:23.109261 pait-1.0.0a7/pait/app/any/util.py
+-rw-r--r--   0        0        0      562 2023-02-15 10:04:32.538762 pait-1.0.0a7/pait/app/auto_load_app.py
+-rw-r--r--   0        0        0      121 2023-01-09 15:13:50.000000 pait-1.0.0a7/pait/app/base/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a7/pait/app/base/adapter/__init__.py
+-rw-r--r--   0        0        0     2427 2023-04-08 08:28:39.674480 pait-1.0.0a7/pait/app/base/adapter/request.py
+-rw-r--r--   0        0        0     1806 2023-05-10 15:19:11.476786 pait-1.0.0a7/pait/app/base/app_helper.py
+-rw-r--r--   0        0        0        0 2023-02-10 10:23:08.836059 pait-1.0.0a7/pait/app/base/security/__init__.py
+-rw-r--r--   0        0        0     1778 2023-07-07 10:50:44.765821 pait-1.0.0a7/pait/app/base/security/api_key.py
+-rw-r--r--   0        0        0     1303 2023-07-07 10:43:33.927811 pait-1.0.0a7/pait/app/base/security/base.py
+-rw-r--r--   0        0        0     7453 2023-07-07 10:43:33.915811 pait-1.0.0a7/pait/app/base/security/http.py
+-rw-r--r--   0        0        0     5121 2023-07-07 10:48:48.593293 pait-1.0.0a7/pait/app/base/security/oauth2.py
+-rw-r--r--   0        0        0      794 2023-05-16 11:28:00.165083 pait-1.0.0a7/pait/app/base/security/util.py
+-rw-r--r--   0        0        0      649 2023-05-10 15:19:11.476786 pait-1.0.0a7/pait/app/base/simple_route.py
+-rw-r--r--   0        0        0    14223 2023-07-05 10:09:10.863486 pait-1.0.0a7/pait/app/base/test_helper.py
+-rw-r--r--   0        0        0      332 2023-07-03 05:59:15.586022 pait-1.0.0a7/pait/app/flask/__init__.py
+-rw-r--r--   0        0        0      719 2023-03-21 10:06:14.408062 pait-1.0.0a7/pait/app/flask/_app_helper.py
+-rw-r--r--   0        0        0      394 2023-03-21 10:06:14.408062 pait-1.0.0a7/pait/app/flask/_attribute.py
+-rw-r--r--   0        0        0      792 2023-05-10 15:19:11.476786 pait-1.0.0a7/pait/app/flask/_exception.py
+-rw-r--r--   0        0        0     3495 2023-05-10 15:19:11.476786 pait-1.0.0a7/pait/app/flask/_load_app.py
+-rw-r--r--   0        0        0      269 2022-01-10 09:58:31.000000 pait-1.0.0a7/pait/app/flask/_pait.py
+-rw-r--r--   0        0        0     1775 2023-05-10 15:19:11.476786 pait-1.0.0a7/pait/app/flask/_simple_route.py
+-rw-r--r--   0        0        0     1872 2023-07-04 16:28:15.974810 pait-1.0.0a7/pait/app/flask/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a7/pait/app/flask/adapter/__init__.py
+-rw-r--r--   0        0        0     1689 2023-04-08 08:28:39.674480 pait-1.0.0a7/pait/app/flask/adapter/request.py
+-rw-r--r--   0        0        0     1070 2023-05-10 15:19:11.476786 pait-1.0.0a7/pait/app/flask/adapter/response.py
+-rw-r--r--   0        0        0      784 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/flask/plugin/__init__.py
+-rw-r--r--   0        0        0      117 2023-02-06 11:24:42.996357 pait-1.0.0a7/pait/app/flask/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      138 2023-05-23 09:37:36.512526 pait-1.0.0a7/pait/app/flask/plugin/cache_response.py
+-rw-r--r--   0        0        0      556 2023-05-10 15:19:11.476786 pait-1.0.0a7/pait/app/flask/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1208 2023-05-23 03:11:41.942069 pait-1.0.0a7/pait/app/flask/plugin/mock_response.py
+-rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/flask/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a7/pait/app/flask/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/flask/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/flask/security/http.py
+-rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/flask/security/oauth2.py
+-rw-r--r--   0        0        0      321 2023-05-10 15:19:11.476786 pait-1.0.0a7/pait/app/flask/security/util.py
+-rw-r--r--   0        0        0      332 2023-07-03 05:59:15.586022 pait-1.0.0a7/pait/app/sanic/__init__.py
+-rw-r--r--   0        0        0      938 2023-03-21 10:06:14.408062 pait-1.0.0a7/pait/app/sanic/_app_helper.py
+-rw-r--r--   0        0        0      403 2023-03-21 10:06:14.412062 pait-1.0.0a7/pait/app/sanic/_attribute.py
+-rw-r--r--   0        0        0      319 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/sanic/_exception.py
+-rw-r--r--   0        0        0     3902 2023-05-19 10:54:00.027470 pait-1.0.0a7/pait/app/sanic/_load_app.py
+-rw-r--r--   0        0        0      374 2023-05-09 02:55:20.341357 pait-1.0.0a7/pait/app/sanic/_pait.py
+-rw-r--r--   0        0        0     1749 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/sanic/_simple_route.py
+-rw-r--r--   0        0        0     2144 2023-07-04 16:28:15.982810 pait-1.0.0a7/pait/app/sanic/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a7/pait/app/sanic/adapter/__init__.py
+-rw-r--r--   0        0        0     2067 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/sanic/adapter/request.py
+-rw-r--r--   0        0        0     1102 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/sanic/adapter/response.py
+-rw-r--r--   0        0        0      716 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/sanic/plugin/__init__.py
+-rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/sanic/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      138 2023-05-23 09:37:36.508526 pait-1.0.0a7/pait/app/sanic/plugin/cache_response.py
+-rw-r--r--   0        0        0      934 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/sanic/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1432 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/sanic/plugin/mock_response.py
+-rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/sanic/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a7/pait/app/sanic/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/sanic/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/sanic/security/http.py
+-rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/sanic/security/oauth2.py
+-rw-r--r--   0        0        0      321 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/sanic/security/util.py
+-rw-r--r--   0        0        0      336 2023-07-03 05:59:15.586022 pait-1.0.0a7/pait/app/starlette/__init__.py
+-rw-r--r--   0        0        0      651 2023-03-21 10:06:14.412062 pait-1.0.0a7/pait/app/starlette/_app_helper.py
+-rw-r--r--   0        0        0      430 2023-03-21 10:06:14.412062 pait-1.0.0a7/pait/app/starlette/_attribute.py
+-rw-r--r--   0        0        0      319 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/starlette/_exception.py
+-rw-r--r--   0        0        0     3877 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/starlette/_load_app.py
+-rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a7/pait/app/starlette/_pait.py
+-rw-r--r--   0        0        0      996 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/starlette/_simple_route.py
+-rw-r--r--   0        0        0     1993 2023-07-04 16:28:15.954809 pait-1.0.0a7/pait/app/starlette/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a7/pait/app/starlette/adapter/__init__.py
+-rw-r--r--   0        0        0     2718 2023-04-08 08:28:39.674480 pait-1.0.0a7/pait/app/starlette/adapter/request.py
+-rw-r--r--   0        0        0     1065 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/starlette/adapter/response.py
+-rw-r--r--   0        0        0      800 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/starlette/plugin/__init__.py
+-rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/starlette/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      138 2023-05-23 09:37:36.560526 pait-1.0.0a7/pait/app/starlette/plugin/cache_response.py
+-rw-r--r--   0        0        0      785 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/starlette/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1626 2023-02-16 07:49:53.639890 pait-1.0.0a7/pait/app/starlette/plugin/mock_response.py
+-rw-r--r--   0        0        0      702 2023-02-07 03:41:51.356781 pait-1.0.0a7/pait/app/starlette/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a7/pait/app/starlette/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/starlette/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/starlette/security/http.py
+-rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/starlette/security/oauth2.py
+-rw-r--r--   0        0        0      325 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/starlette/security/util.py
+-rw-r--r--   0        0        0      334 2023-07-03 05:59:15.586022 pait-1.0.0a7/pait/app/tornado/__init__.py
+-rw-r--r--   0        0        0     1002 2023-03-21 10:06:14.412062 pait-1.0.0a7/pait/app/tornado/_app_helper.py
+-rw-r--r--   0        0        0      424 2023-03-21 10:06:14.412062 pait-1.0.0a7/pait/app/tornado/_attribute.py
+-rw-r--r--   0        0        0      298 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/tornado/_exception.py
+-rw-r--r--   0        0        0     2559 2023-05-19 10:54:00.027470 pait-1.0.0a7/pait/app/tornado/_load_app.py
+-rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a7/pait/app/tornado/_pait.py
+-rw-r--r--   0        0        0     2839 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/tornado/_simple_route.py
+-rw-r--r--   0        0        0     4636 2023-07-04 16:28:15.966810 pait-1.0.0a7/pait/app/tornado/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a7/pait/app/tornado/adapter/__init__.py
+-rw-r--r--   0        0        0     2244 2023-04-08 08:28:39.674480 pait-1.0.0a7/pait/app/tornado/adapter/request.py
+-rw-r--r--   0        0        0     1130 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/tornado/adapter/response.py
+-rw-r--r--   0        0        0      792 2023-02-07 03:41:51.360782 pait-1.0.0a7/pait/app/tornado/plugin/__init__.py
+-rw-r--r--   0        0        0      574 2023-02-07 03:41:51.360782 pait-1.0.0a7/pait/app/tornado/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0     1411 2023-05-23 09:37:36.612527 pait-1.0.0a7/pait/app/tornado/plugin/cache_response.py
+-rw-r--r--   0        0        0     1211 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/tornado/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1237 2023-02-07 03:41:51.360782 pait-1.0.0a7/pait/app/tornado/plugin/mock_response.py
+-rw-r--r--   0        0        0     1247 2023-02-07 03:41:51.360782 pait-1.0.0a7/pait/app/tornado/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-02-03 19:54:29.188502 pait-1.0.0a7/pait/app/tornado/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/tornado/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/tornado/security/http.py
+-rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a7/pait/app/tornado/security/oauth2.py
+-rw-r--r--   0        0        0      323 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/app/tornado/security/util.py
+-rw-r--r--   0        0        0    18186 2023-05-23 08:13:27.664682 pait-1.0.0a7/pait/core.py
+-rw-r--r--   0        0        0     1645 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/data.py
+-rw-r--r--   0        0        0      688 2023-01-11 17:12:40.000000 pait-1.0.0a7/pait/exceptions.py
+-rw-r--r--   0        0        0        0 2022-04-03 14:03:33.000000 pait-1.0.0a7/pait/extra/__init__.py
+-rw-r--r--   0        0        0     7254 2023-05-19 10:54:00.027470 pait-1.0.0a7/pait/extra/config.py
+-rw-r--r--   0        0        0      996 2023-07-04 06:31:08.417272 pait-1.0.0a7/pait/extra/util.py
+-rw-r--r--   0        0        0    11023 2023-07-07 10:37:02.645782 pait-1.0.0a7/pait/field.py
+-rw-r--r--   0        0        0     1261 2023-05-10 15:19:11.480786 pait-1.0.0a7/pait/g.py
+-rw-r--r--   0        0        0      559 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/model/__init__.py
+-rw-r--r--   0        0        0     3305 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/model/config.py
+-rw-r--r--   0        0        0     1606 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/model/context.py
+-rw-r--r--   0        0        0     9443 2023-05-23 09:37:37.408529 pait-1.0.0a7/pait/model/core.py
+-rw-r--r--   0        0        0     6051 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/model/response.py
+-rw-r--r--   0        0        0      908 2023-05-28 10:00:37.748027 pait-1.0.0a7/pait/model/status.py
+-rw-r--r--   0        0        0     1400 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/model/tag.py
+-rw-r--r--   0        0        0     1166 2022-09-26 15:06:36.000000 pait-1.0.0a7/pait/model/template.py
+-rw-r--r--   0        0        0        0 2022-01-21 03:47:13.000000 pait-1.0.0a7/pait/openapi/__init__.py
+-rw-r--r--   0        0        0     9701 2023-06-18 05:44:11.012681 pait-1.0.0a7/pait/openapi/doc_route.py
+-rw-r--r--   0        0        0    12159 2023-05-28 10:02:29.009525 pait-1.0.0a7/pait/openapi/openapi.py
+-rw-r--r--   0        0        0      105 2023-02-07 03:41:51.360782 pait-1.0.0a7/pait/param_handle/__init__.py
+-rw-r--r--   0        0        0     6319 2023-06-12 07:13:53.829457 pait-1.0.0a7/pait/param_handle/_async.py
+-rw-r--r--   0        0        0     5262 2023-06-12 07:13:53.829457 pait-1.0.0a7/pait/param_handle/_sync.py
+-rw-r--r--   0        0        0    12598 2023-06-12 07:13:53.829457 pait-1.0.0a7/pait/param_handle/base.py
+-rw-r--r--   0        0        0       87 2023-02-07 03:41:51.360782 pait-1.0.0a7/pait/plugin/__init__.py
+-rw-r--r--   0        0        0     2298 2023-02-07 03:41:51.360782 pait-1.0.0a7/pait/plugin/at_most_one_of.py
+-rw-r--r--   0        0        0     2599 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0     3592 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/plugin/base.py
+-rw-r--r--   0        0        0     8867 2023-05-23 09:45:50.401974 pait-1.0.0a7/pait/plugin/cache_response.py
+-rw-r--r--   0        0        0     2228 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     5145 2023-05-23 09:37:37.272529 pait-1.0.0a7/pait/plugin/mock_response.py
+-rw-r--r--   0        0        0     3312 2023-02-07 03:41:51.360782 pait-1.0.0a7/pait/plugin/required.py
+-rw-r--r--   0        0        0     2109 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/plugin/unified_response.py
+-rw-r--r--   0        0        0     1407 2023-07-07 10:36:04.885454 pait-1.0.0a7/pait/types.py
+-rw-r--r--   0        0        0      524 2023-02-14 09:33:41.434168 pait-1.0.0a7/pait/util/__init__.py
+-rw-r--r--   0        0        0     2185 2023-06-12 07:13:53.829457 pait-1.0.0a7/pait/util/_func_sig.py
+-rw-r--r--   0        0        0     2607 2023-01-12 10:30:13.000000 pait-1.0.0a7/pait/util/_gen_tip.py
+-rw-r--r--   0        0        0     1907 2022-04-10 08:10:06.000000 pait-1.0.0a7/pait/util/_lazy_property.py
+-rw-r--r--   0        0        0      957 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/util/_pydantic_util.py
+-rw-r--r--   0        0        0     4211 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/util/_types.py
+-rw-r--r--   0        0        0    13534 2023-05-30 08:34:59.099755 pait-1.0.0a7/pait/util/_util.py
+-rw-r--r--   0        0        0      869 2023-05-10 15:19:11.484786 pait-1.0.0a7/pait/util/encoder.py
+-rw-r--r--   0        0        0     3140 2023-07-07 10:53:37.998595 pait-1.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0     7093 1970-01-01 00:00:00.000000 pait-1.0.0a7/setup.py
+-rw-r--r--   0        0        0     6619 1970-01-01 00:00:00.000000 pait-1.0.0a7/PKG-INFO
```

### Comparing `pait-1.0.0a6/LICENSE` & `pait-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/README.md` & `pait-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/any/__init__.py` & `pait-1.0.0a7/pait/app/any/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/any/plugin/__init__.py` & `pait-1.0.0a7/pait/app/any/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/any/security/http.py` & `pait-1.0.0a7/pait/app/any/security/http.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/any/security/oauth2.py` & `pait-1.0.0a7/pait/app/any/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/any/util.py` & `pait-1.0.0a7/pait/app/any/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,18 @@
         raise NotImplementedError(f"Pait not support app name:{app_name}, please check app:{app}")
 
 
 def import_func_from_app(fun_name: str, app: Any = None, module_name: str = "") -> Callable:
     from pait.app.auto_load_app import auto_load_app_class
 
     if app:
+        # support werkzeug LocalProxy
+        _get_current_object = getattr(app, "_get_current_object", None)
+        if _get_current_object:
+            app = _get_current_object()
         app_name: str = sniffing(app)
     else:
         app_name = auto_load_app_class().__name__.lower()
     if module_name:
         return getattr(import_module(f"pait.app.{app_name}.{module_name}"), fun_name)
     else:
         return getattr(import_module(f"pait.app.{app_name}"), fun_name)
```

### Comparing `pait-1.0.0a6/pait/app/auto_load_app.py` & `pait-1.0.0a7/pait/app/auto_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/base/adapter/request.py` & `pait-1.0.0a7/pait/app/base/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/base/app_helper.py` & `pait-1.0.0a7/pait/app/base/app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/base/security/api_key.py` & `pait-1.0.0a7/pait/app/base/security/api_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,11 +33,14 @@
         self.security_name = security_name or self.__class__.__name__
 
         def pait_handler(authorization: str = field) -> str:
             return self.authorization_handler(authorization)
 
         self.set_pait_handler(pait_handler)
 
+    def __call__(self, authorization: str = Query.i()) -> str:
+        raise RuntimeError("should not call this method")  # pragma: no cover
+
     def authorization_handler(self, authorization: str) -> str:
         if self.verify_api_key_callable and not self.verify_api_key_callable(authorization):
             raise self.not_authenticated_exc
         return authorization
```

### Comparing `pait-1.0.0a6/pait/app/base/security/http.py` & `pait-1.0.0a7/pait/app/base/security/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,17 @@
         set_and_check_field(self.header_field, "Authorization", self.not_authorization_exc if is_raise else None)
 
         def pait_handler(authorization: str = self.header_field) -> Optional[HTTPBasicCredentials]:
             return self.authorization_handler(authorization)
 
         self.set_pait_handler(pait_handler)
 
+    def __call__(self, authorization: str = Header.i()) -> Optional[HTTPBasicCredentials]:
+        raise RuntimeError("should not call this method")  # pragma: no cover
+
     def authorization_handler(self, authorization: str) -> Optional[HTTPBasicCredentials]:
         scheme, param = get_authorization_scheme_param(authorization)
         if not authorization or (scheme.lower() != "basic"):
             if self.is_raise:
                 raise self.not_authorization_exc
             else:
                 return None
@@ -102,14 +105,17 @@
         set_and_check_field(self.header_field, "Authorization", self.not_authenticated_exc if is_raise else None)
 
         def pait_handler(authorization: str = self.header_field) -> Optional[str]:
             return self.authorization_handler(authorization)
 
         self.set_pait_handler(pait_handler)
 
+    def __call__(self, authorization: str = Header.i()) -> Optional[str]:
+        raise RuntimeError("should not call this method")  # pragma: no cover
+
     def authorization_handler(self, authorization: str) -> Optional[str]:
         scheme, credentials = get_authorization_scheme_param(authorization)
         if (not (authorization and scheme and credentials)) or (scheme.lower() != self.model.scheme):
             if self.is_raise:
                 raise self.not_authenticated_exc
             else:
                 return None
```

### Comparing `pait-1.0.0a6/pait/app/base/security/oauth2.py` & `pait-1.0.0a7/pait/app/base/security/oauth2.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,17 @@
         self.security_name = security.security_name
 
         def pait_handler(authorization: str = security.header_field) -> str:
             return self.authorization_handler(authorization)
 
         self.set_pait_handler(pait_handler)
 
+    def __call__(self, authorization: str = Header.i()) -> str:
+        raise RuntimeError("should not call this method")  # pragma: no cover
+
     @property
     def model(self) -> SecurityModelType:
         if self.use_scopes:
             return UserScopesOauth2SecurityModel(
                 use_scopes=self.use_scopes, model=self.security.model, flows=self.security.model.flows
             )
         return self.security.model
```

### Comparing `pait-1.0.0a6/pait/app/base/security/util.py` & `pait-1.0.0a7/pait/app/base/security/util.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/base/simple_route.py` & `pait-1.0.0a7/pait/app/base/simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/base/test_helper.py` & `pait-1.0.0a7/pait/app/base/test_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pait.model import response
 from pait.util import gen_example_dict_from_schema, gen_example_value_from_python, get_pait_response_model
 
 if TYPE_CHECKING:
     from pait.model import PaitCoreModel
 
 RESP_T = TypeVar("RESP_T")
+_error_separator = "\n" + ">" * 20 + "\n"
 
 
 class CheckResponseException(Exception):
     def __init__(
         self,
         status_code: Optional[int] = None,
         media_type: Optional[str] = None,
@@ -45,15 +46,14 @@
         cookie_dict: Optional[dict] = None,
         file_dict: Optional[dict] = None,
         form_dict: Optional[dict] = None,
         header_dict: Optional[dict] = None,
         path_dict: Optional[dict] = None,
         query_dict: Optional[dict] = None,
         strict_inspection_check_json_content: bool = True,
-        find_response_model: bool = False,
         enable_assert_response: bool = True,
         target_pait_response_class: Optional[Type["response.BaseResponseModel"]] = None,
     ):
         """
         :param client:  test client
         :param func:  route handle decorated by pait
         :param pait_dict:  pait core data
@@ -105,15 +105,14 @@
 
         # add query path by path
         if self.query_dict:
             self.path = self.path + "?" + urlencode(self.query_dict, True)
         if not self.path.startswith("/"):
             self.path = "/" + self.path
 
-        self.find_response_model: bool = find_response_model
         self.target_pait_response_class: Optional[Type["response.BaseResponseModel"]] = target_pait_response_class
         self._app_init_field()
 
     def _app_init_field(self) -> None:
         """init request param by application framework"""
         raise NotImplementedError()
 
@@ -173,25 +172,25 @@
                     return False
                 return True
             else:
                 return True
         except KeyError:
             raise RuntimeError(f"Can not found key from model, key:{' -> '.join(parent_key_list or '')}")
 
-    def _assert_response(self, resp: RESP_T) -> None:
+    def _assert_response(self, resp: RESP_T) -> Optional[Exception]:
         """Whether the structure of the check response is correct"""
         if not self.pait_core_model.response_model_list:
-            return
+            return None
 
         real_response_model: Optional[Type[response.BaseResponseModel]] = None
         max_quick_ratio: float = 0.0
         model_check_msg_dict: Dict[Type[response.BaseResponseModel], List[str]] = {}
         response_model_list: List[Type[response.BaseResponseModel]] = (
             self.pait_core_model.response_model_list
-            if not self.find_response_model
+            if not self.target_pait_response_class
             else [
                 get_pait_response_model(
                     self.pait_core_model.response_model_list,
                     target_pait_response_class=self.target_pait_response_class,
                 )
             ]
         )
@@ -225,15 +224,15 @@
                 response_data_model: Type[BaseModel] = response_model.response_data
                 resp_dict: Optional[dict] = None
                 try:
                     resp_dict = self._get_json(resp)
                 except Exception:
                     pass
 
-                if not resp_dict:
+                if not resp_dict and not isinstance(resp_dict, dict):
                     continue
                 response_data_default_dict: dict = gen_example_dict_from_schema(response_data_model.schema())
                 ratio: float = difflib.SequenceMatcher(
                     None,
                     str(gen_example_value_from_python(resp_dict)),
                     str(response_data_default_dict),
                 ).quick_ratio()
@@ -242,59 +241,63 @@
                     real_response_model = response_model
                 try:
                     response_data_model(**resp_dict)
                     # like Basemodel.config.extra = forbid
                     if self.strict_inspection_check_json_content and not self._check_diff_resp_dict(
                         resp_dict, response_data_default_dict
                     ):
-                        error_msg_list.append("check json structure error")
+                        differ = difflib.Differ()
+                        diff_iterator = differ.compare(str(response_data_default_dict), str(resp_dict))
+                        diff_content = "\n".join(diff_iterator)
+                        error_msg_list.append(f"check json structure error, \n{diff_content}")
                 except (ValidationError, RuntimeError) as e:
                     error_msg_list.append(f"check json content error, exec: {e}")
 
             elif issubclass(response_model, response.HtmlResponseModel) or issubclass(
                 response_model, response.TextResponseModel
             ):
                 real_response_model = response_model
                 if not isinstance(self._get_text(resp), type(response_model.response_data)):
                     error_msg_list.append("check text content type error")  # pragma: no cover
             elif issubclass(response_model, response.FileResponseModel):
                 real_response_model = response_model
                 if not isinstance(self._get_bytes(resp), type(response_model.response_data)):
                     error_msg_list.append("check bytes content type error")  # pragma: no cover
             else:
-                raise TypeError(f"Pait not support response model:{response_model}")
+                return TypeError(f"Pait not support response model:{response_model}")
             if not error_msg_list:
-                return
+                return None
             else:
                 model_check_msg_dict[response_model] = error_msg_list
         if real_response_model in model_check_msg_dict:
             error_str: str = "\n    ".join(model_check_msg_dict[real_response_model])
-            raise CheckResponseException(
+            return CheckResponseException(
                 status_code=self._get_status_code(resp),
                 media_type=self._get_content_type(resp),
                 headers=self._get_headers(resp),
                 resp=resp,
                 func=self.func,
                 message=(
-                    " maybe error result: \n" f"    {error_str}\n\n" f" by response model:{real_response_model}\n"
+                    f"maybe error result: {_error_separator}{error_str}\n"
+                    f"{_error_separator}by response model:{real_response_model}\n"
                 ),
             )
 
         error_str = ""
         for k, v in model_check_msg_dict.items():
             error_str += str(k) + ":\n" + "    \n".join(v)
-        raise CheckResponseException(
+        return CheckResponseException(
             status_code=self._get_status_code(resp),
             media_type=self._get_content_type(resp),
             headers=self._get_headers(resp),
             resp=resp,
             func=self.func,
             message=(
-                f"response error result:{error_str} \n"
-                f"by response model list:{self.pait_core_model.response_model_list}. \n"
+                f"response error result: {_error_separator}{error_str} \n"
+                f"{_error_separator}by response model list:{self.pait_core_model.response_model_list}.\n"
             ),
         )
 
     def _replace_path(self, path_str: str) -> Optional[str]:
         raise NotImplementedError()
 
     def _real_request(self, method: str) -> RESP_T:
@@ -309,15 +312,17 @@
                 method = self.pait_core_model.method_list[0]
             else:
                 raise RuntimeError(
                     f"Pait Can not auto select method, please choice method in {self.pait_core_model.method_list}"
                 )
         resp: RESP_T = self._real_request(method)
         if self.pait_core_model.response_model_list and self.enable_assert_response:
-            self._assert_response(resp)
+            exc = self._assert_response(resp)
+            if exc:
+                raise exc
         return resp
 
     def json(self, method: Optional[str] = None) -> dict:
         return self._get_json(self.request(method))
 
     def text(self, method: Optional[str] = None) -> str:
         return self._get_text(self.request(method))
```

### Comparing `pait-1.0.0a6/pait/app/flask/_app_helper.py` & `pait-1.0.0a7/pait/app/flask/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/flask/_exception.py` & `pait-1.0.0a7/pait/app/flask/_exception.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/flask/_load_app.py` & `pait-1.0.0a7/pait/app/flask/_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/flask/_simple_route.py` & `pait-1.0.0a7/pait/app/flask/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/flask/_test_helper.py` & `pait-1.0.0a7/pait/app/flask/_test_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,8 +60,8 @@
     def _real_request(self, method: str) -> Response:
         return self.client.open(
             self.path, data=self.form_dict, json=self.body_dict, headers=self.header_dict, method=method
         )
 
 
 class FlaskTestHelper(TestHelper):
-    """Will remove on version 1.0"""
+    pass
```

### Comparing `pait-1.0.0a6/pait/app/flask/adapter/request.py` & `pait-1.0.0a7/pait/app/flask/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/flask/adapter/response.py` & `pait-1.0.0a7/pait/app/flask/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/flask/plugin/__init__.py` & `pait-1.0.0a7/pait/app/flask/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/flask/plugin/check_json_resp.py` & `pait-1.0.0a7/pait/app/flask/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/flask/plugin/mock_response.py` & `pait-1.0.0a7/pait/app/flask/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/flask/plugin/unified_response.py` & `pait-1.0.0a7/pait/app/flask/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/flask/security/oauth2.py` & `pait-1.0.0a7/pait/app/flask/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/_app_helper.py` & `pait-1.0.0a7/pait/app/sanic/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/_load_app.py` & `pait-1.0.0a7/pait/app/sanic/_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/_simple_route.py` & `pait-1.0.0a7/pait/app/sanic/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/_test_helper.py` & `pait-1.0.0a7/pait/app/sanic/_test_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,8 +65,8 @@
                 headers=self.header_dict,
                 files=self.file_dict,
             )
         return resp
 
 
 class SanicTestHelper(TestHelper):
-    """Will remove on version 1.0"""
+    pass
```

### Comparing `pait-1.0.0a6/pait/app/sanic/adapter/request.py` & `pait-1.0.0a7/pait/app/sanic/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/adapter/response.py` & `pait-1.0.0a7/pait/app/sanic/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/plugin/__init__.py` & `pait-1.0.0a7/pait/app/sanic/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/plugin/auto_complete_json_resp.py` & `pait-1.0.0a7/pait/app/sanic/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/plugin/check_json_resp.py` & `pait-1.0.0a7/pait/app/sanic/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/plugin/mock_response.py` & `pait-1.0.0a7/pait/app/sanic/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/plugin/unified_response.py` & `pait-1.0.0a7/pait/app/sanic/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/sanic/security/oauth2.py` & `pait-1.0.0a7/pait/app/sanic/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/_app_helper.py` & `pait-1.0.0a7/pait/app/starlette/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/_load_app.py` & `pait-1.0.0a7/pait/app/starlette/_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/_simple_route.py` & `pait-1.0.0a7/pait/app/starlette/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/_test_helper.py` & `pait-1.0.0a7/pait/app/starlette/_test_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,8 +62,8 @@
             headers=self.header_dict,
             files=self.file_dict,
         )
         return resp
 
 
 class StarletteTestHelper(TestHelper):
-    """Will remove on version 1.0"""
+    pass
```

### Comparing `pait-1.0.0a6/pait/app/starlette/adapter/request.py` & `pait-1.0.0a7/pait/app/starlette/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/adapter/response.py` & `pait-1.0.0a7/pait/app/starlette/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/plugin/__init__.py` & `pait-1.0.0a7/pait/app/starlette/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/plugin/auto_complete_json_resp.py` & `pait-1.0.0a7/pait/app/starlette/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/plugin/check_json_resp.py` & `pait-1.0.0a7/pait/app/starlette/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/plugin/mock_response.py` & `pait-1.0.0a7/pait/app/starlette/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/plugin/unified_response.py` & `pait-1.0.0a7/pait/app/starlette/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/starlette/security/oauth2.py` & `pait-1.0.0a7/pait/app/starlette/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/_app_helper.py` & `pait-1.0.0a7/pait/app/tornado/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/_load_app.py` & `pait-1.0.0a7/pait/app/tornado/_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/_simple_route.py` & `pait-1.0.0a7/pait/app/tornado/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/_test_helper.py` & `pait-1.0.0a7/pait/app/tornado/_test_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,8 +116,8 @@
 
         body.write(("--%s--\r\n" % boundary).encode(encoding="utf-8"))
         content_type: str = "multipart/form-data;boundary=%s" % boundary
         return content_type, body.getvalue()
 
 
 class TornadoTestHelper(TestHelper):
-    """Will remove on version 1.0"""
+    pass
```

### Comparing `pait-1.0.0a6/pait/app/tornado/adapter/request.py` & `pait-1.0.0a7/pait/app/tornado/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/adapter/response.py` & `pait-1.0.0a7/pait/app/tornado/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/plugin/__init__.py` & `pait-1.0.0a7/pait/app/tornado/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/plugin/auto_complete_json_resp.py` & `pait-1.0.0a7/pait/app/tornado/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/plugin/cache_response.py` & `pait-1.0.0a7/pait/app/tornado/plugin/cache_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/plugin/check_json_resp.py` & `pait-1.0.0a7/pait/app/tornado/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/plugin/mock_response.py` & `pait-1.0.0a7/pait/app/tornado/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/plugin/unified_response.py` & `pait-1.0.0a7/pait/app/tornado/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/app/tornado/security/oauth2.py` & `pait-1.0.0a7/pait/app/tornado/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/core.py` & `pait-1.0.0a7/pait/core.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/data.py` & `pait-1.0.0a7/pait/data.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/exceptions.py` & `pait-1.0.0a7/pait/exceptions.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/extra/config.py` & `pait-1.0.0a7/pait/extra/config.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/field.py` & `pait-1.0.0a7/pait/field.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/g.py` & `pait-1.0.0a7/pait/g.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/model/__init__.py` & `pait-1.0.0a7/pait/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/model/config.py` & `pait-1.0.0a7/pait/model/config.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/model/context.py` & `pait-1.0.0a7/pait/model/context.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/model/core.py` & `pait-1.0.0a7/pait/model/core.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/model/response.py` & `pait-1.0.0a7/pait/model/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/model/status.py` & `pait-1.0.0a7/pait/model/status.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/model/tag.py` & `pait-1.0.0a7/pait/model/tag.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/model/template.py` & `pait-1.0.0a7/pait/model/template.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/openapi/doc_route.py` & `pait-1.0.0a7/pait/openapi/doc_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/openapi/openapi.py` & `pait-1.0.0a7/pait/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/param_handle/_async.py` & `pait-1.0.0a7/pait/param_handle/_async.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/param_handle/_sync.py` & `pait-1.0.0a7/pait/param_handle/_sync.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/param_handle/base.py` & `pait-1.0.0a7/pait/param_handle/base.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/plugin/at_most_one_of.py` & `pait-1.0.0a7/pait/plugin/at_most_one_of.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/plugin/auto_complete_json_resp.py` & `pait-1.0.0a7/pait/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/plugin/base.py` & `pait-1.0.0a7/pait/plugin/base.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/plugin/cache_response.py` & `pait-1.0.0a7/pait/plugin/cache_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/plugin/check_json_resp.py` & `pait-1.0.0a7/pait/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/plugin/mock_response.py` & `pait-1.0.0a7/pait/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/plugin/required.py` & `pait-1.0.0a7/pait/plugin/required.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/plugin/unified_response.py` & `pait-1.0.0a7/pait/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/types.py` & `pait-1.0.0a7/pait/types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import Any, Callable, Union
+from typing import Any, Callable, TypeVar, Union
 
 # copy from https://github.com/agronholm/typeguard/blob/master/src/typeguard/__init__.py#L64
 if sys.version_info >= (3, 10):
     from typing import ParamSpec  # pragma: no cover
     from typing import is_typeddict  # pragma: no cover
     from typing import Literal, Protocol
 else:
@@ -23,20 +23,23 @@
     except ImportError:  # pragma: no cover
         pass
 
     def is_typeddict(tp) -> bool:  # type: ignore
         return isinstance(tp, _typed_dict_meta_types)
 
 
+PaitCallTypeT = TypeVar("PaitCallTypeT", covariant=True)
+
+
 class _CallType(Protocol):
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         ...
 
 
-class _PaitCallType(Protocol):
-    def pait_handler(self, *args: Any, **kwargs: Any) -> Any:
+class PaitCallType(Protocol[PaitCallTypeT]):
+    def pait_handler(self, *args: Any, **kwargs: Any) -> PaitCallTypeT:
         ...
 
 
-CallType = Union[Callable, _CallType, _PaitCallType]
+CallType = Union[Callable, _CallType, PaitCallType]
 
-__all__ = ["ParamSpec", "Literal", "is_typeddict", "CallType"]
+__all__ = ["ParamSpec", "Literal", "is_typeddict", "CallType", "PaitCallTypeT", "PaitCallType"]
```

### Comparing `pait-1.0.0a6/pait/util/__init__.py` & `pait-1.0.0a7/pait/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/util/_func_sig.py` & `pait-1.0.0a7/pait/util/_func_sig.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/util/_gen_tip.py` & `pait-1.0.0a7/pait/util/_gen_tip.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/util/_lazy_property.py` & `pait-1.0.0a7/pait/util/_lazy_property.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/util/_pydantic_util.py` & `pait-1.0.0a7/pait/util/_pydantic_util.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/util/_types.py` & `pait-1.0.0a7/pait/util/_types.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/util/_util.py` & `pait-1.0.0a7/pait/util/_util.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pait/util/encoder.py` & `pait-1.0.0a7/pait/util/encoder.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a6/pyproject.toml` & `pait-1.0.0a7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 [tool.poetry]
 name = "pait"
-version = "v1.0.0-alpha.6"
+version = "v1.0.0-alpha.7"
 description = "Pait is a Python api tool. Pait enables your Python web framework to have type checking, parameter type conversion, interface document generation and can display your documents through Redoc or Swagger (power by inspect, pydantic)"
 authors = ["So1n <so1n897046026@gmail.com>"]
 license = "Apache Software License"
 readme = "./README.md"
 repository = "https://github.com/so1n/pait"
 homepage = "https://github.com/so1n/pait"
 
-[tool.poetry.scripts]
-protoc-gen-pait-route = "pait.grpc.plugin.main:main"
-
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = "^1.7.3"
 typing-extensions = "^4.1.1"
-
 any-api = "^0.1.0.4"
-protobuf-to-pydantic = "^0.1.7.3"
 
 redis = { version = "^4.2.2", optional = true }
-jinja2 = {version = ">=2.0.0", optional = true}
 
 [tool.poetry.urls]
 "Source" = "https://github.com/so1n/pait"
 "Tracker" = "https://github.com/so1n/pait/issues"
 "Changelog" = "https://github.com/so1n/pait/blob/master/CHANGELOG.md"
 "Documentation" = "https://so1n.me/pait/"
 
 
 [tool.poetry.extras]
 redis = ["redis"]
-grpc = ["protobuf-to-pydantic", "jinja2"]
-all = ["redis", "protobuf-to-pydantic", "jinja2"]
+all = ["redis"]
 
 [tool.poetry.group.framework.dependencies]
 werkzeug = "1.0.1"
 Flask = "1.1.2"
 jinja2 = "^2.0.0"
 sanic = "21.3.4"
 sanic-testing = "0.3.0"
@@ -92,29 +85,22 @@
 ensure_newline_before_comments = true
 line_length = 120
 
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
 python_executable = ".venv/bin/python"
-exclude = [
-    "^example/example_grpc/python_example_proto_code/example_proto",
-    "^pait/http"
-]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.coverage.run]
 branch = true
 source = ["pait"]
-omit = [
-    "pait/grpc/plugin/*",
-    "pait/grpc/proto/*",
-]
+omit = []
 
 [tool.coverage.report]
 exclude_lines = [
     # Have to re-enable the standard pragma
     "pragma: no cover",
 
     # Don't complain about missing debug-only code:
```

### Comparing `pait-1.0.0a6/setup.py` & `pait-1.0.0a7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,14 @@
  'pait.app.starlette.plugin',
  'pait.app.starlette.security',
  'pait.app.tornado',
  'pait.app.tornado.adapter',
  'pait.app.tornado.plugin',
  'pait.app.tornado.security',
  'pait.extra',
- 'pait.grpc',
- 'pait.grpc.plugin',
- 'pait.grpc.proto',
  'pait.model',
  'pait.openapi',
  'pait.param_handle',
  'pait.plugin',
  'pait.util']
 
 package_data = \
@@ -41,35 +38,28 @@
 
 install_requires = \
 ['any-api>=0.1.0.4,<0.2.0.0',
  'pydantic>=1.7.3,<2.0.0',
  'typing-extensions>=4.1.1,<5.0.0']
 
 extras_require = \
-{':extra == "grpc" or extra == "all"': ['protobuf-to-pydantic>=0.1.7.3,<0.2.0.0'],
- 'all': ['redis>=4.2.2,<5.0.0', 'jinja2>=2.0.0'],
- 'grpc': ['jinja2>=2.0.0'],
- 'redis': ['redis>=4.2.2,<5.0.0']}
-
-entry_points = \
-{'console_scripts': ['protoc-gen-pait-route = pait.grpc.plugin.main:main']}
+{'all': ['redis>=4.2.2,<5.0.0'], 'redis': ['redis>=4.2.2,<5.0.0']}
 
 setup_kwargs = {
     'name': 'pait',
-    'version': '1.0.0a6',
+    'version': '1.0.0a7',
     'description': 'Pait is a Python api tool. Pait enables your Python web framework to have type checking, parameter type conversion, interface document generation and can display your documents through Redoc or Swagger (power by inspect, pydantic)',
     'long_description': '![](https://cdn.jsdelivr.net/gh/so1n/so1n_blog_photo@master/blog_photo/1652600629491%E6%9C%AA%E5%91%BD%E5%90%8D.jpg)\n<p align="center">\n    Pait(π tool) - <em>Python Modern API Tools, easier to use web frameworks/write API routing</em>\n</p>\n<p align="center">\n    <a href="https://codecov.io/gh/so1n/pait" target="_blank">\n        <img src="https://codecov.io/gh/so1n/pait/branch/master/graph/badge.svg?token=NEVM1VODHR" alt="Coverage">\n    </a>\n</p>\n<p align="center">\n    <a href="https://pypi.org/project/pait/" target="_blank">\n        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pait">\n    </a>\n    <a href="https://pypi.org/project/pait/" target="_blank">\n        <img alt="PyPI" src="https://img.shields.io/pypi/v/pait">\n    </a>\n</p>\n<p align="center">\n    <a href="https://github.com/so1n/pait/actions?query=event%3Apush+branch%3Amaster" target="_blank">\n        <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/so1n/pait/python-package.yml">\n    </a>\n    <a href="https://github.com/so1n/pait/releases" target="_blank">\n        <img alt="GitHub release (release name instead of tag name)" src="https://img.shields.io/github/v/release/so1n/pait?include_prereleases">\n    </a>\n    <a href="https://github.com/so1n/pait/actions?query=event%3Apush+branch%3Amaster" target="_blank">\n        <img src="https://github.com/so1n/pait/actions/workflows/python-package.yml/badge.svg?event=push&branch=master" alt="Test">\n    </a>\n</p>\n<p align="center">\n    <a href="https://github.com/so1n/pait/tree/master/example" target="_blank">\n        <img src="https://img.shields.io/badge/Support%20framework-Flask%2CSanic%2CStarlette%2CTornado-brightgreen" alt="Support framework">\n    </a>\n</p>\n\n\n---\n**Documentation**: [https://so1n.me/pait/](https://so1n.me/pait/)\n\n**中文文档**: [https://so1n.me/pait-zh-doc/](https://so1n.me/pait-zh-doc/)\n\n---\n\n# Warning\nThere are changes between the current version and the 0.8 version of the API, For more information, please refer to [1.0.0version change](https://github.com/so1n/pait/blob/master/CHANGELOG.md)\n\n# pait\n\nPait is an api tool that can be used in any python web framework, the features provided are as follows:\n - [x] Parameter checksum automatic conversion (parameter check depends on `Pydantic`)\n - [x] Parameter dependency verification\n - [x] Automatically generate openapi files\n - [x] Swagger, Redoc, Rapidoc, Elements, OpenAPI route\n - [x] gRPC Gateway route\n - [x] TestClient support, support response result verification\n - [x] Support for plugin extensions, such as the Mock plugin, CheckResponse Plugin, Cache Response Plugin\n - [ ] WebSocket support\n - [ ] Auto API Test support\n\n\n> Note:\n>\n> - mypy check 100%\n>\n> - python version >= 3.7 (support postponed annotations)\n\n\n\n# Installation\n```Bash\npip install pait --pre\n```\nIf want to use the gRPC gateway feature, need to add a \'grpc\' dependency:\n```bash\npip install pait[grpc] --pre\n```\n# Simple Example\n```python\nfrom typing import Type\nimport uvicorn  # type: ignore\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\n\nfrom pait.app.starlette import pait\nfrom pait.field import Body\nfrom pait.openapi.doc_route import add_doc_route\nfrom pait.model.response import JsonResponseModel\nfrom pydantic import BaseModel, Field\n\n\nclass DemoResponseModel(JsonResponseModel):\n    """demo post api response model"""\n    class ResponseModel(BaseModel):\n        uid: int = Field()\n        user_name: str = Field()\n\n    description: str = "demo response"\n    response_data: Type[BaseModel] = ResponseModel\n\n\n@pait(response_model_list=[DemoResponseModel])\nasync def demo_post(\n    uid: int = Body.i(description="user id", gt=10, lt=1000),\n    user_name: str = Body.i(description="user name", min_length=2, max_length=4)\n) -> JSONResponse:\n    return JSONResponse({\'uid\': uid, \'user_name\': user_name})\n\n\napp = Starlette(routes=[Route(\'/api\', demo_post, methods=[\'POST\'])])\nadd_doc_route(app)\nuvicorn.run(app)\n```\nSee [documentation](https://so1n.me/pait/) for more features\n\n# Support Web framework\n\n| Framework | Description            |\n|-----------|------------------------|\n| Flask     | All features supported |\n| Sanic     | All features supported |\n| Starlette | All features supported |\n| Tornado   | All features supported |\n| Django    | Coming soon            |\n\n\nIf the web framework is not supported(which you are using).\n\nCan be modified sync web framework according to [pait.app.flask](https://github.com/so1n/pait/blob/master/pait/app/flask.py)\n\nCan be modified async web framework according to [pait.app.starlette](https://github.com/so1n/pait/blob/master/pait/app/starlette.py)\n\n# Performance\nFor the parameter validation and transformation feature, Pait is mainly responsible for injecting the request data dependency into the `Pydantic` model, and then the `Pydanitc` verifies and transforms the data.\n\nThe time consumed by this process <=0.0003 (s), for benchmarks data and subsequent optimization, see [#27](https://github.com/so1n/pait/issues/27)\n\n\n# Full example\nFor more complete examples, please refer to [example](https://github.com/so1n/pait/tree/master/example)\n',
     'author': 'So1n',
     'author_email': 'so1n897046026@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/so1n/pait',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -3,28 +3,23 @@
 'pait.app.base', 'pait.app.base.adapter', 'pait.app.base.security',
 'pait.app.flask', 'pait.app.flask.adapter', 'pait.app.flask.plugin',
 'pait.app.flask.security', 'pait.app.sanic', 'pait.app.sanic.adapter',
 'pait.app.sanic.plugin', 'pait.app.sanic.security', 'pait.app.starlette',
 'pait.app.starlette.adapter', 'pait.app.starlette.plugin',
 'pait.app.starlette.security', 'pait.app.tornado', 'pait.app.tornado.adapter',
 'pait.app.tornado.plugin', 'pait.app.tornado.security', 'pait.extra',
-'pait.grpc', 'pait.grpc.plugin', 'pait.grpc.proto', 'pait.model',
-'pait.openapi', 'pait.param_handle', 'pait.plugin', 'pait.util'] package_data =
-\ {'': ['*']} install_requires = \ ['any-api>=0.1.0.4,<0.2.0.0',
+'pait.model', 'pait.openapi', 'pait.param_handle', 'pait.plugin', 'pait.util']
+package_data = \ {'': ['*']} install_requires = \ ['any-api>=0.1.0.4,<0.2.0.0',
 'pydantic>=1.7.3,<2.0.0', 'typing-extensions>=4.1.1,<5.0.0'] extras_require = \
-{':extra == "grpc" or extra == "all"': ['protobuf-to-
-pydantic>=0.1.7.3,<0.2.0.0'], 'all': ['redis>=4.2.2,<5.0.0', 'jinja2>=2.0.0'],
-'grpc': ['jinja2>=2.0.0'], 'redis': ['redis>=4.2.2,<5.0.0']} entry_points = \
-{'console_scripts': ['protoc-gen-pait-route = pait.grpc.plugin.main:main']}
-setup_kwargs = { 'name': 'pait', 'version': '1.0.0a6', 'description': 'Pait is
-a Python api tool. Pait enables your Python web framework to have type
-checking, parameter type conversion, interface document generation and can
-display your documents through Redoc or Swagger (power by inspect, pydantic)',
-'long_description': '![](https://cdn.jsdelivr.net/gh/so1n/
-so1n_blog_photo@master/blog_photo/
+{'all': ['redis>=4.2.2,<5.0.0'], 'redis': ['redis>=4.2.2,<5.0.0']} setup_kwargs
+= { 'name': 'pait', 'version': '1.0.0a7', 'description': 'Pait is a Python api
+tool. Pait enables your Python web framework to have type checking, parameter
+type conversion, interface document generation and can display your documents
+through Redoc or Swagger (power by inspect, pydantic)', 'long_description': '!
+[](https://cdn.jsdelivr.net/gh/so1n/so1n_blog_photo@master/blog_photo/
 1652600629491%E6%9C%AA%E5%91%BD%E5%90%8D.jpg)\n
 \n Pait(Ï tool) - Python Modern API Tools, easier to use web frameworks/write
                                  API routing\n
 \n
                              \n \n_[Coverage]\n\n
 \n
                 \n \n_[PyPI_-_Python_Version]\n\n \n_[PyPI]\n\n
@@ -80,9 +75,8 @@
 (s), for benchmarks data and subsequent optimization, see [#27](https://
 github.com/so1n/pait/issues/27)\n\n\n# Full example\nFor more complete
 examples, please refer to [example](https://github.com/so1n/pait/tree/master/
 example)\n', 'author': 'So1n', 'author_email': 'so1n897046026@gmail.com',
 'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
 so1n/pait', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'extras_require': extras_require,
-'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `pait-1.0.0a6/PKG-INFO` & `pait-1.0.0a7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: pait
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Pait is a Python api tool. Pait enables your Python web framework to have type checking, parameter type conversion, interface document generation and can display your documents through Redoc or Swagger (power by inspect, pydantic)
 Home-page: https://github.com/so1n/pait
 License: Apache Software License
 Author: So1n
 Author-email: so1n897046026@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
-Provides-Extra: grpc
 Provides-Extra: redis
 Requires-Dist: any-api (>=0.1.0.4,<0.2.0.0)
-Requires-Dist: jinja2 (>=2.0.0) ; extra == "grpc" or extra == "all"
-Requires-Dist: protobuf-to-pydantic (>=0.1.7.3,<0.2.0.0) ; extra == "grpc" or extra == "all"
 Requires-Dist: pydantic (>=1.7.3,<2.0.0)
 Requires-Dist: redis (>=4.2.2,<5.0.0) ; extra == "redis" or extra == "all"
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Project-URL: Changelog, https://github.com/so1n/pait/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://so1n.me/pait/
 Project-URL: Repository, https://github.com/so1n/pait
 Project-URL: Source, https://github.com/so1n/pait
```

