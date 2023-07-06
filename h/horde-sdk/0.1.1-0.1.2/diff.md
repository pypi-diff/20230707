# Comparing `tmp/horde_sdk-0.1.1.tar.gz` & `tmp/horde_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horde_sdk-0.1.1.tar", last modified: Thu Jul  6 22:38:23 2023, max compression
+gzip compressed data, was "horde_sdk-0.1.2.tar", last modified: Thu Jul  6 22:40:46 2023, max compression
```

## Comparing `horde_sdk-0.1.1.tar` & `horde_sdk-0.1.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.239290 horde_sdk-0.1.1/
--rw-rw-rw-   0        0        0    35164 2023-03-31 20:26:08.000000 horde_sdk-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      139 2023-07-06 22:38:14.000000 horde_sdk-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    41017 2023-07-06 22:38:23.238288 horde_sdk-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      600 2023-07-06 22:29:03.000000 horde_sdk-0.1.1/README.md
--rw-rw-rw-   0        0        0     1571 2023-07-06 22:37:17.000000 horde_sdk-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 22:38:23.239290 horde_sdk-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       55 2023-07-04 14:28:55.000000 horde_sdk-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.128708 horde_sdk-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.150282 horde_sdk-0.1.1/src/horde_sdk/
--rw-rw-rw-   0        0        0       80 2023-03-31 20:20:58.000000 horde_sdk-0.1.1/src/horde_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.172891 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/
--rw-rw-rw-   0        0        0      986 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/__init__.py
--rw-rw-rw-   0        0        0     2284 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/ai_horde_client.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.176891 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/
--rw-rw-rw-   0        0        0        0 2023-07-03 23:30:55.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/__init__.py
--rw-rw-rw-   0        0        0      429 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/_base.py
--rw-rw-rw-   0        0        0     3090 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/_shared.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.184195 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/
--rw-rw-rw-   0        0        0      634 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/__init__.py
--rw-rw-rw-   0        0        0     2236 2023-07-06 22:27:43.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/_async.py
--rw-rw-rw-   0        0        0     2400 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/_check.py
--rw-rw-rw-   0        0        0     6423 2023-07-06 22:27:43.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/_pop.py
--rw-rw-rw-   0        0        0     2870 2023-07-06 22:27:43.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/_status.py
--rw-rw-rw-   0        0        0     1689 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/_submit.py
--rw-rw-rw-   0        0        0     1109 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/stats.py
--rw-rw-rw-   0        0        0      669 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/consts.py
--rw-rw-rw-   0        0        0     2490 2023-07-06 22:32:55.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/endpoints.py
--rw-rw-rw-   0        0        0     1572 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/fields.py
--rw-rw-rw-   0        0        0      385 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/metadata.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.185197 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/utils/
--rw-rw-rw-   0        0        0     9016 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/utils/swagger.py
--rw-rw-rw-   0        0        0     1005 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/consts.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.195713 horde_sdk-0.1.1/src/horde_sdk/generic_api/
--rw-rw-rw-   0        0        0      722 2023-07-04 14:29:22.000000 horde_sdk-0.1.1/src/horde_sdk/generic_api/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-07-06 22:27:43.000000 horde_sdk-0.1.1/src/horde_sdk/generic_api/_error.py
--rw-rw-rw-   0        0        0      676 2023-07-04 15:25:34.000000 horde_sdk-0.1.1/src/horde_sdk/generic_api/_reflection.py
--rw-rw-rw-   0        0        0     3571 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/generic_api/apimodels.py
--rw-rw-rw-   0        0        0     1237 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/generic_api/endpoints.py
--rw-rw-rw-   0        0        0    10583 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/generic_api/generic_client.py
--rw-rw-rw-   0        0        0      799 2023-07-05 21:42:10.000000 horde_sdk-0.1.1/src/horde_sdk/generic_api/metadata.py
--rw-rw-rw-   0        0        0      466 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/models.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.202755 horde_sdk-0.1.1/src/horde_sdk/ratings_api/
--rw-rw-rw-   0        0        0      853 2023-07-04 15:25:51.000000 horde_sdk-0.1.1/src/horde_sdk/ratings_api/__init__.py
--rw-rw-rw-   0        0        0     8599 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ratings_api/apimodels.py
--rw-rw-rw-   0        0        0      573 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/src/horde_sdk/ratings_api/endpoints.py
--rw-rw-rw-   0        0        0      886 2023-07-04 14:29:22.000000 horde_sdk-0.1.1/src/horde_sdk/ratings_api/metadata.py
--rw-rw-rw-   0        0        0      561 2023-07-04 14:29:22.000000 horde_sdk-0.1.1/src/horde_sdk/ratings_api/ratings_client.py
--rw-rw-rw-   0        0        0      433 2023-07-03 23:40:43.000000 horde_sdk-0.1.1/src/horde_sdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.164794 horde_sdk-0.1.1/src/horde_sdk.egg-info/
--rw-rw-rw-   0        0        0    41017 2023-07-06 22:38:23.000000 horde_sdk-0.1.1/src/horde_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2794 2023-07-06 22:38:23.000000 horde_sdk-0.1.1/src/horde_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 22:38:23.000000 horde_sdk-0.1.1/src/horde_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-06 22:38:23.000000 horde_sdk-0.1.1/src/horde_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 22:38:23.000000 horde_sdk-0.1.1/src/horde_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.212271 horde_sdk-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-06 22:20:28.000000 horde_sdk-0.1.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.218780 horde_sdk-0.1.1/tests/ai_horde_api/
--rw-rw-rw-   0        0        0        0 2023-07-06 22:18:04.000000 horde_sdk-0.1.1/tests/ai_horde_api/__init__.py
--rw-rw-rw-   0        0        0     3885 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/ai_horde_api/test_ai_horde_api_models.py
--rw-rw-rw-   0        0        0     1860 2023-07-06 21:50:09.000000 horde_sdk-0.1.1/tests/ai_horde_api/test_api_calls.py
--rw-rw-rw-   0        0        0     2824 2023-07-06 21:50:09.000000 horde_sdk-0.1.1/tests/ai_horde_api/test_dynamically_validate_against_swagger.py
--rw-rw-rw-   0        0        0      819 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/ai_horde_api/test_swagger.py
--rw-rw-rw-   0        0        0      708 2023-07-06 21:50:09.000000 horde_sdk-0.1.1/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.221782 horde_sdk-0.1.1/tests/test_data/
--rw-rw-rw-   0        0        0       93 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/RequestErrorResponse.json
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.134707 horde_sdk-0.1.1/tests/test_data/ai_horde_api/
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.229824 horde_sdk-0.1.1/tests/test_data/ai_horde_api/example_responses/
--rw-rw-rw-   0        0        0       69 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/ai_horde_api/example_responses/ImageGenerateAsyncResponse.json
--rw-rw-rw-   0        0        0      219 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/ai_horde_api/example_responses/ImageGenerateCheckResponse.json
--rw-rw-rw-   0        0        0     1531 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/ai_horde_api/example_responses/ImageGenerateJobResponse.json
--rw-rw-rw-   0        0        0      510 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/ai_horde_api/example_responses/ImageGenerateStatusResponse.json
--rw-rw-rw-   0        0        0    18362 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/ai_horde_api/example_responses/StatsModelsResponse.json
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.230824 horde_sdk-0.1.1/tests/test_data/ai_horde_api/production_responses/
--rw-rw-rw-   0        0        0    20811 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.135710 horde_sdk-0.1.1/tests/test_data/ratings_api/
-drwxrwxrwx   0        0        0        0 2023-07-06 22:38:23.236826 horde_sdk-0.1.1/tests/test_data/ratings_api/example_responses/
--rw-rw-rw-   0        0        0      666 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json
--rw-rw-rw-   0        0        0      251 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/ratings_api/example_responses/UserCheckResponse.json
--rw-rw-rw-   0        0        0    64737 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json
--rw-rw-rw-   0        0        0     5726 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/ratings_api/example_responses/UserValidateResponse.json
--rw-rw-rw-   0        0        0   237970 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_data/swagger.json
--rw-rw-rw-   0        0        0     3396 2023-07-06 22:28:39.000000 horde_sdk-0.1.1/tests/test_dynamically_check_apimodels.py
--rw-rw-rw-   0        0        0      302 2023-07-05 21:06:36.000000 horde_sdk-0.1.1/tests/test_generic.py
--rw-rw-rw-   0        0        0     1697 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_ratings_api_models.py
--rw-rw-rw-   0        0        0      466 2023-07-06 20:14:23.000000 horde_sdk-0.1.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.449876 horde_sdk-0.1.2/
+-rw-rw-rw-   0        0        0    35164 2023-03-31 20:26:08.000000 horde_sdk-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      139 2023-07-06 22:38:14.000000 horde_sdk-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    41660 2023-07-06 22:40:46.448873 horde_sdk-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-07-06 22:29:03.000000 horde_sdk-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1593 2023-07-06 22:40:36.000000 horde_sdk-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 22:40:46.449876 horde_sdk-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       55 2023-07-04 14:28:55.000000 horde_sdk-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.352225 horde_sdk-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.373150 horde_sdk-0.1.2/src/horde_sdk/
+-rw-rw-rw-   0        0        0       80 2023-03-31 20:20:58.000000 horde_sdk-0.1.2/src/horde_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.396176 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/
+-rw-rw-rw-   0        0        0      986 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/__init__.py
+-rw-rw-rw-   0        0        0     2284 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/ai_horde_client.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.401177 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/
+-rw-rw-rw-   0        0        0        0 2023-07-03 23:30:55.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/_base.py
+-rw-rw-rw-   0        0        0     3090 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/_shared.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.407277 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/
+-rw-rw-rw-   0        0        0      634 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/__init__.py
+-rw-rw-rw-   0        0        0     2236 2023-07-06 22:27:43.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/_async.py
+-rw-rw-rw-   0        0        0     2400 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/_check.py
+-rw-rw-rw-   0        0        0     6423 2023-07-06 22:27:43.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/_pop.py
+-rw-rw-rw-   0        0        0     2870 2023-07-06 22:27:43.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/_status.py
+-rw-rw-rw-   0        0        0     1689 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/_submit.py
+-rw-rw-rw-   0        0        0     1109 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/stats.py
+-rw-rw-rw-   0        0        0      669 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/consts.py
+-rw-rw-rw-   0        0        0     2490 2023-07-06 22:32:55.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/endpoints.py
+-rw-rw-rw-   0        0        0     1572 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/fields.py
+-rw-rw-rw-   0        0        0      385 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.408276 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/utils/
+-rw-rw-rw-   0        0        0     9016 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/utils/swagger.py
+-rw-rw-rw-   0        0        0     1005 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.416788 horde_sdk-0.1.2/src/horde_sdk/generic_api/
+-rw-rw-rw-   0        0        0      722 2023-07-04 14:29:22.000000 horde_sdk-0.1.2/src/horde_sdk/generic_api/__init__.py
+-rw-rw-rw-   0        0        0     1520 2023-07-06 22:27:43.000000 horde_sdk-0.1.2/src/horde_sdk/generic_api/_error.py
+-rw-rw-rw-   0        0        0      676 2023-07-04 15:25:34.000000 horde_sdk-0.1.2/src/horde_sdk/generic_api/_reflection.py
+-rw-rw-rw-   0        0        0     3571 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/generic_api/apimodels.py
+-rw-rw-rw-   0        0        0     1237 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/generic_api/endpoints.py
+-rw-rw-rw-   0        0        0    10583 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/generic_api/generic_client.py
+-rw-rw-rw-   0        0        0      799 2023-07-05 21:42:10.000000 horde_sdk-0.1.2/src/horde_sdk/generic_api/metadata.py
+-rw-rw-rw-   0        0        0      466 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/models.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.422293 horde_sdk-0.1.2/src/horde_sdk/ratings_api/
+-rw-rw-rw-   0        0        0      853 2023-07-04 15:25:51.000000 horde_sdk-0.1.2/src/horde_sdk/ratings_api/__init__.py
+-rw-rw-rw-   0        0        0     8599 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ratings_api/apimodels.py
+-rw-rw-rw-   0        0        0      573 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/src/horde_sdk/ratings_api/endpoints.py
+-rw-rw-rw-   0        0        0      886 2023-07-04 14:29:22.000000 horde_sdk-0.1.2/src/horde_sdk/ratings_api/metadata.py
+-rw-rw-rw-   0        0        0      561 2023-07-04 14:29:22.000000 horde_sdk-0.1.2/src/horde_sdk/ratings_api/ratings_client.py
+-rw-rw-rw-   0        0        0      433 2023-07-03 23:40:43.000000 horde_sdk-0.1.2/src/horde_sdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.389664 horde_sdk-0.1.2/src/horde_sdk.egg-info/
+-rw-rw-rw-   0        0        0    41660 2023-07-06 22:40:46.000000 horde_sdk-0.1.2/src/horde_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2794 2023-07-06 22:40:46.000000 horde_sdk-0.1.2/src/horde_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 22:40:46.000000 horde_sdk-0.1.2/src/horde_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-06 22:40:46.000000 horde_sdk-0.1.2/src/horde_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 22:40:46.000000 horde_sdk-0.1.2/src/horde_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.428299 horde_sdk-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-06 22:20:28.000000 horde_sdk-0.1.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.434362 horde_sdk-0.1.2/tests/ai_horde_api/
+-rw-rw-rw-   0        0        0        0 2023-07-06 22:18:04.000000 horde_sdk-0.1.2/tests/ai_horde_api/__init__.py
+-rw-rw-rw-   0        0        0     3885 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/ai_horde_api/test_ai_horde_api_models.py
+-rw-rw-rw-   0        0        0     1860 2023-07-06 21:50:09.000000 horde_sdk-0.1.2/tests/ai_horde_api/test_api_calls.py
+-rw-rw-rw-   0        0        0     2824 2023-07-06 21:50:09.000000 horde_sdk-0.1.2/tests/ai_horde_api/test_dynamically_validate_against_swagger.py
+-rw-rw-rw-   0        0        0      819 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/ai_horde_api/test_swagger.py
+-rw-rw-rw-   0        0        0      708 2023-07-06 21:50:09.000000 horde_sdk-0.1.2/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.436361 horde_sdk-0.1.2/tests/test_data/
+-rw-rw-rw-   0        0        0       93 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/RequestErrorResponse.json
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.358608 horde_sdk-0.1.2/tests/test_data/ai_horde_api/
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.442361 horde_sdk-0.1.2/tests/test_data/ai_horde_api/example_responses/
+-rw-rw-rw-   0        0        0       69 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/ai_horde_api/example_responses/ImageGenerateAsyncResponse.json
+-rw-rw-rw-   0        0        0      219 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/ai_horde_api/example_responses/ImageGenerateCheckResponse.json
+-rw-rw-rw-   0        0        0     1531 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/ai_horde_api/example_responses/ImageGenerateJobResponse.json
+-rw-rw-rw-   0        0        0      510 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/ai_horde_api/example_responses/ImageGenerateStatusResponse.json
+-rw-rw-rw-   0        0        0    18362 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/ai_horde_api/example_responses/StatsModelsResponse.json
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.442866 horde_sdk-0.1.2/tests/test_data/ai_horde_api/production_responses/
+-rw-rw-rw-   0        0        0    20811 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.358608 horde_sdk-0.1.2/tests/test_data/ratings_api/
+drwxrwxrwx   0        0        0        0 2023-07-06 22:40:46.447872 horde_sdk-0.1.2/tests/test_data/ratings_api/example_responses/
+-rw-rw-rw-   0        0        0      666 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json
+-rw-rw-rw-   0        0        0      251 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/ratings_api/example_responses/UserCheckResponse.json
+-rw-rw-rw-   0        0        0    64737 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json
+-rw-rw-rw-   0        0        0     5726 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/ratings_api/example_responses/UserValidateResponse.json
+-rw-rw-rw-   0        0        0   237970 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_data/swagger.json
+-rw-rw-rw-   0        0        0     3396 2023-07-06 22:28:39.000000 horde_sdk-0.1.2/tests/test_dynamically_check_apimodels.py
+-rw-rw-rw-   0        0        0      302 2023-07-05 21:06:36.000000 horde_sdk-0.1.2/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1697 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_ratings_api_models.py
+-rw-rw-rw-   0        0        0      466 2023-07-06 20:14:23.000000 horde_sdk-0.1.2/tests/test_utils.py
```

### Comparing `horde_sdk-0.1.1/LICENSE` & `horde_sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/PKG-INFO` & `horde_sdk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horde_sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python toolkit for interacting with the horde APIs, services, and ecosystem.
 Author-email: tazlin <tazlin.on.github@gmail.com>, db0 <mail@dbzer0.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -667,8 +667,19 @@
         
 Project-URL: Homepage, https://github.com/Haidra-Org/horde-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# AI-Horde-Shared-Models
+
+With the power of pydantic, you can simplify interfacing with the [AI-Horde's suite of APIs](https://github.com/db0/AI-Horde). Whether you want to request your own images, or roll your own worker software, this package may suit your needs for anything horde related.
+
+## AI-Horde
+`TODO`
+
+## Ratings API
+There is currently some support for the [Image Ratings](https://dbzer0.com/blog/the-image-ratings-are-flooding-in/) API that are rating images from the [DiffusionDB](https://poloclub.github.io/diffusiondb/) dataset. See `example.py` for an idea of how to start.
```

### Comparing `horde_sdk-0.1.1/README.md` & `horde_sdk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/pyproject.toml` & `horde_sdk-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "horde_sdk"
-version = "0.1.1"
+version = "0.1.2"
 description = "A python toolkit for interacting with the horde APIs, services, and ecosystem."
 authors = [
     {name = "tazlin", email = "tazlin.on.github@gmail.com"},
     {name = "db0", email = "mail@dbzer0.com"},
 ]
+readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "pydantic",
     "requests",
     "StrEnum",
     "loguru",
 ]
```

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/__init__.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/__init__.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/ai_horde_client.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/ai_horde_client.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/_shared.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/_shared.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/__init__.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/_async.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/_async.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/_check.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/_check.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/_pop.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/_pop.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/_status.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/_status.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/generate/_submit.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/generate/_submit.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/apimodels/stats.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/apimodels/stats.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/consts.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/consts.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/endpoints.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/fields.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/fields.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ai_horde_api/utils/swagger.py` & `horde_sdk-0.1.2/src/horde_sdk/ai_horde_api/utils/swagger.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/consts.py` & `horde_sdk-0.1.2/src/horde_sdk/consts.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/generic_api/__init__.py` & `horde_sdk-0.1.2/src/horde_sdk/generic_api/__init__.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/generic_api/_error.py` & `horde_sdk-0.1.2/src/horde_sdk/generic_api/_error.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/generic_api/_reflection.py` & `horde_sdk-0.1.2/src/horde_sdk/generic_api/_reflection.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/generic_api/apimodels.py` & `horde_sdk-0.1.2/src/horde_sdk/generic_api/apimodels.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/generic_api/endpoints.py` & `horde_sdk-0.1.2/src/horde_sdk/generic_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/generic_api/generic_client.py` & `horde_sdk-0.1.2/src/horde_sdk/generic_api/generic_client.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/generic_api/metadata.py` & `horde_sdk-0.1.2/src/horde_sdk/generic_api/metadata.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ratings_api/__init__.py` & `horde_sdk-0.1.2/src/horde_sdk/ratings_api/__init__.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ratings_api/apimodels.py` & `horde_sdk-0.1.2/src/horde_sdk/ratings_api/apimodels.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ratings_api/endpoints.py` & `horde_sdk-0.1.2/src/horde_sdk/ratings_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ratings_api/metadata.py` & `horde_sdk-0.1.2/src/horde_sdk/ratings_api/metadata.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk/ratings_api/ratings_client.py` & `horde_sdk-0.1.2/src/horde_sdk/ratings_api/ratings_client.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/src/horde_sdk.egg-info/PKG-INFO` & `horde_sdk-0.1.2/src/horde_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horde-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python toolkit for interacting with the horde APIs, services, and ecosystem.
 Author-email: tazlin <tazlin.on.github@gmail.com>, db0 <mail@dbzer0.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -667,8 +667,19 @@
         
 Project-URL: Homepage, https://github.com/Haidra-Org/horde-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# AI-Horde-Shared-Models
+
+With the power of pydantic, you can simplify interfacing with the [AI-Horde's suite of APIs](https://github.com/db0/AI-Horde). Whether you want to request your own images, or roll your own worker software, this package may suit your needs for anything horde related.
+
+## AI-Horde
+`TODO`
+
+## Ratings API
+There is currently some support for the [Image Ratings](https://dbzer0.com/blog/the-image-ratings-are-flooding-in/) API that are rating images from the [DiffusionDB](https://poloclub.github.io/diffusiondb/) dataset. See `example.py` for an idea of how to start.
```

### Comparing `horde_sdk-0.1.1/src/horde_sdk.egg-info/SOURCES.txt` & `horde_sdk-0.1.2/src/horde_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/ai_horde_api/test_ai_horde_api_models.py` & `horde_sdk-0.1.2/tests/ai_horde_api/test_ai_horde_api_models.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/ai_horde_api/test_api_calls.py` & `horde_sdk-0.1.2/tests/ai_horde_api/test_api_calls.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/ai_horde_api/test_dynamically_validate_against_swagger.py` & `horde_sdk-0.1.2/tests/ai_horde_api/test_dynamically_validate_against_swagger.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/ai_horde_api/test_swagger.py` & `horde_sdk-0.1.2/tests/ai_horde_api/test_swagger.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/conftest.py` & `horde_sdk-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/test_data/ai_horde_api/example_responses/ImageGenerateJobResponse.json` & `horde_sdk-0.1.2/tests/test_data/ai_horde_api/example_responses/ImageGenerateJobResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/test_data/ai_horde_api/example_responses/StatsModelsResponse.json` & `horde_sdk-0.1.2/tests/test_data/ai_horde_api/example_responses/StatsModelsResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json` & `horde_sdk-0.1.2/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json` & `horde_sdk-0.1.2/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json` & `horde_sdk-0.1.2/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/test_data/ratings_api/example_responses/UserValidateResponse.json` & `horde_sdk-0.1.2/tests/test_data/ratings_api/example_responses/UserValidateResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/test_data/swagger.json` & `horde_sdk-0.1.2/tests/test_data/swagger.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/test_dynamically_check_apimodels.py` & `horde_sdk-0.1.2/tests/test_dynamically_check_apimodels.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.1.1/tests/test_ratings_api_models.py` & `horde_sdk-0.1.2/tests/test_ratings_api_models.py`

 * *Files identical despite different names*

