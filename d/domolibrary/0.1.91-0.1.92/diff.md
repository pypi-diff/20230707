# Comparing `tmp/domolibrary-0.1.91.tar.gz` & `tmp/domolibrary-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.91.tar", last modified: Tue Jun 27 22:45:16 2023, max compression
+gzip compressed data, was "domolibrary-0.1.92.tar", last modified: Fri Jul  7 16:58:19 2023, max compression
```

## Comparing `domolibrary-0.1.91.tar` & `domolibrary-0.1.92.tar`

### file list

```diff
@@ -1,153 +1,154 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.253153 domolibrary-0.1.91/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.125153 domolibrary-0.1.91/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.91/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-06-01 20:57:16.000000 domolibrary-0.1.91/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.129153 domolibrary-0.1.91/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.91/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.153153 domolibrary-0.1.91/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.91/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.173153 domolibrary-0.1.91/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.91/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-06-01 20:57:16.000000 domolibrary-0.1.91/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.173153 domolibrary-0.1.91/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.91/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-01 20:57:16.000000 domolibrary-0.1.91/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-06-01 20:57:16.000000 domolibrary-0.1.91/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-06-01 20:57:16.000000 domolibrary-0.1.91/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-06-27 22:45:16.253153 domolibrary-0.1.91/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-06-01 20:57:16.000000 domolibrary-0.1.91/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.177153 domolibrary-0.1.91/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   179282 2023-06-27 22:44:36.000000 domolibrary-0.1.91/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.197153 domolibrary-0.1.91/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24128 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3477 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3962 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21366 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12330 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.205153 domolibrary-0.1.91/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12077 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.209153 domolibrary-0.1.91/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/integrations/Automation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.217153 domolibrary-0.1.91/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/application.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2369 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8439 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/job.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/stream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.221153 domolibrary-0.1.91/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-06-27 22:44:35.000000 domolibrary-0.1.91/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.181153 domolibrary-0.1.91/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-06-27 22:45:16.000000 domolibrary-0.1.91/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4106 2023-06-27 22:45:16.000000 domolibrary-0.1.91/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-27 22:45:16.000000 domolibrary-0.1.91/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-06-27 22:45:16.000000 domolibrary-0.1.91/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-01 20:57:34.000000 domolibrary-0.1.91/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-06-27 22:45:16.000000 domolibrary-0.1.91/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-06-27 22:45:16.000000 domolibrary-0.1.91/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-06-27 22:45:12.000000 domolibrary-0.1.91/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-27 22:45:16.253153 domolibrary-0.1.91/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-06-01 20:57:16.000000 domolibrary-0.1.91/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-27 22:45:16.249153 domolibrary-0.1.91/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-06-01 20:57:16.000000 domolibrary-0.1.91/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-06-01 20:57:16.000000 domolibrary-0.1.91/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-06-01 20:57:16.000000 domolibrary-0.1.91/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-06-01 20:57:16.000000 domolibrary-0.1.91/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-06-01 20:57:16.000000 domolibrary-0.1.91/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.91/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-06-01 20:57:16.000000 domolibrary-0.1.91/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-06-01 20:57:16.000000 domolibrary-0.1.91/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-06-01 20:57:16.000000 domolibrary-0.1.91/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-01 20:57:16.000000 domolibrary-0.1.91/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-06-01 20:57:16.000000 domolibrary-0.1.91/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.167051 domolibrary-0.1.92/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.723051 domolibrary-0.1.92/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-06-01 20:57:16.000000 domolibrary-0.1.92/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.727051 domolibrary-0.1.92/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.751051 domolibrary-0.1.92/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.783051 domolibrary-0.1.92/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.791051 domolibrary-0.1.92/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-01 20:57:16.000000 domolibrary-0.1.92/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-06-01 20:57:16.000000 domolibrary-0.1.92/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-06-01 20:57:16.000000 domolibrary-0.1.92/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 16:58:19.167051 domolibrary-0.1.92/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-06-01 20:57:16.000000 domolibrary-0.1.92/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.795051 domolibrary-0.1.92/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   182743 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.955051 domolibrary-0.1.92/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24179 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3477 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3962 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6722 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23039 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12268 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.019051 domolibrary-0.1.92/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12077 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.027051 domolibrary-0.1.92/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/integrations/Automation.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.131051 domolibrary-0.1.92/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/application.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2369 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8439 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/job.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/stream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.147051 domolibrary-0.1.92/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.835051 domolibrary-0.1.92/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4141 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-01 20:57:34.000000 domolibrary-0.1.92/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-07-07 16:58:04.000000 domolibrary-0.1.92/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-07 16:58:19.167051 domolibrary-0.1.92/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-06-01 20:57:16.000000 domolibrary-0.1.92/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.167051 domolibrary-0.1.92/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/upload_data.py
```

### Comparing `domolibrary-0.1.91/Automation/automation.py` & `domolibrary-0.1.92/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DataOcean/Transport.py` & `domolibrary-0.1.92/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.92/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.92/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DataOcean/cnfg_s3.py` & `domolibrary-0.1.92/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.92/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoAccount.py` & `domolibrary-0.1.92/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.92/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.92/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoApplication.py` & `domolibrary-0.1.92/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoAuth.py` & `domolibrary-0.1.92/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.92/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoCard.py` & `domolibrary-0.1.92/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoCertification.py` & `domolibrary-0.1.92/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.92/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.92/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoDataset.py` & `domolibrary-0.1.92/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoGrant.py` & `domolibrary-0.1.92/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoGroup.py` & `domolibrary-0.1.92/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.92/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoJob.py` & `domolibrary-0.1.92/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoLineage.py` & `domolibrary-0.1.92/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoPDP.py` & `domolibrary-0.1.92/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoPage.py` & `domolibrary-0.1.92/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoPublish.py` & `domolibrary-0.1.92/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoRole.py` & `domolibrary-0.1.92/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.92/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoStream.py` & `domolibrary-0.1.92/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoTag.py` & `domolibrary-0.1.92/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/DomoUser.py` & `domolibrary-0.1.92/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/get_data.py` & `domolibrary-0.1.92/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.92/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/LICENSE` & `domolibrary-0.1.92/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/PKG-INFO` & `domolibrary-0.1.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.91
+Version: 0.1.92
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary-0.1.91/README.md` & `domolibrary-0.1.92/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/_modidx.py` & `domolibrary-0.1.92/domolibrary/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,14 +369,30 @@
                                                                                                              'domolibrary/classes/DomoJob.py'),
                                              'domolibrary.classes.DomoJob.DomoTrigger_Schedule.to_obj': ( 'classes/domojob.html#domotrigger_schedule.to_obj',
                                                                                                           'domolibrary/classes/DomoJob.py'),
                                              'domolibrary.classes.DomoJob.DomoTrigger_Schedule.to_schedule_obj': ( 'classes/domojob.html#domotrigger_schedule.to_schedule_obj',
                                                                                                                    'domolibrary/classes/DomoJob.py'),
                                              'domolibrary.classes.DomoJob.WatchDogType': ( 'classes/domojob.html#watchdogtype',
                                                                                            'domolibrary/classes/DomoJob.py')},
+            'domolibrary.classes.DomoLineage': { 'domolibrary.classes.DomoLineage.DomoLineage': ( 'classes/domolineage.html#domolineage',
+                                                                                                  'domolibrary/classes/DomoLineage.py'),
+                                                 'domolibrary.classes.DomoLineage.DomoLineage.__post_init__': ( 'classes/domolineage.html#domolineage.__post_init__',
+                                                                                                                'domolibrary/classes/DomoLineage.py'),
+                                                 'domolibrary.classes.DomoLineage.DomoLineage._get_content_list_ls': ( 'classes/domolineage.html#domolineage._get_content_list_ls',
+                                                                                                                       'domolibrary/classes/DomoLineage.py'),
+                                                 'domolibrary.classes.DomoLineage.DomoLineage._get_page_card_ids': ( 'classes/domolineage.html#domolineage._get_page_card_ids',
+                                                                                                                     'domolibrary/classes/DomoLineage.py'),
+                                                 'domolibrary.classes.DomoLineage.DomoLineage._reset_lineage_and_sync_parent': ( 'classes/domolineage.html#domolineage._reset_lineage_and_sync_parent',
+                                                                                                                                 'domolibrary/classes/DomoLineage.py'),
+                                                 'domolibrary.classes.DomoLineage.DomoLineage.get': ( 'classes/domolineage.html#domolineage.get',
+                                                                                                      'domolibrary/classes/DomoLineage.py'),
+                                                 'domolibrary.classes.DomoLineage.DomoLineage.get_entity_lineage_upstream': ( 'classes/domolineage.html#domolineage.get_entity_lineage_upstream',
+                                                                                                                              'domolibrary/classes/DomoLineage.py'),
+                                                 'domolibrary.classes.DomoLineage.DomoLineage_Type': ( 'classes/domolineage.html#domolineage_type',
+                                                                                                       'domolibrary/classes/DomoLineage.py')},
             'domolibrary.classes.DomoPDP': { 'domolibrary.classes.DomoPDP.Dataset_PDP_Policies': ( 'classes/domopdp.html#dataset_pdp_policies',
                                                                                                    'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.__init__': ( 'classes/domopdp.html#dataset_pdp_policies.__init__',
                                                                                                             'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.get_policies': ( 'classes/domopdp.html#dataset_pdp_policies.get_policies',
                                                                                                                 'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.Dataset_PDP_Policies.search_pdp_policies': ( 'classes/domopdp.html#dataset_pdp_policies.search_pdp_policies',
@@ -419,14 +435,18 @@
                                                                                                          'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.display_url': ( 'classes/domopage.html#domopage.display_url',
                                                                                                      'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.get_accesslist': ( 'classes/domopage.html#domopage.get_accesslist',
                                                                                                         'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.get_by_id': ( 'classes/domopage.html#domopage.get_by_id',
                                                                                                    'domolibrary/classes/DomoPage.py'),
+                                              'domolibrary.classes.DomoPage.DomoPage.get_cards': ( 'classes/domopage.html#domopage.get_cards',
+                                                                                                   'domolibrary/classes/DomoPage.py'),
+                                              'domolibrary.classes.DomoPage.DomoPage.get_datasets': ( 'classes/domopage.html#domopage.get_datasets',
+                                                                                                      'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.share': ( 'classes/domopage.html#domopage.share',
                                                                                                'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.update_layout': ( 'classes/domopage.html#domopage.update_layout',
                                                                                                        'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPages': ( 'classes/domopage.html#domopages',
                                                                                           'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPages.get_pages': ( 'classes/domopage.html#domopages.get_pages',
@@ -463,14 +483,16 @@
                                                                                                    'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.PageLayoutTemplate._from_json': ( 'classes/domopage.html#pagelayouttemplate._from_json',
                                                                                                               'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.PageLayoutTemplate.get_body': ( 'classes/domopage.html#pagelayouttemplate.get_body',
                                                                                                             'domolibrary/classes/DomoPage.py')},
             'domolibrary.classes.DomoPublish': { 'domolibrary.classes.DomoPublish.DomoPublication': ( 'classes/domopublish.html#domopublication',
                                                                                                       'domolibrary/classes/DomoPublish.py'),
+                                                 'domolibrary.classes.DomoPublish.DomoPublication.__post_init__': ( 'classes/domopublish.html#domopublication.__post_init__',
+                                                                                                                    'domolibrary/classes/DomoPublish.py'),
                                                  'domolibrary.classes.DomoPublish.DomoPublication._from_json': ( 'classes/domopublish.html#domopublication._from_json',
                                                                                                                  'domolibrary/classes/DomoPublish.py'),
                                                  'domolibrary.classes.DomoPublish.DomoPublication.accept_invite_by_id': ( 'classes/domopublish.html#domopublication.accept_invite_by_id',
                                                                                                                           'domolibrary/classes/DomoPublish.py'),
                                                  'domolibrary.classes.DomoPublish.DomoPublication.create_publication': ( 'classes/domopublish.html#domopublication.create_publication',
                                                                                                                          'domolibrary/classes/DomoPublish.py'),
                                                  'domolibrary.classes.DomoPublish.DomoPublication.get_from_id': ( 'classes/domopublish.html#domopublication.get_from_id',
```

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.92/domolibrary/classes/DomoAccount.py`

 * *Files 0% similar despite different names*

```diff
@@ -601,18 +601,19 @@
 
     if debug_prn:
         print(
             f"ℹ️ - {auth.domo_instance} - {'is' if is_v2 else 'is not'} v2_group_ownership")
 
     if is_v2 is None:
         raise Exception(
-            """🛑 ERROR must pass `is_v2` bool to share_accounts function IF NOT pass `dmda.DomoFullAuth`.
-the group management v2 API has a different body.  
-Alternatively pass a full auth object to auto check the bootstrap.
-""")
+            """🛑 ERROR must explicitly pass a value for the `is_v2` boolean to share_accounts function.ABC
+alternatively, use `dmda.DomoFullAuth` to automatically retrieve the correct setting.ABC
+account sharing differs between v1 and v2 of the API.""")
+        
+        return None
 
     res = None
 
     if is_v2:
         share_payload = account_routes.generate_share_account_payload_v2(
             user_id=user_id, access_level=access_level or ShareAccount_V2_AccessLevel.CAN_VIEW
         )
@@ -635,25 +636,22 @@
             account_id=self.id,
             share_payload=share_payload,
             debug_api=debug_api,
             session=session,
         )
 
     if res.status == 500 and res.response == 'Internal Server Error':
-        res.response = f'ℹ️ - {res.response + "| User may own account."}'
+        res.response = f'ℹ️ - {res.response + " | User may own account."}'
 
     if res.status == 200:
         res.response = f"shared {self.id} - {self.name} with {user_id}"
 
     return res
 
-
-
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 38
+# %% ../../nbs/classes/50_DomoAccount.ipynb 39
 @patch_to(DomoAccount)
 async def share(
     self: DomoAccount,
     domo_user = None,
     domo_group = None,
     auth: dmda.DomoAuth = None,
     is_v2: bool = None,
@@ -716,20 +714,20 @@
 
     if res.status == 200:
         domo_entity = domo_user or domo_group
         res.response = f"shared {self.id} - {self.name} with {domo_entity.id}"
 
     return res
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 41
+# %% ../../nbs/classes/50_DomoAccount.ipynb 42
 @dataclass
 class DomoAccounts:
     auth: dmda.DomoAuth
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 42
+# %% ../../nbs/classes/50_DomoAccount.ipynb 43
 @patch_to(DomoAccounts, cls_method=True)
 async def _get_accounts_accountsapi(
     cls: DomoAccounts,
     auth: dmda.DomoAuth,
     debug_api: bool = False,
     session: httpx.AsyncClient = None,
     return_raw: bool = False,
```

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.92/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoApplication.py` & `domolibrary-0.1.92/domolibrary/classes/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.92/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoCard.py` & `domolibrary-0.1.92/domolibrary/classes/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.92/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.92/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.92/domolibrary/classes/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.92/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.92/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.92/domolibrary/classes/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoJob.py` & `domolibrary-0.1.92/domolibrary/classes/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.92/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoPage.py` & `domolibrary-0.1.92/domolibrary/classes/DomoPage.py`

 * *Files 5% similar despite different names*

```diff
@@ -629,55 +629,56 @@
         debug_api=debug_api, session=session,
     )
 
     return res
 
 
 # %% ../../nbs/classes/50_DomoPage.ipynb 20
-@dataclass
-class DomoPages:
-    pass
+@patch_to(DomoPage, cls_method=True)
+async def get_cards(cls,
+                    auth: dmda.DomoAuth,
+                    page_id, debug_api: bool = False,
+                    session: httpx.AsyncClient = None):
 
-# %% ../../nbs/classes/50_DomoPage.ipynb 21
-@patch_to(DomoPages, cls_method=True)
-async def get_pages(
-    cls: DomoPages,
-    auth=dmda.DomoAuth,
-    return_raw: bool = False,
-    debug_loop: bool = False,
-    debug_api: bool = False,
-    session: httpx.AsyncClient = None,
-):
-    is_close_session = False if session else True
+    import domolibrary.classes.DomoCard as dc
 
-    session = session or httpx.AsyncClient()
+    res = await page_routes.get_page_definition(auth=auth, page_id=page_id, debug_api=debug_api, session=session)
 
-    try:
-        res = await page_routes.get_pages_adminsummary(
-            auth=auth, debug_loop=False, debug_api=False, session=session
-        )
+    if res.status != 200:
+        raise Exception(
+            f"unable to retrieve page definition for {page_id} in {auth.domo_instance}")
 
-        if return_raw:
-            return res
+    if len(res.response.get('cards')) == 0:
+        return []
 
-        if not res.is_success:
-            raise Exception("unable to retrieve pages")
+    return await asyncio.gather(*[dc.DomoCard.get_by_id(card_id=card['id'],
+                                                  auth=auth) for card in res.response.get('cards')])
 
-        return await asyncio.gather(
-            *[
-                DomoPage._from_adminsummary(page_obj, auth=auth)
-                for page_obj in res.response
-            ]
-        )
 
-    finally:
-        if is_close_session:
-            await session.aclose()
+@patch_to(DomoPage, cls_method=True)
+async def get_datasets(cls,
+                       auth: dmda.DomoAuth,
+                       page_id,
+                       debug_api: bool = False,
+                       session: httpx.AsyncClient = None):
+
+    import domolibrary.classes.DomoDataset as dmds
 
-# %% ../../nbs/classes/50_DomoPage.ipynb 24
+    res = await page_routes.get_page_definition(auth=auth, page_id=page_id,
+                                                debug_api=debug_api, session=session)
+
+    if res.status != 200:
+        raise Exception( f"unable to retrieve datasets for page {page_id} in {auth.domo_instance}")
+
+    if len(res.response.get('cards')) == 0:
+        return []
+
+    return await asyncio.gather(*[ dmds.DomoDataset.get_from_id(dataset_id = ds.get('dataSourceId'), auth = auth) for card in res.response.get('cards') for ds in card.get('datasources')])
+
+# %% ../../nbs/classes/50_DomoPage.ipynb 23
 from datetime import datetime
 from utils import convert
 
 
 @patch_to(DomoPage, cls_method=True)
 async def update_layout(
     cls, auth: dmda.DomoAuth, body: dict, layout_id: str, debug_api: bool = False
@@ -705,7 +706,46 @@
         if res_writelock.status != 200:
             return False
 
     else:
         return False
 
     return True
+
+# %% ../../nbs/classes/50_DomoPage.ipynb 28
+@dataclass
+class DomoPages:
+    
+    @classmethod
+    async def get_pages(
+        cls,
+        auth=dmda.DomoAuth,
+        return_raw: bool = False,
+        debug_loop: bool = False,
+        debug_api: bool = False,
+        session: httpx.AsyncClient = None,
+    ):
+        is_close_session = False if session else True
+
+        session = session or httpx.AsyncClient()
+
+        try:
+            res = await page_routes.get_pages_adminsummary(
+                auth=auth, debug_loop=False, debug_api=False, session=session
+            )
+
+            if return_raw:
+                return res
+
+            if not res.is_success:
+                raise Exception("unable to retrieve pages")
+
+            return await asyncio.gather(
+                *[
+                    DomoPage._from_adminsummary(page_obj, auth=auth)
+                    for page_obj in res.response
+                ]
+            )
+
+        finally:
+            if is_close_session:
+                await session.aclose()
```

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoPublish.py` & `domolibrary-0.1.92/domolibrary/classes/DomoPublish.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.DomoError as de
 import domolibrary.routes.publish as publish_routes
 
 # import Library.DomoClasses.DomoDataset as dmda
-# import Library.DomoClasses.DomoLineage as dmdl
+import domolibrary.classes.DomoLineage as dmdl
 
 # %% ../../nbs/classes/50_DomoPublish.ipynb 4
 @dataclass
 class DomoPublication_Subscription:
     subscription_id: str
     publication_id: str
     domain: str
@@ -112,19 +112,18 @@
         default_factory=list
     )
     content: [DomoPublication_Content] = field(default_factory=list)
 
     content_page_id_ls: [str] = field(default_factory=list)
     content_dataset_id_ls: [str] = field(default_factory=list)
 
-    # lineage: dmdl.DomoLineage = None
+    lineage: dmdl.DomoLineage = None
 
-    # def __post_init__(self):
-    #     self.lineage = dmdl.DomoLineage(id=self.id,
-    #                                     parent=self)
+    def __post_init__(self):
+        self.lineage = dmdl.DomoLineage(parent=self)
 
     @classmethod
     def _from_json(cls, obj, auth: dmda.DomoAuth = None):
 
         dd = util_dd.DictDot(obj)
 
         domo_pub = cls(
@@ -162,15 +161,15 @@
                         publication_id=domo_pub.id, 
                         content_type=dmpc.entity_type, 
                         domo_instance=auth.domo_instance)
 
         return domo_pub
 
 
-# %% ../../nbs/classes/50_DomoPublish.ipynb 11
+# %% ../../nbs/classes/50_DomoPublish.ipynb 10
 @patch_to(DomoPublication, cls_method=True)
 async def get_from_id(cls, publication_id=None, auth: dmda.DomoAuth = None, timeout = 10):
 
     auth = auth or cls.auth
 
     publication_id = publication_id or cls.publication_id
 
@@ -180,15 +179,15 @@
     )
 
     if not res.is_success:
         return None
 
     return cls._from_json(obj=res.response, auth=auth)
 
-# %% ../../nbs/classes/50_DomoPublish.ipynb 16
+# %% ../../nbs/classes/50_DomoPublish.ipynb 15
 @dataclass
 class DomoPublications:
 
     @classmethod
     async def get_subscription_summaries(cls, 
                                          auth: dmda.DomoAuth,
                                          session: httpx.AsyncClient = None,
@@ -210,15 +209,15 @@
         sub_ls = res.response
 
         return [ sub for sub in sub_ls]
         
         
 
 
-# %% ../../nbs/classes/50_DomoPublish.ipynb 19
+# %% ../../nbs/classes/50_DomoPublish.ipynb 18
 @patch_to(DomoPublications, cls_method=True)
 async def search_publications(cls: DomoPublications,
                               auth = dmda.DomoAuth,
                               search_term: str = None,
                               session: httpx.AsyncClient = None,
                               debug_api: bool = False,
                               return_raw: bool = False):
@@ -230,15 +229,15 @@
 
     if not res.is_success or (res.is_success and len(res.response) == 0):
         return None
 
     return [DomoPublication._from_json(sub_obj)for sub_obj in res.response]
 
 
-# %% ../../nbs/classes/50_DomoPublish.ipynb 22
+# %% ../../nbs/classes/50_DomoPublish.ipynb 21
 @patch_to(DomoPublication, cls_method=True)
 async def create_publication(cls,
                                  name: str,
                                  content_ls: [DomoPublication_Content],
                                  subscription_ls: [DomoPublication_Subscription],
                                  unique_id: str = None,
                                  description: str = None,
@@ -280,15 +279,15 @@
             return None
         else:
             return cls._from_json(obj=res.response, auth=auth)
 
     return cls._from_json(obj=res.response, auth=auth)
 
 
-# %% ../../nbs/classes/50_DomoPublish.ipynb 24
+# %% ../../nbs/classes/50_DomoPublish.ipynb 23
 @patch_to(DomoPublication, cls_method=True)
 async def update_publication(cls,
                                  name: str,
                                  content_ls: [DomoPublication_Content],
                                  subscription_ls: [DomoPublication_Subscription],
                                  publication_id: str,
                                  description: str = None,
@@ -331,15 +330,15 @@
             return cls._from_json(obj=res.response, auth=auth)
 
     return cls._from_json(obj=res.response, auth=auth)
 
 
 
 
-# %% ../../nbs/classes/50_DomoPublish.ipynb 26
+# %% ../../nbs/classes/50_DomoPublish.ipynb 25
 @patch_to(DomoPublication, cls_method=True)
 async def get_subscription_invites_list(cls, auth: dmda.DomoAuth,
                                             debug_api: bool = False):
 
     res = await publish_routes.get_subscription_invititations(auth=auth,
                                                                 debug_api=debug_api)
     if debug_api:
```

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.92/domolibrary/classes/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoStream.py` & `domolibrary-0.1.92/domolibrary/classes/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.92/domolibrary/classes/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.92/domolibrary/client/DomoAuth.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,72 +242,82 @@
     def generate_auth_header(self, token: str) -> dict:
         self.auth_header = {"x-domo-authentication": token}
         return self.auth_header
 
     async def get_auth_token(
         self,
         session: Optional[httpx.AsyncClient] = None,
+        return_raw: bool = False,
         debug_api : bool = False
     ) -> str:
         """returns `token` if valid credentials provided else raises Exception and returns None"""
 
         res = await get_full_auth(
             domo_instance=self.domo_instance,
             domo_username=self.domo_username,
             domo_password=self.domo_password,
             session=session,
             debug_api = debug_api
         )
 
+        if return_raw:
+            return res
+
+
         if res.is_success and res.response.get("reason") == "INVALID_CREDENTIALS":
             self.is_valid_token = False
             raise InvalidCredentialsError(
                 function_name = "get_auth_token",
                 status=res.status,
                 message=str(res.response.get("reason")),
                 domo_instance=self.domo_instance,
             )
+            return None
 
-        if res.status == 403:
+        if res.status == 403: # invalid instance
             self.is_valid_token = False
             raise InvalidInstanceError(
                 function_name = "get_auth_token",
                 status=res.status,
                 message="INVALID INSTANCE",
                 domo_instance=self.domo_instance,
             )
+            return None
         
-        if res.is_success and res.response == {}:
+        if res.is_success and ( res.response == {} or res.response == '') : # no access token
             self.is_valid_token = False
             raise NoAccessTokenReturned(
                 function_name="get_auth_token",
                 status=res.status, 
                 domo_instance=self.domo_instance)
-        
+
+            return None
+
+
         self.is_valid_token = True
 
         token = str(res.response.get("sessionToken"))
         self.token = token
         self.user_id = str(res.response.get("userId"))
 
         self.auth_header = self.generate_auth_header(token=token)
 
         if not self.token_name:
             self.token_name = "full_auth"
 
         return self.token
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 36
+# %% ../../nbs/client/95_DomoAuth.ipynb 35
 @dataclass
 class _DomoTokenAuth_Required(_DomoAuth_Required):
     """mix requied parameters for DomoFullAuth"""
 
     domo_access_token: str = field(repr=False)
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 37
+# %% ../../nbs/client/95_DomoAuth.ipynb 36
 @dataclass
 class DomoTokenAuth(_DomoAuth_Optional, _DomoTokenAuth_Required):
     
 
     """
     use for access_token authentication.
     Tokens are generated in domo > admin > access token
@@ -351,23 +361,23 @@
         self.auth_header = self.generate_auth_header(token=self.token)
 
         if not self.token_name:
             self.token_name = "token_auth"
 
         return self.token
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 41
+# %% ../../nbs/client/95_DomoAuth.ipynb 40
 @dataclass
 class _DomoDeveloperAuth_Required(_DomoAuth_Required):
     """mix requied parameters for DomoFullAuth"""
 
     domo_client_id: str
     domo_client_secret: str = field(repr=False)
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 42
+# %% ../../nbs/client/95_DomoAuth.ipynb 41
 @dataclass(init=False)
 class DomoDeveloperAuth(_DomoAuth_Optional, _DomoDeveloperAuth_Required):
     """use for full authentication token"""
 
     def __init__(self, domo_client_id: str, domo_client_secret: str):
         self.domo_client_id = domo_client_id
         self.domo_client_secret = domo_client_secret
```

### Comparing `domolibrary-0.1.91/domolibrary/client/DomoError.py` & `domolibrary-0.1.92/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/client/Logger.py` & `domolibrary-0.1.92/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.92/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/client/get_data.py` & `domolibrary-0.1.92/domolibrary/client/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/integrations/Automation.py` & `domolibrary-0.1.92/domolibrary/integrations/Automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.92/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.92/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/account.py` & `domolibrary-0.1.92/domolibrary/routes/account.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/activity_log.py` & `domolibrary-0.1.92/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/application.py` & `domolibrary-0.1.92/domolibrary/routes/application.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.92/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/card.py` & `domolibrary-0.1.92/domolibrary/routes/card.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/datacenter.py` & `domolibrary-0.1.92/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/dataflow.py` & `domolibrary-0.1.92/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/dataset.py` & `domolibrary-0.1.92/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/grant.py` & `domolibrary-0.1.92/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/group.py` & `domolibrary-0.1.92/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/instance_config.py` & `domolibrary-0.1.92/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/job.py` & `domolibrary-0.1.92/domolibrary/routes/job.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/page.py` & `domolibrary-0.1.92/domolibrary/routes/page.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/pdp.py` & `domolibrary-0.1.92/domolibrary/routes/pdp.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/publish.py` & `domolibrary-0.1.92/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/role.py` & `domolibrary-0.1.92/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/stream.py` & `domolibrary-0.1.92/domolibrary/routes/stream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/routes/user.py` & `domolibrary-0.1.92/domolibrary/routes/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/utils/DictDot.py` & `domolibrary-0.1.92/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.92/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/utils/convert.py` & `domolibrary-0.1.92/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.92/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary/utils/upload_data.py` & `domolibrary-0.1.92/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.92/domolibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.91
+Version: 0.1.92
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary-0.1.91/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.92/domolibrary.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 domolibrary/classes/DomoDatacenter.py
 domolibrary/classes/DomoDataflow.py
 domolibrary/classes/DomoDataset.py
 domolibrary/classes/DomoGrant.py
 domolibrary/classes/DomoGroup.py
 domolibrary/classes/DomoInstanceConfig.py
 domolibrary/classes/DomoJob.py
+domolibrary/classes/DomoLineage.py
 domolibrary/classes/DomoPDP.py
 domolibrary/classes/DomoPage.py
 domolibrary/classes/DomoPublish.py
 domolibrary/classes/DomoRole.py
 domolibrary/classes/DomoStream.py
 domolibrary/classes/DomoUser.py
 domolibrary/classes/__init__.py
```

### Comparing `domolibrary-0.1.91/settings.ini` & `domolibrary-0.1.92/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.91
+version = 0.1.92
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.91/setup.py` & `domolibrary-0.1.92/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/utils/Base.py` & `domolibrary-0.1.92/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/utils/DictDot.py` & `domolibrary-0.1.92/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/utils/Exceptions.py` & `domolibrary-0.1.92/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/utils/LoggerClass.py` & `domolibrary-0.1.92/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/utils/chunk_execution.py` & `domolibrary-0.1.92/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/utils/consol_get_creds.py` & `domolibrary-0.1.92/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/utils/convert.py` & `domolibrary-0.1.92/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.92/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.91/utils/upload_data.py` & `domolibrary-0.1.92/utils/upload_data.py`

 * *Files identical despite different names*

