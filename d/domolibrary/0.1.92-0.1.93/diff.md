# Comparing `tmp/domolibrary-0.1.92.tar.gz` & `tmp/domolibrary-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.92.tar", last modified: Fri Jul  7 16:58:19 2023, max compression
+gzip compressed data, was "domolibrary-0.1.93.tar", last modified: Fri Jul  7 17:26:21 2023, max compression
```

## Comparing `domolibrary-0.1.92.tar` & `domolibrary-0.1.93.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.167051 domolibrary-0.1.92/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.723051 domolibrary-0.1.92/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-06-01 20:57:16.000000 domolibrary-0.1.92/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.727051 domolibrary-0.1.92/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.751051 domolibrary-0.1.92/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.783051 domolibrary-0.1.92/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-06-01 20:57:16.000000 domolibrary-0.1.92/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.791051 domolibrary-0.1.92/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-01 20:57:16.000000 domolibrary-0.1.92/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-06-01 20:57:16.000000 domolibrary-0.1.92/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-06-01 20:57:16.000000 domolibrary-0.1.92/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 16:58:19.167051 domolibrary-0.1.92/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-06-01 20:57:16.000000 domolibrary-0.1.92/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.795051 domolibrary-0.1.92/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   182743 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.955051 domolibrary-0.1.92/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24179 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3477 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3962 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6722 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23039 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12268 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.019051 domolibrary-0.1.92/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12077 2023-07-07 16:54:46.000000 domolibrary-0.1.92/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.027051 domolibrary-0.1.92/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/integrations/Automation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.131051 domolibrary-0.1.92/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/application.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2369 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8439 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/job.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/stream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.147051 domolibrary-0.1.92/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-07-07 16:54:47.000000 domolibrary-0.1.92/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:18.835051 domolibrary-0.1.92/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4141 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-01 20:57:34.000000 domolibrary-0.1.92/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-07-07 16:58:18.000000 domolibrary-0.1.92/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-07-07 16:58:04.000000 domolibrary-0.1.92/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-07 16:58:19.167051 domolibrary-0.1.92/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-06-01 20:57:16.000000 domolibrary-0.1.92/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 16:58:19.167051 domolibrary-0.1.92/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.92/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-06-01 20:57:16.000000 domolibrary-0.1.92/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.529397 domolibrary-0.1.93/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.481397 domolibrary-0.1.93/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-06-01 20:57:16.000000 domolibrary-0.1.93/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.485397 domolibrary-0.1.93/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.489397 domolibrary-0.1.93/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.497397 domolibrary-0.1.93/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-06-01 20:57:16.000000 domolibrary-0.1.93/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.497397 domolibrary-0.1.93/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-01 20:57:16.000000 domolibrary-0.1.93/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-06-01 20:57:16.000000 domolibrary-0.1.93/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-06-01 20:57:16.000000 domolibrary-0.1.93/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 17:26:21.529397 domolibrary-0.1.93/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8233 2023-06-01 20:57:16.000000 domolibrary-0.1.93/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.497397 domolibrary-0.1.93/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   182743 2023-07-07 17:25:48.000000 domolibrary-0.1.93/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.509397 domolibrary-0.1.93/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24179 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4968 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3477 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3815 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3962 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3034 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30233 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17308 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7498 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12866 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6722 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10353 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23039 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12268 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15694 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6668 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14376 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.509397 domolibrary-0.1.93/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12946 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12077 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.509397 domolibrary-0.1.93/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1807 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/integrations/Automation.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13823 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.521397 domolibrary-0.1.93/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8573 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1563 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/application.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2369 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4717 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8439 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1323 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20295 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4810 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6157 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/job.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4701 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7357 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6181 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2466 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/stream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.525397 domolibrary-0.1.93/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4713 2023-07-07 17:25:47.000000 domolibrary-0.1.93/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.497397 domolibrary-0.1.93/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8973 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4141 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-01 20:57:34.000000 domolibrary-0.1.93/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-07-07 17:26:21.000000 domolibrary-0.1.93/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-07-07 17:24:47.000000 domolibrary-0.1.93/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-07 17:26:21.529397 domolibrary-0.1.93/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-06-01 20:57:16.000000 domolibrary-0.1.93/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-07 17:26:21.529397 domolibrary-0.1.93/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-01 20:57:58.000000 domolibrary-0.1.93/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-06-01 20:57:16.000000 domolibrary-0.1.93/utils/upload_data.py
```

### Comparing `domolibrary-0.1.92/Automation/automation.py` & `domolibrary-0.1.93/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DataOcean/Transport.py` & `domolibrary-0.1.93/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.93/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.93/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DataOcean/cnfg_s3.py` & `domolibrary-0.1.93/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.93/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoAccount.py` & `domolibrary-0.1.93/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.93/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.93/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoApplication.py` & `domolibrary-0.1.93/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoAuth.py` & `domolibrary-0.1.93/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.93/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoCard.py` & `domolibrary-0.1.93/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoCertification.py` & `domolibrary-0.1.93/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.93/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.93/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoDataset.py` & `domolibrary-0.1.93/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoGrant.py` & `domolibrary-0.1.93/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoGroup.py` & `domolibrary-0.1.93/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.93/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoJob.py` & `domolibrary-0.1.93/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoLineage.py` & `domolibrary-0.1.93/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoPDP.py` & `domolibrary-0.1.93/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoPage.py` & `domolibrary-0.1.93/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoPublish.py` & `domolibrary-0.1.93/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoRole.py` & `domolibrary-0.1.93/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.93/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoStream.py` & `domolibrary-0.1.93/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoTag.py` & `domolibrary-0.1.93/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/DomoUser.py` & `domolibrary-0.1.93/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/get_data.py` & `domolibrary-0.1.93/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.93/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/LICENSE` & `domolibrary-0.1.93/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/PKG-INFO` & `domolibrary-0.1.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.92
+Version: 0.1.93
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary-0.1.92/README.md` & `domolibrary-0.1.93/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/_modidx.py` & `domolibrary-0.1.93/domolibrary/_modidx.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.93/domolibrary/classes/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.93/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoApplication.py` & `domolibrary-0.1.93/domolibrary/classes/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.93/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoCard.py` & `domolibrary-0.1.93/domolibrary/classes/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.93/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.93/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.93/domolibrary/classes/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.93/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.93/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.93/domolibrary/classes/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoJob.py` & `domolibrary-0.1.93/domolibrary/classes/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoLineage.py` & `domolibrary-0.1.93/domolibrary/classes/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.93/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoPage.py` & `domolibrary-0.1.93/domolibrary/classes/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoPublish.py` & `domolibrary-0.1.93/domolibrary/classes/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.93/domolibrary/classes/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoStream.py` & `domolibrary-0.1.93/domolibrary/classes/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.93/domolibrary/classes/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.93/domolibrary/client/DomoAuth.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,17 @@
             debug_api = debug_api
         )
 
         if return_raw:
             return res
 
 
-        if res.is_success and res.response.get("reason") == "INVALID_CREDENTIALS":
+        if res.is_success and (
+            res.response.get("reason") == "INVALID_CREDENTIALS" 
+            or res.response.get("reason") == "ACCOUNT_LOCKED" ) :
             self.is_valid_token = False
             raise InvalidCredentialsError(
                 function_name = "get_auth_token",
                 status=res.status,
                 message=str(res.response.get("reason")),
                 domo_instance=self.domo_instance,
             )
```

### Comparing `domolibrary-0.1.92/domolibrary/client/DomoError.py` & `domolibrary-0.1.93/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/client/Logger.py` & `domolibrary-0.1.93/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.93/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/client/get_data.py` & `domolibrary-0.1.93/domolibrary/client/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/integrations/Automation.py` & `domolibrary-0.1.93/domolibrary/integrations/Automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.93/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.93/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/account.py` & `domolibrary-0.1.93/domolibrary/routes/account.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/activity_log.py` & `domolibrary-0.1.93/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/application.py` & `domolibrary-0.1.93/domolibrary/routes/application.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.93/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/card.py` & `domolibrary-0.1.93/domolibrary/routes/card.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/datacenter.py` & `domolibrary-0.1.93/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/dataflow.py` & `domolibrary-0.1.93/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/dataset.py` & `domolibrary-0.1.93/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/grant.py` & `domolibrary-0.1.93/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/group.py` & `domolibrary-0.1.93/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/instance_config.py` & `domolibrary-0.1.93/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/job.py` & `domolibrary-0.1.93/domolibrary/routes/job.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/page.py` & `domolibrary-0.1.93/domolibrary/routes/page.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/pdp.py` & `domolibrary-0.1.93/domolibrary/routes/pdp.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/publish.py` & `domolibrary-0.1.93/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/role.py` & `domolibrary-0.1.93/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/stream.py` & `domolibrary-0.1.93/domolibrary/routes/stream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/routes/user.py` & `domolibrary-0.1.93/domolibrary/routes/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/utils/DictDot.py` & `domolibrary-0.1.93/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.93/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/utils/convert.py` & `domolibrary-0.1.93/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.93/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary/utils/upload_data.py` & `domolibrary-0.1.93/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.93/domolibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.92
+Version: 0.1.93
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary-0.1.92/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.93/domolibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/settings.ini` & `domolibrary-0.1.93/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.92
+version = 0.1.93
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.92/setup.py` & `domolibrary-0.1.93/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/utils/Base.py` & `domolibrary-0.1.93/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/utils/DictDot.py` & `domolibrary-0.1.93/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/utils/Exceptions.py` & `domolibrary-0.1.93/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/utils/LoggerClass.py` & `domolibrary-0.1.93/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/utils/chunk_execution.py` & `domolibrary-0.1.93/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/utils/consol_get_creds.py` & `domolibrary-0.1.93/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/utils/convert.py` & `domolibrary-0.1.93/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.93/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.92/utils/upload_data.py` & `domolibrary-0.1.93/utils/upload_data.py`

 * *Files identical despite different names*

