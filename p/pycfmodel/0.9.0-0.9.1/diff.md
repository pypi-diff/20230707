# Comparing `tmp/pycfmodel-0.9.0.tar.gz` & `tmp/pycfmodel-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycfmodel-0.9.0.tar", last modified: Wed May  5 09:00:23 2021, max compression
+gzip compressed data, was "dist/pycfmodel-0.9.1.tar", last modified: Thu May  6 11:53:01 2021, max compression
```

## Comparing `pycfmodel-0.9.0.tar` & `pycfmodel-0.9.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     5062 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3752 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/pycfmodel/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/action_expander.py
--rw-r--r--   0 runner    (1001) docker     (121)   368012 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/cloudformation_actions.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/pycfmodel/model/
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5500 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/cf_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/pycfmodel/model/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/ec2_vpc_endpoint_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/generic_resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/iam_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/iam_managed_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/iam_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/iam_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/iam_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/kms_key.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/pycfmodel/model/resources/properties/
--rw-r--r--   0 runner    (1001) docker     (121)      585 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/properties/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4240 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/properties/policy_document.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/properties/property.py
--rw-r--r--   0 runner    (1001) docker     (121)     2593 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/properties/security_group_egress_prop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2858 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/properties/security_group_ingress_prop.py
--rw-r--r--   0 runner    (1001) docker     (121)     6568 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/properties/statement.py
--rw-r--r--   0 runner    (1001) docker     (121)    21904 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/properties/statement_condition.py
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/s3_bucket_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/security_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/security_group_egress.py
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/security_group_ingress.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/sns_topic_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/sqs_queue_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/resources/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7773 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pycfmodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/pycfmodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5062 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/pycfmodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/pycfmodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/pycfmodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/pycfmodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/pycfmodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      800 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/scripts/generate_cloudformation_actions_file.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 09:00:23.000000 pycfmodel-0.9.0/tests/resources/properties/
--rw-r--r--   0 runner    (1001) docker     (121)     6984 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/properties/test_policy_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     7112 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/properties/test_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)    26685 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/properties/test_statement_condition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2557 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_ec2_vpc_endpoint_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_iam_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_iam_managed_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_iam_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_iam_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_iam_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_kms_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_s3_bucket_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_security_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_security_group_egress.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_security_group_ingress.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_sns_topic_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-05-05 09:00:19.000000 pycfmodel-0.9.0/tests/resources/test_sqs_queue_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     5062 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3752 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/pycfmodel/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/action_expander.py
+-rw-r--r--   0 runner    (1001) docker     (121)   368144 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/cloudformation_actions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/pycfmodel/model/
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5500 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/cf_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1861 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/pycfmodel/model/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     2427 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/ec2_vpc_endpoint_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/generic_resource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/iam_managed_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/iam_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2289 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2611 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2086 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/kms_key.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/pycfmodel/model/resources/properties/
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/properties/policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4240 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/properties/policy_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/properties/property.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2593 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/properties/security_group_egress_prop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2858 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/properties/security_group_ingress_prop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6568 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/properties/statement.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21727 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/properties/statement_condition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1711 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1449 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/s3_bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1897 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1817 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/security_group_egress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2015 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/security_group_ingress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/sns_topic_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1439 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/sqs_queue_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/resources/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7773 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pycfmodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/pycfmodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5062 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/pycfmodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2285 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/pycfmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/pycfmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/pycfmodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/pycfmodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/scripts/generate_cloudformation_actions_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 11:53:01.000000 pycfmodel-0.9.1/tests/resources/properties/
+-rw-r--r--   0 runner    (1001) docker     (121)     6984 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/properties/test_policy_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7112 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/properties/test_statement.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26862 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/properties/test_statement_condition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2557 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_ec2_vpc_endpoint_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_iam_managed_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_iam_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1545 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_kms_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_s3_bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1849 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_security_group_egress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1901 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_security_group_ingress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_sns_topic_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-05-06 11:52:56.000000 pycfmodel-0.9.1/tests/resources/test_sqs_queue_policy.py
```

### Comparing `pycfmodel-0.9.0/PKG-INFO` & `pycfmodel-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycfmodel
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python model for CloudFormation scripts
 Home-page: https://github.com/Skyscanner/pycfmodel
 Author: Skyscanner Product Security
 Author-email: security@skyscanner.net
 License: UNKNOWN
 Description: # pycfmodel
```

### Comparing `pycfmodel-0.9.0/README.md` & `pycfmodel-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/action_expander.py` & `pycfmodel-0.9.1/pycfmodel/action_expander.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/cloudformation_actions.py` & `pycfmodel-0.9.1/pycfmodel/cloudformation_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3434,14 +3434,15 @@
     "ecs:DescribeClusters",
     "ecs:DescribeContainerInstances",
     "ecs:DescribeServices",
     "ecs:DescribeTaskDefinition",
     "ecs:DescribeTaskSets",
     "ecs:DescribeTasks",
     "ecs:DiscoverPollEndpoint",
+    "ecs:ExecuteCommand",
     "ecs:ListAccountSettings",
     "ecs:ListAttributes",
     "ecs:ListClusters",
     "ecs:ListContainerInstances",
     "ecs:ListServices",
     "ecs:ListTagsForResource",
     "ecs:ListTaskDefinitionFamilies",
@@ -3459,14 +3460,16 @@
     "ecs:StartTelemetrySession",
     "ecs:StopTask",
     "ecs:SubmitAttachmentStateChanges",
     "ecs:SubmitContainerStateChange",
     "ecs:SubmitTaskStateChange",
     "ecs:TagResource",
     "ecs:UntagResource",
+    "ecs:UpdateCapacityProvider",
+    "ecs:UpdateCluster",
     "ecs:UpdateClusterSettings",
     "ecs:UpdateContainerAgent",
     "ecs:UpdateContainerInstancesState",
     "ecs:UpdateService",
     "ecs:UpdateServicePrimaryTaskSet",
     "ecs:UpdateTaskSet",
     "eks:AccessKubernetesApi",
@@ -6854,14 +6857,15 @@
     "opsworks-cm:DeleteServer",
     "opsworks-cm:DescribeAccountAttributes",
     "opsworks-cm:DescribeBackups",
     "opsworks-cm:DescribeEvents",
     "opsworks-cm:DescribeNodeAssociationStatus",
     "opsworks-cm:DescribeServers",
     "opsworks-cm:DisassociateNode",
+    "opsworks-cm:ExportServerEngineAttribute",
     "opsworks-cm:ListTagsForResource",
     "opsworks-cm:RestoreServer",
     "opsworks-cm:StartMaintenance",
     "opsworks-cm:TagResource",
     "opsworks-cm:UntagResource",
     "opsworks-cm:UpdateServer",
     "opsworks-cm:UpdateServerEngineAttributes",
```

### Comparing `pycfmodel-0.9.0/pycfmodel/model/base.py` & `pycfmodel-0.9.1/pycfmodel/model/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pycfmodel.utils import is_resolvable_dict
 
 
 class CustomModel(BaseModel):
     class Config(BaseModel.Config):
         extra = Extra.forbid
+        underscore_attrs_are_private = True
 
     def dict(self, *args, exclude_unset=True, **kwargs):
         return super().dict(*args, **kwargs, exclude_unset=exclude_unset)
 
 
 class FunctionDict(BaseModel):
     # Inheriting directly from base model as we want to allow extra fields
```

### Comparing `pycfmodel-0.9.0/pycfmodel/model/cf_model.py` & `pycfmodel-0.9.1/pycfmodel/model/cf_model.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/parameter.py` & `pycfmodel-0.9.1/pycfmodel/model/parameter.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/ec2_vpc_endpoint_policy.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/ec2_vpc_endpoint_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/generic_resource.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/generic_resource.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/iam_group.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/iam_group.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/iam_managed_policy.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/iam_managed_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/iam_policy.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/iam_role.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/iam_role.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/iam_user.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/iam_user.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/kms_key.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/kms_key.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/properties/policy.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/properties/policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/properties/policy_document.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/properties/policy_document.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/properties/security_group_egress_prop.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/properties/security_group_egress_prop.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/properties/security_group_ingress_prop.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/properties/security_group_ingress_prop.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/properties/statement.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/properties/statement.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/properties/statement_condition.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/properties/statement_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import binascii
 import logging
 from base64 import b64decode
 from typing import Any, Callable, Dict, Optional, Tuple, Union
 from unicodedata import normalize
 
-from pydantic import BaseModel, root_validator, validator
+from pydantic import root_validator, validator
 
-from pycfmodel.model.base import FunctionDict
+from pycfmodel.model.base import CustomModel, FunctionDict
 from pycfmodel.model.types import (
     ResolvableArnOrList,
     ResolvableBool,
     ResolvableBoolOrList,
     ResolvableBytesOrList,
     ResolvableDatetimeOrList,
     ResolvableIntOrList,
@@ -110,15 +110,15 @@
                 group_of_nodes.append(lambda kwargs: any(node(kwargs) for node in nodes))
             else:
                 group_of_nodes.append(build_evaluator(new_function, arg_a, arg_b))
 
     return lambda kwargs: all(group(kwargs) for group in group_of_nodes)
 
 
-class StatementCondition(BaseModel):
+class StatementCondition(CustomModel):
     """
     Contains the condition to be matched to apply the statement that belongs to.
 
     | Type                       | Operators                 | ...IfExists | ForAllValues... | ForAnyValue... |
     | -------------------------- | ------------------------- | ----------- | --------------- | -------------- |
     | String                     | StringEquals              | Yes         | Yes             | Yes            |
     | String                     | StringNotEquals           | Yes         | Yes             | Yes            |
@@ -314,15 +314,15 @@
     ForAnyValueStringEqualsIfExists: Optional[Dict[str, ResolvableStrOrList]]
     ForAnyValueStringNotEqualsIfExists: Optional[Dict[str, ResolvableStrOrList]]
     ForAnyValueStringEqualsIgnoreCaseIfExists: Optional[Dict[str, ResolvableStrOrList]]
     ForAnyValueStringNotEqualsIgnoreCaseIfExists: Optional[Dict[str, ResolvableStrOrList]]
     ForAnyValueStringLikeIfExists: Optional[Dict[str, ResolvableStrOrList]]
     ForAnyValueStringNotLikeIfExists: Optional[Dict[str, ResolvableStrOrList]]
 
-    eval: Optional[Callable]
+    _eval: Optional[Callable] = None
 
     @root_validator(pre=True)
     def remove_colon(cls, values):
         return {key.replace(":", ""): value for key, value in values.items()}
 
     @validator(
         "BinaryEquals",
@@ -337,27 +337,25 @@
     def validate_binary(cls, value: Any) -> bytearray:
         try:
             value = b64decode(value)
         except binascii.Error:
             raise ValueError("Binary value not valid")
         return value
 
-    @root_validator()
+    def eval(self, values):
+        if self._eval is None:
+            self._eval = self.build_eval(self.dict())
+        return self._eval(values)
+
+    @classmethod
     def build_eval(cls, values: Dict) -> Dict:
-        try:
-            conditions_lambdas = [
-                build_root_evaluator(function=key, arguments=value)
-                for key, value in values.items()
-                if value is not None
-            ]
-            values["eval"] = lambda kwargs: all(condition(kwargs) for condition in conditions_lambdas)
-        except StatementConditionBuildEvaluatorError:
-            values["eval"] = lambda kwargs: (_ for _ in ()).throw(StatementConditionBuildEvaluatorError)
-            logger.error("Resolvable function found. Try resolving the model.")
-        return values
+        conditions_lambdas = [
+            build_root_evaluator(function=key, arguments=value) for key, value in values.items() if value is not None
+        ]
+        return lambda kwargs: all(condition(kwargs) for condition in conditions_lambdas)
 
     def __call__(self, kwargs) -> Optional[bool]:
         try:
             return self.eval(kwargs)
         except Exception:
             logger.exception("Error raised while evaluating condition")
             return None
```

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/resource.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/resource.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/s3_bucket_policy.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/s3_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/security_group.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/security_group.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/security_group_egress.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/security_group_egress.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/security_group_ingress.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/security_group_ingress.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/sns_topic_policy.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/sns_topic_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/sqs_queue_policy.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/sqs_queue_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/resources/types.py` & `pycfmodel-0.9.1/pycfmodel/model/resources/types.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/model/types.py` & `pycfmodel-0.9.1/pycfmodel/model/types.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/resolver.py` & `pycfmodel-0.9.1/pycfmodel/resolver.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel/utils.py` & `pycfmodel-0.9.1/pycfmodel/utils.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/pycfmodel.egg-info/PKG-INFO` & `pycfmodel-0.9.1/pycfmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycfmodel
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python model for CloudFormation scripts
 Home-page: https://github.com/Skyscanner/pycfmodel
 Author: Skyscanner Product Security
 Author-email: security@skyscanner.net
 License: UNKNOWN
 Description: # pycfmodel
```

### Comparing `pycfmodel-0.9.0/pycfmodel.egg-info/SOURCES.txt` & `pycfmodel-0.9.1/pycfmodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/scripts/generate_cloudformation_actions_file.py` & `pycfmodel-0.9.1/scripts/generate_cloudformation_actions_file.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/setup.py` & `pycfmodel-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "pytest-cov>=2.10.1",
 ]
 
 docs_requires = ["AutoMacDoc==0.3", "mkdocs-material==4.6.3", "mkdocs==1.1", "mkdocstrings==0.10.0"]
 
 setup(
     name="pycfmodel",
-    version="0.9.0",
+    version="0.9.1",
     description="A python model for CloudFormation scripts",
     author="Skyscanner Product Security",
     author_email="security@skyscanner.net",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Skyscanner/pycfmodel",
     packages=find_namespace_packages(exclude=("tests", "docs")),
```

### Comparing `pycfmodel-0.9.0/tests/resources/properties/test_policy_document.py` & `pycfmodel-0.9.1/tests/resources/properties/test_policy_document.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/properties/test_statement.py` & `pycfmodel-0.9.1/tests/resources/properties/test_statement.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/properties/test_statement_condition.py` & `pycfmodel-0.9.1/tests/resources/properties/test_statement_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,21 +72,28 @@
     assert implemented_operators == sorted(all_operators)
 
 
 def test_statement_condition_remove_colon():
     assert StatementCondition.parse_obj(
         {
             "ForAllValues:ArnEqualsIfExists": {"patata_1": "test_1"},
-            "ForAnyValue:ARNEquals": {"patata_2": ["test_2", "test_3"]},
+            "ForAnyValue:ArnEquals": {"patata_2": ["test_2", "test_3"]},
         }
     ) == StatementCondition(
-        ForAllValuesArnEqualsIfExists={"patata_1": "test_1"}, ForAnyValueARNEquals={"patata_2": ["test_2", "test_3"]}
+        ForAllValuesArnEqualsIfExists={"patata_1": "test_1"}, ForAnyValueArnEquals={"patata_2": ["test_2", "test_3"]}
     )
 
 
+def test_eval_is_built_only_if_called():
+    condition = StatementCondition()
+    assert condition._eval is None
+    condition.eval({})
+    assert condition._eval is not None
+
+
 @pytest.mark.parametrize(
     "function, arg_a, arg_b, params, expected_output",
     [
         ("Bool", "patata", True, {"patata": True}, True),
         ("Bool", "patata", True, {"patata": False}, False),
         ("Bool", "patata", False, {"patata": True}, False),
         ("Bool", "patata", False, {"patata": False}, True),
```

### Comparing `pycfmodel-0.9.0/tests/resources/test_ec2_vpc_endpoint_policy.py` & `pycfmodel-0.9.1/tests/resources/test_ec2_vpc_endpoint_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_iam_group.py` & `pycfmodel-0.9.1/tests/resources/test_iam_group.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_iam_managed_policy.py` & `pycfmodel-0.9.1/tests/resources/test_iam_managed_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_iam_policy.py` & `pycfmodel-0.9.1/tests/resources/test_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_iam_role.py` & `pycfmodel-0.9.1/tests/resources/test_iam_role.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_iam_user.py` & `pycfmodel-0.9.1/tests/resources/test_iam_user.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_kms_key.py` & `pycfmodel-0.9.1/tests/resources/test_kms_key.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_s3_bucket_policy.py` & `pycfmodel-0.9.1/tests/resources/test_s3_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_security_group.py` & `pycfmodel-0.9.1/tests/resources/test_security_group.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_security_group_egress.py` & `pycfmodel-0.9.1/tests/resources/test_security_group_egress.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_security_group_ingress.py` & `pycfmodel-0.9.1/tests/resources/test_security_group_ingress.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_sns_topic_policy.py` & `pycfmodel-0.9.1/tests/resources/test_sns_topic_policy.py`

 * *Files identical despite different names*

### Comparing `pycfmodel-0.9.0/tests/resources/test_sqs_queue_policy.py` & `pycfmodel-0.9.1/tests/resources/test_sqs_queue_policy.py`

 * *Files identical despite different names*

