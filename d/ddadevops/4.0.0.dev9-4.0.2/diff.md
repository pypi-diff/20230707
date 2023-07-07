# Comparing `tmp/ddadevops-4.0.0.dev9.tar.gz` & `tmp/ddadevops-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddadevops-4.0.0.dev9.tar", last modified: Fri Mar 17 14:59:47 2023, max compression
+gzip compressed data, was "ddadevops-4.0.2.tar", last modified: Fri Jul  7 06:51:22 2023, max compression
```

## Comparing `ddadevops-4.0.0.dev9.tar` & `ddadevops-4.0.2.tar`

### file list

```diff
@@ -1,63 +1,71 @@
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.018865 ddadevops-4.0.0.dev9/
--rw-rw-r--   0 jem       (1000) jem       (1000)      137 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/MANIFEST.in
--rw-rw-r--   0 jem       (1000) jem       (1000)     7958 2023-03-17 14:59:47.018865 ddadevops-4.0.0.dev9/PKG-INFO
--rw-rw-r--   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/__init__.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.014865 ddadevops-4.0.0.dev9/ddadevops/
--rw-rw-r--   0 jem       (1000) jem       (1000)    11357 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/LICENSE
--rw-rw-r--   0 jem       (1000) jem       (1000)     1501 2023-03-14 14:07:46.000000 ddadevops-4.0.0.dev9/ddadevops/__init__.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2070 2023-03-16 12:54:27.000000 ddadevops-4.0.0.dev9/ddadevops/application.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1962 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/aws_backend_properties_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3815 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/aws_mfa_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     5988 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/aws_rds_pg_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2648 2023-03-14 14:05:21.000000 ddadevops-4.0.0.dev9/ddadevops/c4k_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)      468 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/credential.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1922 2023-03-16 13:01:31.000000 ddadevops-4.0.0.dev9/ddadevops/devops_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2710 2023-03-17 14:59:22.000000 ddadevops-4.0.0.dev9/ddadevops/devops_docker_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     9996 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/devops_terraform_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2885 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/digitalocean_backend_properties_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3489 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/digitalocean_terraform_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     4283 2023-03-14 17:32:30.000000 ddadevops-4.0.0.dev9/ddadevops/domain.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1265 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/exoscale_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)      981 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/hetzner_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3494 2023-03-17 14:55:32.000000 ddadevops-4.0.0.dev9/ddadevops/infrastructure.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     4712 2023-03-03 18:37:44.000000 ddadevops-4.0.0.dev9/ddadevops/provs_k3s_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)      475 2023-03-17 12:15:02.000000 ddadevops-4.0.0.dev9/ddadevops/python_util.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.014865 ddadevops-4.0.0.dev9/ddadevops/release_mixin/
--rw-rw-r--   0 jem       (1000) jem       (1000)        0 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/__init__.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1175 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2724 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/domain.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2100 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/infrastructure.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     8136 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/infrastructure_api.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1808 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/release_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1391 2023-03-11 08:22:26.000000 ddadevops-4.0.0.dev9/ddadevops/release_mixin/services.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.010865 ddadevops-4.0.0.dev9/ddadevops/src/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.010865 ddadevops-4.0.0.dev9/ddadevops/src/main/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.010865 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.010865 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/docker/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.010865 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/docker/image/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.014865 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/docker/image/resources/
--rwxrwxr-x   0 jem       (1000) jem       (1000)      628 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/docker/image/resources/install_functions.sh
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.018865 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/
--rw-rw-r--   0 jem       (1000) jem       (1000)      111 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/aws_backend_properties_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       59 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/aws_backend_with_properties.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       41 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/aws_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      109 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/do_backend_properties_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      191 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/do_backend_with_properties.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       99 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/do_mixin_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      145 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/do_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       67 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/exoscale_mixin_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       97 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/exoscale_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       31 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/hetzner_mixin_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       91 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/hetzner_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      483 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/provider_registry.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       40 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/terraform_build_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       46 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops/src/main/resources/terraform/versions.tf
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-03-17 14:59:47.014865 ddadevops-4.0.0.dev9/ddadevops.egg-info/
--rw-rw-r--   0 jem       (1000) jem       (1000)     7958 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/PKG-INFO
--rw-rw-r--   0 jem       (1000) jem       (1000)     1990 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/SOURCES.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/dependency_links.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/namespace_packages.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)       11 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/top_level.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/ddadevops.egg-info/zip-safe
--rw-rw-r--   0 jem       (1000) jem       (1000)       38 2023-03-17 14:59:47.018865 ddadevops-4.0.0.dev9/setup.cfg
--rwxr-xr-x   0 jem       (1000) jem       (1000)     9507 2023-03-17 14:59:46.000000 ddadevops-4.0.0.dev9/setup.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.471142 ddadevops-4.0.2/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      137 2023-07-07 06:51:21.000000 ddadevops-4.0.2/MANIFEST.in
+-rw-rw-r--   0 jem       (1000) jem       (1000)     6741 2023-07-07 06:51:22.467141 ddadevops-4.0.2/PKG-INFO
+-rw-rw-r--   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:21.000000 ddadevops-4.0.2/__init__.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.463138 ddadevops-4.0.2/ddadevops/
+-rw-rw-r--   0 jem       (1000) jem       (1000)    11357 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/LICENSE
+-rw-rw-r--   0 jem       (1000) jem       (1000)      640 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/__init__.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.463138 ddadevops-4.0.2/ddadevops/application/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      150 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/application/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2463 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/application/image_build_service.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2525 2023-06-28 06:35:08.000000 ddadevops-4.0.2/ddadevops/application/release_mixin_services.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     9245 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/application/terraform_service.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3953 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/aws_mfa_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1540 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/c4k_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)      504 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/credential.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1018 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/devops_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1358 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/devops_image_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2284 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/devops_terraform_build.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.463138 ddadevops-4.0.2/ddadevops/domain/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      647 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/domain/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4796 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/domain/build_file.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2982 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/domain/c4k.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3284 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/domain/common.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1916 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/domain/credentials.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1870 2023-06-27 17:01:05.000000 ddadevops-4.0.2/ddadevops/domain/devops_factory.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1753 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/domain/image.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4531 2023-06-27 17:01:05.000000 ddadevops-4.0.2/ddadevops/domain/init_service.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3687 2023-07-06 16:08:05.000000 ddadevops-4.0.2/ddadevops/domain/provider_aws.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3891 2023-07-06 16:08:05.000000 ddadevops-4.0.2/ddadevops/domain/provider_digitalocean.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)      907 2023-07-06 16:08:05.000000 ddadevops-4.0.2/ddadevops/domain/provider_hetzner.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3422 2023-06-13 11:42:08.000000 ddadevops-4.0.2/ddadevops/domain/provs_k3s.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2339 2023-07-07 06:44:48.000000 ddadevops-4.0.2/ddadevops/domain/release.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4101 2023-06-16 09:16:24.000000 ddadevops-4.0.2/ddadevops/domain/terraform.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3489 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/domain/version.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.467141 ddadevops-4.0.2/ddadevops/infrastructure/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      226 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/infrastructure/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     6645 2023-06-28 06:16:44.000000 ddadevops-4.0.2/ddadevops/infrastructure/infrastructure.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1097 2023-06-02 15:15:05.000000 ddadevops-4.0.2/ddadevops/infrastructure/repository.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1332 2023-06-13 11:36:37.000000 ddadevops-4.0.2/ddadevops/provs_k3s_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1177 2023-06-28 06:49:15.000000 ddadevops-4.0.2/ddadevops/release_mixin.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.459136 ddadevops-4.0.2/ddadevops/src/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.459136 ddadevops-4.0.2/ddadevops/src/main/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.459136 ddadevops-4.0.2/ddadevops/src/main/resources/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.459136 ddadevops-4.0.2/ddadevops/src/main/resources/docker/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.459136 ddadevops-4.0.2/ddadevops/src/main/resources/docker/image/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.467141 ddadevops-4.0.2/ddadevops/src/main/resources/docker/image/resources/
+-rwxrwxr-x   0 jem       (1000) jem       (1000)      628 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/docker/image/resources/install_functions.sh
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.467141 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/
+-rw-rw-r--   0 jem       (1000) jem       (1000)       59 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/aws_backend.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       90 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/aws_backend_wkms_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       65 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/aws_backend_wokms_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      113 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/aws_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       83 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/aws_provider_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      191 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/do_backend.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      109 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/do_backend_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      145 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/do_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       99 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/do_provider_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       91 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/hetzner_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       31 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/hetzner_provider_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      392 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/provider_registry.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       40 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/terraform_build_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       46 2023-07-07 06:51:21.000000 ddadevops-4.0.2/ddadevops/src/main/resources/terraform/versions.tf
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-07 06:51:22.463138 ddadevops-4.0.2/ddadevops.egg-info/
+-rw-rw-r--   0 jem       (1000) jem       (1000)     6741 2023-07-07 06:51:22.000000 ddadevops-4.0.2/ddadevops.egg-info/PKG-INFO
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2144 2023-07-07 06:51:22.000000 ddadevops-4.0.2/ddadevops.egg-info/SOURCES.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-07 06:51:22.000000 ddadevops-4.0.2/ddadevops.egg-info/dependency_links.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-07 06:51:22.000000 ddadevops-4.0.2/ddadevops.egg-info/namespace_packages.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)       11 2023-07-07 06:51:22.000000 ddadevops-4.0.2/ddadevops.egg-info/top_level.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-07 06:51:22.000000 ddadevops-4.0.2/ddadevops.egg-info/zip-safe
+-rw-rw-r--   0 jem       (1000) jem       (1000)       38 2023-07-07 06:51:22.471142 ddadevops-4.0.2/setup.cfg
+-rwxr-xr-x   0 jem       (1000) jem       (1000)     8273 2023-07-07 06:51:21.000000 ddadevops-4.0.2/setup.py
```

### Comparing `ddadevops-4.0.0.dev9/ddadevops/LICENSE` & `ddadevops-4.0.2/ddadevops/LICENSE`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev9/ddadevops/aws_mfa_mixin.py` & `ddadevops-4.0.2/ddadevops/aws_mfa_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from boto3 import Session
-from .python_util import execute
-from .aws_backend_properties_mixin import AwsBackendPropertiesMixin
-
-
-def add_aws_mfa_mixin_config(config, account_id, region,
-                             mfa_role='developer', mfa_account_prefix='',
-                             mfa_login_account_suffix='main'):
-    config.update({'AwsMfaMixin':
-                   {'account_id': account_id,
-                    'region': region,
-                    'mfa_role': mfa_role,
-                    'mfa_account_prefix': mfa_account_prefix,
-                    'mfa_login_account_suffix': mfa_login_account_suffix}})
-    return config
-
-
-class AwsMfaMixin(AwsBackendPropertiesMixin):
-
-    def __init__(self, project, config):
-        super().__init__(project, config)
-        project.build_depends_on('boto3')
-        project.build_depends_on('mfa')
-        aws_mfa_mixin_config = config['AwsMfaMixin']
-        self.account_id = aws_mfa_mixin_config['account_id']
-        self.region = aws_mfa_mixin_config['region']
-        self.mfa_role = aws_mfa_mixin_config['mfa_role']
-        self.mfa_account_prefix = aws_mfa_mixin_config['mfa_account_prefix']
-        self.mfa_login_account_suffix = aws_mfa_mixin_config['mfa_login_account_suffix']
-
-    def project_vars(self):
-        ret = super().project_vars()
-        ret.update({'account_name': self.account_name,
-                    'account_id': self.account_id,
-                    'region': self.region,
-                    'mfa_role': self.mfa_role,
-                    'mfa_account_prefix': self.mfa_account_prefix,
-                    'mfa_login_account_suffix': self.mfa_login_account_suffix})
-        return ret
-
-    def get_username_from_account(self, p_account_name):
-        login_id = execute(r'cat ~/.aws/accounts | grep -A 2 "\[' + p_account_name +
-                           r'\]"  | grep username | awk -F= \'{print $2}\'', shell=True)
-        return login_id
-
-    def get_account_id_from_account(self, p_account_name):
-        account_id = execute(r'cat ~/.aws/accounts | grep -A 2 "\[' + p_account_name +
-                             r'\]"  | grep account | awk -F= \'{print $2}\'', shell=True)
-        return account_id
-
-    def get_mfa(self, mfa_path='aws'):
-        mfa_token = execute('mfa otp ' + mfa_path, shell=True)
-        return mfa_token
-
-    def write_aws_config(self, to_profile, key, secret):
-        execute('aws configure --profile ' + to_profile +
-                ' set ' + key + ' ' + secret, shell=True)
-
-    def get_mfa_session(self):
-        from_account_name = self.mfa_account_prefix + self.mfa_login_account_suffix
-        from_account_id = self.get_account_id_from_account(from_account_name)
-        to_account_name = self.mfa_account_prefix + self.account_name
-        to_account_id = self.get_account_id_from_account(to_account_name)
-        login_id = self.get_username_from_account(from_account_name)
-        mfa_token = self.get_mfa()
-        ses = Session(profile_name=from_account_name)
-        sts_client = ses.client('sts')
-        response = sts_client.assume_role(
-            RoleArn='arn:aws:iam::' + to_account_id + ':role/' + self.mfa_role,
-            RoleSessionName=to_account_id + '-' + self.account_name + '-' + self.mfa_role,
-            SerialNumber='arn:aws:iam::' + from_account_id + ':mfa/' + login_id,
-            TokenCode=mfa_token
-        )
-
-        self.write_aws_config(to_account_name, 'aws_access_key_id',
-                              response['Credentials']['AccessKeyId'])
-        self.write_aws_config(to_account_name, 'aws_secret_access_key',
-                              response['Credentials']['SecretAccessKey'])
-        self.write_aws_config(to_account_name, 'aws_session_token',
-                              response['Credentials']['SessionToken'])
-        print('got token')
+# from boto3 import Session
+# from .python_util import execute
+# from .aws_backend_properties_mixin import AwsBackendPropertiesMixin
+
+
+# def add_aws_mfa_mixin_config(config, account_id, region,
+#                              mfa_role='developer', mfa_account_prefix='',
+#                              mfa_login_account_suffix='main'):
+#     config.update({'AwsMfaMixin':
+#                    {'account_id': account_id,
+#                     'region': region,
+#                     'mfa_role': mfa_role,
+#                     'mfa_account_prefix': mfa_account_prefix,
+#                     'mfa_login_account_suffix': mfa_login_account_suffix}})
+#     return config
+
+
+# class AwsMfaMixin(AwsBackendPropertiesMixin):
+
+#     def __init__(self, project, config):
+#         super().__init__(project, config)
+#         project.build_depends_on('boto3')
+#         project.build_depends_on('mfa')
+#         aws_mfa_mixin_config = config['AwsMfaMixin']
+#         self.account_id = aws_mfa_mixin_config['account_id']
+#         self.region = aws_mfa_mixin_config['region']
+#         self.mfa_role = aws_mfa_mixin_config['mfa_role']
+#         self.mfa_account_prefix = aws_mfa_mixin_config['mfa_account_prefix']
+#         self.mfa_login_account_suffix = aws_mfa_mixin_config['mfa_login_account_suffix']
+
+#     def project_vars(self):
+#         ret = super().project_vars()
+#         ret.update({'account_name': self.account_name,
+#                     'account_id': self.account_id,
+#                     'region': self.region,
+#                     'mfa_role': self.mfa_role,
+#                     'mfa_account_prefix': self.mfa_account_prefix,
+#                     'mfa_login_account_suffix': self.mfa_login_account_suffix})
+#         return ret
+
+#     def get_username_from_account(self, p_account_name):
+#         login_id = execute(r'cat ~/.aws/accounts | grep -A 2 "\[' + p_account_name +
+#                            r'\]"  | grep username | awk -F= \'{print $2}\'', shell=True)
+#         return login_id
+
+#     def get_account_id_from_account(self, p_account_name):
+#         account_id = execute(r'cat ~/.aws/accounts | grep -A 2 "\[' + p_account_name +
+#                              r'\]"  | grep account | awk -F= \'{print $2}\'', shell=True)
+#         return account_id
+
+#     def get_mfa(self, mfa_path='aws'):
+#         mfa_token = execute('mfa otp ' + mfa_path, shell=True)
+#         return mfa_token
+
+#     def write_aws_config(self, to_profile, key, secret):
+#         execute('aws configure --profile ' + to_profile +
+#                 ' set ' + key + ' ' + secret, shell=True)
+
+#     def get_mfa_session(self):
+#         from_account_name = self.mfa_account_prefix + self.mfa_login_account_suffix
+#         from_account_id = self.get_account_id_from_account(from_account_name)
+#         to_account_name = self.mfa_account_prefix + self.account_name
+#         to_account_id = self.get_account_id_from_account(to_account_name)
+#         login_id = self.get_username_from_account(from_account_name)
+#         mfa_token = self.get_mfa()
+#         ses = Session(profile_name=from_account_name)
+#         sts_client = ses.client('sts')
+#         response = sts_client.assume_role(
+#             RoleArn='arn:aws:iam::' + to_account_id + ':role/' + self.mfa_role,
+#             RoleSessionName=to_account_id + '-' + self.account_name + '-' + self.mfa_role,
+#             SerialNumber='arn:aws:iam::' + from_account_id + ':mfa/' + login_id,
+#             TokenCode=mfa_token
+#         )
+
+#         self.write_aws_config(to_account_name, 'aws_access_key_id',
+#                               response['Credentials']['AccessKeyId'])
+#         self.write_aws_config(to_account_name, 'aws_secret_access_key',
+#                               response['Credentials']['SecretAccessKey'])
+#         self.write_aws_config(to_account_name, 'aws_session_token',
+#                               response['Credentials']['SessionToken'])
+#         print('got token')
```

### Comparing `ddadevops-4.0.0.dev9/ddadevops/devops_build.py` & `ddadevops-4.0.2/ddadevops/c4k_build.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,38 @@
-import deprecation
-from subprocess import run, CalledProcessError
-from .domain import Devops
-from .infrastructure import ProjectRepository, FileApi
-
-
-@deprecation.deprecated(deprecated_in="3.2", details="create objects direct instead")
-def create_devops_build_config(
-    stage, project_root_path, module, build_dir_name="target"
-):
-    return {
-        "stage": stage,
-        "project_root_path": project_root_path,
-        "module": module,
-        "build_dir_name": build_dir_name,
-    }
-
-def get_devops_build(project):
-    return project.get_property("devops_build")
-
-
-@deprecation.deprecated(deprecated_in="3.2")
-# TODO: Remove from here!
-def get_tag_from_latest_commit():
-    try:
-        value = run(
-            "git describe --abbrev=0 --tags --exact-match",
-            shell=True,
-            capture_output=True,
-            check=True,
+from .domain import BuildType, DnsRecord
+from .devops_build import DevopsBuild
+from .infrastructure import ExecutionApi
+
+
+class C4kBuild(DevopsBuild):
+    def __init__(self, project, config):
+        super().__init__(project, config)
+        self.execution_api = ExecutionApi()
+        devops = self.devops_repo.get_devops(self.project)
+        if BuildType.C4K not in devops.specialized_builds:
+            raise ValueError("C4kBuild requires BuildType.C4K")
+
+    def update_runtime_config(self, dns_record: DnsRecord):
+        super().update_runtime_config(dns_record)
+        devops = self.devops_repo.get_devops(self.project)
+        devops.specialized_builds[BuildType.C4K].update_runtime_config(dns_record)
+        self.devops_repo.set_devops(self.project, devops)
+
+    def write_c4k_config(self):
+        devops = self.devops_repo.get_devops(self.project)
+        path = devops.build_path() + "/out_c4k_config.yaml"
+        self.file_api.write_yaml_to_file(
+            path, devops.specialized_builds[BuildType.C4K].config()
+        )
+
+    def write_c4k_auth(self):
+        devops = self.devops_repo.get_devops(self.project)
+        path = devops.build_path() + "/out_c4k_auth.yaml"
+        self.file_api.write_yaml_to_file(
+            path, devops.specialized_builds[BuildType.C4K].auth()
+        )
+
+    def c4k_apply(self, dry_run=False):
+        devops = self.devops_repo.get_devops(self.project)
+        return self.execution_api.execute(
+            devops.specialized_builds[BuildType.C4K].command(devops), dry_run
         )
-        return value.stdout.decode("UTF-8").rstrip()
-    except CalledProcessError:
-        return None
-
-
-class DevopsBuild:
-    def __init__(self, project, config: map = None, devops: Devops = None):
-        self.project = project
-        self.file_api = FileApi()
-        self.repo = ProjectRepository()
-        if not devops:
-            devops = Devops(
-                stage=config["stage"],
-                project_root_path=config["project_root_path"],
-                module=config["module"],
-                name=project.name,
-                build_dir_name=config["build_dir_name"],
-            )
-        self.repo.set_devops(self.project, devops)
-        self.repo.set_build(self.project, self)
-
-    def name(self):
-        devops = self.repo.get_devops(self.project)
-        return devops.name
-
-    def build_path(self):
-        devops = self.repo.get_devops(self.project)
-        return devops.build_path()
-
-    def initialize_build_dir(self):
-        devops = self.repo.get_devops(self.project)
-        self.file_api.clean_dir(devops.build_path())
```

### Comparing `ddadevops-4.0.0.dev9/ddadevops/devops_terraform_build.py` & `ddadevops-4.0.2/ddadevops/application/terraform_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,221 +1,221 @@
-import sys
-from os import chmod
-from json import load, dumps
-from subprocess import run
-from packaging import version
-from pkg_resources import resource_string
+from pathlib import Path
 from dda_python_terraform import Terraform, IsFlagged
-from .python_util import filter_none
-from .devops_build import DevopsBuild, create_devops_build_config
-
+from packaging import version
 
+from ..domain import Devops, BuildType
+from ..infrastructure import FileApi, ResourceApi, TerraformApi
 
 
-def create_devops_terraform_build_config(stage,
-                                         project_root_path,
-                                         module,
-                                         additional_vars,
-                                         build_dir_name='target',
-                                         output_json_name=None,
-                                         use_workspace=True,
-                                         use_package_common_files=True,
-                                         build_commons_path=None,
-                                         terraform_build_commons_dir_name='terraform',
-                                         debug_print_terraform_command=False,
-                                         additional_tfvar_files=None,
-                                         terraform_semantic_version="1.0.8"):
-    if not output_json_name:
-        output_json_name = 'out_' + module + '.json'
-    if not additional_tfvar_files:
-        additional_tfvar_files = []
-    ret = create_devops_build_config(
-        stage, project_root_path, module, build_dir_name)
-    ret.update({'additional_vars': additional_vars,
-                'output_json_name': output_json_name,
-                'use_workspace': use_workspace,
-                'use_package_common_files': use_package_common_files,
-                'build_commons_path': build_commons_path,
-                'terraform_build_commons_dir_name': terraform_build_commons_dir_name,
-                'debug_print_terraform_command': debug_print_terraform_command,
-                'additional_tfvar_files': additional_tfvar_files,
-                'terraform_semantic_version': terraform_semantic_version})
-    return ret
-
-class DevopsTerraformBuild(DevopsBuild):
-
-    def __init__(self, project, config):
-        super().__init__(project, config)
-        project.build_depends_on('dda-python-terraform')
-        self.additional_vars = config['additional_vars']
-        self.output_json_name = config['output_json_name']
-        self.use_workspace = config['use_workspace']
-        self.use_package_common_files = config['use_package_common_files']
-        self.build_commons_path = config['build_commons_path']
-        self.terraform_build_commons_dir_name = config['terraform_build_commons_dir_name']
-        self.debug_print_terraform_command = config['debug_print_terraform_command']
-        self.additional_tfvar_files = config['additional_tfvar_files']
-        self.terraform_semantic_version = config['terraform_semantic_version']
-
-    def terraform_build_commons_path(self):
-        mylist = [self.build_commons_path,
-                  self.terraform_build_commons_dir_name]
-        return '/'.join(filter_none(mylist)) + '/'
-
-    def project_vars(self):
-        ret = {'stage': self.stage}
-        if self.module:
-            ret['module'] = self.module
-        if self.additional_vars:
-            ret.update(self.additional_vars)
-        return ret
-
-    def copy_build_resource_file_from_package(self, name):
-        my_data = resource_string(
-            __name__, "src/main/resources/terraform/" + name)
-        with open(self.build_path() + '/' + name, "w", encoding="utf-8") as output_file:
-            output_file.write(my_data.decode(sys.stdout.encoding))
-
-    def copy_build_resources_from_package(self):
-        self.copy_build_resource_file_from_package('versions.tf')
-        self.copy_build_resource_file_from_package('terraform_build_vars.tf')
-
-    def copy_build_resources_from_dir(self):
-        run('cp -f ' + self.terraform_build_commons_path() +
-            '* ' + self.build_path(), shell=False, check=False)
-
-    def copy_local_state(self):
-        run('cp terraform.tfstate '  + self.build_path(), shell=False, check=False)
-
-    def rescue_local_state(self):
-        run('cp ' + self.build_path() + '/terraform.tfstate .', shell=False, check=False)
-
-    def initialize_build_dir(self):
-        super().initialize_build_dir()
-        if self.use_package_common_files:
-            self.copy_build_resources_from_package()
-        else:
-            self.copy_build_resources_from_dir()
-        self.copy_local_state()
-        run('cp *.tf ' + self.build_path(), shell=True, check=False)
-        run('cp *.properties ' + self.build_path(), shell=True, check=False)
-        run('cp *.tfvars ' + self.build_path(), shell=True, check=False)
-        run('cp -r scripts ' + self.build_path(), shell=True, check=False)
-
-    def post_build(self):
-        self.rescue_local_state()
-
-    def init_client(self):
-        terraform = Terraform(working_dir=self.build_path(), terraform_semantic_version=self.terraform_semantic_version)
-        terraform.init()
-        self.print_terraform_command(terraform)
-        if self.use_workspace:
-            try:
-                terraform.workspace('select', self.stage)
-                self.print_terraform_command(terraform)
-            except:
-                terraform.workspace('new', self.stage)
-                self.print_terraform_command(terraform)
-        return terraform
-
-    def write_output(self, terraform):
-        result = terraform.output(json=IsFlagged)
-        self.print_terraform_command(terraform)
-        with open(self.build_path() + self.output_json_name, "w", encoding="utf-8") as output_file:
-            output_file.write(dumps(result))
-        chmod(self.build_path() + self.output_json_name, 0o600)
-
-    def read_output_json(self):
-        with open(self.build_path() + self.output_json_name, 'r', encoding="utf-8") as file:
-            return load(file)
-
-    def plan(self):
-        terraform = self.init_client()
-        return_code, _, stderr = terraform.plan(detailed_exitcode=None, capture_output=False, raise_on_error=False,
-                var=self.project_vars(),
-                var_file=self.additional_tfvar_files)
-        self.post_build()
-        self.print_terraform_command(terraform)
-        if return_code > 0:
-            raise Exception(return_code, "terraform error:", stderr)
-
-    def plan_fail_on_diff(self):
-        terraform = self.init_client()
-        return_code, _, stderr = terraform.plan(detailed_exitcode=IsFlagged, capture_output=False, raise_on_error=False,
-                var=self.project_vars(),
-                var_file=self.additional_tfvar_files)
-        self.post_build()
-        self.print_terraform_command(terraform)
+# TODO: mv more fkt to Terraform_api ?
+class TerraformService:
+    def __init__(
+        self, file_api: FileApi, resource_api: ResourceApi, terraform_api: TerraformApi
+    ):
+        self.file_api = file_api
+        self.resource_api = resource_api
+        self.terraform_api = terraform_api
+
+    @classmethod
+    def prod(cls):
+        return cls(
+            FileApi(),
+            ResourceApi(),
+            TerraformApi(),
+        )
+
+    def initialize_build_dir(self, devops: Devops):
+        terraform = devops.specialized_builds[BuildType.TERRAFORM]
+        if terraform.tf_use_package_common_files:
+            self.__copy_build_resources_from_package__(devops)
+        else:
+            self.__copy_build_resources_from_dir__(devops)
+        self.__copy_local_state__(devops)
+        self.file_api.cp("*.tf", devops.build_path(), check=False)
+        self.file_api.cp("*.properties", devops.build_path(), check=False)
+        self.file_api.cp("*.tfvars", devops.build_path(), check=False)
+        self.file_api.cp_recursive("scripts", devops.build_path(), check=False)
+
+    def read_output(self, devops: Devops) -> map:
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
+        return self.file_api.read_json_fro_file(
+            Path(f"{devops.build_path()}{terraform_domain.tf_output_json_name}")
+        )
+
+    def plan(self, devops: Devops, fail_on_diff=False):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
+        if fail_on_diff:
+            detailed_exitcode = IsFlagged
+        else:
+            detailed_exitcode = None
+        terraform = self.__init_client__(devops)
+        return_code, _, stderr = terraform.plan(
+            detailed_exitcode=detailed_exitcode,
+            capture_output=False,
+            raise_on_error=False,
+            var=terraform_domain.project_vars(),
+            var_file=terraform_domain.tf_additional_tfvar_files,
+        )
+        self.__print_terraform_command__(terraform, devops)
         if return_code not in (0, 2):
-            raise Exception(return_code, "terraform error:", stderr)
+            raise RuntimeError(return_code, "terraform error:", stderr)
         if return_code == 2:
-            raise Exception(return_code, "diff in config found:", stderr)
+            raise RuntimeError(return_code, "diff in config found:", stderr)
 
-    def apply(self, auto_approve=False):
-        terraform = self.init_client()
+    def apply(self, devops: Devops, auto_approve=False):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
         if auto_approve:
             auto_approve_flag = IsFlagged
         else:
             auto_approve_flag = None
-        if version.parse(self.terraform_semantic_version) >= version.parse("1.0.0"):
-            return_code, _, stderr = terraform.apply(capture_output=False, raise_on_error=True,
-                    auto_approve=auto_approve_flag,
-                    var=self.project_vars(),
-                    var_file=self.additional_tfvar_files)
-        else:
-            return_code, _, stderr = terraform.apply(capture_output=False, raise_on_error=True,
-                    skip_plan=auto_approve,
-                    var=self.project_vars(),
-                    var_file=self.additional_tfvar_files)
-        self.write_output(terraform)
-        self.post_build()
-        self.print_terraform_command(terraform)
+        terraform = self.__init_client__(devops)
+        if version.parse(
+            terraform_domain.tf_terraform_semantic_version
+        ) >= version.parse("1.0.0"):
+            return_code, _, stderr = terraform.apply(
+                capture_output=False,
+                raise_on_error=True,
+                auto_approve=auto_approve_flag,
+                var=terraform_domain.project_vars(),
+                var_file=terraform_domain.tf_additional_tfvar_files,
+            )
+        else:
+            return_code, _, stderr = terraform.apply(
+                capture_output=False,
+                raise_on_error=True,
+                skip_plan=auto_approve,
+                var=terraform_domain.project_vars(),
+                var_file=terraform_domain.tf_additional_tfvar_files,
+            )
+        self.__print_terraform_command__(terraform, devops)
         if return_code > 0:
-            raise Exception(return_code, "terraform error:", stderr)
+            raise RuntimeError(return_code, "terraform error:", stderr)
+        self.__write_output__(terraform, devops)
 
-    def refresh(self):
-        terraform = self.init_client()
+    def refresh(self, devops: Devops):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
+        terraform = self.__init_client__(devops)
         return_code, _, stderr = terraform.refresh(
-                var=self.project_vars(),
-                var_file=self.additional_tfvar_files)
-        self.write_output(terraform)
-        self.post_build()
-        self.print_terraform_command(terraform)
+            var=terraform_domain.project_vars(),
+            var_file=terraform_domain.tf_additional_tfvar_files,
+        )
+        self.__print_terraform_command__(terraform, devops)
         if return_code > 0:
-            raise Exception(return_code, "terraform error:", stderr)
+            raise RuntimeError(return_code, "terraform error:", stderr)
+        self.__write_output__(terraform, devops)
 
-    def destroy(self, auto_approve=False):
-        terraform = self.init_client()
+    def destroy(self, devops: Devops, auto_approve=False):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
         if auto_approve:
             auto_approve_flag = IsFlagged
         else:
             auto_approve_flag = None
-        if version.parse(self.terraform_semantic_version) >= version.parse("1.0.0"):
-            return_code, _, stderr = terraform.destroy(capture_output=False, raise_on_error=True,
-                    auto_approve=auto_approve_flag,
-                    var=self.project_vars(),
-                    var_file=self.additional_tfvar_files)
-        else:
-            return_code, _, stderr = terraform.destroy(capture_output=False, raise_on_error=True,
-                    force=auto_approve_flag,
-                    var=self.project_vars(),
-                    var_file=self.additional_tfvar_files)
-        self.post_build()
-        self.print_terraform_command(terraform)
+        terraform = self.__init_client__(devops)
+        if version.parse(
+            terraform_domain.tf_terraform_semantic_version
+        ) >= version.parse("1.0.0"):
+            return_code, _, stderr = terraform.destroy(
+                capture_output=False,
+                raise_on_error=True,
+                auto_approve=auto_approve_flag,
+                var=terraform_domain.project_vars(),
+                var_file=terraform_domain.tf_additional_tfvar_files,
+            )
+        else:
+            return_code, _, stderr = terraform.destroy(
+                capture_output=False,
+                raise_on_error=True,
+                force=auto_approve_flag,
+                var=terraform_domain.project_vars(),
+                var_file=terraform_domain.tf_additional_tfvar_files,
+            )
+        self.__print_terraform_command__(terraform, devops)
         if return_code > 0:
-            raise Exception(return_code, "terraform error:", stderr)
+            raise RuntimeError(return_code, "terraform error:", stderr)
 
-    def tf_import(self, tf_import_name, tf_import_resource,):
-        terraform = self.init_client()
-        return_code, _, stderr = terraform.import_cmd(tf_import_name, tf_import_resource,
-                      capture_output=False, raise_on_error=True,
-                      var=self.project_vars(),
-                      var_file=self.additional_tfvar_files)
-        self.post_build()
-        self.print_terraform_command(terraform)
+    def tf_import(
+        self,
+        devops: Devops,
+        tf_import_name,
+        tf_import_resource,
+    ):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
+        terraform = self.__init_client__(devops)
+        return_code, _, stderr = terraform.import_cmd(
+            tf_import_name,
+            tf_import_resource,
+            capture_output=False,
+            raise_on_error=True,
+            var=terraform_domain.project_vars(),
+            var_file=terraform_domain.tf_additional_tfvar_files,
+        )
+        self.__print_terraform_command__(terraform, devops)
         if return_code > 0:
-            raise Exception(return_code, "terraform error:", stderr)
+            raise RuntimeError(return_code, "terraform error:", stderr)
 
-    def print_terraform_command(self, terraform):
-        if self.debug_print_terraform_command:
-            output = 'cd ' + self.build_path() + ' && ' + terraform.latest_cmd()
+    def post_build(self, devops: Devops):
+        self.__rescue_local_state__(devops)
+
+    def __copy_build_resource_file_from_package__(self, resource_name, devops: Devops):
+        data = self.resource_api.read_resource(
+            f"src/main/resources/terraform/{resource_name}"
+        )
+        self.file_api.write_data_to_file(
+            Path(f"{devops.build_path()}/{resource_name}"), data
+        )
+
+    def __copy_build_resources_from_package__(self, devops: Devops):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
+        for resource in terraform_domain.resources_from_package():
+            self.__copy_build_resource_file_from_package__(resource, devops)
+
+    def __copy_build_resources_from_dir__(self, devops: Devops):
+        terraform = devops.specialized_builds[BuildType.TERRAFORM]
+        self.file_api.cp_force(
+            f"{terraform.build_commons_path()}/*", devops.build_path()
+        )
+
+    def __print_terraform_command__(self, terraform: Terraform, devops: Devops):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
+        if terraform_domain.tf_debug_print_terraform_command:
+            output = f"cd {devops.build_path()} && {terraform.latest_cmd()}"
             print(output)
+
+    def __copy_local_state__(self, devops: Devops):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
+        if terraform_domain.is_local_state():
+            self.file_api.cp("terraform.tfstate", devops.build_path(), check=False)
+
+    def __rescue_local_state__(self, devops: Devops):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
+        if terraform_domain.is_local_state():
+            self.file_api.cp(
+                f"{devops.build_path()}/terraform.tfstate", ".", check=False
+            )
+
+    def __init_client__(self, devops: Devops):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
+        terraform = Terraform(
+            working_dir=devops.build_path(),
+            terraform_semantic_version=terraform_domain.tf_terraform_semantic_version,
+        )
+        if terraform_domain.is_local_state():
+            terraform.init()
+        else:
+            terraform.init(backend_config=terraform_domain.backend_config())
+        self.__print_terraform_command__(terraform, devops)
+        if terraform_domain.tf_use_workspace:
+            try:
+                terraform.workspace("select", devops.stage)
+                self.__print_terraform_command__(terraform, devops)
+            except:
+                terraform.workspace("new", devops.stage)
+                self.__print_terraform_command__(terraform, devops)
+        return terraform
+
+    def __write_output__(self, terraform, devops: Devops):
+        terraform_domain = devops.specialized_builds[BuildType.TERRAFORM]
+        result = terraform.output(json=IsFlagged)
+        self.__print_terraform_command__(terraform, devops)
+        self.file_api.write_json_to_file(
+            Path(f"{devops.build_path()}{terraform_domain.tf_output_json_name}"), result
+        )
```

### Comparing `ddadevops-4.0.0.dev9/ddadevops/src/main/resources/docker/image/resources/install_functions.sh` & `ddadevops-4.0.2/ddadevops/src/main/resources/docker/image/resources/install_functions.sh`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.0.dev9/ddadevops.egg-info/SOURCES.txt` & `ddadevops-4.0.2/ddadevops.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 MANIFEST.in
 __init__.py
 setup.py
 ddadevops/LICENSE
 ddadevops/__init__.py
-ddadevops/application.py
-ddadevops/aws_backend_properties_mixin.py
 ddadevops/aws_mfa_mixin.py
-ddadevops/aws_rds_pg_mixin.py
-ddadevops/c4k_mixin.py
+ddadevops/c4k_build.py
 ddadevops/credential.py
 ddadevops/devops_build.py
-ddadevops/devops_docker_build.py
+ddadevops/devops_image_build.py
 ddadevops/devops_terraform_build.py
-ddadevops/digitalocean_backend_properties_mixin.py
-ddadevops/digitalocean_terraform_build.py
-ddadevops/domain.py
-ddadevops/exoscale_mixin.py
-ddadevops/hetzner_mixin.py
-ddadevops/infrastructure.py
-ddadevops/provs_k3s_mixin.py
-ddadevops/python_util.py
+ddadevops/provs_k3s_build.py
+ddadevops/release_mixin.py
 ddadevops.egg-info/PKG-INFO
 ddadevops.egg-info/SOURCES.txt
 ddadevops.egg-info/dependency_links.txt
 ddadevops.egg-info/namespace_packages.txt
 ddadevops.egg-info/top_level.txt
 ddadevops.egg-info/zip-safe
-ddadevops/release_mixin/__init__.py
-ddadevops/release_mixin/build.py
-ddadevops/release_mixin/domain.py
-ddadevops/release_mixin/infrastructure.py
-ddadevops/release_mixin/infrastructure_api.py
-ddadevops/release_mixin/release_mixin.py
-ddadevops/release_mixin/services.py
+ddadevops/application/__init__.py
+ddadevops/application/image_build_service.py
+ddadevops/application/release_mixin_services.py
+ddadevops/application/terraform_service.py
+ddadevops/domain/__init__.py
+ddadevops/domain/build_file.py
+ddadevops/domain/c4k.py
+ddadevops/domain/common.py
+ddadevops/domain/credentials.py
+ddadevops/domain/devops_factory.py
+ddadevops/domain/image.py
+ddadevops/domain/init_service.py
+ddadevops/domain/provider_aws.py
+ddadevops/domain/provider_digitalocean.py
+ddadevops/domain/provider_hetzner.py
+ddadevops/domain/provs_k3s.py
+ddadevops/domain/release.py
+ddadevops/domain/terraform.py
+ddadevops/domain/version.py
+ddadevops/infrastructure/__init__.py
+ddadevops/infrastructure/infrastructure.py
+ddadevops/infrastructure/repository.py
 ddadevops/src/main/resources/docker/image/resources/install_functions.sh
-ddadevops/src/main/resources/terraform/aws_backend_properties_vars.tf
-ddadevops/src/main/resources/terraform/aws_backend_with_properties.tf
+ddadevops/src/main/resources/terraform/aws_backend.tf
+ddadevops/src/main/resources/terraform/aws_backend_wkms_vars.tf
+ddadevops/src/main/resources/terraform/aws_backend_wokms_vars.tf
 ddadevops/src/main/resources/terraform/aws_provider.tf
-ddadevops/src/main/resources/terraform/do_backend_properties_vars.tf
-ddadevops/src/main/resources/terraform/do_backend_with_properties.tf
-ddadevops/src/main/resources/terraform/do_mixin_vars.tf
+ddadevops/src/main/resources/terraform/aws_provider_vars.tf
+ddadevops/src/main/resources/terraform/do_backend.tf
+ddadevops/src/main/resources/terraform/do_backend_vars.tf
 ddadevops/src/main/resources/terraform/do_provider.tf
-ddadevops/src/main/resources/terraform/exoscale_mixin_vars.tf
-ddadevops/src/main/resources/terraform/exoscale_provider.tf
-ddadevops/src/main/resources/terraform/hetzner_mixin_vars.tf
+ddadevops/src/main/resources/terraform/do_provider_vars.tf
 ddadevops/src/main/resources/terraform/hetzner_provider.tf
+ddadevops/src/main/resources/terraform/hetzner_provider_vars.tf
 ddadevops/src/main/resources/terraform/provider_registry.tf
 ddadevops/src/main/resources/terraform/terraform_build_vars.tf
 ddadevops/src/main/resources/terraform/versions.tf
```

