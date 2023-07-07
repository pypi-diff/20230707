# Comparing `tmp/pait-1.0.0a8.tar.gz` & `tmp/pait-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pait-1.0.0a8.tar", max compression
+gzip compressed data, was "pait-1.0.0a9.tar", max compression
```

## Comparing `pait-1.0.0a8.tar` & `pait-1.0.0a9.tar`

### file list

```diff
@@ -1,162 +1,162 @@
--rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 pait-1.0.0a8/LICENSE
--rw-r--r--   0        0        0     5244 2023-05-10 15:19:11.464788 pait-1.0.0a8/README.md
--rw-r--r--   0        0        0       37 2023-05-24 03:47:38.134524 pait-1.0.0a8/pait/__init__.py
--rw-r--r--   0        0        0       31 2023-07-07 17:36:35.303602 pait-1.0.0a8/pait/__version__.py
--rw-r--r--   0        0        0      216 2023-07-03 05:59:15.586022 pait-1.0.0a8/pait/app/__init__.py
--rw-r--r--   0        0        0     5528 2023-05-23 09:37:37.084528 pait-1.0.0a8/pait/app/any/__init__.py
--rw-r--r--   0        0        0      535 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/any/plugin/__init__.py
--rw-r--r--   0        0        0      460 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/any/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0      425 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/any/plugin/cache_response.py
--rw-r--r--   0        0        0      405 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/any/plugin/check_json_resp.py
--rw-r--r--   0        0        0      373 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/any/plugin/mock_response.py
--rw-r--r--   0        0        0      424 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/any/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-17 11:47:59.744123 pait-1.0.0a8/pait/app/any/security/__init__.py
--rw-r--r--   0        0        0      342 2023-02-08 03:58:49.610123 pait-1.0.0a8/pait/app/any/security/api_key.py
--rw-r--r--   0        0        0      653 2023-02-10 15:24:31.281635 pait-1.0.0a8/pait/app/any/security/http.py
--rw-r--r--   0        0        0      660 2023-02-08 03:43:07.655826 pait-1.0.0a8/pait/app/any/security/oauth2.py
--rw-r--r--   0        0        0     1813 2023-07-07 17:33:22.996081 pait-1.0.0a8/pait/app/any/util.py
--rw-r--r--   0        0        0      562 2023-02-15 10:04:32.538762 pait-1.0.0a8/pait/app/auto_load_app.py
--rw-r--r--   0        0        0      121 2023-01-09 15:13:50.000000 pait-1.0.0a8/pait/app/base/__init__.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a8/pait/app/base/adapter/__init__.py
--rw-r--r--   0        0        0     2427 2023-04-08 08:28:39.674480 pait-1.0.0a8/pait/app/base/adapter/request.py
--rw-r--r--   0        0        0     1806 2023-05-10 15:19:11.476786 pait-1.0.0a8/pait/app/base/app_helper.py
--rw-r--r--   0        0        0        0 2023-02-10 10:23:08.836059 pait-1.0.0a8/pait/app/base/security/__init__.py
--rw-r--r--   0        0        0     1778 2023-07-07 10:50:44.765821 pait-1.0.0a8/pait/app/base/security/api_key.py
--rw-r--r--   0        0        0     1303 2023-07-07 10:43:33.927811 pait-1.0.0a8/pait/app/base/security/base.py
--rw-r--r--   0        0        0     7453 2023-07-07 10:43:33.915811 pait-1.0.0a8/pait/app/base/security/http.py
--rw-r--r--   0        0        0     5121 2023-07-07 10:48:48.593293 pait-1.0.0a8/pait/app/base/security/oauth2.py
--rw-r--r--   0        0        0      794 2023-05-16 11:28:00.165083 pait-1.0.0a8/pait/app/base/security/util.py
--rw-r--r--   0        0        0      649 2023-05-10 15:19:11.476786 pait-1.0.0a8/pait/app/base/simple_route.py
--rw-r--r--   0        0        0    14223 2023-07-05 10:09:10.863486 pait-1.0.0a8/pait/app/base/test_helper.py
--rw-r--r--   0        0        0      332 2023-07-03 05:59:15.586022 pait-1.0.0a8/pait/app/flask/__init__.py
--rw-r--r--   0        0        0      719 2023-03-21 10:06:14.408062 pait-1.0.0a8/pait/app/flask/_app_helper.py
--rw-r--r--   0        0        0      394 2023-03-21 10:06:14.408062 pait-1.0.0a8/pait/app/flask/_attribute.py
--rw-r--r--   0        0        0      792 2023-05-10 15:19:11.476786 pait-1.0.0a8/pait/app/flask/_exception.py
--rw-r--r--   0        0        0     3495 2023-05-10 15:19:11.476786 pait-1.0.0a8/pait/app/flask/_load_app.py
--rw-r--r--   0        0        0      269 2022-01-10 09:58:31.000000 pait-1.0.0a8/pait/app/flask/_pait.py
--rw-r--r--   0        0        0     1775 2023-05-10 15:19:11.476786 pait-1.0.0a8/pait/app/flask/_simple_route.py
--rw-r--r--   0        0        0     1872 2023-07-04 16:28:15.974810 pait-1.0.0a8/pait/app/flask/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a8/pait/app/flask/adapter/__init__.py
--rw-r--r--   0        0        0     1689 2023-04-08 08:28:39.674480 pait-1.0.0a8/pait/app/flask/adapter/request.py
--rw-r--r--   0        0        0     1070 2023-05-10 15:19:11.476786 pait-1.0.0a8/pait/app/flask/adapter/response.py
--rw-r--r--   0        0        0      784 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/flask/plugin/__init__.py
--rw-r--r--   0        0        0      117 2023-02-06 11:24:42.996357 pait-1.0.0a8/pait/app/flask/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0      138 2023-05-23 09:37:36.512526 pait-1.0.0a8/pait/app/flask/plugin/cache_response.py
--rw-r--r--   0        0        0      556 2023-05-10 15:19:11.476786 pait-1.0.0a8/pait/app/flask/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1208 2023-05-23 03:11:41.942069 pait-1.0.0a8/pait/app/flask/plugin/mock_response.py
--rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/flask/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a8/pait/app/flask/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/flask/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/flask/security/http.py
--rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/flask/security/oauth2.py
--rw-r--r--   0        0        0      321 2023-05-10 15:19:11.476786 pait-1.0.0a8/pait/app/flask/security/util.py
--rw-r--r--   0        0        0      332 2023-07-03 05:59:15.586022 pait-1.0.0a8/pait/app/sanic/__init__.py
--rw-r--r--   0        0        0      938 2023-03-21 10:06:14.408062 pait-1.0.0a8/pait/app/sanic/_app_helper.py
--rw-r--r--   0        0        0      403 2023-03-21 10:06:14.412062 pait-1.0.0a8/pait/app/sanic/_attribute.py
--rw-r--r--   0        0        0      319 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/sanic/_exception.py
--rw-r--r--   0        0        0     3902 2023-05-19 10:54:00.027470 pait-1.0.0a8/pait/app/sanic/_load_app.py
--rw-r--r--   0        0        0      374 2023-05-09 02:55:20.341357 pait-1.0.0a8/pait/app/sanic/_pait.py
--rw-r--r--   0        0        0     1749 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/sanic/_simple_route.py
--rw-r--r--   0        0        0     2144 2023-07-04 16:28:15.982810 pait-1.0.0a8/pait/app/sanic/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a8/pait/app/sanic/adapter/__init__.py
--rw-r--r--   0        0        0     2067 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/sanic/adapter/request.py
--rw-r--r--   0        0        0     1102 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/sanic/adapter/response.py
--rw-r--r--   0        0        0      716 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/sanic/plugin/__init__.py
--rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/sanic/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0      138 2023-05-23 09:37:36.508526 pait-1.0.0a8/pait/app/sanic/plugin/cache_response.py
--rw-r--r--   0        0        0      934 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/sanic/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1432 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/sanic/plugin/mock_response.py
--rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/sanic/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a8/pait/app/sanic/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/sanic/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/sanic/security/http.py
--rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/sanic/security/oauth2.py
--rw-r--r--   0        0        0      321 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/sanic/security/util.py
--rw-r--r--   0        0        0      336 2023-07-03 05:59:15.586022 pait-1.0.0a8/pait/app/starlette/__init__.py
--rw-r--r--   0        0        0      651 2023-03-21 10:06:14.412062 pait-1.0.0a8/pait/app/starlette/_app_helper.py
--rw-r--r--   0        0        0      430 2023-03-21 10:06:14.412062 pait-1.0.0a8/pait/app/starlette/_attribute.py
--rw-r--r--   0        0        0      319 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/starlette/_exception.py
--rw-r--r--   0        0        0     3877 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/starlette/_load_app.py
--rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a8/pait/app/starlette/_pait.py
--rw-r--r--   0        0        0      996 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/starlette/_simple_route.py
--rw-r--r--   0        0        0     1993 2023-07-04 16:28:15.954809 pait-1.0.0a8/pait/app/starlette/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a8/pait/app/starlette/adapter/__init__.py
--rw-r--r--   0        0        0     2718 2023-04-08 08:28:39.674480 pait-1.0.0a8/pait/app/starlette/adapter/request.py
--rw-r--r--   0        0        0     1065 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/starlette/adapter/response.py
--rw-r--r--   0        0        0      800 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/starlette/plugin/__init__.py
--rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/starlette/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0      138 2023-05-23 09:37:36.560526 pait-1.0.0a8/pait/app/starlette/plugin/cache_response.py
--rw-r--r--   0        0        0      785 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/starlette/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1626 2023-02-16 07:49:53.639890 pait-1.0.0a8/pait/app/starlette/plugin/mock_response.py
--rw-r--r--   0        0        0      702 2023-02-07 03:41:51.356781 pait-1.0.0a8/pait/app/starlette/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a8/pait/app/starlette/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/starlette/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/starlette/security/http.py
--rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/starlette/security/oauth2.py
--rw-r--r--   0        0        0      325 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/starlette/security/util.py
--rw-r--r--   0        0        0      334 2023-07-03 05:59:15.586022 pait-1.0.0a8/pait/app/tornado/__init__.py
--rw-r--r--   0        0        0     1002 2023-03-21 10:06:14.412062 pait-1.0.0a8/pait/app/tornado/_app_helper.py
--rw-r--r--   0        0        0      424 2023-03-21 10:06:14.412062 pait-1.0.0a8/pait/app/tornado/_attribute.py
--rw-r--r--   0        0        0      298 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/tornado/_exception.py
--rw-r--r--   0        0        0     2559 2023-05-19 10:54:00.027470 pait-1.0.0a8/pait/app/tornado/_load_app.py
--rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a8/pait/app/tornado/_pait.py
--rw-r--r--   0        0        0     2839 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/tornado/_simple_route.py
--rw-r--r--   0        0        0     4636 2023-07-04 16:28:15.966810 pait-1.0.0a8/pait/app/tornado/_test_helper.py
--rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a8/pait/app/tornado/adapter/__init__.py
--rw-r--r--   0        0        0     2244 2023-04-08 08:28:39.674480 pait-1.0.0a8/pait/app/tornado/adapter/request.py
--rw-r--r--   0        0        0     1130 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/tornado/adapter/response.py
--rw-r--r--   0        0        0      792 2023-02-07 03:41:51.360782 pait-1.0.0a8/pait/app/tornado/plugin/__init__.py
--rw-r--r--   0        0        0      574 2023-02-07 03:41:51.360782 pait-1.0.0a8/pait/app/tornado/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0     1411 2023-05-23 09:37:36.612527 pait-1.0.0a8/pait/app/tornado/plugin/cache_response.py
--rw-r--r--   0        0        0     1211 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/tornado/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1237 2023-02-07 03:41:51.360782 pait-1.0.0a8/pait/app/tornado/plugin/mock_response.py
--rw-r--r--   0        0        0     1247 2023-02-07 03:41:51.360782 pait-1.0.0a8/pait/app/tornado/plugin/unified_response.py
--rw-r--r--   0        0        0        0 2023-02-03 19:54:29.188502 pait-1.0.0a8/pait/app/tornado/security/__init__.py
--rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/tornado/security/api_key.py
--rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/tornado/security/http.py
--rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a8/pait/app/tornado/security/oauth2.py
--rw-r--r--   0        0        0      323 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/app/tornado/security/util.py
--rw-r--r--   0        0        0    18186 2023-05-23 08:13:27.664682 pait-1.0.0a8/pait/core.py
--rw-r--r--   0        0        0     1645 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/data.py
--rw-r--r--   0        0        0      688 2023-01-11 17:12:40.000000 pait-1.0.0a8/pait/exceptions.py
--rw-r--r--   0        0        0        0 2022-04-03 14:03:33.000000 pait-1.0.0a8/pait/extra/__init__.py
--rw-r--r--   0        0        0     7254 2023-05-19 10:54:00.027470 pait-1.0.0a8/pait/extra/config.py
--rw-r--r--   0        0        0      996 2023-07-04 06:31:08.417272 pait-1.0.0a8/pait/extra/util.py
--rw-r--r--   0        0        0    11023 2023-07-07 10:37:02.645782 pait-1.0.0a8/pait/field.py
--rw-r--r--   0        0        0     1261 2023-05-10 15:19:11.480786 pait-1.0.0a8/pait/g.py
--rw-r--r--   0        0        0      559 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/model/__init__.py
--rw-r--r--   0        0        0     3305 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/model/config.py
--rw-r--r--   0        0        0     1606 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/model/context.py
--rw-r--r--   0        0        0     9443 2023-05-23 09:37:37.408529 pait-1.0.0a8/pait/model/core.py
--rw-r--r--   0        0        0     6051 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/model/response.py
--rw-r--r--   0        0        0      908 2023-05-28 10:00:37.748027 pait-1.0.0a8/pait/model/status.py
--rw-r--r--   0        0        0     1400 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/model/tag.py
--rw-r--r--   0        0        0     1166 2022-09-26 15:06:36.000000 pait-1.0.0a8/pait/model/template.py
--rw-r--r--   0        0        0        0 2022-01-21 03:47:13.000000 pait-1.0.0a8/pait/openapi/__init__.py
--rw-r--r--   0        0        0     9701 2023-06-18 05:44:11.012681 pait-1.0.0a8/pait/openapi/doc_route.py
--rw-r--r--   0        0        0    12159 2023-05-28 10:02:29.009525 pait-1.0.0a8/pait/openapi/openapi.py
--rw-r--r--   0        0        0      105 2023-02-07 03:41:51.360782 pait-1.0.0a8/pait/param_handle/__init__.py
--rw-r--r--   0        0        0     6319 2023-06-12 07:13:53.829457 pait-1.0.0a8/pait/param_handle/_async.py
--rw-r--r--   0        0        0     5262 2023-06-12 07:13:53.829457 pait-1.0.0a8/pait/param_handle/_sync.py
--rw-r--r--   0        0        0    12598 2023-06-12 07:13:53.829457 pait-1.0.0a8/pait/param_handle/base.py
--rw-r--r--   0        0        0       87 2023-02-07 03:41:51.360782 pait-1.0.0a8/pait/plugin/__init__.py
--rw-r--r--   0        0        0     2298 2023-02-07 03:41:51.360782 pait-1.0.0a8/pait/plugin/at_most_one_of.py
--rw-r--r--   0        0        0     2599 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0     3592 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/plugin/base.py
--rw-r--r--   0        0        0     8867 2023-05-23 09:45:50.401974 pait-1.0.0a8/pait/plugin/cache_response.py
--rw-r--r--   0        0        0     2228 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/plugin/check_json_resp.py
--rw-r--r--   0        0        0     5145 2023-05-23 09:37:37.272529 pait-1.0.0a8/pait/plugin/mock_response.py
--rw-r--r--   0        0        0     3312 2023-02-07 03:41:51.360782 pait-1.0.0a8/pait/plugin/required.py
--rw-r--r--   0        0        0     2109 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/plugin/unified_response.py
--rw-r--r--   0        0        0     1407 2023-07-07 10:36:04.885454 pait-1.0.0a8/pait/types.py
--rw-r--r--   0        0        0      524 2023-02-14 09:33:41.434168 pait-1.0.0a8/pait/util/__init__.py
--rw-r--r--   0        0        0     2185 2023-06-12 07:13:53.829457 pait-1.0.0a8/pait/util/_func_sig.py
--rw-r--r--   0        0        0     2607 2023-01-12 10:30:13.000000 pait-1.0.0a8/pait/util/_gen_tip.py
--rw-r--r--   0        0        0     1907 2022-04-10 08:10:06.000000 pait-1.0.0a8/pait/util/_lazy_property.py
--rw-r--r--   0        0        0      957 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/util/_pydantic_util.py
--rw-r--r--   0        0        0     4211 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/util/_types.py
--rw-r--r--   0        0        0    13534 2023-05-30 08:34:59.099755 pait-1.0.0a8/pait/util/_util.py
--rw-r--r--   0        0        0      869 2023-05-10 15:19:11.484786 pait-1.0.0a8/pait/util/encoder.py
--rw-r--r--   0        0        0     3140 2023-07-07 17:36:35.299601 pait-1.0.0a8/pyproject.toml
--rw-r--r--   0        0        0     7093 1970-01-01 00:00:00.000000 pait-1.0.0a8/setup.py
--rw-r--r--   0        0        0     6619 1970-01-01 00:00:00.000000 pait-1.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 pait-1.0.0a9/LICENSE
+-rw-r--r--   0        0        0     5244 2023-05-10 15:19:11.464788 pait-1.0.0a9/README.md
+-rw-r--r--   0        0        0       37 2023-05-24 03:47:38.134524 pait-1.0.0a9/pait/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-07 19:10:56.774946 pait-1.0.0a9/pait/__version__.py
+-rw-r--r--   0        0        0      216 2023-07-03 05:59:15.586022 pait-1.0.0a9/pait/app/__init__.py
+-rw-r--r--   0        0        0     5528 2023-05-23 09:37:37.084528 pait-1.0.0a9/pait/app/any/__init__.py
+-rw-r--r--   0        0        0      535 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/any/plugin/__init__.py
+-rw-r--r--   0        0        0      460 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/any/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      425 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/any/plugin/cache_response.py
+-rw-r--r--   0        0        0      405 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/any/plugin/check_json_resp.py
+-rw-r--r--   0        0        0      373 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/any/plugin/mock_response.py
+-rw-r--r--   0        0        0      424 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/any/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-17 11:47:59.744123 pait-1.0.0a9/pait/app/any/security/__init__.py
+-rw-r--r--   0        0        0      342 2023-02-08 03:58:49.610123 pait-1.0.0a9/pait/app/any/security/api_key.py
+-rw-r--r--   0        0        0      653 2023-02-10 15:24:31.281635 pait-1.0.0a9/pait/app/any/security/http.py
+-rw-r--r--   0        0        0      660 2023-02-08 03:43:07.655826 pait-1.0.0a9/pait/app/any/security/oauth2.py
+-rw-r--r--   0        0        0     1943 2023-07-07 19:09:24.678676 pait-1.0.0a9/pait/app/any/util.py
+-rw-r--r--   0        0        0      562 2023-02-15 10:04:32.538762 pait-1.0.0a9/pait/app/auto_load_app.py
+-rw-r--r--   0        0        0      121 2023-01-09 15:13:50.000000 pait-1.0.0a9/pait/app/base/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a9/pait/app/base/adapter/__init__.py
+-rw-r--r--   0        0        0     2427 2023-04-08 08:28:39.674480 pait-1.0.0a9/pait/app/base/adapter/request.py
+-rw-r--r--   0        0        0     1806 2023-05-10 15:19:11.476786 pait-1.0.0a9/pait/app/base/app_helper.py
+-rw-r--r--   0        0        0        0 2023-02-10 10:23:08.836059 pait-1.0.0a9/pait/app/base/security/__init__.py
+-rw-r--r--   0        0        0     1778 2023-07-07 10:50:44.765821 pait-1.0.0a9/pait/app/base/security/api_key.py
+-rw-r--r--   0        0        0     1303 2023-07-07 10:43:33.927811 pait-1.0.0a9/pait/app/base/security/base.py
+-rw-r--r--   0        0        0     7453 2023-07-07 10:43:33.915811 pait-1.0.0a9/pait/app/base/security/http.py
+-rw-r--r--   0        0        0     5121 2023-07-07 10:48:48.593293 pait-1.0.0a9/pait/app/base/security/oauth2.py
+-rw-r--r--   0        0        0      794 2023-05-16 11:28:00.165083 pait-1.0.0a9/pait/app/base/security/util.py
+-rw-r--r--   0        0        0      649 2023-05-10 15:19:11.476786 pait-1.0.0a9/pait/app/base/simple_route.py
+-rw-r--r--   0        0        0    14223 2023-07-05 10:09:10.863486 pait-1.0.0a9/pait/app/base/test_helper.py
+-rw-r--r--   0        0        0      332 2023-07-03 05:59:15.586022 pait-1.0.0a9/pait/app/flask/__init__.py
+-rw-r--r--   0        0        0      719 2023-03-21 10:06:14.408062 pait-1.0.0a9/pait/app/flask/_app_helper.py
+-rw-r--r--   0        0        0      394 2023-03-21 10:06:14.408062 pait-1.0.0a9/pait/app/flask/_attribute.py
+-rw-r--r--   0        0        0      792 2023-05-10 15:19:11.476786 pait-1.0.0a9/pait/app/flask/_exception.py
+-rw-r--r--   0        0        0     3495 2023-05-10 15:19:11.476786 pait-1.0.0a9/pait/app/flask/_load_app.py
+-rw-r--r--   0        0        0      269 2022-01-10 09:58:31.000000 pait-1.0.0a9/pait/app/flask/_pait.py
+-rw-r--r--   0        0        0     1775 2023-05-10 15:19:11.476786 pait-1.0.0a9/pait/app/flask/_simple_route.py
+-rw-r--r--   0        0        0     1872 2023-07-04 16:28:15.974810 pait-1.0.0a9/pait/app/flask/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a9/pait/app/flask/adapter/__init__.py
+-rw-r--r--   0        0        0     1689 2023-04-08 08:28:39.674480 pait-1.0.0a9/pait/app/flask/adapter/request.py
+-rw-r--r--   0        0        0     1070 2023-05-10 15:19:11.476786 pait-1.0.0a9/pait/app/flask/adapter/response.py
+-rw-r--r--   0        0        0      784 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/flask/plugin/__init__.py
+-rw-r--r--   0        0        0      117 2023-02-06 11:24:42.996357 pait-1.0.0a9/pait/app/flask/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      138 2023-05-23 09:37:36.512526 pait-1.0.0a9/pait/app/flask/plugin/cache_response.py
+-rw-r--r--   0        0        0      556 2023-05-10 15:19:11.476786 pait-1.0.0a9/pait/app/flask/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1208 2023-05-23 03:11:41.942069 pait-1.0.0a9/pait/app/flask/plugin/mock_response.py
+-rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/flask/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a9/pait/app/flask/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/flask/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/flask/security/http.py
+-rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/flask/security/oauth2.py
+-rw-r--r--   0        0        0      321 2023-05-10 15:19:11.476786 pait-1.0.0a9/pait/app/flask/security/util.py
+-rw-r--r--   0        0        0      332 2023-07-03 05:59:15.586022 pait-1.0.0a9/pait/app/sanic/__init__.py
+-rw-r--r--   0        0        0      938 2023-03-21 10:06:14.408062 pait-1.0.0a9/pait/app/sanic/_app_helper.py
+-rw-r--r--   0        0        0      403 2023-03-21 10:06:14.412062 pait-1.0.0a9/pait/app/sanic/_attribute.py
+-rw-r--r--   0        0        0      319 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/sanic/_exception.py
+-rw-r--r--   0        0        0     3902 2023-05-19 10:54:00.027470 pait-1.0.0a9/pait/app/sanic/_load_app.py
+-rw-r--r--   0        0        0      374 2023-05-09 02:55:20.341357 pait-1.0.0a9/pait/app/sanic/_pait.py
+-rw-r--r--   0        0        0     1749 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/sanic/_simple_route.py
+-rw-r--r--   0        0        0     2144 2023-07-04 16:28:15.982810 pait-1.0.0a9/pait/app/sanic/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a9/pait/app/sanic/adapter/__init__.py
+-rw-r--r--   0        0        0     2067 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/sanic/adapter/request.py
+-rw-r--r--   0        0        0     1102 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/sanic/adapter/response.py
+-rw-r--r--   0        0        0      716 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/sanic/plugin/__init__.py
+-rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/sanic/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      138 2023-05-23 09:37:36.508526 pait-1.0.0a9/pait/app/sanic/plugin/cache_response.py
+-rw-r--r--   0        0        0      934 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/sanic/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1432 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/sanic/plugin/mock_response.py
+-rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/sanic/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a9/pait/app/sanic/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/sanic/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/sanic/security/http.py
+-rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/sanic/security/oauth2.py
+-rw-r--r--   0        0        0      321 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/sanic/security/util.py
+-rw-r--r--   0        0        0      336 2023-07-03 05:59:15.586022 pait-1.0.0a9/pait/app/starlette/__init__.py
+-rw-r--r--   0        0        0      651 2023-03-21 10:06:14.412062 pait-1.0.0a9/pait/app/starlette/_app_helper.py
+-rw-r--r--   0        0        0      430 2023-03-21 10:06:14.412062 pait-1.0.0a9/pait/app/starlette/_attribute.py
+-rw-r--r--   0        0        0      319 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/starlette/_exception.py
+-rw-r--r--   0        0        0     3877 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/starlette/_load_app.py
+-rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a9/pait/app/starlette/_pait.py
+-rw-r--r--   0        0        0      996 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/starlette/_simple_route.py
+-rw-r--r--   0        0        0     1993 2023-07-04 16:28:15.954809 pait-1.0.0a9/pait/app/starlette/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a9/pait/app/starlette/adapter/__init__.py
+-rw-r--r--   0        0        0     2718 2023-04-08 08:28:39.674480 pait-1.0.0a9/pait/app/starlette/adapter/request.py
+-rw-r--r--   0        0        0     1065 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/starlette/adapter/response.py
+-rw-r--r--   0        0        0      800 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/starlette/plugin/__init__.py
+-rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/starlette/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      138 2023-05-23 09:37:36.560526 pait-1.0.0a9/pait/app/starlette/plugin/cache_response.py
+-rw-r--r--   0        0        0      785 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/starlette/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1626 2023-02-16 07:49:53.639890 pait-1.0.0a9/pait/app/starlette/plugin/mock_response.py
+-rw-r--r--   0        0        0      702 2023-02-07 03:41:51.356781 pait-1.0.0a9/pait/app/starlette/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a9/pait/app/starlette/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/starlette/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/starlette/security/http.py
+-rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/starlette/security/oauth2.py
+-rw-r--r--   0        0        0      325 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/starlette/security/util.py
+-rw-r--r--   0        0        0      334 2023-07-03 05:59:15.586022 pait-1.0.0a9/pait/app/tornado/__init__.py
+-rw-r--r--   0        0        0     1002 2023-03-21 10:06:14.412062 pait-1.0.0a9/pait/app/tornado/_app_helper.py
+-rw-r--r--   0        0        0      424 2023-03-21 10:06:14.412062 pait-1.0.0a9/pait/app/tornado/_attribute.py
+-rw-r--r--   0        0        0      298 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/tornado/_exception.py
+-rw-r--r--   0        0        0     2559 2023-05-19 10:54:00.027470 pait-1.0.0a9/pait/app/tornado/_load_app.py
+-rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a9/pait/app/tornado/_pait.py
+-rw-r--r--   0        0        0     2839 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/tornado/_simple_route.py
+-rw-r--r--   0        0        0     4636 2023-07-04 16:28:15.966810 pait-1.0.0a9/pait/app/tornado/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a9/pait/app/tornado/adapter/__init__.py
+-rw-r--r--   0        0        0     2244 2023-04-08 08:28:39.674480 pait-1.0.0a9/pait/app/tornado/adapter/request.py
+-rw-r--r--   0        0        0     1130 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/tornado/adapter/response.py
+-rw-r--r--   0        0        0      792 2023-02-07 03:41:51.360782 pait-1.0.0a9/pait/app/tornado/plugin/__init__.py
+-rw-r--r--   0        0        0      574 2023-02-07 03:41:51.360782 pait-1.0.0a9/pait/app/tornado/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0     1411 2023-05-23 09:37:36.612527 pait-1.0.0a9/pait/app/tornado/plugin/cache_response.py
+-rw-r--r--   0        0        0     1211 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/tornado/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1237 2023-02-07 03:41:51.360782 pait-1.0.0a9/pait/app/tornado/plugin/mock_response.py
+-rw-r--r--   0        0        0     1247 2023-02-07 03:41:51.360782 pait-1.0.0a9/pait/app/tornado/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-02-03 19:54:29.188502 pait-1.0.0a9/pait/app/tornado/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/tornado/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/tornado/security/http.py
+-rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a9/pait/app/tornado/security/oauth2.py
+-rw-r--r--   0        0        0      323 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/app/tornado/security/util.py
+-rw-r--r--   0        0        0    18186 2023-05-23 08:13:27.664682 pait-1.0.0a9/pait/core.py
+-rw-r--r--   0        0        0     1645 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/data.py
+-rw-r--r--   0        0        0      688 2023-01-11 17:12:40.000000 pait-1.0.0a9/pait/exceptions.py
+-rw-r--r--   0        0        0        0 2022-04-03 14:03:33.000000 pait-1.0.0a9/pait/extra/__init__.py
+-rw-r--r--   0        0        0     7254 2023-05-19 10:54:00.027470 pait-1.0.0a9/pait/extra/config.py
+-rw-r--r--   0        0        0      996 2023-07-04 06:31:08.417272 pait-1.0.0a9/pait/extra/util.py
+-rw-r--r--   0        0        0    11023 2023-07-07 10:37:02.645782 pait-1.0.0a9/pait/field.py
+-rw-r--r--   0        0        0     1261 2023-05-10 15:19:11.480786 pait-1.0.0a9/pait/g.py
+-rw-r--r--   0        0        0      559 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/model/__init__.py
+-rw-r--r--   0        0        0     3305 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/model/config.py
+-rw-r--r--   0        0        0     1606 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/model/context.py
+-rw-r--r--   0        0        0     9443 2023-05-23 09:37:37.408529 pait-1.0.0a9/pait/model/core.py
+-rw-r--r--   0        0        0     6051 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/model/response.py
+-rw-r--r--   0        0        0      908 2023-05-28 10:00:37.748027 pait-1.0.0a9/pait/model/status.py
+-rw-r--r--   0        0        0     1400 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/model/tag.py
+-rw-r--r--   0        0        0     1166 2022-09-26 15:06:36.000000 pait-1.0.0a9/pait/model/template.py
+-rw-r--r--   0        0        0        0 2022-01-21 03:47:13.000000 pait-1.0.0a9/pait/openapi/__init__.py
+-rw-r--r--   0        0        0     9701 2023-06-18 05:44:11.012681 pait-1.0.0a9/pait/openapi/doc_route.py
+-rw-r--r--   0        0        0    12159 2023-05-28 10:02:29.009525 pait-1.0.0a9/pait/openapi/openapi.py
+-rw-r--r--   0        0        0      105 2023-02-07 03:41:51.360782 pait-1.0.0a9/pait/param_handle/__init__.py
+-rw-r--r--   0        0        0     6319 2023-06-12 07:13:53.829457 pait-1.0.0a9/pait/param_handle/_async.py
+-rw-r--r--   0        0        0     5262 2023-06-12 07:13:53.829457 pait-1.0.0a9/pait/param_handle/_sync.py
+-rw-r--r--   0        0        0    12598 2023-06-12 07:13:53.829457 pait-1.0.0a9/pait/param_handle/base.py
+-rw-r--r--   0        0        0       87 2023-02-07 03:41:51.360782 pait-1.0.0a9/pait/plugin/__init__.py
+-rw-r--r--   0        0        0     2298 2023-02-07 03:41:51.360782 pait-1.0.0a9/pait/plugin/at_most_one_of.py
+-rw-r--r--   0        0        0     2599 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0     3592 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/plugin/base.py
+-rw-r--r--   0        0        0     8867 2023-05-23 09:45:50.401974 pait-1.0.0a9/pait/plugin/cache_response.py
+-rw-r--r--   0        0        0     2228 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     5145 2023-05-23 09:37:37.272529 pait-1.0.0a9/pait/plugin/mock_response.py
+-rw-r--r--   0        0        0     3312 2023-02-07 03:41:51.360782 pait-1.0.0a9/pait/plugin/required.py
+-rw-r--r--   0        0        0     2109 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/plugin/unified_response.py
+-rw-r--r--   0        0        0     1407 2023-07-07 10:36:04.885454 pait-1.0.0a9/pait/types.py
+-rw-r--r--   0        0        0      524 2023-02-14 09:33:41.434168 pait-1.0.0a9/pait/util/__init__.py
+-rw-r--r--   0        0        0     2185 2023-06-12 07:13:53.829457 pait-1.0.0a9/pait/util/_func_sig.py
+-rw-r--r--   0        0        0     2607 2023-01-12 10:30:13.000000 pait-1.0.0a9/pait/util/_gen_tip.py
+-rw-r--r--   0        0        0     1907 2022-04-10 08:10:06.000000 pait-1.0.0a9/pait/util/_lazy_property.py
+-rw-r--r--   0        0        0      957 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/util/_pydantic_util.py
+-rw-r--r--   0        0        0     4211 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/util/_types.py
+-rw-r--r--   0        0        0    13534 2023-05-30 08:34:59.099755 pait-1.0.0a9/pait/util/_util.py
+-rw-r--r--   0        0        0      869 2023-05-10 15:19:11.484786 pait-1.0.0a9/pait/util/encoder.py
+-rw-r--r--   0        0        0     3140 2023-07-07 19:10:56.774946 pait-1.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0     7093 1970-01-01 00:00:00.000000 pait-1.0.0a9/setup.py
+-rw-r--r--   0        0        0     6619 1970-01-01 00:00:00.000000 pait-1.0.0a9/PKG-INFO
```

### Comparing `pait-1.0.0a8/LICENSE` & `pait-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/README.md` & `pait-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/any/__init__.py` & `pait-1.0.0a9/pait/app/any/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/any/plugin/__init__.py` & `pait-1.0.0a9/pait/app/any/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/any/security/http.py` & `pait-1.0.0a9/pait/app/any/security/http.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/any/security/oauth2.py` & `pait-1.0.0a9/pait/app/any/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/any/util.py` & `pait-1.0.0a9/pait/app/any/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,28 @@
 support_app_list: List[SupportAppLiteral] = ["flask", "starlette", "sanic", "tornado"]
 
 sniffing_dict: Dict[Type, Callable[[Any], str]] = {}
 framework_location_dict: Dict[str, str] = {}
 
 
 def sniffing(app: Any) -> SupportAppLiteral:
-    app_name: str = app.__class__.__name__.lower()
-    if app_name in support_app_list:
-        return app_name  # type: ignore
-    elif app_name == "application" and app.__class__.__module__ == "tornado.web":
-        return "tornado"
+    try:
+        for base_class in [app.__class__, app.__class__.__base__]:
+            app_name: str = base_class.__name__.lower()
+            if app_name in support_app_list:
+                return app_name  # type: ignore
+            elif app_name == "application" and base_class.__module__ == "tornado.web":
+                return "tornado"
+    except Exception:
+        pass
 
     if app.__class__ in sniffing_dict:
         return sniffing_dict[app.__class__](app)  # type: ignore
 
-    raise NotImplementedError(f"Pait not support app name:{app_name}, please check app:{app}")
+    raise NotImplementedError(f"Pait not support app: {app}, please check app")
 
 
 def import_func_from_app(fun_name: str, app: Any = None, module_name: str = "") -> Callable:
     from pait.app.auto_load_app import auto_load_app_class
 
     if app:
         # support werkzeug LocalProxy
```

### Comparing `pait-1.0.0a8/pait/app/auto_load_app.py` & `pait-1.0.0a9/pait/app/auto_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/base/adapter/request.py` & `pait-1.0.0a9/pait/app/base/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/base/app_helper.py` & `pait-1.0.0a9/pait/app/base/app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/base/security/api_key.py` & `pait-1.0.0a9/pait/app/base/security/api_key.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/base/security/base.py` & `pait-1.0.0a9/pait/app/base/security/base.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/base/security/http.py` & `pait-1.0.0a9/pait/app/base/security/http.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/base/security/oauth2.py` & `pait-1.0.0a9/pait/app/base/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/base/security/util.py` & `pait-1.0.0a9/pait/app/base/security/util.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/base/simple_route.py` & `pait-1.0.0a9/pait/app/base/simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/base/test_helper.py` & `pait-1.0.0a9/pait/app/base/test_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/_app_helper.py` & `pait-1.0.0a9/pait/app/flask/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/_exception.py` & `pait-1.0.0a9/pait/app/flask/_exception.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/_load_app.py` & `pait-1.0.0a9/pait/app/flask/_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/_simple_route.py` & `pait-1.0.0a9/pait/app/flask/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/_test_helper.py` & `pait-1.0.0a9/pait/app/flask/_test_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/adapter/request.py` & `pait-1.0.0a9/pait/app/flask/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/adapter/response.py` & `pait-1.0.0a9/pait/app/flask/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/plugin/__init__.py` & `pait-1.0.0a9/pait/app/flask/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/plugin/check_json_resp.py` & `pait-1.0.0a9/pait/app/flask/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/plugin/mock_response.py` & `pait-1.0.0a9/pait/app/flask/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/plugin/unified_response.py` & `pait-1.0.0a9/pait/app/flask/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/flask/security/oauth2.py` & `pait-1.0.0a9/pait/app/flask/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/_app_helper.py` & `pait-1.0.0a9/pait/app/sanic/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/_load_app.py` & `pait-1.0.0a9/pait/app/sanic/_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/_simple_route.py` & `pait-1.0.0a9/pait/app/sanic/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/_test_helper.py` & `pait-1.0.0a9/pait/app/sanic/_test_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/adapter/request.py` & `pait-1.0.0a9/pait/app/sanic/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/adapter/response.py` & `pait-1.0.0a9/pait/app/sanic/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/plugin/__init__.py` & `pait-1.0.0a9/pait/app/sanic/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/plugin/auto_complete_json_resp.py` & `pait-1.0.0a9/pait/app/sanic/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/plugin/check_json_resp.py` & `pait-1.0.0a9/pait/app/sanic/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/plugin/mock_response.py` & `pait-1.0.0a9/pait/app/sanic/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/plugin/unified_response.py` & `pait-1.0.0a9/pait/app/sanic/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/sanic/security/oauth2.py` & `pait-1.0.0a9/pait/app/sanic/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/_app_helper.py` & `pait-1.0.0a9/pait/app/starlette/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/_load_app.py` & `pait-1.0.0a9/pait/app/starlette/_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/_simple_route.py` & `pait-1.0.0a9/pait/app/starlette/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/_test_helper.py` & `pait-1.0.0a9/pait/app/starlette/_test_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/adapter/request.py` & `pait-1.0.0a9/pait/app/starlette/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/adapter/response.py` & `pait-1.0.0a9/pait/app/starlette/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/plugin/__init__.py` & `pait-1.0.0a9/pait/app/starlette/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/plugin/auto_complete_json_resp.py` & `pait-1.0.0a9/pait/app/starlette/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/plugin/check_json_resp.py` & `pait-1.0.0a9/pait/app/starlette/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/plugin/mock_response.py` & `pait-1.0.0a9/pait/app/starlette/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/plugin/unified_response.py` & `pait-1.0.0a9/pait/app/starlette/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/starlette/security/oauth2.py` & `pait-1.0.0a9/pait/app/starlette/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/_app_helper.py` & `pait-1.0.0a9/pait/app/tornado/_app_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/_load_app.py` & `pait-1.0.0a9/pait/app/tornado/_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/_simple_route.py` & `pait-1.0.0a9/pait/app/tornado/_simple_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/_test_helper.py` & `pait-1.0.0a9/pait/app/tornado/_test_helper.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/adapter/request.py` & `pait-1.0.0a9/pait/app/tornado/adapter/request.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/adapter/response.py` & `pait-1.0.0a9/pait/app/tornado/adapter/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/plugin/__init__.py` & `pait-1.0.0a9/pait/app/tornado/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/plugin/auto_complete_json_resp.py` & `pait-1.0.0a9/pait/app/tornado/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/plugin/cache_response.py` & `pait-1.0.0a9/pait/app/tornado/plugin/cache_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/plugin/check_json_resp.py` & `pait-1.0.0a9/pait/app/tornado/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/plugin/mock_response.py` & `pait-1.0.0a9/pait/app/tornado/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/plugin/unified_response.py` & `pait-1.0.0a9/pait/app/tornado/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/app/tornado/security/oauth2.py` & `pait-1.0.0a9/pait/app/tornado/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/core.py` & `pait-1.0.0a9/pait/core.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/data.py` & `pait-1.0.0a9/pait/data.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/exceptions.py` & `pait-1.0.0a9/pait/exceptions.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/extra/config.py` & `pait-1.0.0a9/pait/extra/config.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/extra/util.py` & `pait-1.0.0a9/pait/extra/util.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/field.py` & `pait-1.0.0a9/pait/field.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/g.py` & `pait-1.0.0a9/pait/g.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/model/__init__.py` & `pait-1.0.0a9/pait/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/model/config.py` & `pait-1.0.0a9/pait/model/config.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/model/context.py` & `pait-1.0.0a9/pait/model/context.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/model/core.py` & `pait-1.0.0a9/pait/model/core.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/model/response.py` & `pait-1.0.0a9/pait/model/response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/model/status.py` & `pait-1.0.0a9/pait/model/status.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/model/tag.py` & `pait-1.0.0a9/pait/model/tag.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/model/template.py` & `pait-1.0.0a9/pait/model/template.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/openapi/doc_route.py` & `pait-1.0.0a9/pait/openapi/doc_route.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/openapi/openapi.py` & `pait-1.0.0a9/pait/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/param_handle/_async.py` & `pait-1.0.0a9/pait/param_handle/_async.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/param_handle/_sync.py` & `pait-1.0.0a9/pait/param_handle/_sync.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/param_handle/base.py` & `pait-1.0.0a9/pait/param_handle/base.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/plugin/at_most_one_of.py` & `pait-1.0.0a9/pait/plugin/at_most_one_of.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/plugin/auto_complete_json_resp.py` & `pait-1.0.0a9/pait/plugin/auto_complete_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/plugin/base.py` & `pait-1.0.0a9/pait/plugin/base.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/plugin/cache_response.py` & `pait-1.0.0a9/pait/plugin/cache_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/plugin/check_json_resp.py` & `pait-1.0.0a9/pait/plugin/check_json_resp.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/plugin/mock_response.py` & `pait-1.0.0a9/pait/plugin/mock_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/plugin/required.py` & `pait-1.0.0a9/pait/plugin/required.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/plugin/unified_response.py` & `pait-1.0.0a9/pait/plugin/unified_response.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/types.py` & `pait-1.0.0a9/pait/types.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/util/__init__.py` & `pait-1.0.0a9/pait/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/util/_func_sig.py` & `pait-1.0.0a9/pait/util/_func_sig.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/util/_gen_tip.py` & `pait-1.0.0a9/pait/util/_gen_tip.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/util/_lazy_property.py` & `pait-1.0.0a9/pait/util/_lazy_property.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/util/_pydantic_util.py` & `pait-1.0.0a9/pait/util/_pydantic_util.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/util/_types.py` & `pait-1.0.0a9/pait/util/_types.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/util/_util.py` & `pait-1.0.0a9/pait/util/_util.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pait/util/encoder.py` & `pait-1.0.0a9/pait/util/encoder.py`

 * *Files identical despite different names*

### Comparing `pait-1.0.0a8/pyproject.toml` & `pait-1.0.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pait"
-version = "v1.0.0-alpha.8"
+version = "v1.0.0-alpha.9"
 description = "Pait is a Python api tool. Pait enables your Python web framework to have type checking, parameter type conversion, interface document generation and can display your documents through Redoc or Swagger (power by inspect, pydantic)"
 authors = ["So1n <so1n897046026@gmail.com>"]
 license = "Apache Software License"
 readme = "./README.md"
 repository = "https://github.com/so1n/pait"
 homepage = "https://github.com/so1n/pait"
```

### Comparing `pait-1.0.0a8/setup.py` & `pait-1.0.0a9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
  'typing-extensions>=4.1.1,<5.0.0']
 
 extras_require = \
 {'all': ['redis>=4.2.2,<5.0.0'], 'redis': ['redis>=4.2.2,<5.0.0']}
 
 setup_kwargs = {
     'name': 'pait',
-    'version': '1.0.0a8',
+    'version': '1.0.0a9',
     'description': 'Pait is a Python api tool. Pait enables your Python web framework to have type checking, parameter type conversion, interface document generation and can display your documents through Redoc or Swagger (power by inspect, pydantic)',
     'long_description': '![](https://cdn.jsdelivr.net/gh/so1n/so1n_blog_photo@master/blog_photo/1652600629491%E6%9C%AA%E5%91%BD%E5%90%8D.jpg)\n<p align="center">\n    Pait(π tool) - <em>Python Modern API Tools, easier to use web frameworks/write API routing</em>\n</p>\n<p align="center">\n    <a href="https://codecov.io/gh/so1n/pait" target="_blank">\n        <img src="https://codecov.io/gh/so1n/pait/branch/master/graph/badge.svg?token=NEVM1VODHR" alt="Coverage">\n    </a>\n</p>\n<p align="center">\n    <a href="https://pypi.org/project/pait/" target="_blank">\n        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pait">\n    </a>\n    <a href="https://pypi.org/project/pait/" target="_blank">\n        <img alt="PyPI" src="https://img.shields.io/pypi/v/pait">\n    </a>\n</p>\n<p align="center">\n    <a href="https://github.com/so1n/pait/actions?query=event%3Apush+branch%3Amaster" target="_blank">\n        <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/so1n/pait/python-package.yml">\n    </a>\n    <a href="https://github.com/so1n/pait/releases" target="_blank">\n        <img alt="GitHub release (release name instead of tag name)" src="https://img.shields.io/github/v/release/so1n/pait?include_prereleases">\n    </a>\n    <a href="https://github.com/so1n/pait/actions?query=event%3Apush+branch%3Amaster" target="_blank">\n        <img src="https://github.com/so1n/pait/actions/workflows/python-package.yml/badge.svg?event=push&branch=master" alt="Test">\n    </a>\n</p>\n<p align="center">\n    <a href="https://github.com/so1n/pait/tree/master/example" target="_blank">\n        <img src="https://img.shields.io/badge/Support%20framework-Flask%2CSanic%2CStarlette%2CTornado-brightgreen" alt="Support framework">\n    </a>\n</p>\n\n\n---\n**Documentation**: [https://so1n.me/pait/](https://so1n.me/pait/)\n\n**中文文档**: [https://so1n.me/pait-zh-doc/](https://so1n.me/pait-zh-doc/)\n\n---\n\n# Warning\nThere are changes between the current version and the 0.8 version of the API, For more information, please refer to [1.0.0version change](https://github.com/so1n/pait/blob/master/CHANGELOG.md)\n\n# pait\n\nPait is an api tool that can be used in any python web framework, the features provided are as follows:\n - [x] Parameter checksum automatic conversion (parameter check depends on `Pydantic`)\n - [x] Parameter dependency verification\n - [x] Automatically generate openapi files\n - [x] Swagger, Redoc, Rapidoc, Elements, OpenAPI route\n - [x] gRPC Gateway route\n - [x] TestClient support, support response result verification\n - [x] Support for plugin extensions, such as the Mock plugin, CheckResponse Plugin, Cache Response Plugin\n - [ ] WebSocket support\n - [ ] Auto API Test support\n\n\n> Note:\n>\n> - mypy check 100%\n>\n> - python version >= 3.7 (support postponed annotations)\n\n\n\n# Installation\n```Bash\npip install pait --pre\n```\nIf want to use the gRPC gateway feature, need to add a \'grpc\' dependency:\n```bash\npip install pait[grpc] --pre\n```\n# Simple Example\n```python\nfrom typing import Type\nimport uvicorn  # type: ignore\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\n\nfrom pait.app.starlette import pait\nfrom pait.field import Body\nfrom pait.openapi.doc_route import add_doc_route\nfrom pait.model.response import JsonResponseModel\nfrom pydantic import BaseModel, Field\n\n\nclass DemoResponseModel(JsonResponseModel):\n    """demo post api response model"""\n    class ResponseModel(BaseModel):\n        uid: int = Field()\n        user_name: str = Field()\n\n    description: str = "demo response"\n    response_data: Type[BaseModel] = ResponseModel\n\n\n@pait(response_model_list=[DemoResponseModel])\nasync def demo_post(\n    uid: int = Body.i(description="user id", gt=10, lt=1000),\n    user_name: str = Body.i(description="user name", min_length=2, max_length=4)\n) -> JSONResponse:\n    return JSONResponse({\'uid\': uid, \'user_name\': user_name})\n\n\napp = Starlette(routes=[Route(\'/api\', demo_post, methods=[\'POST\'])])\nadd_doc_route(app)\nuvicorn.run(app)\n```\nSee [documentation](https://so1n.me/pait/) for more features\n\n# Support Web framework\n\n| Framework | Description            |\n|-----------|------------------------|\n| Flask     | All features supported |\n| Sanic     | All features supported |\n| Starlette | All features supported |\n| Tornado   | All features supported |\n| Django    | Coming soon            |\n\n\nIf the web framework is not supported(which you are using).\n\nCan be modified sync web framework according to [pait.app.flask](https://github.com/so1n/pait/blob/master/pait/app/flask.py)\n\nCan be modified async web framework according to [pait.app.starlette](https://github.com/so1n/pait/blob/master/pait/app/starlette.py)\n\n# Performance\nFor the parameter validation and transformation feature, Pait is mainly responsible for injecting the request data dependency into the `Pydantic` model, and then the `Pydanitc` verifies and transforms the data.\n\nThe time consumed by this process <=0.0003 (s), for benchmarks data and subsequent optimization, see [#27](https://github.com/so1n/pait/issues/27)\n\n\n# Full example\nFor more complete examples, please refer to [example](https://github.com/so1n/pait/tree/master/example)\n',
     'author': 'So1n',
     'author_email': 'so1n897046026@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/so1n/pait',
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 'pait.app.starlette.adapter', 'pait.app.starlette.plugin',
 'pait.app.starlette.security', 'pait.app.tornado', 'pait.app.tornado.adapter',
 'pait.app.tornado.plugin', 'pait.app.tornado.security', 'pait.extra',
 'pait.model', 'pait.openapi', 'pait.param_handle', 'pait.plugin', 'pait.util']
 package_data = \ {'': ['*']} install_requires = \ ['any-api>=0.1.0.4,<0.2.0.0',
 'pydantic>=1.7.3,<2.0.0', 'typing-extensions>=4.1.1,<5.0.0'] extras_require = \
 {'all': ['redis>=4.2.2,<5.0.0'], 'redis': ['redis>=4.2.2,<5.0.0']} setup_kwargs
-= { 'name': 'pait', 'version': '1.0.0a8', 'description': 'Pait is a Python api
+= { 'name': 'pait', 'version': '1.0.0a9', 'description': 'Pait is a Python api
 tool. Pait enables your Python web framework to have type checking, parameter
 type conversion, interface document generation and can display your documents
 through Redoc or Swagger (power by inspect, pydantic)', 'long_description': '!
 [](https://cdn.jsdelivr.net/gh/so1n/so1n_blog_photo@master/blog_photo/
 1652600629491%E6%9C%AA%E5%91%BD%E5%90%8D.jpg)\n
 \n Pait(Ï tool) - Python Modern API Tools, easier to use web frameworks/write
                                  API routing\n
```

### Comparing `pait-1.0.0a8/PKG-INFO` & `pait-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pait
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Pait is a Python api tool. Pait enables your Python web framework to have type checking, parameter type conversion, interface document generation and can display your documents through Redoc or Swagger (power by inspect, pydantic)
 Home-page: https://github.com/so1n/pait
 License: Apache Software License
 Author: So1n
 Author-email: so1n897046026@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

