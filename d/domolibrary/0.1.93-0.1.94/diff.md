# Comparing `tmp/domolibrary-0.1.93.tar.gz` & `tmp/domolibrary-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.93.tar", last modified: Fri Jul  7 17:26:21 2023, max compression
+gzip compressed data, was "domolibrary-0.1.94.tar", last modified: Fri Jul  7 19:28:23 2023, max compression
```

## Comparing `domolibrary-0.1.93.tar` & `domolibrary-0.1.94.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.529397 domolibrary-0.1.93/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.481397 domolibrary-0.1.93/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-06-01 20:57:16.000000 domolibrary-0.1.93/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.485397 domolibrary-0.1.93/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.489397 domolibrary-0.1.93/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.497397 domolibrary-0.1.93/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.497397 domolibrary-0.1.93/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-01 20:57:16.000000 domolibrary-0.1.93/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-06-01 20:57:16.000000 domolibrary-0.1.93/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-06-01 20:57:16.000000 domolibrary-0.1.93/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 17:26:21.529397 domolibrary-0.1.93/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-06-01 20:57:16.000000 domolibrary-0.1.93/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.497397 domolibrary-0.1.93/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   182743 2023-07-07 17:25:48.000000 domolibrary-0.1.93/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.509397 domolibrary-0.1.93/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24179 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3477 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3962 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6722 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23039 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12268 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.509397 domolibrary-0.1.93/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12946 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12077 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.509397 domolibrary-0.1.93/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/integrations/Automation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.521397 domolibrary-0.1.93/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/application.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2369 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8439 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/job.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/stream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.525397 domolibrary-0.1.93/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.497397 domolibrary-0.1.93/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4141 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-01 20:57:34.000000 domolibrary-0.1.93/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-07-07 17:24:47.000000 domolibrary-0.1.93/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-07 17:26:21.529397 domolibrary-0.1.93/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-06-01 20:57:16.000000 domolibrary-0.1.93/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.529397 domolibrary-0.1.93/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.663216 domolibrary-0.1.94/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.579216 domolibrary-0.1.94/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.94/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-06-01 20:57:16.000000 domolibrary-0.1.94/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.591216 domolibrary-0.1.94/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.94/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.607216 domolibrary-0.1.94/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.94/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.623216 domolibrary-0.1.94/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.94/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-06-01 20:57:16.000000 domolibrary-0.1.94/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.623216 domolibrary-0.1.94/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.94/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-01 20:57:16.000000 domolibrary-0.1.94/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-06-01 20:57:16.000000 domolibrary-0.1.94/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-06-01 20:57:16.000000 domolibrary-0.1.94/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 19:28:23.663216 domolibrary-0.1.94/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-06-01 20:57:16.000000 domolibrary-0.1.94/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.623216 domolibrary-0.1.94/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   183314 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.647216 domolibrary-0.1.94/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24179 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3477 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3962 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6722 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23039 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12268 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.651216 domolibrary-0.1.94/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12946 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12077 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.651216 domolibrary-0.1.94/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/integrations/Automation.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.655216 domolibrary-0.1.94/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/application.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2369 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8439 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/job.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/stream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10314 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.659216 domolibrary-0.1.94/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-07-07 19:25:49.000000 domolibrary-0.1.94/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.627216 domolibrary-0.1.94/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 19:28:23.000000 domolibrary-0.1.94/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4141 2023-07-07 19:28:23.000000 domolibrary-0.1.94/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-07 19:28:23.000000 domolibrary-0.1.94/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-07-07 19:28:23.000000 domolibrary-0.1.94/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-01 20:57:34.000000 domolibrary-0.1.94/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-07-07 19:28:23.000000 domolibrary-0.1.94/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-07-07 19:28:23.000000 domolibrary-0.1.94/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-07-07 19:28:21.000000 domolibrary-0.1.94/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-07 19:28:23.663216 domolibrary-0.1.94/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-06-01 20:57:16.000000 domolibrary-0.1.94/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 19:28:23.663216 domolibrary-0.1.94/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-06-01 20:57:16.000000 domolibrary-0.1.94/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-06-01 20:57:16.000000 domolibrary-0.1.94/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-06-01 20:57:16.000000 domolibrary-0.1.94/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-06-01 20:57:16.000000 domolibrary-0.1.94/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-06-01 20:57:16.000000 domolibrary-0.1.94/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.94/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-06-01 20:57:16.000000 domolibrary-0.1.94/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-06-01 20:57:16.000000 domolibrary-0.1.94/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-06-01 20:57:16.000000 domolibrary-0.1.94/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-01 20:57:16.000000 domolibrary-0.1.94/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-06-01 20:57:16.000000 domolibrary-0.1.94/utils/upload_data.py
```

### Comparing `domolibrary-0.1.93/Automation/automation.py` & `domolibrary-0.1.94/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DataOcean/Transport.py` & `domolibrary-0.1.94/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.94/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.94/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DataOcean/cnfg_s3.py` & `domolibrary-0.1.94/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.94/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoAccount.py` & `domolibrary-0.1.94/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.94/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.94/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoApplication.py` & `domolibrary-0.1.94/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoAuth.py` & `domolibrary-0.1.94/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.94/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoCard.py` & `domolibrary-0.1.94/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoCertification.py` & `domolibrary-0.1.94/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.94/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.94/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoDataset.py` & `domolibrary-0.1.94/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoGrant.py` & `domolibrary-0.1.94/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoGroup.py` & `domolibrary-0.1.94/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.94/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoJob.py` & `domolibrary-0.1.94/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoLineage.py` & `domolibrary-0.1.94/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoPDP.py` & `domolibrary-0.1.94/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoPage.py` & `domolibrary-0.1.94/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoPublish.py` & `domolibrary-0.1.94/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoRole.py` & `domolibrary-0.1.94/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.94/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoStream.py` & `domolibrary-0.1.94/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoTag.py` & `domolibrary-0.1.94/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/DomoUser.py` & `domolibrary-0.1.94/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/get_data.py` & `domolibrary-0.1.94/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.94/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/LICENSE` & `domolibrary-0.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/PKG-INFO` & `domolibrary-0.1.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.93
+Version: 0.1.94
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary-0.1.93/README.md` & `domolibrary-0.1.94/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/_modidx.py` & `domolibrary-0.1.94/domolibrary/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1132,15 +1132,19 @@
                                                                                         'domolibrary/routes/stream.py'),
                                            'domolibrary.routes.stream.execute_stream': ( 'routes/stream.html#execute_stream',
                                                                                          'domolibrary/routes/stream.py'),
                                            'domolibrary.routes.stream.get_stream_by_id': ( 'routes/stream.html#get_stream_by_id',
                                                                                            'domolibrary/routes/stream.py'),
                                            'domolibrary.routes.stream.update_stream': ( 'routes/stream.html#update_stream',
                                                                                         'domolibrary/routes/stream.py')},
-            'domolibrary.routes.user': { 'domolibrary.routes.user.SearchUser_NoResults': ( 'routes/user.html#searchuser_noresults',
+            'domolibrary.routes.user': { 'domolibrary.routes.user.ResetPassword_PasswordUsed': ( 'routes/user.html#resetpassword_passwordused',
+                                                                                                 'domolibrary/routes/user.py'),
+                                         'domolibrary.routes.user.ResetPassword_PasswordUsed.__init__': ( 'routes/user.html#resetpassword_passwordused.__init__',
+                                                                                                          'domolibrary/routes/user.py'),
+                                         'domolibrary.routes.user.SearchUser_NoResults': ( 'routes/user.html#searchuser_noresults',
                                                                                            'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.SearchUser_NoResults.__init__': ( 'routes/user.html#searchuser_noresults.__init__',
                                                                                                     'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.UserProperty': ( 'routes/user.html#userproperty',
                                                                                    'domolibrary/routes/user.py'),
                                          'domolibrary.routes.user.UserProperty.__init__': ( 'routes/user.html#userproperty.__init__',
                                                                                             'domolibrary/routes/user.py'),
```

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.94/domolibrary/classes/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.94/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoApplication.py` & `domolibrary-0.1.94/domolibrary/classes/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.94/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoCard.py` & `domolibrary-0.1.94/domolibrary/classes/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.94/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.94/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.94/domolibrary/classes/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.94/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.94/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.94/domolibrary/classes/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoJob.py` & `domolibrary-0.1.94/domolibrary/classes/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoLineage.py` & `domolibrary-0.1.94/domolibrary/classes/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.94/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoPage.py` & `domolibrary-0.1.94/domolibrary/classes/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoPublish.py` & `domolibrary-0.1.94/domolibrary/classes/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.94/domolibrary/classes/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoStream.py` & `domolibrary-0.1.94/domolibrary/classes/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.94/domolibrary/classes/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.94/domolibrary/client/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/client/DomoError.py` & `domolibrary-0.1.94/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/client/Logger.py` & `domolibrary-0.1.94/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.94/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/client/get_data.py` & `domolibrary-0.1.94/domolibrary/client/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/integrations/Automation.py` & `domolibrary-0.1.94/domolibrary/integrations/Automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.94/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.94/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/account.py` & `domolibrary-0.1.94/domolibrary/routes/account.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/activity_log.py` & `domolibrary-0.1.94/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/application.py` & `domolibrary-0.1.94/domolibrary/routes/application.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.94/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/card.py` & `domolibrary-0.1.94/domolibrary/routes/card.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/datacenter.py` & `domolibrary-0.1.94/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/dataflow.py` & `domolibrary-0.1.94/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/dataset.py` & `domolibrary-0.1.94/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/grant.py` & `domolibrary-0.1.94/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/group.py` & `domolibrary-0.1.94/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/instance_config.py` & `domolibrary-0.1.94/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/job.py` & `domolibrary-0.1.94/domolibrary/routes/job.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/page.py` & `domolibrary-0.1.94/domolibrary/routes/page.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/pdp.py` & `domolibrary-0.1.94/domolibrary/routes/pdp.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/publish.py` & `domolibrary-0.1.94/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/role.py` & `domolibrary-0.1.94/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/stream.py` & `domolibrary-0.1.94/domolibrary/routes/stream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/routes/user.py` & `domolibrary-0.1.94/domolibrary/routes/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/user.ipynb.
 
 # %% auto 0
 __all__ = ['get_all_users', 'get_by_id', 'generate_search_users_body_by_id', 'generate_search_users_body_by_email',
            'process_v1_search_users', 'SearchUser_NoResults', 'search_users',
-           'search_virtual_user_by_subscriber_instance', 'create_user', 'set_user_landing_page', 'reset_password',
-           'request_password_reset', 'UserProperty_Type', 'UserProperty', 'generate_patch_user_property_body',
-           'update_user']
+           'search_virtual_user_by_subscriber_instance', 'create_user', 'set_user_landing_page',
+           'ResetPassword_PasswordUsed', 'reset_password', 'request_password_reset', 'UserProperty_Type',
+           'UserProperty', 'generate_patch_user_property_body', 'update_user']
 
 # %% ../../nbs/routes/user.ipynb 3
 from enum import Enum
 import httpx
 import asyncio
 
 import utils.DictDot as dd
@@ -219,50 +219,73 @@
         auth=auth,
         # body = body,
         debug_api=debug_api,
     )
 
 
 # %% ../../nbs/routes/user.ipynb 26
+class ResetPassword_PasswordUsed(de.DomoError):
+    def __init__(
+        self, status, domo_instance, 
+        function_name="reset_password", 
+        entity_id = None,
+        message="Password used previously"
+    ):
+
+        super().__init__(
+            message=message, status=status, function_name=function_name,
+            entity_id = entity_id,
+            domo_instance=domo_instance
+        )
+
+
 async def reset_password(
     auth: dmda.DomoAuth,
     user_id: str,
     new_password: str,
-    debug_api: bool = False,
+    debug_api: bool = False
 ) -> rgd.ResponseGetData:
 
     url = f"https://{auth.domo_instance}.domo.com/api/identity/v1/password"
 
     body = {"domoUserId": user_id, "password": new_password}
 
-    return await gd.get_data(
+    res = await gd.get_data(
         url=url,
         method="PUT",
         auth=auth,
         body=body,
         debug_api=debug_api,
     )
 
+    if res.status == 200 and res.response['description'] == 'Password has been used previously.':
+        raise ResetPassword_PasswordUsed(status=res.status,
+                                         entity_id=user_id,
+                                         domo_instance=auth.domo_instance,
+                                         message=res.response['description'].replace('.', ''))
+
+    return res
 
-# %% ../../nbs/routes/user.ipynb 27
+
+# %% ../../nbs/routes/user.ipynb 29
 async def request_password_reset(
     domo_instance: str, 
     email: str, locale="en-us", debug_api: bool = False,
     session : httpx.AsyncClient = None
 ):
     url = f"https://{domo_instance}.domo.com/api/domoweb/auth/sendReset"
 
     params = {"email": email, "local": locale}
 
     return await gd.get_data(
         url=url, method="GET", params=params, auth=None, debug_api=debug_api
     )
 
 
-# %% ../../nbs/routes/user.ipynb 29
+# %% ../../nbs/routes/user.ipynb 31
 class UserProperty_Type(Enum):
     display_name = "displayName"
     email_address = "emailAddress"
     phone_number = "phoneNumber"
     title = "title"
     department = "department"
     web_landing_page = "webLandingPage"
@@ -288,21 +311,21 @@
 
     def to_json(self):
         return {
             "key": self.property_type.value,
             "values": self._valid_value(self.values),
         }
 
-# %% ../../nbs/routes/user.ipynb 30
+# %% ../../nbs/routes/user.ipynb 32
 def generate_patch_user_property_body(user_property_ls: [UserProperty]):
     return {
         "attributes": [user_property.to_json() for user_property in user_property_ls]
     }
 
-# %% ../../nbs/routes/user.ipynb 33
+# %% ../../nbs/routes/user.ipynb 35
 async def update_user(
     user_id: str,
     user_property_ls: [UserProperty],
     auth: dmda.DomoAuth = None,
     debug_api: bool = False,
     session: httpx.AsyncClient = None,
 ):
```

### Comparing `domolibrary-0.1.93/domolibrary/utils/DictDot.py` & `domolibrary-0.1.94/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.94/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/utils/convert.py` & `domolibrary-0.1.94/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.94/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary/utils/upload_data.py` & `domolibrary-0.1.94/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.94/domolibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.93
+Version: 0.1.94
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary-0.1.93/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.94/domolibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/settings.ini` & `domolibrary-0.1.94/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.93
+version = 0.1.94
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.93/setup.py` & `domolibrary-0.1.94/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/utils/Base.py` & `domolibrary-0.1.94/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/utils/DictDot.py` & `domolibrary-0.1.94/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/utils/Exceptions.py` & `domolibrary-0.1.94/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/utils/LoggerClass.py` & `domolibrary-0.1.94/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/utils/chunk_execution.py` & `domolibrary-0.1.94/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/utils/consol_get_creds.py` & `domolibrary-0.1.94/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/utils/convert.py` & `domolibrary-0.1.94/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.94/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.93/utils/upload_data.py` & `domolibrary-0.1.94/utils/upload_data.py`

 * *Files identical despite different names*

