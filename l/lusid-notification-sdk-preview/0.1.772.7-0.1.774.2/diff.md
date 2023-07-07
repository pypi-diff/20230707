# Comparing `tmp/lusid-notification-sdk-preview-0.1.772.7.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.774.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.772.7.tar", last modified: Thu Jul  6 10:58:32 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.774.2.tar", last modified: Thu Jul  6 14:13:53 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.772.7.tar` & `lusid-notification-sdk-preview-0.1.774.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8240 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4691 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      442 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6851 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7824 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52809 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47815 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27787 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16637 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5101 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     3401 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7256 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9019 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    11057 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     8320 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/amazon_sqs_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)    10620 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    12415 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15031 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    10459 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/email_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)     4728 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/event_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     9780 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8023 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9512 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6427 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9541 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10706 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5088 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6881 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7438 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    16039 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5156 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)    33960 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/notification_type.py
--rw-r--r--   0 root         (0) root         (0)    24079 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)     6100 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7770 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7518 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8106 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/sms_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)    16642 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     8449 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    11553 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15901 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13100 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/webhook_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)    13562 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2868 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 10:58:32.000000 lusid-notification-sdk-preview-0.1.772.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-07-06 10:58:05.000000 lusid-notification-sdk-preview-0.1.772.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-06 14:12:58.000000 lusid-notification-sdk-preview-0.1.774.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8240 2023-07-06 14:12:58.000000 lusid-notification-sdk-preview-0.1.774.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6851 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7824 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52809 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47815 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27787 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16637 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5101 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9019 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    11057 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     8320 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/amazon_sqs_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    10620 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15031 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    10459 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/email_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/event_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9780 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8023 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9512 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9541 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10706 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6881 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    16039 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)    33960 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    24079 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     6100 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7770 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8106 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/sms_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    16642 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8449 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    11553 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15901 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13100 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/webhook_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    13562 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 14:13:53.000000 lusid-notification-sdk-preview-0.1.774.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-07-06 14:12:59.000000 lusid-notification-sdk-preview-0.1.774.2/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/README.md` & `lusid-notification-sdk-preview-0.1.774.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.772.7
-- Package version: 0.1.772.7
+- API version: 0.1.774.2
+- Package version: 0.1.774.2
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.772.7"
+__version__ = "0.1.774.2"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
 from lusid_notification.api.subscriptions_api import SubscriptionsApi
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/event_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/manual_event_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.7'
+        header_params['X-LUSID-SDK-Version'] = '0.1.774.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.772.7/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.774.2/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.772.7\n"\
-               "SDK Package Version: 0.1.772.7".\
+               "Version of the API: 0.1.774.2\n"\
+               "SDK Package Version: 0.1.774.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/__init__.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/amazon_sqs_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/amazon_sqs_notification_type_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/create_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/email_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/email_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/email_notification_type_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/event_field_definition.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/event_field_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/manual_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/manual_event_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/manual_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/notification_type.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/notification_type_response.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/notification_type_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/sms_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/sms_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/sms_notification_type_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/update_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/webhook_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/models/webhook_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/models/webhook_notification_type_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.7
+    The version of the OpenAPI document: 0.1.774.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.772.7/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.774.2/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.772.7/setup.py` & `lusid-notification-sdk-preview-0.1.774.2/setup.py`

 * *Files identical despite different names*

