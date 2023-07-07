# Comparing `tmp/juju-3.1.2.0.tar.gz` & `tmp/juju-3.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juju-3.1.2.0.tar", last modified: Fri May  5 08:28:36 2023, max compression
+gzip compressed data, was "juju-3.2.0.0.tar", last modified: Wed Jun  7 09:17:55 2023, max compression
```

## Comparing `juju-3.1.2.0.tar` & `juju-3.2.0.0.tar`

### file list

```diff
@@ -1,170 +1,169 @@
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.316959 juju-3.1.2.0/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)       65 2023-05-05 08:26:05.000000 juju-3.1.2.0/CONTRIBUTORS
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    11344 2023-05-05 08:26:05.000000 juju-3.1.2.0/LICENSE
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      159 2023-05-05 08:26:05.000000 juju-3.1.2.0/MANIFEST.in
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    32904 2023-05-05 08:28:36.316959 juju-3.1.2.0/PKG-INFO
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3085 2023-05-05 08:26:05.000000 juju-3.1.2.0/README.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        8 2023-05-05 08:26:05.000000 juju-3.1.2.0/VERSION
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.288959 juju-3.1.2.0/docs/
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.292959 juju-3.1.2.0/docs/api/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      190 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.action.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      206 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.annotation.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      210 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.application.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2352 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.client.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      186 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.cloud.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      210 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.constraints.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      206 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.controller.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      186 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.delta.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      190 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.errors.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      206 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.exceptions.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      182 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.juju.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      182 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.loop.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      194 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.machine.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      186 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.model.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      202 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.placement.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      198 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.relation.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      178 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.tag.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      182 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.unit.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      186 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/juju.utils.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      575 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/api/modules.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    29234 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/changelog.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      666 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/index.rst
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.292959 juju-3.1.2.0/docs/narrative/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3213 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/narrative/application.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2751 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/narrative/controller.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      100 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/narrative/index.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8727 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/narrative/model.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1469 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/narrative/unit.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3085 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/readme.rst
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.292959 juju-3.1.2.0/docs/upstream-updates/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     6676 2023-05-05 08:26:05.000000 juju-3.1.2.0/docs/upstream-updates/index.rst
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.300959 juju-3.1.2.0/examples/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1159 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/action.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1662 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/add_k8s.py
--rwxrwxr-x   0 jtirado   (1000) jtirado   (1000)     1593 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/add_machine.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1689 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/add_model.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1978 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/add_secrets_backend.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      819 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/allwatcher.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      938 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/charmhub_deploy_k8s.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      830 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/charmhub_deploy_machine.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      861 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/charmhub_find.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      701 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/charmhub_info.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      532 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/cloud.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      556 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/clouds.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1389 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/config.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      703 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/connect_current_model.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      955 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/controller.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1446 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/credential.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2148 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/crossmodel.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2261 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/crossmodel_bundle.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2466 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/crossmodel_controller.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2879 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/crossmodel_relation.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      841 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/debug-log.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      888 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/deploy.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1462 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/deploy_bundle.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      863 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/deploy_bundle_charmhub.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1075 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/deploy_bundle_with_trust.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      950 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/deploy_constraints.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      737 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/deploy_local_big_k8s_bundle.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1060 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/deploy_local_bundle_with_resources.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1220 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/deploy_local_file_resource.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1203 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/deploy_local_resource.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      803 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/deploy_with_revision.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2457 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/expose-application.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1236 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/formatted_status.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      422 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/fullstatus.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1070 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/future.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      642 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/get_cloud.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      583 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/leadership.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      250 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/list_secrets.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      669 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/livemodel.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      682 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/local_refresh.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      729 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/localcharm.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1073 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/machine_hostname.py
--rwxrwxr-x   0 jtirado   (1000) jtirado   (1000)      732 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/model.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1046 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/modelsummaries.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3239 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/relate.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      853 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/run_action.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1114 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/scp.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1195 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/status.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1619 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/unitrun.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1194 2023-05-05 08:26:05.000000 juju-3.1.2.0/examples/upgrade_local_charm_k8s.py
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.304959 juju-3.1.2.0/juju/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/__init__.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      642 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/action.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      119 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/annotation.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1072 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/annotationhelper.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    35814 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/application.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    49766 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/bundle.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      712 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/charm.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     7189 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/charmhub.py
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.316959 juju-3.1.2.0/juju/client/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/__init__.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8561 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   661969 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client1.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    41474 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client10.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   196176 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client11.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   245218 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client12.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   244188 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client13.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   115453 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client14.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   108914 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client15.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   103511 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client16.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   103511 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client17.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   368569 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client18.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   324521 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client2.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   192270 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client3.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   201775 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client4.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    41639 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client5.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   162109 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client6.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   153764 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client7.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    45251 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client8.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    56944 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_client9.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)  1210112 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/_definitions.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1224 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/client.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1347 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/codegen.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    38724 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/connection.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8034 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/connector.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    31664 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/facade.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      321 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/flags.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3660 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/gocookies.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     5968 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/jujudata.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    12465 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/overrides.py
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.316959 juju-3.1.2.0/juju/client/proxy/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      679 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/proxy/factory.py
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.316959 juju-3.1.2.0/juju/client/proxy/kubernetes/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2115 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/proxy/kubernetes/proxy.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      468 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/proxy/proxy.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      799 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/client/runner.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4478 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/constraints.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    37481 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/controller.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2637 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/delta.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3138 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/errors.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)       47 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/exceptions.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4219 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/jasyncio.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1162 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/juju.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      136 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/loop.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8768 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/machine.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   109382 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/model.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2134 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/names.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     6450 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/offerendpoints.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     5850 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/origin.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1829 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/placement.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    11423 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/provisioner.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/py.typed
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4954 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/relation.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1273 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/remoteapplication.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     6521 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/status.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1313 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/tag.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    14678 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/unit.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4576 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/url.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2182 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/user.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    17342 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/utils.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      415 2023-05-05 08:26:05.000000 juju-3.1.2.0/juju/version.py
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-05-05 08:28:36.304959 juju-3.1.2.0/juju.egg-info/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    32904 2023-05-05 08:28:36.000000 juju-3.1.2.0/juju.egg-info/PKG-INFO
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3644 2023-05-05 08:28:36.000000 juju-3.1.2.0/juju.egg-info/SOURCES.txt
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        1 2023-05-05 08:28:36.000000 juju-3.1.2.0/juju.egg-info/dependency_links.txt
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      308 2023-05-05 08:28:36.000000 juju-3.1.2.0/juju.egg-info/requires.txt
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        5 2023-05-05 08:28:36.000000 juju-3.1.2.0/juju.egg-info/top_level.txt
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)       38 2023-05-05 08:28:36.316959 juju-3.1.2.0/setup.cfg
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2260 2023-05-05 08:26:05.000000 juju-3.1.2.0/setup.py
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.208830 juju-3.2.0.0/
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)       65 2023-06-07 08:30:31.000000 juju-3.2.0.0/CONTRIBUTORS
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    11344 2023-06-07 08:30:31.000000 juju-3.2.0.0/LICENSE
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      159 2023-06-07 08:30:31.000000 juju-3.2.0.0/MANIFEST.in
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    34081 2023-06-07 09:17:55.208830 juju-3.2.0.0/PKG-INFO
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3085 2023-06-07 08:30:31.000000 juju-3.2.0.0/README.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        8 2023-06-07 08:30:31.000000 juju-3.2.0.0/VERSION
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.192830 juju-3.2.0.0/docs/
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.196830 juju-3.2.0.0/docs/api/
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      190 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.action.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      206 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.annotation.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      210 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.application.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2352 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.client.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      210 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.constraints.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      206 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.controller.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      186 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.delta.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      190 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.errors.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      206 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.exceptions.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      182 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.juju.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      182 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.loop.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      194 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.machine.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      186 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.model.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      202 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.placement.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      198 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.relation.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      178 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.tag.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      182 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.unit.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      186 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.utils.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      575 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/modules.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    30411 2023-06-07 09:17:40.000000 juju-3.2.0.0/docs/changelog.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      666 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/index.rst
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.196830 juju-3.2.0.0/docs/narrative/
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3213 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/narrative/application.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2751 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/narrative/controller.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      100 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/narrative/index.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8727 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/narrative/model.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1469 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/narrative/unit.rst
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3085 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/readme.rst
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.196830 juju-3.2.0.0/docs/upstream-updates/
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     6676 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/upstream-updates/index.rst
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.200830 juju-3.2.0.0/examples/
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1159 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/action.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1662 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/add_k8s.py
+-rwxrwxr-x   0 jtirado   (1000) jtirado   (1000)     1593 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/add_machine.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1689 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/add_model.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1978 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/add_secrets_backend.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      819 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/allwatcher.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      938 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/charmhub_deploy_k8s.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      830 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/charmhub_deploy_machine.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      861 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/charmhub_find.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      701 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/charmhub_info.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      532 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/cloud.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      556 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/clouds.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1389 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/config.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      703 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/connect_current_model.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      955 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/controller.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1446 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/credential.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2148 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/crossmodel.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2261 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/crossmodel_bundle.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2466 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/crossmodel_controller.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2879 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/crossmodel_relation.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      841 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/debug-log.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      888 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1462 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_bundle.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      863 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_bundle_charmhub.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1075 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_bundle_with_trust.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      950 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_constraints.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      737 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_local_big_k8s_bundle.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1060 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_local_bundle_with_resources.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1220 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_local_file_resource.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1203 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_local_resource.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      803 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_with_revision.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2457 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/expose-application.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1236 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/formatted_status.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      422 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/fullstatus.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1070 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/future.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      642 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/get_cloud.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      583 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/leadership.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      250 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/list_secrets.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      669 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/livemodel.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      682 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/local_refresh.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      729 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/localcharm.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1073 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/machine_hostname.py
+-rwxrwxr-x   0 jtirado   (1000) jtirado   (1000)      732 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/model.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1046 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/modelsummaries.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3239 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/relate.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      853 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/run_action.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1114 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/scp.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1195 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/status.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1619 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/unitrun.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1194 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/upgrade_local_charm_k8s.py
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.200830 juju-3.2.0.0/juju/
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/__init__.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      642 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/action.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      119 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/annotation.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1072 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/annotationhelper.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    36725 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/application.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    49702 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/bundle.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      712 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/charm.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     7189 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/charmhub.py
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.208830 juju-3.2.0.0/juju/client/
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/__init__.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8722 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   688237 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client1.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    41552 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client10.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   196254 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client11.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   245218 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client12.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   244188 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client13.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   115453 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client14.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   108914 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client15.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   103511 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client16.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   103511 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client17.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   369150 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client18.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   383690 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client2.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   192763 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client3.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   201969 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client4.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    41639 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client5.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   162109 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client6.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   154579 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client7.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    45251 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client8.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    56944 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client9.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)  1229695 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_definitions.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1224 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/client.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1347 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/codegen.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    38886 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/connection.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8034 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/connector.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    31664 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/facade.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      321 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/flags.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3660 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/gocookies.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     5968 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/jujudata.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    12465 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/overrides.py
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.208830 juju-3.2.0.0/juju/client/proxy/
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      679 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/proxy/factory.py
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.208830 juju-3.2.0.0/juju/client/proxy/kubernetes/
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2115 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/proxy/kubernetes/proxy.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      468 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/proxy/proxy.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      799 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/runner.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4478 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/constraints.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    37481 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/controller.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2637 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/delta.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3138 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/errors.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)       47 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/exceptions.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4219 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/jasyncio.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1162 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/juju.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      136 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/loop.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8768 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/machine.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   112234 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/model.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2134 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/names.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     6450 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/offerendpoints.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     5798 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/origin.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1829 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/placement.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    11423 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/provisioner.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/py.typed
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4954 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/relation.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1273 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/remoteapplication.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     6521 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/status.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1313 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/tag.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    14678 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/unit.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4576 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/url.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2182 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/user.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    17231 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/utils.py
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      415 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/version.py
+drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.200830 juju-3.2.0.0/juju.egg-info/
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    34081 2023-06-07 09:17:55.000000 juju-3.2.0.0/juju.egg-info/PKG-INFO
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3620 2023-06-07 09:17:55.000000 juju-3.2.0.0/juju.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        1 2023-06-07 09:17:55.000000 juju-3.2.0.0/juju.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      308 2023-06-07 09:17:55.000000 juju-3.2.0.0/juju.egg-info/requires.txt
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        5 2023-06-07 09:17:55.000000 juju-3.2.0.0/juju.egg-info/top_level.txt
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)       38 2023-06-07 09:17:55.208830 juju-3.2.0.0/setup.cfg
+-rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2260 2023-06-07 08:30:31.000000 juju-3.2.0.0/setup.py
```

### Comparing `juju-3.1.2.0/LICENSE` & `juju-3.2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/PKG-INFO` & `juju-3.2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juju
-Version: 3.1.2.0
+Version: 3.2.0.0
 Summary: Python library for Juju
 Home-page: https://github.com/juju/python-libjuju
 Maintainer: Juju Ecosystem Engineering
 Maintainer-email: juju@lists.ubuntu.com
 License: Apache 2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -145,25 +145,47 @@
 Pylibjuju releases now track the Juju release cadence. New generated schemas
 will be updated per Juju releases.
 
 
 Changelog
 ---------
 
+3.2.0.0
+^^^^^^^
+
+Wednesday 7th June 2023
+
+This release contains the new endpoints for Juju 3.2.0.
+
+This release works with any Juju 3.x controller.
+
+What's Changed
+""""""""""""""
+* Add base.bootstrapped decorator to integration test by @cderici in https://github.com/juju/python-libjuju/pull/856
+* Add mantic and lunar to list of ubuntu series by @addyess in https://github.com/juju/python-libjuju/pull/853
+* [JUJU-3885] forward port ipv6 support by @cderici in https://github.com/juju/python-libjuju/pull/866
+* Revisit auto documentation generation with sphinx on RTD by @cderici in https://github.com/juju/python-libjuju/pull/871
+* [JUJU-3894] Forward port some fixes from 2.9 to master by @cderici in https://github.com/juju/python-libjuju/pull/870
+* Revisit the secret backend integration test by @cderici in https://github.com/juju/python-libjuju/pull/858
+* [JUJU-3954] Fix incorrect base channel computation by @cderici in https://github.com/juju/python-libjuju/pull/875
+* [JUJU-3927] Add 3.2.0 facades  by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/874
+
 3.1.2.0
 ^^^^^^^
 
-Friday 5th May 2022
+Friday 5th May 2023
 
 This release has been tested with Juju 3.1.2 and contains the new 
 endpoints for secrets backend.
 
 This release works with any Juju 3.x controller.
 
-## What's Changed
+What's Changed
+""""""""""""""
+
 * [JUJU-3202] Add facades for 3.1.1. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/807
 * Add destroy units by @cderici in https://github.com/juju/python-libjuju/pull/812
 * [JUJU-3517] Revisit _build_facades in connection by @cderici in https://github.com/juju/python-libjuju/pull/826
 * [JUJU-3527] Added 3.1.2 and 3.2-beta2 schemas. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/828
 * [JUJU-1628] Deploy by revision by @cderici in https://github.com/juju/python-libjuju/pull/830
 * [JUJU-3552] Prepare 3.1.2.1 release by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/836
 
@@ -173,53 +195,62 @@
 Friday 10th February 2023
 
 This release targets juju version 3.1.0 and enables the new secrets backend api.
 Connectivity with juju controllers in the 3.x series is allowed, connections with different major version controllers (e.g. 2.x, 4.x, etc.) will be cancelled.
 
 This version is only tested using Juju 3.1.0.
 
-## What's Changed
+What's Changed
+""""""""""""""
+
 * setup.py: adjust websockets versions for py38-310 by @mert-kirpici in https://github.com/juju/python-libjuju/pull/731
 * [JUJU-2175] Remove juju 2.9 support on 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/774
 * [JUJU-2276] Series or base for local charms by @cderici in https://github.com/juju/python-libjuju/pull/777
 * [JUJU-2391] Fix wrong bases analysis. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/782
 * [JUJU-2401] Added release candidate workflow. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/784
 * [JUJU-2402] Prepare nightly juju edge testing. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/785
 * [JUJU-2237] Remove charmstore charm support from pylibjuju by @cderici in https://github.com/juju/python-libjuju/pull/786
 * [JUJU-2426] Secrets support by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/791
 * [JUJU-2573] Base argument for model deploy by @cderici in https://github.com/juju/python-libjuju/pull/798
 * Add compatibility for juju 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/799
 * Replace schemas.json with a wellformed version. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/800
 
-## New Contributors
+New Contributors
+""""""""""""""""
+
 * @mert-kirpici made their first contribution in https://github.com/juju/python-libjuju/pull/731
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.4...3.1.0.1
 
 3.0.4
 ^^^^^
 
 Wednesday 26th October
 
-## What's Changed
+What's Changed
+""""""""""""""
+
 * [JUJU-2027] Local refresh with resoruces by @cderici in https://github.com/juju/python-libjuju/pull/757
 * [JUJU-2026] Improve resolve charm by @cderici in https://github.com/juju/python-libjuju/pull/761
 * Add owner and data to license file by @arturo-seijas in https://github.com/juju/python-libjuju/pull/760
 
-## New Contributors
+New Contributors
+""""""""""""""""
+
 * @arturo-seijas made their first contribution in https://github.com/juju/python-libjuju/pull/760
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.3...3.0.4
 
 3.0.3
 ^^^^^
 
 Saturay October 22 2022
 
-## What's Changed
+What's Changed
+""""""""""""""
 
 * Wait for idle arg type check by @cderici in https://github.com/juju/python-libjuju/pull/741
 * [JUJU-1970] Revise local refresh by @cderici in https://github.com/juju/python-libjuju/pull/742
 * [JUJU-1984] Update facade schemas for juju 3.0-rc1-2 by @cderici in https://github.com/juju/python-libjuju/pull/745
 * [JUJU-1992] Fix charmhub series deploy 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/746
 * [JUJU-2001] Fix base for local charms and bundles for CharmOrigin 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/749
 * [JUJU-2017] Check subordinate field value instead of existence by @cderici in https://github.com/juju/python-libjuju/pull/751
@@ -231,15 +262,16 @@
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.2...3.0.3
 
 3.0.2
 ^^^^^
 
 Wednesday October 5 2022
 
-## What's Changed
+What's Changed
+""""""""""""""
 
 * Model name can now be accessed through model.name by @jack-w-shaw in https://github.com/juju/python-libjuju/pull/702
 * [JUJU-1593] Fix `unit.run()` and update the old client codes by @cderici in https://github.com/juju/python-libjuju/pull/710
 * Add py.typed marker by @sed-i in https://github.com/juju/python-libjuju/pull/709
 * [JUJU-1664] Add force, no-wait, destroy-storage params to app.destroy by @cderici in https://github.com/juju/python-libjuju/pull/714
 * snapcraft.io access should use https requests by @addyess in https://github.com/juju/python-libjuju/pull/715
 * [JUJU-1680] Add issue and PR templates by @cderici in https://github.com/juju/python-libjuju/pull/718
```

### Comparing `juju-3.1.2.0/README.rst` & `juju-3.2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/docs/api/juju.client.rst` & `juju-3.2.0.0/docs/api/juju.client.rst`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/docs/api/modules.rst` & `juju-3.2.0.0/docs/api/modules.rst`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/docs/changelog.rst` & `juju-3.2.0.0/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 Changelog
 ---------
 
+3.2.0.0
+^^^^^^^
+
+Wednesday 7th June 2023
+
+This release contains the new endpoints for Juju 3.2.0.
+
+This release works with any Juju 3.x controller.
+
+What's Changed
+""""""""""""""
+* Add base.bootstrapped decorator to integration test by @cderici in https://github.com/juju/python-libjuju/pull/856
+* Add mantic and lunar to list of ubuntu series by @addyess in https://github.com/juju/python-libjuju/pull/853
+* [JUJU-3885] forward port ipv6 support by @cderici in https://github.com/juju/python-libjuju/pull/866
+* Revisit auto documentation generation with sphinx on RTD by @cderici in https://github.com/juju/python-libjuju/pull/871
+* [JUJU-3894] Forward port some fixes from 2.9 to master by @cderici in https://github.com/juju/python-libjuju/pull/870
+* Revisit the secret backend integration test by @cderici in https://github.com/juju/python-libjuju/pull/858
+* [JUJU-3954] Fix incorrect base channel computation by @cderici in https://github.com/juju/python-libjuju/pull/875
+* [JUJU-3927] Add 3.2.0 facades  by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/874
+
 3.1.2.0
 ^^^^^^^
 
-Friday 5th May 2022
+Friday 5th May 2023
 
 This release has been tested with Juju 3.1.2 and contains the new 
 endpoints for secrets backend.
 
 This release works with any Juju 3.x controller.
 
-## What's Changed
+What's Changed
+""""""""""""""
+
 * [JUJU-3202] Add facades for 3.1.1. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/807
 * Add destroy units by @cderici in https://github.com/juju/python-libjuju/pull/812
 * [JUJU-3517] Revisit _build_facades in connection by @cderici in https://github.com/juju/python-libjuju/pull/826
 * [JUJU-3527] Added 3.1.2 and 3.2-beta2 schemas. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/828
 * [JUJU-1628] Deploy by revision by @cderici in https://github.com/juju/python-libjuju/pull/830
 * [JUJU-3552] Prepare 3.1.2.1 release by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/836
 
@@ -25,53 +47,62 @@
 Friday 10th February 2023
 
 This release targets juju version 3.1.0 and enables the new secrets backend api.
 Connectivity with juju controllers in the 3.x series is allowed, connections with different major version controllers (e.g. 2.x, 4.x, etc.) will be cancelled.
 
 This version is only tested using Juju 3.1.0.
 
-## What's Changed
+What's Changed
+""""""""""""""
+
 * setup.py: adjust websockets versions for py38-310 by @mert-kirpici in https://github.com/juju/python-libjuju/pull/731
 * [JUJU-2175] Remove juju 2.9 support on 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/774
 * [JUJU-2276] Series or base for local charms by @cderici in https://github.com/juju/python-libjuju/pull/777
 * [JUJU-2391] Fix wrong bases analysis. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/782
 * [JUJU-2401] Added release candidate workflow. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/784
 * [JUJU-2402] Prepare nightly juju edge testing. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/785
 * [JUJU-2237] Remove charmstore charm support from pylibjuju by @cderici in https://github.com/juju/python-libjuju/pull/786
 * [JUJU-2426] Secrets support by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/791
 * [JUJU-2573] Base argument for model deploy by @cderici in https://github.com/juju/python-libjuju/pull/798
 * Add compatibility for juju 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/799
 * Replace schemas.json with a wellformed version. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/800
 
-## New Contributors
+New Contributors
+""""""""""""""""
+
 * @mert-kirpici made their first contribution in https://github.com/juju/python-libjuju/pull/731
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.4...3.1.0.1
 
 3.0.4
 ^^^^^
 
 Wednesday 26th October
 
-## What's Changed
+What's Changed
+""""""""""""""
+
 * [JUJU-2027] Local refresh with resoruces by @cderici in https://github.com/juju/python-libjuju/pull/757
 * [JUJU-2026] Improve resolve charm by @cderici in https://github.com/juju/python-libjuju/pull/761
 * Add owner and data to license file by @arturo-seijas in https://github.com/juju/python-libjuju/pull/760
 
-## New Contributors
+New Contributors
+""""""""""""""""
+
 * @arturo-seijas made their first contribution in https://github.com/juju/python-libjuju/pull/760
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.3...3.0.4
 
 3.0.3
 ^^^^^
 
 Saturay October 22 2022
 
-## What's Changed
+What's Changed
+""""""""""""""
 
 * Wait for idle arg type check by @cderici in https://github.com/juju/python-libjuju/pull/741
 * [JUJU-1970] Revise local refresh by @cderici in https://github.com/juju/python-libjuju/pull/742
 * [JUJU-1984] Update facade schemas for juju 3.0-rc1-2 by @cderici in https://github.com/juju/python-libjuju/pull/745
 * [JUJU-1992] Fix charmhub series deploy 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/746
 * [JUJU-2001] Fix base for local charms and bundles for CharmOrigin 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/749
 * [JUJU-2017] Check subordinate field value instead of existence by @cderici in https://github.com/juju/python-libjuju/pull/751
@@ -83,15 +114,16 @@
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.2...3.0.3
 
 3.0.2
 ^^^^^
 
 Wednesday October 5 2022
 
-## What's Changed
+What's Changed
+""""""""""""""
 
 * Model name can now be accessed through model.name by @jack-w-shaw in https://github.com/juju/python-libjuju/pull/702
 * [JUJU-1593] Fix `unit.run()` and update the old client codes by @cderici in https://github.com/juju/python-libjuju/pull/710
 * Add py.typed marker by @sed-i in https://github.com/juju/python-libjuju/pull/709
 * [JUJU-1664] Add force, no-wait, destroy-storage params to app.destroy by @cderici in https://github.com/juju/python-libjuju/pull/714
 * snapcraft.io access should use https requests by @addyess in https://github.com/juju/python-libjuju/pull/715
 * [JUJU-1680] Add issue and PR templates by @cderici in https://github.com/juju/python-libjuju/pull/718
```

### Comparing `juju-3.1.2.0/docs/index.rst` & `juju-3.2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/docs/narrative/application.rst` & `juju-3.2.0.0/docs/narrative/application.rst`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/docs/narrative/controller.rst` & `juju-3.2.0.0/docs/narrative/controller.rst`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/docs/narrative/model.rst` & `juju-3.2.0.0/docs/narrative/model.rst`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/docs/narrative/unit.rst` & `juju-3.2.0.0/docs/narrative/unit.rst`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/docs/readme.rst` & `juju-3.2.0.0/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/docs/upstream-updates/index.rst` & `juju-3.2.0.0/docs/upstream-updates/index.rst`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/action.py` & `juju-3.2.0.0/examples/action.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/add_k8s.py` & `juju-3.2.0.0/examples/add_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/add_machine.py` & `juju-3.2.0.0/examples/add_machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/add_model.py` & `juju-3.2.0.0/examples/add_model.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/add_secrets_backend.py` & `juju-3.2.0.0/examples/add_secrets_backend.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/allwatcher.py` & `juju-3.2.0.0/examples/allwatcher.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/charmhub_deploy_k8s.py` & `juju-3.2.0.0/examples/charmhub_deploy_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/charmhub_deploy_machine.py` & `juju-3.2.0.0/examples/charmhub_deploy_machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/charmhub_find.py` & `juju-3.2.0.0/examples/charmhub_find.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/charmhub_info.py` & `juju-3.2.0.0/examples/charmhub_info.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/cloud.py` & `juju-3.2.0.0/examples/cloud.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/clouds.py` & `juju-3.2.0.0/examples/clouds.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/config.py` & `juju-3.2.0.0/examples/config.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/connect_current_model.py` & `juju-3.2.0.0/examples/connect_current_model.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/controller.py` & `juju-3.2.0.0/examples/controller.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/credential.py` & `juju-3.2.0.0/examples/credential.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/crossmodel.py` & `juju-3.2.0.0/examples/crossmodel.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/crossmodel_bundle.py` & `juju-3.2.0.0/examples/crossmodel_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/crossmodel_controller.py` & `juju-3.2.0.0/examples/crossmodel_controller.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/crossmodel_relation.py` & `juju-3.2.0.0/examples/crossmodel_relation.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/debug-log.py` & `juju-3.2.0.0/examples/debug-log.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/deploy.py` & `juju-3.2.0.0/examples/deploy.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/deploy_bundle.py` & `juju-3.2.0.0/examples/deploy_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/deploy_bundle_charmhub.py` & `juju-3.2.0.0/examples/deploy_bundle_charmhub.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/deploy_bundle_with_trust.py` & `juju-3.2.0.0/examples/deploy_bundle_with_trust.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/deploy_constraints.py` & `juju-3.2.0.0/examples/deploy_constraints.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/deploy_local_big_k8s_bundle.py` & `juju-3.2.0.0/examples/deploy_local_big_k8s_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/deploy_local_bundle_with_resources.py` & `juju-3.2.0.0/examples/deploy_local_bundle_with_resources.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/deploy_local_file_resource.py` & `juju-3.2.0.0/examples/deploy_local_file_resource.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/deploy_local_resource.py` & `juju-3.2.0.0/examples/deploy_local_resource.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/deploy_with_revision.py` & `juju-3.2.0.0/examples/deploy_with_revision.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/expose-application.py` & `juju-3.2.0.0/examples/expose-application.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/formatted_status.py` & `juju-3.2.0.0/examples/formatted_status.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/future.py` & `juju-3.2.0.0/examples/future.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/get_cloud.py` & `juju-3.2.0.0/examples/get_cloud.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/leadership.py` & `juju-3.2.0.0/examples/leadership.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/livemodel.py` & `juju-3.2.0.0/examples/livemodel.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/local_refresh.py` & `juju-3.2.0.0/examples/local_refresh.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/localcharm.py` & `juju-3.2.0.0/examples/localcharm.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/machine_hostname.py` & `juju-3.2.0.0/examples/machine_hostname.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/model.py` & `juju-3.2.0.0/examples/model.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/modelsummaries.py` & `juju-3.2.0.0/examples/modelsummaries.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/relate.py` & `juju-3.2.0.0/examples/relate.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/run_action.py` & `juju-3.2.0.0/examples/run_action.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/scp.py` & `juju-3.2.0.0/examples/scp.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/status.py` & `juju-3.2.0.0/examples/status.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/unitrun.py` & `juju-3.2.0.0/examples/unitrun.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/examples/upgrade_local_charm_k8s.py` & `juju-3.2.0.0/examples/upgrade_local_charm_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/action.py` & `juju-3.2.0.0/juju/action.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/annotationhelper.py` & `juju-3.2.0.0/juju/annotationhelper.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/application.py` & `juju-3.2.0.0/juju/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,18 +87,23 @@
         """Get the application status.
 
         If the application is unknown it will attempt to derive the unit
         workload status and highlight the most relevant (severity).
         """
         status = self.safe_data['status']['current']
         if status == "unset":
-            unit_status = []
+            known_statuses = []
             for unit in self.units:
-                unit_status.append(unit.workload_status)
-            return derive_status(unit_status)
+                known_statuses.append(unit.workload_status)
+            # If the self.get_status() is called (i.e. the status
+            # is received by FullStatus from the API) then add
+            # that into this computation as it might be more up
+            # to date (and more severe).
+            known_statuses.append(self._status)
+            return derive_status(known_statuses)
         return status
 
     @property
     def status_message(self):
         """Get the application status message, as set by the charm's leader.
 
         """
@@ -461,14 +466,31 @@
             if result.application_tag == self.tag and result.actions:
                 actions = result.actions
                 break
         if not schema:
             actions = {k: v.description for k, v in actions.items()}
         return actions
 
+    async def get_status(self):
+        """Get the application status using info from the FullStatus
+        as well, because it might be more up to date than our model
+
+        :return: str status
+        """
+
+        client_facade = client.ClientFacade.from_connection(self.connection)
+
+        full_status = await client_facade.FullStatus(patterns=None)
+        _app = full_status.applications.get(self.name, None)
+        if not _app:
+            raise JujuError(f"application is not in FullStatus : {self.name}")
+
+        self._status = derive_status([self.status, _app.status.status])
+        return self._status
+
     def attach_resource(self, resource_name, file_name, file_obj):
         """Updates the resource for an application by uploading file from
         local disk to the Juju controller.
 
         :param str resource_name: Name of the resource to be updated.
         :param str file_name: Name of the local file to be uploaded.
         :param TextIOWrapper file_obj: Actual object to be read for data.
```

### Comparing `juju-3.1.2.0/juju/bundle.py` & `juju-3.2.0.0/juju/bundle.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 class BundleHandler:
     """
     Handle bundles by using the API to translate bundle YAML into a plan of
     steps and then dispatching each of those using the API.
     """
+
     def __init__(self, model, trusted=False, forced=False):
         self.model = model
         self.trusted = trusted
         self.forced = forced
         self.bundle = None
         self.overlays = []
         self.overlay_removed_charms = set()
@@ -155,16 +156,15 @@
                     metadata,
                     resources=bundle.get('applications', {app_name: {}})[app_name].get("resources", {}),
                 )
                 apps_dict[app_name]['charm'] = charm_url
                 apps_dict[app_name]["resources"] = resources
                 origin = client.CharmOrigin(source="local", risk="stable")
                 if not self.model.connection().is_using_old_client:
-                    origin.base = utils.get_local_charm_base(series, '',
-                                                             metadata,
+                    origin.base = utils.get_local_charm_base(series,
                                                              charm_dir,
                                                              client.Base)
                 self.origins[charm_url] = {str(None): origin}
 
         return bundle
 
     def _resolve_include_file_config(self, bundle_dir):
@@ -519,14 +519,15 @@
     :devices: optional devices constraints.
     :endpoint_bindings: optional endpoint bindings
     :resources: identifies the revision to use for each resource of the
         application's charm.
     :local_resources: identifies the path to the local resource of the
         application's charm.
     """
+
     def __init__(self, change_id, requires, params=None):
         super(AddApplicationChange, self).__init__(change_id, requires)
 
         if isinstance(params, list):
             self.charm = params[0]
             self.series = params[1]
             self.application = params[2]
@@ -665,14 +666,15 @@
 
     Params holds the following values:
         :charm: URL of the charm to be added.
         :series: series of the charm to be added if the charm default is
            not sufficient.
         :channel: preferred channel for obtaining the charm.
     """
+
     def __init__(self, change_id, requires, params=None):
         super(AddCharmChange, self).__init__(change_id, requires)
 
         if isinstance(params, list):
             self.charm = params[0]
             self.series = params[1]
             if len(params) > 2 and params[2] != "":
@@ -766,14 +768,15 @@
     Params holds the following values:
         :series: optional machine OS series.
         :constraints: optional machine constraints.
         :container_type: optionally type of the container (for instance
             "lxc" or kvm"). It is not specified for top level machines.
         :parent_id: id of the parent machine.
     """
+
     def __init__(self, change_id, requires, params=None):
         super(AddMachineChange, self).__init__(change_id, requires)
         # this one is weird, as it returns a set of parameters inside a list.
         if isinstance(params, list):
             options = params[0] or {}
             self.series = options.get("series")
             self.constraints = options.get("constraints")
@@ -857,14 +860,15 @@
         Endpoint1 and Endpoint2 hold relation endpoints in the
         "application:interface" form, where the application is either a
         placeholder pointing to an application change or in the case of a model
         that already has this application deployed, the name of the
         application, and the interface is optional. Examples are
         "$deploy-42:web", "$deploy-42", "mysql:db".
     """
+
     def __init__(self, change_id, requires, params=None):
         super(AddRelationChange, self).__init__(change_id, requires)
 
         if isinstance(params, list):
             self.endpoint1 = params[0]
             self.endpoint2 = params[1]
         elif isinstance(params, dict):
@@ -918,14 +922,15 @@
 
     Params holds the following values:
         :application: application placeholder name for which a unit is
             added.
         :to: optional location where to add the unit, as a placeholder
             pointing to another unit change or to a machine change.
     """
+
     def __init__(self, change_id, requires, params=None):
         super(AddUnitChange, self).__init__(change_id, requires)
 
         if isinstance(params, list):
             self.application = params[0]
             self.to = params[1]
         elif isinstance(params, dict):
@@ -986,14 +991,15 @@
     Params holds the following values:
         :application: is the name of the application to create an offer for.
             added.
         :endpoint: is a list of application endpoint to expose as part of an
             offer.
         :offer_name: describes the offer name.
     """
+
     def __init__(self, change_id, requires, params=None):
         super(CreateOfferChange, self).__init__(change_id, requires)
 
         if isinstance(params, list):
             self.application = params[0]
             self.endpoints = params[1]
             self.offer_name = params[2]
@@ -1040,14 +1046,15 @@
         params could either be a list or a dict. The later being the newer
         return results.
 
     Params holds the following values:
         :url: contains the location of the offer
         :application_name: describes the application name on offer.
     """
+
     def __init__(self, change_id, requires, params=None):
         super(ConsumeOfferChange, self).__init__(change_id, requires)
 
         if isinstance(params, list):
             self.url = params[0]
             self.application_name = params[1]
         elif isinstance(params, dict):
@@ -1095,14 +1102,15 @@
         :application: placeholder name of the application that must be
             exposed.
         :exposed_endpoints: a an optional dictionary where keys are endpoint
             names and values are dicts that specify the space names and CIDRs
             that should be able to access the port ranges that the application
             has opened for each endpoint.
     """
+
     def __init__(self, change_id, requires, params=None):
         super(ExposeChange, self).__init__(change_id, requires)
 
         self.exposed_endpoints = None
         if isinstance(params, list):
             self.application = params[0]
         elif isinstance(params, dict):
@@ -1144,14 +1152,15 @@
         params could either be a list or a dict. The later being the newer
         return results.
 
     Params holds the following values:
         :application: placeholder name of the application to be scaled.
         :scale: is the new scale value to use.
     """
+
     def __init__(self, change_id, requires, params=None):
         super(ScaleChange, self).__init__(change_id, requires)
 
         if isinstance(params, list):
             self.application = params[0]
             self.scale = params[1]
         elif isinstance(params, dict):
@@ -1196,14 +1205,15 @@
 
     Params holds the following values:
         :id: is the placeholder for the application or machine change
             corresponding to the entity to be annotated.
         :entity_type: type of the entity, "application" or "machine".
         :ennotations: annotations as key/value pairs.
     """
+
     def __init__(self, change_id, requires, params=None):
         super(SetAnnotationsChange, self).__init__(change_id, requires)
 
         if isinstance(params, list):
             self.id = params[0]
             self.entity_type = params[1]
             self.annotations = params[2]
```

### Comparing `juju-3.1.2.0/juju/charm.py` & `juju-3.2.0.0/juju/charm.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/charmhub.py` & `juju-3.2.0.0/juju/charmhub.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_client.py` & `juju-3.2.0.0/juju/client/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,18 @@
     pass
 
 
 class AgentFacade(TypeFactory):
     pass
 
 
+class AgentLifeFlagFacade(TypeFactory):
+    pass
+
+
 class AgentToolsFacade(TypeFactory):
     pass
 
 
 class AllModelWatcherFacade(TypeFactory):
     pass
 
@@ -469,22 +473,30 @@
     pass
 
 
 class SecretBackendsRotateWatcherFacade(TypeFactory):
     pass
 
 
+class SecretsDrainFacade(TypeFactory):
+    pass
+
+
 class SecretsFacade(TypeFactory):
     pass
 
 
 class SecretsManagerFacade(TypeFactory):
     pass
 
 
+class SecretsRevisionWatcherFacade(TypeFactory):
+    pass
+
+
 class SecretsTriggerWatcherFacade(TypeFactory):
     pass
 
 
 class SingularFacade(TypeFactory):
     pass
```

### Comparing `juju-3.1.2.0/juju/client/_client1.py` & `juju-3.2.0.0/juju/client/_client1.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,113 @@
                    params=_params)
 
         reply = await self.rpc(msg)
         return reply
 
 
 
+class AgentLifeFlagFacade(Type):
+    name = 'AgentLifeFlag'
+    version = 1
+    schema =     {'definitions': {'Entities': {'additionalProperties': False,
+                                  'properties': {'entities': {'items': {'$ref': '#/definitions/Entity'},
+                                                              'type': 'array'}},
+                                  'required': ['entities'],
+                                  'type': 'object'},
+                     'Entity': {'additionalProperties': False,
+                                'properties': {'tag': {'type': 'string'}},
+                                'required': ['tag'],
+                                'type': 'object'},
+                     'Error': {'additionalProperties': False,
+                               'properties': {'code': {'type': 'string'},
+                                              'info': {'patternProperties': {'.*': {'additionalProperties': True,
+                                                                                    'type': 'object'}},
+                                                       'type': 'object'},
+                                              'message': {'type': 'string'}},
+                               'required': ['message', 'code'],
+                               'type': 'object'},
+                     'LifeResult': {'additionalProperties': False,
+                                    'properties': {'error': {'$ref': '#/definitions/Error'},
+                                                   'life': {'type': 'string'}},
+                                    'required': ['life'],
+                                    'type': 'object'},
+                     'LifeResults': {'additionalProperties': False,
+                                     'properties': {'results': {'items': {'$ref': '#/definitions/LifeResult'},
+                                                                'type': 'array'}},
+                                     'required': ['results'],
+                                     'type': 'object'},
+                     'NotifyWatchResult': {'additionalProperties': False,
+                                           'properties': {'NotifyWatcherId': {'type': 'string'},
+                                                          'error': {'$ref': '#/definitions/Error'}},
+                                           'required': ['NotifyWatcherId'],
+                                           'type': 'object'},
+                     'NotifyWatchResults': {'additionalProperties': False,
+                                            'properties': {'results': {'items': {'$ref': '#/definitions/NotifyWatchResult'},
+                                                                       'type': 'array'}},
+                                            'required': ['results'],
+                                            'type': 'object'}},
+     'properties': {'Life': {'description': 'Life returns the life status of every '
+                                            'supplied entity, where available.',
+                             'properties': {'Params': {'$ref': '#/definitions/Entities'},
+                                            'Result': {'$ref': '#/definitions/LifeResults'}},
+                             'type': 'object'},
+                    'Watch': {'description': 'Watch starts an NotifyWatcher for '
+                                             'each given entity.',
+                              'properties': {'Params': {'$ref': '#/definitions/Entities'},
+                                             'Result': {'$ref': '#/definitions/NotifyWatchResults'}},
+                              'type': 'object'}},
+     'type': 'object'}
+    
+
+    @ReturnMapping(LifeResults)
+    async def Life(self, entities=None):
+        '''
+        Life returns the life status of every supplied entity, where available.
+
+        entities : typing.Sequence[~Entity]
+        Returns -> LifeResults
+        '''
+        if entities is not None and not isinstance(entities, (bytes, str, list)):
+            raise Exception("Expected entities to be a Sequence, received: {}".format(type(entities)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='AgentLifeFlag',
+                   request='Life',
+                   version=1,
+                   params=_params)
+        _params['entities'] = entities
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(NotifyWatchResults)
+    async def Watch(self, entities=None):
+        '''
+        Watch starts an NotifyWatcher for each given entity.
+
+        entities : typing.Sequence[~Entity]
+        Returns -> NotifyWatchResults
+        '''
+        if entities is not None and not isinstance(entities, (bytes, str, list)):
+            raise Exception("Expected entities to be a Sequence, received: {}".format(type(entities)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='AgentLifeFlag',
+                   request='Watch',
+                   version=1,
+                   params=_params)
+        _params['entities'] = entities
+        reply = await self.rpc(msg)
+        return reply
+
+
+
 class AgentToolsFacade(Type):
     name = 'AgentTools'
     version = 1
     schema =     {'properties': {'UpdateToolsAvailable': {'description': 'UpdateToolsAvailable '
                                                             'invokes a lookup and '
                                                             'further update in '
                                                             'environ\n'
@@ -522,46 +621,35 @@
                                                             'info'],
                                                'type': 'object'},
                      'Base': {'additionalProperties': False,
                               'properties': {'channel': {'type': 'string'},
                                              'name': {'type': 'string'}},
                               'required': ['name', 'channel'],
                               'type': 'object'},
-                     'CAASApplicationGarbageCollectArg': {'additionalProperties': False,
-                                                          'properties': {'active-pod-names': {'items': {'type': 'string'},
-                                                                                              'type': 'array'},
-                                                                         'application': {'$ref': '#/definitions/Entity'},
-                                                                         'desired-replicas': {'type': 'integer'},
-                                                                         'force': {'type': 'boolean'},
-                                                                         'observed-units': {'$ref': '#/definitions/Entities'}},
-                                                          'required': ['application',
-                                                                       'observed-units',
-                                                                       'desired-replicas',
-                                                                       'active-pod-names',
-                                                                       'force'],
-                                                          'type': 'object'},
-                     'CAASApplicationGarbageCollectArgs': {'additionalProperties': False,
-                                                           'properties': {'args': {'items': {'$ref': '#/definitions/CAASApplicationGarbageCollectArg'},
-                                                                                   'type': 'array'}},
-                                                           'required': ['args'],
-                                                           'type': 'object'},
                      'CAASApplicationOCIResourceResult': {'additionalProperties': False,
                                                           'properties': {'error': {'$ref': '#/definitions/Error'},
                                                                          'result': {'$ref': '#/definitions/CAASApplicationOCIResources'}},
                                                           'type': 'object'},
                      'CAASApplicationOCIResourceResults': {'additionalProperties': False,
                                                            'properties': {'results': {'items': {'$ref': '#/definitions/CAASApplicationOCIResourceResult'},
                                                                                       'type': 'array'}},
                                                            'required': ['results'],
                                                            'type': 'object'},
                      'CAASApplicationOCIResources': {'additionalProperties': False,
                                                      'properties': {'images': {'patternProperties': {'.*': {'$ref': '#/definitions/DockerImageInfo'}},
                                                                                'type': 'object'}},
                                                      'required': ['images'],
                                                      'type': 'object'},
+                     'CAASApplicationProvisionerConfig': {'additionalProperties': False,
+                                                          'properties': {'unmanaged-applications': {'$ref': '#/definitions/Entities'}},
+                                                          'type': 'object'},
+                     'CAASApplicationProvisionerConfigResult': {'additionalProperties': False,
+                                                                'properties': {'error': {'$ref': '#/definitions/Error'},
+                                                                               'provisioner-config': {'$ref': '#/definitions/CAASApplicationProvisionerConfig'}},
+                                                                'type': 'object'},
                      'CAASApplicationProvisioningInfo': {'additionalProperties': False,
                                                          'properties': {'api-addresses': {'items': {'type': 'string'},
                                                                                           'type': 'array'},
                                                                         'base': {'$ref': '#/definitions/Base'},
                                                                         'ca-cert': {'type': 'string'},
                                                                         'charm-modified-version': {'type': 'integer'},
                                                                         'charm-url': {'type': 'string'},
@@ -585,14 +673,30 @@
                                                                       'constraints'],
                                                          'type': 'object'},
                      'CAASApplicationProvisioningInfoResults': {'additionalProperties': False,
                                                                 'properties': {'results': {'items': {'$ref': '#/definitions/CAASApplicationProvisioningInfo'},
                                                                                            'type': 'array'}},
                                                                 'required': ['results'],
                                                                 'type': 'object'},
+                     'CAASApplicationProvisioningState': {'additionalProperties': False,
+                                                          'properties': {'scale-target': {'type': 'integer'},
+                                                                         'scaling': {'type': 'boolean'}},
+                                                          'required': ['scaling',
+                                                                       'scale-target'],
+                                                          'type': 'object'},
+                     'CAASApplicationProvisioningStateArg': {'additionalProperties': False,
+                                                             'properties': {'application': {'$ref': '#/definitions/Entity'},
+                                                                            'provisioning-state': {'$ref': '#/definitions/CAASApplicationProvisioningState'}},
+                                                             'required': ['application',
+                                                                          'provisioning-state'],
+                                                             'type': 'object'},
+                     'CAASApplicationProvisioningStateResult': {'additionalProperties': False,
+                                                                'properties': {'error': {'$ref': '#/definitions/Error'},
+                                                                               'provisioning-state': {'$ref': '#/definitions/CAASApplicationProvisioningState'}},
+                                                                'type': 'object'},
                      'CAASUnitInfo': {'additionalProperties': False,
                                       'properties': {'tag': {'type': 'string'},
                                                      'unit-status': {'$ref': '#/definitions/UnitStatus'}},
                                       'required': ['tag'],
                                       'type': 'object'},
                      'CAASUnitsResult': {'additionalProperties': False,
                                          'properties': {'error': {'$ref': '#/definitions/Error'},
@@ -790,14 +894,41 @@
                                                    'count-max',
                                                    'minimum-size'],
                                       'type': 'object'},
                      'CharmURL': {'additionalProperties': False,
                                   'properties': {'url': {'type': 'string'}},
                                   'required': ['url'],
                                   'type': 'object'},
+                     'DestroyUnitInfo': {'additionalProperties': False,
+                                         'properties': {'destroyed-storage': {'items': {'$ref': '#/definitions/Entity'},
+                                                                              'type': 'array'},
+                                                        'detached-storage': {'items': {'$ref': '#/definitions/Entity'},
+                                                                             'type': 'array'}},
+                                         'type': 'object'},
+                     'DestroyUnitParams': {'additionalProperties': False,
+                                           'properties': {'destroy-storage': {'type': 'boolean'},
+                                                          'dry-run': {'type': 'boolean'},
+                                                          'force': {'type': 'boolean'},
+                                                          'max-wait': {'type': 'integer'},
+                                                          'unit-tag': {'type': 'string'}},
+                                           'required': ['unit-tag'],
+                                           'type': 'object'},
+                     'DestroyUnitResult': {'additionalProperties': False,
+                                           'properties': {'error': {'$ref': '#/definitions/Error'},
+                                                          'info': {'$ref': '#/definitions/DestroyUnitInfo'}},
+                                           'type': 'object'},
+                     'DestroyUnitResults': {'additionalProperties': False,
+                                            'properties': {'results': {'items': {'$ref': '#/definitions/DestroyUnitResult'},
+                                                                       'type': 'array'}},
+                                            'type': 'object'},
+                     'DestroyUnitsParams': {'additionalProperties': False,
+                                            'properties': {'units': {'items': {'$ref': '#/definitions/DestroyUnitParams'},
+                                                                     'type': 'array'}},
+                                            'required': ['units'],
+                                            'type': 'object'},
                      'DetailedStatus': {'additionalProperties': False,
                                         'properties': {'data': {'patternProperties': {'.*': {'additionalProperties': True,
                                                                                              'type': 'object'}},
                                                                 'type': 'object'},
                                                        'err': {'$ref': '#/definitions/Error'},
                                                        'info': {'type': 'string'},
                                                        'kind': {'type': 'string'},
@@ -1076,14 +1207,15 @@
                                                     'type': 'object'},
                      'Value': {'additionalProperties': False,
                                'properties': {'allocate-public-ip': {'type': 'boolean'},
                                               'arch': {'type': 'string'},
                                               'container': {'type': 'string'},
                                               'cores': {'type': 'integer'},
                                               'cpu-power': {'type': 'integer'},
+                                              'image-id': {'type': 'string'},
                                               'instance-role': {'type': 'string'},
                                               'instance-type': {'type': 'string'},
                                               'mem': {'type': 'integer'},
                                               'root-disk': {'type': 'integer'},
                                               'root-disk-source': {'type': 'string'},
                                               'spaces': {'items': {'type': 'string'},
                                                          'type': 'array'},
@@ -1104,38 +1236,14 @@
                                                                'returns the OCI '
                                                                'image resources '
                                                                'for an '
                                                                'application.',
                                                 'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                                                'Result': {'$ref': '#/definitions/CAASApplicationOCIResourceResults'}},
                                                 'type': 'object'},
-                    'CAASApplicationGarbageCollect': {'description': 'CAASApplicationGarbageCollect '
-                                                                     'cleans up '
-                                                                     'units that '
-                                                                     'have gone '
-                                                                     'away '
-                                                                     'permanently.\n'
-                                                                     'Only '
-                                                                     'observed '
-                                                                     'units will '
-                                                                     'be deleted '
-                                                                     'as new units '
-                                                                     'could have '
-                                                                     'surfaced '
-                                                                     'between\n'
-                                                                     'the '
-                                                                     'capturing of '
-                                                                     'kuberentes '
-                                                                     'pod '
-                                                                     'state/application '
-                                                                     'state and '
-                                                                     'this call.',
-                                                      'properties': {'Params': {'$ref': '#/definitions/CAASApplicationGarbageCollectArgs'},
-                                                                     'Result': {'$ref': '#/definitions/ErrorResults'}},
-                                                      'type': 'object'},
                     'CharmInfo': {'description': 'CharmInfo returns information '
                                                  'about the requested charm.',
                                   'properties': {'Params': {'$ref': '#/definitions/CharmURL'},
                                                  'Result': {'$ref': '#/definitions/Charm'}},
                                   'type': 'object'},
                     'ClearApplicationsResources': {'description': 'ClearApplicationsResources '
                                                                   'clears the '
@@ -1144,26 +1252,46 @@
                                                                   'applications '
                                                                   'still have '
                                                                   'resources in '
                                                                   'the cluster.',
                                                    'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                                                   'Result': {'$ref': '#/definitions/ErrorResults'}},
                                                    'type': 'object'},
+                    'DestroyUnits': {'description': 'DestroyUnits is responsible '
+                                                    'for scaling down a set of '
+                                                    'units on the this\n'
+                                                    'Application.',
+                                     'properties': {'Params': {'$ref': '#/definitions/DestroyUnitsParams'},
+                                                    'Result': {'$ref': '#/definitions/DestroyUnitResults'}},
+                                     'type': 'object'},
                     'Life': {'description': 'Life returns the life status of every '
                                             'supplied entity, where available.',
                              'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                             'Result': {'$ref': '#/definitions/LifeResults'}},
                              'type': 'object'},
+                    'ProvisionerConfig': {'description': 'ProvisionerConfig '
+                                                         'returns the '
+                                                         "provisioner's "
+                                                         'configuration.',
+                                          'properties': {'Result': {'$ref': '#/definitions/CAASApplicationProvisionerConfigResult'}},
+                                          'type': 'object'},
                     'ProvisioningInfo': {'description': 'ProvisioningInfo returns '
                                                         'the info needed to '
                                                         'provision a caas '
                                                         'application.',
                                          'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                                         'Result': {'$ref': '#/definitions/CAASApplicationProvisioningInfoResults'}},
                                          'type': 'object'},
+                    'ProvisioningState': {'description': 'ProvisioningState '
+                                                         'returns the provisioning '
+                                                         'state for the '
+                                                         'application.',
+                                          'properties': {'Params': {'$ref': '#/definitions/Entity'},
+                                                         'Result': {'$ref': '#/definitions/CAASApplicationProvisioningStateResult'}},
+                                          'type': 'object'},
                     'Remove': {'description': 'Remove removes every given entity '
                                               'from state, calling EnsureDead\n'
                                               'first, then Remove. It will fail if '
                                               'the entity is not present.',
                                'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                               'Result': {'$ref': '#/definitions/ErrorResults'}},
                                'type': 'object'},
@@ -1175,14 +1303,21 @@
                                           'type': 'object'},
                     'SetPasswords': {'description': 'SetPasswords sets the given '
                                                     'password for each supplied '
                                                     'entity, if possible.',
                                      'properties': {'Params': {'$ref': '#/definitions/EntityPasswords'},
                                                     'Result': {'$ref': '#/definitions/ErrorResults'}},
                                      'type': 'object'},
+                    'SetProvisioningState': {'description': 'SetProvisioningState '
+                                                            'sets the provisioning '
+                                                            'state for the '
+                                                            'application.',
+                                             'properties': {'Params': {'$ref': '#/definitions/CAASApplicationProvisioningStateArg'},
+                                                            'Result': {'$ref': '#/definitions/ErrorResult'}},
+                                             'type': 'object'},
                     'Units': {'description': 'Units returns all the units for each '
                                              'application specified.',
                               'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                              'Result': {'$ref': '#/definitions/CAASUnitsResults'}},
                               'type': 'object'},
                     'UpdateApplicationsUnits': {'description': 'UpdateApplicationsUnits '
                                                                'updates the Juju '
@@ -1272,39 +1407,14 @@
                    params=_params)
         _params['entities'] = entities
         reply = await self.rpc(msg)
         return reply
 
 
 
-    @ReturnMapping(ErrorResults)
-    async def CAASApplicationGarbageCollect(self, args=None):
-        '''
-        CAASApplicationGarbageCollect cleans up units that have gone away permanently.
-        Only observed units will be deleted as new units could have surfaced between
-        the capturing of kuberentes pod state/application state and this call.
-
-        args : typing.Sequence[~CAASApplicationGarbageCollectArg]
-        Returns -> ErrorResults
-        '''
-        if args is not None and not isinstance(args, (bytes, str, list)):
-            raise Exception("Expected args to be a Sequence, received: {}".format(type(args)))
-
-        # map input types to rpc msg
-        _params = dict()
-        msg = dict(type='CAASApplicationProvisioner',
-                   request='CAASApplicationGarbageCollect',
-                   version=1,
-                   params=_params)
-        _params['args'] = args
-        reply = await self.rpc(msg)
-        return reply
-
-
-
     @ReturnMapping(Charm)
     async def CharmInfo(self, url=None):
         '''
         CharmInfo returns information about the requested charm.
 
         url : str
         Returns -> Charm
@@ -1344,14 +1454,38 @@
                    params=_params)
         _params['entities'] = entities
         reply = await self.rpc(msg)
         return reply
 
 
 
+    @ReturnMapping(DestroyUnitResults)
+    async def DestroyUnits(self, units=None):
+        '''
+        DestroyUnits is responsible for scaling down a set of units on the this
+        Application.
+
+        units : typing.Sequence[~DestroyUnitParams]
+        Returns -> DestroyUnitResults
+        '''
+        if units is not None and not isinstance(units, (bytes, str, list)):
+            raise Exception("Expected units to be a Sequence, received: {}".format(type(units)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='CAASApplicationProvisioner',
+                   request='DestroyUnits',
+                   version=1,
+                   params=_params)
+        _params['units'] = units
+        reply = await self.rpc(msg)
+        return reply
+
+
+
     @ReturnMapping(LifeResults)
     async def Life(self, entities=None):
         '''
         Life returns the life status of every supplied entity, where available.
 
         entities : typing.Sequence[~Entity]
         Returns -> LifeResults
@@ -1367,14 +1501,35 @@
                    params=_params)
         _params['entities'] = entities
         reply = await self.rpc(msg)
         return reply
 
 
 
+    @ReturnMapping(CAASApplicationProvisionerConfigResult)
+    async def ProvisionerConfig(self):
+        '''
+        ProvisionerConfig returns the provisioner's configuration.
+
+
+        Returns -> CAASApplicationProvisionerConfigResult
+        '''
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='CAASApplicationProvisioner',
+                   request='ProvisionerConfig',
+                   version=1,
+                   params=_params)
+
+        reply = await self.rpc(msg)
+        return reply
+
+
+
     @ReturnMapping(CAASApplicationProvisioningInfoResults)
     async def ProvisioningInfo(self, entities=None):
         '''
         ProvisioningInfo returns the info needed to provision a caas application.
 
         entities : typing.Sequence[~Entity]
         Returns -> CAASApplicationProvisioningInfoResults
@@ -1390,14 +1545,37 @@
                    params=_params)
         _params['entities'] = entities
         reply = await self.rpc(msg)
         return reply
 
 
 
+    @ReturnMapping(CAASApplicationProvisioningStateResult)
+    async def ProvisioningState(self, tag=None):
+        '''
+        ProvisioningState returns the provisioning state for the application.
+
+        tag : str
+        Returns -> CAASApplicationProvisioningStateResult
+        '''
+        if tag is not None and not isinstance(tag, (bytes, str)):
+            raise Exception("Expected tag to be a str, received: {}".format(type(tag)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='CAASApplicationProvisioner',
+                   request='ProvisioningState',
+                   version=1,
+                   params=_params)
+        _params['tag'] = tag
+        reply = await self.rpc(msg)
+        return reply
+
+
+
     @ReturnMapping(ErrorResults)
     async def Remove(self, entities=None):
         '''
         Remove removes every given entity from state, calling EnsureDead
         first, then Remove. It will fail if the entity is not present.
 
         entities : typing.Sequence[~Entity]
@@ -1460,14 +1638,42 @@
                    params=_params)
         _params['changes'] = changes
         reply = await self.rpc(msg)
         return reply
 
 
 
+    @ReturnMapping(ErrorResult)
+    async def SetProvisioningState(self, application=None, provisioning_state=None):
+        '''
+        SetProvisioningState sets the provisioning state for the application.
+
+        application : Entity
+        provisioning_state : CAASApplicationProvisioningState
+        Returns -> ErrorResult
+        '''
+        if application is not None and not isinstance(application, (dict, Entity)):
+            raise Exception("Expected application to be a Entity, received: {}".format(type(application)))
+
+        if provisioning_state is not None and not isinstance(provisioning_state, (dict, CAASApplicationProvisioningState)):
+            raise Exception("Expected provisioning_state to be a CAASApplicationProvisioningState, received: {}".format(type(provisioning_state)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='CAASApplicationProvisioner',
+                   request='SetProvisioningState',
+                   version=1,
+                   params=_params)
+        _params['application'] = application
+        _params['provisioning-state'] = provisioning_state
+        reply = await self.rpc(msg)
+        return reply
+
+
+
     @ReturnMapping(CAASUnitsResults)
     async def Units(self, entities=None):
         '''
         Units returns all the units for each application specified.
 
         entities : typing.Sequence[~Entity]
         Returns -> CAASUnitsResults
@@ -9810,14 +10016,198 @@
 
         from .facade import TypeEncoder
         reply = await self.connection.rpc(msg, encoder=TypeEncoder)
         return reply
 
 
 
+class SecretsDrainFacade(Type):
+    name = 'SecretsDrain'
+    version = 1
+    schema =     {'definitions': {'ChangeSecretBackendArg': {'additionalProperties': False,
+                                                'properties': {'content': {'$ref': '#/definitions/SecretContentParams'},
+                                                               'revision': {'type': 'integer'},
+                                                               'uri': {'type': 'string'}},
+                                                'required': ['uri', 'revision'],
+                                                'type': 'object'},
+                     'ChangeSecretBackendArgs': {'additionalProperties': False,
+                                                 'properties': {'args': {'items': {'$ref': '#/definitions/ChangeSecretBackendArg'},
+                                                                         'type': 'array'}},
+                                                 'required': ['args'],
+                                                 'type': 'object'},
+                     'Error': {'additionalProperties': False,
+                               'properties': {'code': {'type': 'string'},
+                                              'info': {'patternProperties': {'.*': {'additionalProperties': True,
+                                                                                    'type': 'object'}},
+                                                       'type': 'object'},
+                                              'message': {'type': 'string'}},
+                               'required': ['message', 'code'],
+                               'type': 'object'},
+                     'ErrorResult': {'additionalProperties': False,
+                                     'properties': {'error': {'$ref': '#/definitions/Error'}},
+                                     'type': 'object'},
+                     'ErrorResults': {'additionalProperties': False,
+                                      'properties': {'results': {'items': {'$ref': '#/definitions/ErrorResult'},
+                                                                 'type': 'array'}},
+                                      'required': ['results'],
+                                      'type': 'object'},
+                     'ListSecretResult': {'additionalProperties': False,
+                                          'properties': {'create-time': {'format': 'date-time',
+                                                                         'type': 'string'},
+                                                         'description': {'type': 'string'},
+                                                         'label': {'type': 'string'},
+                                                         'latest-expire-time': {'format': 'date-time',
+                                                                                'type': 'string'},
+                                                         'latest-revision': {'type': 'integer'},
+                                                         'next-rotate-time': {'format': 'date-time',
+                                                                              'type': 'string'},
+                                                         'owner-tag': {'type': 'string'},
+                                                         'revisions': {'items': {'$ref': '#/definitions/SecretRevision'},
+                                                                       'type': 'array'},
+                                                         'rotate-policy': {'type': 'string'},
+                                                         'update-time': {'format': 'date-time',
+                                                                         'type': 'string'},
+                                                         'uri': {'type': 'string'},
+                                                         'value': {'$ref': '#/definitions/SecretValueResult'},
+                                                         'version': {'type': 'integer'}},
+                                          'required': ['uri',
+                                                       'version',
+                                                       'owner-tag',
+                                                       'latest-revision',
+                                                       'create-time',
+                                                       'update-time',
+                                                       'revisions'],
+                                          'type': 'object'},
+                     'ListSecretResults': {'additionalProperties': False,
+                                           'properties': {'results': {'items': {'$ref': '#/definitions/ListSecretResult'},
+                                                                      'type': 'array'}},
+                                           'required': ['results'],
+                                           'type': 'object'},
+                     'NotifyWatchResult': {'additionalProperties': False,
+                                           'properties': {'NotifyWatcherId': {'type': 'string'},
+                                                          'error': {'$ref': '#/definitions/Error'}},
+                                           'required': ['NotifyWatcherId'],
+                                           'type': 'object'},
+                     'SecretContentParams': {'additionalProperties': False,
+                                             'properties': {'data': {'patternProperties': {'.*': {'type': 'string'}},
+                                                                     'type': 'object'},
+                                                            'value-ref': {'$ref': '#/definitions/SecretValueRef'}},
+                                             'type': 'object'},
+                     'SecretRevision': {'additionalProperties': False,
+                                        'properties': {'backend-name': {'type': 'string'},
+                                                       'create-time': {'format': 'date-time',
+                                                                       'type': 'string'},
+                                                       'expire-time': {'format': 'date-time',
+                                                                       'type': 'string'},
+                                                       'revision': {'type': 'integer'},
+                                                       'update-time': {'format': 'date-time',
+                                                                       'type': 'string'},
+                                                       'value-ref': {'$ref': '#/definitions/SecretValueRef'}},
+                                        'required': ['revision'],
+                                        'type': 'object'},
+                     'SecretValueRef': {'additionalProperties': False,
+                                        'properties': {'backend-id': {'type': 'string'},
+                                                       'revision-id': {'type': 'string'}},
+                                        'required': ['backend-id', 'revision-id'],
+                                        'type': 'object'},
+                     'SecretValueResult': {'additionalProperties': False,
+                                           'properties': {'data': {'patternProperties': {'.*': {'type': 'string'}},
+                                                                   'type': 'object'},
+                                                          'error': {'$ref': '#/definitions/Error'}},
+                                           'type': 'object'}},
+     'properties': {'ChangeSecretBackend': {'description': 'ChangeSecretBackend '
+                                                           'updates the backend '
+                                                           'for the specified '
+                                                           'secret after migration '
+                                                           'done.',
+                                            'properties': {'Params': {'$ref': '#/definitions/ChangeSecretBackendArgs'},
+                                                           'Result': {'$ref': '#/definitions/ErrorResults'}},
+                                            'type': 'object'},
+                    'GetSecretsToDrain': {'description': 'GetSecretsToDrain '
+                                                         'returns metadata for the '
+                                                         'secrets that need to be '
+                                                         'drained.',
+                                          'properties': {'Result': {'$ref': '#/definitions/ListSecretResults'}},
+                                          'type': 'object'},
+                    'WatchSecretBackendChanged': {'description': 'WatchSecretBackendChanged '
+                                                                 'sets up a '
+                                                                 'watcher to '
+                                                                 'notify of '
+                                                                 'changes to the '
+                                                                 'secret backend.',
+                                                  'properties': {'Result': {'$ref': '#/definitions/NotifyWatchResult'}},
+                                                  'type': 'object'}},
+     'type': 'object'}
+    
+
+    @ReturnMapping(ErrorResults)
+    async def ChangeSecretBackend(self, args=None):
+        '''
+        ChangeSecretBackend updates the backend for the specified secret after migration done.
+
+        args : typing.Sequence[~ChangeSecretBackendArg]
+        Returns -> ErrorResults
+        '''
+        if args is not None and not isinstance(args, (bytes, str, list)):
+            raise Exception("Expected args to be a Sequence, received: {}".format(type(args)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsDrain',
+                   request='ChangeSecretBackend',
+                   version=1,
+                   params=_params)
+        _params['args'] = args
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(ListSecretResults)
+    async def GetSecretsToDrain(self):
+        '''
+        GetSecretsToDrain returns metadata for the secrets that need to be drained.
+
+
+        Returns -> ListSecretResults
+        '''
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsDrain',
+                   request='GetSecretsToDrain',
+                   version=1,
+                   params=_params)
+
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(NotifyWatchResult)
+    async def WatchSecretBackendChanged(self):
+        '''
+        WatchSecretBackendChanged sets up a watcher to notify of changes to the secret backend.
+
+
+        Returns -> NotifyWatchResult
+        '''
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsDrain',
+                   request='WatchSecretBackendChanged',
+                   version=1,
+                   params=_params)
+
+        reply = await self.rpc(msg)
+        return reply
+
+
+
 class SecretsFacade(Type):
     name = 'Secrets'
     version = 1
     schema =     {'definitions': {'Error': {'additionalProperties': False,
                                'properties': {'code': {'type': 'string'},
                                               'info': {'patternProperties': {'.*': {'additionalProperties': True,
                                                                                     'type': 'object'}},
@@ -10772,14 +11162,109 @@
                    params=_params)
         _params['entities'] = entities
         reply = await self.rpc(msg)
         return reply
 
 
 
+class SecretsRevisionWatcherFacade(Type):
+    name = 'SecretsRevisionWatcher'
+    version = 1
+    schema =     {'definitions': {'Error': {'additionalProperties': False,
+                               'properties': {'code': {'type': 'string'},
+                                              'info': {'patternProperties': {'.*': {'additionalProperties': True,
+                                                                                    'type': 'object'}},
+                                                       'type': 'object'},
+                                              'message': {'type': 'string'}},
+                               'required': ['message', 'code'],
+                               'type': 'object'},
+                     'SecretRevisionChange': {'additionalProperties': False,
+                                              'properties': {'revision': {'type': 'integer'},
+                                                             'uri': {'type': 'string'}},
+                                              'required': ['uri', 'revision'],
+                                              'type': 'object'},
+                     'SecretRevisionWatchResult': {'additionalProperties': False,
+                                                   'properties': {'changes': {'items': {'$ref': '#/definitions/SecretRevisionChange'},
+                                                                              'type': 'array'},
+                                                                  'error': {'$ref': '#/definitions/Error'},
+                                                                  'watcher-id': {'type': 'string'}},
+                                                   'required': ['watcher-id',
+                                                                'changes'],
+                                                   'type': 'object'}},
+     'properties': {'Next': {'description': 'Next returns when a change has '
+                                            'occurred to an entity of the\n'
+                                            'collection being watched since the '
+                                            'most recent call to Next\n'
+                                            'or the Watch call that created the '
+                                            'srvSecretRotationWatcher.',
+                             'properties': {'Result': {'$ref': '#/definitions/SecretRevisionWatchResult'}},
+                             'type': 'object'},
+                    'Stop': {'description': 'Stop stops the watcher.',
+                             'type': 'object'}},
+     'type': 'object'}
+    
+
+    @ReturnMapping(SecretRevisionWatchResult)
+    async def Next(self):
+        '''
+        Next returns when a change has occurred to an entity of the
+        collection being watched since the most recent call to Next
+        or the Watch call that created the srvSecretRotationWatcher.
+
+
+        Returns -> SecretRevisionWatchResult
+        '''
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsRevisionWatcher',
+                   request='Next',
+                   version=1,
+                   params=_params)
+
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(None)
+    async def Stop(self):
+        '''
+        Stop stops the watcher.
+
+
+        Returns -> None
+        '''
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsRevisionWatcher',
+                   request='Stop',
+                   version=1,
+                   params=_params)
+
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    async def rpc(self, msg):
+        '''
+        Patch rpc method to add Id.
+        '''
+        if not hasattr(self, 'Id'):
+            raise RuntimeError('Missing "Id" field')
+        msg['Id'] = id
+
+        from .facade import TypeEncoder
+        reply = await self.connection.rpc(msg, encoder=TypeEncoder)
+        return reply
+
+
+
 class SecretsTriggerWatcherFacade(Type):
     name = 'SecretsTriggerWatcher'
     version = 1
     schema =     {'definitions': {'Error': {'additionalProperties': False,
                                'properties': {'code': {'type': 'string'},
                                               'info': {'patternProperties': {'.*': {'additionalProperties': True,
                                                                                     'type': 'object'}},
```

### Comparing `juju-3.1.2.0/juju/client/_client10.py` & `juju-3.2.0.0/juju/client/_client10.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,14 +248,15 @@
                                                    'type': 'object'},
                      'Value': {'additionalProperties': False,
                                'properties': {'allocate-public-ip': {'type': 'boolean'},
                                               'arch': {'type': 'string'},
                                               'container': {'type': 'string'},
                                               'cores': {'type': 'integer'},
                                               'cpu-power': {'type': 'integer'},
+                                              'image-id': {'type': 'string'},
                                               'instance-role': {'type': 'string'},
                                               'instance-type': {'type': 'string'},
                                               'mem': {'type': 'integer'},
                                               'root-disk': {'type': 'integer'},
                                               'root-disk-source': {'type': 'string'},
                                               'spaces': {'items': {'type': 'string'},
                                                          'type': 'array'},
```

### Comparing `juju-3.1.2.0/juju/client/_client11.py` & `juju-3.2.0.0/juju/client/_client11.py`

 * *Files 0% similar despite different names*

```diff
@@ -1748,14 +1748,15 @@
                                         'type': 'object'},
                      'Value': {'additionalProperties': False,
                                'properties': {'allocate-public-ip': {'type': 'boolean'},
                                               'arch': {'type': 'string'},
                                               'container': {'type': 'string'},
                                               'cores': {'type': 'integer'},
                                               'cpu-power': {'type': 'integer'},
+                                              'image-id': {'type': 'string'},
                                               'instance-role': {'type': 'string'},
                                               'instance-type': {'type': 'string'},
                                               'mem': {'type': 'integer'},
                                               'root-disk': {'type': 'integer'},
                                               'root-disk-source': {'type': 'string'},
                                               'spaces': {'items': {'type': 'string'},
                                                          'type': 'array'},
```

### Comparing `juju-3.1.2.0/juju/client/_client12.py` & `juju-3.2.0.0/juju/client/_client12.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_client13.py` & `juju-3.2.0.0/juju/client/_client13.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_client14.py` & `juju-3.2.0.0/juju/client/_client14.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_client15.py` & `juju-3.2.0.0/juju/client/_client15.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_client16.py` & `juju-3.2.0.0/juju/client/_client16.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_client17.py` & `juju-3.2.0.0/juju/client/_client17.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_client18.py` & `juju-3.2.0.0/juju/client/_client18.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,19 +258,14 @@
                                             'required': ['applications'],
                                             'type': 'object'},
                      'Base': {'additionalProperties': False,
                               'properties': {'channel': {'type': 'string'},
                                              'name': {'type': 'string'}},
                               'required': ['name', 'channel'],
                               'type': 'object'},
-                     'Channel': {'additionalProperties': False,
-                                 'properties': {'branch': {'type': 'string'},
-                                                'risk': {'type': 'string'},
-                                                'track': {'type': 'string'}},
-                                 'type': 'object'},
                      'CharmOrigin': {'additionalProperties': False,
                                      'properties': {'architecture': {'type': 'string'},
                                                     'base': {'$ref': '#/definitions/Base'},
                                                     'branch': {'type': 'string'},
                                                     'hash': {'type': 'string'},
                                                     'id': {'type': 'string'},
                                                     'instance-key': {'type': 'string'},
@@ -330,14 +325,15 @@
                                                     'Size': {'type': 'integer'}},
                                      'required': ['Pool', 'Size', 'Count'],
                                      'type': 'object'},
                      'ConsumeApplicationArg': {'additionalProperties': False,
                                                'properties': {'ApplicationOfferDetails': {'$ref': '#/definitions/ApplicationOfferDetails'},
                                                               'application-alias': {'type': 'string'},
                                                               'application-description': {'type': 'string'},
+                                                              'auth-token': {'type': 'string'},
                                                               'bindings': {'patternProperties': {'.*': {'type': 'string'}},
                                                                            'type': 'object'},
                                                               'endpoints': {'items': {'$ref': '#/definitions/RemoteEndpoint'},
                                                                             'type': 'array'},
                                                               'external-controller': {'$ref': '#/definitions/ExternalControllerInfo'},
                                                               'macaroon': {'$ref': '#/definitions/Macaroon'},
                                                               'offer-name': {'type': 'string'},
@@ -359,62 +355,66 @@
                                                 'properties': {'args': {'items': {'$ref': '#/definitions/ConsumeApplicationArg'},
                                                                         'type': 'array'}},
                                                 'type': 'object'},
                      'DeployFromRepositoryArg': {'additionalProperties': False,
                                                  'properties': {'ApplicationName': {'type': 'string'},
                                                                 'AttachStorage': {'items': {'type': 'string'},
                                                                                   'type': 'array'},
-                                                                'Base': {'$ref': '#/definitions/Base'},
-                                                                'Channel': {'$ref': '#/definitions/Channel'},
                                                                 'CharmName': {'type': 'string'},
                                                                 'ConfigYAML': {'type': 'string'},
                                                                 'Cons': {'$ref': '#/definitions/Value'},
                                                                 'Devices': {'patternProperties': {'.*': {'$ref': '#/definitions/Constraints'}},
                                                                             'type': 'object'},
                                                                 'DryRun': {'type': 'boolean'},
-                                                                'EndpointBindings': {'patternProperties': {'.*': {'type': 'string'}},
-                                                                                     'type': 'object'},
-                                                                'Force': {'type': 'boolean'},
-                                                                'NumUnits': {'type': 'integer'},
                                                                 'Placement': {'items': {'$ref': '#/definitions/Placement'},
                                                                               'type': 'array'},
-                                                                'Resources': {'patternProperties': {'.*': {'type': 'string'}},
-                                                                              'type': 'object'},
-                                                                'Revision': {'type': 'integer'},
                                                                 'Storage': {'patternProperties': {'.*': {'$ref': '#/definitions/Constraints'}},
                                                                             'type': 'object'},
-                                                                'Trust': {'type': 'boolean'}},
+                                                                'Trust': {'type': 'boolean'},
+                                                                'base': {'$ref': '#/definitions/Base'},
+                                                                'channel': {'type': 'string'},
+                                                                'endpoint-bindings': {'patternProperties': {'.*': {'type': 'string'}},
+                                                                                      'type': 'object'},
+                                                                'force': {'type': 'boolean'},
+                                                                'num-units': {'type': 'integer'},
+                                                                'resources': {'patternProperties': {'.*': {'type': 'string'}},
+                                                                              'type': 'object'},
+                                                                'revision': {'type': 'integer'}},
                                                  'required': ['CharmName',
                                                               'ApplicationName',
                                                               'AttachStorage',
-                                                              'Base',
-                                                              'Channel',
                                                               'ConfigYAML',
                                                               'Cons',
                                                               'Devices',
                                                               'DryRun',
-                                                              'EndpointBindings',
-                                                              'Force',
-                                                              'NumUnits',
                                                               'Placement',
-                                                              'Revision',
-                                                              'Resources',
                                                               'Storage',
                                                               'Trust'],
                                                  'type': 'object'},
                      'DeployFromRepositoryArgs': {'additionalProperties': False,
                                                   'properties': {'Args': {'items': {'$ref': '#/definitions/DeployFromRepositoryArg'},
                                                                           'type': 'array'}},
                                                   'required': ['Args'],
                                                   'type': 'object'},
+                     'DeployFromRepositoryInfo': {'additionalProperties': False,
+                                                  'properties': {'architecture': {'type': 'string'},
+                                                                 'base': {'$ref': '#/definitions/Base'},
+                                                                 'channel': {'type': 'string'},
+                                                                 'effective-channel': {'type': 'string'},
+                                                                 'name': {'type': 'string'},
+                                                                 'revision': {'type': 'integer'}},
+                                                  'required': ['architecture',
+                                                               'channel',
+                                                               'name',
+                                                               'revision'],
+                                                  'type': 'object'},
                      'DeployFromRepositoryResult': {'additionalProperties': False,
                                                     'properties': {'Errors': {'items': {'$ref': '#/definitions/Error'},
                                                                               'type': 'array'},
-                                                                   'Info': {'items': {'type': 'string'},
-                                                                            'type': 'array'},
+                                                                   'Info': {'$ref': '#/definitions/DeployFromRepositoryInfo'},
                                                                    'PendingResourceUploads': {'items': {'$ref': '#/definitions/PendingResourceUpload'},
                                                                                               'type': 'array'}},
                                                     'required': ['Errors',
                                                                  'Info',
                                                                  'PendingResourceUploads'],
                                                     'type': 'object'},
                      'DeployFromRepositoryResults': {'additionalProperties': False,
@@ -565,19 +565,19 @@
                                           'required': ['user',
                                                        'display-name',
                                                        'access'],
                                           'type': 'object'},
                      'PendingResourceUpload': {'additionalProperties': False,
                                                'properties': {'Filename': {'type': 'string'},
                                                               'Name': {'type': 'string'},
-                                                              'PendingID': {'type': 'string'},
-                                                              'Type': {'type': 'string'}},
+                                                              'Type': {'type': 'string'},
+                                                              'pending-id': {'type': 'string'}},
                                                'required': ['Name',
                                                             'Filename',
-                                                            'PendingID',
+                                                            'pending-id',
                                                             'Type'],
                                                'type': 'object'},
                      'Placement': {'additionalProperties': False,
                                    'properties': {'directive': {'type': 'string'},
                                                   'scope': {'type': 'string'}},
                                    'required': ['scope', 'directive'],
                                    'type': 'object'},
@@ -730,14 +730,15 @@
                                            'type': 'object'},
                      'Value': {'additionalProperties': False,
                                'properties': {'allocate-public-ip': {'type': 'boolean'},
                                               'arch': {'type': 'string'},
                                               'container': {'type': 'string'},
                                               'cores': {'type': 'integer'},
                                               'cpu-power': {'type': 'integer'},
+                                              'image-id': {'type': 'string'},
                                               'instance-role': {'type': 'string'},
                                               'instance-type': {'type': 'string'},
                                               'mem': {'type': 'integer'},
                                               'root-disk': {'type': 'integer'},
                                               'root-disk-source': {'type': 'string'},
                                               'spaces': {'items': {'type': 'string'},
                                                          'type': 'array'},
@@ -2532,32 +2533,42 @@
                                             'required': ['mode'],
                                             'type': 'object'},
                      'ResolvedModeResults': {'additionalProperties': False,
                                              'properties': {'results': {'items': {'$ref': '#/definitions/ResolvedModeResult'},
                                                                         'type': 'array'}},
                                              'required': ['results'],
                                              'type': 'object'},
+                     'SecretBackendArgs': {'additionalProperties': False,
+                                           'properties': {'backend-ids': {'items': {'type': 'string'},
+                                                                          'type': 'array'}},
+                                           'required': ['backend-ids'],
+                                           'type': 'object'},
                      'SecretBackendConfig': {'additionalProperties': False,
                                              'properties': {'params': {'patternProperties': {'.*': {'additionalProperties': True,
                                                                                                     'type': 'object'}},
                                                                        'type': 'object'},
                                                             'type': {'type': 'string'}},
                                              'required': ['type'],
                                              'type': 'object'},
+                     'SecretBackendConfigResult': {'additionalProperties': False,
+                                                   'properties': {'config': {'$ref': '#/definitions/SecretBackendConfig'},
+                                                                  'draining': {'type': 'boolean'},
+                                                                  'model-controller': {'type': 'string'},
+                                                                  'model-name': {'type': 'string'},
+                                                                  'model-uuid': {'type': 'string'}},
+                                                   'required': ['model-controller',
+                                                                'model-uuid',
+                                                                'model-name',
+                                                                'draining'],
+                                                   'type': 'object'},
                      'SecretBackendConfigResults': {'additionalProperties': False,
                                                     'properties': {'active-id': {'type': 'string'},
-                                                                   'configs': {'patternProperties': {'.*': {'$ref': '#/definitions/SecretBackendConfig'}},
-                                                                               'type': 'object'},
-                                                                   'model-controller': {'type': 'string'},
-                                                                   'model-name': {'type': 'string'},
-                                                                   'model-uuid': {'type': 'string'}},
-                                                    'required': ['model-controller',
-                                                                 'model-uuid',
-                                                                 'model-name',
-                                                                 'active-id'],
+                                                                   'results': {'patternProperties': {'.*': {'$ref': '#/definitions/SecretBackendConfigResult'}},
+                                                                               'type': 'object'}},
+                                                    'required': ['active-id'],
                                                     'type': 'object'},
                      'SecretConsumerInfoResult': {'additionalProperties': False,
                                                   'properties': {'error': {'$ref': '#/definitions/Error'},
                                                                  'label': {'type': 'string'},
                                                                  'revision': {'type': 'integer'}},
                                                   'required': ['revision', 'label'],
                                                   'type': 'object'},
@@ -2568,16 +2579,18 @@
                                                    'type': 'object'},
                      'SecretContentParams': {'additionalProperties': False,
                                              'properties': {'data': {'patternProperties': {'.*': {'type': 'string'}},
                                                                      'type': 'object'},
                                                             'value-ref': {'$ref': '#/definitions/SecretValueRef'}},
                                              'type': 'object'},
                      'SecretContentResult': {'additionalProperties': False,
-                                             'properties': {'content': {'$ref': '#/definitions/SecretContentParams'},
-                                                            'error': {'$ref': '#/definitions/Error'}},
+                                             'properties': {'backend-config': {'$ref': '#/definitions/SecretBackendConfigResult'},
+                                                            'content': {'$ref': '#/definitions/SecretContentParams'},
+                                                            'error': {'$ref': '#/definitions/Error'},
+                                                            'latest-revision': {'type': 'integer'}},
                                              'required': ['content'],
                                              'type': 'object'},
                      'SecretContentResults': {'additionalProperties': False,
                                               'properties': {'results': {'items': {'$ref': '#/definitions/SecretContentResult'},
                                                                          'type': 'array'}},
                                               'required': ['results'],
                                               'type': 'object'},
@@ -3118,21 +3131,22 @@
                                      'type': 'object'},
                     'GetRawK8sSpec': {'description': 'GetRawK8sSpec gets the raw '
                                                      'k8s specs for a set of '
                                                      'applications.',
                                       'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                                      'Result': {'$ref': '#/definitions/StringResults'}},
                                       'type': 'object'},
-                    'GetSecretBackendConfig': {'description': 'GetSecretBackendConfig '
-                                                              'gets the config '
-                                                              'needed to create a '
-                                                              'client to secret '
-                                                              'backends.',
-                                               'properties': {'Result': {'$ref': '#/definitions/SecretBackendConfigResults'}},
-                                               'type': 'object'},
+                    'GetSecretBackendConfigs': {'description': 'GetSecretBackendConfigs '
+                                                               'gets the config '
+                                                               'needed to create a '
+                                                               'client to secret '
+                                                               'backends.',
+                                                'properties': {'Params': {'$ref': '#/definitions/SecretBackendArgs'},
+                                                               'Result': {'$ref': '#/definitions/SecretBackendConfigResults'}},
+                                                'type': 'object'},
                     'GetSecretContentInfo': {'description': 'GetSecretContentInfo '
                                                             'returns the secret '
                                                             'values for the '
                                                             'specified secrets.',
                                              'properties': {'Params': {'$ref': '#/definitions/GetSecretContentArgs'},
                                                             'Result': {'$ref': '#/definitions/SecretContentResults'}},
                                              'type': 'object'},
@@ -3147,22 +3161,14 @@
                                                                     'for the '
                                                                     'specified '
                                                                     'secret '
                                                                     'revisions.',
                                                      'properties': {'Params': {'$ref': '#/definitions/SecretRevisionArg'},
                                                                     'Result': {'$ref': '#/definitions/SecretContentResults'}},
                                                      'type': 'object'},
-                    'GetSecretStoreConfig': {'description': 'GetSecretStoreConfig '
-                                                            'is for 3.0.x agents.\n'
-                                                            'TODO(wallyworld) - '
-                                                            'remove when we auto '
-                                                            'upgrade migrated '
-                                                            'models.',
-                                             'properties': {'Result': {'$ref': '#/definitions/SecretBackendConfig'}},
-                                             'type': 'object'},
                     'GoalStates': {'description': 'GoalStates returns information '
                                                   'of charm units and relations.',
                                    'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                                   'Result': {'$ref': '#/definitions/GoalStateResults'}},
                                    'type': 'object'},
                     'HasSubordinates': {'description': 'HasSubordinates returns '
                                                        'the whether each given '
@@ -4587,29 +4593,31 @@
         _params['entities'] = entities
         reply = await self.rpc(msg)
         return reply
 
 
 
     @ReturnMapping(SecretBackendConfigResults)
-    async def GetSecretBackendConfig(self):
+    async def GetSecretBackendConfigs(self, backend_ids=None):
         '''
-        GetSecretBackendConfig gets the config needed to create a client to secret backends.
-
+        GetSecretBackendConfigs gets the config needed to create a client to secret backends.
 
+        backend_ids : typing.Sequence[str]
         Returns -> SecretBackendConfigResults
         '''
+        if backend_ids is not None and not isinstance(backend_ids, (bytes, str, list)):
+            raise Exception("Expected backend_ids to be a Sequence, received: {}".format(type(backend_ids)))
 
         # map input types to rpc msg
         _params = dict()
         msg = dict(type='Uniter',
-                   request='GetSecretBackendConfig',
+                   request='GetSecretBackendConfigs',
                    version=18,
                    params=_params)
-
+        _params['backend-ids'] = backend_ids
         reply = await self.rpc(msg)
         return reply
 
 
 
     @ReturnMapping(SecretContentResults)
     async def GetSecretContentInfo(self, args=None):
@@ -4684,36 +4692,14 @@
         _params['revisions'] = revisions
         _params['uri'] = uri
         reply = await self.rpc(msg)
         return reply
 
 
 
-    @ReturnMapping(SecretBackendConfig)
-    async def GetSecretStoreConfig(self):
-        '''
-        GetSecretStoreConfig is for 3.0.x agents.
-        TODO(wallyworld) - remove when we auto upgrade migrated models.
-
-
-        Returns -> SecretBackendConfig
-        '''
-
-        # map input types to rpc msg
-        _params = dict()
-        msg = dict(type='Uniter',
-                   request='GetSecretStoreConfig',
-                   version=18,
-                   params=_params)
-
-        reply = await self.rpc(msg)
-        return reply
-
-
-
     @ReturnMapping(GoalStateResults)
     async def GoalStates(self, entities=None):
         '''
         GoalStates returns information of charm units and relations.
 
         entities : typing.Sequence[~Entity]
         Returns -> GoalStateResults
```

### Comparing `juju-3.1.2.0/juju/client/_client2.py` & `juju-3.2.0.0/juju/client/_client2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1095,14 +1095,15 @@
                                                     'type': 'object'},
                      'Value': {'additionalProperties': False,
                                'properties': {'allocate-public-ip': {'type': 'boolean'},
                                               'arch': {'type': 'string'},
                                               'container': {'type': 'string'},
                                               'cores': {'type': 'integer'},
                                               'cpu-power': {'type': 'integer'},
+                                              'image-id': {'type': 'string'},
                                               'instance-role': {'type': 'string'},
                                               'instance-type': {'type': 'string'},
                                               'mem': {'type': 'integer'},
                                               'root-disk': {'type': 'integer'},
                                               'root-disk-source': {'type': 'string'},
                                               'spaces': {'items': {'type': 'string'},
                                                          'type': 'array'},
@@ -1991,14 +1992,15 @@
                      'OfferStatusWatchResults': {'additionalProperties': False,
                                                  'properties': {'results': {'items': {'$ref': '#/definitions/OfferStatusWatchResult'},
                                                                             'type': 'array'}},
                                                  'required': ['results'],
                                                  'type': 'object'},
                      'RegisterRemoteRelationArg': {'additionalProperties': False,
                                                    'properties': {'application-token': {'type': 'string'},
+                                                                  'auth-token': {'type': 'string'},
                                                                   'bakery-version': {'type': 'integer'},
                                                                   'consume-version': {'type': 'integer'},
                                                                   'local-endpoint-name': {'type': 'string'},
                                                                   'macaroons': {'items': {'$ref': '#/definitions/Macaroon'},
                                                                                 'type': 'array'},
                                                                   'offer-uuid': {'type': 'string'},
                                                                   'relation-token': {'type': 'string'},
@@ -2134,14 +2136,32 @@
                                                                 'type': 'array'}},
                                      'required': ['cloud-type',
                                                   'name',
                                                   'provider-id',
                                                   'provider-attributes',
                                                   'subnets'],
                                      'type': 'object'},
+                     'SecretRevisionChange': {'additionalProperties': False,
+                                              'properties': {'revision': {'type': 'integer'},
+                                                             'uri': {'type': 'string'}},
+                                              'required': ['uri', 'revision'],
+                                              'type': 'object'},
+                     'SecretRevisionWatchResult': {'additionalProperties': False,
+                                                   'properties': {'changes': {'items': {'$ref': '#/definitions/SecretRevisionChange'},
+                                                                              'type': 'array'},
+                                                                  'error': {'$ref': '#/definitions/Error'},
+                                                                  'watcher-id': {'type': 'string'}},
+                                                   'required': ['watcher-id',
+                                                                'changes'],
+                                                   'type': 'object'},
+                     'SecretRevisionWatchResults': {'additionalProperties': False,
+                                                    'properties': {'results': {'items': {'$ref': '#/definitions/SecretRevisionWatchResult'},
+                                                                               'type': 'array'}},
+                                                    'required': ['results'],
+                                                    'type': 'object'},
                      'StringsWatchResult': {'additionalProperties': False,
                                             'properties': {'changes': {'items': {'type': 'string'},
                                                                        'type': 'array'},
                                                            'error': {'$ref': '#/definitions/Error'},
                                                            'watcher-id': {'type': 'string'}},
                                             'required': ['watcher-id'],
                                             'type': 'object'},
@@ -2162,15 +2182,27 @@
                                                'zones': {'items': {'type': 'string'},
                                                          'type': 'array'}},
                                 'required': ['cidr',
                                              'vlan-tag',
                                              'life',
                                              'space-tag',
                                              'zones'],
-                                'type': 'object'}},
+                                'type': 'object'},
+                     'WatchRemoteSecretChangesArg': {'additionalProperties': False,
+                                                     'properties': {'application-token': {'type': 'string'},
+                                                                    'bakery-version': {'type': 'integer'},
+                                                                    'macaroons': {'items': {'$ref': '#/definitions/Macaroon'},
+                                                                                  'type': 'array'}},
+                                                     'required': ['application-token'],
+                                                     'type': 'object'},
+                     'WatchRemoteSecretChangesArgs': {'additionalProperties': False,
+                                                      'properties': {'relations': {'items': {'$ref': '#/definitions/WatchRemoteSecretChangesArg'},
+                                                                                   'type': 'array'}},
+                                                      'required': ['relations'],
+                                                      'type': 'object'}},
      'properties': {'PublishIngressNetworkChanges': {'description': 'PublishIngressNetworkChanges '
                                                                     'publishes '
                                                                     'changes to '
                                                                     'the required\n'
                                                                     'ingress '
                                                                     'addresses to '
                                                                     'the model '
@@ -2196,14 +2228,27 @@
                                                                'in the specified '
                                                                'relations. This '
                                                                'operation is '
                                                                'idempotent.',
                                                 'properties': {'Params': {'$ref': '#/definitions/RegisterRemoteRelationArgs'},
                                                                'Result': {'$ref': '#/definitions/RegisterRemoteRelationResults'}},
                                                 'type': 'object'},
+                    'WatchConsumedSecretsChanges': {'description': 'WatchConsumedSecretsChanges '
+                                                                   'returns a '
+                                                                   'watcher which '
+                                                                   'notifies of '
+                                                                   'changes to any '
+                                                                   'secrets\n'
+                                                                   'for the '
+                                                                   'specified '
+                                                                   'remote '
+                                                                   'consumers.',
+                                                    'properties': {'Params': {'$ref': '#/definitions/WatchRemoteSecretChangesArgs'},
+                                                                   'Result': {'$ref': '#/definitions/SecretRevisionWatchResults'}},
+                                                    'type': 'object'},
                     'WatchEgressAddressesForRelations': {'description': 'WatchEgressAddressesForRelations '
                                                                         'creates a '
                                                                         'watcher '
                                                                         'that '
                                                                         'notifies '
                                                                         'when '
                                                                         'addresses, '
@@ -2336,14 +2381,38 @@
                    params=_params)
         _params['relations'] = relations
         reply = await self.rpc(msg)
         return reply
 
 
 
+    @ReturnMapping(SecretRevisionWatchResults)
+    async def WatchConsumedSecretsChanges(self, relations=None):
+        '''
+        WatchConsumedSecretsChanges returns a watcher which notifies of changes to any secrets
+        for the specified remote consumers.
+
+        relations : typing.Sequence[~WatchRemoteSecretChangesArg]
+        Returns -> SecretRevisionWatchResults
+        '''
+        if relations is not None and not isinstance(relations, (bytes, str, list)):
+            raise Exception("Expected relations to be a Sequence, received: {}".format(type(relations)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='CrossModelRelations',
+                   request='WatchConsumedSecretsChanges',
+                   version=2,
+                   params=_params)
+        _params['relations'] = relations
+        reply = await self.rpc(msg)
+        return reply
+
+
+
     @ReturnMapping(StringsWatchResults)
     async def WatchEgressAddressesForRelations(self, args=None):
         '''
         WatchEgressAddressesForRelations creates a watcher that notifies when addresses, from which
         connections will originate for the relation, change.
         Each event contains the entire set of addresses which are required for ingress for the relation.
 
@@ -2752,14 +2821,15 @@
                                'type': 'object'},
                      'Value': {'additionalProperties': False,
                                'properties': {'allocate-public-ip': {'type': 'boolean'},
                                               'arch': {'type': 'string'},
                                               'container': {'type': 'string'},
                                               'cores': {'type': 'integer'},
                                               'cpu-power': {'type': 'integer'},
+                                              'image-id': {'type': 'string'},
                                               'instance-role': {'type': 'string'},
                                               'instance-type': {'type': 'string'},
                                               'mem': {'type': 'integer'},
                                               'root-disk': {'type': 'integer'},
                                               'root-disk-source': {'type': 'string'},
                                               'spaces': {'items': {'type': 'string'},
                                                          'type': 'array'},
@@ -4280,14 +4350,19 @@
                                      'required': ['tag'],
                                      'type': 'object'},
                      'GetTokenArgs': {'additionalProperties': False,
                                       'properties': {'Args': {'items': {'$ref': '#/definitions/GetTokenArg'},
                                                               'type': 'array'}},
                                       'required': ['Args'],
                                       'type': 'object'},
+                     'LatestSecretRevisionChanges': {'additionalProperties': False,
+                                                     'properties': {'changes': {'items': {'$ref': '#/definitions/SecretRevisionChange'},
+                                                                                'type': 'array'}},
+                                                     'required': ['changes'],
+                                                     'type': 'object'},
                      'Macaroon': {'additionalProperties': False, 'type': 'object'},
                      'RemoteApplication': {'additionalProperties': False,
                                            'properties': {'consume-version': {'type': 'integer'},
                                                           'is-consumer-proxy': {'type': 'boolean'},
                                                           'life': {'type': 'string'},
                                                           'macaroon': {'$ref': '#/definitions/Macaroon'},
                                                           'model-uuid': {'type': 'string'},
@@ -4400,14 +4475,19 @@
                                                                                'type': 'array'}},
                                                     'required': ['results'],
                                                     'type': 'object'},
                      'RemoteRelationsChanges': {'additionalProperties': False,
                                                 'properties': {'changes': {'items': {'$ref': '#/definitions/RemoteRelationChangeEvent'},
                                                                            'type': 'array'}},
                                                 'type': 'object'},
+                     'SecretRevisionChange': {'additionalProperties': False,
+                                              'properties': {'revision': {'type': 'integer'},
+                                                             'uri': {'type': 'string'}},
+                                              'required': ['uri', 'revision'],
+                                              'type': 'object'},
                      'SetStatus': {'additionalProperties': False,
                                    'properties': {'entities': {'items': {'$ref': '#/definitions/EntityStatusArgs'},
                                                                'type': 'array'}},
                                    'required': ['entities'],
                                    'type': 'object'},
                      'StringResult': {'additionalProperties': False,
                                       'properties': {'error': {'$ref': '#/definitions/Error'},
@@ -4457,14 +4537,27 @@
                                                                     'from the '
                                                                     'remote/offering '
                                                                     'side of '
                                                                     'relations.',
                                                      'properties': {'Params': {'$ref': '#/definitions/RemoteRelationsChanges'},
                                                                     'Result': {'$ref': '#/definitions/ErrorResults'}},
                                                      'type': 'object'},
+                    'ConsumeRemoteSecretChanges': {'description': 'ConsumeRemoteSecretChanges '
+                                                                  'updates the '
+                                                                  'local model '
+                                                                  'with secret '
+                                                                  'revision '
+                                                                  'changes\n'
+                                                                  'originating '
+                                                                  'from the '
+                                                                  'remote/offering '
+                                                                  'model.',
+                                                   'properties': {'Params': {'$ref': '#/definitions/LatestSecretRevisionChanges'},
+                                                                  'Result': {'$ref': '#/definitions/ErrorResults'}},
+                                                   'type': 'object'},
                     'ControllerAPIInfoForModels': {'description': 'ControllerAPIInfoForModels '
                                                                   'returns the '
                                                                   'controller api '
                                                                   'connection '
                                                                   'details for the '
                                                                   'specified '
                                                                   'models.',
@@ -4654,14 +4747,38 @@
                    params=_params)
         _params['changes'] = changes
         reply = await self.rpc(msg)
         return reply
 
 
 
+    @ReturnMapping(ErrorResults)
+    async def ConsumeRemoteSecretChanges(self, changes=None):
+        '''
+        ConsumeRemoteSecretChanges updates the local model with secret revision changes
+        originating from the remote/offering model.
+
+        changes : typing.Sequence[~SecretRevisionChange]
+        Returns -> ErrorResults
+        '''
+        if changes is not None and not isinstance(changes, (bytes, str, list)):
+            raise Exception("Expected changes to be a Sequence, received: {}".format(type(changes)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='RemoteRelations',
+                   request='ConsumeRemoteSecretChanges',
+                   version=2,
+                   params=_params)
+        _params['changes'] = changes
+        reply = await self.rpc(msg)
+        return reply
+
+
+
     @ReturnMapping(ControllerAPIInfoResults)
     async def ControllerAPIInfoForModels(self, entities=None):
         '''
         ControllerAPIInfoForModels returns the controller api connection details for the specified models.
 
         entities : typing.Sequence[~Entity]
         Returns -> ControllerAPIInfoResults
@@ -4985,14 +5102,850 @@
                    params=_params)
 
         reply = await self.rpc(msg)
         return reply
 
 
 
+class SecretsManagerFacade(Type):
+    name = 'SecretsManager'
+    version = 2
+    schema =     {'definitions': {'CreateSecretArg': {'additionalProperties': False,
+                                         'properties': {'UpsertSecretArg': {'$ref': '#/definitions/UpsertSecretArg'},
+                                                        'content': {'$ref': '#/definitions/SecretContentParams'},
+                                                        'description': {'type': 'string'},
+                                                        'expire-time': {'format': 'date-time',
+                                                                        'type': 'string'},
+                                                        'label': {'type': 'string'},
+                                                        'owner-tag': {'type': 'string'},
+                                                        'params': {'patternProperties': {'.*': {'additionalProperties': True,
+                                                                                                'type': 'object'}},
+                                                                   'type': 'object'},
+                                                        'rotate-policy': {'type': 'string'},
+                                                        'uri': {'type': 'string'}},
+                                         'required': ['UpsertSecretArg',
+                                                      'owner-tag'],
+                                         'type': 'object'},
+                     'CreateSecretArgs': {'additionalProperties': False,
+                                          'properties': {'args': {'items': {'$ref': '#/definitions/CreateSecretArg'},
+                                                                  'type': 'array'}},
+                                          'required': ['args'],
+                                          'type': 'object'},
+                     'CreateSecretURIsArg': {'additionalProperties': False,
+                                             'properties': {'count': {'type': 'integer'}},
+                                             'required': ['count'],
+                                             'type': 'object'},
+                     'DeleteSecretArg': {'additionalProperties': False,
+                                         'properties': {'revisions': {'items': {'type': 'integer'},
+                                                                      'type': 'array'},
+                                                        'uri': {'type': 'string'}},
+                                         'required': ['uri'],
+                                         'type': 'object'},
+                     'DeleteSecretArgs': {'additionalProperties': False,
+                                          'properties': {'args': {'items': {'$ref': '#/definitions/DeleteSecretArg'},
+                                                                  'type': 'array'}},
+                                          'required': ['args'],
+                                          'type': 'object'},
+                     'Entities': {'additionalProperties': False,
+                                  'properties': {'entities': {'items': {'$ref': '#/definitions/Entity'},
+                                                              'type': 'array'}},
+                                  'required': ['entities'],
+                                  'type': 'object'},
+                     'Entity': {'additionalProperties': False,
+                                'properties': {'tag': {'type': 'string'}},
+                                'required': ['tag'],
+                                'type': 'object'},
+                     'Error': {'additionalProperties': False,
+                               'properties': {'code': {'type': 'string'},
+                                              'info': {'patternProperties': {'.*': {'additionalProperties': True,
+                                                                                    'type': 'object'}},
+                                                       'type': 'object'},
+                                              'message': {'type': 'string'}},
+                               'required': ['message', 'code'],
+                               'type': 'object'},
+                     'ErrorResult': {'additionalProperties': False,
+                                     'properties': {'error': {'$ref': '#/definitions/Error'}},
+                                     'type': 'object'},
+                     'ErrorResults': {'additionalProperties': False,
+                                      'properties': {'results': {'items': {'$ref': '#/definitions/ErrorResult'},
+                                                                 'type': 'array'}},
+                                      'required': ['results'],
+                                      'type': 'object'},
+                     'GetSecretConsumerInfoArgs': {'additionalProperties': False,
+                                                   'properties': {'consumer-tag': {'type': 'string'},
+                                                                  'uris': {'items': {'type': 'string'},
+                                                                           'type': 'array'}},
+                                                   'required': ['consumer-tag',
+                                                                'uris'],
+                                                   'type': 'object'},
+                     'GetSecretContentArg': {'additionalProperties': False,
+                                             'properties': {'label': {'type': 'string'},
+                                                            'peek': {'type': 'boolean'},
+                                                            'refresh': {'type': 'boolean'},
+                                                            'uri': {'type': 'string'}},
+                                             'required': ['uri'],
+                                             'type': 'object'},
+                     'GetSecretContentArgs': {'additionalProperties': False,
+                                              'properties': {'args': {'items': {'$ref': '#/definitions/GetSecretContentArg'},
+                                                                      'type': 'array'}},
+                                              'required': ['args'],
+                                              'type': 'object'},
+                     'GrantRevokeSecretArg': {'additionalProperties': False,
+                                              'properties': {'role': {'type': 'string'},
+                                                             'scope-tag': {'type': 'string'},
+                                                             'subject-tags': {'items': {'type': 'string'},
+                                                                              'type': 'array'},
+                                                             'uri': {'type': 'string'}},
+                                              'required': ['uri',
+                                                           'scope-tag',
+                                                           'subject-tags',
+                                                           'role'],
+                                              'type': 'object'},
+                     'GrantRevokeSecretArgs': {'additionalProperties': False,
+                                               'properties': {'args': {'items': {'$ref': '#/definitions/GrantRevokeSecretArg'},
+                                                                       'type': 'array'}},
+                                               'required': ['args'],
+                                               'type': 'object'},
+                     'ListSecretResult': {'additionalProperties': False,
+                                          'properties': {'create-time': {'format': 'date-time',
+                                                                         'type': 'string'},
+                                                         'description': {'type': 'string'},
+                                                         'label': {'type': 'string'},
+                                                         'latest-expire-time': {'format': 'date-time',
+                                                                                'type': 'string'},
+                                                         'latest-revision': {'type': 'integer'},
+                                                         'next-rotate-time': {'format': 'date-time',
+                                                                              'type': 'string'},
+                                                         'owner-tag': {'type': 'string'},
+                                                         'revisions': {'items': {'$ref': '#/definitions/SecretRevision'},
+                                                                       'type': 'array'},
+                                                         'rotate-policy': {'type': 'string'},
+                                                         'update-time': {'format': 'date-time',
+                                                                         'type': 'string'},
+                                                         'uri': {'type': 'string'},
+                                                         'value': {'$ref': '#/definitions/SecretValueResult'},
+                                                         'version': {'type': 'integer'}},
+                                          'required': ['uri',
+                                                       'version',
+                                                       'owner-tag',
+                                                       'latest-revision',
+                                                       'create-time',
+                                                       'update-time',
+                                                       'revisions'],
+                                          'type': 'object'},
+                     'ListSecretResults': {'additionalProperties': False,
+                                           'properties': {'results': {'items': {'$ref': '#/definitions/ListSecretResult'},
+                                                                      'type': 'array'}},
+                                           'required': ['results'],
+                                           'type': 'object'},
+                     'SecretBackendArgs': {'additionalProperties': False,
+                                           'properties': {'backend-ids': {'items': {'type': 'string'},
+                                                                          'type': 'array'}},
+                                           'required': ['backend-ids'],
+                                           'type': 'object'},
+                     'SecretBackendConfig': {'additionalProperties': False,
+                                             'properties': {'params': {'patternProperties': {'.*': {'additionalProperties': True,
+                                                                                                    'type': 'object'}},
+                                                                       'type': 'object'},
+                                                            'type': {'type': 'string'}},
+                                             'required': ['type'],
+                                             'type': 'object'},
+                     'SecretBackendConfigResult': {'additionalProperties': False,
+                                                   'properties': {'config': {'$ref': '#/definitions/SecretBackendConfig'},
+                                                                  'draining': {'type': 'boolean'},
+                                                                  'model-controller': {'type': 'string'},
+                                                                  'model-name': {'type': 'string'},
+                                                                  'model-uuid': {'type': 'string'}},
+                                                   'required': ['model-controller',
+                                                                'model-uuid',
+                                                                'model-name',
+                                                                'draining'],
+                                                   'type': 'object'},
+                     'SecretBackendConfigResults': {'additionalProperties': False,
+                                                    'properties': {'active-id': {'type': 'string'},
+                                                                   'results': {'patternProperties': {'.*': {'$ref': '#/definitions/SecretBackendConfigResult'}},
+                                                                               'type': 'object'}},
+                                                    'required': ['active-id'],
+                                                    'type': 'object'},
+                     'SecretConsumerInfoResult': {'additionalProperties': False,
+                                                  'properties': {'error': {'$ref': '#/definitions/Error'},
+                                                                 'label': {'type': 'string'},
+                                                                 'revision': {'type': 'integer'}},
+                                                  'required': ['revision', 'label'],
+                                                  'type': 'object'},
+                     'SecretConsumerInfoResults': {'additionalProperties': False,
+                                                   'properties': {'results': {'items': {'$ref': '#/definitions/SecretConsumerInfoResult'},
+                                                                              'type': 'array'}},
+                                                   'required': ['results'],
+                                                   'type': 'object'},
+                     'SecretContentParams': {'additionalProperties': False,
+                                             'properties': {'data': {'patternProperties': {'.*': {'type': 'string'}},
+                                                                     'type': 'object'},
+                                                            'value-ref': {'$ref': '#/definitions/SecretValueRef'}},
+                                             'type': 'object'},
+                     'SecretContentResult': {'additionalProperties': False,
+                                             'properties': {'backend-config': {'$ref': '#/definitions/SecretBackendConfigResult'},
+                                                            'content': {'$ref': '#/definitions/SecretContentParams'},
+                                                            'error': {'$ref': '#/definitions/Error'},
+                                                            'latest-revision': {'type': 'integer'}},
+                                             'required': ['content'],
+                                             'type': 'object'},
+                     'SecretContentResults': {'additionalProperties': False,
+                                              'properties': {'results': {'items': {'$ref': '#/definitions/SecretContentResult'},
+                                                                         'type': 'array'}},
+                                              'required': ['results'],
+                                              'type': 'object'},
+                     'SecretRevision': {'additionalProperties': False,
+                                        'properties': {'backend-name': {'type': 'string'},
+                                                       'create-time': {'format': 'date-time',
+                                                                       'type': 'string'},
+                                                       'expire-time': {'format': 'date-time',
+                                                                       'type': 'string'},
+                                                       'revision': {'type': 'integer'},
+                                                       'update-time': {'format': 'date-time',
+                                                                       'type': 'string'},
+                                                       'value-ref': {'$ref': '#/definitions/SecretValueRef'}},
+                                        'required': ['revision'],
+                                        'type': 'object'},
+                     'SecretRevisionArg': {'additionalProperties': False,
+                                           'properties': {'pending-delete': {'type': 'boolean'},
+                                                          'revisions': {'items': {'type': 'integer'},
+                                                                        'type': 'array'},
+                                                          'uri': {'type': 'string'}},
+                                           'required': ['uri',
+                                                        'revisions',
+                                                        'pending-delete'],
+                                           'type': 'object'},
+                     'SecretRotatedArg': {'additionalProperties': False,
+                                          'properties': {'original-revision': {'type': 'integer'},
+                                                         'skip': {'type': 'boolean'},
+                                                         'uri': {'type': 'string'}},
+                                          'required': ['uri',
+                                                       'original-revision',
+                                                       'skip'],
+                                          'type': 'object'},
+                     'SecretRotatedArgs': {'additionalProperties': False,
+                                           'properties': {'args': {'items': {'$ref': '#/definitions/SecretRotatedArg'},
+                                                                   'type': 'array'}},
+                                           'required': ['args'],
+                                           'type': 'object'},
+                     'SecretTriggerChange': {'additionalProperties': False,
+                                             'properties': {'next-trigger-time': {'format': 'date-time',
+                                                                                  'type': 'string'},
+                                                            'revision': {'type': 'integer'},
+                                                            'uri': {'type': 'string'}},
+                                             'required': ['uri',
+                                                          'next-trigger-time'],
+                                             'type': 'object'},
+                     'SecretTriggerWatchResult': {'additionalProperties': False,
+                                                  'properties': {'changes': {'items': {'$ref': '#/definitions/SecretTriggerChange'},
+                                                                             'type': 'array'},
+                                                                 'error': {'$ref': '#/definitions/Error'},
+                                                                 'watcher-id': {'type': 'string'}},
+                                                  'required': ['watcher-id',
+                                                               'changes'],
+                                                  'type': 'object'},
+                     'SecretValueRef': {'additionalProperties': False,
+                                        'properties': {'backend-id': {'type': 'string'},
+                                                       'revision-id': {'type': 'string'}},
+                                        'required': ['backend-id', 'revision-id'],
+                                        'type': 'object'},
+                     'SecretValueResult': {'additionalProperties': False,
+                                           'properties': {'data': {'patternProperties': {'.*': {'type': 'string'}},
+                                                                   'type': 'object'},
+                                                          'error': {'$ref': '#/definitions/Error'}},
+                                           'type': 'object'},
+                     'StringResult': {'additionalProperties': False,
+                                      'properties': {'error': {'$ref': '#/definitions/Error'},
+                                                     'result': {'type': 'string'}},
+                                      'required': ['result'],
+                                      'type': 'object'},
+                     'StringResults': {'additionalProperties': False,
+                                       'properties': {'results': {'items': {'$ref': '#/definitions/StringResult'},
+                                                                  'type': 'array'}},
+                                       'required': ['results'],
+                                       'type': 'object'},
+                     'StringsWatchResult': {'additionalProperties': False,
+                                            'properties': {'changes': {'items': {'type': 'string'},
+                                                                       'type': 'array'},
+                                                           'error': {'$ref': '#/definitions/Error'},
+                                                           'watcher-id': {'type': 'string'}},
+                                            'required': ['watcher-id'],
+                                            'type': 'object'},
+                     'StringsWatchResults': {'additionalProperties': False,
+                                             'properties': {'results': {'items': {'$ref': '#/definitions/StringsWatchResult'},
+                                                                        'type': 'array'}},
+                                             'required': ['results'],
+                                             'type': 'object'},
+                     'UpdateSecretArg': {'additionalProperties': False,
+                                         'properties': {'UpsertSecretArg': {'$ref': '#/definitions/UpsertSecretArg'},
+                                                        'content': {'$ref': '#/definitions/SecretContentParams'},
+                                                        'description': {'type': 'string'},
+                                                        'expire-time': {'format': 'date-time',
+                                                                        'type': 'string'},
+                                                        'label': {'type': 'string'},
+                                                        'params': {'patternProperties': {'.*': {'additionalProperties': True,
+                                                                                                'type': 'object'}},
+                                                                   'type': 'object'},
+                                                        'rotate-policy': {'type': 'string'},
+                                                        'uri': {'type': 'string'}},
+                                         'required': ['UpsertSecretArg', 'uri'],
+                                         'type': 'object'},
+                     'UpdateSecretArgs': {'additionalProperties': False,
+                                          'properties': {'args': {'items': {'$ref': '#/definitions/UpdateSecretArg'},
+                                                                  'type': 'array'}},
+                                          'required': ['args'],
+                                          'type': 'object'},
+                     'UpsertSecretArg': {'additionalProperties': False,
+                                         'properties': {'content': {'$ref': '#/definitions/SecretContentParams'},
+                                                        'description': {'type': 'string'},
+                                                        'expire-time': {'format': 'date-time',
+                                                                        'type': 'string'},
+                                                        'label': {'type': 'string'},
+                                                        'params': {'patternProperties': {'.*': {'additionalProperties': True,
+                                                                                                'type': 'object'}},
+                                                                   'type': 'object'},
+                                                        'rotate-policy': {'type': 'string'}},
+                                         'type': 'object'}},
+     'properties': {'CreateSecretURIs': {'description': 'CreateSecretURIs creates '
+                                                        'new secret URIs.',
+                                         'properties': {'Params': {'$ref': '#/definitions/CreateSecretURIsArg'},
+                                                        'Result': {'$ref': '#/definitions/StringResults'}},
+                                         'type': 'object'},
+                    'CreateSecrets': {'description': 'CreateSecrets creates new '
+                                                     'secrets.',
+                                      'properties': {'Params': {'$ref': '#/definitions/CreateSecretArgs'},
+                                                     'Result': {'$ref': '#/definitions/StringResults'}},
+                                      'type': 'object'},
+                    'GetConsumerSecretsRevisionInfo': {'description': 'GetConsumerSecretsRevisionInfo '
+                                                                      'returns the '
+                                                                      'latest '
+                                                                      'secret '
+                                                                      'revisions '
+                                                                      'for the '
+                                                                      'specified '
+                                                                      'secrets.\n'
+                                                                      'This facade '
+                                                                      'method is '
+                                                                      'used for '
+                                                                      'remote '
+                                                                      'watcher to '
+                                                                      'get the '
+                                                                      'latest '
+                                                                      'secret '
+                                                                      'revisions '
+                                                                      'and labels '
+                                                                      'for a '
+                                                                      'secret '
+                                                                      'changed '
+                                                                      'hook.',
+                                                       'properties': {'Params': {'$ref': '#/definitions/GetSecretConsumerInfoArgs'},
+                                                                      'Result': {'$ref': '#/definitions/SecretConsumerInfoResults'}},
+                                                       'type': 'object'},
+                    'GetSecretBackendConfigs': {'description': 'GetSecretBackendConfigs '
+                                                               'gets the config '
+                                                               'needed to create a '
+                                                               'client to secret '
+                                                               'backends.',
+                                                'properties': {'Params': {'$ref': '#/definitions/SecretBackendArgs'},
+                                                               'Result': {'$ref': '#/definitions/SecretBackendConfigResults'}},
+                                                'type': 'object'},
+                    'GetSecretContentInfo': {'description': 'GetSecretContentInfo '
+                                                            'returns the secret '
+                                                            'values for the '
+                                                            'specified secrets.',
+                                             'properties': {'Params': {'$ref': '#/definitions/GetSecretContentArgs'},
+                                                            'Result': {'$ref': '#/definitions/SecretContentResults'}},
+                                             'type': 'object'},
+                    'GetSecretMetadata': {'description': 'GetSecretMetadata '
+                                                         'returns metadata for the '
+                                                         "caller's secrets.",
+                                          'properties': {'Result': {'$ref': '#/definitions/ListSecretResults'}},
+                                          'type': 'object'},
+                    'GetSecretRevisionContentInfo': {'description': 'GetSecretRevisionContentInfo '
+                                                                    'returns the '
+                                                                    'secret values '
+                                                                    'for the '
+                                                                    'specified '
+                                                                    'secret '
+                                                                    'revisions.',
+                                                     'properties': {'Params': {'$ref': '#/definitions/SecretRevisionArg'},
+                                                                    'Result': {'$ref': '#/definitions/SecretContentResults'}},
+                                                     'type': 'object'},
+                    'RemoveSecrets': {'description': 'RemoveSecrets removes the '
+                                                     'specified secrets.',
+                                      'properties': {'Params': {'$ref': '#/definitions/DeleteSecretArgs'},
+                                                     'Result': {'$ref': '#/definitions/ErrorResults'}},
+                                      'type': 'object'},
+                    'SecretsGrant': {'description': 'SecretsGrant grants access to '
+                                                    'a secret for the specified '
+                                                    'subjects.',
+                                     'properties': {'Params': {'$ref': '#/definitions/GrantRevokeSecretArgs'},
+                                                    'Result': {'$ref': '#/definitions/ErrorResults'}},
+                                     'type': 'object'},
+                    'SecretsRevoke': {'description': 'SecretsRevoke revokes access '
+                                                     'to a secret for the '
+                                                     'specified subjects.',
+                                      'properties': {'Params': {'$ref': '#/definitions/GrantRevokeSecretArgs'},
+                                                     'Result': {'$ref': '#/definitions/ErrorResults'}},
+                                      'type': 'object'},
+                    'SecretsRotated': {'description': 'SecretsRotated records when '
+                                                      'secrets were last rotated.',
+                                       'properties': {'Params': {'$ref': '#/definitions/SecretRotatedArgs'},
+                                                      'Result': {'$ref': '#/definitions/ErrorResults'}},
+                                       'type': 'object'},
+                    'UpdateSecrets': {'description': 'UpdateSecrets updates the '
+                                                     'specified secrets.',
+                                      'properties': {'Params': {'$ref': '#/definitions/UpdateSecretArgs'},
+                                                     'Result': {'$ref': '#/definitions/ErrorResults'}},
+                                      'type': 'object'},
+                    'WatchConsumedSecretsChanges': {'description': 'WatchConsumedSecretsChanges '
+                                                                   'sets up a '
+                                                                   'watcher to '
+                                                                   'notify of '
+                                                                   'changes to '
+                                                                   'secret '
+                                                                   'revisions for '
+                                                                   'the specified '
+                                                                   'consumers.',
+                                                    'properties': {'Params': {'$ref': '#/definitions/Entities'},
+                                                                   'Result': {'$ref': '#/definitions/StringsWatchResults'}},
+                                                    'type': 'object'},
+                    'WatchObsolete': {'description': 'WatchObsolete returns a '
+                                                     'watcher for notifying when:\n'
+                                                     '  - a secret owned by the '
+                                                     'entity is deleted\n'
+                                                     '  - a secret revision owed '
+                                                     'by the entity no longer\n'
+                                                     '    has any consumers\n'
+                                                     '\n'
+                                                     'Obsolete revisions results '
+                                                     'are "uri/revno" and deleted\n'
+                                                     'secret results are "uri".',
+                                      'properties': {'Params': {'$ref': '#/definitions/Entities'},
+                                                     'Result': {'$ref': '#/definitions/StringsWatchResult'}},
+                                      'type': 'object'},
+                    'WatchSecretRevisionsExpiryChanges': {'description': 'WatchSecretRevisionsExpiryChanges '
+                                                                         'sets up '
+                                                                         'a '
+                                                                         'watcher '
+                                                                         'to '
+                                                                         'notify '
+                                                                         'of '
+                                                                         'changes '
+                                                                         'to '
+                                                                         'secret '
+                                                                         'revision '
+                                                                         'expiry '
+                                                                         'config.',
+                                                          'properties': {'Params': {'$ref': '#/definitions/Entities'},
+                                                                         'Result': {'$ref': '#/definitions/SecretTriggerWatchResult'}},
+                                                          'type': 'object'},
+                    'WatchSecretsRotationChanges': {'description': 'WatchSecretsRotationChanges '
+                                                                   'sets up a '
+                                                                   'watcher to '
+                                                                   'notify of '
+                                                                   'changes to '
+                                                                   'secret '
+                                                                   'rotation '
+                                                                   'config.',
+                                                    'properties': {'Params': {'$ref': '#/definitions/Entities'},
+                                                                   'Result': {'$ref': '#/definitions/SecretTriggerWatchResult'}},
+                                                    'type': 'object'}},
+     'type': 'object'}
+    
+
+    @ReturnMapping(StringResults)
+    async def CreateSecretURIs(self, count=None):
+        '''
+        CreateSecretURIs creates new secret URIs.
+
+        count : int
+        Returns -> StringResults
+        '''
+        if count is not None and not isinstance(count, int):
+            raise Exception("Expected count to be a int, received: {}".format(type(count)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='CreateSecretURIs',
+                   version=2,
+                   params=_params)
+        _params['count'] = count
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(StringResults)
+    async def CreateSecrets(self, args=None):
+        '''
+        CreateSecrets creates new secrets.
+
+        args : typing.Sequence[~CreateSecretArg]
+        Returns -> StringResults
+        '''
+        if args is not None and not isinstance(args, (bytes, str, list)):
+            raise Exception("Expected args to be a Sequence, received: {}".format(type(args)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='CreateSecrets',
+                   version=2,
+                   params=_params)
+        _params['args'] = args
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(SecretConsumerInfoResults)
+    async def GetConsumerSecretsRevisionInfo(self, consumer_tag=None, uris=None):
+        '''
+        GetConsumerSecretsRevisionInfo returns the latest secret revisions for the specified secrets.
+        This facade method is used for remote watcher to get the latest secret revisions and labels for a secret changed hook.
+
+        consumer_tag : str
+        uris : typing.Sequence[str]
+        Returns -> SecretConsumerInfoResults
+        '''
+        if consumer_tag is not None and not isinstance(consumer_tag, (bytes, str)):
+            raise Exception("Expected consumer_tag to be a str, received: {}".format(type(consumer_tag)))
+
+        if uris is not None and not isinstance(uris, (bytes, str, list)):
+            raise Exception("Expected uris to be a Sequence, received: {}".format(type(uris)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='GetConsumerSecretsRevisionInfo',
+                   version=2,
+                   params=_params)
+        _params['consumer-tag'] = consumer_tag
+        _params['uris'] = uris
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(SecretBackendConfigResults)
+    async def GetSecretBackendConfigs(self, backend_ids=None):
+        '''
+        GetSecretBackendConfigs gets the config needed to create a client to secret backends.
+
+        backend_ids : typing.Sequence[str]
+        Returns -> SecretBackendConfigResults
+        '''
+        if backend_ids is not None and not isinstance(backend_ids, (bytes, str, list)):
+            raise Exception("Expected backend_ids to be a Sequence, received: {}".format(type(backend_ids)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='GetSecretBackendConfigs',
+                   version=2,
+                   params=_params)
+        _params['backend-ids'] = backend_ids
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(SecretContentResults)
+    async def GetSecretContentInfo(self, args=None):
+        '''
+        GetSecretContentInfo returns the secret values for the specified secrets.
+
+        args : typing.Sequence[~GetSecretContentArg]
+        Returns -> SecretContentResults
+        '''
+        if args is not None and not isinstance(args, (bytes, str, list)):
+            raise Exception("Expected args to be a Sequence, received: {}".format(type(args)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='GetSecretContentInfo',
+                   version=2,
+                   params=_params)
+        _params['args'] = args
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(ListSecretResults)
+    async def GetSecretMetadata(self):
+        '''
+        GetSecretMetadata returns metadata for the caller's secrets.
+
+
+        Returns -> ListSecretResults
+        '''
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='GetSecretMetadata',
+                   version=2,
+                   params=_params)
+
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(SecretContentResults)
+    async def GetSecretRevisionContentInfo(self, pending_delete=None, revisions=None, uri=None):
+        '''
+        GetSecretRevisionContentInfo returns the secret values for the specified secret revisions.
+
+        pending_delete : bool
+        revisions : typing.Sequence[int]
+        uri : str
+        Returns -> SecretContentResults
+        '''
+        if pending_delete is not None and not isinstance(pending_delete, bool):
+            raise Exception("Expected pending_delete to be a bool, received: {}".format(type(pending_delete)))
+
+        if revisions is not None and not isinstance(revisions, (bytes, str, list)):
+            raise Exception("Expected revisions to be a Sequence, received: {}".format(type(revisions)))
+
+        if uri is not None and not isinstance(uri, (bytes, str)):
+            raise Exception("Expected uri to be a str, received: {}".format(type(uri)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='GetSecretRevisionContentInfo',
+                   version=2,
+                   params=_params)
+        _params['pending-delete'] = pending_delete
+        _params['revisions'] = revisions
+        _params['uri'] = uri
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(ErrorResults)
+    async def RemoveSecrets(self, args=None):
+        '''
+        RemoveSecrets removes the specified secrets.
+
+        args : typing.Sequence[~DeleteSecretArg]
+        Returns -> ErrorResults
+        '''
+        if args is not None and not isinstance(args, (bytes, str, list)):
+            raise Exception("Expected args to be a Sequence, received: {}".format(type(args)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='RemoveSecrets',
+                   version=2,
+                   params=_params)
+        _params['args'] = args
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(ErrorResults)
+    async def SecretsGrant(self, args=None):
+        '''
+        SecretsGrant grants access to a secret for the specified subjects.
+
+        args : typing.Sequence[~GrantRevokeSecretArg]
+        Returns -> ErrorResults
+        '''
+        if args is not None and not isinstance(args, (bytes, str, list)):
+            raise Exception("Expected args to be a Sequence, received: {}".format(type(args)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='SecretsGrant',
+                   version=2,
+                   params=_params)
+        _params['args'] = args
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(ErrorResults)
+    async def SecretsRevoke(self, args=None):
+        '''
+        SecretsRevoke revokes access to a secret for the specified subjects.
+
+        args : typing.Sequence[~GrantRevokeSecretArg]
+        Returns -> ErrorResults
+        '''
+        if args is not None and not isinstance(args, (bytes, str, list)):
+            raise Exception("Expected args to be a Sequence, received: {}".format(type(args)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='SecretsRevoke',
+                   version=2,
+                   params=_params)
+        _params['args'] = args
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(ErrorResults)
+    async def SecretsRotated(self, args=None):
+        '''
+        SecretsRotated records when secrets were last rotated.
+
+        args : typing.Sequence[~SecretRotatedArg]
+        Returns -> ErrorResults
+        '''
+        if args is not None and not isinstance(args, (bytes, str, list)):
+            raise Exception("Expected args to be a Sequence, received: {}".format(type(args)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='SecretsRotated',
+                   version=2,
+                   params=_params)
+        _params['args'] = args
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(ErrorResults)
+    async def UpdateSecrets(self, args=None):
+        '''
+        UpdateSecrets updates the specified secrets.
+
+        args : typing.Sequence[~UpdateSecretArg]
+        Returns -> ErrorResults
+        '''
+        if args is not None and not isinstance(args, (bytes, str, list)):
+            raise Exception("Expected args to be a Sequence, received: {}".format(type(args)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='UpdateSecrets',
+                   version=2,
+                   params=_params)
+        _params['args'] = args
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(StringsWatchResults)
+    async def WatchConsumedSecretsChanges(self, entities=None):
+        '''
+        WatchConsumedSecretsChanges sets up a watcher to notify of changes to secret revisions for the specified consumers.
+
+        entities : typing.Sequence[~Entity]
+        Returns -> StringsWatchResults
+        '''
+        if entities is not None and not isinstance(entities, (bytes, str, list)):
+            raise Exception("Expected entities to be a Sequence, received: {}".format(type(entities)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='WatchConsumedSecretsChanges',
+                   version=2,
+                   params=_params)
+        _params['entities'] = entities
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(StringsWatchResult)
+    async def WatchObsolete(self, entities=None):
+        '''
+        WatchObsolete returns a watcher for notifying when:
+          - a secret owned by the entity is deleted
+          - a secret revision owed by the entity no longer
+            has any consumers
+
+        Obsolete revisions results are "uri/revno" and deleted
+        secret results are "uri".
+
+        entities : typing.Sequence[~Entity]
+        Returns -> StringsWatchResult
+        '''
+        if entities is not None and not isinstance(entities, (bytes, str, list)):
+            raise Exception("Expected entities to be a Sequence, received: {}".format(type(entities)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='WatchObsolete',
+                   version=2,
+                   params=_params)
+        _params['entities'] = entities
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(SecretTriggerWatchResult)
+    async def WatchSecretRevisionsExpiryChanges(self, entities=None):
+        '''
+        WatchSecretRevisionsExpiryChanges sets up a watcher to notify of changes to secret revision expiry config.
+
+        entities : typing.Sequence[~Entity]
+        Returns -> SecretTriggerWatchResult
+        '''
+        if entities is not None and not isinstance(entities, (bytes, str, list)):
+            raise Exception("Expected entities to be a Sequence, received: {}".format(type(entities)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='WatchSecretRevisionsExpiryChanges',
+                   version=2,
+                   params=_params)
+        _params['entities'] = entities
+        reply = await self.rpc(msg)
+        return reply
+
+
+
+    @ReturnMapping(SecretTriggerWatchResult)
+    async def WatchSecretsRotationChanges(self, entities=None):
+        '''
+        WatchSecretsRotationChanges sets up a watcher to notify of changes to secret rotation config.
+
+        entities : typing.Sequence[~Entity]
+        Returns -> SecretTriggerWatchResult
+        '''
+        if entities is not None and not isinstance(entities, (bytes, str, list)):
+            raise Exception("Expected entities to be a Sequence, received: {}".format(type(entities)))
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='SecretsManager',
+                   request='WatchSecretsRotationChanges',
+                   version=2,
+                   params=_params)
+        _params['entities'] = entities
+        reply = await self.rpc(msg)
+        return reply
+
+
+
 class SingularFacade(Type):
     name = 'Singular'
     version = 2
     schema =     {'definitions': {'Entities': {'additionalProperties': False,
                                   'properties': {'entities': {'items': {'$ref': '#/definitions/Entity'},
                                                               'type': 'array'}},
                                   'required': ['entities'],
```

### Comparing `juju-3.1.2.0/juju/client/_client3.py` & `juju-3.2.0.0/juju/client/_client3.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
                                                      'cli-args': {'type': 'string'},
                                                      'client-version': {'type': 'string'},
                                                      'credentials': {'type': 'string'},
                                                      'macaroons': {'items': {'items': {'$ref': '#/definitions/Macaroon'},
                                                                              'type': 'array'},
                                                                    'type': 'array'},
                                                      'nonce': {'type': 'string'},
+                                                     'token': {'type': 'string'},
                                                      'user-data': {'type': 'string'}},
                                       'required': ['auth-tag',
                                                    'credentials',
                                                    'nonce',
                                                    'macaroons',
                                                    'user-data'],
                                       'type': 'object'},
@@ -113,26 +114,27 @@
                                                     'controllers.',
                                      'properties': {'Result': {'$ref': '#/definitions/RedirectInfoResult'}},
                                      'type': 'object'}},
      'type': 'object'}
     
 
     @ReturnMapping(LoginResult)
-    async def Login(self, auth_tag=None, bakery_version=None, cli_args=None, client_version=None, credentials=None, macaroons=None, nonce=None, user_data=None):
+    async def Login(self, auth_tag=None, bakery_version=None, cli_args=None, client_version=None, credentials=None, macaroons=None, nonce=None, token=None, user_data=None):
         '''
         Login logs in with the provided credentials.  All subsequent requests on the
         connection will act as the authenticated user.
 
         auth_tag : str
         bakery_version : int
         cli_args : str
         client_version : str
         credentials : str
         macaroons : typing.Sequence[~Macaroon]
         nonce : str
+        token : str
         user_data : str
         Returns -> LoginResult
         '''
         if auth_tag is not None and not isinstance(auth_tag, (bytes, str)):
             raise Exception("Expected auth_tag to be a str, received: {}".format(type(auth_tag)))
 
         if bakery_version is not None and not isinstance(bakery_version, int):
@@ -149,14 +151,17 @@
 
         if macaroons is not None and not isinstance(macaroons, (bytes, str, list)):
             raise Exception("Expected macaroons to be a Sequence, received: {}".format(type(macaroons)))
 
         if nonce is not None and not isinstance(nonce, (bytes, str)):
             raise Exception("Expected nonce to be a str, received: {}".format(type(nonce)))
 
+        if token is not None and not isinstance(token, (bytes, str)):
+            raise Exception("Expected token to be a str, received: {}".format(type(token)))
+
         if user_data is not None and not isinstance(user_data, (bytes, str)):
             raise Exception("Expected user_data to be a str, received: {}".format(type(user_data)))
 
         # map input types to rpc msg
         _params = dict()
         msg = dict(type='Admin',
                    request='Login',
@@ -165,14 +170,15 @@
         _params['auth-tag'] = auth_tag
         _params['bakery-version'] = bakery_version
         _params['cli-args'] = cli_args
         _params['client-version'] = client_version
         _params['credentials'] = credentials
         _params['macaroons'] = macaroons
         _params['nonce'] = nonce
+        _params['token'] = token
         _params['user-data'] = user_data
         reply = await self.rpc(msg)
         return reply
 
 
 
     @ReturnMapping(RedirectInfoResult)
@@ -2005,14 +2011,15 @@
                                       'type': 'object'},
                      'Value': {'additionalProperties': False,
                                'properties': {'allocate-public-ip': {'type': 'boolean'},
                                               'arch': {'type': 'string'},
                                               'container': {'type': 'string'},
                                               'cores': {'type': 'integer'},
                                               'cpu-power': {'type': 'integer'},
+                                              'image-id': {'type': 'string'},
                                               'instance-role': {'type': 'string'},
                                               'instance-type': {'type': 'string'},
                                               'mem': {'type': 'integer'},
                                               'root-disk': {'type': 'integer'},
                                               'root-disk-source': {'type': 'string'},
                                               'spaces': {'items': {'type': 'string'},
                                                          'type': 'array'},
@@ -2572,15 +2579,16 @@
                                               'type': 'object'},
                      'PinApplicationsResults': {'additionalProperties': False,
                                                 'properties': {'results': {'items': {'$ref': '#/definitions/PinApplicationResult'},
                                                                            'type': 'array'}},
                                                 'required': ['results'],
                                                 'type': 'object'},
                      'PinnedLeadershipResult': {'additionalProperties': False,
-                                                'properties': {'result': {'patternProperties': {'.*': {'items': {'type': 'string'},
+                                                'properties': {'error': {'$ref': '#/definitions/Error'},
+                                                               'result': {'patternProperties': {'.*': {'items': {'type': 'string'},
                                                                                                        'type': 'array'}},
                                                                           'type': 'object'}},
                                                 'type': 'object'},
                      'SetStatus': {'additionalProperties': False,
                                    'properties': {'entities': {'items': {'$ref': '#/definitions/EntityStatusArgs'},
                                                                'type': 'array'}},
                                    'required': ['entities'],
```

### Comparing `juju-3.1.2.0/juju/client/_client4.py` & `juju-3.2.0.0/juju/client/_client4.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,25 +161,27 @@
                                                                'result': {'$ref': '#/definitions/ApplicationOfferAdminDetails'}},
                                                 'type': 'object'},
                      'ApplicationOffersResults': {'additionalProperties': False,
                                                   'properties': {'results': {'items': {'$ref': '#/definitions/ApplicationOfferResult'},
                                                                              'type': 'array'}},
                                                   'type': 'object'},
                      'ConsumeOfferDetails': {'additionalProperties': False,
-                                             'properties': {'external-controller': {'$ref': '#/definitions/ExternalControllerInfo'},
+                                             'properties': {'auth-token': {'type': 'string'},
+                                                            'external-controller': {'$ref': '#/definitions/ExternalControllerInfo'},
                                                             'macaroon': {'$ref': '#/definitions/Macaroon'},
                                                             'offer': {'$ref': '#/definitions/ApplicationOfferDetails'}},
                                              'type': 'object'},
                      'ConsumeOfferDetailsArg': {'additionalProperties': False,
                                                 'properties': {'offer-urls': {'$ref': '#/definitions/OfferURLs'},
                                                                'user-tag': {'type': 'string'}},
                                                 'required': ['offer-urls'],
                                                 'type': 'object'},
                      'ConsumeOfferDetailsResult': {'additionalProperties': False,
                                                    'properties': {'ConsumeOfferDetails': {'$ref': '#/definitions/ConsumeOfferDetails'},
+                                                                  'auth-token': {'type': 'string'},
                                                                   'error': {'$ref': '#/definitions/Error'},
                                                                   'external-controller': {'$ref': '#/definitions/ExternalControllerInfo'},
                                                                   'macaroon': {'$ref': '#/definitions/Macaroon'},
                                                                   'offer': {'$ref': '#/definitions/ApplicationOfferDetails'}},
                                                    'required': ['ConsumeOfferDetails'],
                                                    'type': 'object'},
                      'ConsumeOfferDetailsResults': {'additionalProperties': False,
```

### Comparing `juju-3.1.2.0/juju/client/_client5.py` & `juju-3.2.0.0/juju/client/_client5.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_client6.py` & `juju-3.2.0.0/juju/client/_client6.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_client7.py` & `juju-3.2.0.0/juju/client/_client7.py`

 * *Files 2% similar despite different names*

```diff
@@ -837,14 +837,15 @@
                                     'type': 'object'},
                      'Value': {'additionalProperties': False,
                                'properties': {'allocate-public-ip': {'type': 'boolean'},
                                               'arch': {'type': 'string'},
                                               'container': {'type': 'string'},
                                               'cores': {'type': 'integer'},
                                               'cpu-power': {'type': 'integer'},
+                                              'image-id': {'type': 'string'},
                                               'instance-role': {'type': 'string'},
                                               'instance-type': {'type': 'string'},
                                               'mem': {'type': 'integer'},
                                               'root-disk': {'type': 'integer'},
                                               'root-disk-source': {'type': 'string'},
                                               'spaces': {'items': {'type': 'string'},
                                                          'type': 'array'},
@@ -1591,40 +1592,36 @@
                                                                              'type': 'array'}},
                                          'type': 'object'},
                      'FanConfigEntry': {'additionalProperties': False,
                                         'properties': {'overlay': {'type': 'string'},
                                                        'underlay': {'type': 'string'}},
                                         'required': ['underlay', 'overlay'],
                                         'type': 'object'},
-                     'FirewallRule': {'additionalProperties': False,
-                                      'properties': {'known-service': {'type': 'string'},
-                                                     'whitelist-cidrs': {'items': {'type': 'string'},
-                                                                         'type': 'array'}},
-                                      'required': ['known-service'],
-                                      'type': 'object'},
-                     'KnownServiceArgs': {'additionalProperties': False,
-                                          'properties': {'known-services': {'items': {'type': 'string'},
-                                                                            'type': 'array'}},
-                                          'required': ['known-services'],
-                                          'type': 'object'},
+                     'IngressRule': {'additionalProperties': False,
+                                     'properties': {'port-range': {'$ref': '#/definitions/PortRange'},
+                                                    'source-cidrs': {'items': {'type': 'string'},
+                                                                     'type': 'array'}},
+                                     'required': ['port-range', 'source-cidrs'],
+                                     'type': 'object'},
+                     'IngressRulesResult': {'additionalProperties': False,
+                                            'properties': {'error': {'$ref': '#/definitions/Error'},
+                                                           'rules': {'items': {'$ref': '#/definitions/IngressRule'},
+                                                                     'type': 'array'}},
+                                            'required': ['rules'],
+                                            'type': 'object'},
                      'LifeResult': {'additionalProperties': False,
                                     'properties': {'error': {'$ref': '#/definitions/Error'},
                                                    'life': {'type': 'string'}},
                                     'required': ['life'],
                                     'type': 'object'},
                      'LifeResults': {'additionalProperties': False,
                                      'properties': {'results': {'items': {'$ref': '#/definitions/LifeResult'},
                                                                 'type': 'array'}},
                                      'required': ['results'],
                                      'type': 'object'},
-                     'ListFirewallRulesResults': {'additionalProperties': False,
-                                                  'properties': {'Rules': {'items': {'$ref': '#/definitions/FirewallRule'},
-                                                                           'type': 'array'}},
-                                                  'required': ['Rules'],
-                                                  'type': 'object'},
                      'Macaroon': {'additionalProperties': False, 'type': 'object'},
                      'MacaroonResult': {'additionalProperties': False,
                                         'properties': {'error': {'$ref': '#/definitions/Error'},
                                                        'result': {'$ref': '#/definitions/Macaroon'}},
                                         'type': 'object'},
                      'MacaroonResults': {'additionalProperties': False,
                                          'properties': {'results': {'items': {'$ref': '#/definitions/MacaroonResult'},
@@ -1809,21 +1806,14 @@
                                                                   'Result': {'$ref': '#/definitions/ControllerAPIInfoResults'}},
                                                    'type': 'object'},
                     'ControllerConfig': {'description': 'ControllerConfig returns '
                                                         "the controller's "
                                                         'configuration.',
                                          'properties': {'Result': {'$ref': '#/definitions/ControllerConfigResult'}},
                                          'type': 'object'},
-                    'FirewallRules': {'description': 'FirewallRules returns the '
-                                                     'firewall rules for the '
-                                                     'specified well known service '
-                                                     'types.',
-                                      'properties': {'Params': {'$ref': '#/definitions/KnownServiceArgs'},
-                                                     'Result': {'$ref': '#/definitions/ListFirewallRulesResults'}},
-                                      'type': 'object'},
                     'GetAssignedMachine': {'description': 'GetAssignedMachine '
                                                           'returns the assigned '
                                                           'machine tag (if any) '
                                                           'for\n'
                                                           'each given unit.',
                                            'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                                           'Result': {'$ref': '#/definitions/StringResults'}},
@@ -1863,14 +1853,21 @@
                                              'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                                             'Result': {'$ref': '#/definitions/MacaroonResults'}},
                                              'type': 'object'},
                     'ModelConfig': {'description': 'ModelConfig returns the '
                                                    "current model's configuration.",
                                     'properties': {'Result': {'$ref': '#/definitions/ModelConfigResult'}},
                                     'type': 'object'},
+                    'ModelFirewallRules': {'description': 'ModelFirewallRules '
+                                                          'returns the firewall '
+                                                          'rules that this model '
+                                                          'is\n'
+                                                          'configured to open',
+                                           'properties': {'Result': {'$ref': '#/definitions/IngressRulesResult'}},
+                                           'type': 'object'},
                     'OpenedMachinePortRanges': {'description': 'OpenedMachinePortRanges '
                                                                'returns a list of '
                                                                'the opened port '
                                                                'ranges for the\n'
                                                                'specified machines '
                                                                'where each result '
                                                                'is broken down by '
@@ -1984,14 +1981,24 @@
                                                                          'against '
                                                                          'the '
                                                                          'specified '
                                                                          'relations.',
                                                           'properties': {'Params': {'$ref': '#/definitions/Entities'},
                                                                          'Result': {'$ref': '#/definitions/StringsWatchResults'}},
                                                           'type': 'object'},
+                    'WatchModelFirewallRules': {'description': 'WatchModelFirewallRules '
+                                                               'returns a '
+                                                               'NotifyWatcher that '
+                                                               'notifies of\n'
+                                                               'potential changes '
+                                                               "to a model's "
+                                                               'configured '
+                                                               'firewall rules',
+                                                'properties': {'Result': {'$ref': '#/definitions/NotifyWatchResult'}},
+                                                'type': 'object'},
                     'WatchModelMachineStartTimes': {'description': 'WatchModelMachineStartTimes '
                                                                    'watches the '
                                                                    'non-container '
                                                                    'machines in '
                                                                    'the model\n'
                                                                    'for changes to '
                                                                    'the Life or '
@@ -2125,37 +2132,14 @@
                    params=_params)
 
         reply = await self.rpc(msg)
         return reply
 
 
 
-    @ReturnMapping(ListFirewallRulesResults)
-    async def FirewallRules(self, known_services=None):
-        '''
-        FirewallRules returns the firewall rules for the specified well known service types.
-
-        known_services : typing.Sequence[str]
-        Returns -> ListFirewallRulesResults
-        '''
-        if known_services is not None and not isinstance(known_services, (bytes, str, list)):
-            raise Exception("Expected known_services to be a Sequence, received: {}".format(type(known_services)))
-
-        # map input types to rpc msg
-        _params = dict()
-        msg = dict(type='Firewaller',
-                   request='FirewallRules',
-                   version=7,
-                   params=_params)
-        _params['known-services'] = known_services
-        reply = await self.rpc(msg)
-        return reply
-
-
-
     @ReturnMapping(StringResults)
     async def GetAssignedMachine(self, entities=None):
         '''
         GetAssignedMachine returns the assigned machine tag (if any) for
         each given unit.
 
         entities : typing.Sequence[~Entity]
@@ -2308,14 +2292,36 @@
                    params=_params)
 
         reply = await self.rpc(msg)
         return reply
 
 
 
+    @ReturnMapping(IngressRulesResult)
+    async def ModelFirewallRules(self):
+        '''
+        ModelFirewallRules returns the firewall rules that this model is
+        configured to open
+
+
+        Returns -> IngressRulesResult
+        '''
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='Firewaller',
+                   request='ModelFirewallRules',
+                   version=7,
+                   params=_params)
+
+        reply = await self.rpc(msg)
+        return reply
+
+
+
     @ReturnMapping(OpenMachinePortRangesResults)
     async def OpenedMachinePortRanges(self, entities=None):
         '''
         OpenedMachinePortRanges returns a list of the opened port ranges for the
         specified machines where each result is broken down by unit. The list of
         opened ports for each unit is further grouped by endpoint name and includes
         the subnet CIDRs that belong to the space that each endpoint is bound to.
@@ -2501,14 +2507,36 @@
                    params=_params)
         _params['entities'] = entities
         reply = await self.rpc(msg)
         return reply
 
 
 
+    @ReturnMapping(NotifyWatchResult)
+    async def WatchModelFirewallRules(self):
+        '''
+        WatchModelFirewallRules returns a NotifyWatcher that notifies of
+        potential changes to a model's configured firewall rules
+
+
+        Returns -> NotifyWatchResult
+        '''
+
+        # map input types to rpc msg
+        _params = dict()
+        msg = dict(type='Firewaller',
+                   request='WatchModelFirewallRules',
+                   version=7,
+                   params=_params)
+
+        reply = await self.rpc(msg)
+        return reply
+
+
+
     @ReturnMapping(StringsWatchResult)
     async def WatchModelMachineStartTimes(self):
         '''
         WatchModelMachineStartTimes watches the non-container machines in the model
         for changes to the Life or AgentStartTime fields and reports them as a batch.
```

### Comparing `juju-3.1.2.0/juju/client/_client8.py` & `juju-3.2.0.0/juju/client/_client8.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_client9.py` & `juju-3.2.0.0/juju/client/_client9.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/_definitions.py` & `juju-3.2.0.0/juju/client/_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3792,14 +3792,56 @@
             raise Exception("Expected images_ to be a Mapping, received: {}".format(type(images_)))
 
         self.images = images_
         self.unknown_fields = unknown_fields
 
 
 
+class CAASApplicationProvisionerConfig(Type):
+    _toSchema = {'unmanaged_applications': 'unmanaged-applications'}
+    _toPy = {'unmanaged-applications': 'unmanaged_applications'}
+    def __init__(self, unmanaged_applications=None, **unknown_fields):
+        '''
+        unmanaged_applications : Entities
+        '''
+        unmanaged_applications_ = Entities.from_json(unmanaged_applications) if unmanaged_applications else None
+
+        # Validate arguments against known Juju API types.
+        if unmanaged_applications_ is not None and not isinstance(unmanaged_applications_, (dict, Entities)):
+            raise Exception("Expected unmanaged_applications_ to be a Entities, received: {}".format(type(unmanaged_applications_)))
+
+        self.unmanaged_applications = unmanaged_applications_
+        self.unknown_fields = unknown_fields
+
+
+
+class CAASApplicationProvisionerConfigResult(Type):
+    _toSchema = {'error': 'error', 'provisioner_config': 'provisioner-config'}
+    _toPy = {'error': 'error', 'provisioner-config': 'provisioner_config'}
+    def __init__(self, error=None, provisioner_config=None, **unknown_fields):
+        '''
+        error : Error
+        provisioner_config : CAASApplicationProvisionerConfig
+        '''
+        error_ = Error.from_json(error) if error else None
+        provisioner_config_ = CAASApplicationProvisionerConfig.from_json(provisioner_config) if provisioner_config else None
+
+        # Validate arguments against known Juju API types.
+        if error_ is not None and not isinstance(error_, (dict, Error)):
+            raise Exception("Expected error_ to be a Error, received: {}".format(type(error_)))
+
+        if provisioner_config_ is not None and not isinstance(provisioner_config_, (dict, CAASApplicationProvisionerConfig)):
+            raise Exception("Expected provisioner_config_ to be a CAASApplicationProvisionerConfig, received: {}".format(type(provisioner_config_)))
+
+        self.error = error_
+        self.provisioner_config = provisioner_config_
+        self.unknown_fields = unknown_fields
+
+
+
 class CAASApplicationProvisioningInfo(Type):
     _toSchema = {'api_addresses': 'api-addresses', 'base': 'base', 'ca_cert': 'ca-cert', 'charm_modified_version': 'charm-modified-version', 'charm_url': 'charm-url', 'constraints': 'constraints', 'devices': 'devices', 'error': 'error', 'filesystems': 'filesystems', 'image_repo': 'image-repo', 'scale': 'scale', 'tags': 'tags', 'trust': 'trust', 'version': 'version', 'volumes': 'volumes'}
     _toPy = {'api-addresses': 'api_addresses', 'base': 'base', 'ca-cert': 'ca_cert', 'charm-modified-version': 'charm_modified_version', 'charm-url': 'charm_url', 'constraints': 'constraints', 'devices': 'devices', 'error': 'error', 'filesystems': 'filesystems', 'image-repo': 'image_repo', 'scale': 'scale', 'tags': 'tags', 'trust': 'trust', 'version': 'version', 'volumes': 'volumes'}
     def __init__(self, api_addresses=None, base=None, ca_cert=None, charm_modified_version=None, charm_url=None, constraints=None, devices=None, error=None, filesystems=None, image_repo=None, scale=None, tags=None, trust=None, version=None, volumes=None, **unknown_fields):
         '''
         api_addresses : typing.Sequence[str]
         base : Base
@@ -3912,14 +3954,86 @@
             raise Exception("Expected results_ to be a Sequence, received: {}".format(type(results_)))
 
         self.results = results_
         self.unknown_fields = unknown_fields
 
 
 
+class CAASApplicationProvisioningState(Type):
+    _toSchema = {'scale_target': 'scale-target', 'scaling': 'scaling'}
+    _toPy = {'scale-target': 'scale_target', 'scaling': 'scaling'}
+    def __init__(self, scale_target=None, scaling=None, **unknown_fields):
+        '''
+        scale_target : int
+        scaling : bool
+        '''
+        scale_target_ = scale_target
+        scaling_ = scaling
+
+        # Validate arguments against known Juju API types.
+        if scale_target_ is not None and not isinstance(scale_target_, int):
+            raise Exception("Expected scale_target_ to be a int, received: {}".format(type(scale_target_)))
+
+        if scaling_ is not None and not isinstance(scaling_, bool):
+            raise Exception("Expected scaling_ to be a bool, received: {}".format(type(scaling_)))
+
+        self.scale_target = scale_target_
+        self.scaling = scaling_
+        self.unknown_fields = unknown_fields
+
+
+
+class CAASApplicationProvisioningStateArg(Type):
+    _toSchema = {'application': 'application', 'provisioning_state': 'provisioning-state'}
+    _toPy = {'application': 'application', 'provisioning-state': 'provisioning_state'}
+    def __init__(self, application=None, provisioning_state=None, **unknown_fields):
+        '''
+        application : Entity
+        provisioning_state : CAASApplicationProvisioningState
+        '''
+        application_ = Entity.from_json(application) if application else None
+        provisioning_state_ = CAASApplicationProvisioningState.from_json(provisioning_state) if provisioning_state else None
+
+        # Validate arguments against known Juju API types.
+        if application_ is not None and not isinstance(application_, (dict, Entity)):
+            raise Exception("Expected application_ to be a Entity, received: {}".format(type(application_)))
+
+        if provisioning_state_ is not None and not isinstance(provisioning_state_, (dict, CAASApplicationProvisioningState)):
+            raise Exception("Expected provisioning_state_ to be a CAASApplicationProvisioningState, received: {}".format(type(provisioning_state_)))
+
+        self.application = application_
+        self.provisioning_state = provisioning_state_
+        self.unknown_fields = unknown_fields
+
+
+
+class CAASApplicationProvisioningStateResult(Type):
+    _toSchema = {'error': 'error', 'provisioning_state': 'provisioning-state'}
+    _toPy = {'error': 'error', 'provisioning-state': 'provisioning_state'}
+    def __init__(self, error=None, provisioning_state=None, **unknown_fields):
+        '''
+        error : Error
+        provisioning_state : CAASApplicationProvisioningState
+        '''
+        error_ = Error.from_json(error) if error else None
+        provisioning_state_ = CAASApplicationProvisioningState.from_json(provisioning_state) if provisioning_state else None
+
+        # Validate arguments against known Juju API types.
+        if error_ is not None and not isinstance(error_, (dict, Error)):
+            raise Exception("Expected error_ to be a Error, received: {}".format(type(error_)))
+
+        if provisioning_state_ is not None and not isinstance(provisioning_state_, (dict, CAASApplicationProvisioningState)):
+            raise Exception("Expected provisioning_state_ to be a CAASApplicationProvisioningState, received: {}".format(type(provisioning_state_)))
+
+        self.error = error_
+        self.provisioning_state = provisioning_state_
+        self.unknown_fields = unknown_fields
+
+
+
 class CAASUnitInfo(Type):
     _toSchema = {'tag': 'tag', 'unit_status': 'unit-status'}
     _toPy = {'tag': 'tag', 'unit-status': 'unit_status'}
     def __init__(self, tag=None, unit_status=None, **unknown_fields):
         '''
         tag : str
         unit_status : UnitStatus
@@ -4134,14 +4248,62 @@
             raise Exception("Expected model_credentials_ to be a Sequence, received: {}".format(type(model_credentials_)))
 
         self.model_credentials = model_credentials_
         self.unknown_fields = unknown_fields
 
 
 
+class ChangeSecretBackendArg(Type):
+    _toSchema = {'content': 'content', 'revision': 'revision', 'uri': 'uri'}
+    _toPy = {'content': 'content', 'revision': 'revision', 'uri': 'uri'}
+    def __init__(self, content=None, revision=None, uri=None, **unknown_fields):
+        '''
+        content : SecretContentParams
+        revision : int
+        uri : str
+        '''
+        content_ = SecretContentParams.from_json(content) if content else None
+        revision_ = revision
+        uri_ = uri
+
+        # Validate arguments against known Juju API types.
+        if content_ is not None and not isinstance(content_, (dict, SecretContentParams)):
+            raise Exception("Expected content_ to be a SecretContentParams, received: {}".format(type(content_)))
+
+        if revision_ is not None and not isinstance(revision_, int):
+            raise Exception("Expected revision_ to be a int, received: {}".format(type(revision_)))
+
+        if uri_ is not None and not isinstance(uri_, (bytes, str)):
+            raise Exception("Expected uri_ to be a str, received: {}".format(type(uri_)))
+
+        self.content = content_
+        self.revision = revision_
+        self.uri = uri_
+        self.unknown_fields = unknown_fields
+
+
+
+class ChangeSecretBackendArgs(Type):
+    _toSchema = {'args': 'args'}
+    _toPy = {'args': 'args'}
+    def __init__(self, args=None, **unknown_fields):
+        '''
+        args : typing.Sequence[~ChangeSecretBackendArg]
+        '''
+        args_ = [ChangeSecretBackendArg.from_json(o) for o in args or []]
+
+        # Validate arguments against known Juju API types.
+        if args_ is not None and not isinstance(args_, (bytes, str, list)):
+            raise Exception("Expected args_ to be a Sequence, received: {}".format(type(args_)))
+
+        self.args = args_
+        self.unknown_fields = unknown_fields
+
+
+
 class Channel(Type):
     _toSchema = {'branch': 'branch', 'risk': 'risk', 'track': 'track'}
     _toPy = {'branch': 'branch', 'risk': 'risk', 'track': 'track'}
     def __init__(self, branch=None, risk=None, track=None, **unknown_fields):
         '''
         branch : str
         risk : str
@@ -6415,35 +6577,37 @@
 
         self.results = results_
         self.unknown_fields = unknown_fields
 
 
 
 class ConsumeApplicationArg(Type):
-    _toSchema = {'application_alias': 'application-alias', 'application_description': 'application-description', 'applicationofferdetails': 'ApplicationOfferDetails', 'bindings': 'bindings', 'endpoints': 'endpoints', 'external_controller': 'external-controller', 'macaroon': 'macaroon', 'offer_name': 'offer-name', 'offer_url': 'offer-url', 'offer_uuid': 'offer-uuid', 'source_model_tag': 'source-model-tag', 'spaces': 'spaces', 'users': 'users'}
-    _toPy = {'ApplicationOfferDetails': 'applicationofferdetails', 'application-alias': 'application_alias', 'application-description': 'application_description', 'bindings': 'bindings', 'endpoints': 'endpoints', 'external-controller': 'external_controller', 'macaroon': 'macaroon', 'offer-name': 'offer_name', 'offer-url': 'offer_url', 'offer-uuid': 'offer_uuid', 'source-model-tag': 'source_model_tag', 'spaces': 'spaces', 'users': 'users'}
-    def __init__(self, applicationofferdetails=None, application_alias=None, application_description=None, bindings=None, endpoints=None, external_controller=None, macaroon=None, offer_name=None, offer_url=None, offer_uuid=None, source_model_tag=None, spaces=None, users=None, **unknown_fields):
+    _toSchema = {'application_alias': 'application-alias', 'application_description': 'application-description', 'applicationofferdetails': 'ApplicationOfferDetails', 'auth_token': 'auth-token', 'bindings': 'bindings', 'endpoints': 'endpoints', 'external_controller': 'external-controller', 'macaroon': 'macaroon', 'offer_name': 'offer-name', 'offer_url': 'offer-url', 'offer_uuid': 'offer-uuid', 'source_model_tag': 'source-model-tag', 'spaces': 'spaces', 'users': 'users'}
+    _toPy = {'ApplicationOfferDetails': 'applicationofferdetails', 'application-alias': 'application_alias', 'application-description': 'application_description', 'auth-token': 'auth_token', 'bindings': 'bindings', 'endpoints': 'endpoints', 'external-controller': 'external_controller', 'macaroon': 'macaroon', 'offer-name': 'offer_name', 'offer-url': 'offer_url', 'offer-uuid': 'offer_uuid', 'source-model-tag': 'source_model_tag', 'spaces': 'spaces', 'users': 'users'}
+    def __init__(self, applicationofferdetails=None, application_alias=None, application_description=None, auth_token=None, bindings=None, endpoints=None, external_controller=None, macaroon=None, offer_name=None, offer_url=None, offer_uuid=None, source_model_tag=None, spaces=None, users=None, **unknown_fields):
         '''
         applicationofferdetails : ApplicationOfferDetails
         application_alias : str
         application_description : str
+        auth_token : str
         bindings : typing.Mapping[str, str]
         endpoints : typing.Sequence[~RemoteEndpoint]
         external_controller : ExternalControllerInfo
         macaroon : Macaroon
         offer_name : str
         offer_url : str
         offer_uuid : str
         source_model_tag : str
         spaces : typing.Sequence[~RemoteSpace]
         users : typing.Sequence[~OfferUserDetails]
         '''
         applicationofferdetails_ = ApplicationOfferDetails.from_json(applicationofferdetails) if applicationofferdetails else None
         application_alias_ = application_alias
         application_description_ = application_description
+        auth_token_ = auth_token
         bindings_ = bindings
         endpoints_ = [RemoteEndpoint.from_json(o) for o in endpoints or []]
         external_controller_ = ExternalControllerInfo.from_json(external_controller) if external_controller else None
         macaroon_ = Macaroon.from_json(macaroon) if macaroon else None
         offer_name_ = offer_name
         offer_url_ = offer_url
         offer_uuid_ = offer_uuid
@@ -6457,14 +6621,17 @@
 
         if application_alias_ is not None and not isinstance(application_alias_, (bytes, str)):
             raise Exception("Expected application_alias_ to be a str, received: {}".format(type(application_alias_)))
 
         if application_description_ is not None and not isinstance(application_description_, (bytes, str)):
             raise Exception("Expected application_description_ to be a str, received: {}".format(type(application_description_)))
 
+        if auth_token_ is not None and not isinstance(auth_token_, (bytes, str)):
+            raise Exception("Expected auth_token_ to be a str, received: {}".format(type(auth_token_)))
+
         if bindings_ is not None and not isinstance(bindings_, dict):
             raise Exception("Expected bindings_ to be a Mapping, received: {}".format(type(bindings_)))
 
         if endpoints_ is not None and not isinstance(endpoints_, (bytes, str, list)):
             raise Exception("Expected endpoints_ to be a Sequence, received: {}".format(type(endpoints_)))
 
         if external_controller_ is not None and not isinstance(external_controller_, (dict, ExternalControllerInfo)):
@@ -6490,14 +6657,15 @@
 
         if users_ is not None and not isinstance(users_, (bytes, str, list)):
             raise Exception("Expected users_ to be a Sequence, received: {}".format(type(users_)))
 
         self.applicationofferdetails = applicationofferdetails_
         self.application_alias = application_alias_
         self.application_description = application_description_
+        self.auth_token = auth_token_
         self.bindings = bindings_
         self.endpoints = endpoints_
         self.external_controller = external_controller_
         self.macaroon = macaroon_
         self.offer_name = offer_name_
         self.offer_url = offer_url_
         self.offer_uuid = offer_uuid_
@@ -6523,36 +6691,42 @@
 
         self.args = args_
         self.unknown_fields = unknown_fields
 
 
 
 class ConsumeOfferDetails(Type):
-    _toSchema = {'external_controller': 'external-controller', 'macaroon': 'macaroon', 'offer': 'offer'}
-    _toPy = {'external-controller': 'external_controller', 'macaroon': 'macaroon', 'offer': 'offer'}
-    def __init__(self, external_controller=None, macaroon=None, offer=None, **unknown_fields):
+    _toSchema = {'auth_token': 'auth-token', 'external_controller': 'external-controller', 'macaroon': 'macaroon', 'offer': 'offer'}
+    _toPy = {'auth-token': 'auth_token', 'external-controller': 'external_controller', 'macaroon': 'macaroon', 'offer': 'offer'}
+    def __init__(self, auth_token=None, external_controller=None, macaroon=None, offer=None, **unknown_fields):
         '''
+        auth_token : str
         external_controller : ExternalControllerInfo
         macaroon : Macaroon
         offer : ApplicationOfferDetails
         '''
+        auth_token_ = auth_token
         external_controller_ = ExternalControllerInfo.from_json(external_controller) if external_controller else None
         macaroon_ = Macaroon.from_json(macaroon) if macaroon else None
         offer_ = ApplicationOfferDetails.from_json(offer) if offer else None
 
         # Validate arguments against known Juju API types.
+        if auth_token_ is not None and not isinstance(auth_token_, (bytes, str)):
+            raise Exception("Expected auth_token_ to be a str, received: {}".format(type(auth_token_)))
+
         if external_controller_ is not None and not isinstance(external_controller_, (dict, ExternalControllerInfo)):
             raise Exception("Expected external_controller_ to be a ExternalControllerInfo, received: {}".format(type(external_controller_)))
 
         if macaroon_ is not None and not isinstance(macaroon_, (dict, Macaroon)):
             raise Exception("Expected macaroon_ to be a Macaroon, received: {}".format(type(macaroon_)))
 
         if offer_ is not None and not isinstance(offer_, (dict, ApplicationOfferDetails)):
             raise Exception("Expected offer_ to be a ApplicationOfferDetails, received: {}".format(type(offer_)))
 
+        self.auth_token = auth_token_
         self.external_controller = external_controller_
         self.macaroon = macaroon_
         self.offer = offer_
         self.unknown_fields = unknown_fields
 
 
 
@@ -6577,47 +6751,53 @@
         self.offer_urls = offer_urls_
         self.user_tag = user_tag_
         self.unknown_fields = unknown_fields
 
 
 
 class ConsumeOfferDetailsResult(Type):
-    _toSchema = {'consumeofferdetails': 'ConsumeOfferDetails', 'error': 'error', 'external_controller': 'external-controller', 'macaroon': 'macaroon', 'offer': 'offer'}
-    _toPy = {'ConsumeOfferDetails': 'consumeofferdetails', 'error': 'error', 'external-controller': 'external_controller', 'macaroon': 'macaroon', 'offer': 'offer'}
-    def __init__(self, consumeofferdetails=None, error=None, external_controller=None, macaroon=None, offer=None, **unknown_fields):
+    _toSchema = {'auth_token': 'auth-token', 'consumeofferdetails': 'ConsumeOfferDetails', 'error': 'error', 'external_controller': 'external-controller', 'macaroon': 'macaroon', 'offer': 'offer'}
+    _toPy = {'ConsumeOfferDetails': 'consumeofferdetails', 'auth-token': 'auth_token', 'error': 'error', 'external-controller': 'external_controller', 'macaroon': 'macaroon', 'offer': 'offer'}
+    def __init__(self, consumeofferdetails=None, auth_token=None, error=None, external_controller=None, macaroon=None, offer=None, **unknown_fields):
         '''
         consumeofferdetails : ConsumeOfferDetails
+        auth_token : str
         error : Error
         external_controller : ExternalControllerInfo
         macaroon : Macaroon
         offer : ApplicationOfferDetails
         '''
         consumeofferdetails_ = ConsumeOfferDetails.from_json(consumeofferdetails) if consumeofferdetails else None
+        auth_token_ = auth_token
         error_ = Error.from_json(error) if error else None
         external_controller_ = ExternalControllerInfo.from_json(external_controller) if external_controller else None
         macaroon_ = Macaroon.from_json(macaroon) if macaroon else None
         offer_ = ApplicationOfferDetails.from_json(offer) if offer else None
 
         # Validate arguments against known Juju API types.
         if consumeofferdetails_ is not None and not isinstance(consumeofferdetails_, (dict, ConsumeOfferDetails)):
             raise Exception("Expected consumeofferdetails_ to be a ConsumeOfferDetails, received: {}".format(type(consumeofferdetails_)))
 
+        if auth_token_ is not None and not isinstance(auth_token_, (bytes, str)):
+            raise Exception("Expected auth_token_ to be a str, received: {}".format(type(auth_token_)))
+
         if error_ is not None and not isinstance(error_, (dict, Error)):
             raise Exception("Expected error_ to be a Error, received: {}".format(type(error_)))
 
         if external_controller_ is not None and not isinstance(external_controller_, (dict, ExternalControllerInfo)):
             raise Exception("Expected external_controller_ to be a ExternalControllerInfo, received: {}".format(type(external_controller_)))
 
         if macaroon_ is not None and not isinstance(macaroon_, (dict, Macaroon)):
             raise Exception("Expected macaroon_ to be a Macaroon, received: {}".format(type(macaroon_)))
 
         if offer_ is not None and not isinstance(offer_, (dict, ApplicationOfferDetails)):
             raise Exception("Expected offer_ to be a ApplicationOfferDetails, received: {}".format(type(offer_)))
 
         self.consumeofferdetails = consumeofferdetails_
+        self.auth_token = auth_token_
         self.error = error_
         self.external_controller = external_controller_
         self.macaroon = macaroon_
         self.offer = offer_
         self.unknown_fields = unknown_fields
 
 
@@ -7486,67 +7666,61 @@
         self.entity = entity_
         self.removed = removed_
         self.unknown_fields = unknown_fields
 
 
 
 class DeployFromRepositoryArg(Type):
-    _toSchema = {'applicationname': 'ApplicationName', 'attachstorage': 'AttachStorage', 'base': 'Base', 'channel': 'Channel', 'charmname': 'CharmName', 'configyaml': 'ConfigYAML', 'cons': 'Cons', 'devices': 'Devices', 'dryrun': 'DryRun', 'endpointbindings': 'EndpointBindings', 'force': 'Force', 'numunits': 'NumUnits', 'placement': 'Placement', 'resources': 'Resources', 'revision': 'Revision', 'storage': 'Storage', 'trust': 'Trust'}
-    _toPy = {'ApplicationName': 'applicationname', 'AttachStorage': 'attachstorage', 'Base': 'base', 'Channel': 'channel', 'CharmName': 'charmname', 'ConfigYAML': 'configyaml', 'Cons': 'cons', 'Devices': 'devices', 'DryRun': 'dryrun', 'EndpointBindings': 'endpointbindings', 'Force': 'force', 'NumUnits': 'numunits', 'Placement': 'placement', 'Resources': 'resources', 'Revision': 'revision', 'Storage': 'storage', 'Trust': 'trust'}
-    def __init__(self, applicationname=None, attachstorage=None, base=None, channel=None, charmname=None, configyaml=None, cons=None, devices=None, dryrun=None, endpointbindings=None, force=None, numunits=None, placement=None, resources=None, revision=None, storage=None, trust=None, **unknown_fields):
+    _toSchema = {'applicationname': 'ApplicationName', 'attachstorage': 'AttachStorage', 'base': 'base', 'channel': 'channel', 'charmname': 'CharmName', 'configyaml': 'ConfigYAML', 'cons': 'Cons', 'devices': 'Devices', 'dryrun': 'DryRun', 'endpoint_bindings': 'endpoint-bindings', 'force': 'force', 'num_units': 'num-units', 'placement': 'Placement', 'resources': 'resources', 'revision': 'revision', 'storage': 'Storage', 'trust': 'Trust'}
+    _toPy = {'ApplicationName': 'applicationname', 'AttachStorage': 'attachstorage', 'CharmName': 'charmname', 'ConfigYAML': 'configyaml', 'Cons': 'cons', 'Devices': 'devices', 'DryRun': 'dryrun', 'Placement': 'placement', 'Storage': 'storage', 'Trust': 'trust', 'base': 'base', 'channel': 'channel', 'endpoint-bindings': 'endpoint_bindings', 'force': 'force', 'num-units': 'num_units', 'resources': 'resources', 'revision': 'revision'}
+    def __init__(self, applicationname=None, attachstorage=None, charmname=None, configyaml=None, cons=None, devices=None, dryrun=None, placement=None, storage=None, trust=None, base=None, channel=None, endpoint_bindings=None, force=None, num_units=None, resources=None, revision=None, **unknown_fields):
         '''
         applicationname : str
         attachstorage : typing.Sequence[str]
-        base : Base
-        channel : Channel
         charmname : str
         configyaml : str
         cons : Value
         devices : typing.Mapping[str, ~Constraints]
         dryrun : bool
-        endpointbindings : typing.Mapping[str, str]
-        force : bool
-        numunits : int
         placement : typing.Sequence[~Placement]
-        resources : typing.Mapping[str, str]
-        revision : int
         storage : typing.Mapping[str, ~Constraints]
         trust : bool
+        base : Base
+        channel : str
+        endpoint_bindings : typing.Mapping[str, str]
+        force : bool
+        num_units : int
+        resources : typing.Mapping[str, str]
+        revision : int
         '''
         applicationname_ = applicationname
         attachstorage_ = attachstorage
-        base_ = Base.from_json(base) if base else None
-        channel_ = Channel.from_json(channel) if channel else None
         charmname_ = charmname
         configyaml_ = configyaml
         cons_ = Value.from_json(cons) if cons else None
         devices_ = {k: Constraints.from_json(v) for k, v in (devices or dict()).items()}
         dryrun_ = dryrun
-        endpointbindings_ = endpointbindings
-        force_ = force
-        numunits_ = numunits
         placement_ = [Placement.from_json(o) for o in placement or []]
-        resources_ = resources
-        revision_ = revision
         storage_ = {k: Constraints.from_json(v) for k, v in (storage or dict()).items()}
         trust_ = trust
+        base_ = Base.from_json(base) if base else None
+        channel_ = channel
+        endpoint_bindings_ = endpoint_bindings
+        force_ = force
+        num_units_ = num_units
+        resources_ = resources
+        revision_ = revision
 
         # Validate arguments against known Juju API types.
         if applicationname_ is not None and not isinstance(applicationname_, (bytes, str)):
             raise Exception("Expected applicationname_ to be a str, received: {}".format(type(applicationname_)))
 
         if attachstorage_ is not None and not isinstance(attachstorage_, (bytes, str, list)):
             raise Exception("Expected attachstorage_ to be a Sequence, received: {}".format(type(attachstorage_)))
 
-        if base_ is not None and not isinstance(base_, (dict, Base)):
-            raise Exception("Expected base_ to be a Base, received: {}".format(type(base_)))
-
-        if channel_ is not None and not isinstance(channel_, (dict, Channel)):
-            raise Exception("Expected channel_ to be a Channel, received: {}".format(type(channel_)))
-
         if charmname_ is not None and not isinstance(charmname_, (bytes, str)):
             raise Exception("Expected charmname_ to be a str, received: {}".format(type(charmname_)))
 
         if configyaml_ is not None and not isinstance(configyaml_, (bytes, str)):
             raise Exception("Expected configyaml_ to be a str, received: {}".format(type(configyaml_)))
 
         if cons_ is not None and not isinstance(cons_, (dict, Value)):
@@ -7554,55 +7728,61 @@
 
         if devices_ is not None and not isinstance(devices_, dict):
             raise Exception("Expected devices_ to be a Mapping, received: {}".format(type(devices_)))
 
         if dryrun_ is not None and not isinstance(dryrun_, bool):
             raise Exception("Expected dryrun_ to be a bool, received: {}".format(type(dryrun_)))
 
-        if endpointbindings_ is not None and not isinstance(endpointbindings_, dict):
-            raise Exception("Expected endpointbindings_ to be a Mapping, received: {}".format(type(endpointbindings_)))
+        if placement_ is not None and not isinstance(placement_, (bytes, str, list)):
+            raise Exception("Expected placement_ to be a Sequence, received: {}".format(type(placement_)))
+
+        if storage_ is not None and not isinstance(storage_, dict):
+            raise Exception("Expected storage_ to be a Mapping, received: {}".format(type(storage_)))
+
+        if trust_ is not None and not isinstance(trust_, bool):
+            raise Exception("Expected trust_ to be a bool, received: {}".format(type(trust_)))
+
+        if base_ is not None and not isinstance(base_, (dict, Base)):
+            raise Exception("Expected base_ to be a Base, received: {}".format(type(base_)))
+
+        if channel_ is not None and not isinstance(channel_, (bytes, str)):
+            raise Exception("Expected channel_ to be a str, received: {}".format(type(channel_)))
+
+        if endpoint_bindings_ is not None and not isinstance(endpoint_bindings_, dict):
+            raise Exception("Expected endpoint_bindings_ to be a Mapping, received: {}".format(type(endpoint_bindings_)))
 
         if force_ is not None and not isinstance(force_, bool):
             raise Exception("Expected force_ to be a bool, received: {}".format(type(force_)))
 
-        if numunits_ is not None and not isinstance(numunits_, int):
-            raise Exception("Expected numunits_ to be a int, received: {}".format(type(numunits_)))
-
-        if placement_ is not None and not isinstance(placement_, (bytes, str, list)):
-            raise Exception("Expected placement_ to be a Sequence, received: {}".format(type(placement_)))
+        if num_units_ is not None and not isinstance(num_units_, int):
+            raise Exception("Expected num_units_ to be a int, received: {}".format(type(num_units_)))
 
         if resources_ is not None and not isinstance(resources_, dict):
             raise Exception("Expected resources_ to be a Mapping, received: {}".format(type(resources_)))
 
         if revision_ is not None and not isinstance(revision_, int):
             raise Exception("Expected revision_ to be a int, received: {}".format(type(revision_)))
 
-        if storage_ is not None and not isinstance(storage_, dict):
-            raise Exception("Expected storage_ to be a Mapping, received: {}".format(type(storage_)))
-
-        if trust_ is not None and not isinstance(trust_, bool):
-            raise Exception("Expected trust_ to be a bool, received: {}".format(type(trust_)))
-
         self.applicationname = applicationname_
         self.attachstorage = attachstorage_
-        self.base = base_
-        self.channel = channel_
         self.charmname = charmname_
         self.configyaml = configyaml_
         self.cons = cons_
         self.devices = devices_
         self.dryrun = dryrun_
-        self.endpointbindings = endpointbindings_
-        self.force = force_
-        self.numunits = numunits_
         self.placement = placement_
-        self.resources = resources_
-        self.revision = revision_
         self.storage = storage_
         self.trust = trust_
+        self.base = base_
+        self.channel = channel_
+        self.endpoint_bindings = endpoint_bindings_
+        self.force = force_
+        self.num_units = num_units_
+        self.resources = resources_
+        self.revision = revision_
         self.unknown_fields = unknown_fields
 
 
 
 class DeployFromRepositoryArgs(Type):
     _toSchema = {'args': 'Args'}
     _toPy = {'Args': 'args'}
@@ -7617,33 +7797,81 @@
             raise Exception("Expected args_ to be a Sequence, received: {}".format(type(args_)))
 
         self.args = args_
         self.unknown_fields = unknown_fields
 
 
 
+class DeployFromRepositoryInfo(Type):
+    _toSchema = {'architecture': 'architecture', 'base': 'base', 'channel': 'channel', 'effective_channel': 'effective-channel', 'name': 'name', 'revision': 'revision'}
+    _toPy = {'architecture': 'architecture', 'base': 'base', 'channel': 'channel', 'effective-channel': 'effective_channel', 'name': 'name', 'revision': 'revision'}
+    def __init__(self, architecture=None, base=None, channel=None, effective_channel=None, name=None, revision=None, **unknown_fields):
+        '''
+        architecture : str
+        base : Base
+        channel : str
+        effective_channel : str
+        name : str
+        revision : int
+        '''
+        architecture_ = architecture
+        base_ = Base.from_json(base) if base else None
+        channel_ = channel
+        effective_channel_ = effective_channel
+        name_ = name
+        revision_ = revision
+
+        # Validate arguments against known Juju API types.
+        if architecture_ is not None and not isinstance(architecture_, (bytes, str)):
+            raise Exception("Expected architecture_ to be a str, received: {}".format(type(architecture_)))
+
+        if base_ is not None and not isinstance(base_, (dict, Base)):
+            raise Exception("Expected base_ to be a Base, received: {}".format(type(base_)))
+
+        if channel_ is not None and not isinstance(channel_, (bytes, str)):
+            raise Exception("Expected channel_ to be a str, received: {}".format(type(channel_)))
+
+        if effective_channel_ is not None and not isinstance(effective_channel_, (bytes, str)):
+            raise Exception("Expected effective_channel_ to be a str, received: {}".format(type(effective_channel_)))
+
+        if name_ is not None and not isinstance(name_, (bytes, str)):
+            raise Exception("Expected name_ to be a str, received: {}".format(type(name_)))
+
+        if revision_ is not None and not isinstance(revision_, int):
+            raise Exception("Expected revision_ to be a int, received: {}".format(type(revision_)))
+
+        self.architecture = architecture_
+        self.base = base_
+        self.channel = channel_
+        self.effective_channel = effective_channel_
+        self.name = name_
+        self.revision = revision_
+        self.unknown_fields = unknown_fields
+
+
+
 class DeployFromRepositoryResult(Type):
     _toSchema = {'errors': 'Errors', 'info': 'Info', 'pendingresourceuploads': 'PendingResourceUploads'}
     _toPy = {'Errors': 'errors', 'Info': 'info', 'PendingResourceUploads': 'pendingresourceuploads'}
     def __init__(self, errors=None, info=None, pendingresourceuploads=None, **unknown_fields):
         '''
         errors : typing.Sequence[~Error]
-        info : typing.Sequence[str]
+        info : DeployFromRepositoryInfo
         pendingresourceuploads : typing.Sequence[~PendingResourceUpload]
         '''
         errors_ = [Error.from_json(o) for o in errors or []]
-        info_ = info
+        info_ = DeployFromRepositoryInfo.from_json(info) if info else None
         pendingresourceuploads_ = [PendingResourceUpload.from_json(o) for o in pendingresourceuploads or []]
 
         # Validate arguments against known Juju API types.
         if errors_ is not None and not isinstance(errors_, (bytes, str, list)):
             raise Exception("Expected errors_ to be a Sequence, received: {}".format(type(errors_)))
 
-        if info_ is not None and not isinstance(info_, (bytes, str, list)):
-            raise Exception("Expected info_ to be a Sequence, received: {}".format(type(info_)))
+        if info_ is not None and not isinstance(info_, (dict, DeployFromRepositoryInfo)):
+            raise Exception("Expected info_ to be a DeployFromRepositoryInfo, received: {}".format(type(info_)))
 
         if pendingresourceuploads_ is not None and not isinstance(pendingresourceuploads_, (bytes, str, list)):
             raise Exception("Expected pendingresourceuploads_ to be a Sequence, received: {}".format(type(pendingresourceuploads_)))
 
         self.errors = errors_
         self.info = info_
         self.pendingresourceuploads = pendingresourceuploads_
@@ -11328,14 +11556,62 @@
             raise Exception("Expected changes_ to be a Sequence, received: {}".format(type(changes_)))
 
         self.changes = changes_
         self.unknown_fields = unknown_fields
 
 
 
+class IngressRule(Type):
+    _toSchema = {'port_range': 'port-range', 'source_cidrs': 'source-cidrs'}
+    _toPy = {'port-range': 'port_range', 'source-cidrs': 'source_cidrs'}
+    def __init__(self, port_range=None, source_cidrs=None, **unknown_fields):
+        '''
+        port_range : PortRange
+        source_cidrs : typing.Sequence[str]
+        '''
+        port_range_ = PortRange.from_json(port_range) if port_range else None
+        source_cidrs_ = source_cidrs
+
+        # Validate arguments against known Juju API types.
+        if port_range_ is not None and not isinstance(port_range_, (dict, PortRange)):
+            raise Exception("Expected port_range_ to be a PortRange, received: {}".format(type(port_range_)))
+
+        if source_cidrs_ is not None and not isinstance(source_cidrs_, (bytes, str, list)):
+            raise Exception("Expected source_cidrs_ to be a Sequence, received: {}".format(type(source_cidrs_)))
+
+        self.port_range = port_range_
+        self.source_cidrs = source_cidrs_
+        self.unknown_fields = unknown_fields
+
+
+
+class IngressRulesResult(Type):
+    _toSchema = {'error': 'error', 'rules': 'rules'}
+    _toPy = {'error': 'error', 'rules': 'rules'}
+    def __init__(self, error=None, rules=None, **unknown_fields):
+        '''
+        error : Error
+        rules : typing.Sequence[~IngressRule]
+        '''
+        error_ = Error.from_json(error) if error else None
+        rules_ = [IngressRule.from_json(o) for o in rules or []]
+
+        # Validate arguments against known Juju API types.
+        if error_ is not None and not isinstance(error_, (dict, Error)):
+            raise Exception("Expected error_ to be a Error, received: {}".format(type(error_)))
+
+        if rules_ is not None and not isinstance(rules_, (bytes, str, list)):
+            raise Exception("Expected rules_ to be a Sequence, received: {}".format(type(rules_)))
+
+        self.error = error_
+        self.rules = rules_
+        self.unknown_fields = unknown_fields
+
+
+
 class InitiateMigrationArgs(Type):
     _toSchema = {'specs': 'specs'}
     _toPy = {'specs': 'specs'}
     def __init__(self, specs=None, **unknown_fields):
         '''
         specs : typing.Sequence[~MigrationSpec]
         '''
@@ -12336,14 +12612,32 @@
         self.config = config_
         self.description = description_
         self.devices = devices_
         self.unknown_fields = unknown_fields
 
 
 
+class LatestSecretRevisionChanges(Type):
+    _toSchema = {'changes': 'changes'}
+    _toPy = {'changes': 'changes'}
+    def __init__(self, changes=None, **unknown_fields):
+        '''
+        changes : typing.Sequence[~SecretRevisionChange]
+        '''
+        changes_ = [SecretRevisionChange.from_json(o) for o in changes or []]
+
+        # Validate arguments against known Juju API types.
+        if changes_ is not None and not isinstance(changes_, (bytes, str, list)):
+            raise Exception("Expected changes_ to be a Sequence, received: {}".format(type(changes_)))
+
+        self.changes = changes_
+        self.unknown_fields = unknown_fields
+
+
+
 class LeaseOperationCommand(Type):
     _toSchema = {'duration': 'duration', 'holder': 'holder', 'lease': 'lease', 'model_uuid': 'model-uuid', 'namespace': 'namespace', 'new_time': 'new-time', 'old_time': 'old-time', 'operation': 'operation', 'pin_entity': 'pin-entity', 'version': 'version'}
     _toPy = {'duration': 'duration', 'holder': 'holder', 'lease': 'lease', 'model-uuid': 'model_uuid', 'namespace': 'namespace', 'new-time': 'new_time', 'old-time': 'old_time', 'operation': 'operation', 'pin-entity': 'pin_entity', 'version': 'version'}
     def __init__(self, duration=None, holder=None, lease=None, model_uuid=None, namespace=None, new_time=None, old_time=None, operation=None, pin_entity=None, version=None, **unknown_fields):
         '''
         duration : int
         holder : str
@@ -13015,34 +13309,36 @@
 
         self.params = params_
         self.unknown_fields = unknown_fields
 
 
 
 class LoginRequest(Type):
-    _toSchema = {'auth_tag': 'auth-tag', 'bakery_version': 'bakery-version', 'cli_args': 'cli-args', 'client_version': 'client-version', 'credentials': 'credentials', 'macaroons': 'macaroons', 'nonce': 'nonce', 'user_data': 'user-data'}
-    _toPy = {'auth-tag': 'auth_tag', 'bakery-version': 'bakery_version', 'cli-args': 'cli_args', 'client-version': 'client_version', 'credentials': 'credentials', 'macaroons': 'macaroons', 'nonce': 'nonce', 'user-data': 'user_data'}
-    def __init__(self, auth_tag=None, bakery_version=None, cli_args=None, client_version=None, credentials=None, macaroons=None, nonce=None, user_data=None, **unknown_fields):
+    _toSchema = {'auth_tag': 'auth-tag', 'bakery_version': 'bakery-version', 'cli_args': 'cli-args', 'client_version': 'client-version', 'credentials': 'credentials', 'macaroons': 'macaroons', 'nonce': 'nonce', 'token': 'token', 'user_data': 'user-data'}
+    _toPy = {'auth-tag': 'auth_tag', 'bakery-version': 'bakery_version', 'cli-args': 'cli_args', 'client-version': 'client_version', 'credentials': 'credentials', 'macaroons': 'macaroons', 'nonce': 'nonce', 'token': 'token', 'user-data': 'user_data'}
+    def __init__(self, auth_tag=None, bakery_version=None, cli_args=None, client_version=None, credentials=None, macaroons=None, nonce=None, token=None, user_data=None, **unknown_fields):
         '''
         auth_tag : str
         bakery_version : int
         cli_args : str
         client_version : str
         credentials : str
         macaroons : typing.Sequence[~Macaroon]
         nonce : str
+        token : str
         user_data : str
         '''
         auth_tag_ = auth_tag
         bakery_version_ = bakery_version
         cli_args_ = cli_args
         client_version_ = client_version
         credentials_ = credentials
         macaroons_ = [Macaroon.from_json(o) for o in macaroons or []]
         nonce_ = nonce
+        token_ = token
         user_data_ = user_data
 
         # Validate arguments against known Juju API types.
         if auth_tag_ is not None and not isinstance(auth_tag_, (bytes, str)):
             raise Exception("Expected auth_tag_ to be a str, received: {}".format(type(auth_tag_)))
 
         if bakery_version_ is not None and not isinstance(bakery_version_, int):
@@ -13059,24 +13355,28 @@
 
         if macaroons_ is not None and not isinstance(macaroons_, (bytes, str, list)):
             raise Exception("Expected macaroons_ to be a Sequence, received: {}".format(type(macaroons_)))
 
         if nonce_ is not None and not isinstance(nonce_, (bytes, str)):
             raise Exception("Expected nonce_ to be a str, received: {}".format(type(nonce_)))
 
+        if token_ is not None and not isinstance(token_, (bytes, str)):
+            raise Exception("Expected token_ to be a str, received: {}".format(type(token_)))
+
         if user_data_ is not None and not isinstance(user_data_, (bytes, str)):
             raise Exception("Expected user_data_ to be a str, received: {}".format(type(user_data_)))
 
         self.auth_tag = auth_tag_
         self.bakery_version = bakery_version_
         self.cli_args = cli_args_
         self.client_version = client_version_
         self.credentials = credentials_
         self.macaroons = macaroons_
         self.nonce = nonce_
+        self.token = token_
         self.user_data = user_data_
         self.unknown_fields = unknown_fields
 
 
 
 class LoginResult(Type):
     _toSchema = {'bakery_discharge_required': 'bakery-discharge-required', 'controller_tag': 'controller-tag', 'discharge_required': 'discharge-required', 'discharge_required_error': 'discharge-required-error', 'facades': 'facades', 'model_tag': 'model-tag', 'public_dns_name': 'public-dns-name', 'server_version': 'server-version', 'servers': 'servers', 'user_info': 'user-info'}
@@ -17777,45 +18077,45 @@
 
         self.results = results_
         self.unknown_fields = unknown_fields
 
 
 
 class PendingResourceUpload(Type):
-    _toSchema = {'filename': 'Filename', 'name': 'Name', 'pendingid': 'PendingID', 'type_': 'Type'}
-    _toPy = {'Filename': 'filename', 'Name': 'name', 'PendingID': 'pendingid', 'Type': 'type_'}
-    def __init__(self, filename=None, name=None, pendingid=None, type_=None, **unknown_fields):
+    _toSchema = {'filename': 'Filename', 'name': 'Name', 'pending_id': 'pending-id', 'type_': 'Type'}
+    _toPy = {'Filename': 'filename', 'Name': 'name', 'Type': 'type_', 'pending-id': 'pending_id'}
+    def __init__(self, filename=None, name=None, type_=None, pending_id=None, **unknown_fields):
         '''
         filename : str
         name : str
-        pendingid : str
         type_ : str
+        pending_id : str
         '''
         filename_ = filename
         name_ = name
-        pendingid_ = pendingid
         type__ = type_
+        pending_id_ = pending_id
 
         # Validate arguments against known Juju API types.
         if filename_ is not None and not isinstance(filename_, (bytes, str)):
             raise Exception("Expected filename_ to be a str, received: {}".format(type(filename_)))
 
         if name_ is not None and not isinstance(name_, (bytes, str)):
             raise Exception("Expected name_ to be a str, received: {}".format(type(name_)))
 
-        if pendingid_ is not None and not isinstance(pendingid_, (bytes, str)):
-            raise Exception("Expected pendingid_ to be a str, received: {}".format(type(pendingid_)))
-
         if type__ is not None and not isinstance(type__, (bytes, str)):
             raise Exception("Expected type__ to be a str, received: {}".format(type(type__)))
 
+        if pending_id_ is not None and not isinstance(pending_id_, (bytes, str)):
+            raise Exception("Expected pending_id_ to be a str, received: {}".format(type(pending_id_)))
+
         self.filename = filename_
         self.name = name_
-        self.pendingid = pendingid_
         self.type_ = type__
+        self.pending_id = pending_id_
         self.unknown_fields = unknown_fields
 
 
 
 class PhaseResult(Type):
     _toSchema = {'error': 'error', 'phase': 'phase'}
     _toPy = {'error': 'error', 'phase': 'phase'}
@@ -17897,26 +18197,32 @@
 
         self.results = results_
         self.unknown_fields = unknown_fields
 
 
 
 class PinnedLeadershipResult(Type):
-    _toSchema = {'result': 'result'}
-    _toPy = {'result': 'result'}
-    def __init__(self, result=None, **unknown_fields):
+    _toSchema = {'error': 'error', 'result': 'result'}
+    _toPy = {'error': 'error', 'result': 'result'}
+    def __init__(self, error=None, result=None, **unknown_fields):
         '''
+        error : Error
         result : typing.Mapping[str, typing.Sequence[str]]
         '''
+        error_ = Error.from_json(error) if error else None
         result_ = result
 
         # Validate arguments against known Juju API types.
+        if error_ is not None and not isinstance(error_, (dict, Error)):
+            raise Exception("Expected error_ to be a Error, received: {}".format(type(error_)))
+
         if result_ is not None and not isinstance(result_, dict):
             raise Exception("Expected result_ to be a Mapping, received: {}".format(type(result_)))
 
+        self.error = error_
         self.result = result_
         self.unknown_fields = unknown_fields
 
 
 
 class Placement(Type):
     _toSchema = {'directive': 'directive', 'scope': 'scope'}
@@ -18686,44 +18992,49 @@
         self.region_name = region_name_
         self.value = value_
         self.unknown_fields = unknown_fields
 
 
 
 class RegisterRemoteRelationArg(Type):
-    _toSchema = {'application_token': 'application-token', 'bakery_version': 'bakery-version', 'consume_version': 'consume-version', 'local_endpoint_name': 'local-endpoint-name', 'macaroons': 'macaroons', 'offer_uuid': 'offer-uuid', 'relation_token': 'relation-token', 'remote_endpoint': 'remote-endpoint', 'remote_space': 'remote-space', 'source_model_tag': 'source-model-tag'}
-    _toPy = {'application-token': 'application_token', 'bakery-version': 'bakery_version', 'consume-version': 'consume_version', 'local-endpoint-name': 'local_endpoint_name', 'macaroons': 'macaroons', 'offer-uuid': 'offer_uuid', 'relation-token': 'relation_token', 'remote-endpoint': 'remote_endpoint', 'remote-space': 'remote_space', 'source-model-tag': 'source_model_tag'}
-    def __init__(self, application_token=None, bakery_version=None, consume_version=None, local_endpoint_name=None, macaroons=None, offer_uuid=None, relation_token=None, remote_endpoint=None, remote_space=None, source_model_tag=None, **unknown_fields):
+    _toSchema = {'application_token': 'application-token', 'auth_token': 'auth-token', 'bakery_version': 'bakery-version', 'consume_version': 'consume-version', 'local_endpoint_name': 'local-endpoint-name', 'macaroons': 'macaroons', 'offer_uuid': 'offer-uuid', 'relation_token': 'relation-token', 'remote_endpoint': 'remote-endpoint', 'remote_space': 'remote-space', 'source_model_tag': 'source-model-tag'}
+    _toPy = {'application-token': 'application_token', 'auth-token': 'auth_token', 'bakery-version': 'bakery_version', 'consume-version': 'consume_version', 'local-endpoint-name': 'local_endpoint_name', 'macaroons': 'macaroons', 'offer-uuid': 'offer_uuid', 'relation-token': 'relation_token', 'remote-endpoint': 'remote_endpoint', 'remote-space': 'remote_space', 'source-model-tag': 'source_model_tag'}
+    def __init__(self, application_token=None, auth_token=None, bakery_version=None, consume_version=None, local_endpoint_name=None, macaroons=None, offer_uuid=None, relation_token=None, remote_endpoint=None, remote_space=None, source_model_tag=None, **unknown_fields):
         '''
         application_token : str
+        auth_token : str
         bakery_version : int
         consume_version : int
         local_endpoint_name : str
         macaroons : typing.Sequence[~Macaroon]
         offer_uuid : str
         relation_token : str
         remote_endpoint : RemoteEndpoint
         remote_space : RemoteSpace
         source_model_tag : str
         '''
         application_token_ = application_token
+        auth_token_ = auth_token
         bakery_version_ = bakery_version
         consume_version_ = consume_version
         local_endpoint_name_ = local_endpoint_name
         macaroons_ = [Macaroon.from_json(o) for o in macaroons or []]
         offer_uuid_ = offer_uuid
         relation_token_ = relation_token
         remote_endpoint_ = RemoteEndpoint.from_json(remote_endpoint) if remote_endpoint else None
         remote_space_ = RemoteSpace.from_json(remote_space) if remote_space else None
         source_model_tag_ = source_model_tag
 
         # Validate arguments against known Juju API types.
         if application_token_ is not None and not isinstance(application_token_, (bytes, str)):
             raise Exception("Expected application_token_ to be a str, received: {}".format(type(application_token_)))
 
+        if auth_token_ is not None and not isinstance(auth_token_, (bytes, str)):
+            raise Exception("Expected auth_token_ to be a str, received: {}".format(type(auth_token_)))
+
         if bakery_version_ is not None and not isinstance(bakery_version_, int):
             raise Exception("Expected bakery_version_ to be a int, received: {}".format(type(bakery_version_)))
 
         if consume_version_ is not None and not isinstance(consume_version_, int):
             raise Exception("Expected consume_version_ to be a int, received: {}".format(type(consume_version_)))
 
         if local_endpoint_name_ is not None and not isinstance(local_endpoint_name_, (bytes, str)):
@@ -18744,14 +19055,15 @@
         if remote_space_ is not None and not isinstance(remote_space_, (dict, RemoteSpace)):
             raise Exception("Expected remote_space_ to be a RemoteSpace, received: {}".format(type(remote_space_)))
 
         if source_model_tag_ is not None and not isinstance(source_model_tag_, (bytes, str)):
             raise Exception("Expected source_model_tag_ to be a str, received: {}".format(type(source_model_tag_)))
 
         self.application_token = application_token_
+        self.auth_token = auth_token_
         self.bakery_version = bakery_version_
         self.consume_version = consume_version_
         self.local_endpoint_name = local_endpoint_name_
         self.macaroons = macaroons_
         self.offer_uuid = offer_uuid_
         self.relation_token = relation_token_
         self.remote_endpoint = remote_endpoint_
@@ -21542,51 +21854,33 @@
         self.model_name = model_name_
         self.model_uuid = model_uuid_
         self.unknown_fields = unknown_fields
 
 
 
 class SecretBackendConfigResults(Type):
-    _toSchema = {'active_id': 'active-id', 'configs': 'configs', 'model_controller': 'model-controller', 'model_name': 'model-name', 'model_uuid': 'model-uuid'}
-    _toPy = {'active-id': 'active_id', 'configs': 'configs', 'model-controller': 'model_controller', 'model-name': 'model_name', 'model-uuid': 'model_uuid'}
-    def __init__(self, active_id=None, configs=None, model_controller=None, model_name=None, model_uuid=None, **unknown_fields):
+    _toSchema = {'active_id': 'active-id', 'results': 'results'}
+    _toPy = {'active-id': 'active_id', 'results': 'results'}
+    def __init__(self, active_id=None, results=None, **unknown_fields):
         '''
         active_id : str
-        configs : typing.Mapping[str, ~SecretBackendConfig]
-        model_controller : str
-        model_name : str
-        model_uuid : str
+        results : typing.Mapping[str, ~SecretBackendConfigResult]
         '''
         active_id_ = active_id
-        configs_ = {k: SecretBackendConfig.from_json(v) for k, v in (configs or dict()).items()}
-        model_controller_ = model_controller
-        model_name_ = model_name
-        model_uuid_ = model_uuid
+        results_ = {k: SecretBackendConfigResult.from_json(v) for k, v in (results or dict()).items()}
 
         # Validate arguments against known Juju API types.
         if active_id_ is not None and not isinstance(active_id_, (bytes, str)):
             raise Exception("Expected active_id_ to be a str, received: {}".format(type(active_id_)))
 
-        if configs_ is not None and not isinstance(configs_, dict):
-            raise Exception("Expected configs_ to be a Mapping, received: {}".format(type(configs_)))
-
-        if model_controller_ is not None and not isinstance(model_controller_, (bytes, str)):
-            raise Exception("Expected model_controller_ to be a str, received: {}".format(type(model_controller_)))
-
-        if model_name_ is not None and not isinstance(model_name_, (bytes, str)):
-            raise Exception("Expected model_name_ to be a str, received: {}".format(type(model_name_)))
-
-        if model_uuid_ is not None and not isinstance(model_uuid_, (bytes, str)):
-            raise Exception("Expected model_uuid_ to be a str, received: {}".format(type(model_uuid_)))
+        if results_ is not None and not isinstance(results_, dict):
+            raise Exception("Expected results_ to be a Mapping, received: {}".format(type(results_)))
 
         self.active_id = active_id_
-        self.configs = configs_
-        self.model_controller = model_controller_
-        self.model_name = model_name_
-        self.model_uuid = model_uuid_
+        self.results = results_
         self.unknown_fields = unknown_fields
 
 
 
 class SecretBackendResult(Type):
     _toSchema = {'error': 'error', 'id_': 'id', 'message': 'message', 'num_secrets': 'num-secrets', 'result': 'result', 'status': 'status'}
     _toPy = {'error': 'error', 'id': 'id_', 'message': 'message', 'num-secrets': 'num_secrets', 'result': 'result', 'status': 'status'}
@@ -21764,33 +22058,45 @@
         self.data = data_
         self.value_ref = value_ref_
         self.unknown_fields = unknown_fields
 
 
 
 class SecretContentResult(Type):
-    _toSchema = {'content': 'content', 'error': 'error'}
-    _toPy = {'content': 'content', 'error': 'error'}
-    def __init__(self, content=None, error=None, **unknown_fields):
+    _toSchema = {'backend_config': 'backend-config', 'content': 'content', 'error': 'error', 'latest_revision': 'latest-revision'}
+    _toPy = {'backend-config': 'backend_config', 'content': 'content', 'error': 'error', 'latest-revision': 'latest_revision'}
+    def __init__(self, backend_config=None, content=None, error=None, latest_revision=None, **unknown_fields):
         '''
+        backend_config : SecretBackendConfigResult
         content : SecretContentParams
         error : Error
+        latest_revision : int
         '''
+        backend_config_ = SecretBackendConfigResult.from_json(backend_config) if backend_config else None
         content_ = SecretContentParams.from_json(content) if content else None
         error_ = Error.from_json(error) if error else None
+        latest_revision_ = latest_revision
 
         # Validate arguments against known Juju API types.
+        if backend_config_ is not None and not isinstance(backend_config_, (dict, SecretBackendConfigResult)):
+            raise Exception("Expected backend_config_ to be a SecretBackendConfigResult, received: {}".format(type(backend_config_)))
+
         if content_ is not None and not isinstance(content_, (dict, SecretContentParams)):
             raise Exception("Expected content_ to be a SecretContentParams, received: {}".format(type(content_)))
 
         if error_ is not None and not isinstance(error_, (dict, Error)):
             raise Exception("Expected error_ to be a Error, received: {}".format(type(error_)))
 
+        if latest_revision_ is not None and not isinstance(latest_revision_, int):
+            raise Exception("Expected latest_revision_ to be a int, received: {}".format(type(latest_revision_)))
+
+        self.backend_config = backend_config_
         self.content = content_
         self.error = error_
+        self.latest_revision = latest_revision_
         self.unknown_fields = unknown_fields
 
 
 
 class SecretContentResults(Type):
     _toSchema = {'results': 'results'}
     _toPy = {'results': 'results'}
@@ -21883,14 +22189,86 @@
         self.pending_delete = pending_delete_
         self.revisions = revisions_
         self.uri = uri_
         self.unknown_fields = unknown_fields
 
 
 
+class SecretRevisionChange(Type):
+    _toSchema = {'revision': 'revision', 'uri': 'uri'}
+    _toPy = {'revision': 'revision', 'uri': 'uri'}
+    def __init__(self, revision=None, uri=None, **unknown_fields):
+        '''
+        revision : int
+        uri : str
+        '''
+        revision_ = revision
+        uri_ = uri
+
+        # Validate arguments against known Juju API types.
+        if revision_ is not None and not isinstance(revision_, int):
+            raise Exception("Expected revision_ to be a int, received: {}".format(type(revision_)))
+
+        if uri_ is not None and not isinstance(uri_, (bytes, str)):
+            raise Exception("Expected uri_ to be a str, received: {}".format(type(uri_)))
+
+        self.revision = revision_
+        self.uri = uri_
+        self.unknown_fields = unknown_fields
+
+
+
+class SecretRevisionWatchResult(Type):
+    _toSchema = {'changes': 'changes', 'error': 'error', 'watcher_id': 'watcher-id'}
+    _toPy = {'changes': 'changes', 'error': 'error', 'watcher-id': 'watcher_id'}
+    def __init__(self, changes=None, error=None, watcher_id=None, **unknown_fields):
+        '''
+        changes : typing.Sequence[~SecretRevisionChange]
+        error : Error
+        watcher_id : str
+        '''
+        changes_ = [SecretRevisionChange.from_json(o) for o in changes or []]
+        error_ = Error.from_json(error) if error else None
+        watcher_id_ = watcher_id
+
+        # Validate arguments against known Juju API types.
+        if changes_ is not None and not isinstance(changes_, (bytes, str, list)):
+            raise Exception("Expected changes_ to be a Sequence, received: {}".format(type(changes_)))
+
+        if error_ is not None and not isinstance(error_, (dict, Error)):
+            raise Exception("Expected error_ to be a Error, received: {}".format(type(error_)))
+
+        if watcher_id_ is not None and not isinstance(watcher_id_, (bytes, str)):
+            raise Exception("Expected watcher_id_ to be a str, received: {}".format(type(watcher_id_)))
+
+        self.changes = changes_
+        self.error = error_
+        self.watcher_id = watcher_id_
+        self.unknown_fields = unknown_fields
+
+
+
+class SecretRevisionWatchResults(Type):
+    _toSchema = {'results': 'results'}
+    _toPy = {'results': 'results'}
+    def __init__(self, results=None, **unknown_fields):
+        '''
+        results : typing.Sequence[~SecretRevisionWatchResult]
+        '''
+        results_ = [SecretRevisionWatchResult.from_json(o) for o in results or []]
+
+        # Validate arguments against known Juju API types.
+        if results_ is not None and not isinstance(results_, (bytes, str, list)):
+            raise Exception("Expected results_ to be a Sequence, received: {}".format(type(results_)))
+
+        self.results = results_
+        self.unknown_fields = unknown_fields
+
+
+
 class SecretRotatedArg(Type):
     _toSchema = {'original_revision': 'original-revision', 'skip': 'skip', 'uri': 'uri'}
     _toPy = {'original-revision': 'original_revision', 'skip': 'skip', 'uri': 'uri'}
     def __init__(self, original_revision=None, skip=None, uri=None, **unknown_fields):
         '''
         original_revision : int
         skip : bool
@@ -26425,23 +26803,24 @@
 
         self.user_models = user_models_
         self.unknown_fields = unknown_fields
 
 
 
 class Value(Type):
-    _toSchema = {'allocate_public_ip': 'allocate-public-ip', 'arch': 'arch', 'container': 'container', 'cores': 'cores', 'cpu_power': 'cpu-power', 'instance_role': 'instance-role', 'instance_type': 'instance-type', 'mem': 'mem', 'root_disk': 'root-disk', 'root_disk_source': 'root-disk-source', 'spaces': 'spaces', 'tags': 'tags', 'virt_type': 'virt-type', 'zones': 'zones'}
-    _toPy = {'allocate-public-ip': 'allocate_public_ip', 'arch': 'arch', 'container': 'container', 'cores': 'cores', 'cpu-power': 'cpu_power', 'instance-role': 'instance_role', 'instance-type': 'instance_type', 'mem': 'mem', 'root-disk': 'root_disk', 'root-disk-source': 'root_disk_source', 'spaces': 'spaces', 'tags': 'tags', 'virt-type': 'virt_type', 'zones': 'zones'}
-    def __init__(self, allocate_public_ip=None, arch=None, container=None, cores=None, cpu_power=None, instance_role=None, instance_type=None, mem=None, root_disk=None, root_disk_source=None, spaces=None, tags=None, virt_type=None, zones=None, **unknown_fields):
+    _toSchema = {'allocate_public_ip': 'allocate-public-ip', 'arch': 'arch', 'container': 'container', 'cores': 'cores', 'cpu_power': 'cpu-power', 'image_id': 'image-id', 'instance_role': 'instance-role', 'instance_type': 'instance-type', 'mem': 'mem', 'root_disk': 'root-disk', 'root_disk_source': 'root-disk-source', 'spaces': 'spaces', 'tags': 'tags', 'virt_type': 'virt-type', 'zones': 'zones'}
+    _toPy = {'allocate-public-ip': 'allocate_public_ip', 'arch': 'arch', 'container': 'container', 'cores': 'cores', 'cpu-power': 'cpu_power', 'image-id': 'image_id', 'instance-role': 'instance_role', 'instance-type': 'instance_type', 'mem': 'mem', 'root-disk': 'root_disk', 'root-disk-source': 'root_disk_source', 'spaces': 'spaces', 'tags': 'tags', 'virt-type': 'virt_type', 'zones': 'zones'}
+    def __init__(self, allocate_public_ip=None, arch=None, container=None, cores=None, cpu_power=None, image_id=None, instance_role=None, instance_type=None, mem=None, root_disk=None, root_disk_source=None, spaces=None, tags=None, virt_type=None, zones=None, **unknown_fields):
         '''
         allocate_public_ip : bool
         arch : str
         container : str
         cores : int
         cpu_power : int
+        image_id : str
         instance_role : str
         instance_type : str
         mem : int
         root_disk : int
         root_disk_source : str
         spaces : typing.Sequence[str]
         tags : typing.Sequence[str]
@@ -26449,14 +26828,15 @@
         zones : typing.Sequence[str]
         '''
         allocate_public_ip_ = allocate_public_ip
         arch_ = arch
         container_ = container
         cores_ = cores
         cpu_power_ = cpu_power
+        image_id_ = image_id
         instance_role_ = instance_role
         instance_type_ = instance_type
         mem_ = mem
         root_disk_ = root_disk
         root_disk_source_ = root_disk_source
         spaces_ = spaces
         tags_ = tags
@@ -26475,14 +26855,17 @@
 
         if cores_ is not None and not isinstance(cores_, int):
             raise Exception("Expected cores_ to be a int, received: {}".format(type(cores_)))
 
         if cpu_power_ is not None and not isinstance(cpu_power_, int):
             raise Exception("Expected cpu_power_ to be a int, received: {}".format(type(cpu_power_)))
 
+        if image_id_ is not None and not isinstance(image_id_, (bytes, str)):
+            raise Exception("Expected image_id_ to be a str, received: {}".format(type(image_id_)))
+
         if instance_role_ is not None and not isinstance(instance_role_, (bytes, str)):
             raise Exception("Expected instance_role_ to be a str, received: {}".format(type(instance_role_)))
 
         if instance_type_ is not None and not isinstance(instance_type_, (bytes, str)):
             raise Exception("Expected instance_type_ to be a str, received: {}".format(type(instance_type_)))
 
         if mem_ is not None and not isinstance(mem_, int):
@@ -26507,14 +26890,15 @@
             raise Exception("Expected zones_ to be a Sequence, received: {}".format(type(zones_)))
 
         self.allocate_public_ip = allocate_public_ip_
         self.arch = arch_
         self.container = container_
         self.cores = cores_
         self.cpu_power = cpu_power_
+        self.image_id = image_id_
         self.instance_role = instance_role_
         self.instance_type = instance_type_
         self.mem = mem_
         self.root_disk = root_disk_
         self.root_disk_source = root_disk_source_
         self.spaces = spaces_
         self.tags = tags_
@@ -27420,14 +27804,62 @@
             raise Exception("Expected params_ to be a Sequence, received: {}".format(type(params_)))
 
         self.params = params_
         self.unknown_fields = unknown_fields
 
 
 
+class WatchRemoteSecretChangesArg(Type):
+    _toSchema = {'application_token': 'application-token', 'bakery_version': 'bakery-version', 'macaroons': 'macaroons'}
+    _toPy = {'application-token': 'application_token', 'bakery-version': 'bakery_version', 'macaroons': 'macaroons'}
+    def __init__(self, application_token=None, bakery_version=None, macaroons=None, **unknown_fields):
+        '''
+        application_token : str
+        bakery_version : int
+        macaroons : typing.Sequence[~Macaroon]
+        '''
+        application_token_ = application_token
+        bakery_version_ = bakery_version
+        macaroons_ = [Macaroon.from_json(o) for o in macaroons or []]
+
+        # Validate arguments against known Juju API types.
+        if application_token_ is not None and not isinstance(application_token_, (bytes, str)):
+            raise Exception("Expected application_token_ to be a str, received: {}".format(type(application_token_)))
+
+        if bakery_version_ is not None and not isinstance(bakery_version_, int):
+            raise Exception("Expected bakery_version_ to be a int, received: {}".format(type(bakery_version_)))
+
+        if macaroons_ is not None and not isinstance(macaroons_, (bytes, str, list)):
+            raise Exception("Expected macaroons_ to be a Sequence, received: {}".format(type(macaroons_)))
+
+        self.application_token = application_token_
+        self.bakery_version = bakery_version_
+        self.macaroons = macaroons_
+        self.unknown_fields = unknown_fields
+
+
+
+class WatchRemoteSecretChangesArgs(Type):
+    _toSchema = {'relations': 'relations'}
+    _toPy = {'relations': 'relations'}
+    def __init__(self, relations=None, **unknown_fields):
+        '''
+        relations : typing.Sequence[~WatchRemoteSecretChangesArg]
+        '''
+        relations_ = [WatchRemoteSecretChangesArg.from_json(o) for o in relations or []]
+
+        # Validate arguments against known Juju API types.
+        if relations_ is not None and not isinstance(relations_, (bytes, str, list)):
+            raise Exception("Expected relations_ to be a Sequence, received: {}".format(type(relations_)))
+
+        self.relations = relations_
+        self.unknown_fields = unknown_fields
+
+
+
 class ZoneResult(Type):
     _toSchema = {'available': 'available', 'error': 'error', 'name': 'name'}
     _toPy = {'available': 'available', 'error': 'error', 'name': 'name'}
     def __init__(self, available=None, error=None, name=None, **unknown_fields):
         '''
         available : bool
         error : Error
```

### Comparing `juju-3.1.2.0/juju/client/client.py` & `juju-3.2.0.0/juju/client/client.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/codegen.py` & `juju-3.2.0.0/juju/client/codegen.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/connection.py` & `juju-3.2.0.0/juju/client/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     'Resumer': {'versions': [2]},
     'RetryStrategy': {'versions': [1]},
     'Secrets': {'versions': [1]},
     'SecretsManager': {'versions': [1, 2]},
     'SecretBackends': {'versions': [1]},
     'SecretBackendsManager': {'versions': [1]},
     'SecretBackendsRotateWatcher': {'versions': [1]},
+    'SecretsDrain': {'versions': [1]},
     'SecretsRevisionWatcher': {'versions': [1]},
     'SecretsRotationWatcher': {'versions': [1]},
     'SecretsTriggerWatcher': {'versions': [1]},
     'Singular': {'versions': [2]},
     'Spaces': {'versions': [6]},
     'StatusHistory': {'versions': [2]},
     'Storage': {'versions': [3, 4, 6]},
@@ -690,15 +691,17 @@
 
             1. The :class:`HTTPSConnection` instance
             2. Dictionary of auth headers to be used with the connection
             3. The root url path (str) to be used for requests.
 
         """
         endpoint = self.endpoint
-        host, remainder = endpoint.split(':', 1)
+        # Support IPv6 by right splitting on : and removing [] around IP address for host
+        host, remainder = endpoint.rsplit(':', 1)
+        host = host.strip("[]")
         port = remainder
         if '/' in remainder:
             port, _ = remainder.split('/', 1)
 
         conn = HTTPSConnection(
             host, int(port),
             context=self._get_ssl(self.cacert),
```

### Comparing `juju-3.1.2.0/juju/client/connector.py` & `juju-3.2.0.0/juju/client/connector.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/facade.py` & `juju-3.2.0.0/juju/client/facade.py`

 * *Files 1% similar despite different names*

```diff
@@ -681,15 +681,15 @@
                 if '>' in entry or '>=' in entry:
                     # something like juju >= 2.9.31
                     i = entry.index('>')
                     key = entry[:i].strip()
                     value = entry[i:].strip()
                     d[key] = value
                 else:
-                    # something like k8s-api
+                    # this is a simple entry
                     d[entry] = ''
             return cls(**d)
         return None
 
     def serialize(self):
         d = {}
         for attr, tgt in self._toSchema.items():
```

### Comparing `juju-3.1.2.0/juju/client/gocookies.py` & `juju-3.2.0.0/juju/client/gocookies.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/jujudata.py` & `juju-3.2.0.0/juju/client/jujudata.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/overrides.py` & `juju-3.2.0.0/juju/client/overrides.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/proxy/factory.py` & `juju-3.2.0.0/juju/client/proxy/factory.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/proxy/kubernetes/proxy.py` & `juju-3.2.0.0/juju/client/proxy/kubernetes/proxy.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/client/runner.py` & `juju-3.2.0.0/juju/client/runner.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/constraints.py` & `juju-3.2.0.0/juju/constraints.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/controller.py` & `juju-3.2.0.0/juju/controller.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/delta.py` & `juju-3.2.0.0/juju/delta.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/errors.py` & `juju-3.2.0.0/juju/errors.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/jasyncio.py` & `juju-3.2.0.0/juju/jasyncio.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/juju.py` & `juju-3.2.0.0/juju/juju.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/machine.py` & `juju-3.2.0.0/juju/machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/model.py` & `juju-3.2.0.0/juju/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,14 +258,15 @@
 
         """
         self.entity_id = entity_id
         self.model = model
         self._history_index = history_index
         self.connected = connected
         self.connection = model.connection()
+        self._status = 'unknown'
 
     def __repr__(self):
         return '<{} entity_id="{}">'.format(type(self).__name__,
                                             self.entity_id)
 
     def __getattr__(self, name):
         """Fetch object attributes from the underlying data dict held in the
@@ -512,14 +513,15 @@
         if channel is not None:
             ch = Channel.parse(channel).normalize()
 
         base = client.Base()
         if series:
             base.channel = ch.normalize().compute_base_channel(series=series)
             base.name = 'ubuntu'
+
         origin = client.CharmOrigin(source=Source.CHARM_HUB.value,
                                     architecture=architecture,
                                     risk=ch.risk,
                                     track=ch.track,
                                     base=base,
                                     revision=revision,
                                     )
@@ -736,15 +738,34 @@
 
         # Wait for the first packet of data from the AllWatcher,
         # which contains all information on the model.
         # TODO this means that we can't do anything until
         # we've received all the model data, which might be
         # a whole load of unneeded data if all the client wants
         # to do is make one RPC call.
-        await self._watch_received.wait()
+        async def watch_received_waiter():
+            await self._watch_received.wait()
+        waiter = jasyncio.create_task(watch_received_waiter())
+
+        # If we just wait for the _watch_received event and the _all_watcher task
+        # fails (e.g. because API fails like migration is in progress), then
+        # we'll hang because the _watch_received will never be set
+        # Instead, we watch for two things, 1) _watch_received, 2) _all_watcher done
+        # If _all_watcher is done before the _watch_received, then we should see
+        # (and raise) an exception coming from the _all_watcher
+        # Otherwise (i.e. _watch_received is set), then we're good to go
+        done, pending = await jasyncio.wait([waiter, self._watcher_task],
+                                            return_when=jasyncio.FIRST_COMPLETED)
+        if self._watcher_task in done:
+            # Cancel the _watch_received.wait
+            waiter.cancel()
+            # If there's no exception, then why did the _all_watcher broke its loop?
+            if not self._watcher_task.exception():
+                raise JujuError("AllWatcher task is finished abruptly without an exception.")
+            raise self._watcher_task.exception()
 
         if self.info is None:
             contr = await self.get_controller()
             self._info = await contr.get_model_info(model_name, model_uuid)
             log.debug('Got ModelInfo: %s', vars(self.info))
 
         self.uuid = self.info.uuid
@@ -752,14 +773,20 @@
     async def disconnect(self):
         """Shut down the watcher task and close websockets.
 
         """
         if not self._watch_stopped.is_set():
             log.debug('Stopping watcher task')
             self._watch_stopping.set()
+            # If the _all_watcher task is finished,
+            # check to see an exception, if yes, raise,
+            # otherwise we should see the _watch_stopped
+            # flag is set
+            if self._watcher_task.done() and self._watcher_task.exception():
+                raise self._watcher_task.exception()
             await self._watch_stopped.wait()
             self._watch_stopping.clear()
 
         if self.is_connected():
             log.debug('Closing model connection')
             await self._connector.disconnect()
             self._info = None
@@ -1129,14 +1156,15 @@
 
     def _watch(self):
         """Start an asynchronous watch against this model.
 
         See :meth:`add_observer` to register an onchange callback.
 
         """
+
         def _post_step(obj):
             # Once we get the model, ensure we're running in the correct state
             # as a post step.
             if isinstance(obj, ModelInfo) and obj.safe_data is not None:
                 model_config = obj.safe_data["config"]
                 if "mode" in model_config:
                     self._mode = model_config["mode"]
@@ -1218,15 +1246,15 @@
             finally:
                 self._watch_stopped.set()
 
         log.debug('Starting watcher task')
         self._watch_received.clear()
         self._watch_stopping.clear()
         self._watch_stopped.clear()
-        jasyncio.ensure_future(_all_watcher())
+        self._watcher_task = jasyncio.create_task(_all_watcher())
 
     async def _notify_observers(self, delta, old_obj, new_obj):
         """Call observing callbacks, notifying them of a change in model state
 
         :param delta: The raw change from the watcher
             (:class:`juju.client.overrides.Delta`)
         :param old_obj: The object in the model that this delta updates.
@@ -1740,19 +1768,18 @@
                             raise JujuError("cannot use num_units with subordinate application")
                         num_units = 0
 
             else:
                 # We have a local charm dir that needs to be uploaded
                 charm_dir = os.path.abspath(os.path.expanduser(identifier))
                 metadata = utils.get_local_charm_metadata(charm_dir)
-                charm_series = charm_series or await get_charm_series(metadata,
-                                                                      self)
-                if not base:
-                    charm_origin.base = utils.get_local_charm_base(
-                        charm_series, channel, metadata, charm_dir, client.Base)
+                charm_series = charm_series or await get_charm_series(metadata, self)
+
+                base = utils.get_local_charm_base(charm_series, charm_dir, client.Base)
+                charm_origin.base = base
 
                 if not application_name:
                     application_name = metadata['name']
                 if not application_name:
                     application_name = metadata['name']
                 if base is None and charm_series is None:
                     raise JujuError(
@@ -1835,26 +1862,26 @@
             'charm-origin': resolve_origin
         }])
         if len(resp.results) != 1:
             raise JujuError("expected one result, received {}".format(resp.results))
 
         result = resp.results[0]
         if result.error:
-            raise JujuError(result.error.message)
+            raise JujuError(f'resolving {url} : {result.error.message}')
 
         supported_series = result.supported_series
         resolved_origin = result.charm_origin
         charm_url = URL.parse(result.url)
 
         # run the series selector to get a series for the base
         selected_series = utils.series_selector(series, url, model_config, supported_series, force)
         result.charm_origin.base = utils.get_base_from_origin_or_channel(resolved_origin, selected_series)
         charm_url.series = selected_series
 
-        return result.url, result.charm_origin
+        return str(charm_url), resolved_origin
 
     async def _resolve_architecture(self, url):
         if url.architecture:
             return url.architecture
 
         constraints = await self.get_constraints()
         if 'arch' in constraints:
@@ -2493,15 +2520,15 @@
                 if current.controller_name is not None:
                     controller_name = current.controller_name
         await controller.connect(controller_name=controller_name)
         return controller
 
     async def wait_for_idle(self, apps=None, raise_on_error=True, raise_on_blocked=False,
                             wait_for_active=False, timeout=10 * 60, idle_period=15, check_freq=0.5,
-                            status=None, wait_for_units=1, wait_for_exact_units=None):
+                            status=None, wait_for_units=None, wait_for_exact_units=None):
         """Wait for applications in the model to settle into an idle state.
 
         :param apps (list[str]): Optional list of specific app names to wait on.
             If given, all apps must be present in the model and idle, while other
             apps in the model can still be busy. If not given, all apps currently
             in the model must be idle.
 
@@ -2541,25 +2568,28 @@
             going into the idle state. (e.g. useful for scaling down).
             When set, takes precedence over the `wait_for_units` parameter.
         """
         if wait_for_active:
             warnings.warn("wait_for_active is deprecated; use status", DeprecationWarning)
             status = "active"
 
+        _wait_for_units = wait_for_units if wait_for_units is not None else 1
+
         timeout = timedelta(seconds=timeout) if timeout is not None else None
         idle_period = timedelta(seconds=idle_period)
         start_time = datetime.now()
         # Type check against the common error of passing a str for apps
         if apps is not None and (not isinstance(apps, list) or
                                  any(not isinstance(o, str)
                                      for o in apps)):
             raise JujuError(f'Expected a List[str] for apps, given {apps}')
 
         apps = apps or self.applications
         idle_times = {}
+        units_ready = set()  # The units that are in the desired state
         last_log_time = None
         log_interval = timedelta(seconds=30)
 
         def _raise_for_status(entities, status):
             if not entities:
                 return
             for entity_name, error_type in (("Machine", JujuMachineError),
@@ -2577,52 +2607,71 @@
                 ))
 
         if wait_for_exact_units is not None:
             assert type(wait_for_exact_units) == int and wait_for_exact_units >= 0, \
                 'Invalid value for wait_for_exact_units : %s' % wait_for_exact_units
 
         while True:
+            # The list 'busy' is what keeps this loop going,
+            # i.e. it'll stop when busy is empty after all the
+            # units are scanned
             busy = []
             errors = {}
             blocks = {}
             for app_name in apps:
                 if app_name not in self.applications:
                     busy.append(app_name + " (missing)")
                     continue
                 app = self.applications[app_name]
-                if raise_on_error and app.status == "error":
+                app_status = await app.get_status()
+                if raise_on_error and app_status == "error":
                     errors.setdefault("App", []).append(app.name)
-                if raise_on_blocked and app.status == "blocked":
+                if raise_on_blocked and app_status == "blocked":
                     blocks.setdefault("App", []).append(app.name)
+
+                # Check if wait_for_exact_units flag is used
                 if wait_for_exact_units is not None:
                     if len(app.units) != wait_for_exact_units:
                         busy.append(app.name + " (waiting for exactly %s units, current : %s)" %
                                     (wait_for_exact_units, len(app.units)))
                         continue
-                elif len(app.units) < wait_for_units:
+                # If we have less # of units then required, then wait a bit more
+                elif len(app.units) < _wait_for_units:
                     busy.append(app.name + " (not enough units yet - %s/%s)" %
-                                (len(app.units), wait_for_units))
+                                (len(app.units), _wait_for_units))
                     continue
+                # User wants to see a certain # of units, and we have enough
+                elif wait_for_units and len(units_ready) >= _wait_for_units:
+                    # So no need to keep looking, we have the desired number of units ready to go,
+                    # exit the loop. Don't return, though, we might still have some errors to raise
+                    break
                 for unit in app.units:
                     if unit.machine is not None and unit.machine.status == "error":
                         errors.setdefault("Machine", []).append(unit.machine.id)
                         continue
                     if unit.agent_status == "error":
                         errors.setdefault("Agent", []).append(unit.name)
                         continue
                     if raise_on_error and unit.workload_status == "error":
                         errors.setdefault("Unit", []).append(unit.name)
                         continue
                     if raise_on_blocked and unit.workload_status == "blocked":
                         blocks.setdefault("Unit", []).append(unit.name)
                         continue
-                    waiting_for_status = status and unit.workload_status != status
-                    if not waiting_for_status and unit.agent_status == "idle":
+                    waiting_for_a_particular_status = status and unit.workload_status != status
+                    if not waiting_for_a_particular_status and unit.agent_status == "idle":
+                        # We'll be here in two cases:
+                        # 1) We're not waiting for a particular status and the agent is "idle"
+                        # 2) We're waiting for a particular status and the workload is in that status
+                        # Either way, the unit is ready, start measuring the time period that
+                        # it needs to stay in that state (i.e. idle_period)
+                        units_ready.add(unit.name)
                         now = datetime.now()
                         idle_start = idle_times.setdefault(unit.name, now)
+
                         if now - idle_start < idle_period:
                             busy.append("{} [{}] {}: {}".format(unit.name,
                                                                 unit.agent_status,
                                                                 unit.workload_status,
                                                                 unit.workload_status_message))
                     else:
                         idle_times.pop(unit.name, None)
```

### Comparing `juju-3.1.2.0/juju/names.py` & `juju-3.2.0.0/juju/names.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/offerendpoints.py` & `juju-3.2.0.0/juju/offerendpoints.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/origin.py` & `juju-3.2.0.0/juju/origin.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,23 +109,21 @@
 
     def __str__(self):
         path = self.risk
         if self.track != "":
             path = "{}/{}".format(self.track, path)
         return path
 
-    def compute_base_channel(self, series=None):
+    def compute_base_channel(self, series):
         """Determines the channel for a client.Base
         A base channel is a track/risk/branch
 
         """
         _ch = [self.risk]
-        tr = self.track
-        if series:
-            tr = utils.get_series_version(series)
+        tr = utils.get_series_version(series)
         if tr:
             _ch = [tr] + _ch
         return "/".join(_ch)
 
 
 class Platform:
     """ParsePlatform parses a string representing a store platform.
```

### Comparing `juju-3.1.2.0/juju/placement.py` & `juju-3.2.0.0/juju/placement.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/provisioner.py` & `juju-3.2.0.0/juju/provisioner.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/relation.py` & `juju-3.2.0.0/juju/relation.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/remoteapplication.py` & `juju-3.2.0.0/juju/remoteapplication.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/status.py` & `juju-3.2.0.0/juju/status.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/tag.py` & `juju-3.2.0.0/juju/tag.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/unit.py` & `juju-3.2.0.0/juju/unit.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/url.py` & `juju-3.2.0.0/juju/url.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/user.py` & `juju-3.2.0.0/juju/user.py`

 * *Files identical despite different names*

### Comparing `juju-3.1.2.0/juju/utils.py` & `juju-3.2.0.0/juju/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -288,14 +288,16 @@
 EOAN = "eoan"
 FOCAL = "focal"
 GROOVY = "groovy"
 HIRSUTE = "hirsute"
 IMPISH = "impish"
 JAMMY = "jammy"
 KINETIC = "kinetic"
+LUNAR = "lunar"
+MANTIC = "mantic"
 
 UBUNTU_SERIES = {
     PRECISE: "12.04",
     QUANTAL: "12.10",
     RARING: "13.04",
     SAUCY: "13.10",
     TRUSTY: "14.04",
@@ -312,94 +314,99 @@
     EOAN: "19.10",
     FOCAL: "20.04",
     GROOVY: "20.10",
     HIRSUTE: "21.04",
     IMPISH: "21.10",
     JAMMY: "22.04",
     KINETIC: "22.10",
+    LUNAR: "23.04",
+    MANTIC: "23.10",
 }
 
+KUBERNETES = "kubernetes"
+KUBERNETES_SERIES = {
+    KUBERNETES: "kubernetes"
+}
+
+ALL_SERIES_VERSIONS = {**UBUNTU_SERIES, **KUBERNETES_SERIES}
+
 
 def get_series_version(series_name):
-    if series_name not in UBUNTU_SERIES:
+    """get_series_version outputs the version of the OS based on the given series
+    e.g. jammy -> 22.04, kubernetes -> kubernetes
+
+    :param str series_name: name of the series
+    :return str: os version
+    """
+    if series_name not in ALL_SERIES_VERSIONS:
         raise errors.JujuError("Unknown series : %s", series_name)
-    return UBUNTU_SERIES[series_name]
+    return ALL_SERIES_VERSIONS[series_name]
 
 
 def get_version_series(version):
+    """get_version_series is the opposite of the get_series_version. It outputs the series based
+    on given OS version
+
+    :param str version: version of the OS
+    return str: name of the series corresponding to the given version
+    """
     if version not in UBUNTU_SERIES.values():
         raise errors.JujuError("Unknown version : %s", version)
     return list(UBUNTU_SERIES.keys())[list(UBUNTU_SERIES.values()).index(version)]
 
 
-def get_local_charm_base(series, channel_from_arg, charm_metadata,
-                         charm_path, baseCls):
+def get_local_charm_base(series, charm_path, base_class):
     """Deduce the base [channel/osname] of a local charm based on what we
     know already
 
     :param str series: This may come from the argument or the metadata.yaml
-    :param str channel_from_arg: This is channel passed as argument, if any.
-    :param dict charm_metadata: metadata.yaml
     :param str charm_path: Path of charm directory/.charm file
-    :param class baseCls:
+    :param class base_class:
     :return: Instance of the baseCls with channel/osname informaiton
     """
 
     channel_for_base = ''
     os_name_for_base = ''
-    # If user passed a channel_arg, then check the supported series against
-    # the channel's track
-    chnl_check = origin.Channel.parse(channel_from_arg) if channel_from_arg \
-        else None
-    if chnl_check:
-        not_supported_error = errors.JujuError(
-            "Given channel [track/risk] is not supported --"
-            "\n - Given channel : %s"
-            "\n - Series in Charm Metadata : %s" %
-            (channel_from_arg, charm_metadata['series']))
-        channel_for_base = chnl_check.track
-        intented_series = get_version_series(channel_for_base)
-        if intented_series not in charm_metadata['series']:
-            raise not_supported_error
-        # Also check the manifest if there's one
-        charm_manifest = get_local_charm_manifest(charm_path)
-        if 'bases' in charm_manifest:
-            for base in charm_manifest['bases']:
-                if channel_for_base == base['channel']:
-                    break
-            else:
-                raise not_supported_error
 
-    # If we know the series, use it to get a channel
-    if channel_for_base == '':
+    # We should know the series, so use it to get a channel
+    if series:
         channel_for_base = get_series_version(series) if series else ''
         if channel_for_base:
             # we currently only support ubuntu series (statically)
             # TODO (cderici) : go juju/core/series/supported.go and get the
             #  others here too
-            os_name_for_base = 'ubuntu'
+            if series in KUBERNETES_SERIES:
+                os_name_for_base = 'kubernetes'
+            else:
+                os_name_for_base = 'ubuntu'
 
     # Check the charm manifest
     if channel_for_base == '':
         charm_manifest = get_local_charm_manifest(charm_path)
         if 'bases' in charm_manifest:
             channel_for_base = charm_manifest['bases'][0]['channel']
             os_name_for_base = charm_manifest['bases'][0]['name']
-        else:
-            # Also check the charmcraft.yaml
-            charmcraft_yaml = get_local_charm_charmcraft_yaml(charm_path)
-            if 'bases' in charmcraft_yaml:
-                channel_for_base = charmcraft_yaml['bases'][0]['run-on'][0]['channel']
-                os_name_for_base = charmcraft_yaml['bases'][0]['run-on'][0]['name']
+
+    # Also check the charmcraft.yaml
+    if channel_for_base == '':
+        charmcraft_yaml = get_local_charm_charmcraft_yaml(charm_path)
+        if 'bases' in charmcraft_yaml:
+            channel_for_base = charmcraft_yaml['bases'][0]['run-on'][0]['channel']
+            os_name_for_base = charmcraft_yaml['bases'][0]['run-on'][0]['name']
 
     if channel_for_base == '':
         raise errors.JujuError("Unable to determine base for charm : %s" %
                                charm_path)
 
-    return baseCls(channel_for_base, os_name_for_base)
+    # Legacy k8s charms - assume ubuntu focal
+    # as per juju/cmd/juju/application/utils.DeduceOrigin()
+    if channel_for_base == "kubernetes" or os_name_for_base == "kubernetes":
+        channel_for_base = '20.04/stable'
+        os_name_for_base = 'ubuntu'
+    return base_class(channel_for_base, os_name_for_base)
 
 
 def base_channel_to_series(channel):
     """Returns the series string using the track inside the base channel
 
     :param str channel: is track/risk (e.g. 20.04/stable)
     :return: str series (e.g. focal)
@@ -419,27 +426,29 @@
     return client.Base(name=name, channel=channel)
 
 
 DEFAULT_SUPPORTED_LTS = 'jammy'
 DEFAULT_SUPPORTED_LTS_BASE = client.Base(channel='22.04', name='ubuntu')
 
 
-def base_channel_from_series(track, risk, series=None):
+def base_channel_from_series(track, risk, series):
     return origin.Channel(track=track, risk=risk).normalize().compute_base_channel(series=series)
 
 
-def get_os_from_series(series=None):
-    if not series or series in UBUNTU_SERIES:
+def get_os_from_series(series):
+    if series in UBUNTU_SERIES:
         return 'ubuntu'
     raise JujuError(f'os for the series {series} needs to be added')
 
 
 def get_base_from_origin_or_channel(origin_or_channel, series=None):
-    channel = base_channel_from_series(origin_or_channel.track, origin_or_channel.risk, series)
-    os_name = get_os_from_series(series)
+    channel, os_name = None, None
+    if series:
+        channel = base_channel_from_series(origin_or_channel.track, origin_or_channel.risk, series)
+        os_name = get_os_from_series(series)
     return client.Base(channel=channel, name=os_name)
 
 
 def series_for_charm(requested_series, supported_series):
     """series_for_charm takes a requested series and a list of series supported by a
     charm and returns the series which is relevant.
     If the requested series is empty, then the first supported series is used,
```

### Comparing `juju-3.1.2.0/juju.egg-info/PKG-INFO` & `juju-3.2.0.0/juju.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juju
-Version: 3.1.2.0
+Version: 3.2.0.0
 Summary: Python library for Juju
 Home-page: https://github.com/juju/python-libjuju
 Maintainer: Juju Ecosystem Engineering
 Maintainer-email: juju@lists.ubuntu.com
 License: Apache 2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -145,25 +145,47 @@
 Pylibjuju releases now track the Juju release cadence. New generated schemas
 will be updated per Juju releases.
 
 
 Changelog
 ---------
 
+3.2.0.0
+^^^^^^^
+
+Wednesday 7th June 2023
+
+This release contains the new endpoints for Juju 3.2.0.
+
+This release works with any Juju 3.x controller.
+
+What's Changed
+""""""""""""""
+* Add base.bootstrapped decorator to integration test by @cderici in https://github.com/juju/python-libjuju/pull/856
+* Add mantic and lunar to list of ubuntu series by @addyess in https://github.com/juju/python-libjuju/pull/853
+* [JUJU-3885] forward port ipv6 support by @cderici in https://github.com/juju/python-libjuju/pull/866
+* Revisit auto documentation generation with sphinx on RTD by @cderici in https://github.com/juju/python-libjuju/pull/871
+* [JUJU-3894] Forward port some fixes from 2.9 to master by @cderici in https://github.com/juju/python-libjuju/pull/870
+* Revisit the secret backend integration test by @cderici in https://github.com/juju/python-libjuju/pull/858
+* [JUJU-3954] Fix incorrect base channel computation by @cderici in https://github.com/juju/python-libjuju/pull/875
+* [JUJU-3927] Add 3.2.0 facades  by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/874
+
 3.1.2.0
 ^^^^^^^
 
-Friday 5th May 2022
+Friday 5th May 2023
 
 This release has been tested with Juju 3.1.2 and contains the new 
 endpoints for secrets backend.
 
 This release works with any Juju 3.x controller.
 
-## What's Changed
+What's Changed
+""""""""""""""
+
 * [JUJU-3202] Add facades for 3.1.1. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/807
 * Add destroy units by @cderici in https://github.com/juju/python-libjuju/pull/812
 * [JUJU-3517] Revisit _build_facades in connection by @cderici in https://github.com/juju/python-libjuju/pull/826
 * [JUJU-3527] Added 3.1.2 and 3.2-beta2 schemas. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/828
 * [JUJU-1628] Deploy by revision by @cderici in https://github.com/juju/python-libjuju/pull/830
 * [JUJU-3552] Prepare 3.1.2.1 release by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/836
 
@@ -173,53 +195,62 @@
 Friday 10th February 2023
 
 This release targets juju version 3.1.0 and enables the new secrets backend api.
 Connectivity with juju controllers in the 3.x series is allowed, connections with different major version controllers (e.g. 2.x, 4.x, etc.) will be cancelled.
 
 This version is only tested using Juju 3.1.0.
 
-## What's Changed
+What's Changed
+""""""""""""""
+
 * setup.py: adjust websockets versions for py38-310 by @mert-kirpici in https://github.com/juju/python-libjuju/pull/731
 * [JUJU-2175] Remove juju 2.9 support on 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/774
 * [JUJU-2276] Series or base for local charms by @cderici in https://github.com/juju/python-libjuju/pull/777
 * [JUJU-2391] Fix wrong bases analysis. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/782
 * [JUJU-2401] Added release candidate workflow. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/784
 * [JUJU-2402] Prepare nightly juju edge testing. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/785
 * [JUJU-2237] Remove charmstore charm support from pylibjuju by @cderici in https://github.com/juju/python-libjuju/pull/786
 * [JUJU-2426] Secrets support by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/791
 * [JUJU-2573] Base argument for model deploy by @cderici in https://github.com/juju/python-libjuju/pull/798
 * Add compatibility for juju 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/799
 * Replace schemas.json with a wellformed version. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/800
 
-## New Contributors
+New Contributors
+""""""""""""""""
+
 * @mert-kirpici made their first contribution in https://github.com/juju/python-libjuju/pull/731
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.4...3.1.0.1
 
 3.0.4
 ^^^^^
 
 Wednesday 26th October
 
-## What's Changed
+What's Changed
+""""""""""""""
+
 * [JUJU-2027] Local refresh with resoruces by @cderici in https://github.com/juju/python-libjuju/pull/757
 * [JUJU-2026] Improve resolve charm by @cderici in https://github.com/juju/python-libjuju/pull/761
 * Add owner and data to license file by @arturo-seijas in https://github.com/juju/python-libjuju/pull/760
 
-## New Contributors
+New Contributors
+""""""""""""""""
+
 * @arturo-seijas made their first contribution in https://github.com/juju/python-libjuju/pull/760
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.3...3.0.4
 
 3.0.3
 ^^^^^
 
 Saturay October 22 2022
 
-## What's Changed
+What's Changed
+""""""""""""""
 
 * Wait for idle arg type check by @cderici in https://github.com/juju/python-libjuju/pull/741
 * [JUJU-1970] Revise local refresh by @cderici in https://github.com/juju/python-libjuju/pull/742
 * [JUJU-1984] Update facade schemas for juju 3.0-rc1-2 by @cderici in https://github.com/juju/python-libjuju/pull/745
 * [JUJU-1992] Fix charmhub series deploy 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/746
 * [JUJU-2001] Fix base for local charms and bundles for CharmOrigin 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/749
 * [JUJU-2017] Check subordinate field value instead of existence by @cderici in https://github.com/juju/python-libjuju/pull/751
@@ -231,15 +262,16 @@
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.2...3.0.3
 
 3.0.2
 ^^^^^
 
 Wednesday October 5 2022
 
-## What's Changed
+What's Changed
+""""""""""""""
 
 * Model name can now be accessed through model.name by @jack-w-shaw in https://github.com/juju/python-libjuju/pull/702
 * [JUJU-1593] Fix `unit.run()` and update the old client codes by @cderici in https://github.com/juju/python-libjuju/pull/710
 * Add py.typed marker by @sed-i in https://github.com/juju/python-libjuju/pull/709
 * [JUJU-1664] Add force, no-wait, destroy-storage params to app.destroy by @cderici in https://github.com/juju/python-libjuju/pull/714
 * snapcraft.io access should use https requests by @addyess in https://github.com/juju/python-libjuju/pull/715
 * [JUJU-1680] Add issue and PR templates by @cderici in https://github.com/juju/python-libjuju/pull/718
```

### Comparing `juju-3.1.2.0/juju.egg-info/SOURCES.txt` & `juju-3.2.0.0/juju.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 docs/changelog.rst
 docs/index.rst
 docs/readme.rst
 docs/api/juju.action.rst
 docs/api/juju.annotation.rst
 docs/api/juju.application.rst
 docs/api/juju.client.rst
-docs/api/juju.cloud.rst
 docs/api/juju.constraints.rst
 docs/api/juju.controller.rst
 docs/api/juju.delta.rst
 docs/api/juju.errors.rst
 docs/api/juju.exceptions.rst
 docs/api/juju.juju.rst
 docs/api/juju.loop.rst
```

### Comparing `juju-3.1.2.0/setup.py` & `juju-3.2.0.0/setup.py`

 * *Files identical despite different names*

