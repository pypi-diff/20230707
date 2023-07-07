# Comparing `tmp/resc_backend-1.3.0.tar.gz` & `tmp/resc_backend-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-1.3.0.tar", last modified: Thu May 25 09:51:22 2023, max compression
+gzip compressed data, was "resc_backend-1.4.0.tar", last modified: Fri Jul  7 10:41:44 2023, max compression
```

## Comparing `resc_backend-1.3.0.tar` & `resc_backend-1.4.0.tar`

### file list

```diff
@@ -1,113 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.436169 resc_backend-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-05-25 09:51:22.436169 resc_backend-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-25 09:51:22.436169 resc_backend-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-25 09:51:15.000000 resc_backend-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/resc_backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/resc_backend/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/bin/rabbitmq_bootup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/resc_backend/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/resc_backend/db/model/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/git_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/resc_web_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17644 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/findings.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/scans.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.436169 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/date_count_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/date_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/status_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.436169 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/findings.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/scans.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/resc_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.333938 resc_backend-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-07-07 10:41:44.333938 resc_backend-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-07 10:41:44.333938 resc_backend-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 10:41:39.000000 resc_backend-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.309938 resc_backend-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.313938 resc_backend-1.4.0/src/resc_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.317938 resc_backend-1.4.0/src/resc_backend/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/bin/rabbitmq_bootup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.317938 resc_backend-1.4.0/src/resc_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.321938 resc_backend-1.4.0/src/resc_backend/db/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/db/model/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.321938 resc_backend-1.4.0/src/resc_backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/helpers/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/helpers/git_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.321938 resc_backend-1.4.0/src/resc_backend/helpers/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/helpers/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/helpers/rabbitmq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.321938 resc_backend-1.4.0/src/resc_backend/resc_web_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.325938 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39346 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.329938 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.329938 resc_backend-1.4.0/src/resc_backend/resc_web_service/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/helpers/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.333938 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/date_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/date_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/finding_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/status_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/time_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.333938 resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-07 10:41:39.000000 resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:41:44.317938 resc_backend-1.4.0/src/resc_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-07-07 10:41:44.000000 resc_backend-1.4.0/src/resc_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-07 10:41:44.000000 resc_backend-1.4.0/src/resc_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:41:44.000000 resc_backend-1.4.0/src/resc_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-07 10:41:44.000000 resc_backend-1.4.0/src/resc_backend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:41:44.000000 resc_backend-1.4.0/src/resc_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-07 10:41:44.000000 resc_backend-1.4.0/src/resc_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 10:41:44.000000 resc_backend-1.4.0/src/resc_backend.egg-info/top_level.txt
```

### Comparing `resc_backend-1.3.0/PKG-INFO` & `resc_backend-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 1.3.0
+Version: 1.4.0
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -18,14 +18,15 @@
     - [Prerequisites](#prerequisites)
     - [Run RESC Web service locally from source](#run-resc-web-service-locally-from-source)
     - [Run RESC Web service locally through Make](#run-resc-web-service-locally-through-make)
     - [Run locally using docker](#run-locally-using-docker)
 3. [Testing](#testing)
     - [Run unit tests, linting and import checks locally](#run-unit-tests-linting-and-import-checks-locally)
     - [Run Newman tests locally](#run-newman-tests-locally)
+    - [Run OWASP ZAP API Security tests locally](#run-owasp-zap-api-security-tests-locally)
 4. [Create a migration for database changes](#create-a-migration-for-database-changes)
     - [Use Alembic to create a new migration script](#use-alembic-to-create-a-new-migration-script)
     - [Use the --autogenerate parameter](#use-the---autogenerate-parameter)
     - [Running migration and rollback](#running-migration-and-rollback)
 5. [Documentation](#documentation)
 
 <!-- ABOUT THE COMPONENT -->
@@ -179,14 +180,28 @@
 ```bash
 cd tests/newman_tests
 ./run_newman_tests.sh -b <resc-backend image:tag> -d <resc-database image:tag>  -n <newman image:tag> 
 
 Example: ./run_newman_tests.sh -b 'rescabnamro/resc-backend:1.0.1' -d 'mcr.microsoft.com/azure-sql-edge:1.0.5' -n 'postman/newman:5.3.1-alpine'
 ```
 
+### Run OWASP ZAP API Security tests locally:
+If you don't provide any argument to the script, then the default image value will be used
+```bash
+cd tests/zap_tests
+./run_run_zap_api_tests.sh
+```
+
+If you can override the images by providing below arguments to the script.
+```bash
+cd tests/zap_tests
+./run_run_zap_api_tests.sh -b <resc-backend image:tag> -d <resc-database image:tag>  -z <zap image:tag>
+
+Example: ./run_newman_tests.sh -b 'rescabnamro/resc-backend:1.0.1' -d 'mcr.microsoft.com/azure-sql-edge:1.0.5' -n 'owasp/zap2docker-weekly'
+```
 
 
 ## Create a migration for database changes
 [(Back to top)](#table-of-contents)
 
 ### Use Alembic to create a new migration script
 <details>
```

### Comparing `resc_backend-1.3.0/setup.cfg` & `resc_backend-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_backend
 description = Repository Scanner - Backend
-version = 1.3.0
+version = 1.4.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_backend-1.3.0/src/resc_backend/bin/rabbitmq_bootup.py` & `resc_backend-1.4.0/src/resc_backend/bin/rabbitmq_bootup.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/common.py` & `resc_backend-1.4.0/src/resc_backend/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/constants.py` & `resc_backend-1.4.0/src/resc_backend/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 BITBUCKET = "BITBUCKET"
 AZURE_DEVOPS = "AZURE_DEVOPS"
 GITHUB_PUBLIC = "GITHUB_PUBLIC"
 
 # RWS: RESC Web Service
 RWS_VERSION_PREFIX = "/resc/v1"
 RWS_ROUTE_REPOSITORIES = "/repositories"
-RWS_ROUTE_BRANCHES = "/branches"
 RWS_ROUTE_SCANS = "/scans"
 RWS_ROUTE_LAST_SCAN = "/last-scan"
 RWS_ROUTE_FINDINGS = "/findings"
 RWS_ROUTE_RULES = "/rules"
 RWS_ROUTE_METRICS = "/metrics"
 RWS_ROUTE_DETAILED_FINDINGS = "/detailed-findings"
 RWS_ROUTE_TOTAL_COUNT_BY_RULE = "/total-count-by-rule"
 RWS_ROUTE_BY_RULE = "/by-rule"
 RWS_ROUTE_DETECTED_RULES = "/detected-rules"
 RWS_ROUTE_FINDINGS_METADATA = "/findings-metadata"
 RWS_ROUTE_FINDING_STATUS_COUNT = "/finding-status-count"
 RWS_ROUTE_RULE_PACKS = "/rule-packs"
 RWS_ROUTE_VCS = "/vcs-instances"
 
+
+RWS_ROUTE_PERSONAL_AUDITS = "/personal-audits"
+RWS_ROUTE_AUDIT_COUNT_BY_AUDITOR_OVER_TIME = "/audit-count-by-auditor-over-time"
 RWS_ROUTE_AUDITED_COUNT_OVER_TIME = "/audited-count-over-time"
 RWS_ROUTE_UN_TRIAGED_COUNT_OVER_TIME = "/un-triaged-count-over-time"
 RWS_ROUTE_COUNT_BY_TIME = "/count-by-time"
 RWS_ROUTE_COUNT_PER_VCS_PROVIDER_BY_WEEK = "/count-per-vcs-provider-by-week"
 RWS_ROUTE_SUPPORTED_VCS_PROVIDERS = "/supported-vcs-providers"
 RWS_ROUTE_SUPPORTED_STATUSES = "/supported-statuses"
 RWS_ROUTE_DISTINCT_PROJECTS = "/distinct-projects"
@@ -36,15 +38,14 @@
 RWS_ROUTE_AUDIT = "/audit"
 
 RWS_ROUTE_AUTH_CHECK = "/auth-check"
 
 RWS_ROUTE_HEALTH = "/health"
 
 REPOSITORIES_TAG = "resc-repositories"
-BRANCHES_TAG = "resc-branches"
 SCANS_TAG = "resc-scans"
 FINDINGS_TAG = "resc-findings"
 RULES_TAG = "resc-rules"
 RULE_PACKS_TAG = "resc-rule-packs"
 HEALTH_TAG = "health"
 VCS_TAG = "resc-vcs-instances"
 METRICS_TAG = "resc-metrics"
```

### Comparing `resc_backend-1.3.0/src/resc_backend/db/connection.py` & `resc_backend-1.4.0/src/resc_backend/db/connection.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/db/model/__init__.py` & `resc_backend-1.4.0/src/resc_backend/db/model/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 Base = declarative_base()
 basedir = os.path.abspath(os.path.dirname(__file__))
 logger = logging.getLogger(__name__)
 
 
 # First Party
 from resc_backend.db.model.audit import DBaudit
-from resc_backend.db.model.branch import DBbranch
 from resc_backend.db.model.finding import DBfinding
 from resc_backend.db.model.repository import DBrepository
 from resc_backend.db.model.rule import DBrule
 from resc_backend.db.model.rule_allow_list import DBruleAllowList
 from resc_backend.db.model.rule_pack import DBrulePack
 from resc_backend.db.model.rule_tag import DBruleTag
 from resc_backend.db.model.scan import DBscan
```

### Comparing `resc_backend-1.3.0/src/resc_backend/db/model/audit.py` & `resc_backend-1.4.0/src/resc_backend/db/model/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/db/model/finding.py` & `resc_backend-1.4.0/src/resc_backend/db/model/finding.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,42 +8,42 @@
 # First Party
 from resc_backend.db.model import Base
 
 
 class DBfinding(Base):
     __tablename__ = "finding"
     id_ = Column("id", Integer, primary_key=True)
-    branch_id = Column(Integer, ForeignKey("branch.id"), nullable=False)
+    repository_id = Column(Integer, ForeignKey("repository.id"), nullable=False)
     rule_name = Column(String(400), nullable=False)
     file_path = Column(String(500), nullable=False)
     line_number = Column(Integer, nullable=False)
     column_start = Column(Integer, nullable=False, default=0)
     column_end = Column(Integer, nullable=False, default=0)
     commit_id = Column(String(120))
     commit_message = Column(Text)
     commit_timestamp = Column(DateTime, default=datetime.utcnow().isoformat())
     author = Column(String(200))
     email = Column(String(100))
     event_sent_on = Column(DateTime, nullable=True)
 
-    __table_args__ = (UniqueConstraint("commit_id", "branch_id", "rule_name", "file_path", "line_number",
-                                       "column_start", "column_end", name="uc_finding_per_branch"),)
+    __table_args__ = (UniqueConstraint("commit_id", "repository_id", "rule_name", "file_path", "line_number",
+                                       "column_start", "column_end", name="uc_finding_per_repository"),)
 
     def __init__(self, rule_name, file_path, line_number, commit_id, commit_message, commit_timestamp, author,
-                 email, event_sent_on, branch_id, column_start, column_end):
+                 email, event_sent_on, repository_id, column_start, column_end):
         self.email = email
         self.author = author
         self.commit_timestamp = commit_timestamp
         self.commit_message = commit_message
         self.commit_id = commit_id
         self.line_number = line_number
         self.file_path = file_path
         self.rule_name = rule_name
         self.event_sent_on = event_sent_on
-        self.branch_id = branch_id
+        self.repository_id = repository_id
         self.column_start = column_start
         self.column_end = column_end
 
     @staticmethod
     def create_from_finding(finding):
         db_finding = DBfinding(
             rule_name=finding.rule_name,
@@ -51,12 +51,12 @@
             line_number=finding.line_number,
             email=finding.email,
             commit_id=finding.commit_id,
             commit_message=finding.commit_message,
             commit_timestamp=finding.commit_timestamp,
             author=finding.author,
             event_sent_on=finding.event_sent_on,
-            branch_id=finding.branch_id,
+            repository_id=finding.repository_id,
             column_start=finding.column_start,
             column_end=finding.column_end
         )
         return db_finding
```

### Comparing `resc_backend-1.3.0/src/resc_backend/db/model/repository.py` & `resc_backend-1.4.0/src/resc_backend/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/db/model/rule.py` & `resc_backend-1.4.0/src/resc_backend/db/model/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/db/model/rule_allow_list.py` & `resc_backend-1.4.0/src/resc_backend/db/model/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/db/model/rule_pack.py` & `resc_backend-1.4.0/src/resc_backend/db/model/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/db/model/scan.py` & `resc_backend-1.4.0/src/resc_backend/db/model/scan.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,41 +6,41 @@
 
 # First Party
 from resc_backend.constants import BASE_SCAN
 from resc_backend.db.model import Base
 from resc_backend.db.model.rule_pack import DBrulePack
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 
-BRANCH_ID = "branch.id"
+REPOSITORY_ID = "repository.id"
 
 
 class DBscan(Base):
     __tablename__ = "scan"
     id_ = Column("id", Integer, primary_key=True)
-    branch_id = Column(Integer, ForeignKey(BRANCH_ID))
+    repository_id = Column(Integer, ForeignKey(REPOSITORY_ID))
     rule_pack = Column(String(100), ForeignKey(DBrulePack.version), nullable=False)
     scan_type = Column(Enum(ScanType), default=ScanType.BASE, server_default=BASE_SCAN, nullable=False)
     last_scanned_commit = Column(String(100), nullable=False)
     timestamp = Column(DateTime, nullable=False, default=datetime.utcnow)
     increment_number = Column(Integer, server_default=text("0"), default=0, nullable=False)
 
-    def __init__(self, branch_id: int, scan_type: ScanType, last_scanned_commit: str, timestamp: datetime,
+    def __init__(self, repository_id: int, scan_type: ScanType, last_scanned_commit: str, timestamp: datetime,
                  increment_number: int, rule_pack: str):
-        self.branch_id = branch_id
+        self.repository_id = repository_id
         self.scan_type = scan_type
         self.last_scanned_commit = last_scanned_commit
         self.timestamp = timestamp
         self.increment_number = increment_number
         self.rule_pack = rule_pack
 
     @staticmethod
     def create_from_metadata(timestamp: datetime, scan_type: ScanType, last_scanned_commit: str, increment_number: int,
-                             rule_pack: str, branch_id: int):
+                             rule_pack: str, repository_id: int):
         db_scan = DBscan(
             timestamp=timestamp,
             scan_type=scan_type,
             last_scanned_commit=last_scanned_commit,
             increment_number=increment_number,
             rule_pack=rule_pack,
-            branch_id=branch_id
+            repository_id=repository_id
         )
         return db_scan
```

### Comparing `resc_backend-1.3.0/src/resc_backend/db/model/vcs_instance.py` & `resc_backend-1.4.0/src/resc_backend/db/model/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/helpers/dict_remapper.py` & `resc_backend-1.4.0/src/resc_backend/helpers/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/helpers/environment_wrapper.py` & `resc_backend-1.4.0/src/resc_backend/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/helpers/git_operation.py` & `resc_backend-1.4.0/src/resc_backend/helpers/git_operation.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,33 +8,30 @@
 # Third Party
 from git import Repo  # noqa: E402
 
 logger = logging.getLogger(__name__)
 
 
 def clone_repository(repository_url: str,
-                     branch_name: str,
                      repo_clone_path: str,
                      username: str = "",
                      personal_access_token: str = ""):
     """
         Clones the given repository
     :param repository_url:
         Repository url to clone
-    :param branch_name:
-        Branch name of the repository url to clone
     :param repo_clone_path:
         Path where to clone the repository
     :param username:
         Username to clone the repository, only needed if the repository is private
     :param personal_access_token:
         Personal access token|password to clone the repository, only needed if the repository is private
     """
     url = repository_url.replace("https://", "")
     if username:
         repo_clone_url = f"https://{username}:{personal_access_token}@{url}"
     else:
         repo_clone_url = f"https://{personal_access_token}@{url}"
         logger.debug(f"username is not specified, so cloning the repository with only personal access token: {url}")
 
-    Repo.clone_from(repo_clone_url, repo_clone_path, branch=branch_name)
-    logger.debug(f"Repository {repository_url}:{branch_name} cloned successfully")
+    Repo.clone_from(repo_clone_url, repo_clone_path)
+    logger.debug(f"Repository {repository_url} cloned successfully")
```

### Comparing `resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/configuration.py` & `resc_backend-1.4.0/src/resc_backend/helpers/rabbitmq/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py` & `resc_backend-1.4.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/api.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # pylint: disable=C0413,W0611,W0404
 # Standard Library
 import logging.config
 import os
 
 # Third Party
-from fastapi import Depends, FastAPI
+from fastapi import Depends, FastAPI, Request
 from fastapi.middleware.cors import CORSMiddleware
+from fastapi.middleware import Middleware
+from fastapi.middleware.trustedhost import TrustedHostMiddleware
 from starlette.responses import RedirectResponse
 from starlette.status import HTTP_302_FOUND
 from tenacity import RetryError
 
 # First Party
 from resc_backend.common import get_package_version
 from resc_backend.constants import RWS_VERSION_PREFIX
 from resc_backend.db.connection import Session, engine
 from resc_backend.resc_web_service.dependencies import (
     check_db_initialized,
     requires_auth,
-    requires_no_auth
+    requires_no_auth,
+    add_security_headers
 )
 from resc_backend.resc_web_service.endpoints import (
-    branches,
     common,
     detailed_findings,
     findings,
     health,
     metrics,
     repositories,
     rules,
@@ -88,15 +90,14 @@
 logger = logging.getLogger(__name__)
 tags_metadata = [
     {"name": "health", "description": "Checks health for API"},
     {"name": "resc-common", "description": "Manage common information"},
     {"name": "resc-rules", "description": "Manage rule information"},
     {"name": "resc-rule-packs", "description": "Manage rule pack information"},
     {"name": "resc-repositories", "description": "Manage repository information"},
-    {"name": "resc-branches", "description": "Manage branch information"},
     {"name": "resc-scans", "description": "Manage scan information"},
     {"name": "resc-findings", "description": "Manage findings information"},
     {"name": "resc-vcs-instances", "description": "Manage vcs instance information"},
     {"name": "resc-metrics", "description": "Retrieve metrics"},
 ]
 
 # Check if authentication is required for api endpoints
@@ -116,24 +117,28 @@
         allow_credentials=True,
         allow_methods=["*"],
         allow_headers=["*"],
     )
 
 app.include_router(health.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(common.router, prefix=RWS_VERSION_PREFIX)
-app.include_router(branches.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(rules.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(rule_packs.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(findings.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(detailed_findings.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(repositories.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(scans.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(vcs_instances.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(metrics.router, prefix=RWS_VERSION_PREFIX)
 
+
+# Apply the security headers to the app in the form of middleware
+app.middleware("http")(add_security_headers)
+
+
 # Add exception handlers
 add_exception_handlers(app=app)
 
 
 @app.on_event("startup")
 def app_startup():
     try:
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/detailed_finding.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/detailed_finding.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,21 @@
         integer amount of records to skip to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     :return: [DetailedFindingRead]
         The output will contain a list of DetailedFindingRead objects,
         or an empty list if no finding was found for the given findings_filter
     """
-    max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+    max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
                                                  func.max(model.DBscan.id_).label("latest_base_scan_id"))
     max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
     if findings_filter.rule_pack_versions:
         max_base_scan_subquery = max_base_scan_subquery.filter(
             model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
-    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
+    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
 
     # subquery to select latest audit ids of findings
     max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                              func.max(model.DBaudit.id_).label("audit_id")) \
         .group_by(model.DBaudit.finding_id).subquery()
 
     rule_tag_subquery = db_connection.query(model.DBruleTag.rule_id) \
@@ -74,33 +74,31 @@
         model.DBaudit.status,
         model.DBaudit.comment,
         model.DBfinding.rule_name,
         model.DBscan.rule_pack,
         model.DBfinding.event_sent_on,
         model.DBscan.timestamp,
         model.DBscan.id_.label("scan_id"),
-        model.DBbranch.branch_name,
         model.DBscan.last_scanned_commit,
         model.DBVcsInstance.provider_type.label("vcs_provider"),
         model.DBrepository.project_key,
         model.DBrepository.repository_name,
         model.DBrepository.repository_url,
     )
     query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
     if findings_filter.scan_ids:
         query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
                                               model.DBscan.id_.in_(findings_filter.scan_ids)))
     else:
-        query = query.join(max_base_scan_subquery, model.DBfinding.branch_id == max_base_scan_subquery.c.branch_id)
+        query = query.join(max_base_scan_subquery,
+                           model.DBfinding.repository_id == max_base_scan_subquery.c.repository_id)
         query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
                                               model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
-    query = query.join(model.DBbranch,
-                       model.branch.DBbranch.id_ == model.finding.DBfinding.branch_id) \
-        .join(model.DBrepository,
-              model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
+    query = query.join(model.DBrepository,
+                       model.repository.DBrepository.id_ == model.finding.DBfinding.repository_id) \
         .join(model.DBVcsInstance,
               model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
     query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
                        isouter=True)
     query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
                                            model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
                        isouter=True)
@@ -119,16 +117,14 @@
 
     if findings_filter.event_sent is not None:
         if findings_filter.event_sent:
             query = query.filter(model.finding.DBfinding.event_sent_on.is_not(None))
         else:
             query = query.filter(model.finding.DBfinding.event_sent_on.is_(None))
 
-    if findings_filter.branch_name:
-        query = query.filter(model.DBbranch.branch_name == findings_filter.branch_name)
     if findings_filter.repository_name:
         query = query.filter(model.DBrepository.repository_name == findings_filter.repository_name)
     if findings_filter.vcs_providers and findings_filter.vcs_providers is not None:
         query = query.filter(model.vcs_instance.DBVcsInstance.provider_type.in_(findings_filter.vcs_providers))
     if findings_filter.project_name:
         query = query.filter(model.repository.DBrepository.project_key == findings_filter.project_name)
     if findings_filter.rule_names:
@@ -158,21 +154,21 @@
         count of findings
     """
     # subquery to select latest audit ids of findings
     max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                              func.max(model.DBaudit.id_).label("audit_id")) \
         .group_by(model.DBaudit.finding_id).subquery()
 
-    max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+    max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
                                                  func.max(model.DBscan.id_).label("latest_base_scan_id"))
     max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
     if findings_filter.rule_pack_versions:
         max_base_scan_subquery = max_base_scan_subquery.filter(
             model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
-    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
+    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
 
     rule_tag_subquery = db_connection.query(model.DBruleTag.rule_id) \
         .join(model.DBtag, model.DBruleTag.tag_id == model.DBtag.id_)
     if findings_filter.rule_tags:
         rule_tag_subquery = rule_tag_subquery.filter(model.DBtag.name.in_(findings_filter.rule_tags))
     if findings_filter.rule_pack_versions or findings_filter.rule_names:
         rule_tag_subquery = rule_tag_subquery.join(model.DBrule, model.DBrule.id_ == model.DBruleTag.rule_id)
@@ -185,22 +181,21 @@
     query = db_connection.query(func.count(model.DBfinding.id_))
 
     query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
     if findings_filter.scan_ids:
         query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
                                               model.DBscan.id_.in_(findings_filter.scan_ids)))
     else:
-        query = query.join(max_base_scan_subquery, model.DBfinding.branch_id == max_base_scan_subquery.c.branch_id)
+        query = query.join(max_base_scan_subquery,
+                           model.DBfinding.repository_id == max_base_scan_subquery.c.repository_id)
         query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
                                               model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
 
-    query = query.join(model.DBbranch,
-                       model.branch.DBbranch.id_ == model.finding.DBfinding.branch_id) \
-        .join(model.DBrepository,
-              model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
+    query = query.join(model.DBrepository,
+                       model.repository.DBrepository.id_ == model.finding.DBfinding.repository_id) \
         .join(model.DBVcsInstance,
               model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
     query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
                        isouter=True)
     query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
                                            model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
                        isouter=True)
@@ -219,16 +214,14 @@
 
     if findings_filter.event_sent is not None:
         if findings_filter.event_sent:
             query = query.filter(model.finding.DBfinding.event_sent_on.is_not(None))
         else:
             query = query.filter(model.finding.DBfinding.event_sent_on.is_(None))
 
-    if findings_filter.branch_name:
-        query = query.filter(model.DBbranch.branch_name == findings_filter.branch_name)
     if findings_filter.repository_name:
         query = query.filter(model.DBrepository.repository_name == findings_filter.repository_name)
     if findings_filter.vcs_providers and findings_filter.vcs_providers is not None:
         query = query.filter(model.vcs_instance.DBVcsInstance.provider_type.in_(findings_filter.vcs_providers))
     if findings_filter.project_name:
         query = query.filter(model.repository.DBrepository.project_key == findings_filter.project_name)
     if findings_filter.rule_names:
@@ -278,27 +271,24 @@
         model.DBfinding.email,
         model.DBaudit.status,
         model.DBaudit.comment,
         model.DBfinding.rule_name,
         model.DBscan.rule_pack,
         model.DBscan.timestamp,
         scan_id,
-        model.DBbranch.branch_name,
         model.DBscan.last_scanned_commit,
         model.DBVcsInstance.provider_type.label("vcs_provider"),
         model.DBrepository.project_key,
         model.DBrepository.repository_name,
         model.DBrepository.repository_url,
     ).join(max_scan_subquery, model.finding.DBfinding.id_ == max_scan_subquery.c.finding_id) \
         .join(model.DBscan,
               model.scan.DBscan.id_ == max_scan_subquery.c.scan_id) \
-        .join(model.DBbranch,
-              model.branch.DBbranch.id_ == model.scan.DBscan.branch_id) \
         .join(model.DBrepository,
-              model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
+              model.repository.DBrepository.id_ == model.scan.DBscan.repository_id) \
         .join(model.DBVcsInstance,
               model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance) \
         .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
               isouter=True) \
         .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
                                   model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
               isouter=True) \
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/finding.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/finding.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,39 +35,40 @@
     return db_finding
 
 
 def create_findings(db_connection: Session, findings: List[finding_schema.FindingCreate]) -> List[model.DBfinding]:
     if len(findings) < 1:
         # Function is called with an empty list of findings
         return []
-    branch_id = findings[0].branch_id
+    repository_id = findings[0].repository_id
 
-    # get a list of known / registered findings for this branch
-    db_branch_findings = db_connection.query(model.DBfinding).filter(model.DBfinding.branch_id == branch_id).all()
+    # get a list of known / registered findings for this repository
+    db_repository_findings = db_connection.query(model.DBfinding).\
+        filter(model.DBfinding.repository_id == repository_id).all()
 
     # Compare new findings list with findings in the db
     new_findings = findings[:]
     db_findings = []
     for finding in findings:
-        for branch_finding in db_branch_findings:
+        for repository_finding in db_repository_findings:
             # Compare based on the unique key in the findings table
-            if branch_finding.commit_id == finding.commit_id and \
-                    branch_finding.rule_name == finding.rule_name and \
-                    branch_finding.file_path == finding.file_path and \
-                    branch_finding.line_number == finding.line_number and \
-                    branch_finding.column_start == finding.column_start and \
-                    branch_finding.column_end == finding.column_end:
+            if repository_finding.commit_id == finding.commit_id and \
+                    repository_finding.rule_name == finding.rule_name and \
+                    repository_finding.file_path == finding.file_path and \
+                    repository_finding.line_number == finding.line_number and \
+                    repository_finding.column_start == finding.column_start and \
+                    repository_finding.column_end == finding.column_end:
                 # Store the already known finding
-                db_findings.append(branch_finding)
-                # Remove from the db_branch_findings to increase performance for the next loop
-                db_branch_findings.remove(branch_finding)
+                db_findings.append(repository_finding)
+                # Remove from the db_repository_findings to increase performance for the next loop
+                db_repository_findings.remove(repository_finding)
                 # Remove from the to be created findings
                 new_findings.remove(finding)
                 break
-    logger.info(f"create_findings branch {branch_id}, Requested: {len(findings)}. "
+    logger.info(f"create_findings repository {repository_id}, Requested: {len(findings)}. "
                 f"New findings: {len(new_findings)}. Already in db: {len(db_findings)}")
 
     db_create_findings = []
     # Map the to be created findings to the DBfinding type object
     for new_finding in new_findings:
         db_create_finding = model.finding.DBfinding.create_from_finding(new_finding)
         db_create_findings.append(db_create_finding)
@@ -171,37 +172,33 @@
             total_count_query = total_count_query \
                 .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
                       isouter=True) \
                 .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
                                           model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
                       isouter=True)
         if (findings_filter.vcs_providers and findings_filter.vcs_providers is not None) \
-                or findings_filter.project_name or findings_filter.branch_name \
+                or findings_filter.project_name \
                 or findings_filter.repository_name or findings_filter.start_date_time \
                 or findings_filter.end_date_time:
             total_count_query = total_count_query \
                 .join(model.DBscanFinding,
                       model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_) \
                 .join(model.DBscan,
                       model.scan.DBscan.id_ == model.scan_finding.DBscanFinding.scan_id) \
-                .join(model.DBbranch,
-                      model.branch.DBbranch.id_ == model.scan.DBscan.branch_id) \
                 .join(model.DBrepository,
-                      model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
+                      model.repository.DBrepository.id_ == model.scan.DBscan.repository_id) \
                 .join(model.DBVcsInstance,
                       model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
 
         if findings_filter.start_date_time:
             total_count_query = total_count_query.filter(
                 model.scan.DBscan.timestamp >= findings_filter.start_date_time)
         if findings_filter.end_date_time:
             total_count_query = total_count_query.filter(model.scan.DBscan.timestamp <= findings_filter.end_date_time)
 
-        if findings_filter.branch_name:
-            total_count_query = total_count_query.filter(model.DBbranch.branch_name == findings_filter.branch_name)
         if findings_filter.repository_name:
             total_count_query = total_count_query.filter(
                 model.DBrepository.repository_name == findings_filter.repository_name)
 
         if findings_filter.vcs_providers and findings_filter.vcs_providers is not None:
             total_count_query = total_count_query.filter(
                 model.vcs_instance.DBVcsInstance.provider_type.in_(findings_filter.vcs_providers))
@@ -279,18 +276,16 @@
     if (vcs_providers or project_name or repository_name or start_date_time or end_date_time or rule_pack_versions) \
             and scan_id < 0:
         query = query \
             .join(model.DBscanFinding,
                   model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_) \
             .join(model.DBscan,
                   model.scan.DBscan.id_ == model.scan_finding.DBscanFinding.scan_id) \
-            .join(model.DBbranch,
-                  model.branch.DBbranch.id_ == model.scan.DBscan.branch_id) \
             .join(model.DBrepository,
-                  model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
+                  model.repository.DBrepository.id_ == model.scan.DBscan.repository_id) \
             .join(model.DBVcsInstance,
                   model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
     if finding_statuses:
         # subquery to select latest audit ids findings
         max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                                  func.max(model.DBaudit.id_).label("audit_id")) \
             .group_by(model.DBaudit.finding_id).subquery()
@@ -400,27 +395,27 @@
     :return: findings_count
         per rulename and status the count of findings
     """
     query = db_connection.query(model.DBfinding.rule_name,
                                 model.DBaudit.status,
                                 func.count(model.DBfinding.id_))
 
-    max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+    max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
                                                  func.max(model.DBscan.id_).label("latest_base_scan_id"))
     max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
     if rule_pack_versions:
         max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.rule_pack.in_(rule_pack_versions))
-    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
+    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
 
     max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                              func.max(model.DBaudit.id_).label("audit_id")) \
         .group_by(model.DBaudit.finding_id).subquery()
 
     query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
-    query = query.join(max_base_scan_subquery, model.DBfinding.branch_id == max_base_scan_subquery.c.branch_id)
+    query = query.join(max_base_scan_subquery, model.DBfinding.repository_id == max_base_scan_subquery.c.repository_id)
     query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
                                           model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
     if rule_tags:
         rule_tag_subquery = db_connection.query(model.DBruleTag.rule_id) \
             .join(model.DBtag, model.DBruleTag.tag_id == model.DBtag.id_)
         if rule_pack_versions:
             rule_tag_subquery = rule_tag_subquery.join(model.DBrule, model.DBrule.id_ == model.DBruleTag.rule_id)
@@ -596,55 +591,38 @@
 
     db_connection.query(model.DBfinding) \
         .filter(model.finding.DBfinding.id_ == finding_id) \
         .delete(synchronize_session=False)
     db_connection.commit()
 
 
-def delete_findings_by_branch_id(db_connection: Session, branch_id: int):
-    """
-        Delete findings for a given branch
-    :param db_connection:
-        Session of the database connection
-    :param branch_id:
-        id of the branch
-    """
-    db_connection.query(model.DBfinding) \
-        .filter(model.finding.DBfinding.branch_id == branch_id) \
-        .delete(synchronize_session=False)
-    db_connection.commit()
-
-
 def delete_findings_by_repository_id(db_connection: Session, repository_id: int):
     """
         Delete findings for a given repository
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository
     """
     db_connection.query(model.DBfinding) \
-        .filter(model.finding.DBfinding.branch_id == model.branch.DBbranch.id_,
-                model.branch.DBbranch.repository_id == model.repository.DBrepository.id_,
-                model.repository.DBrepository.id_ == repository_id) \
+        .filter(model.finding.DBfinding.repository_id == repository_id) \
         .delete(synchronize_session=False)
     db_connection.commit()
 
 
 def delete_findings_by_vcs_instance_id(db_connection: Session, vcs_instance_id: int):
     """
         Delete findings for a given vcs instance
     :param db_connection:
         Session of the database connection
     :param vcs_instance_id:
         id of the vcs instance
     """
     db_connection.query(model.DBfinding) \
-        .filter(model.finding.DBfinding.branch_id == model.branch.DBbranch.id_,
-                model.branch.DBbranch.repository_id == model.repository.DBrepository.id_,
+        .filter(model.finding.DBfinding.repository_id == model.repository.DBrepository.id_,
                 model.repository.DBrepository.vcs_instance == model.vcs_instance.DBVcsInstance.id_,
                 model.vcs_instance.DBVcsInstance.id_ == vcs_instance_id) \
         .delete(synchronize_session=False)
     db_connection.commit()
 
 
 def get_finding_audit_status_count_over_time(db_connection: Session, status: FindingStatus, weeks: int = 13) -> dict:
@@ -669,16 +647,15 @@
                                     )
         max_audit_subquery = db_connection.query(func.max(model.DBaudit.id_).label("audit_id")) \
             .filter(extract('year', model.DBaudit.timestamp) == extract('year', last_nth_week_date_time)) \
             .filter(extract('week', model.DBaudit.timestamp) <= extract('week', last_nth_week_date_time)) \
             .group_by(model.DBaudit.finding_id).subquery()
         query = query.join(max_audit_subquery, max_audit_subquery.c.audit_id == model.DBaudit.id_)
         query = query.join(model.DBfinding, model.DBfinding.id_ == model.DBaudit.finding_id)
-        query = query.join(model.DBbranch, model.DBbranch.id_ == model.DBfinding.branch_id)
-        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBbranch.repository_id)
+        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBfinding.repository_id)
         query = query.join(model.DBVcsInstance, model.DBVcsInstance.id_ == model.DBrepository.vcs_instance)
         query = query.filter(model.DBaudit.status == status)
         query = query.group_by(model.DBVcsInstance.provider_type)
 
         all_tables.append(query)
 
     # union
@@ -702,35 +679,34 @@
         last_nth_week_date_time = datetime.utcnow() - timedelta(weeks=week)
         query = db_connection.query(extract('year', last_nth_week_date_time).label("year"),
                                     extract('week', last_nth_week_date_time).label("week"),
                                     model.DBVcsInstance.provider_type.label("provider_type"),
                                     func.count(model.DBfinding.id_).label("finding_count")
                                     )
         max_base_scan = db_connection.query(func.max(model.DBscan.id_).label("scan_id"),
-                                            model.DBscan.branch_id) \
+                                            model.DBscan.repository_id) \
             .filter(extract('year', model.DBscan.timestamp) == extract('year', last_nth_week_date_time)) \
             .filter(extract('week', model.DBscan.timestamp) <= extract('week', last_nth_week_date_time)) \
             .filter(model.DBscan.scan_type == ScanType.BASE) \
-            .group_by(model.DBscan.branch_id).subquery()
+            .group_by(model.DBscan.repository_id).subquery()
 
         query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
         query = query.join(model.DBscan, model.DBscan.id_ == model.DBscanFinding.scan_id)
-        query = query.join(max_base_scan, and_(max_base_scan.c.branch_id == model.DBscan.branch_id,
+        query = query.join(max_base_scan, and_(max_base_scan.c.repository_id == model.DBscan.repository_id,
                                                or_(model.DBscan.id_ == max_base_scan.c.scan_id,
                                                    (and_(model.DBscan.id_ > max_base_scan.c.scan_id,
                                                          model.DBscan.scan_type == ScanType.INCREMENTAL,
                                                          extract('week', model.DBscan.timestamp) <=
                                                          extract('week', last_nth_week_date_time),
                                                          extract('year', model.DBscan.timestamp) ==
                                                          extract('year', last_nth_week_date_time)))
                                                    )
                                                )
                            )
-        query = query.join(model.DBbranch, model.DBbranch.id_ == model.DBscan.branch_id)
-        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBbranch.repository_id)
+        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBscan.repository_id)
         query = query.join(model.DBVcsInstance, model.DBVcsInstance.id_ == model.DBrepository.vcs_instance)
         query = query.group_by(model.DBVcsInstance.provider_type)
 
         all_tables.append(query)
 
     # union
     unioned_query = union(*all_tables)
@@ -753,41 +729,40 @@
         last_nth_week_date_time = datetime.utcnow() - timedelta(weeks=week)
         query = db_connection.query(extract('year', last_nth_week_date_time).label("year"),
                                     extract('week', last_nth_week_date_time).label("week"),
                                     model.DBVcsInstance.provider_type.label("provider_type"),
                                     func.count(model.DBfinding.id_).label("finding_count")
                                     )
         max_base_scan = db_connection.query(func.max(model.DBscan.id_).label("scan_id"),
-                                            model.DBscan.branch_id) \
+                                            model.DBscan.repository_id) \
             .filter(extract('year', model.DBscan.timestamp) == extract('year', last_nth_week_date_time)) \
             .filter(extract('week', model.DBscan.timestamp) <= extract('week', last_nth_week_date_time)) \
             .filter(model.DBscan.scan_type == ScanType.BASE) \
-            .group_by(model.DBscan.branch_id).subquery()
+            .group_by(model.DBscan.repository_id).subquery()
 
         max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                                  func.max(model.DBaudit.id_).label("audit_id")) \
             .filter(extract('year', model.DBaudit.timestamp) == extract('year', last_nth_week_date_time)) \
             .filter(extract('week', model.DBaudit.timestamp) <= extract('week', last_nth_week_date_time)) \
             .group_by(model.DBaudit.finding_id).subquery()
 
         query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
         query = query.join(model.DBscan, model.DBscan.id_ == model.DBscanFinding.scan_id)
-        query = query.join(max_base_scan, and_(max_base_scan.c.branch_id == model.DBscan.branch_id,
+        query = query.join(max_base_scan, and_(max_base_scan.c.repository_id == model.DBscan.repository_id,
                                                or_(model.DBscan.id_ == max_base_scan.c.scan_id,
                                                    (and_(model.DBscan.id_ > max_base_scan.c.scan_id,
                                                          model.DBscan.scan_type == ScanType.INCREMENTAL,
                                                          extract('week', model.DBscan.timestamp) <=
                                                          extract('week', last_nth_week_date_time),
                                                          extract('year', model.DBscan.timestamp) ==
                                                          extract('year', last_nth_week_date_time)))
                                                    )
                                                )
                            )
-        query = query.join(model.DBbranch, model.DBbranch.id_ == model.DBscan.branch_id)
-        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBbranch.repository_id)
+        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBscan.repository_id)
         query = query.join(model.DBVcsInstance, model.DBVcsInstance.id_ == model.DBrepository.vcs_instance)
 
         query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
                            isouter=True)
         query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
                                                model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
                            isouter=True)
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/repository.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Third Party
 from sqlalchemy import and_, func
 from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
 from resc_backend.db import model
-from resc_backend.resc_web_service.crud import branch as branch_crud
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import scan as scan_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.schema import repository as repository_schema
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
@@ -34,40 +33,53 @@
         optional, filter on repository name. Is used as a string contains filter
     :param only_if_has_findings:
         optional, filter on repositories with findings
     :return: repositories
         list of DBrepository objects
     """
     limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+
+    # Get the latest scan for repository
+    repo_last_scan_sub_query = db_connection.query(model.DBscan.repository_id,
+                                                   func.max(model.DBscan.timestamp).label("max_timestamp"))
+    repo_last_scan_sub_query = repo_last_scan_sub_query.group_by(model.DBscan.repository_id).subquery()
+
     query = db_connection.query(
         model.DBrepository.id_,
         model.DBrepository.project_key,
         model.DBrepository.repository_id,
         model.DBrepository.repository_name,
         model.DBrepository.repository_url,
         model.DBrepository.vcs_instance,
-        model.DBVcsInstance.provider_type) \
-        .join(model.DBVcsInstance,
-              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
+        model.DBVcsInstance.provider_type,
+        func.coalesce(model.DBscan.id_, None).label('last_scan_id'),
+        func.coalesce(model.DBscan.timestamp, None).label('last_scan_timestamp'))
+    query = query.join(model.DBVcsInstance,
+                       model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
+    query = query.join(repo_last_scan_sub_query,
+                       model.repository.DBrepository.id_ == repo_last_scan_sub_query.c.repository_id, isouter=True)
+    query = query.join(model.DBscan,
+                       and_(model.scan.DBscan.repository_id == model.repository.DBrepository.id_,
+                            model.scan.DBscan.timestamp == repo_last_scan_sub_query.c.max_timestamp), isouter=True)
 
     if only_if_has_findings:
-        max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+        max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
                                                      func.max(model.DBscan.id_).label("latest_base_scan_id"))
         max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
-        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
+        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
 
         sub_query = db_connection.query(model.DBrepository.id_)
-        sub_query = sub_query.join(model.DBbranch, model.DBbranch.repository_id == model.DBrepository.id_)
-        sub_query = sub_query.join(max_base_scan_subquery, model.DBbranch.id_ == max_base_scan_subquery.c.branch_id)
-        sub_query = sub_query.join(model.DBscan, and_(model.DBbranch.id_ == model.DBscan.branch_id,
+        sub_query = sub_query.join(max_base_scan_subquery,
+                                   model.DBrepository.id_ == max_base_scan_subquery.c.repository_id)
+        sub_query = sub_query.join(model.DBscan, and_(model.DBrepository.id_ == model.DBscan.repository_id,
                                                       model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
         sub_query = sub_query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
         sub_query = sub_query.distinct()
 
-        # Filter on repositories that are in the branches selection
+        # Filter on repositories that are in the selection
         query = query.filter(model.DBrepository.id_.in_(sub_query))
 
     if vcs_providers and vcs_providers is not None:
         query = query.filter(model.DBVcsInstance.provider_type.in_(vcs_providers))
 
     if project_filter:
         query = query.filter(model.DBrepository.project_key == project_filter)
@@ -96,28 +108,28 @@
         optional, filter on repositories with findings
     :return: total_count
         count of repositories
     """
     query = db_connection.query(func.count(model.DBrepository.id_))
 
     if only_if_has_findings:
-        max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+        max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
                                                      func.max(model.DBscan.id_).label("latest_base_scan_id"))
         max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
-        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
+        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
 
         sub_query = db_connection.query(model.DBrepository.id_)
-        sub_query = sub_query.join(model.DBbranch, model.DBbranch.repository_id == model.DBrepository.id_)
-        sub_query = sub_query.join(max_base_scan_subquery, model.DBbranch.id_ == max_base_scan_subquery.c.branch_id)
-        sub_query = sub_query.join(model.DBscan, and_(model.DBbranch.id_ == model.DBscan.branch_id,
+        sub_query = sub_query.join(max_base_scan_subquery,
+                                   model.DBrepository.id_ == max_base_scan_subquery.c.repository_id)
+        sub_query = sub_query.join(model.DBscan, and_(model.DBrepository.id_ == model.DBscan.repository_id,
                                                       model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
         sub_query = sub_query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
         sub_query = sub_query.distinct()
 
-        # Filter on repositories that are in the branches selection
+        # Filter on repositories that are in the selection
         query = query.filter(model.DBrepository.id_.in_(sub_query))
 
     if vcs_providers and vcs_providers is not None:
         query = query.join(model.DBVcsInstance,
                            model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
         query = query.filter(model.DBVcsInstance.provider_type.in_(vcs_providers))
 
@@ -192,22 +204,21 @@
         optional, filter on repositories that have findings
     :return: distinct_projects
         The output will contain a list of unique projects
     """
     query = db_connection.query(model.DBrepository.project_key)
 
     if only_if_has_findings:
-        max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+        max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
                                                      func.max(model.DBscan.id_).label("latest_base_scan_id"))
         max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
-        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
+        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
 
-        query = query.join(model.DBbranch, model.DBbranch.repository_id == model.DBrepository.id_)
-        query = query.join(max_base_scan_subquery, model.DBbranch.id_ == max_base_scan_subquery.c.branch_id)
-        query = query.join(model.DBscan, and_(model.DBbranch.id_ == model.DBscan.branch_id,
+        query = query.join(max_base_scan_subquery, model.DBrepository.id_ == max_base_scan_subquery.c.repository_id)
+        query = query.join(model.DBscan, and_(model.DBrepository.id_ == model.DBscan.repository_id,
                                               model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
         query = query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
 
     if vcs_providers and vcs_providers is not None:
         query = query.join(model.DBVcsInstance,
                            model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
         query = query.filter(model.DBVcsInstance.provider_type.in_(vcs_providers))
@@ -233,22 +244,21 @@
         optional, filter on repositories that have findings
     :return: distinct_repositories
         The output will contain a list of unique repositories
     """
     query = db_connection.query(model.DBrepository.repository_name)
 
     if only_if_has_findings:
-        max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+        max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
                                                      func.max(model.DBscan.id_).label("latest_base_scan_id"))
         max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
-        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
+        max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
 
-        query = query.join(model.DBbranch, model.DBbranch.repository_id == model.DBrepository.id_)
-        query = query.join(max_base_scan_subquery, model.DBbranch.id_ == max_base_scan_subquery.c.branch_id)
-        query = query.join(model.DBscan, and_(model.DBbranch.id_ == model.DBscan.branch_id,
+        query = query.join(max_base_scan_subquery, model.DBrepository.id_ == max_base_scan_subquery.c.repository_id)
+        query = query.join(model.DBscan, and_(model.DBrepository.id_ == model.DBscan.repository_id,
                                               model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
         query = query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
 
     if vcs_providers and vcs_providers is not None:
         query = query.join(model.DBVcsInstance,
                            model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
         query = query.filter(model.DBVcsInstance.provider_type.in_(vcs_providers))
@@ -270,26 +280,25 @@
     :return: findings_metadata
         findings_metadata containing the count for each status
     """
     query = db_connection.query(model.DBrepository.id_,
                                 model.DBaudit.status,
                                 func.count(model.DBscanFinding.finding_id))
 
-    max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+    max_base_scan_subquery = db_connection.query(model.DBscan.repository_id,
                                                  func.max(model.DBscan.id_).label("latest_base_scan_id"))
     max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
-    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
+    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.repository_id).subquery()
 
     max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                              func.max(model.DBaudit.id_).label("audit_id")) \
         .group_by(model.DBaudit.finding_id).subquery()
 
-    query = query.join(model.DBbranch, model.DBbranch.repository_id == model.DBrepository.id_)
-    query = query.join(max_base_scan_subquery, model.DBbranch.id_ == max_base_scan_subquery.c.branch_id)
-    query = query.join(model.DBscan, and_(model.DBbranch.id_ == model.DBscan.branch_id,
+    query = query.join(max_base_scan_subquery, model.DBrepository.id_ == max_base_scan_subquery.c.repository_id)
+    query = query.join(model.DBscan, and_(model.DBrepository.id_ == model.DBscan.repository_id,
                                           model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
     query = query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
     query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.DBscanFinding.finding_id,
                        isouter=True)
     query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.DBscanFinding.finding_id,
                                            model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id), isouter=True)
     query = query.filter(model.DBrepository.id_.in_(repository_ids))
@@ -331,15 +340,14 @@
     :param delete_related:
         if related records need to be deleted
     """
     if delete_related:
         scan_finding_crud.delete_scan_finding_by_repository_id(db_connection, repository_id=repository_id)
         finding_crud.delete_findings_by_repository_id(db_connection, repository_id=repository_id)
         scan_crud.delete_scans_by_repository_id(db_connection, repository_id=repository_id)
-        branch_crud.delete_branches_by_repository_id(db_connection, repository_id=repository_id)
     db_connection.query(model.DBrepository) \
         .filter(model.repository.DBrepository.id_ == repository_id) \
         .delete(synchronize_session=False)
     db_connection.commit()
 
 
 def delete_repositories_by_vcs_instance_id(db_connection: Session, vcs_instance_id: int):
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule_pack.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule_tag.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/rule_tag.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/scan_finding.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/scan_finding.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,45 +47,27 @@
             query = query.filter(model.scan_finding.DBscanFinding.finding_id == finding_id)
         if scan_id:
             query = query.filter(model.scan_finding.DBscanFinding.scan_id == scan_id)
         query.delete(synchronize_session=False)
         db_connection.commit()
 
 
-def delete_scan_finding_by_branch_id(db_connection: Session, branch_id: int):
-    """
-        Delete scan findings for a given branch
-    :param db_connection:
-        Session of the database connection
-    :param branch_id:
-        id of the branch
-    """
-    db_connection.query(model.DBscanFinding) \
-        .filter(model.scan_finding.DBscanFinding.scan_id == model.scan.DBscan.id_,
-                model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_,
-                model.scan.DBscan.branch_id == model.finding.DBfinding.branch_id,
-                model.scan.DBscan.branch_id == branch_id) \
-        .delete(synchronize_session=False)
-    db_connection.commit()
-
-
 def delete_scan_finding_by_repository_id(db_connection: Session, repository_id: int):
     """
         Delete scan findings for a given repository
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository
     """
     db_connection.query(model.DBscanFinding) \
         .filter(model.scan_finding.DBscanFinding.scan_id == model.scan.DBscan.id_,
                 model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_,
-                model.scan.DBscan.branch_id == model.branch.DBbranch.id_,
-                model.branch.DBbranch.repository_id == model.repository.DBrepository.id_,
-                model.repository.DBrepository.id_ == repository_id) \
+                model.scan.DBscan.repository_id == model.finding.DBfinding.repository_id,
+                model.scan.DBscan.repository_id == repository_id) \
         .delete(synchronize_session=False)
     db_connection.commit()
 
 
 def delete_scan_finding_by_vcs_instance_id(db_connection: Session, vcs_instance_id: int):
     """
         Delete scan findings for a given vcs instance
@@ -93,13 +75,12 @@
         Session of the database connection
     :param vcs_instance_id:
         id of the vcs instance
     """
     db_connection.query(model.DBscanFinding) \
         .filter(model.scan_finding.DBscanFinding.scan_id == model.scan.DBscan.id_,
                 model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_,
-                model.scan.DBscan.branch_id == model.branch.DBbranch.id_,
-                model.branch.DBbranch.repository_id == model.repository.DBrepository.id_,
+                model.scan.DBscan.repository_id == model.repository.DBrepository.id_,
                 model.repository.DBrepository.vcs_instance == model.vcs_instance.DBVcsInstance.id_,
                 model.vcs_instance.DBVcsInstance.id_ == vcs_instance_id) \
         .delete(synchronize_session=False)
     db_connection.commit()
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/vcs_instance.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/crud/vcs_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # Third Party
 from sqlalchemy import func
 from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
 from resc_backend.db import model
-from resc_backend.resc_web_service.crud import branch as branch_crud
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import repository as repository_crud
 from resc_backend.resc_web_service.crud import scan as scan_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.schema import vcs_instance as vcs_instance_schema
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
@@ -143,12 +142,11 @@
     :param delete_related:
         if related records need to be deleted
     """
     if delete_related:
         scan_finding_crud.delete_scan_finding_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
         finding_crud.delete_findings_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
         scan_crud.delete_scans_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
-        branch_crud.delete_branches_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
         repository_crud.delete_repositories_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
     db_vcs_instance = db_connection.query(model.DBVcsInstance).filter_by(id_=vcs_instance_id).first()
     db_connection.delete(db_vcs_instance)
     db_connection.commit()
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/common.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,14 @@
             - rule_tags of type [String] findings in the result will have at least one of the specified tags
               for the rules
 
             - project_name of type String
 
             - repository_names of type [String]
 
-            - branch_name of type String
-
             - scan_ids of type list Integer
 
             - start_date_time of type datetime with the following format: 1970-01-31T00:00:00
 
             - end_date_time of type datetime with the following format: 1970-01-31T00:00:00
 
     - **db_connection**
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/findings.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/findings.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     - **commit_id**: commit hash
     - **commit_message**: Commit message
     - **commit_timestamp**: Commit timestamp
     - **author**: Author name
     - **email**: Email of the author
     - **event_sent_on**: event sent timestamp
     - **rule_name**: rule name
-    - **branch_id**: branch id of the finding
+    - **repository_id**: repository id of the finding
     - **return**: int
           The output will contain the number of successful created findings
       """
     try:
         created_findings = finding_crud.create_findings(db_connection=db_connection, findings=findings)
 
     except KeyError as err:
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/health.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/repositories.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/repositories.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 # Standard Library
-import datetime
 from typing import List, Optional
 
 # Third Party
 from fastapi import APIRouter, Depends, HTTPException, Query, status
 
 # First Party
 from resc_backend.constants import (
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     REPOSITORIES_TAG,
-    RWS_ROUTE_BRANCHES,
     RWS_ROUTE_DISTINCT_PROJECTS,
     RWS_ROUTE_DISTINCT_REPOSITORIES,
     RWS_ROUTE_FINDINGS_METADATA,
-    RWS_ROUTE_REPOSITORIES
+    RWS_ROUTE_LAST_SCAN,
+    RWS_ROUTE_REPOSITORIES,
+    RWS_ROUTE_SCANS
 )
 from resc_backend.db.connection import Session
-from resc_backend.db.model import DBbranch
-from resc_backend.resc_web_service.crud import branch as branch_crud
-from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import repository as repository_crud
 from resc_backend.resc_web_service.crud import scan as scan_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
-from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model404
-from resc_backend.resc_web_service.schema import branch as branch_schema
 from resc_backend.resc_web_service.schema import repository as repository_schema
 from resc_backend.resc_web_service.schema import repository_enriched as repository_enriched_schema
+from resc_backend.resc_web_service.schema import scan as scan_schema
 from resc_backend.resc_web_service.schema.finding_count_model import FindingCountModel
 from resc_backend.resc_web_service.schema.pagination_model import PaginationModel
-from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 router = APIRouter(prefix=f"{RWS_ROUTE_REPOSITORIES}", tags=[REPOSITORIES_TAG])
 
 
 @router.get("",
             response_model=PaginationModel[repository_schema.RepositoryRead],
@@ -181,88 +176,14 @@
     db_repository = repository_crud.get_repository(db_connection, repository_id=repository_id)
     if db_repository is None:
         raise HTTPException(status_code=404, detail="Repository not found")
     repository_crud.delete_repository(db_connection, repository_id=repository_id, delete_related=True)
     return {"ok": True}
 
 
-@router.get("/{repository_id}"f"{RWS_ROUTE_BRANCHES}",
-            response_model=PaginationModel[branch_schema.ViewableBranch],
-            summary="Get branches for a repository",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Retrieve all the branches of a repository, enriched with the recent scan "
-                                     "information"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def get_branches_for_repository(repository_id: int, skip: int = Query(default=0, ge=0),
-                                limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-                                db_connection: Session = Depends(get_db_connection)) \
-        -> PaginationModel[branch_schema.ViewableBranch]:
-    """
-        Retrieve all branches enriched with most recent scan information for a repository
-
-    - **db_connection**: Session of the database connection
-    - **repository_id**: ID of the parent repository object for which branch objects need to be retrieved
-    - **skip**: Integer amount of records to skip to support pagination
-    - **limit**: Integer amount of records to return, to support pagination
-    - **return**: [ViewableBranch]
-        The output will contain a PaginationModel containing the list of ViewableBranch type objects,
-        or an empty list if no branch was found for the given repository_id
-    """
-    branches = branch_crud.get_branches_for_repository(db_connection, skip=skip, limit=limit,
-                                                       repository_id=repository_id)
-    for branch in branches:
-        branch = enrich_branch_with_latest_scan_data(db_connection, branch)
-
-    total_branches = branch_crud.get_branches_count_for_repository(db_connection,
-                                                                   repository_id=repository_id)
-    return PaginationModel[branch_schema.ViewableBranch](data=branches, total=total_branches,
-                                                         limit=limit, skip=skip)
-
-
-def enrich_branch_with_latest_scan_data(db_connection: Session, branch: DBbranch):
-    """
-        Enriches a branch object retrieved from the database with most recent scan information
-    :param db_connection:
-        Session of the database connection
-    :param branch:
-        DBbranch object to enrich with scan information
-    :return: branch
-        DBbranch object enriched with latest scan information as type ViewableBranch
-    """
-
-    branch.last_scan_datetime = datetime.datetime.min
-    branch.last_scan_id = None
-    branch.last_scan_finding_count = 0
-    branch.scan_finding_count = 0
-
-    latest_scan = scan_crud.get_latest_scan_for_branch(db_connection, branch_id=branch.id_)
-    if latest_scan is not None:
-        branch.last_scan_datetime = latest_scan.timestamp
-        branch.last_scan_id = latest_scan.id_
-        branch.last_scan_finding_count = finding_crud.get_total_findings_count(
-            db_connection, FindingsFilter(scan_ids=[latest_scan.id_]))
-
-        scan_ids_latest_to_base = []
-        scans = scan_crud.get_scans(db_connection=db_connection, branch_id=branch.id_, limit=1000000)
-        scans.sort(key=lambda x: x.timestamp, reverse=True)
-        for scan in scans:
-            if scan.timestamp <= latest_scan.timestamp:
-                scan_ids_latest_to_base.append(scan.id_)
-                if scan.scan_type == ScanType.BASE:
-                    break
-
-        branch.scan_finding_count = finding_crud.get_total_findings_count(
-            db_connection, FindingsFilter(scan_ids=scan_ids_latest_to_base))
-
-    return branch
-
-
 @router.get(f"{RWS_ROUTE_DISTINCT_PROJECTS}/",
             response_model=List[str],
             summary="Get all unique project names",
             status_code=status.HTTP_200_OK,
             responses={
                 200: {"description": "Retrieve all the unique project-names"},
                 500: {"description": ERROR_MESSAGE_500},
@@ -416,19 +337,77 @@
         enriched_repository = repository_enriched_schema.RepositoryEnrichedRead(
             id_=repo.id_,
             project_key=repo.project_key,
             repository_id=repo.repository_id,
             repository_name=repo.repository_name,
             repository_url=repo.repository_url,
             vcs_provider=repo.provider_type,
+            last_scan_id=repo.last_scan_id,
+            last_scan_timestamp=repo.last_scan_timestamp,
             true_positive=repo_findings_meta_data[repo.id_]["true_positive"],
             false_positive=repo_findings_meta_data[repo.id_]["false_positive"],
             not_analyzed=repo_findings_meta_data[repo.id_]["not_analyzed"],
             under_review=repo_findings_meta_data[repo.id_]["under_review"],
             clarification_required=repo_findings_meta_data[repo.id_]["clarification_required"],
             total_findings_count=repo_findings_meta_data[repo.id_]["total_findings_count"]
         )
         repository_list.append(enriched_repository)
 
     return PaginationModel[repository_enriched_schema.RepositoryEnrichedRead](data=repository_list,
                                                                               total=total_repositories,
                                                                               limit=limit, skip=skip)
+
+
+@router.get("/{repository_id}"f"{RWS_ROUTE_LAST_SCAN}",
+            response_model=scan_schema.ScanRead,
+            summary="Get latest scan for repository",
+            status_code=status.HTTP_200_OK,
+            responses={
+                200: {"description": "Retrieve the latest scan related to a repository"},
+                500: {"description": ERROR_MESSAGE_500},
+                503: {"description": ERROR_MESSAGE_503}
+            })
+def get_last_scan_for_repository(repository_id: int, db_connection: Session = Depends(get_db_connection)) \
+        -> scan_schema.ScanRead:
+    """
+        Retrieve the latest scan object related to a repository
+
+    - **db_connection**: Session of the database connection
+    - **repository_id**: ID of the parent repository object for which scan objects to be retrieved
+    - **return**: ScanRead
+        The output will contain a ScanRead type object,
+        or empty if no scan was found
+    """
+    last_scan = scan_crud.get_latest_scan_for_repository(db_connection, repository_id=repository_id)
+
+    return last_scan
+
+
+@router.get("/{repository_id}"f"{RWS_ROUTE_SCANS}",
+            summary="Get scans for repository",
+            response_model=PaginationModel[scan_schema.ScanRead],
+            status_code=status.HTTP_200_OK,
+            responses={
+                200: {"description": "Retrieve all the scans related to a repository"},
+                500: {"description": ERROR_MESSAGE_500},
+                503: {"description": ERROR_MESSAGE_503}
+            })
+def get_scans_for_repository(repository_id: int, skip: int = Query(default=0, ge=0),
+                             limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+                             db_connection: Session = Depends(get_db_connection)) \
+        -> PaginationModel[scan_schema.ScanRead]:
+    """
+        Retrieve all scan objects related to a repository paginated
+
+    - **db_connection**: Session of the database connection
+    - **repository_id**: ID of the parent repository object for which scan objects to be retrieved
+    - **skip**: Integer amount of records to skip to support pagination
+    - **limit**: Integer amount of records to return, to support pagination
+    - **return**: [ScanRead]
+        The output will contain a PaginationModel containing the list of ScanRead type objects,
+        or an empty list if no scan was found
+    """
+    scans = scan_crud.get_scans(db_connection, skip=skip, limit=limit, repository_id=repository_id)
+
+    total_scans = scan_crud.get_scans_count(db_connection, repository_id=repository_id)
+
+    return PaginationModel[scan_schema.ScanRead](data=scans, total=total_scans, limit=limit, skip=skip)
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/rules.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/rules.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/scans.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/scans.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,19 +78,19 @@
 
     - **db_connection**: Session of the database connection
     - **scan_type**: scan type, supported values are BASE or INCREMENTAL
     - **last_scanned_commit**: last scanned commit hash
     - **timestamp**: creation timestamp
     - **increment_number**: scan increment number
     - **rule_pack**: rule pack version
-    - **branch_id**: branch id
+    - **repository_id**: repository id
     """
     # Determine the increment number if needed and not supplied
     if scan.scan_type == ScanType.INCREMENTAL and (not scan.increment_number or scan.increment_number <= 0):
-        last_scan = scan_crud.get_latest_scan_for_branch(db_connection, branch_id=scan.branch_id)
+        last_scan = scan_crud.get_latest_scan_for_repository(db_connection, repository_id=scan.repository_id)
         new_increment = last_scan.increment_number + 1
         scan.increment_number = new_increment
 
     try:
         created_scan = scan_crud.create_scan(db_connection=db_connection, scan=scan)
     except IntegrityError as err:
         logger.debug(f"Error creating new scan object: {err}")
@@ -141,15 +141,15 @@
 
     - **db_connection**: Session of the database connection
     - **scan_type**: scan type, supported values are BASE or INCREMENTAL
     - **last_scanned_commit**: last scanned commit
     - **timestamp**: scan timestamp
     - **increment_number**: scan increment number
     - **rule_pack**: rule pack version
-    - **branch_id**: branch id
+    - **repository_id**: repository id
 
     """
     db_scan = scan_crud.get_scan(db_connection, scan_id=scan_id)
     if db_scan is None:
         raise HTTPException(status_code=404, detail="Scan not found")
     return scan_crud.update_scan(db_connection=db_connection, scan_id=scan_id, scan=scan)
 
@@ -170,15 +170,15 @@
     - **db_connection**: Session of the database connection
     - **scan_id**: ID of the scan to delete
     - **return**: The output will contain a success or error message based on the success of the deletion
     """
     db_scan = scan_crud.get_scan(db_connection, scan_id=scan_id)
     if db_scan is None:
         raise HTTPException(status_code=404, detail="Scan not found")
-    scan_crud.delete_scan(db_connection, branch_id=db_scan.branch_id, scan_id=scan_id, delete_related=True)
+    scan_crud.delete_scan(db_connection, repository_id=db_scan.repository_id, scan_id=scan_id, delete_related=True)
     return {"ok": True}
 
 
 @router.post("/{scan_id}"f"{RWS_ROUTE_FINDINGS}",
              response_model=int,
              summary="Create scan findings",
              status_code=status.HTTP_201_CREATED,
@@ -206,15 +206,15 @@
     - **author**: Author name
     - **email**: Email of the author
     - **status**: Status of the finding, Valid values are NOT_ANALYZED, UNDER_REVIEW,
                   CLARIFICATION_REQUIRED, FALSE_POSITIVE, TRUE_POSITIVE
     - **comment**: Comment
     - **event_sent_on**: event sent timestamp
     - **rule_name**: rule name
-    - **branch_id**: branch id of the finding
+    - **repository_id**: repository id of the finding
     - **return**: [FindingRead]
         The output will contain a PaginationModel containing the list of FindingRead type objects,
         or an empty list if no scan was found
     """
 
     created_findings = finding_crud.create_findings(db_connection=db_connection, findings=findings)
     scan_findings = []
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/filters.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 class FindingsFilter:
     vcs_providers: List[VCSProviders] = None
     finding_statuses: List[FindingStatus] = None
     rule_names: List[str] = None
     rule_tags: List[str] = None
     project_name: str = None
     repository_name: str = None
-    branch_name: str = None
     scan_ids: List[int] = None
     start_date_time: datetime = None
     end_date_time: datetime = None
     event_sent: bool = None
     rule_pack_versions: List[str] = None
 
     @validator("end_date_time")
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/exception_handler.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/helpers/exception_handler.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/rule.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/helpers/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/audit.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/detailed_finding.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/detailed_finding.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     rule_name: constr(max_length=200)
     rule_pack: constr(max_length=100)
     project_key: constr(min_length=1, max_length=100)
     repository_name: constr(min_length=1, max_length=100)
     repository_url: HttpUrl
     timestamp: datetime.datetime
     vcs_provider: VCSProviders
-    branch_name: constr(min_length=1, max_length=200)
     last_scanned_commit: constr(min_length=1, max_length=100)
     scan_id: conint(gt=0)
     event_sent_on: Optional[datetime.datetime]
 
 
 class DetailedFinding(DetailedFindingBase):
     pass
@@ -61,28 +60,24 @@
         bitbucket_commit_url = f"{repo_base_url}/projects/{project_key}/repos/" \
                                f"{repository_name}/browse/{file_path}?at={commit_id}"
         commit_url = bitbucket_commit_url
         return commit_url
 
     @staticmethod
     def build_ado_commit_url(repository_url: str,
-                             branch_name: str,
                              file_path: str,
                              commit_id: str) -> str:
-        ado_commit_url = f"{repository_url}/commit/{commit_id}?" \
-                         f"refName=refs/heads/{branch_name}&path=/{file_path}"
+        ado_commit_url = f"{repository_url}/commit/{commit_id}?path=/{file_path}"
         return ado_commit_url
 
     @staticmethod
     def build_github_commit_url(repository_url: str,
-                                branch_name: str,
                                 file_path: str,
                                 commit_id: str) -> str:
-        github_commit_url = f"{repository_url}/commit/{commit_id}?" \
-                            f"refName=refs/heads/{branch_name}&path=/{file_path}"
+        github_commit_url = f"{repository_url}/commit/{commit_id}?path=/{file_path}"
         return github_commit_url
 
     @root_validator
     def build_commit_url(cls, values) -> Dict:
         if values["status"] is None:
             values["status"] = FindingStatus.NOT_ANALYZED
         if values["comment"] is None:
@@ -91,21 +86,19 @@
             values["commit_url"] = cls.build_bitbucket_commit_url(repository_url=values["repository_url"],
                                                                   repository_name=values["repository_name"],
                                                                   project_key=values["project_key"],
                                                                   file_path=values["file_path"],
                                                                   commit_id=values["commit_id"])
         elif values["vcs_provider"] == VCSProviders.AZURE_DEVOPS:
             values["commit_url"] = cls.build_ado_commit_url(repository_url=values["repository_url"],
-                                                            branch_name=values["branch_name"],
                                                             file_path=values["file_path"],
                                                             commit_id=values["commit_id"])
 
         elif values["vcs_provider"] == VCSProviders.GITHUB_PUBLIC:
             values["commit_url"] = cls.build_github_commit_url(repository_url=values["repository_url"],
-                                                               branch_name=values["branch_name"],
                                                                file_path=values["file_path"],
                                                                commit_id=values["commit_id"])
         else:
             raise Exception(f"Unsupported VCSProvider: {values['vcs_provider']}")
         return values
 
     class Config:
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/finding.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 
 
 class FindingPatch(BaseModel):
     event_sent_on: datetime.datetime
 
 
 class FindingCreate(FindingBase):
-    branch_id: conint(gt=0)
+    repository_id: conint(gt=0)
 
     @classmethod
-    def create_from_base_class(cls, base_object: FindingBase, branch_id: int):
-        return cls(**(dict(base_object)), branch_id=branch_id)
+    def create_from_base_class(cls, base_object: FindingBase, repository_id: int):
+        return cls(**(dict(base_object)), repository_id=repository_id)
 
 
 class Finding(FindingBase):
     pass
 
 
 class FindingRead(FindingCreate):
@@ -59,10 +59,10 @@
             commit_id=db_finding.commit_id,
             commit_message=db_finding.commit_message,
             commit_timestamp=db_finding.commit_timestamp,
             author=db_finding.author,
             email=db_finding.email,
             event_sent_on=db_finding.event_sent_on,
             rule_name=db_finding.rule_name,
-            branch_id=db_finding.branch_id,
+            repository_id=db_finding.repository_id,
             scan_ids=scan_ids
         )
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding_count_model.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/finding_count_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Model = TypeVar("Model", bound=BaseModel)
 
 
 class FindingCountModel(GenericModel, Generic[Model]):
     """
         Generic encapsulation class for findings count end points to standardize output of the API
-        example creation, FindingCountModel[BranchRead](data=db_findings, true_positive=true_positive,
+        example creation, FindingCountModel[FindingRead](data=db_findings, true_positive=true_positive,
         false_positive=false_positive, not_analyzed=not_analyzed, under_review=under_review,
         clarification_required=clarification_required, total_findings_count=total_findings_count)
     :param Generic[Model]:
         Type of the object in the data list
     """
     data: Optional[Model]
     true_positive: conint(gt=-1)
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/pagination_model.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/pagination_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_count_model.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/rule_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_pack.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/scan.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/scan.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     last_scanned_commit: constr(min_length=1, max_length=100)
     timestamp: datetime.datetime
     increment_number: conint(gt=-1) = 0
     rule_pack: constr(max_length=100)
 
 
 class ScanCreate(ScanBase):
-    branch_id: conint(gt=0)
+    repository_id: conint(gt=0)
 
     @classmethod
-    def create_from_base_class(cls, base_object: ScanBase, branch_id: int):
-        return cls(**(dict(base_object)), branch_id=branch_id)
+    def create_from_base_class(cls, base_object: ScanBase, repository_id: int):
+        return cls(**(dict(base_object)), repository_id=repository_id)
 
 
 class Scan(ScanBase):
     pass
 
 
 class ScanRead(ScanCreate):
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/vcs_instance.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service/schema/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/branches.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/repositories.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Standard Library
 import logging
 
 # Third Party
 import requests
 
 # First Party
-from resc_backend.constants import RWS_ROUTE_BRANCHES, RWS_ROUTE_LAST_SCAN, RWS_VERSION_PREFIX
-from resc_backend.resc_web_service.schema.branch import BranchCreate
+from resc_backend.constants import RWS_ROUTE_LAST_SCAN, RWS_ROUTE_REPOSITORIES, RWS_VERSION_PREFIX
+from resc_backend.resc_web_service.schema.repository import Repository
 
 logger = logging.getLogger(__name__)
 
 
-def create_branch(url: str, branch: BranchCreate):
-    api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_BRANCHES}"
-    response = requests.post(api_url, data=branch.json(), proxies={"http": "", "https": ""})
+def create_repository(url: str, repository: Repository):
+    api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_REPOSITORIES}"
+    response = requests.post(api_url, data=repository.json(), proxies={"http": "", "https": ""})
     return response
 
 
-def get_last_scan_for_branch(url: str, branch_id: int):
-    api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_BRANCHES}/{branch_id}{RWS_ROUTE_LAST_SCAN}"
+def get_last_scan_for_repository(url: str, repository_id: int):
+    api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_REPOSITORIES}/{repository_id}{RWS_ROUTE_LAST_SCAN}"
     response = requests.get(api_url, proxies={"http": "", "https": ""})
     return response
```

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/findings.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/rule_packs.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/vcs_instances.py` & `resc_backend-1.4.0/src/resc_backend/resc_web_service_interface/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.3.0/src/resc_backend.egg-info/PKG-INFO` & `resc_backend-1.4.0/src/resc_backend.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-backend
-Version: 1.3.0
+Version: 1.4.0
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -18,14 +18,15 @@
     - [Prerequisites](#prerequisites)
     - [Run RESC Web service locally from source](#run-resc-web-service-locally-from-source)
     - [Run RESC Web service locally through Make](#run-resc-web-service-locally-through-make)
     - [Run locally using docker](#run-locally-using-docker)
 3. [Testing](#testing)
     - [Run unit tests, linting and import checks locally](#run-unit-tests-linting-and-import-checks-locally)
     - [Run Newman tests locally](#run-newman-tests-locally)
+    - [Run OWASP ZAP API Security tests locally](#run-owasp-zap-api-security-tests-locally)
 4. [Create a migration for database changes](#create-a-migration-for-database-changes)
     - [Use Alembic to create a new migration script](#use-alembic-to-create-a-new-migration-script)
     - [Use the --autogenerate parameter](#use-the---autogenerate-parameter)
     - [Running migration and rollback](#running-migration-and-rollback)
 5. [Documentation](#documentation)
 
 <!-- ABOUT THE COMPONENT -->
@@ -179,14 +180,28 @@
 ```bash
 cd tests/newman_tests
 ./run_newman_tests.sh -b <resc-backend image:tag> -d <resc-database image:tag>  -n <newman image:tag> 
 
 Example: ./run_newman_tests.sh -b 'rescabnamro/resc-backend:1.0.1' -d 'mcr.microsoft.com/azure-sql-edge:1.0.5' -n 'postman/newman:5.3.1-alpine'
 ```
 
+### Run OWASP ZAP API Security tests locally:
+If you don't provide any argument to the script, then the default image value will be used
+```bash
+cd tests/zap_tests
+./run_run_zap_api_tests.sh
+```
+
+If you can override the images by providing below arguments to the script.
+```bash
+cd tests/zap_tests
+./run_run_zap_api_tests.sh -b <resc-backend image:tag> -d <resc-database image:tag>  -z <zap image:tag>
+
+Example: ./run_newman_tests.sh -b 'rescabnamro/resc-backend:1.0.1' -d 'mcr.microsoft.com/azure-sql-edge:1.0.5' -n 'owasp/zap2docker-weekly'
+```
 
 
 ## Create a migration for database changes
 [(Back to top)](#table-of-contents)
 
 ### Use Alembic to create a new migration script
 <details>
```

### Comparing `resc_backend-1.3.0/src/resc_backend.egg-info/SOURCES.txt` & `resc_backend-1.4.0/src/resc_backend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 src/resc_backend.egg-info/top_level.txt
 src/resc_backend/bin/__init__.py
 src/resc_backend/bin/rabbitmq_bootup.py
 src/resc_backend/db/__init__.py
 src/resc_backend/db/connection.py
 src/resc_backend/db/model/__init__.py
 src/resc_backend/db/model/audit.py
-src/resc_backend/db/model/branch.py
 src/resc_backend/db/model/finding.py
 src/resc_backend/db/model/repository.py
 src/resc_backend/db/model/rule.py
 src/resc_backend/db/model/rule_allow_list.py
 src/resc_backend/db/model/rule_pack.py
 src/resc_backend/db/model/rule_tag.py
 src/resc_backend/db/model/scan.py
@@ -36,26 +35,24 @@
 src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
 src/resc_backend/resc_web_service/__init__.py
 src/resc_backend/resc_web_service/api.py
 src/resc_backend/resc_web_service/dependencies.py
 src/resc_backend/resc_web_service/filters.py
 src/resc_backend/resc_web_service/crud/__init__.py
 src/resc_backend/resc_web_service/crud/audit.py
-src/resc_backend/resc_web_service/crud/branch.py
 src/resc_backend/resc_web_service/crud/detailed_finding.py
 src/resc_backend/resc_web_service/crud/finding.py
 src/resc_backend/resc_web_service/crud/repository.py
 src/resc_backend/resc_web_service/crud/rule.py
 src/resc_backend/resc_web_service/crud/rule_pack.py
 src/resc_backend/resc_web_service/crud/rule_tag.py
 src/resc_backend/resc_web_service/crud/scan.py
 src/resc_backend/resc_web_service/crud/scan_finding.py
 src/resc_backend/resc_web_service/crud/vcs_instance.py
 src/resc_backend/resc_web_service/endpoints/__init__.py
-src/resc_backend/resc_web_service/endpoints/branches.py
 src/resc_backend/resc_web_service/endpoints/common.py
 src/resc_backend/resc_web_service/endpoints/detailed_findings.py
 src/resc_backend/resc_web_service/endpoints/findings.py
 src/resc_backend/resc_web_service/endpoints/health.py
 src/resc_backend/resc_web_service/endpoints/metrics.py
 src/resc_backend/resc_web_service/endpoints/repositories.py
 src/resc_backend/resc_web_service/endpoints/rule_packs.py
@@ -64,34 +61,35 @@
 src/resc_backend/resc_web_service/endpoints/vcs_instances.py
 src/resc_backend/resc_web_service/helpers/__init__.py
 src/resc_backend/resc_web_service/helpers/exception_handler.py
 src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
 src/resc_backend/resc_web_service/helpers/rule.py
 src/resc_backend/resc_web_service/schema/__init__.py
 src/resc_backend/resc_web_service/schema/audit.py
-src/resc_backend/resc_web_service/schema/branch.py
+src/resc_backend/resc_web_service/schema/audit_count_over_time.py
 src/resc_backend/resc_web_service/schema/date_count_model.py
 src/resc_backend/resc_web_service/schema/date_filter.py
 src/resc_backend/resc_web_service/schema/detailed_finding.py
 src/resc_backend/resc_web_service/schema/finding.py
 src/resc_backend/resc_web_service/schema/finding_count_model.py
 src/resc_backend/resc_web_service/schema/finding_count_over_time.py
 src/resc_backend/resc_web_service/schema/finding_status.py
 src/resc_backend/resc_web_service/schema/pagination_model.py
+src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
 src/resc_backend/resc_web_service/schema/repository.py
 src/resc_backend/resc_web_service/schema/repository_enriched.py
 src/resc_backend/resc_web_service/schema/rule.py
 src/resc_backend/resc_web_service/schema/rule_allow_list.py
 src/resc_backend/resc_web_service/schema/rule_count_model.py
 src/resc_backend/resc_web_service/schema/rule_pack.py
 src/resc_backend/resc_web_service/schema/scan.py
 src/resc_backend/resc_web_service/schema/scan_type.py
 src/resc_backend/resc_web_service/schema/status_count.py
+src/resc_backend/resc_web_service/schema/time_period.py
 src/resc_backend/resc_web_service/schema/vcs_instance.py
 src/resc_backend/resc_web_service/schema/vcs_provider.py
 src/resc_backend/resc_web_service_interface/__init__.py
-src/resc_backend/resc_web_service_interface/branches.py
 src/resc_backend/resc_web_service_interface/findings.py
 src/resc_backend/resc_web_service_interface/repositories.py
 src/resc_backend/resc_web_service_interface/rule_packs.py
 src/resc_backend/resc_web_service_interface/scans.py
 src/resc_backend/resc_web_service_interface/vcs_instances.py
```

