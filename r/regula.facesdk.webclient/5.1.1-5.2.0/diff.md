# Comparing `tmp/regula.facesdk.webclient-5.1.1.tar.gz` & `tmp/regula.facesdk.webclient-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regula.facesdk.webclient-5.1.1.tar", last modified: Tue Apr 11 02:08:46 2023, max compression
+gzip compressed data, was "regula.facesdk.webclient-5.2.0.tar", last modified: Fri Jul  7 09:45:35 2023, max compression
```

## Comparing `regula.facesdk.webclient-5.1.1.tar` & `regula.facesdk.webclient-5.2.0.tar`

### file list

```diff
@@ -1,126 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.611455 regula.facesdk.webclient-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-11 02:08:46.611455 regula.facesdk.webclient-5.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.587455 regula.facesdk.webclient-5.1.1/regula/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.591455 regula.facesdk.webclient-5.1.1/regula/facesdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.591455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.591455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      309 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.591455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)      193 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/group_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2083 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/matching_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/person_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/search_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.591455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)      280 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/detect_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/match_image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/match_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.595455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.595455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47391 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/liveness_2_0_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/liveness_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/matching_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    68455 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/person_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27677 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.595455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.611455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection_face.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_align_type_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_align_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_config_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_rectangular.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_sdk_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_sdk_result_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/faces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/faces_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_page_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_to_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_fields_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_page_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/liveness_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request_all_of_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response_all_of_detections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/operation_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/output_image_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_with_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_with_images_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/persons_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/persons_page_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/process_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_config_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_details_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/recognize_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/recognize_image_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_person_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/transaction_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/transaction_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/update_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    82471 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.611455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.587455 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-11 02:08:46.000000 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-11 02:08:46.000000 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:08:46.000000 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-11 02:08:46.000000 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 02:08:46.000000 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:08:46.611455 regula.facesdk.webclient-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.942441 regula.facesdk.webclient-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-07 09:45:35.942441 regula.facesdk.webclient-5.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.914441 regula.facesdk.webclient-5.2.0/regula/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.918441 regula.facesdk.webclient-5.2.0/regula/facesdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.918441 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.918441 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      309 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.918441 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      193 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/group_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2083 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/matching_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/person_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/search_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.918441 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      280 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/models/detect_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/models/match_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/models/match_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.922441 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.922441 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/diagnostics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47689 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/liveness_2_0_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/liveness_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20063 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/matching_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62036 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/person_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27677 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.922441 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.942441 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detect_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detect_request_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detect_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detect_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detect_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detection_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detection_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_align_type_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_image_quality_align_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_image_quality_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_image_quality_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_quality_config_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_quality_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_quality_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_rectangular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_sdk_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_sdk_result_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/faces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/faces_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/group_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/group_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/group_page_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/group_to_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/image_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/image_fields_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/image_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/image_page_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/image_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/liveness_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_request_all_of_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_response_all_of_detections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_image_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_image_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/operation_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/output_image_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person_created_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person_with_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person_with_images_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/persons_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/persons_page_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/process_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/quality_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/quality_config_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/quality_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/quality_details_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/quality_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/recognize_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/recognize_image_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/resize_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_bad_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_parameters_create_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_person_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/transaction_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/transaction_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/update_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82471 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.942441 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:45:35.914441 regula.facesdk.webclient-5.2.0/regula.facesdk.webclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-07 09:45:35.000000 regula.facesdk.webclient-5.2.0/regula.facesdk.webclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-07 09:45:35.000000 regula.facesdk.webclient-5.2.0/regula.facesdk.webclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:45:35.000000 regula.facesdk.webclient-5.2.0/regula.facesdk.webclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-07 09:45:35.000000 regula.facesdk.webclient-5.2.0/regula.facesdk.webclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 09:45:35.000000 regula.facesdk.webclient-5.2.0/regula.facesdk.webclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:45:35.942441 regula.facesdk.webclient-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 09:44:32.000000 regula.facesdk.webclient-5.2.0/setup.py
```

### Comparing `regula.facesdk.webclient-5.1.1/PKG-INFO` & `regula.facesdk.webclient-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regula.facesdk.webclient
-Version: 5.1.1
+Version: 5.2.0
 Summary: Regula's FaceSDK web python client
 Home-page: https://mobile.regulaforensics.com
 Author: Regula Forensics, Inc.
 Author-email: support@regulaforensics.com
 Keywords: face recognition,facesdk,regulaforensics,regula
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `regula.facesdk.webclient-5.1.1/README.md` & `regula.facesdk.webclient-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/__init__.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/group_api.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/group_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
     def create_group(self, group_name: str, metadata=None, **kwargs) -> Group:
         if metadata is None:
             metadata = {}
         group_to_create = GroupToCreate(group_name, metadata)
         return super().create_group(group_to_create, **kwargs)
 
-    def delete_group(self, group_id: int, **kwargs) -> None:
+    def delete_group(self, group_id: str, **kwargs) -> None:
         return super().delete_group(group_id, **kwargs)
 
     def get_all_groups(self, page: int, size: int, **kwargs) -> GroupPage:
         return super().get_all_groups(page, size, **kwargs)
 
-    def get_all_persons_by_group_id(self, page: int, size: int, group_id: int, **kwargs) -> PersonsPage:
+    def get_all_persons_by_group_id(self, page: int, size: int, group_id: str, **kwargs) -> PersonsPage:
         return super().get_all_persons_by_group_id(page, size, group_id, **kwargs)
 
-    def get_group(self, group_id: int, **kwargs) -> Group:
+    def get_group(self, group_id: str, **kwargs) -> Group:
         return super().get_group(group_id, **kwargs)
 
-    def update_group(self, group_id: int, group_to_create: GroupToCreate, **kwargs) -> None:
+    def update_group(self, group_id: str, group_to_create: GroupToCreate, **kwargs) -> None:
         return super().update_group(group_id, group_to_create, **kwargs)
 
-    def update_persons_in_group(self, group_id: int, update_group: UpdateGroup, **kwargs) -> None:
+    def update_persons_in_group(self, group_id: str, update_group: UpdateGroup, **kwargs) -> None:
         return super().update_persons_in_group(group_id, update_group, **kwargs)
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/matching_api.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/matching_api.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/person_api.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/person_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,45 +4,41 @@
 from regula.facesdk.webclient.gen.api.person_api import PersonApi as GenPersonApi
 from regula.facesdk.webclient.gen.model.image import Image
 from regula.facesdk.webclient.gen.model.image_fields import ImageFields
 from regula.facesdk.webclient.gen.model.image_fields_image import ImageFieldsImage
 from regula.facesdk.webclient.gen.model.image_page import ImagePage
 from regula.facesdk.webclient.gen.model.person import Person
 from regula.facesdk.webclient.gen.model.person_fields import PersonFields
-from regula.facesdk.webclient.gen.model.persons_page import PersonsPage
 
 
 class PersonApi(GenPersonApi):
     def __init__(self, api_client: ApiClient):
         super().__init__(api_client)
 
-    def add_image_to_person(self, person_id: int, content: bytes, content_type: str = None, **kwargs) -> Image:
+    def add_image_to_person(self, person_id: str, content: bytes, content_type: str = None, **kwargs) -> Image:
         base_image = base64.b64encode(content).decode("UTF-8")
         image = ImageFields(ImageFieldsImage(content_type, base_image))
         return super().add_image_to_person(person_id, image, **kwargs)
 
     def create_person(self, person_fields: PersonFields, **kwargs) -> Person:
         return super().create_person(person_fields, **kwargs)
 
-    def delete_image_of_person(self, image_id: int, person_id: int, **kwargs) -> None:
+    def delete_image_of_person(self, image_id: str, person_id: str, **kwargs) -> None:
         return super().delete_image_of_person(image_id, person_id, **kwargs)
 
-    def delete_person(self, person_id: int, **kwargs) -> None:
+    def delete_person(self, person_id: str, **kwargs) -> None:
         return super().delete_person(person_id, **kwargs)
 
-    def get_all_groups_by_person_id(self, page: int, size: int, person_id: int, **kwargs):
+    def get_all_groups_by_person_id(self, page: int, size: int, person_id: str, **kwargs):
         return super().get_all_groups_by_person_id(page, size, person_id)
 
-    def get_all_images_by_person_id(self, page: int, size: int, person_id: int, **kwargs) -> ImagePage:
+    def get_all_images_by_person_id(self, page: int, size: int, person_id: str, **kwargs) -> ImagePage:
         return super().get_all_images_by_person_id(page, size, person_id, **kwargs)
 
-    def get_all_persons(self, page: int, size: int, **kwargs) -> PersonsPage:
-        return super().get_all_persons(page, size, **kwargs)
-
-    def get_image_of_person(self, image_id: int, person_id: int, **kwargs):
+    def get_image_of_person(self, image_id: str, person_id: str, **kwargs):
         return super().get_image_of_person(image_id, person_id, **kwargs)
 
-    def get_person(self, person_id: int, **kwargs) -> Person:
+    def get_person(self, person_id: str, **kwargs) -> Person:
         return super().get_person(person_id, **kwargs)
 
-    def update_person(self, person_id: int, person_fields: PersonFields, **kwargs) -> None:
+    def update_person(self, person_id: str, person_fields: PersonFields, **kwargs) -> None:
         return super().update_person(person_id, person_fields, **kwargs)
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/sdk.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/sdk.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/search_api.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/api/search_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 
 class SearchApi(GenSearchApi):
     def __init__(self, api_client: ApiClient):
         super().__init__(api_client)
 
     def search(self, search_request: SearchRequest, **kwargs) -> SearchResult:
-        search_request.image.content = base64.b64encode(search_request.image.content).decode("utf-8")
+        search_request.image.content = base64.b64encode(search_request.image.content.encode("UTF-8")).decode("utf-8")
         return super().search(search_request, **kwargs)
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/detect_request.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/models/detect_request.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/match_image.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/models/match_image.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/match_request.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/ext/models/match_request.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/__init__.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/group_api.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/group_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -43,15 +43,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_group(group_to_create, async_req=True)
         >>> result = thread.get()
 
         :param group_to_create: Request body for the group to create. (required)
         :type group_to_create: GroupToCreate
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -74,15 +74,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_group_with_http_info(group_to_create, async_req=True)
         >>> result = thread.get()
 
         :param group_to_create: Request body for the group to create. (required)
         :type group_to_create: GroupToCreate
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -182,16 +182,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_group(group_id, async_req=True)
         >>> result = thread.get()
 
         :param group_id: Group ID. (required)
-        :type group_id: int
-        :param x_request_id:
+        :type group_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -213,16 +213,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_group_with_http_info(group_id, async_req=True)
         >>> result = thread.get()
 
         :param group_id: Group ID. (required)
-        :type group_id: int
-        :param x_request_id:
+        :type group_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -272,15 +272,15 @@
                                                         local_var_params['group_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `group_id` when calling `delete_group`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'group_id' in local_var_params:
-            path_params['group_id'] = local_var_params['group_id']  # noqa: E501
+            path_params['groupId'] = local_var_params['group_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
         if 'x_request_id' in local_var_params:
             header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
@@ -292,15 +292,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/groups/{group_id}', 'DELETE',
+            '/api/groups/{groupId}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
@@ -321,15 +321,15 @@
         >>> thread = api.get_all_groups(page, size, async_req=True)
         >>> result = thread.get()
 
         :param page: The page number to get a list of persons or groups. (required)
         :type page: int
         :param size: The page size with a list of persons or groups, items. (required)
         :type size: int
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -354,15 +354,15 @@
         >>> thread = api.get_all_groups_with_http_info(page, size, async_req=True)
         >>> result = thread.get()
 
         :param page: The page number to get a list of persons or groups. (required)
         :type page: int
         :param size: The page size with a list of persons or groups, items. (required)
         :type size: int
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -469,16 +469,16 @@
         >>> result = thread.get()
 
         :param page: The page number to get a list of persons or groups. (required)
         :type page: int
         :param size: The page size with a list of persons or groups, items. (required)
         :type size: int
         :param group_id: Group ID. (required)
-        :type group_id: int
-        :param x_request_id:
+        :type group_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -504,16 +504,16 @@
         >>> result = thread.get()
 
         :param page: The page number to get a list of persons or groups. (required)
         :type page: int
         :param size: The page size with a list of persons or groups, items. (required)
         :type size: int
         :param group_id: Group ID. (required)
-        :type group_id: int
-        :param x_request_id:
+        :type group_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -573,15 +573,15 @@
                                                         local_var_params['group_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `group_id` when calling `get_all_persons_by_group_id`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'group_id' in local_var_params:
-            path_params['group_id'] = local_var_params['group_id']  # noqa: E501
+            path_params['groupId'] = local_var_params['group_id']  # noqa: E501
 
         query_params = []
         if 'page' in local_var_params and local_var_params['page'] is not None:  # noqa: E501
             query_params.append(('page', local_var_params['page']))  # noqa: E501
         if 'size' in local_var_params and local_var_params['size'] is not None:  # noqa: E501
             query_params.append(('size', local_var_params['size']))  # noqa: E501
 
@@ -597,15 +597,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/groups/{group_id}/persons', 'GET',
+            '/api/groups/{groupId}/persons', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='PersonsPage',  # noqa: E501
@@ -623,16 +623,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_group(group_id, async_req=True)
         >>> result = thread.get()
 
         :param group_id: Group ID. (required)
-        :type group_id: int
-        :param x_request_id:
+        :type group_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -654,16 +654,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_group_with_http_info(group_id, async_req=True)
         >>> result = thread.get()
 
         :param group_id: Group ID. (required)
-        :type group_id: int
-        :param x_request_id:
+        :type group_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -713,15 +713,15 @@
                                                         local_var_params['group_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `group_id` when calling `get_group`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'group_id' in local_var_params:
-            path_params['group_id'] = local_var_params['group_id']  # noqa: E501
+            path_params['groupId'] = local_var_params['group_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
         if 'x_request_id' in local_var_params:
             header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
@@ -733,15 +733,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/groups/{group_id}', 'GET',
+            '/api/groups/{groupId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Group',  # noqa: E501
@@ -759,18 +759,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_group(group_id, group_to_create, async_req=True)
         >>> result = thread.get()
 
         :param group_id: Group ID. (required)
-        :type group_id: int
+        :type group_id: str
         :param group_to_create: Request body for the group to update. (required)
         :type group_to_create: GroupToCreate
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -792,18 +792,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_group_with_http_info(group_id, group_to_create, async_req=True)
         >>> result = thread.get()
 
         :param group_id: Group ID. (required)
-        :type group_id: int
+        :type group_id: str
         :param group_to_create: Request body for the group to update. (required)
         :type group_to_create: GroupToCreate
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -858,15 +858,15 @@
                                                         local_var_params['group_to_create'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `group_to_create` when calling `update_group`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'group_id' in local_var_params:
-            path_params['group_id'] = local_var_params['group_id']  # noqa: E501
+            path_params['groupId'] = local_var_params['group_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
         if 'x_request_id' in local_var_params:
             header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
@@ -884,15 +884,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/groups/{group_id}', 'PUT',
+            '/api/groups/{groupId}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
@@ -910,18 +910,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_persons_in_group(group_id, update_group, async_req=True)
         >>> result = thread.get()
 
         :param group_id: Group ID. (required)
-        :type group_id: int
+        :type group_id: str
         :param update_group: Request body for person IDs to add or remove. (required)
         :type update_group: UpdateGroup
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -943,18 +943,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_persons_in_group_with_http_info(group_id, update_group, async_req=True)
         >>> result = thread.get()
 
         :param group_id: Group ID. (required)
-        :type group_id: int
+        :type group_id: str
         :param update_group: Request body for person IDs to add or remove. (required)
         :type update_group: UpdateGroup
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -1009,15 +1009,15 @@
                                                         local_var_params['update_group'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `update_group` when calling `update_persons_in_group`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'group_id' in local_var_params:
-            path_params['group_id'] = local_var_params['group_id']  # noqa: E501
+            path_params['groupId'] = local_var_params['group_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
         if 'x_request_id' in local_var_params:
             header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
@@ -1035,15 +1035,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/groups/{group_id}/persons', 'PUT',
+            '/api/groups/{groupId}/persons', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/liveness_2_0_api.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/liveness_2_0_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -33,15 +33,15 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def get_liveness_transaction_info(self, transaction_id, **kwargs):  # noqa: E501
-        """liveness  # noqa: E501
+        """Liveness assessment  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_liveness_transaction_info(transaction_id, async_req=True)
         >>> result = thread.get()
 
@@ -62,15 +62,15 @@
                  returns the request thread.
         :rtype: TransactionInfo
         """
         kwargs['_return_http_data_only'] = True
         return self.get_liveness_transaction_info_with_http_info(transaction_id, **kwargs)  # noqa: E501
 
     def get_liveness_transaction_info_with_http_info(self, transaction_id, **kwargs):  # noqa: E501
-        """liveness  # noqa: E501
+        """Liveness assessment  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_liveness_transaction_info_with_http_info(transaction_id, async_req=True)
         >>> result = thread.get()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/liveness_api.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/liveness_api.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/matching_api.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/matching_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -33,25 +33,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def detect(self, detect_request, **kwargs):  # noqa: E501
-        """Detect facial coordinates  # noqa: E501
+        """Detect face, evaluate attributes, assess the portrait quality  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.detect(detect_request, async_req=True)
         >>> result = thread.get()
 
         :param detect_request: (required)
         :type detect_request: DetectRequest
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -64,25 +64,25 @@
                  returns the request thread.
         :rtype: DetectResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.detect_with_http_info(detect_request, **kwargs)  # noqa: E501
 
     def detect_with_http_info(self, detect_request, **kwargs):  # noqa: E501
-        """Detect facial coordinates  # noqa: E501
+        """Detect face, evaluate attributes, assess the portrait quality  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.detect_with_http_info(detect_request, async_req=True)
         >>> result = thread.get()
 
         :param detect_request: (required)
         :type detect_request: DetectRequest
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -173,25 +173,25 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def match(self, match_request, **kwargs):  # noqa: E501
-        """Compare provided face images in all combinations and return the similarity score for each pair.  # noqa: E501
+        """Compare faces in all combinations  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.match(match_request, async_req=True)
         >>> result = thread.get()
 
         :param match_request: (required)
         :type match_request: MatchRequest
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -204,25 +204,25 @@
                  returns the request thread.
         :rtype: MatchResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.match_with_http_info(match_request, **kwargs)  # noqa: E501
 
     def match_with_http_info(self, match_request, **kwargs):  # noqa: E501
-        """Compare provided face images in all combinations and return the similarity score for each pair.  # noqa: E501
+        """Compare faces in all combinations  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.match_with_http_info(match_request, async_req=True)
         >>> result = thread.get()
 
         :param match_request: (required)
         :type match_request: MatchRequest
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -323,15 +323,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.match_and_search(match_and_search_request, async_req=True)
         >>> result = thread.get()
 
         :param match_and_search_request: (required)
         :type match_and_search_request: MatchAndSearchRequest
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -354,15 +354,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.match_and_search_with_http_info(match_and_search_request, async_req=True)
         >>> result = thread.get()
 
         :param match_and_search_request: (required)
         :type match_and_search_request: MatchAndSearchRequest
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/person_api.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/person_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -42,18 +42,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_image_to_person(person_id, image_fields, async_req=True)
         >>> result = thread.get()
 
         :param person_id: Person ID. (required)
-        :type person_id: int
+        :type person_id: str
         :param image_fields: Image to add. (required)
         :type image_fields: ImageFields
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -75,18 +75,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_image_to_person_with_http_info(person_id, image_fields, async_req=True)
         >>> result = thread.get()
 
         :param person_id: Person ID. (required)
-        :type person_id: int
+        :type person_id: str
         :param image_fields: Image to add. (required)
         :type image_fields: ImageFields
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -141,15 +141,15 @@
                                                         local_var_params['image_fields'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `image_fields` when calling `add_image_to_person`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'person_id' in local_var_params:
-            path_params['person_id'] = local_var_params['person_id']  # noqa: E501
+            path_params['personId'] = local_var_params['person_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
         if 'x_request_id' in local_var_params:
             header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
@@ -167,15 +167,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/persons/{person_id}/images', 'POST',
+            '/api/persons/{personId}/images', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Image',  # noqa: E501
@@ -194,15 +194,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_person(person_fields, async_req=True)
         >>> result = thread.get()
 
         :param person_fields: (required)
         :type person_fields: PersonFields
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -225,15 +225,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_person_with_http_info(person_fields, async_req=True)
         >>> result = thread.get()
 
         :param person_fields: (required)
         :type person_fields: PersonFields
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -333,18 +333,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_image_of_person(image_id, person_id, async_req=True)
         >>> result = thread.get()
 
         :param image_id: Image ID. (required)
-        :type image_id: int
+        :type image_id: str
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -366,18 +366,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_image_of_person_with_http_info(image_id, person_id, async_req=True)
         >>> result = thread.get()
 
         :param image_id: Image ID. (required)
-        :type image_id: int
+        :type image_id: str
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -432,17 +432,17 @@
                                                         local_var_params['person_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `person_id` when calling `delete_image_of_person`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'image_id' in local_var_params:
-            path_params['image_id'] = local_var_params['image_id']  # noqa: E501
+            path_params['imageId'] = local_var_params['image_id']  # noqa: E501
         if 'person_id' in local_var_params:
-            path_params['person_id'] = local_var_params['person_id']  # noqa: E501
+            path_params['personId'] = local_var_params['person_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
         if 'x_request_id' in local_var_params:
             header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
@@ -454,15 +454,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/persons/{person_id}/images/{image_id}', 'DELETE',
+            '/api/persons/{personId}/images/{imageId}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
@@ -480,16 +480,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_person(person_id, async_req=True)
         >>> result = thread.get()
 
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -511,16 +511,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_person_with_http_info(person_id, async_req=True)
         >>> result = thread.get()
 
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -570,15 +570,15 @@
                                                         local_var_params['person_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `person_id` when calling `delete_person`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'person_id' in local_var_params:
-            path_params['person_id'] = local_var_params['person_id']  # noqa: E501
+            path_params['personId'] = local_var_params['person_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
         if 'x_request_id' in local_var_params:
             header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
@@ -590,15 +590,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/persons/{person_id}', 'DELETE',
+            '/api/persons/{personId}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
@@ -620,16 +620,16 @@
         >>> result = thread.get()
 
         :param page: The page number to get a list of persons or groups. (required)
         :type page: int
         :param size: The page size with a list of persons or groups, items. (required)
         :type size: int
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -655,16 +655,16 @@
         >>> result = thread.get()
 
         :param page: The page number to get a list of persons or groups. (required)
         :type page: int
         :param size: The page size with a list of persons or groups, items. (required)
         :type size: int
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -724,15 +724,15 @@
                                                         local_var_params['person_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `person_id` when calling `get_all_groups_by_person_id`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'person_id' in local_var_params:
-            path_params['person_id'] = local_var_params['person_id']  # noqa: E501
+            path_params['personId'] = local_var_params['person_id']  # noqa: E501
 
         query_params = []
         if 'page' in local_var_params and local_var_params['page'] is not None:  # noqa: E501
             query_params.append(('page', local_var_params['page']))  # noqa: E501
         if 'size' in local_var_params and local_var_params['size'] is not None:  # noqa: E501
             query_params.append(('size', local_var_params['size']))  # noqa: E501
 
@@ -748,15 +748,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/persons/{person_id}/groups', 'GET',
+            '/api/persons/{personId}/groups', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='GroupPage',  # noqa: E501
@@ -778,16 +778,16 @@
         >>> result = thread.get()
 
         :param page: The page number to get a list of persons or groups. (required)
         :type page: int
         :param size: The page size with a list of persons or groups, items. (required)
         :type size: int
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -813,16 +813,16 @@
         >>> result = thread.get()
 
         :param page: The page number to get a list of persons or groups. (required)
         :type page: int
         :param size: The page size with a list of persons or groups, items. (required)
         :type size: int
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -882,15 +882,15 @@
                                                         local_var_params['person_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `person_id` when calling `get_all_images_by_person_id`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'person_id' in local_var_params:
-            path_params['person_id'] = local_var_params['person_id']  # noqa: E501
+            path_params['personId'] = local_var_params['person_id']  # noqa: E501
 
         query_params = []
         if 'page' in local_var_params and local_var_params['page'] is not None:  # noqa: E501
             query_params.append(('page', local_var_params['page']))  # noqa: E501
         if 'size' in local_var_params and local_var_params['size'] is not None:  # noqa: E501
             query_params.append(('size', local_var_params['size']))  # noqa: E501
 
@@ -906,15 +906,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/persons/{person_id}/images', 'GET',
+            '/api/persons/{personId}/images', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='ImagePage',  # noqa: E501
@@ -922,175 +922,28 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def get_all_persons(self, page, size, **kwargs):  # noqa: E501
-        """Get persons  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_all_persons(page, size, async_req=True)
-        >>> result = thread.get()
-
-        :param page: The page number to get a list of persons or groups. (required)
-        :type page: int
-        :param size: The page size with a list of persons or groups, items. (required)
-        :type size: int
-        :param x_request_id:
-        :type x_request_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: PersonsPage
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_all_persons_with_http_info(page, size, **kwargs)  # noqa: E501
-
-    def get_all_persons_with_http_info(self, page, size, **kwargs):  # noqa: E501
-        """Get persons  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_all_persons_with_http_info(page, size, async_req=True)
-        >>> result = thread.get()
-
-        :param page: The page number to get a list of persons or groups. (required)
-        :type page: int
-        :param size: The page size with a list of persons or groups, items. (required)
-        :type size: int
-        :param x_request_id:
-        :type x_request_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(PersonsPage, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'page'
-            'size'
-            'x_request_id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_all_persons" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'page' is set
-        if self.api_client.client_side_validation and ('page' not in local_var_params or  # noqa: E501
-                                                        local_var_params['page'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `page` when calling `get_all_persons`")  # noqa: E501
-        # verify the required parameter 'size' is set
-        if self.api_client.client_side_validation and ('size' not in local_var_params or  # noqa: E501
-                                                        local_var_params['size'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `size` when calling `get_all_persons`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-        if 'page' in local_var_params and local_var_params['page'] is not None:  # noqa: E501
-            query_params.append(('page', local_var_params['page']))  # noqa: E501
-        if 'size' in local_var_params and local_var_params['size'] is not None:  # noqa: E501
-            query_params.append(('size', local_var_params['size']))  # noqa: E501
-
-        header_params = {}
-        if 'x_request_id' in local_var_params:
-            header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = []  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/persons', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='PersonsPage',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
     def get_image_of_person(self, image_id, person_id, **kwargs):  # noqa: E501
         """Get person image by id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_image_of_person(image_id, person_id, async_req=True)
         >>> result = thread.get()
 
         :param image_id: Image ID. (required)
-        :type image_id: int
+        :type image_id: str
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -1112,18 +965,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_image_of_person_with_http_info(image_id, person_id, async_req=True)
         >>> result = thread.get()
 
         :param image_id: Image ID. (required)
-        :type image_id: int
+        :type image_id: str
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -1178,17 +1031,17 @@
                                                         local_var_params['person_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `person_id` when calling `get_image_of_person`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'image_id' in local_var_params:
-            path_params['image_id'] = local_var_params['image_id']  # noqa: E501
+            path_params['imageId'] = local_var_params['image_id']  # noqa: E501
         if 'person_id' in local_var_params:
-            path_params['person_id'] = local_var_params['person_id']  # noqa: E501
+            path_params['personId'] = local_var_params['person_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
         if 'x_request_id' in local_var_params:
             header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
@@ -1200,15 +1053,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json''image/*'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/persons/{person_id}/images/{image_id}', 'GET',
+            '/api/persons/{personId}/images/{imageId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='file_type',  # noqa: E501
@@ -1226,16 +1079,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_person(person_id, async_req=True)
         >>> result = thread.get()
 
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -1257,16 +1110,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_person_with_http_info(person_id, async_req=True)
         >>> result = thread.get()
 
         :param person_id: Person ID. (required)
-        :type person_id: int
-        :param x_request_id:
+        :type person_id: str
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -1316,15 +1169,15 @@
                                                         local_var_params['person_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `person_id` when calling `get_person`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'person_id' in local_var_params:
-            path_params['person_id'] = local_var_params['person_id']  # noqa: E501
+            path_params['personId'] = local_var_params['person_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
         if 'x_request_id' in local_var_params:
             header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
@@ -1336,15 +1189,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/persons/{person_id}', 'GET',
+            '/api/persons/{personId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Person',  # noqa: E501
@@ -1362,18 +1215,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_person(person_id, person_fields, async_req=True)
         >>> result = thread.get()
 
         :param person_id: Person ID. (required)
-        :type person_id: int
+        :type person_id: str
         :param person_fields: Request body for the Person to update. (required)
         :type person_fields: PersonFields
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -1395,18 +1248,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_person_with_http_info(person_id, person_fields, async_req=True)
         >>> result = thread.get()
 
         :param person_id: Person ID. (required)
-        :type person_id: int
+        :type person_id: str
         :param person_fields: Request body for the Person to update. (required)
         :type person_fields: PersonFields
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -1461,15 +1314,15 @@
                                                         local_var_params['person_fields'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `person_fields` when calling `update_person`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'person_id' in local_var_params:
-            path_params['person_id'] = local_var_params['person_id']  # noqa: E501
+            path_params['personId'] = local_var_params['person_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
         if 'x_request_id' in local_var_params:
             header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
@@ -1487,15 +1340,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/persons/{person_id}', 'PUT',
+            '/api/persons/{personId}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/search_api.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api/search_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -33,25 +33,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def search(self, search_request, **kwargs):  # noqa: E501
-        """Find person by image in groups.  # noqa: E501
+        """Find person by image in groups  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.search(search_request, async_req=True)
         >>> result = thread.get()
 
         :param search_request: (required)
         :type search_request: SearchRequest
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -64,25 +64,25 @@
                  returns the request thread.
         :rtype: SearchResult
         """
         kwargs['_return_http_data_only'] = True
         return self.search_with_http_info(search_request, **kwargs)  # noqa: E501
 
     def search_with_http_info(self, search_request, **kwargs):  # noqa: E501
-        """Find person by image in groups.  # noqa: E501
+        """Find person by image in groups  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.search_with_http_info(search_request, async_req=True)
         >>> result = thread.get()
 
         :param search_request: (required)
         :type search_request: SearchRequest
-        :param x_request_id:
+        :param x_request_id: Request header label.
         :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api_client.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/apis/__init__.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/apis/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 # flake8: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from .api.group_api import GroupApi
+#   from .api.diagnostics_api import DiagnosticsApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
+from regula.facesdk.webclient.gen.api.diagnostics_api import DiagnosticsApi
 from regula.facesdk.webclient.gen.api.group_api import GroupApi
 from regula.facesdk.webclient.gen.api.liveness_2_0_api import Liveness20Api
 from regula.facesdk.webclient.gen.api.matching_api import MatchingApi
 from regula.facesdk.webclient.gen.api.person_api import PersonApi
 from regula.facesdk.webclient.gen.api.search_api import SearchApi
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/configuration.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -375,15 +375,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 5.1.0\n"\
+               "Version of the API: 5.2.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/exceptions.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/crop.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_request.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detect_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -33,26 +33,26 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'tag': 'str',
         'process_param': 'ProcessParam',
         'image': 'str',
         'thumbnails': 'bool',
-        'attributes': 'bool',
+        'attributes': 'DetectRequestAttributes',
     }
 
     attribute_map = {
         'tag': 'tag',
         'process_param': 'processParam',
         'image': 'image',
         'thumbnails': 'thumbnails',
         'attributes': 'attributes',
     }
 
-    def __init__(self, tag=None, process_param=None, image=None, thumbnails=False, attributes=False, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, tag=None, process_param=None, image=None, thumbnails=False, attributes=None, local_vars_configuration=None):  # noqa: E501
         """DetectRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._tag = None
         self._process_param = None
@@ -162,29 +162,27 @@
 
         self._thumbnails = thumbnails
 
     @property
     def attributes(self):
         """Gets the attributes of this DetectRequest.  # noqa: E501
 
-        Whether to evaluate attributes, such as age and emotions.  # noqa: E501
 
         :return: The attributes of this DetectRequest.  # noqa: E501
-        :rtype: bool
+        :rtype: DetectRequestAttributes
         """
         return self._attributes
 
     @attributes.setter
     def attributes(self, attributes):
         """Sets the attributes of this DetectRequest.
 
-        Whether to evaluate attributes, such as age and emotions.  # noqa: E501
 
         :param attributes: The attributes of this DetectRequest.  # noqa: E501
-        :type attributes: bool
+        :type attributes: DetectRequestAttributes
         """
 
         self._attributes = attributes
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_response.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detect_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_response_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detect_response_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_result.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detect_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -31,15 +31,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'crop': 'str',
         'attributes': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
-        'landmarks': '[[float]]',
+        'landmarks': '[[int]]',
         'quality': 'DetectionQuality',
         'roi': 'FaceRectangular',
         'thumbnail': 'str',
     }
 
     attribute_map = {
         'crop': 'crop',
@@ -122,26 +122,26 @@
     @property
     def landmarks(self):
         """Gets the landmarks of this Detection.  # noqa: E501
 
         Absolute coordinates (x,y) of five points of each detected face: left eye, right eye, nose, left point of lips, right point of lips.  # noqa: E501
 
         :return: The landmarks of this Detection.  # noqa: E501
-        :rtype: [[float]]
+        :rtype: [[int]]
         """
         return self._landmarks
 
     @landmarks.setter
     def landmarks(self, landmarks):
         """Sets the landmarks of this Detection.
 
         Absolute coordinates (x,y) of five points of each detected face: left eye, right eye, nose, left point of lips, right point of lips.  # noqa: E501
 
         :param landmarks: The landmarks of this Detection.  # noqa: E501
-        :type landmarks: [[float]]
+        :type landmarks: [[int]]
         """
         if self.local_vars_configuration.client_side_validation and landmarks is None:  # noqa: E501
             raise ValueError("Invalid value for `landmarks`, must not be `None`")  # noqa: E501
 
         self._landmarks = landmarks
 
     @property
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection_face.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detection_face.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -31,62 +31,67 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'face_index': 'float',
         'landmarks': '[[float]]',
+        'rotation_angle': 'float',
         'roi': 'FaceRectangular',
         'thumbnail': 'str',
     }
 
     attribute_map = {
         'face_index': 'faceIndex',
         'landmarks': 'landmarks',
+        'rotation_angle': 'rotationAngle',
         'roi': 'roi',
         'thumbnail': 'thumbnail',
     }
 
-    def __init__(self, face_index=None, landmarks=None, roi=None, thumbnail=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, face_index=None, landmarks=None, rotation_angle=None, roi=None, thumbnail=None, local_vars_configuration=None):  # noqa: E501
         """DetectionFace - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._face_index = None
         self._landmarks = None
+        self._rotation_angle = None
         self._roi = None
         self._thumbnail = None
         self.discriminator = None
 
         if face_index is not None:
             self.face_index = face_index
         if landmarks is not None:
             self.landmarks = landmarks
+        if rotation_angle is not None:
+            self.rotation_angle = rotation_angle
         if roi is not None:
             self.roi = roi
         if thumbnail is not None:
             self.thumbnail = thumbnail
 
     @property
     def face_index(self):
         """Gets the face_index of this DetectionFace.  # noqa: E501
 
-        Faces index used to identify faces in scope of one photo.  # noqa: E501
+        The detected face index number.  # noqa: E501
 
         :return: The face_index of this DetectionFace.  # noqa: E501
         :rtype: float
         """
         return self._face_index
 
     @face_index.setter
     def face_index(self, face_index):
         """Sets the face_index of this DetectionFace.
 
-        Faces index used to identify faces in scope of one photo.  # noqa: E501
+        The detected face index number.  # noqa: E501
 
         :param face_index: The face_index of this DetectionFace.  # noqa: E501
         :type face_index: float
         """
 
         self._face_index = face_index
 
@@ -110,14 +115,37 @@
         :param landmarks: The landmarks of this DetectionFace.  # noqa: E501
         :type landmarks: [[float]]
         """
 
         self._landmarks = landmarks
 
     @property
+    def rotation_angle(self):
+        """Gets the rotation_angle of this DetectionFace.  # noqa: E501
+
+        Angle of rotation of the face from the vertical axis, degrees.  # noqa: E501
+
+        :return: The rotation_angle of this DetectionFace.  # noqa: E501
+        :rtype: float
+        """
+        return self._rotation_angle
+
+    @rotation_angle.setter
+    def rotation_angle(self, rotation_angle):
+        """Sets the rotation_angle of this DetectionFace.
+
+        Angle of rotation of the face from the vertical axis, degrees.  # noqa: E501
+
+        :param rotation_angle: The rotation_angle of this DetectionFace.  # noqa: E501
+        :type rotation_angle: float
+        """
+
+        self._rotation_angle = rotation_angle
+
+    @property
     def roi(self):
         """Gets the roi of this DetectionFace.  # noqa: E501
 
 
         :return: The roi of this DetectionFace.  # noqa: E501
         :rtype: FaceRectangular
         """
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection_quality.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/detection_quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_align_type_quality.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_align_type_quality.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_align_type.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_image_quality_align_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_groups.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_image_quality_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_status.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_image_quality_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_config_name.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_quality_config_name.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -22,17 +22,14 @@
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     ""
-    ART_FACE = "ArtFace"
-
-    ""
     IMAGE_WIDTH = "ImageWidth"
 
     ""
     IMAGE_HEIGHT = "ImageHeight"
 
     ""
     IMAGE_WIDTH_TO_HEIGHT = "ImageWidthToHeight"
@@ -162,15 +159,21 @@
 
     ""
     MEDICAL_MASK = "MedicalMask"
 
     ""
     BACKGROUND_COLOR_MATCH = "BackgroundColorMatch"
 
-    allowable_values = [ART_FACE, IMAGE_WIDTH, IMAGE_HEIGHT, IMAGE_WIDTH_TO_HEIGHT, IMAGE_CHANNELS_NUMBER, PADDING_RATIO, FACE_MID_POINT_HORIZONTAL_POSITION, FACE_MID_POINT_VERTICAL_POSITION, HEAD_WIDTH_RATIO, HEAD_HEIGHT_RATIO, EYES_DISTANCE, YAW, PITCH, ROLL, BLUR_LEVEL, NOISE_LEVEL, EYE_RIGHT_CLOSED, EYE_LEFT_CLOSED, EYE_RIGHT_OCCLUDED, EYE_LEFT_OCCLUDED, EYES_RED, EYE_RIGHT_COVERED_WITH_HAIR, EYE_LEFT_COVERED_WITH_HAIR, OFF_GAZE, FACE_DYNAMIC_RANGE, UNNATURAL_SKIN_TONE, TOO_DARK, TOO_LIGHT, FACE_GLARE, SHADOWS_ON_FACE, DARK_GLASSES, REFLECTION_ON_GLASSES, FRAMES_TOO_HEAVY, FACE_OCCLUDED, HEAD_COVERING, BACKGROUND_UNIFORMITY, SHADOWS_ON_BACKGROUND, OTHER_FACES, SHOULDERS_POSE, EXPRESSION_LEVEL, MOUTH_OPEN, FOREHEAD_COVERING, SMILE, STRONG_MAKEUP, HEADPHONES, MEDICAL_MASK, BACKGROUND_COLOR_MATCH]  # noqa: E501
+    ""
+    ART_FACE = "ArtFace"
+
+    ""
+    CONTACT_LENSES = "ContactLenses"
+
+    allowable_values = [IMAGE_WIDTH, IMAGE_HEIGHT, IMAGE_WIDTH_TO_HEIGHT, IMAGE_CHANNELS_NUMBER, PADDING_RATIO, FACE_MID_POINT_HORIZONTAL_POSITION, FACE_MID_POINT_VERTICAL_POSITION, HEAD_WIDTH_RATIO, HEAD_HEIGHT_RATIO, EYES_DISTANCE, YAW, PITCH, ROLL, BLUR_LEVEL, NOISE_LEVEL, EYE_RIGHT_CLOSED, EYE_LEFT_CLOSED, EYE_RIGHT_OCCLUDED, EYE_LEFT_OCCLUDED, EYES_RED, EYE_RIGHT_COVERED_WITH_HAIR, EYE_LEFT_COVERED_WITH_HAIR, OFF_GAZE, FACE_DYNAMIC_RANGE, UNNATURAL_SKIN_TONE, TOO_DARK, TOO_LIGHT, FACE_GLARE, SHADOWS_ON_FACE, DARK_GLASSES, REFLECTION_ON_GLASSES, FRAMES_TOO_HEAVY, FACE_OCCLUDED, HEAD_COVERING, BACKGROUND_UNIFORMITY, SHADOWS_ON_BACKGROUND, OTHER_FACES, SHOULDERS_POSE, EXPRESSION_LEVEL, MOUTH_OPEN, FOREHEAD_COVERING, SMILE, STRONG_MAKEUP, HEADPHONES, MEDICAL_MASK, BACKGROUND_COLOR_MATCH, ART_FACE, CONTACT_LENSES]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_scenarios.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_quality_scenarios.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_status.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_quality_status.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_rectangular.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_rectangular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_sdk_result.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_sdk_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/faces_response.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/faces_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -31,72 +31,72 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'face_index': 'float',
         'landmarks': '[[float]]',
+        'rotation_angle': 'float',
         'roi': 'FaceRectangular',
         'thumbnail': 'str',
         'persons': '[PersonWithImages]',
-        'rotation_angle': 'float',
     }
 
     attribute_map = {
         'face_index': 'faceIndex',
         'landmarks': 'landmarks',
+        'rotation_angle': 'rotationAngle',
         'roi': 'roi',
         'thumbnail': 'thumbnail',
         'persons': 'persons',
-        'rotation_angle': 'rotationAngle',
     }
 
-    def __init__(self, face_index=None, landmarks=None, roi=None, thumbnail=None, persons=None, rotation_angle=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, face_index=None, landmarks=None, rotation_angle=None, roi=None, thumbnail=None, persons=None, local_vars_configuration=None):  # noqa: E501
         """FacesResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._face_index = None
         self._landmarks = None
+        self._rotation_angle = None
         self._roi = None
         self._thumbnail = None
         self._persons = None
-        self._rotation_angle = None
         self.discriminator = None
 
         if face_index is not None:
             self.face_index = face_index
         if landmarks is not None:
             self.landmarks = landmarks
+        if rotation_angle is not None:
+            self.rotation_angle = rotation_angle
         if roi is not None:
             self.roi = roi
         if thumbnail is not None:
             self.thumbnail = thumbnail
         if persons is not None:
             self.persons = persons
-        if rotation_angle is not None:
-            self.rotation_angle = rotation_angle
 
     @property
     def face_index(self):
         """Gets the face_index of this FacesResponse.  # noqa: E501
 
-        Faces index used to identify faces in scope of one photo.  # noqa: E501
+        The detected face index number.  # noqa: E501
 
         :return: The face_index of this FacesResponse.  # noqa: E501
         :rtype: float
         """
         return self._face_index
 
     @face_index.setter
     def face_index(self, face_index):
         """Sets the face_index of this FacesResponse.
 
-        Faces index used to identify faces in scope of one photo.  # noqa: E501
+        The detected face index number.  # noqa: E501
 
         :param face_index: The face_index of this FacesResponse.  # noqa: E501
         :type face_index: float
         """
 
         self._face_index = face_index
 
@@ -120,14 +120,35 @@
         :param landmarks: The landmarks of this FacesResponse.  # noqa: E501
         :type landmarks: [[float]]
         """
 
         self._landmarks = landmarks
 
     @property
+    def rotation_angle(self):
+        """Gets the rotation_angle of this FacesResponse.  # noqa: E501
+
+
+        :return: The rotation_angle of this FacesResponse.  # noqa: E501
+        :rtype: float
+        """
+        return self._rotation_angle
+
+    @rotation_angle.setter
+    def rotation_angle(self, rotation_angle):
+        """Sets the rotation_angle of this FacesResponse.
+
+
+        :param rotation_angle: The rotation_angle of this FacesResponse.  # noqa: E501
+        :type rotation_angle: float
+        """
+
+        self._rotation_angle = rotation_angle
+
+    @property
     def roi(self):
         """Gets the roi of this FacesResponse.  # noqa: E501
 
 
         :return: The roi of this FacesResponse.  # noqa: E501
         :rtype: FaceRectangular
         """
@@ -184,35 +205,14 @@
 
         :param persons: The persons of this FacesResponse.  # noqa: E501
         :type persons: [PersonWithImages]
         """
 
         self._persons = persons
 
-    @property
-    def rotation_angle(self):
-        """Gets the rotation_angle of this FacesResponse.  # noqa: E501
-
-
-        :return: The rotation_angle of this FacesResponse.  # noqa: E501
-        :rtype: float
-        """
-        return self._rotation_angle
-
-    @rotation_angle.setter
-    def rotation_angle(self, rotation_angle):
-        """Sets the rotation_angle of this FacesResponse.
-
-
-        :param rotation_angle: The rotation_angle of this FacesResponse.  # noqa: E501
-        :type rotation_angle: float
-        """
-
-        self._rotation_angle = rotation_angle
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/faces_response_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/faces_response_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/group.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,49 +29,77 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'tag': 'str',
         'name': 'str',
         'metadata': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
-        'id': 'int',
+        'id': 'str',
         'created_at': 'str',
     }
 
     attribute_map = {
+        'tag': 'tag',
         'name': 'name',
         'metadata': 'metadata',
         'id': 'id',
-        'created_at': 'created_at',
+        'created_at': 'createdAt',
     }
 
-    def __init__(self, name=None, metadata=None, id=None, created_at=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, tag=None, name=None, metadata=None, id=None, created_at=None, local_vars_configuration=None):  # noqa: E501
         """Group - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._tag = None
         self._name = None
         self._metadata = None
         self._id = None
         self._created_at = None
         self.discriminator = None
 
+        if tag is not None:
+            self.tag = tag
         if name is not None:
             self.name = name
         if metadata is not None:
             self.metadata = metadata
         if id is not None:
             self.id = id
         if created_at is not None:
             self.created_at = created_at
 
     @property
+    def tag(self):
+        """Gets the tag of this Group.  # noqa: E501
+
+        Session identificator.  # noqa: E501
+
+        :return: The tag of this Group.  # noqa: E501
+        :rtype: str
+        """
+        return self._tag
+
+    @tag.setter
+    def tag(self, tag):
+        """Sets the tag of this Group.
+
+        Session identificator.  # noqa: E501
+
+        :param tag: The tag of this Group.  # noqa: E501
+        :type tag: str
+        """
+
+        self._tag = tag
+
+    @property
     def name(self):
         """Gets the name of this Group.  # noqa: E501
 
         Group to create name.  # noqa: E501
 
         :return: The name of this Group.  # noqa: E501
         :rtype: str
@@ -116,26 +144,26 @@
     @property
     def id(self):
         """Gets the id of this Group.  # noqa: E501
 
         Group ID.  # noqa: E501
 
         :return: The id of this Group.  # noqa: E501
-        :rtype: int
+        :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this Group.
 
         Group ID.  # noqa: E501
 
         :param id: The id of this Group.  # noqa: E501
-        :type id: int
+        :type id: str
         """
 
         self._id = id
 
     @property
     def created_at(self):
         """Gets the created_at of this Group.  # noqa: E501
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/group_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,21 +29,21 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'int',
+        'id': 'str',
         'created_at': 'str',
     }
 
     attribute_map = {
         'id': 'id',
-        'created_at': 'created_at',
+        'created_at': 'createdAt',
     }
 
     def __init__(self, id=None, created_at=None, local_vars_configuration=None):  # noqa: E501
         """GroupAllOf - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
@@ -60,26 +60,26 @@
     @property
     def id(self):
         """Gets the id of this GroupAllOf.  # noqa: E501
 
         Group ID.  # noqa: E501
 
         :return: The id of this GroupAllOf.  # noqa: E501
-        :rtype: int
+        :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this GroupAllOf.
 
         Group ID.  # noqa: E501
 
         :param id: The id of this GroupAllOf.  # noqa: E501
-        :type id: int
+        :type id: str
         """
 
         self._id = id
 
     @property
     def created_at(self):
         """Gets the created_at of this GroupAllOf.  # noqa: E501
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_page.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/group_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -37,15 +37,15 @@
         'page': 'int',
         'total_pages': 'int',
     }
 
     attribute_map = {
         'items': 'items',
         'page': 'page',
-        'total_pages': 'total_pages',
+        'total_pages': 'totalPages',
     }
 
     def __init__(self, items=None, page=None, total_pages=None, local_vars_configuration=None):  # noqa: E501
         """GroupPage - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
@@ -62,26 +62,26 @@
         if total_pages is not None:
             self.total_pages = total_pages
 
     @property
     def items(self):
         """Gets the items of this GroupPage.  # noqa: E501
 
-        The array of Groups that are found during the search.  # noqa: E501
+        Array of Groups that are found during the search.  # noqa: E501
 
         :return: The items of this GroupPage.  # noqa: E501
         :rtype: [Group]
         """
         return self._items
 
     @items.setter
     def items(self, items):
         """Sets the items of this GroupPage.
 
-        The array of Groups that are found during the search.  # noqa: E501
+        Array of Groups that are found during the search.  # noqa: E501
 
         :param items: The items of this GroupPage.  # noqa: E501
         :type items: [Group]
         """
 
         self._items = items
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_page_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/group_page_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -52,26 +52,26 @@
         if items is not None:
             self.items = items
 
     @property
     def items(self):
         """Gets the items of this GroupPageAllOf.  # noqa: E501
 
-        The array of Groups that are found during the search.  # noqa: E501
+        Array of Groups that are found during the search.  # noqa: E501
 
         :return: The items of this GroupPageAllOf.  # noqa: E501
         :rtype: [Group]
         """
         return self._items
 
     @items.setter
     def items(self, items):
         """Sets the items of this GroupPageAllOf.
 
-        The array of Groups that are found during the search.  # noqa: E501
+        Array of Groups that are found during the search.  # noqa: E501
 
         :param items: The items of this GroupPageAllOf.  # noqa: E501
         :type items: [Group]
         """
 
         self._items = items
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_to_create.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/group_to_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,39 +29,67 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'tag': 'str',
         'name': 'str',
         'metadata': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
     }
 
     attribute_map = {
+        'tag': 'tag',
         'name': 'name',
         'metadata': 'metadata',
     }
 
-    def __init__(self, name=None, metadata=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, tag=None, name=None, metadata=None, local_vars_configuration=None):  # noqa: E501
         """GroupToCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._tag = None
         self._name = None
         self._metadata = None
         self.discriminator = None
 
+        if tag is not None:
+            self.tag = tag
         if name is not None:
             self.name = name
         if metadata is not None:
             self.metadata = metadata
 
     @property
+    def tag(self):
+        """Gets the tag of this GroupToCreate.  # noqa: E501
+
+        Session identificator.  # noqa: E501
+
+        :return: The tag of this GroupToCreate.  # noqa: E501
+        :rtype: str
+        """
+        return self._tag
+
+    @tag.setter
+    def tag(self, tag):
+        """Sets the tag of this GroupToCreate.
+
+        Session identificator.  # noqa: E501
+
+        :param tag: The tag of this GroupToCreate.  # noqa: E501
+        :type tag: str
+        """
+
+        self._tag = tag
+
+    @property
     def name(self):
         """Gets the name of this GroupToCreate.  # noqa: E501
 
         Group to create name.  # noqa: E501
 
         :return: The name of this GroupToCreate.  # noqa: E501
         :rtype: str
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -40,17 +40,17 @@
         'path': 'str',
         'url': 'str',
         'metadata': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
     }
 
     attribute_map = {
         'id': 'id',
-        'content_type': 'content_type',
-        'created_at': 'created_at',
-        'updated_at': 'updated_at',
+        'content_type': 'contentType',
+        'created_at': 'createdAt',
+        'updated_at': 'updatedAt',
         'path': 'path',
         'url': 'url',
         'metadata': 'metadata',
     }
 
     def __init__(self, id=None, content_type=None, created_at=None, updated_at=None, path=None, url=None, metadata=None, local_vars_configuration=None):  # noqa: E501
         """Image - a model defined in OpenAPI"""  # noqa: E501
@@ -82,141 +82,141 @@
         if metadata is not None:
             self.metadata = metadata
 
     @property
     def id(self):
         """Gets the id of this Image.  # noqa: E501
 
-        Response image ID.  # noqa: E501
+        Response image ID. The list is sorted by decreasing ID value.  # noqa: E501
 
         :return: The id of this Image.  # noqa: E501
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this Image.
 
-        Response image ID.  # noqa: E501
+        Response image ID. The list is sorted by decreasing ID value.  # noqa: E501
 
         :param id: The id of this Image.  # noqa: E501
         :type id: int
         """
 
         self._id = id
 
     @property
     def content_type(self):
         """Gets the content_type of this Image.  # noqa: E501
 
-        The original media type of the returned image.  # noqa: E501
+        Original media type of the returned image.  # noqa: E501
 
         :return: The content_type of this Image.  # noqa: E501
         :rtype: str
         """
         return self._content_type
 
     @content_type.setter
     def content_type(self, content_type):
         """Sets the content_type of this Image.
 
-        The original media type of the returned image.  # noqa: E501
+        Original media type of the returned image.  # noqa: E501
 
         :param content_type: The content_type of this Image.  # noqa: E501
         :type content_type: str
         """
 
         self._content_type = content_type
 
     @property
     def created_at(self):
         """Gets the created_at of this Image.  # noqa: E501
 
-        The returned image creation date.  # noqa: E501
+        Returned image creation date.  # noqa: E501
 
         :return: The created_at of this Image.  # noqa: E501
         :rtype: str
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
         """Sets the created_at of this Image.
 
-        The returned image creation date.  # noqa: E501
+        Returned image creation date.  # noqa: E501
 
         :param created_at: The created_at of this Image.  # noqa: E501
         :type created_at: str
         """
 
         self._created_at = created_at
 
     @property
     def updated_at(self):
         """Gets the updated_at of this Image.  # noqa: E501
 
-        The returned image update date.  # noqa: E501
+        Returned image update date.  # noqa: E501
 
         :return: The updated_at of this Image.  # noqa: E501
         :rtype: str
         """
         return self._updated_at
 
     @updated_at.setter
     def updated_at(self, updated_at):
         """Sets the updated_at of this Image.
 
-        The returned image update date.  # noqa: E501
+        Returned image update date.  # noqa: E501
 
         :param updated_at: The updated_at of this Image.  # noqa: E501
         :type updated_at: str
         """
 
         self._updated_at = updated_at
 
     @property
     def path(self):
         """Gets the path of this Image.  # noqa: E501
 
-        The returned image S3 path.  # noqa: E501
+        Returned image S3 path.  # noqa: E501
 
         :return: The path of this Image.  # noqa: E501
         :rtype: str
         """
         return self._path
 
     @path.setter
     def path(self, path):
         """Sets the path of this Image.
 
-        The returned image S3 path.  # noqa: E501
+        Returned image S3 path.  # noqa: E501
 
         :param path: The path of this Image.  # noqa: E501
         :type path: str
         """
 
         self._path = path
 
     @property
     def url(self):
         """Gets the url of this Image.  # noqa: E501
 
-        The returned image URL.  # noqa: E501
+        Returned image URL.  # noqa: E501
 
         :return: The url of this Image.  # noqa: E501
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
         """Sets the url of this Image.
 
-        The returned image URL.  # noqa: E501
+        Returned image URL.  # noqa: E501
 
         :param url: The url of this Image.  # noqa: E501
         :type url: str
         """
 
         self._url = url
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_fields.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/image_page_all_of.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class ImageFields(object):
+class ImagePageAllOf(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'image': 'ImageFieldsImage',
+        'items': '[Image]',
     }
 
     attribute_map = {
-        'image': 'image',
+        'items': 'items',
     }
 
-    def __init__(self, image=None, local_vars_configuration=None):  # noqa: E501
-        """ImageFields - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, items=None, local_vars_configuration=None):  # noqa: E501
+        """ImagePageAllOf - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._image = None
+        self._items = None
         self.discriminator = None
 
-        if image is not None:
-            self.image = image
+        if items is not None:
+            self.items = items
 
     @property
-    def image(self):
-        """Gets the image of this ImageFields.  # noqa: E501
+    def items(self):
+        """Gets the items of this ImagePageAllOf.  # noqa: E501
 
 
-        :return: The image of this ImageFields.  # noqa: E501
-        :rtype: ImageFieldsImage
+        :return: The items of this ImagePageAllOf.  # noqa: E501
+        :rtype: [Image]
         """
-        return self._image
+        return self._items
 
-    @image.setter
-    def image(self, image):
-        """Sets the image of this ImageFields.
+    @items.setter
+    def items(self, items):
+        """Sets the items of this ImagePageAllOf.
 
 
-        :param image: The image of this ImageFields.  # noqa: E501
-        :type image: ImageFieldsImage
+        :param items: The items of this ImagePageAllOf.  # noqa: E501
+        :type items: [Image]
         """
 
-        self._image = image
+        self._items = items
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -103,18 +103,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ImageFields):
+        if not isinstance(other, ImagePageAllOf):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ImageFields):
+        if not isinstance(other, ImagePageAllOf):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_fields_image.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_response_all_of.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,111 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class ImageFieldsImage(object):
+class MatchResponseAllOf(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'content_type': 'str',
-        'content': 'str',
+        'detections': '[MatchImageDetection]',
+        'results': '[MatchImageResult]',
     }
 
     attribute_map = {
-        'content_type': 'content_type',
-        'content': 'content',
+        'detections': 'detections',
+        'results': 'results',
     }
 
-    def __init__(self, content_type=None, content=None, local_vars_configuration=None):  # noqa: E501
-        """ImageFieldsImage - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, detections=None, results=None, local_vars_configuration=None):  # noqa: E501
+        """MatchResponseAllOf - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._content_type = None
-        self._content = None
+        self._detections = None
+        self._results = None
         self.discriminator = None
 
-        if content_type is not None:
-            self.content_type = content_type
-        if content is not None:
-            self.content = content
+        if detections is not None:
+            self.detections = detections
+        if results is not None:
+            self.results = results
 
     @property
-    def content_type(self):
-        """Gets the content_type of this ImageFieldsImage.  # noqa: E501
+    def detections(self):
+        """Gets the detections of this MatchResponseAllOf.  # noqa: E501
 
-        The original media type of the uploaded image.  # noqa: E501
+        The array of detected faces.  # noqa: E501
 
-        :return: The content_type of this ImageFieldsImage.  # noqa: E501
-        :rtype: str
+        :return: The detections of this MatchResponseAllOf.  # noqa: E501
+        :rtype: [MatchImageDetection]
         """
-        return self._content_type
+        return self._detections
 
-    @content_type.setter
-    def content_type(self, content_type):
-        """Sets the content_type of this ImageFieldsImage.
+    @detections.setter
+    def detections(self, detections):
+        """Sets the detections of this MatchResponseAllOf.
 
-        The original media type of the uploaded image.  # noqa: E501
+        The array of detected faces.  # noqa: E501
 
-        :param content_type: The content_type of this ImageFieldsImage.  # noqa: E501
-        :type content_type: str
+        :param detections: The detections of this MatchResponseAllOf.  # noqa: E501
+        :type detections: [MatchImageDetection]
         """
 
-        self._content_type = content_type
+        self._detections = detections
 
     @property
-    def content(self):
-        """Gets the content of this ImageFieldsImage.  # noqa: E501
+    def results(self):
+        """Gets the results of this MatchResponseAllOf.  # noqa: E501
 
-        Base64 encoded image.  # noqa: E501
+        The array of matching results.  # noqa: E501
 
-        :return: The content of this ImageFieldsImage.  # noqa: E501
-        :rtype: str
+        :return: The results of this MatchResponseAllOf.  # noqa: E501
+        :rtype: [MatchImageResult]
         """
-        return self._content
+        return self._results
 
-    @content.setter
-    def content(self, content):
-        """Sets the content of this ImageFieldsImage.
+    @results.setter
+    def results(self, results):
+        """Sets the results of this MatchResponseAllOf.
 
-        Base64 encoded image.  # noqa: E501
+        The array of matching results.  # noqa: E501
 
-        :param content: The content of this ImageFieldsImage.  # noqa: E501
-        :type content: str
+        :param results: The results of this MatchResponseAllOf.  # noqa: E501
+        :type results: [MatchImageResult]
         """
 
-        self._content = content
+        self._results = results
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -133,18 +133,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ImageFieldsImage):
+        if not isinstance(other, MatchResponseAllOf):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ImageFieldsImage):
+        if not isinstance(other, MatchResponseAllOf):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_page.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/image_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -36,15 +36,15 @@
         'page': 'int',
         'total_pages': 'int',
         'items': '[Image]',
     }
 
     attribute_map = {
         'page': 'page',
-        'total_pages': 'total_pages',
+        'total_pages': 'totalPages',
         'items': 'items',
     }
 
     def __init__(self, page=None, total_pages=None, items=None, local_vars_configuration=None):  # noqa: E501
         """ImagePage - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_page_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/image_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,74 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class ImagePageAllOf(object):
+class ImageSource(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+    ""
+    DOCUMENT_PRINTED = int(1)
+
+    ""
+    DOCUMENT_RFID = int(2)
+
+    ""
+    LIVE = int(3)
+
+    ""
+    DOCUMENT_WITH_LIVE = int(4)
+
+    ""
+    EXTERNAL = int(5)
+
+    ""
+    GHOST = int(6)
+
+    allowable_values = [DOCUMENT_PRINTED, DOCUMENT_RFID, LIVE, DOCUMENT_WITH_LIVE, EXTERNAL, GHOST]  # noqa: E501
+
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'items': '[Image]',
     }
 
     attribute_map = {
-        'items': 'items',
     }
 
-    def __init__(self, items=None, local_vars_configuration=None):  # noqa: E501
-        """ImagePageAllOf - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, local_vars_configuration=None):  # noqa: E501
+        """ImageSource - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
-
-        self._items = None
         self.discriminator = None
 
-        if items is not None:
-            self.items = items
-
-    @property
-    def items(self):
-        """Gets the items of this ImagePageAllOf.  # noqa: E501
-
-
-        :return: The items of this ImagePageAllOf.  # noqa: E501
-        :rtype: [Image]
-        """
-        return self._items
-
-    @items.setter
-    def items(self, items):
-        """Sets the items of this ImagePageAllOf.
-
-
-        :param items: The items of this ImagePageAllOf.  # noqa: E501
-        :type items: [Image]
-        """
-
-        self._items = items
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -103,18 +95,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ImagePageAllOf):
+        if not isinstance(other, ImageSource):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ImagePageAllOf):
+        if not isinstance(other, ImageSource):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_source.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/rgb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,49 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class ImageSource(object):
+class RGB(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
-    ""
-    DOCUMENT_PRINTED = int(1)
-
-    ""
-    DOCUMENT_RFID = int(2)
-
-    ""
-    LIVE = int(3)
-
-    ""
-    DOCUMENT_WITH_LIVE = int(4)
-
-    ""
-    EXTERNAL = int(5)
-
-    ""
-    GHOST = int(6)
-
-    allowable_values = [DOCUMENT_PRINTED, DOCUMENT_RFID, LIVE, DOCUMENT_WITH_LIVE, EXTERNAL, GHOST]  # noqa: E501
-
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """ImageSource - a model defined in OpenAPI"""  # noqa: E501
+        """RGB - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -95,18 +75,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ImageSource):
+        if not isinstance(other, RGB):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ImageSource):
+        if not isinstance(other, RGB):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/liveness_transaction.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/liveness_transaction.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,131 +29,131 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'tag': 'str',
         'images': '[MatchAndSearchRequestAllOfImages]',
-        'limit': 'int',
-        'threshold': 'float',
+        'create_person': 'SearchParametersCreatePerson',
         'group_ids': '[int]',
     }
 
     attribute_map = {
+        'tag': 'tag',
         'images': 'images',
-        'limit': 'limit',
-        'threshold': 'threshold',
-        'group_ids': 'group_ids',
+        'create_person': 'createPerson',
+        'group_ids': 'groupIds',
     }
 
-    def __init__(self, images=None, limit=100, threshold=None, group_ids=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, tag=None, images=None, create_person=None, group_ids=None, local_vars_configuration=None):  # noqa: E501
         """MatchAndSearchRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._tag = None
         self._images = None
-        self._limit = None
-        self._threshold = None
+        self._create_person = None
         self._group_ids = None
         self.discriminator = None
 
+        if tag is not None:
+            self.tag = tag
         if images is not None:
             self.images = images
-        if limit is not None:
-            self.limit = limit
-        if threshold is not None:
-            self.threshold = threshold
+        if create_person is not None:
+            self.create_person = create_person
         if group_ids is not None:
             self.group_ids = group_ids
 
     @property
+    def tag(self):
+        """Gets the tag of this MatchAndSearchRequest.  # noqa: E501
+
+        Session identificator.  # noqa: E501
+
+        :return: The tag of this MatchAndSearchRequest.  # noqa: E501
+        :rtype: str
+        """
+        return self._tag
+
+    @tag.setter
+    def tag(self, tag):
+        """Sets the tag of this MatchAndSearchRequest.
+
+        Session identificator.  # noqa: E501
+
+        :param tag: The tag of this MatchAndSearchRequest.  # noqa: E501
+        :type tag: str
+        """
+
+        self._tag = tag
+
+    @property
     def images(self):
         """Gets the images of this MatchAndSearchRequest.  # noqa: E501
 
+        Array of Person images.  # noqa: E501
 
         :return: The images of this MatchAndSearchRequest.  # noqa: E501
         :rtype: [MatchAndSearchRequestAllOfImages]
         """
         return self._images
 
     @images.setter
     def images(self, images):
         """Sets the images of this MatchAndSearchRequest.
 
+        Array of Person images.  # noqa: E501
 
         :param images: The images of this MatchAndSearchRequest.  # noqa: E501
         :type images: [MatchAndSearchRequestAllOfImages]
         """
 
         self._images = images
 
     @property
-    def limit(self):
-        """Gets the limit of this MatchAndSearchRequest.  # noqa: E501
-
-        The number of returned Persons limit.  # noqa: E501
-
-        :return: The limit of this MatchAndSearchRequest.  # noqa: E501
-        :rtype: int
-        """
-        return self._limit
-
-    @limit.setter
-    def limit(self, limit):
-        """Sets the limit of this MatchAndSearchRequest.
-
-        The number of returned Persons limit.  # noqa: E501
-
-        :param limit: The limit of this MatchAndSearchRequest.  # noqa: E501
-        :type limit: int
-        """
-
-        self._limit = limit
-
-    @property
-    def threshold(self):
-        """Gets the threshold of this MatchAndSearchRequest.  # noqa: E501
+    def create_person(self):
+        """Gets the create_person of this MatchAndSearchRequest.  # noqa: E501
 
-        The similarity distance threshold, should be between 0.0 and 2.0, where 0.0 is for returning results for only the most similar persons and 2.0 is for all the persons, even the dissimilar ones. If not set, the default 1.0 value is used.  # noqa: E501
 
-        :return: The threshold of this MatchAndSearchRequest.  # noqa: E501
-        :rtype: float
+        :return: The create_person of this MatchAndSearchRequest.  # noqa: E501
+        :rtype: SearchParametersCreatePerson
         """
-        return self._threshold
+        return self._create_person
 
-    @threshold.setter
-    def threshold(self, threshold):
-        """Sets the threshold of this MatchAndSearchRequest.
+    @create_person.setter
+    def create_person(self, create_person):
+        """Sets the create_person of this MatchAndSearchRequest.
 
-        The similarity distance threshold, should be between 0.0 and 2.0, where 0.0 is for returning results for only the most similar persons and 2.0 is for all the persons, even the dissimilar ones. If not set, the default 1.0 value is used.  # noqa: E501
 
-        :param threshold: The threshold of this MatchAndSearchRequest.  # noqa: E501
-        :type threshold: float
+        :param create_person: The create_person of this MatchAndSearchRequest.  # noqa: E501
+        :type create_person: SearchParametersCreatePerson
         """
 
-        self._threshold = threshold
+        self._create_person = create_person
 
     @property
     def group_ids(self):
         """Gets the group_ids of this MatchAndSearchRequest.  # noqa: E501
 
-        The IDs of the groups in which the search is performed.  # noqa: E501
+        IDs of the groups in which the search is performed.  # noqa: E501
 
         :return: The group_ids of this MatchAndSearchRequest.  # noqa: E501
         :rtype: [int]
         """
         return self._group_ids
 
     @group_ids.setter
     def group_ids(self, group_ids):
         """Sets the group_ids of this MatchAndSearchRequest.
 
-        The IDs of the groups in which the search is performed.  # noqa: E501
+        IDs of the groups in which the search is performed.  # noqa: E501
 
         :param group_ids: The group_ids of this MatchAndSearchRequest.  # noqa: E501
         :type group_ids: [int]
         """
 
         self._group_ids = group_ids
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_request_all_of.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,47 +29,77 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'tag': 'str',
         'images': '[MatchAndSearchRequestAllOfImages]',
     }
 
     attribute_map = {
+        'tag': 'tag',
         'images': 'images',
     }
 
-    def __init__(self, images=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, tag=None, images=None, local_vars_configuration=None):  # noqa: E501
         """MatchAndSearchRequestAllOf - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._tag = None
         self._images = None
         self.discriminator = None
 
+        if tag is not None:
+            self.tag = tag
         if images is not None:
             self.images = images
 
     @property
+    def tag(self):
+        """Gets the tag of this MatchAndSearchRequestAllOf.  # noqa: E501
+
+        Session identificator.  # noqa: E501
+
+        :return: The tag of this MatchAndSearchRequestAllOf.  # noqa: E501
+        :rtype: str
+        """
+        return self._tag
+
+    @tag.setter
+    def tag(self, tag):
+        """Sets the tag of this MatchAndSearchRequestAllOf.
+
+        Session identificator.  # noqa: E501
+
+        :param tag: The tag of this MatchAndSearchRequestAllOf.  # noqa: E501
+        :type tag: str
+        """
+
+        self._tag = tag
+
+    @property
     def images(self):
         """Gets the images of this MatchAndSearchRequestAllOf.  # noqa: E501
 
+        Array of Person images.  # noqa: E501
 
         :return: The images of this MatchAndSearchRequestAllOf.  # noqa: E501
         :rtype: [MatchAndSearchRequestAllOfImages]
         """
         return self._images
 
     @images.setter
     def images(self, images):
         """Sets the images of this MatchAndSearchRequestAllOf.
 
+        Array of Person images.  # noqa: E501
 
         :param images: The images of this MatchAndSearchRequestAllOf.  # noqa: E501
         :type images: [MatchAndSearchRequestAllOfImages]
         """
 
         self._images = images
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request_all_of_images.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_request_all_of_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_response_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response_all_of_detections.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_and_search_response_all_of_detections.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -83,26 +83,26 @@
 
         self._faces = faces
 
     @property
     def image_index(self):
         """Gets the image_index of this MatchAndSearchResponseAllOfDetections.  # noqa: E501
 
-        Image index used to identify input photos between themselves. If not specified, than input list index is used.  # noqa: E501
+        The image index number. Can be given; if not given, the index numbers are set automatically starting from 0. All index numbers must be whole and unique—not repeated.  # noqa: E501
 
         :return: The image_index of this MatchAndSearchResponseAllOfDetections.  # noqa: E501
         :rtype: int
         """
         return self._image_index
 
     @image_index.setter
     def image_index(self, image_index):
         """Sets the image_index of this MatchAndSearchResponseAllOfDetections.
 
-        Image index used to identify input photos between themselves. If not specified, than input list index is used.  # noqa: E501
+        The image index number. Can be given; if not given, the index numbers are set automatically starting from 0. All index numbers must be whole and unique—not repeated.  # noqa: E501
 
         :param image_index: The image_index of this MatchAndSearchResponseAllOfDetections.  # noqa: E501
         :type image_index: int
         """
 
         self._image_index = image_index
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person_created_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,138 +1,139 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class MatchImage(object):
+class PersonCreatedResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'index': 'int',
-        'type': 'ImageSource',
-        'data': 'str',
+        'code': 'int',
+        'persons': '[SearchPerson]',
+        'metadata': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
     }
 
     attribute_map = {
-        'index': 'index',
-        'type': 'type',
-        'data': 'data',
+        'code': 'code',
+        'persons': 'persons',
+        'metadata': 'metadata',
     }
 
-    def __init__(self, index=None, type=None, data=None, local_vars_configuration=None):  # noqa: E501
-        """MatchImage - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, code=None, persons=None, metadata=None, local_vars_configuration=None):  # noqa: E501
+        """PersonCreatedResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._index = None
-        self._type = None
-        self._data = None
+        self._code = None
+        self._persons = None
+        self._metadata = None
         self.discriminator = None
 
-        if index is not None:
-            self.index = index
-        if type is not None:
-            self.type = type
-        self.data = data
+        if code is not None:
+            self.code = code
+        if persons is not None:
+            self.persons = persons
+        if metadata is not None:
+            self.metadata = metadata
 
     @property
-    def index(self):
-        """Gets the index of this MatchImage.  # noqa: E501
+    def code(self):
+        """Gets the code of this PersonCreatedResponse.  # noqa: E501
 
-        Image index used to identify input photos between themselves. If not specified, than input list index is used.  # noqa: E501
+        Result code.  # noqa: E501
 
-        :return: The index of this MatchImage.  # noqa: E501
+        :return: The code of this PersonCreatedResponse.  # noqa: E501
         :rtype: int
         """
-        return self._index
+        return self._code
 
-    @index.setter
-    def index(self, index):
-        """Sets the index of this MatchImage.
+    @code.setter
+    def code(self, code):
+        """Sets the code of this PersonCreatedResponse.
 
-        Image index used to identify input photos between themselves. If not specified, than input list index is used.  # noqa: E501
+        Result code.  # noqa: E501
 
-        :param index: The index of this MatchImage.  # noqa: E501
-        :type index: int
+        :param code: The code of this PersonCreatedResponse.  # noqa: E501
+        :type code: int
         """
 
-        self._index = index
+        self._code = code
 
     @property
-    def type(self):
-        """Gets the type of this MatchImage.  # noqa: E501
+    def persons(self):
+        """Gets the persons of this PersonCreatedResponse.  # noqa: E501
 
+        Array of Person images.  # noqa: E501
 
-        :return: The type of this MatchImage.  # noqa: E501
-        :rtype: ImageSource
+        :return: The persons of this PersonCreatedResponse.  # noqa: E501
+        :rtype: [SearchPerson]
         """
-        return self._type
+        return self._persons
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this MatchImage.
+    @persons.setter
+    def persons(self, persons):
+        """Sets the persons of this PersonCreatedResponse.
 
+        Array of Person images.  # noqa: E501
 
-        :param type: The type of this MatchImage.  # noqa: E501
-        :type type: ImageSource
+        :param persons: The persons of this PersonCreatedResponse.  # noqa: E501
+        :type persons: [SearchPerson]
         """
 
-        self._type = type
+        self._persons = persons
 
     @property
-    def data(self):
-        """Gets the data of this MatchImage.  # noqa: E501
+    def metadata(self):
+        """Gets the metadata of this PersonCreatedResponse.  # noqa: E501
 
-        Base64 encoded image.  # noqa: E501
+        A free-form object containing person's extended attributes.  # noqa: E501
 
-        :return: The data of this MatchImage.  # noqa: E501
-        :rtype: str
+        :return: The metadata of this PersonCreatedResponse.  # noqa: E501
+        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
-        return self._data
+        return self._metadata
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this MatchImage.
+    @metadata.setter
+    def metadata(self, metadata):
+        """Sets the metadata of this PersonCreatedResponse.
 
-        Base64 encoded image.  # noqa: E501
+        A free-form object containing person's extended attributes.  # noqa: E501
 
-        :param data: The data of this MatchImage.  # noqa: E501
-        :type data: str
+        :param metadata: The metadata of this PersonCreatedResponse.  # noqa: E501
+        :type metadata: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
-        if self.local_vars_configuration.client_side_validation and data is None:  # noqa: E501
-            raise ValueError("Invalid value for `data`, must not be `None`")  # noqa: E501
 
-        self._data = data
+        self._metadata = metadata
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -160,18 +161,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MatchImage):
+        if not isinstance(other, PersonCreatedResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MatchImage):
+        if not isinstance(other, PersonCreatedResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image_detection.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_image_detection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -60,47 +60,49 @@
         self.image_index = image_index
         self.status = status
 
     @property
     def faces(self):
         """Gets the faces of this MatchImageDetection.  # noqa: E501
 
+        The array of detected faces.  # noqa: E501
 
         :return: The faces of this MatchImageDetection.  # noqa: E501
         :rtype: [DetectionFace]
         """
         return self._faces
 
     @faces.setter
     def faces(self, faces):
         """Sets the faces of this MatchImageDetection.
 
+        The array of detected faces.  # noqa: E501
 
         :param faces: The faces of this MatchImageDetection.  # noqa: E501
         :type faces: [DetectionFace]
         """
 
         self._faces = faces
 
     @property
     def image_index(self):
         """Gets the image_index of this MatchImageDetection.  # noqa: E501
 
-        Image index used to identify input photos between themselves. If not specified, than input list index is used.  # noqa: E501
+        The image index number. Can be given; if not given, the index numbers are set automatically starting from 0. All index numbers must be whole and unique—not repeated.  # noqa: E501
 
         :return: The image_index of this MatchImageDetection.  # noqa: E501
         :rtype: int
         """
         return self._image_index
 
     @image_index.setter
     def image_index(self, image_index):
         """Sets the image_index of this MatchImageDetection.
 
-        Image index used to identify input photos between themselves. If not specified, than input list index is used.  # noqa: E501
+        The image index number. Can be given; if not given, the index numbers are set automatically starting from 0. All index numbers must be whole and unique—not repeated.  # noqa: E501
 
         :param image_index: The image_index of this MatchImageDetection.  # noqa: E501
         :type image_index: int
         """
         if self.local_vars_configuration.client_side_validation and image_index is None:  # noqa: E501
             raise ValueError("Invalid value for `image_index`, must not be `None`")  # noqa: E501
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image_result.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_image_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -31,250 +31,248 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'first_index': 'int',
         'first_face_index': 'float',
+        'first': 'ImageSource',
         'second_index': 'int',
         'second_face_index': 'float',
+        'second': 'ImageSource',
         'score': 'float',
         'similarity': 'float',
-        'error_code': 'FaceSDKResultCode',
-        'error_msg': 'str',
     }
 
     attribute_map = {
         'first_index': 'firstIndex',
         'first_face_index': 'firstFaceIndex',
+        'first': 'first',
         'second_index': 'secondIndex',
         'second_face_index': 'secondFaceIndex',
+        'second': 'second',
         'score': 'score',
         'similarity': 'similarity',
-        'error_code': 'errorCode',
-        'error_msg': 'errorMsg',
     }
 
-    def __init__(self, first_index=None, first_face_index=None, second_index=None, second_face_index=None, score=None, similarity=None, error_code=None, error_msg=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, first_index=None, first_face_index=None, first=None, second_index=None, second_face_index=None, second=None, score=None, similarity=None, local_vars_configuration=None):  # noqa: E501
         """MatchImageResult - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._first_index = None
         self._first_face_index = None
+        self._first = None
         self._second_index = None
         self._second_face_index = None
+        self._second = None
         self._score = None
         self._similarity = None
-        self._error_code = None
-        self._error_msg = None
         self.discriminator = None
 
         self.first_index = first_index
         if first_face_index is not None:
             self.first_face_index = first_face_index
+        if first is not None:
+            self.first = first
         self.second_index = second_index
         if second_face_index is not None:
             self.second_face_index = second_face_index
+        if second is not None:
+            self.second = second
         if score is not None:
             self.score = score
         if similarity is not None:
             self.similarity = similarity
-        if error_code is not None:
-            self.error_code = error_code
-        if error_msg is not None:
-            self.error_msg = error_msg
 
     @property
     def first_index(self):
         """Gets the first_index of this MatchImageResult.  # noqa: E501
 
-        Image index used to identify input photos between themselves. If not specified, than input list index is used.  # noqa: E501
+        The image index number. Can be given; if not given, the index numbers are set automatically starting from 0. All index numbers must be whole and unique—not repeated.  # noqa: E501
 
         :return: The first_index of this MatchImageResult.  # noqa: E501
         :rtype: int
         """
         return self._first_index
 
     @first_index.setter
     def first_index(self, first_index):
         """Sets the first_index of this MatchImageResult.
 
-        Image index used to identify input photos between themselves. If not specified, than input list index is used.  # noqa: E501
+        The image index number. Can be given; if not given, the index numbers are set automatically starting from 0. All index numbers must be whole and unique—not repeated.  # noqa: E501
 
         :param first_index: The first_index of this MatchImageResult.  # noqa: E501
         :type first_index: int
         """
         if self.local_vars_configuration.client_side_validation and first_index is None:  # noqa: E501
             raise ValueError("Invalid value for `first_index`, must not be `None`")  # noqa: E501
 
         self._first_index = first_index
 
     @property
     def first_face_index(self):
         """Gets the first_face_index of this MatchImageResult.  # noqa: E501
 
-        Faces index used to identify faces in scope of one photo.  # noqa: E501
+        The detected face index number.  # noqa: E501
 
         :return: The first_face_index of this MatchImageResult.  # noqa: E501
         :rtype: float
         """
         return self._first_face_index
 
     @first_face_index.setter
     def first_face_index(self, first_face_index):
         """Sets the first_face_index of this MatchImageResult.
 
-        Faces index used to identify faces in scope of one photo.  # noqa: E501
+        The detected face index number.  # noqa: E501
 
         :param first_face_index: The first_face_index of this MatchImageResult.  # noqa: E501
         :type first_face_index: float
         """
 
         self._first_face_index = first_face_index
 
     @property
+    def first(self):
+        """Gets the first of this MatchImageResult.  # noqa: E501
+
+
+        :return: The first of this MatchImageResult.  # noqa: E501
+        :rtype: ImageSource
+        """
+        return self._first
+
+    @first.setter
+    def first(self, first):
+        """Sets the first of this MatchImageResult.
+
+
+        :param first: The first of this MatchImageResult.  # noqa: E501
+        :type first: ImageSource
+        """
+
+        self._first = first
+
+    @property
     def second_index(self):
         """Gets the second_index of this MatchImageResult.  # noqa: E501
 
-        Image index used to identify input photos between themselves. If not specified, than input list index is used.  # noqa: E501
+        The image index number. Can be given; if not given, the index numbers are set automatically starting from 0. All index numbers must be whole and unique—not repeated.  # noqa: E501
 
         :return: The second_index of this MatchImageResult.  # noqa: E501
         :rtype: int
         """
         return self._second_index
 
     @second_index.setter
     def second_index(self, second_index):
         """Sets the second_index of this MatchImageResult.
 
-        Image index used to identify input photos between themselves. If not specified, than input list index is used.  # noqa: E501
+        The image index number. Can be given; if not given, the index numbers are set automatically starting from 0. All index numbers must be whole and unique—not repeated.  # noqa: E501
 
         :param second_index: The second_index of this MatchImageResult.  # noqa: E501
         :type second_index: int
         """
         if self.local_vars_configuration.client_side_validation and second_index is None:  # noqa: E501
             raise ValueError("Invalid value for `second_index`, must not be `None`")  # noqa: E501
 
         self._second_index = second_index
 
     @property
     def second_face_index(self):
         """Gets the second_face_index of this MatchImageResult.  # noqa: E501
 
-        Faces index used to identify faces in scope of one photo.  # noqa: E501
+        The detected face index number.  # noqa: E501
 
         :return: The second_face_index of this MatchImageResult.  # noqa: E501
         :rtype: float
         """
         return self._second_face_index
 
     @second_face_index.setter
     def second_face_index(self, second_face_index):
         """Sets the second_face_index of this MatchImageResult.
 
-        Faces index used to identify faces in scope of one photo.  # noqa: E501
+        The detected face index number.  # noqa: E501
 
         :param second_face_index: The second_face_index of this MatchImageResult.  # noqa: E501
         :type second_face_index: float
         """
 
         self._second_face_index = second_face_index
 
     @property
+    def second(self):
+        """Gets the second of this MatchImageResult.  # noqa: E501
+
+
+        :return: The second of this MatchImageResult.  # noqa: E501
+        :rtype: ImageSource
+        """
+        return self._second
+
+    @second.setter
+    def second(self, second):
+        """Sets the second of this MatchImageResult.
+
+
+        :param second: The second of this MatchImageResult.  # noqa: E501
+        :type second: ImageSource
+        """
+
+        self._second = second
+
+    @property
     def score(self):
         """Gets the score of this MatchImageResult.  # noqa: E501
 
-        The matching score.  # noqa: E501
+        A dimensionless number that shows how similar the compared faces are. 0—absolutely identical faces.  # noqa: E501
 
         :return: The score of this MatchImageResult.  # noqa: E501
         :rtype: float
         """
         return self._score
 
     @score.setter
     def score(self, score):
         """Sets the score of this MatchImageResult.
 
-        The matching score.  # noqa: E501
+        A dimensionless number that shows how similar the compared faces are. 0—absolutely identical faces.  # noqa: E501
 
         :param score: The score of this MatchImageResult.  # noqa: E501
         :type score: float
         """
 
         self._score = score
 
     @property
     def similarity(self):
         """Gets the similarity of this MatchImageResult.  # noqa: E501
 
-        The similarity score.  # noqa: E501
+        The detected faces similarity, %. 100%—absolutely identical faces, 0%—absolutely not identical.  # noqa: E501
 
         :return: The similarity of this MatchImageResult.  # noqa: E501
         :rtype: float
         """
         return self._similarity
 
     @similarity.setter
     def similarity(self, similarity):
         """Sets the similarity of this MatchImageResult.
 
-        The similarity score.  # noqa: E501
+        The detected faces similarity, %. 100%—absolutely identical faces, 0%—absolutely not identical.  # noqa: E501
 
         :param similarity: The similarity of this MatchImageResult.  # noqa: E501
         :type similarity: float
         """
 
         self._similarity = similarity
 
-    @property
-    def error_code(self):
-        """Gets the error_code of this MatchImageResult.  # noqa: E501
-
-
-        :return: The error_code of this MatchImageResult.  # noqa: E501
-        :rtype: FaceSDKResultCode
-        """
-        return self._error_code
-
-    @error_code.setter
-    def error_code(self, error_code):
-        """Sets the error_code of this MatchImageResult.
-
-
-        :param error_code: The error_code of this MatchImageResult.  # noqa: E501
-        :type error_code: FaceSDKResultCode
-        """
-
-        self._error_code = error_code
-
-    @property
-    def error_msg(self):
-        """Gets the error_msg of this MatchImageResult.  # noqa: E501
-
-        The error message if any.  # noqa: E501
-
-        :return: The error_msg of this MatchImageResult.  # noqa: E501
-        :rtype: str
-        """
-        return self._error_msg
-
-    @error_msg.setter
-    def error_msg(self, error_msg):
-        """Sets the error_msg of this MatchImageResult.
-
-        The error message if any.  # noqa: E501
-
-        :param error_msg: The error_msg of this MatchImageResult.  # noqa: E501
-        :type error_msg: str
-        """
-
-        self._error_msg = error_msg
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_request.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,138 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class MatchRequest(object):
+class MatchResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'tag': 'str',
-        'thumbnails': 'bool',
-        'images': '[MatchImage]',
+        'code': 'FaceSDKResultCode',
+        'detections': '[MatchImageDetection]',
+        'results': '[MatchImageResult]',
     }
 
     attribute_map = {
-        'tag': 'tag',
-        'thumbnails': 'thumbnails',
-        'images': 'images',
+        'code': 'code',
+        'detections': 'detections',
+        'results': 'results',
     }
 
-    def __init__(self, tag=None, thumbnails=False, images=None, local_vars_configuration=None):  # noqa: E501
-        """MatchRequest - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, code=None, detections=None, results=None, local_vars_configuration=None):  # noqa: E501
+        """MatchResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._tag = None
-        self._thumbnails = None
-        self._images = None
+        self._code = None
+        self._detections = None
+        self._results = None
         self.discriminator = None
 
-        if tag is not None:
-            self.tag = tag
-        if thumbnails is not None:
-            self.thumbnails = thumbnails
-        self.images = images
+        self.code = code
+        if detections is not None:
+            self.detections = detections
+        if results is not None:
+            self.results = results
 
     @property
-    def tag(self):
-        """Gets the tag of this MatchRequest.  # noqa: E501
+    def code(self):
+        """Gets the code of this MatchResponse.  # noqa: E501
 
-        Session identificator.  # noqa: E501
 
-        :return: The tag of this MatchRequest.  # noqa: E501
-        :rtype: str
+        :return: The code of this MatchResponse.  # noqa: E501
+        :rtype: FaceSDKResultCode
         """
-        return self._tag
+        return self._code
 
-    @tag.setter
-    def tag(self, tag):
-        """Sets the tag of this MatchRequest.
+    @code.setter
+    def code(self, code):
+        """Sets the code of this MatchResponse.
 
-        Session identificator.  # noqa: E501
 
-        :param tag: The tag of this MatchRequest.  # noqa: E501
-        :type tag: str
+        :param code: The code of this MatchResponse.  # noqa: E501
+        :type code: FaceSDKResultCode
         """
+        if self.local_vars_configuration.client_side_validation and code is None:  # noqa: E501
+            raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
 
-        self._tag = tag
+        self._code = code
 
     @property
-    def thumbnails(self):
-        """Gets the thumbnails of this MatchRequest.  # noqa: E501
+    def detections(self):
+        """Gets the detections of this MatchResponse.  # noqa: E501
 
-        Whether to return cropped portraits of the detected people.  # noqa: E501
+        The array of detected faces.  # noqa: E501
 
-        :return: The thumbnails of this MatchRequest.  # noqa: E501
-        :rtype: bool
+        :return: The detections of this MatchResponse.  # noqa: E501
+        :rtype: [MatchImageDetection]
         """
-        return self._thumbnails
+        return self._detections
 
-    @thumbnails.setter
-    def thumbnails(self, thumbnails):
-        """Sets the thumbnails of this MatchRequest.
+    @detections.setter
+    def detections(self, detections):
+        """Sets the detections of this MatchResponse.
 
-        Whether to return cropped portraits of the detected people.  # noqa: E501
+        The array of detected faces.  # noqa: E501
 
-        :param thumbnails: The thumbnails of this MatchRequest.  # noqa: E501
-        :type thumbnails: bool
+        :param detections: The detections of this MatchResponse.  # noqa: E501
+        :type detections: [MatchImageDetection]
         """
 
-        self._thumbnails = thumbnails
+        self._detections = detections
 
     @property
-    def images(self):
-        """Gets the images of this MatchRequest.  # noqa: E501
+    def results(self):
+        """Gets the results of this MatchResponse.  # noqa: E501
 
-        Base64 images.  # noqa: E501
+        The array of matching results.  # noqa: E501
 
-        :return: The images of this MatchRequest.  # noqa: E501
-        :rtype: [MatchImage]
+        :return: The results of this MatchResponse.  # noqa: E501
+        :rtype: [MatchImageResult]
         """
-        return self._images
+        return self._results
 
-    @images.setter
-    def images(self, images):
-        """Sets the images of this MatchRequest.
+    @results.setter
+    def results(self, results):
+        """Sets the results of this MatchResponse.
 
-        Base64 images.  # noqa: E501
+        The array of matching results.  # noqa: E501
 
-        :param images: The images of this MatchRequest.  # noqa: E501
-        :type images: [MatchImage]
+        :param results: The results of this MatchResponse.  # noqa: E501
+        :type results: [MatchImageResult]
         """
-        if self.local_vars_configuration.client_side_validation and images is None:  # noqa: E501
-            raise ValueError("Invalid value for `images`, must not be `None`")  # noqa: E501
 
-        self._images = images
+        self._results = results
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -162,18 +160,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MatchRequest):
+        if not isinstance(other, MatchResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MatchRequest):
+        if not isinstance(other, MatchResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_response.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_request_all_of.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,139 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 4.1.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class MatchResponse(object):
+class SearchRequestAllOf(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'code': 'FaceSDKResultCode',
-        'results': '[MatchImageResult]',
-        'detections': '[MatchImageDetection]',
+        'limit': 'int',
+        'threshold': 'float',
+        'group_ids': '[int]',
     }
 
     attribute_map = {
-        'code': 'code',
-        'results': 'results',
-        'detections': 'detections',
+        'limit': 'limit',
+        'threshold': 'threshold',
+        'group_ids': 'group_ids',
     }
 
-    def __init__(self, code=None, results=None, detections=None, local_vars_configuration=None):  # noqa: E501
-        """MatchResponse - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, limit=100, threshold=None, group_ids=None, local_vars_configuration=None):  # noqa: E501
+        """SearchRequestAllOf - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._code = None
-        self._results = None
-        self._detections = None
+        self._limit = None
+        self._threshold = None
+        self._group_ids = None
         self.discriminator = None
 
-        self.code = code
-        if results is not None:
-            self.results = results
-        if detections is not None:
-            self.detections = detections
+        if limit is not None:
+            self.limit = limit
+        if threshold is not None:
+            self.threshold = threshold
+        if group_ids is not None:
+            self.group_ids = group_ids
 
     @property
-    def code(self):
-        """Gets the code of this MatchResponse.  # noqa: E501
+    def limit(self):
+        """Gets the limit of this SearchRequestAllOf.  # noqa: E501
 
+        The number of returned Persons limit.  # noqa: E501
 
-        :return: The code of this MatchResponse.  # noqa: E501
-        :rtype: FaceSDKResultCode
+        :return: The limit of this SearchRequestAllOf.  # noqa: E501
+        :rtype: int
         """
-        return self._code
+        return self._limit
 
-    @code.setter
-    def code(self, code):
-        """Sets the code of this MatchResponse.
+    @limit.setter
+    def limit(self, limit):
+        """Sets the limit of this SearchRequestAllOf.
 
+        The number of returned Persons limit.  # noqa: E501
 
-        :param code: The code of this MatchResponse.  # noqa: E501
-        :type code: FaceSDKResultCode
+        :param limit: The limit of this SearchRequestAllOf.  # noqa: E501
+        :type limit: int
         """
-        if self.local_vars_configuration.client_side_validation and code is None:  # noqa: E501
-            raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
 
-        self._code = code
+        self._limit = limit
 
     @property
-    def results(self):
-        """Gets the results of this MatchResponse.  # noqa: E501
+    def threshold(self):
+        """Gets the threshold of this SearchRequestAllOf.  # noqa: E501
 
-        The array of matching results.  # noqa: E501
+        Similarity threshold.  # noqa: E501
 
-        :return: The results of this MatchResponse.  # noqa: E501
-        :rtype: [MatchImageResult]
+        :return: The threshold of this SearchRequestAllOf.  # noqa: E501
+        :rtype: float
         """
-        return self._results
+        return self._threshold
 
-    @results.setter
-    def results(self, results):
-        """Sets the results of this MatchResponse.
+    @threshold.setter
+    def threshold(self, threshold):
+        """Sets the threshold of this SearchRequestAllOf.
 
-        The array of matching results.  # noqa: E501
+        Similarity threshold.  # noqa: E501
 
-        :param results: The results of this MatchResponse.  # noqa: E501
-        :type results: [MatchImageResult]
+        :param threshold: The threshold of this SearchRequestAllOf.  # noqa: E501
+        :type threshold: float
         """
 
-        self._results = results
+        self._threshold = threshold
 
     @property
-    def detections(self):
-        """Gets the detections of this MatchResponse.  # noqa: E501
+    def group_ids(self):
+        """Gets the group_ids of this SearchRequestAllOf.  # noqa: E501
 
+        The IDs of the groups in which the search is performed.  # noqa: E501
 
-        :return: The detections of this MatchResponse.  # noqa: E501
-        :rtype: [MatchImageDetection]
+        :return: The group_ids of this SearchRequestAllOf.  # noqa: E501
+        :rtype: [int]
         """
-        return self._detections
+        return self._group_ids
 
-    @detections.setter
-    def detections(self, detections):
-        """Sets the detections of this MatchResponse.
+    @group_ids.setter
+    def group_ids(self, group_ids):
+        """Sets the group_ids of this SearchRequestAllOf.
 
+        The IDs of the groups in which the search is performed.  # noqa: E501
 
-        :param detections: The detections of this MatchResponse.  # noqa: E501
-        :type detections: [MatchImageDetection]
+        :param group_ids: The group_ids of this SearchRequestAllOf.  # noqa: E501
+        :type group_ids: [int]
         """
 
-        self._detections = detections
+        self._group_ids = group_ids
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -158,18 +161,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MatchResponse):
+        if not isinstance(other, SearchRequestAllOf):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MatchResponse):
+        if not isinstance(other, SearchRequestAllOf):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_response_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_person_all_of.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class MatchResponseAllOf(object):
+class SearchPersonAllOf(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'results': '[MatchImageResult]',
-        'detections': '[MatchImageDetection]',
+        'detection': 'SearchDetection',
+        'images': '[RecognizeImage]',
     }
 
     attribute_map = {
-        'results': 'results',
-        'detections': 'detections',
+        'detection': 'detection',
+        'images': 'images',
     }
 
-    def __init__(self, results=None, detections=None, local_vars_configuration=None):  # noqa: E501
-        """MatchResponseAllOf - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, detection=None, images=None, local_vars_configuration=None):  # noqa: E501
+        """SearchPersonAllOf - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._results = None
-        self._detections = None
+        self._detection = None
+        self._images = None
         self.discriminator = None
 
-        if results is not None:
-            self.results = results
-        if detections is not None:
-            self.detections = detections
+        if detection is not None:
+            self.detection = detection
+        if images is not None:
+            self.images = images
 
     @property
-    def results(self):
-        """Gets the results of this MatchResponseAllOf.  # noqa: E501
+    def detection(self):
+        """Gets the detection of this SearchPersonAllOf.  # noqa: E501
 
-        The array of matching results.  # noqa: E501
 
-        :return: The results of this MatchResponseAllOf.  # noqa: E501
-        :rtype: [MatchImageResult]
+        :return: The detection of this SearchPersonAllOf.  # noqa: E501
+        :rtype: SearchDetection
         """
-        return self._results
+        return self._detection
 
-    @results.setter
-    def results(self, results):
-        """Sets the results of this MatchResponseAllOf.
+    @detection.setter
+    def detection(self, detection):
+        """Sets the detection of this SearchPersonAllOf.
 
-        The array of matching results.  # noqa: E501
 
-        :param results: The results of this MatchResponseAllOf.  # noqa: E501
-        :type results: [MatchImageResult]
+        :param detection: The detection of this SearchPersonAllOf.  # noqa: E501
+        :type detection: SearchDetection
         """
 
-        self._results = results
+        self._detection = detection
 
     @property
-    def detections(self):
-        """Gets the detections of this MatchResponseAllOf.  # noqa: E501
+    def images(self):
+        """Gets the images of this SearchPersonAllOf.  # noqa: E501
 
+        Array of Person images.  # noqa: E501
 
-        :return: The detections of this MatchResponseAllOf.  # noqa: E501
-        :rtype: [MatchImageDetection]
+        :return: The images of this SearchPersonAllOf.  # noqa: E501
+        :rtype: [RecognizeImage]
         """
-        return self._detections
+        return self._images
 
-    @detections.setter
-    def detections(self, detections):
-        """Sets the detections of this MatchResponseAllOf.
+    @images.setter
+    def images(self, images):
+        """Sets the images of this SearchPersonAllOf.
 
+        Array of Person images.  # noqa: E501
 
-        :param detections: The detections of this MatchResponseAllOf.  # noqa: E501
-        :type detections: [MatchImageDetection]
+        :param images: The images of this SearchPersonAllOf.  # noqa: E501
+        :type images: [RecognizeImage]
         """
 
-        self._detections = detections
+        self._images = images
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -131,18 +131,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MatchResponseAllOf):
+        if not isinstance(other, SearchPersonAllOf):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MatchResponseAllOf):
+        if not isinstance(other, SearchPersonAllOf):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/operation_log.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/operation_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -35,15 +35,15 @@
     openapi_types = {
         'status_code': 'int',
         'type': 'str',
         'msg': 'str',
     }
 
     attribute_map = {
-        'status_code': 'status_code',
+        'status_code': 'statusCode',
         'type': 'type',
         'msg': 'msg',
     }
 
     def __init__(self, status_code=None, type=None, msg=None, local_vars_configuration=None):  # noqa: E501
         """OperationLog - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/output_image_params.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/output_image_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/page.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -35,15 +35,15 @@
     openapi_types = {
         'page': 'int',
         'total_pages': 'int',
     }
 
     attribute_map = {
         'page': 'page',
-        'total_pages': 'total_pages',
+        'total_pages': 'totalPages',
     }
 
     def __init__(self, page=None, total_pages=None, local_vars_configuration=None):  # noqa: E501
         """Page - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,54 +29,87 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'tag': 'str',
         'name': 'str',
         'metadata': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
-        'id': 'int',
+        'groups': '[str]',
+        'id': 'str',
         'created_at': 'str',
         'updated_at': 'str',
     }
 
     attribute_map = {
+        'tag': 'tag',
         'name': 'name',
         'metadata': 'metadata',
+        'groups': 'groups',
         'id': 'id',
-        'created_at': 'created_at',
-        'updated_at': 'updated_at',
+        'created_at': 'createdAt',
+        'updated_at': 'updatedAt',
     }
 
-    def __init__(self, name=None, metadata=None, id=None, created_at=None, updated_at=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, tag=None, name=None, metadata=None, groups=None, id=None, created_at=None, updated_at=None, local_vars_configuration=None):  # noqa: E501
         """Person - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._tag = None
         self._name = None
         self._metadata = None
+        self._groups = None
         self._id = None
         self._created_at = None
         self._updated_at = None
         self.discriminator = None
 
+        if tag is not None:
+            self.tag = tag
         if name is not None:
             self.name = name
         if metadata is not None:
             self.metadata = metadata
+        if groups is not None:
+            self.groups = groups
         if id is not None:
             self.id = id
         if created_at is not None:
             self.created_at = created_at
         if updated_at is not None:
             self.updated_at = updated_at
 
     @property
+    def tag(self):
+        """Gets the tag of this Person.  # noqa: E501
+
+        Session identificator.  # noqa: E501
+
+        :return: The tag of this Person.  # noqa: E501
+        :rtype: str
+        """
+        return self._tag
+
+    @tag.setter
+    def tag(self, tag):
+        """Sets the tag of this Person.
+
+        Session identificator.  # noqa: E501
+
+        :param tag: The tag of this Person.  # noqa: E501
+        :type tag: str
+        """
+
+        self._tag = tag
+
+    @property
     def name(self):
         """Gets the name of this Person.  # noqa: E501
 
         Person name.  # noqa: E501
 
         :return: The name of this Person.  # noqa: E501
         :rtype: str
@@ -115,32 +148,55 @@
         :param metadata: The metadata of this Person.  # noqa: E501
         :type metadata: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
 
         self._metadata = metadata
 
     @property
+    def groups(self):
+        """Gets the groups of this Person.  # noqa: E501
+
+        List of groups this person belongs to.  # noqa: E501
+
+        :return: The groups of this Person.  # noqa: E501
+        :rtype: [str]
+        """
+        return self._groups
+
+    @groups.setter
+    def groups(self, groups):
+        """Sets the groups of this Person.
+
+        List of groups this person belongs to.  # noqa: E501
+
+        :param groups: The groups of this Person.  # noqa: E501
+        :type groups: [str]
+        """
+
+        self._groups = groups
+
+    @property
     def id(self):
         """Gets the id of this Person.  # noqa: E501
 
-        Person ID.  # noqa: E501
+        Person ID. The list of persons is sorted by decreasing ID value.  # noqa: E501
 
         :return: The id of this Person.  # noqa: E501
-        :rtype: int
+        :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this Person.
 
-        Person ID.  # noqa: E501
+        Person ID. The list of persons is sorted by decreasing ID value.  # noqa: E501
 
         :param id: The id of this Person.  # noqa: E501
-        :type id: int
+        :type id: str
         """
 
         self._id = id
 
     @property
     def created_at(self):
         """Gets the created_at of this Person.  # noqa: E501
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person_all_of.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,62 +29,67 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'int',
+        'id': 'str',
         'created_at': 'str',
         'updated_at': 'str',
+        'groups': '[str]',
     }
 
     attribute_map = {
         'id': 'id',
-        'created_at': 'created_at',
-        'updated_at': 'updated_at',
+        'created_at': 'createdAt',
+        'updated_at': 'updatedAt',
+        'groups': 'groups',
     }
 
-    def __init__(self, id=None, created_at=None, updated_at=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, created_at=None, updated_at=None, groups=None, local_vars_configuration=None):  # noqa: E501
         """PersonAllOf - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._created_at = None
         self._updated_at = None
+        self._groups = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         if created_at is not None:
             self.created_at = created_at
         if updated_at is not None:
             self.updated_at = updated_at
+        if groups is not None:
+            self.groups = groups
 
     @property
     def id(self):
         """Gets the id of this PersonAllOf.  # noqa: E501
 
-        Person ID.  # noqa: E501
+        Person ID. The list of persons is sorted by decreasing ID value.  # noqa: E501
 
         :return: The id of this PersonAllOf.  # noqa: E501
-        :rtype: int
+        :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this PersonAllOf.
 
-        Person ID.  # noqa: E501
+        Person ID. The list of persons is sorted by decreasing ID value.  # noqa: E501
 
         :param id: The id of this PersonAllOf.  # noqa: E501
-        :type id: int
+        :type id: str
         """
 
         self._id = id
 
     @property
     def created_at(self):
         """Gets the created_at of this PersonAllOf.  # noqa: E501
@@ -127,14 +132,37 @@
 
         :param updated_at: The updated_at of this PersonAllOf.  # noqa: E501
         :type updated_at: str
         """
 
         self._updated_at = updated_at
 
+    @property
+    def groups(self):
+        """Gets the groups of this PersonAllOf.  # noqa: E501
+
+        List of groups this person belongs to.  # noqa: E501
+
+        :return: The groups of this PersonAllOf.  # noqa: E501
+        :rtype: [str]
+        """
+        return self._groups
+
+    @groups.setter
+    def groups(self, groups):
+        """Sets the groups of this PersonAllOf.
+
+        List of groups this person belongs to.  # noqa: E501
+
+        :param groups: The groups of this PersonAllOf.  # noqa: E501
+        :type groups: [str]
+        """
+
+        self._groups = groups
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_fields.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/match_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,140 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class PersonFields(object):
+class MatchRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
-        'metadata': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
+        'tag': 'str',
+        'thumbnails': 'bool',
+        'images': '[MatchImage]',
     }
 
     attribute_map = {
-        'name': 'name',
-        'metadata': 'metadata',
+        'tag': 'tag',
+        'thumbnails': 'thumbnails',
+        'images': 'images',
     }
 
-    def __init__(self, name=None, metadata=None, local_vars_configuration=None):  # noqa: E501
-        """PersonFields - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, tag=None, thumbnails=False, images=None, local_vars_configuration=None):  # noqa: E501
+        """MatchRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self._metadata = None
+        self._tag = None
+        self._thumbnails = None
+        self._images = None
         self.discriminator = None
 
-        if name is not None:
-            self.name = name
-        if metadata is not None:
-            self.metadata = metadata
+        if tag is not None:
+            self.tag = tag
+        if thumbnails is not None:
+            self.thumbnails = thumbnails
+        self.images = images
 
     @property
-    def name(self):
-        """Gets the name of this PersonFields.  # noqa: E501
+    def tag(self):
+        """Gets the tag of this MatchRequest.  # noqa: E501
 
-        Person name.  # noqa: E501
+        Session identificator.  # noqa: E501
 
-        :return: The name of this PersonFields.  # noqa: E501
+        :return: The tag of this MatchRequest.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._tag
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this PersonFields.
+    @tag.setter
+    def tag(self, tag):
+        """Sets the tag of this MatchRequest.
 
-        Person name.  # noqa: E501
+        Session identificator.  # noqa: E501
 
-        :param name: The name of this PersonFields.  # noqa: E501
-        :type name: str
+        :param tag: The tag of this MatchRequest.  # noqa: E501
+        :type tag: str
         """
 
-        self._name = name
+        self._tag = tag
 
     @property
-    def metadata(self):
-        """Gets the metadata of this PersonFields.  # noqa: E501
+    def thumbnails(self):
+        """Gets the thumbnails of this MatchRequest.  # noqa: E501
 
-        A free-form object containing person's extended attributes.  # noqa: E501
+        Whether to return thumbnails: Base64 cropped images that contain vertically aligned faces.  # noqa: E501
 
-        :return: The metadata of this PersonFields.  # noqa: E501
-        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :return: The thumbnails of this MatchRequest.  # noqa: E501
+        :rtype: bool
         """
-        return self._metadata
+        return self._thumbnails
 
-    @metadata.setter
-    def metadata(self, metadata):
-        """Sets the metadata of this PersonFields.
+    @thumbnails.setter
+    def thumbnails(self, thumbnails):
+        """Sets the thumbnails of this MatchRequest.
 
-        A free-form object containing person's extended attributes.  # noqa: E501
+        Whether to return thumbnails: Base64 cropped images that contain vertically aligned faces.  # noqa: E501
 
-        :param metadata: The metadata of this PersonFields.  # noqa: E501
-        :type metadata: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :param thumbnails: The thumbnails of this MatchRequest.  # noqa: E501
+        :type thumbnails: bool
         """
 
-        self._metadata = metadata
+        self._thumbnails = thumbnails
+
+    @property
+    def images(self):
+        """Gets the images of this MatchRequest.  # noqa: E501
+
+        The array of all images included in the comparison.  # noqa: E501
+
+        :return: The images of this MatchRequest.  # noqa: E501
+        :rtype: [MatchImage]
+        """
+        return self._images
+
+    @images.setter
+    def images(self, images):
+        """Sets the images of this MatchRequest.
+
+        The array of all images included in the comparison.  # noqa: E501
+
+        :param images: The images of this MatchRequest.  # noqa: E501
+        :type images: [MatchImage]
+        """
+        if self.local_vars_configuration.client_side_validation and images is None:  # noqa: E501
+            raise ValueError("Invalid value for `images`, must not be `None`")  # noqa: E501
+
+        self._images = images
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -133,18 +162,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PersonFields):
+        if not isinstance(other, MatchRequest):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, PersonFields):
+        if not isinstance(other, MatchRequest):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_with_images.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person_with_images.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -30,50 +30,60 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'images': '[RecognizeImage]',
+        'tag': 'str',
         'name': 'str',
         'metadata': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
-        'id': 'int',
+        'groups': '[str]',
+        'id': 'str',
         'created_at': 'str',
         'updated_at': 'str',
     }
 
     attribute_map = {
         'images': 'images',
+        'tag': 'tag',
         'name': 'name',
         'metadata': 'metadata',
+        'groups': 'groups',
         'id': 'id',
-        'created_at': 'created_at',
-        'updated_at': 'updated_at',
+        'created_at': 'createdAt',
+        'updated_at': 'updatedAt',
     }
 
-    def __init__(self, images=None, name=None, metadata=None, id=None, created_at=None, updated_at=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, images=None, tag=None, name=None, metadata=None, groups=None, id=None, created_at=None, updated_at=None, local_vars_configuration=None):  # noqa: E501
         """PersonWithImages - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._images = None
+        self._tag = None
         self._name = None
         self._metadata = None
+        self._groups = None
         self._id = None
         self._created_at = None
         self._updated_at = None
         self.discriminator = None
 
         if images is not None:
             self.images = images
+        if tag is not None:
+            self.tag = tag
         if name is not None:
             self.name = name
         if metadata is not None:
             self.metadata = metadata
+        if groups is not None:
+            self.groups = groups
         if id is not None:
             self.id = id
         if created_at is not None:
             self.created_at = created_at
         if updated_at is not None:
             self.updated_at = updated_at
 
@@ -95,14 +105,37 @@
         :param images: The images of this PersonWithImages.  # noqa: E501
         :type images: [RecognizeImage]
         """
 
         self._images = images
 
     @property
+    def tag(self):
+        """Gets the tag of this PersonWithImages.  # noqa: E501
+
+        Session identificator.  # noqa: E501
+
+        :return: The tag of this PersonWithImages.  # noqa: E501
+        :rtype: str
+        """
+        return self._tag
+
+    @tag.setter
+    def tag(self, tag):
+        """Sets the tag of this PersonWithImages.
+
+        Session identificator.  # noqa: E501
+
+        :param tag: The tag of this PersonWithImages.  # noqa: E501
+        :type tag: str
+        """
+
+        self._tag = tag
+
+    @property
     def name(self):
         """Gets the name of this PersonWithImages.  # noqa: E501
 
         Person name.  # noqa: E501
 
         :return: The name of this PersonWithImages.  # noqa: E501
         :rtype: str
@@ -141,32 +174,55 @@
         :param metadata: The metadata of this PersonWithImages.  # noqa: E501
         :type metadata: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
 
         self._metadata = metadata
 
     @property
+    def groups(self):
+        """Gets the groups of this PersonWithImages.  # noqa: E501
+
+        List of groups this person belongs to.  # noqa: E501
+
+        :return: The groups of this PersonWithImages.  # noqa: E501
+        :rtype: [str]
+        """
+        return self._groups
+
+    @groups.setter
+    def groups(self, groups):
+        """Sets the groups of this PersonWithImages.
+
+        List of groups this person belongs to.  # noqa: E501
+
+        :param groups: The groups of this PersonWithImages.  # noqa: E501
+        :type groups: [str]
+        """
+
+        self._groups = groups
+
+    @property
     def id(self):
         """Gets the id of this PersonWithImages.  # noqa: E501
 
-        Person ID.  # noqa: E501
+        Person ID. The list of persons is sorted by decreasing ID value.  # noqa: E501
 
         :return: The id of this PersonWithImages.  # noqa: E501
-        :rtype: int
+        :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this PersonWithImages.
 
-        Person ID.  # noqa: E501
+        Person ID. The list of persons is sorted by decreasing ID value.  # noqa: E501
 
         :param id: The id of this PersonWithImages.  # noqa: E501
-        :type id: int
+        :type id: str
         """
 
         self._id = id
 
     @property
     def created_at(self):
         """Gets the created_at of this PersonWithImages.  # noqa: E501
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_with_images_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/person_with_images_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/persons_page.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/persons_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -37,15 +37,15 @@
         'page': 'int',
         'total_pages': 'int',
     }
 
     attribute_map = {
         'items': 'items',
         'page': 'page',
-        'total_pages': 'total_pages',
+        'total_pages': 'totalPages',
     }
 
     def __init__(self, items=None, page=None, total_pages=None, local_vars_configuration=None):  # noqa: E501
         """PersonsPage - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/persons_page_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/persons_page_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/process_param.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/process_param.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_config.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/quality_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,15 +29,15 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'FaceQualityConfigName',
+        'name': 'FaceAttribute',
         'range': '[float]',
     }
 
     attribute_map = {
         'name': 'name',
         'range': 'range',
     }
@@ -59,25 +59,25 @@
 
     @property
     def name(self):
         """Gets the name of this QualityConfig.  # noqa: E501
 
 
         :return: The name of this QualityConfig.  # noqa: E501
-        :rtype: FaceQualityConfigName
+        :rtype: FaceAttribute
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this QualityConfig.
 
 
         :param name: The name of this QualityConfig.  # noqa: E501
-        :type name: FaceQualityConfigName
+        :type name: FaceAttribute
         """
 
         self._name = name
 
     @property
     def range(self):
         """Gets the range of this QualityConfig.  # noqa: E501
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_config_list.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/quality_config_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_detail.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/quality_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_details_groups.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/quality_details_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -30,15 +30,15 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'group_id': 'FaceImageQualityGroups',
-        'name': 'FaceQualityConfigName',
+        'name': 'FaceImageQualityGroups',
         'total_count': 'int',
         'compliant_count': 'int',
     }
 
     attribute_map = {
         'group_id': 'groupId',
         'name': 'name',
@@ -90,25 +90,25 @@
 
     @property
     def name(self):
         """Gets the name of this QualityDetailsGroups.  # noqa: E501
 
 
         :return: The name of this QualityDetailsGroups.  # noqa: E501
-        :rtype: FaceQualityConfigName
+        :rtype: FaceImageQualityGroups
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this QualityDetailsGroups.
 
 
         :param name: The name of this QualityDetailsGroups.  # noqa: E501
-        :type name: FaceQualityConfigName
+        :type name: FaceImageQualityGroups
         """
 
         self._name = name
 
     @property
     def total_count(self):
         """Gets the total_count of this QualityDetailsGroups.  # noqa: E501
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_request.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/quality_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/recognize_image.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/recognize_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -42,17 +42,17 @@
         'metadata': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
         'similarity': 'float',
         'distance': 'float',
     }
 
     attribute_map = {
         'id': 'id',
-        'content_type': 'content_type',
-        'created_at': 'created_at',
-        'updated_at': 'updated_at',
+        'content_type': 'contentType',
+        'created_at': 'createdAt',
+        'updated_at': 'updatedAt',
         'path': 'path',
         'url': 'url',
         'metadata': 'metadata',
         'similarity': 'similarity',
         'distance': 'distance',
     }
 
@@ -92,141 +92,141 @@
         if distance is not None:
             self.distance = distance
 
     @property
     def id(self):
         """Gets the id of this RecognizeImage.  # noqa: E501
 
-        Response image ID.  # noqa: E501
+        Response image ID. The list is sorted by decreasing ID value.  # noqa: E501
 
         :return: The id of this RecognizeImage.  # noqa: E501
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this RecognizeImage.
 
-        Response image ID.  # noqa: E501
+        Response image ID. The list is sorted by decreasing ID value.  # noqa: E501
 
         :param id: The id of this RecognizeImage.  # noqa: E501
         :type id: int
         """
 
         self._id = id
 
     @property
     def content_type(self):
         """Gets the content_type of this RecognizeImage.  # noqa: E501
 
-        The original media type of the returned image.  # noqa: E501
+        Original media type of the returned image.  # noqa: E501
 
         :return: The content_type of this RecognizeImage.  # noqa: E501
         :rtype: str
         """
         return self._content_type
 
     @content_type.setter
     def content_type(self, content_type):
         """Sets the content_type of this RecognizeImage.
 
-        The original media type of the returned image.  # noqa: E501
+        Original media type of the returned image.  # noqa: E501
 
         :param content_type: The content_type of this RecognizeImage.  # noqa: E501
         :type content_type: str
         """
 
         self._content_type = content_type
 
     @property
     def created_at(self):
         """Gets the created_at of this RecognizeImage.  # noqa: E501
 
-        The returned image creation date.  # noqa: E501
+        Returned image creation date.  # noqa: E501
 
         :return: The created_at of this RecognizeImage.  # noqa: E501
         :rtype: str
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
         """Sets the created_at of this RecognizeImage.
 
-        The returned image creation date.  # noqa: E501
+        Returned image creation date.  # noqa: E501
 
         :param created_at: The created_at of this RecognizeImage.  # noqa: E501
         :type created_at: str
         """
 
         self._created_at = created_at
 
     @property
     def updated_at(self):
         """Gets the updated_at of this RecognizeImage.  # noqa: E501
 
-        The returned image update date.  # noqa: E501
+        Returned image update date.  # noqa: E501
 
         :return: The updated_at of this RecognizeImage.  # noqa: E501
         :rtype: str
         """
         return self._updated_at
 
     @updated_at.setter
     def updated_at(self, updated_at):
         """Sets the updated_at of this RecognizeImage.
 
-        The returned image update date.  # noqa: E501
+        Returned image update date.  # noqa: E501
 
         :param updated_at: The updated_at of this RecognizeImage.  # noqa: E501
         :type updated_at: str
         """
 
         self._updated_at = updated_at
 
     @property
     def path(self):
         """Gets the path of this RecognizeImage.  # noqa: E501
 
-        The returned image S3 path.  # noqa: E501
+        Returned image S3 path.  # noqa: E501
 
         :return: The path of this RecognizeImage.  # noqa: E501
         :rtype: str
         """
         return self._path
 
     @path.setter
     def path(self, path):
         """Sets the path of this RecognizeImage.
 
-        The returned image S3 path.  # noqa: E501
+        Returned image S3 path.  # noqa: E501
 
         :param path: The path of this RecognizeImage.  # noqa: E501
         :type path: str
         """
 
         self._path = path
 
     @property
     def url(self):
         """Gets the url of this RecognizeImage.  # noqa: E501
 
-        The returned image URL.  # noqa: E501
+        Returned image URL.  # noqa: E501
 
         :return: The url of this RecognizeImage.  # noqa: E501
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
         """Sets the url of this RecognizeImage.
 
-        The returned image URL.  # noqa: E501
+        Returned image URL.  # noqa: E501
 
         :param url: The url of this RecognizeImage.  # noqa: E501
         :type url: str
         """
 
         self._url = url
 
@@ -253,49 +253,49 @@
 
         self._metadata = metadata
 
     @property
     def similarity(self):
         """Gets the similarity of this RecognizeImage.  # noqa: E501
 
-        The similarity score.  # noqa: E501
+        Similarity score.  # noqa: E501
 
         :return: The similarity of this RecognizeImage.  # noqa: E501
         :rtype: float
         """
         return self._similarity
 
     @similarity.setter
     def similarity(self, similarity):
         """Sets the similarity of this RecognizeImage.
 
-        The similarity score.  # noqa: E501
+        Similarity score.  # noqa: E501
 
         :param similarity: The similarity of this RecognizeImage.  # noqa: E501
         :type similarity: float
         """
 
         self._similarity = similarity
 
     @property
     def distance(self):
         """Gets the distance of this RecognizeImage.  # noqa: E501
 
-        The similarity distance score: the lower the distance, the higher the face's similarity.  # noqa: E501
+        Similarity distance score: the lower the distance, the higher the face's similarity.  # noqa: E501
 
         :return: The distance of this RecognizeImage.  # noqa: E501
         :rtype: float
         """
         return self._distance
 
     @distance.setter
     def distance(self, distance):
         """Sets the distance of this RecognizeImage.
 
-        The similarity distance score: the lower the distance, the higher the face's similarity.  # noqa: E501
+        Similarity distance score: the lower the distance, the higher the face's similarity.  # noqa: E501
 
         :param distance: The distance of this RecognizeImage.  # noqa: E501
         :type distance: float
         """
 
         self._distance = distance
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/recognize_image_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/recognize_image_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -57,49 +57,49 @@
         if distance is not None:
             self.distance = distance
 
     @property
     def similarity(self):
         """Gets the similarity of this RecognizeImageAllOf.  # noqa: E501
 
-        The similarity score.  # noqa: E501
+        Similarity score.  # noqa: E501
 
         :return: The similarity of this RecognizeImageAllOf.  # noqa: E501
         :rtype: float
         """
         return self._similarity
 
     @similarity.setter
     def similarity(self, similarity):
         """Sets the similarity of this RecognizeImageAllOf.
 
-        The similarity score.  # noqa: E501
+        Similarity score.  # noqa: E501
 
         :param similarity: The similarity of this RecognizeImageAllOf.  # noqa: E501
         :type similarity: float
         """
 
         self._similarity = similarity
 
     @property
     def distance(self):
         """Gets the distance of this RecognizeImageAllOf.  # noqa: E501
 
-        The similarity distance score: the lower the distance, the higher the face's similarity.  # noqa: E501
+        Similarity distance score: the lower the distance, the higher the face's similarity.  # noqa: E501
 
         :return: The distance of this RecognizeImageAllOf.  # noqa: E501
         :rtype: float
         """
         return self._distance
 
     @distance.setter
     def distance(self, distance):
         """Sets the distance of this RecognizeImageAllOf.
 
-        The similarity distance score: the lower the distance, the higher the face's similarity.  # noqa: E501
+        Similarity distance score: the lower the distance, the higher the face's similarity.  # noqa: E501
 
         :param distance: The distance of this RecognizeImageAllOf.  # noqa: E501
         :type distance: float
         """
 
         self._distance = distance
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/rgb.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/transaction_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 4.1.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class RGB(object):
+class TransactionConfig(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,15 +35,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """RGB - a model defined in OpenAPI"""  # noqa: E501
+        """TransactionConfig - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -75,18 +75,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RGB):
+        if not isinstance(other, TransactionConfig):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RGB):
+        if not isinstance(other, TransactionConfig):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_parameters.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/resize_options.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,139 +1,139 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class SearchParameters(object):
+class ResizeOptions(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'limit': 'int',
-        'threshold': 'float',
-        'group_ids': '[int]',
+        'width': 'int',
+        'height': 'int',
+        'quality': 'int',
     }
 
     attribute_map = {
-        'limit': 'limit',
-        'threshold': 'threshold',
-        'group_ids': 'group_ids',
+        'width': 'width',
+        'height': 'height',
+        'quality': 'quality',
     }
 
-    def __init__(self, limit=100, threshold=None, group_ids=None, local_vars_configuration=None):  # noqa: E501
-        """SearchParameters - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, width=None, height=None, quality=100, local_vars_configuration=None):  # noqa: E501
+        """ResizeOptions - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._limit = None
-        self._threshold = None
-        self._group_ids = None
+        self._width = None
+        self._height = None
+        self._quality = None
         self.discriminator = None
 
-        if limit is not None:
-            self.limit = limit
-        if threshold is not None:
-            self.threshold = threshold
-        if group_ids is not None:
-            self.group_ids = group_ids
+        if width is not None:
+            self.width = width
+        if height is not None:
+            self.height = height
+        if quality is not None:
+            self.quality = quality
 
     @property
-    def limit(self):
-        """Gets the limit of this SearchParameters.  # noqa: E501
+    def width(self):
+        """Gets the width of this ResizeOptions.  # noqa: E501
 
-        The number of returned Persons limit.  # noqa: E501
+        Resized image width, px.  # noqa: E501
 
-        :return: The limit of this SearchParameters.  # noqa: E501
+        :return: The width of this ResizeOptions.  # noqa: E501
         :rtype: int
         """
-        return self._limit
+        return self._width
 
-    @limit.setter
-    def limit(self, limit):
-        """Sets the limit of this SearchParameters.
+    @width.setter
+    def width(self, width):
+        """Sets the width of this ResizeOptions.
 
-        The number of returned Persons limit.  # noqa: E501
+        Resized image width, px.  # noqa: E501
 
-        :param limit: The limit of this SearchParameters.  # noqa: E501
-        :type limit: int
+        :param width: The width of this ResizeOptions.  # noqa: E501
+        :type width: int
         """
 
-        self._limit = limit
+        self._width = width
 
     @property
-    def threshold(self):
-        """Gets the threshold of this SearchParameters.  # noqa: E501
+    def height(self):
+        """Gets the height of this ResizeOptions.  # noqa: E501
 
-        The similarity distance threshold, should be between 0.0 and 2.0, where 0.0 is for returning results for only the most similar persons and 2.0 is for all the persons, even the dissimilar ones. If not set, the default 1.0 value is used.  # noqa: E501
+        Resized image height, px.  # noqa: E501
 
-        :return: The threshold of this SearchParameters.  # noqa: E501
-        :rtype: float
+        :return: The height of this ResizeOptions.  # noqa: E501
+        :rtype: int
         """
-        return self._threshold
+        return self._height
 
-    @threshold.setter
-    def threshold(self, threshold):
-        """Sets the threshold of this SearchParameters.
+    @height.setter
+    def height(self, height):
+        """Sets the height of this ResizeOptions.
 
-        The similarity distance threshold, should be between 0.0 and 2.0, where 0.0 is for returning results for only the most similar persons and 2.0 is for all the persons, even the dissimilar ones. If not set, the default 1.0 value is used.  # noqa: E501
+        Resized image height, px.  # noqa: E501
 
-        :param threshold: The threshold of this SearchParameters.  # noqa: E501
-        :type threshold: float
+        :param height: The height of this ResizeOptions.  # noqa: E501
+        :type height: int
         """
 
-        self._threshold = threshold
+        self._height = height
 
     @property
-    def group_ids(self):
-        """Gets the group_ids of this SearchParameters.  # noqa: E501
+    def quality(self):
+        """Gets the quality of this ResizeOptions.  # noqa: E501
 
-        The IDs of the groups in which the search is performed.  # noqa: E501
+        Resized image quality, percent.  # noqa: E501
 
-        :return: The group_ids of this SearchParameters.  # noqa: E501
-        :rtype: [int]
+        :return: The quality of this ResizeOptions.  # noqa: E501
+        :rtype: int
         """
-        return self._group_ids
+        return self._quality
 
-    @group_ids.setter
-    def group_ids(self, group_ids):
-        """Sets the group_ids of this SearchParameters.
+    @quality.setter
+    def quality(self, quality):
+        """Sets the quality of this ResizeOptions.
 
-        The IDs of the groups in which the search is performed.  # noqa: E501
+        Resized image quality, percent.  # noqa: E501
 
-        :param group_ids: The group_ids of this SearchParameters.  # noqa: E501
-        :type group_ids: [int]
+        :param quality: The quality of this ResizeOptions.  # noqa: E501
+        :type quality: int
         """
 
-        self._group_ids = group_ids
+        self._quality = quality
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -161,18 +161,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SearchParameters):
+        if not isinstance(other, ResizeOptions):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SearchParameters):
+        if not isinstance(other, ResizeOptions):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_person.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_person.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,59 +29,97 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'tag': 'str',
         'name': 'str',
         'metadata': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
-        'id': 'int',
+        'groups': '[str]',
+        'id': 'str',
         'created_at': 'str',
         'updated_at': 'str',
+        'detection': 'SearchDetection',
         'images': '[RecognizeImage]',
     }
 
     attribute_map = {
+        'tag': 'tag',
         'name': 'name',
         'metadata': 'metadata',
+        'groups': 'groups',
         'id': 'id',
-        'created_at': 'created_at',
-        'updated_at': 'updated_at',
+        'created_at': 'createdAt',
+        'updated_at': 'updatedAt',
+        'detection': 'detection',
         'images': 'images',
     }
 
-    def __init__(self, name=None, metadata=None, id=None, created_at=None, updated_at=None, images=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, tag=None, name=None, metadata=None, groups=None, id=None, created_at=None, updated_at=None, detection=None, images=None, local_vars_configuration=None):  # noqa: E501
         """SearchPerson - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._tag = None
         self._name = None
         self._metadata = None
+        self._groups = None
         self._id = None
         self._created_at = None
         self._updated_at = None
+        self._detection = None
         self._images = None
         self.discriminator = None
 
+        if tag is not None:
+            self.tag = tag
         if name is not None:
             self.name = name
         if metadata is not None:
             self.metadata = metadata
+        if groups is not None:
+            self.groups = groups
         if id is not None:
             self.id = id
         if created_at is not None:
             self.created_at = created_at
         if updated_at is not None:
             self.updated_at = updated_at
+        if detection is not None:
+            self.detection = detection
         if images is not None:
             self.images = images
 
     @property
+    def tag(self):
+        """Gets the tag of this SearchPerson.  # noqa: E501
+
+        Session identificator.  # noqa: E501
+
+        :return: The tag of this SearchPerson.  # noqa: E501
+        :rtype: str
+        """
+        return self._tag
+
+    @tag.setter
+    def tag(self, tag):
+        """Sets the tag of this SearchPerson.
+
+        Session identificator.  # noqa: E501
+
+        :param tag: The tag of this SearchPerson.  # noqa: E501
+        :type tag: str
+        """
+
+        self._tag = tag
+
+    @property
     def name(self):
         """Gets the name of this SearchPerson.  # noqa: E501
 
         Person name.  # noqa: E501
 
         :return: The name of this SearchPerson.  # noqa: E501
         :rtype: str
@@ -120,32 +158,55 @@
         :param metadata: The metadata of this SearchPerson.  # noqa: E501
         :type metadata: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
 
         self._metadata = metadata
 
     @property
+    def groups(self):
+        """Gets the groups of this SearchPerson.  # noqa: E501
+
+        List of groups this person belongs to.  # noqa: E501
+
+        :return: The groups of this SearchPerson.  # noqa: E501
+        :rtype: [str]
+        """
+        return self._groups
+
+    @groups.setter
+    def groups(self, groups):
+        """Sets the groups of this SearchPerson.
+
+        List of groups this person belongs to.  # noqa: E501
+
+        :param groups: The groups of this SearchPerson.  # noqa: E501
+        :type groups: [str]
+        """
+
+        self._groups = groups
+
+    @property
     def id(self):
         """Gets the id of this SearchPerson.  # noqa: E501
 
-        Person ID.  # noqa: E501
+        Person ID. The list of persons is sorted by decreasing ID value.  # noqa: E501
 
         :return: The id of this SearchPerson.  # noqa: E501
-        :rtype: int
+        :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this SearchPerson.
 
-        Person ID.  # noqa: E501
+        Person ID. The list of persons is sorted by decreasing ID value.  # noqa: E501
 
         :param id: The id of this SearchPerson.  # noqa: E501
-        :type id: int
+        :type id: str
         """
 
         self._id = id
 
     @property
     def created_at(self):
         """Gets the created_at of this SearchPerson.  # noqa: E501
@@ -189,27 +250,50 @@
         :param updated_at: The updated_at of this SearchPerson.  # noqa: E501
         :type updated_at: str
         """
 
         self._updated_at = updated_at
 
     @property
+    def detection(self):
+        """Gets the detection of this SearchPerson.  # noqa: E501
+
+
+        :return: The detection of this SearchPerson.  # noqa: E501
+        :rtype: SearchDetection
+        """
+        return self._detection
+
+    @detection.setter
+    def detection(self, detection):
+        """Sets the detection of this SearchPerson.
+
+
+        :param detection: The detection of this SearchPerson.  # noqa: E501
+        :type detection: SearchDetection
+        """
+
+        self._detection = detection
+
+    @property
     def images(self):
         """Gets the images of this SearchPerson.  # noqa: E501
 
+        Array of Person images.  # noqa: E501
 
         :return: The images of this SearchPerson.  # noqa: E501
         :rtype: [RecognizeImage]
         """
         return self._images
 
     @images.setter
     def images(self, images):
         """Sets the images of this SearchPerson.
 
+        Array of Person images.  # noqa: E501
 
         :param images: The images of this SearchPerson.  # noqa: E501
         :type images: [RecognizeImage]
         """
 
         self._images = images
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_person_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/face_attribute.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,95 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class SearchPersonAllOf(object):
+class FaceAttribute(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+    ""
+    AGE = "Age"
+
+    ""
+    EMOTION = "Emotion"
+
+    ""
+    EYE_LEFT = "EyeLeft"
+
+    ""
+    EYE_RIGHT = "EyeRight"
+
+    ""
+    SMILE = "Smile"
+
+    ""
+    GLASSES = "Glasses"
+
+    ""
+    HEAD_COVERING = "HeadCovering"
+
+    ""
+    FOREHEAD_COVERING = "ForeheadCovering"
+
+    ""
+    MOUTH = "Mouth"
+
+    ""
+    MEDICAL_MASK = "MedicalMask"
+
+    ""
+    OCCLUSION = "Occlusion"
+
+    ""
+    STRONG_MAKEUP = "StrongMakeup"
+
+    ""
+    HEADPHONES = "Headphones"
+
+    allowable_values = [AGE, EMOTION, EYE_LEFT, EYE_RIGHT, SMILE, GLASSES, HEAD_COVERING, FOREHEAD_COVERING, MOUTH, MEDICAL_MASK, OCCLUSION, STRONG_MAKEUP, HEADPHONES]  # noqa: E501
+
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'images': '[RecognizeImage]',
     }
 
     attribute_map = {
-        'images': 'images',
     }
 
-    def __init__(self, images=None, local_vars_configuration=None):  # noqa: E501
-        """SearchPersonAllOf - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, local_vars_configuration=None):  # noqa: E501
+        """FaceAttribute - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
-
-        self._images = None
         self.discriminator = None
 
-        if images is not None:
-            self.images = images
-
-    @property
-    def images(self):
-        """Gets the images of this SearchPersonAllOf.  # noqa: E501
-
-
-        :return: The images of this SearchPersonAllOf.  # noqa: E501
-        :rtype: [RecognizeImage]
-        """
-        return self._images
-
-    @images.setter
-    def images(self, images):
-        """Sets the images of this SearchPersonAllOf.
-
-
-        :param images: The images of this SearchPersonAllOf.  # noqa: E501
-        :type images: [RecognizeImage]
-        """
-
-        self._images = images
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -103,18 +116,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SearchPersonAllOf):
+        if not isinstance(other, FaceAttribute):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SearchPersonAllOf):
+        if not isinstance(other, FaceAttribute):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_request.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,118 +29,136 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'limit': 'int',
-        'threshold': 'float',
+        'create_person': 'SearchParametersCreatePerson',
         'group_ids': '[int]',
+        'tag': 'str',
         'image': 'ImageFieldsImage',
+        'output_image_params': 'OutputImageParams',
+        'detect_all': 'bool',
+        'threshold': 'float',
+        'limit': 'int',
     }
 
     attribute_map = {
-        'limit': 'limit',
-        'threshold': 'threshold',
-        'group_ids': 'group_ids',
+        'create_person': 'createPerson',
+        'group_ids': 'groupIds',
+        'tag': 'tag',
         'image': 'image',
+        'output_image_params': 'outputImageParams',
+        'detect_all': 'detectAll',
+        'threshold': 'threshold',
+        'limit': 'limit',
     }
 
-    def __init__(self, limit=100, threshold=None, group_ids=None, image=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, create_person=None, group_ids=None, tag=None, image=None, output_image_params=None, detect_all=False, threshold=None, limit=None, local_vars_configuration=None):  # noqa: E501
         """SearchRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._limit = None
-        self._threshold = None
+        self._create_person = None
         self._group_ids = None
+        self._tag = None
         self._image = None
+        self._output_image_params = None
+        self._detect_all = None
+        self._threshold = None
+        self._limit = None
         self.discriminator = None
 
-        if limit is not None:
-            self.limit = limit
-        if threshold is not None:
-            self.threshold = threshold
+        if create_person is not None:
+            self.create_person = create_person
         if group_ids is not None:
             self.group_ids = group_ids
+        if tag is not None:
+            self.tag = tag
         if image is not None:
             self.image = image
+        if output_image_params is not None:
+            self.output_image_params = output_image_params
+        if detect_all is not None:
+            self.detect_all = detect_all
+        if threshold is not None:
+            self.threshold = threshold
+        if limit is not None:
+            self.limit = limit
 
     @property
-    def limit(self):
-        """Gets the limit of this SearchRequest.  # noqa: E501
-
-        The number of returned Persons limit.  # noqa: E501
-
-        :return: The limit of this SearchRequest.  # noqa: E501
-        :rtype: int
-        """
-        return self._limit
-
-    @limit.setter
-    def limit(self, limit):
-        """Sets the limit of this SearchRequest.
-
-        The number of returned Persons limit.  # noqa: E501
-
-        :param limit: The limit of this SearchRequest.  # noqa: E501
-        :type limit: int
-        """
-
-        self._limit = limit
-
-    @property
-    def threshold(self):
-        """Gets the threshold of this SearchRequest.  # noqa: E501
+    def create_person(self):
+        """Gets the create_person of this SearchRequest.  # noqa: E501
 
-        The similarity distance threshold, should be between 0.0 and 2.0, where 0.0 is for returning results for only the most similar persons and 2.0 is for all the persons, even the dissimilar ones. If not set, the default 1.0 value is used.  # noqa: E501
 
-        :return: The threshold of this SearchRequest.  # noqa: E501
-        :rtype: float
+        :return: The create_person of this SearchRequest.  # noqa: E501
+        :rtype: SearchParametersCreatePerson
         """
-        return self._threshold
+        return self._create_person
 
-    @threshold.setter
-    def threshold(self, threshold):
-        """Sets the threshold of this SearchRequest.
+    @create_person.setter
+    def create_person(self, create_person):
+        """Sets the create_person of this SearchRequest.
 
-        The similarity distance threshold, should be between 0.0 and 2.0, where 0.0 is for returning results for only the most similar persons and 2.0 is for all the persons, even the dissimilar ones. If not set, the default 1.0 value is used.  # noqa: E501
 
-        :param threshold: The threshold of this SearchRequest.  # noqa: E501
-        :type threshold: float
+        :param create_person: The create_person of this SearchRequest.  # noqa: E501
+        :type create_person: SearchParametersCreatePerson
         """
 
-        self._threshold = threshold
+        self._create_person = create_person
 
     @property
     def group_ids(self):
         """Gets the group_ids of this SearchRequest.  # noqa: E501
 
-        The IDs of the groups in which the search is performed.  # noqa: E501
+        IDs of the groups in which the search is performed.  # noqa: E501
 
         :return: The group_ids of this SearchRequest.  # noqa: E501
         :rtype: [int]
         """
         return self._group_ids
 
     @group_ids.setter
     def group_ids(self, group_ids):
         """Sets the group_ids of this SearchRequest.
 
-        The IDs of the groups in which the search is performed.  # noqa: E501
+        IDs of the groups in which the search is performed.  # noqa: E501
 
         :param group_ids: The group_ids of this SearchRequest.  # noqa: E501
         :type group_ids: [int]
         """
 
         self._group_ids = group_ids
 
     @property
+    def tag(self):
+        """Gets the tag of this SearchRequest.  # noqa: E501
+
+        Session identificator.  # noqa: E501
+
+        :return: The tag of this SearchRequest.  # noqa: E501
+        :rtype: str
+        """
+        return self._tag
+
+    @tag.setter
+    def tag(self, tag):
+        """Sets the tag of this SearchRequest.
+
+        Session identificator.  # noqa: E501
+
+        :param tag: The tag of this SearchRequest.  # noqa: E501
+        :type tag: str
+        """
+
+        self._tag = tag
+
+    @property
     def image(self):
         """Gets the image of this SearchRequest.  # noqa: E501
 
 
         :return: The image of this SearchRequest.  # noqa: E501
         :rtype: ImageFieldsImage
         """
@@ -153,14 +171,104 @@
 
         :param image: The image of this SearchRequest.  # noqa: E501
         :type image: ImageFieldsImage
         """
 
         self._image = image
 
+    @property
+    def output_image_params(self):
+        """Gets the output_image_params of this SearchRequest.  # noqa: E501
+
+
+        :return: The output_image_params of this SearchRequest.  # noqa: E501
+        :rtype: OutputImageParams
+        """
+        return self._output_image_params
+
+    @output_image_params.setter
+    def output_image_params(self, output_image_params):
+        """Sets the output_image_params of this SearchRequest.
+
+
+        :param output_image_params: The output_image_params of this SearchRequest.  # noqa: E501
+        :type output_image_params: OutputImageParams
+        """
+
+        self._output_image_params = output_image_params
+
+    @property
+    def detect_all(self):
+        """Gets the detect_all of this SearchRequest.  # noqa: E501
+
+        Whether to detect all faces in the image. If set to false, only the most central face is detected.  # noqa: E501
+
+        :return: The detect_all of this SearchRequest.  # noqa: E501
+        :rtype: bool
+        """
+        return self._detect_all
+
+    @detect_all.setter
+    def detect_all(self, detect_all):
+        """Sets the detect_all of this SearchRequest.
+
+        Whether to detect all faces in the image. If set to false, only the most central face is detected.  # noqa: E501
+
+        :param detect_all: The detect_all of this SearchRequest.  # noqa: E501
+        :type detect_all: bool
+        """
+
+        self._detect_all = detect_all
+
+    @property
+    def threshold(self):
+        """Gets the threshold of this SearchRequest.  # noqa: E501
+
+        The similarity threshold.  # noqa: E501
+
+        :return: The threshold of this SearchRequest.  # noqa: E501
+        :rtype: float
+        """
+        return self._threshold
+
+    @threshold.setter
+    def threshold(self, threshold):
+        """Sets the threshold of this SearchRequest.
+
+        The similarity threshold.  # noqa: E501
+
+        :param threshold: The threshold of this SearchRequest.  # noqa: E501
+        :type threshold: float
+        """
+
+        self._threshold = threshold
+
+    @property
+    def limit(self):
+        """Gets the limit of this SearchRequest.  # noqa: E501
+
+        The maximum number of results to be returned.  # noqa: E501
+
+        :return: The limit of this SearchRequest.  # noqa: E501
+        :rtype: int
+        """
+        return self._limit
+
+    @limit.setter
+    def limit(self, limit):
+        """Sets the limit of this SearchRequest.
+
+        The maximum number of results to be returned.  # noqa: E501
+
+        :param limit: The limit of this SearchRequest.  # noqa: E501
+        :type limit: int
+        """
+
+        self._limit = limit
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_result.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -57,47 +57,49 @@
         if persons is not None:
             self.persons = persons
 
     @property
     def code(self):
         """Gets the code of this SearchResult.  # noqa: E501
 
-        The search result code.  # noqa: E501
+        Search result code.  # noqa: E501
 
         :return: The code of this SearchResult.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this SearchResult.
 
-        The search result code.  # noqa: E501
+        Search result code.  # noqa: E501
 
         :param code: The code of this SearchResult.  # noqa: E501
         :type code: int
         """
 
         self._code = code
 
     @property
     def persons(self):
         """Gets the persons of this SearchResult.  # noqa: E501
 
+        Person data.  # noqa: E501
 
         :return: The persons of this SearchResult.  # noqa: E501
         :rtype: [SearchPerson]
         """
         return self._persons
 
     @persons.setter
     def persons(self, persons):
         """Sets the persons of this SearchResult.
 
+        Person data.  # noqa: E501
 
         :param persons: The persons of this SearchResult.  # noqa: E501
         :type persons: [SearchPerson]
         """
 
         self._persons = persons
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_result_all_of.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/search_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/transaction_info.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/transaction_info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -31,77 +31,87 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'code': 'int',
         'status': 'int',
-        'session_id': 'int',
+        'tag': 'str',
         'transaction_id': 'str',
         'video': 'str',
+        'images': '[str]',
+        'estimated_age': 'int',
         'portrait': 'str',
         'metadata': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
     }
 
     attribute_map = {
         'code': 'code',
         'status': 'status',
-        'session_id': 'sessionId',
+        'tag': 'tag',
         'transaction_id': 'transactionId',
         'video': 'video',
+        'images': 'images',
+        'estimated_age': 'estimatedAge',
         'portrait': 'portrait',
         'metadata': 'metadata',
     }
 
-    def __init__(self, code=None, status=None, session_id=None, transaction_id=None, video=None, portrait=None, metadata=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, code=None, status=None, tag=None, transaction_id=None, video=None, images=None, estimated_age=None, portrait=None, metadata=None, local_vars_configuration=None):  # noqa: E501
         """TransactionInfo - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._code = None
         self._status = None
-        self._session_id = None
+        self._tag = None
         self._transaction_id = None
         self._video = None
+        self._images = None
+        self._estimated_age = None
         self._portrait = None
         self._metadata = None
         self.discriminator = None
 
         if code is not None:
             self.code = code
         if status is not None:
             self.status = status
-        if session_id is not None:
-            self.session_id = session_id
+        if tag is not None:
+            self.tag = tag
         if transaction_id is not None:
             self.transaction_id = transaction_id
         if video is not None:
             self.video = video
+        if images is not None:
+            self.images = images
+        if estimated_age is not None:
+            self.estimated_age = estimated_age
         if portrait is not None:
             self.portrait = portrait
         if metadata is not None:
             self.metadata = metadata
 
     @property
     def code(self):
         """Gets the code of this TransactionInfo.  # noqa: E501
 
-        The result code, one of the FaceSDKResultCode enum values. See the enum: https://docs.regulaforensics.com/develop/face-sdk/web-service/development/enums/face-sdk-result-code/  # noqa: E501
+        Result code, one of the FaceSDKResultCode enum values. See the enum: https://docs.regulaforensics.com/develop/face-sdk/web-service/development/enums/face-sdk-result-code/  # noqa: E501
 
         :return: The code of this TransactionInfo.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this TransactionInfo.
 
-        The result code, one of the FaceSDKResultCode enum values. See the enum: https://docs.regulaforensics.com/develop/face-sdk/web-service/development/enums/face-sdk-result-code/  # noqa: E501
+        Result code, one of the FaceSDKResultCode enum values. See the enum: https://docs.regulaforensics.com/develop/face-sdk/web-service/development/enums/face-sdk-result-code/  # noqa: E501
 
         :param code: The code of this TransactionInfo.  # noqa: E501
         :type code: int
         """
 
         self._code = code
 
@@ -125,35 +135,35 @@
         :param status: The status of this TransactionInfo.  # noqa: E501
         :type status: int
         """
 
         self._status = status
 
     @property
-    def session_id(self):
-        """Gets the session_id of this TransactionInfo.  # noqa: E501
+    def tag(self):
+        """Gets the tag of this TransactionInfo.  # noqa: E501
 
-        Session ID, one session may include many transactions.  # noqa: E501
+        Session identificator.  # noqa: E501
 
-        :return: The session_id of this TransactionInfo.  # noqa: E501
-        :rtype: int
+        :return: The tag of this TransactionInfo.  # noqa: E501
+        :rtype: str
         """
-        return self._session_id
+        return self._tag
 
-    @session_id.setter
-    def session_id(self, session_id):
-        """Sets the session_id of this TransactionInfo.
+    @tag.setter
+    def tag(self, tag):
+        """Sets the tag of this TransactionInfo.
 
-        Session ID, one session may include many transactions.  # noqa: E501
+        Session identificator.  # noqa: E501
 
-        :param session_id: The session_id of this TransactionInfo.  # noqa: E501
-        :type session_id: int
+        :param tag: The tag of this TransactionInfo.  # noqa: E501
+        :type tag: str
         """
 
-        self._session_id = session_id
+        self._tag = tag
 
     @property
     def transaction_id(self):
         """Gets the transaction_id of this TransactionInfo.  # noqa: E501
 
         Transaction ID, there can be several transactions within one session.  # noqa: E501
 
@@ -194,29 +204,75 @@
         :param video: The video of this TransactionInfo.  # noqa: E501
         :type video: str
         """
 
         self._video = video
 
     @property
+    def images(self):
+        """Gets the images of this TransactionInfo.  # noqa: E501
+
+        List of base64 images  # noqa: E501
+
+        :return: The images of this TransactionInfo.  # noqa: E501
+        :rtype: [str]
+        """
+        return self._images
+
+    @images.setter
+    def images(self, images):
+        """Sets the images of this TransactionInfo.
+
+        List of base64 images  # noqa: E501
+
+        :param images: The images of this TransactionInfo.  # noqa: E501
+        :type images: [str]
+        """
+
+        self._images = images
+
+    @property
+    def estimated_age(self):
+        """Gets the estimated_age of this TransactionInfo.  # noqa: E501
+
+        Approximate age with an accuracy of +/-3 years.  # noqa: E501
+
+        :return: The estimated_age of this TransactionInfo.  # noqa: E501
+        :rtype: int
+        """
+        return self._estimated_age
+
+    @estimated_age.setter
+    def estimated_age(self, estimated_age):
+        """Sets the estimated_age of this TransactionInfo.
+
+        Approximate age with an accuracy of +/-3 years.  # noqa: E501
+
+        :param estimated_age: The estimated_age of this TransactionInfo.  # noqa: E501
+        :type estimated_age: int
+        """
+
+        self._estimated_age = estimated_age
+
+    @property
     def portrait(self):
         """Gets the portrait of this TransactionInfo.  # noqa: E501
 
-        An S3 link to the portrait.  # noqa: E501
+        S3 link to the portrait.  # noqa: E501
 
         :return: The portrait of this TransactionInfo.  # noqa: E501
         :rtype: str
         """
         return self._portrait
 
     @portrait.setter
     def portrait(self, portrait):
         """Sets the portrait of this TransactionInfo.
 
-        An S3 link to the portrait.  # noqa: E501
+        S3 link to the portrait.  # noqa: E501
 
         :param portrait: The portrait of this TransactionInfo.  # noqa: E501
         :type portrait: str
         """
 
         self._portrait = portrait
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/update_group.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model/update_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,16 +29,16 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'add_items': '[int]',
-        'remove_items': '[int]',
+        'add_items': '[str]',
+        'remove_items': '[str]',
     }
 
     attribute_map = {
         'add_items': 'addItems',
         'remove_items': 'removeItems',
     }
 
@@ -60,49 +60,49 @@
     @property
     def add_items(self):
         """Gets the add_items of this UpdateGroup.  # noqa: E501
 
         Add items.  # noqa: E501
 
         :return: The add_items of this UpdateGroup.  # noqa: E501
-        :rtype: [int]
+        :rtype: [str]
         """
         return self._add_items
 
     @add_items.setter
     def add_items(self, add_items):
         """Sets the add_items of this UpdateGroup.
 
         Add items.  # noqa: E501
 
         :param add_items: The add_items of this UpdateGroup.  # noqa: E501
-        :type add_items: [int]
+        :type add_items: [str]
         """
 
         self._add_items = add_items
 
     @property
     def remove_items(self):
         """Gets the remove_items of this UpdateGroup.  # noqa: E501
 
         Remove items.  # noqa: E501
 
         :return: The remove_items of this UpdateGroup.  # noqa: E501
-        :rtype: [int]
+        :rtype: [str]
         """
         return self._remove_items
 
     @remove_items.setter
     def remove_items(self, remove_items):
         """Sets the remove_items of this UpdateGroup.
 
         Remove items.  # noqa: E501
 
         :param remove_items: The remove_items of this UpdateGroup.  # noqa: E501
-        :type remove_items: [int]
+        :type remove_items: [str]
         """
 
         self._remove_items = remove_items
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model_utils.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/models/__init__.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 # from from regula.facesdk.webclient.gen.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from regula.facesdk.webclient.gen.model.crop import Crop
 from regula.facesdk.webclient.gen.model.detect_request import DetectRequest
+from regula.facesdk.webclient.gen.model.detect_request_attributes import DetectRequestAttributes
 from regula.facesdk.webclient.gen.model.detect_response import DetectResponse
 from regula.facesdk.webclient.gen.model.detect_response_all_of import DetectResponseAllOf
 from regula.facesdk.webclient.gen.model.detect_result import DetectResult
 from regula.facesdk.webclient.gen.model.detection import Detection
 from regula.facesdk.webclient.gen.model.detection_face import DetectionFace
 from regula.facesdk.webclient.gen.model.detection_quality import DetectionQuality
+from regula.facesdk.webclient.gen.model.face_attribute import FaceAttribute
 from regula.facesdk.webclient.gen.model.face_image_quality_align_type import FaceImageQualityAlignType
 from regula.facesdk.webclient.gen.model.face_image_quality_groups import FaceImageQualityGroups
 from regula.facesdk.webclient.gen.model.face_image_quality_status import FaceImageQualityStatus
 from regula.facesdk.webclient.gen.model.face_quality_config_name import FaceQualityConfigName
 from regula.facesdk.webclient.gen.model.face_quality_scenarios import FaceQualityScenarios
 from regula.facesdk.webclient.gen.model.face_rectangular import FaceRectangular
 from regula.facesdk.webclient.gen.model.face_sdk_result import FaceSDKResult
@@ -51,28 +53,33 @@
 from regula.facesdk.webclient.gen.model.match_response import MatchResponse
 from regula.facesdk.webclient.gen.model.match_response_all_of import MatchResponseAllOf
 from regula.facesdk.webclient.gen.model.operation_log import OperationLog
 from regula.facesdk.webclient.gen.model.output_image_params import OutputImageParams
 from regula.facesdk.webclient.gen.model.page import Page
 from regula.facesdk.webclient.gen.model.person import Person
 from regula.facesdk.webclient.gen.model.person_all_of import PersonAllOf
+from regula.facesdk.webclient.gen.model.person_created_response import PersonCreatedResponse
 from regula.facesdk.webclient.gen.model.person_fields import PersonFields
 from regula.facesdk.webclient.gen.model.person_with_images import PersonWithImages
 from regula.facesdk.webclient.gen.model.person_with_images_all_of import PersonWithImagesAllOf
 from regula.facesdk.webclient.gen.model.persons_page import PersonsPage
 from regula.facesdk.webclient.gen.model.persons_page_all_of import PersonsPageAllOf
 from regula.facesdk.webclient.gen.model.process_param import ProcessParam
 from regula.facesdk.webclient.gen.model.quality_config import QualityConfig
 from regula.facesdk.webclient.gen.model.quality_config_list import QualityConfigList
 from regula.facesdk.webclient.gen.model.quality_detail import QualityDetail
 from regula.facesdk.webclient.gen.model.quality_details_groups import QualityDetailsGroups
 from regula.facesdk.webclient.gen.model.quality_request import QualityRequest
 from regula.facesdk.webclient.gen.model.rgb import RGB
 from regula.facesdk.webclient.gen.model.recognize_image import RecognizeImage
 from regula.facesdk.webclient.gen.model.recognize_image_all_of import RecognizeImageAllOf
+from regula.facesdk.webclient.gen.model.resize_options import ResizeOptions
+from regula.facesdk.webclient.gen.model.search_bad_params import SearchBadParams
+from regula.facesdk.webclient.gen.model.search_detection import SearchDetection
 from regula.facesdk.webclient.gen.model.search_parameters import SearchParameters
+from regula.facesdk.webclient.gen.model.search_parameters_create_person import SearchParametersCreatePerson
 from regula.facesdk.webclient.gen.model.search_person import SearchPerson
 from regula.facesdk.webclient.gen.model.search_person_all_of import SearchPersonAllOf
 from regula.facesdk.webclient.gen.model.search_request import SearchRequest
 from regula.facesdk.webclient.gen.model.search_result import SearchResult
 from regula.facesdk.webclient.gen.model.transaction_info import TransactionInfo
 from regula.facesdk.webclient.gen.model.update_group import UpdateGroup
```

### Comparing `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/rest.py` & `regula.facesdk.webclient-5.2.0/regula/facesdk/webclient/gen/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 5.1.0
+    The version of the OpenAPI document: 5.2.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/PKG-INFO` & `regula.facesdk.webclient-5.2.0/regula.facesdk.webclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regula.facesdk.webclient
-Version: 5.1.1
+Version: 5.2.0
 Summary: Regula's FaceSDK web python client
 Home-page: https://mobile.regulaforensics.com
 Author: Regula Forensics, Inc.
 Author-email: support@regulaforensics.com
 Keywords: face recognition,facesdk,regulaforensics,regula
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/SOURCES.txt` & `regula.facesdk.webclient-5.2.0/regula.facesdk.webclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,31 +23,34 @@
 regula/facesdk/webclient/gen/__init__.py
 regula/facesdk/webclient/gen/api_client.py
 regula/facesdk/webclient/gen/configuration.py
 regula/facesdk/webclient/gen/exceptions.py
 regula/facesdk/webclient/gen/model_utils.py
 regula/facesdk/webclient/gen/rest.py
 regula/facesdk/webclient/gen/api/__init__.py
+regula/facesdk/webclient/gen/api/diagnostics_api.py
 regula/facesdk/webclient/gen/api/group_api.py
 regula/facesdk/webclient/gen/api/liveness_2_0_api.py
 regula/facesdk/webclient/gen/api/liveness_api.py
 regula/facesdk/webclient/gen/api/matching_api.py
 regula/facesdk/webclient/gen/api/person_api.py
 regula/facesdk/webclient/gen/api/search_api.py
 regula/facesdk/webclient/gen/apis/__init__.py
 regula/facesdk/webclient/gen/model/__init__.py
 regula/facesdk/webclient/gen/model/crop.py
 regula/facesdk/webclient/gen/model/detect_request.py
+regula/facesdk/webclient/gen/model/detect_request_attributes.py
 regula/facesdk/webclient/gen/model/detect_response.py
 regula/facesdk/webclient/gen/model/detect_response_all_of.py
 regula/facesdk/webclient/gen/model/detect_result.py
 regula/facesdk/webclient/gen/model/detection.py
 regula/facesdk/webclient/gen/model/detection_face.py
 regula/facesdk/webclient/gen/model/detection_quality.py
 regula/facesdk/webclient/gen/model/face_align_type_quality.py
+regula/facesdk/webclient/gen/model/face_attribute.py
 regula/facesdk/webclient/gen/model/face_image_quality_align_type.py
 regula/facesdk/webclient/gen/model/face_image_quality_groups.py
 regula/facesdk/webclient/gen/model/face_image_quality_status.py
 regula/facesdk/webclient/gen/model/face_quality_config_name.py
 regula/facesdk/webclient/gen/model/face_quality_scenarios.py
 regula/facesdk/webclient/gen/model/face_quality_status.py
 regula/facesdk/webclient/gen/model/face_rectangular.py
@@ -80,29 +83,34 @@
 regula/facesdk/webclient/gen/model/match_response.py
 regula/facesdk/webclient/gen/model/match_response_all_of.py
 regula/facesdk/webclient/gen/model/operation_log.py
 regula/facesdk/webclient/gen/model/output_image_params.py
 regula/facesdk/webclient/gen/model/page.py
 regula/facesdk/webclient/gen/model/person.py
 regula/facesdk/webclient/gen/model/person_all_of.py
+regula/facesdk/webclient/gen/model/person_created_response.py
 regula/facesdk/webclient/gen/model/person_fields.py
 regula/facesdk/webclient/gen/model/person_with_images.py
 regula/facesdk/webclient/gen/model/person_with_images_all_of.py
 regula/facesdk/webclient/gen/model/persons_page.py
 regula/facesdk/webclient/gen/model/persons_page_all_of.py
 regula/facesdk/webclient/gen/model/process_param.py
 regula/facesdk/webclient/gen/model/quality_config.py
 regula/facesdk/webclient/gen/model/quality_config_list.py
 regula/facesdk/webclient/gen/model/quality_detail.py
 regula/facesdk/webclient/gen/model/quality_details_groups.py
 regula/facesdk/webclient/gen/model/quality_request.py
 regula/facesdk/webclient/gen/model/recognize_image.py
 regula/facesdk/webclient/gen/model/recognize_image_all_of.py
+regula/facesdk/webclient/gen/model/resize_options.py
 regula/facesdk/webclient/gen/model/rgb.py
+regula/facesdk/webclient/gen/model/search_bad_params.py
+regula/facesdk/webclient/gen/model/search_detection.py
 regula/facesdk/webclient/gen/model/search_parameters.py
+regula/facesdk/webclient/gen/model/search_parameters_create_person.py
 regula/facesdk/webclient/gen/model/search_person.py
 regula/facesdk/webclient/gen/model/search_person_all_of.py
 regula/facesdk/webclient/gen/model/search_request.py
 regula/facesdk/webclient/gen/model/search_request_all_of.py
 regula/facesdk/webclient/gen/model/search_result.py
 regula/facesdk/webclient/gen/model/search_result_all_of.py
 regula/facesdk/webclient/gen/model/transaction_config.py
```

### Comparing `regula.facesdk.webclient-5.1.1/setup.py` & `regula.facesdk.webclient-5.2.0/setup.py`

 * *Files identical despite different names*

