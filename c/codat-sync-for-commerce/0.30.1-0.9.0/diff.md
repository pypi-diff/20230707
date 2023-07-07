# Comparing `tmp/codat-sync-for-commerce-0.30.1.tar.gz` & `tmp/codat-sync-for-commerce-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-commerce-0.30.1.tar", last modified: Fri Jul  7 09:29:44 2023, max compression
+gzip compressed data, was "codat-sync-for-commerce-0.9.0.tar", last modified: Wed Apr 26 15:03:44 2023, max compression
```

## Comparing `codat-sync-for-commerce-0.30.1.tar` & `codat-sync-for-commerce-0.9.0.tar`

### file list

```diff
@@ -1,97 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:44.665452 codat-sync-for-commerce-0.30.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-07 09:29:44.665452 codat-sync-for-commerce-0.30.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3105 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:29:44.665452 codat-sync-for-commerce-0.30.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:44.657451 codat-sync-for-commerce-0.30.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:44.661452 codat-sync-for-commerce-0.30.1/src/codat_sync_for_commerce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-07 09:29:44.000000 codat-sync-for-commerce-0.30.1/src/codat_sync_for_commerce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-07 09:29:44.000000 codat-sync-for-commerce-0.30.1/src/codat_sync_for_commerce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:29:44.000000 codat-sync-for-commerce-0.30.1/src/codat_sync_for_commerce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-07 09:29:44.000000 codat-sync-for-commerce-0.30.1/src/codat_sync_for_commerce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 09:29:44.000000 codat-sync-for-commerce-0.30.1/src/codat_sync_for_commerce.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:44.661452 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9870 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/company_management.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3984 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4048 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:44.661452 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:44.661452 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/create_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/create_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      799 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_integration_branding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_sync_flow_url.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      949 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_visible_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1617 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/list_companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1764 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/list_connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/list_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1015 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/request_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/request_sync_for_date_range.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      799 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/set_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      622 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/update_config_text_sync_flow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1156 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/update_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:44.665452 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2252 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1385 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/accountoption.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1447 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/branding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/brandingbutton.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/brandingimage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/brandinglogo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1166 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4998 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1720 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/configaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1335 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6202 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1180 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/createcompany.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      995 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/dataconnectionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2680 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/datatypefeature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2497 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/daterange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/featurestate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/featuretype.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1123 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/fees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/feessupplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      912 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/groupinglevels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/groupingperiod.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/halref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/imagereference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3183 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1185 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/invoicelevelselection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/invoicelinelevelselection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      876 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/invoicestatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/localization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/newpayments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/newtaxrates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      758 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/option.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      857 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2182 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/sales.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      338 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/sourcetype.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      750 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/supportedfeature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      558 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/syncflowurl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/syncrange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3832 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/syncsummary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1429 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/synctolatestargs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/taxrateamount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/taxratemapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/updateconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      609 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/visibleaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3294 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/sdkconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6170 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9933 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/sync_flow_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:44.665452 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-07 09:29:34.000000 codat-sync-for-commerce-0.30.1/src/codatsynccommerce/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3066 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.155307 codat-sync-for-commerce-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.155307 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.159307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8903 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/company_management.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3852 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.159307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.159307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      580 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/create_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      926 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/create_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      827 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_integration_branding.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1278 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_sync_flow_url.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      965 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_visible_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1634 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync_for_date_range.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/set_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_config_text_sync_flow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1021 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/accountoption.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1455 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/branding.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingbutton.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandinglogo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1178 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4171 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5409 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1192 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/createcompany.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/dataconnectionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2694 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/datatypefeature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2503 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/daterange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/featurestate_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/featuretype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/fees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/feessupplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupinglevels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupingperiod.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/halref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/imagereference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3226 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      860 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelevelselection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelinelevelselection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicestatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/localization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newpayments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1870 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newtaxrates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      764 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/option.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/sales.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/sourcetype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/supportedfeature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncflowurl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3854 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncsummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/synctolatestargs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxrateamount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxratemapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      596 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/updateconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/visibleaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4263 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4630 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8928 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync_flow_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/utils.py
```

### Comparing `codat-sync-for-commerce-0.30.1/PKG-INFO` & `codat-sync-for-commerce-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: codat-sync-for-commerce
-Version: 0.30.1
-Summary: Python Client SDK Generated by Speakeasy
-Home-page: UNKNOWN
-Author: Speakeasy
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # Sync for Commerce
 
 Embedded accounting integrations for POS and eCommerce platforms.
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
@@ -26,62 +14,61 @@
 <!-- Start SDK Example Usage -->
 ```python
 import codatsynccommerce
 from codatsynccommerce.models import shared
 
 s = codatsynccommerce.CodatSyncCommerce(
     security=shared.Security(
-        auth_header="Basic BASE_64_ENCODED(API_KEY)",
+        auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
+
 req = shared.CreateCompany(
-    name='Bob's Burgers',
+    name="Bob's Burgers",
 )
 
 res = s.company_management.create_company(req)
 
 if res.company is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### [company_management](docs/sdks/companymanagement/README.md)
+### [company_management](docs/companymanagement/README.md)
 
-* [create_company](docs/sdks/companymanagement/README.md#create_company) - Create Sync for Commerce company
-* [create_connection](docs/sdks/companymanagement/README.md#create_connection) - Create connection
-* [list_companies](docs/sdks/companymanagement/README.md#list_companies) - List companies
-* [list_connections](docs/sdks/companymanagement/README.md#list_connections) - List data connections
-* [update_connection](docs/sdks/companymanagement/README.md#update_connection) - Update data connection
+* [create_company](docs/companymanagement/README.md#create_company) - Create Sync for Commerce company
+* [create_connection](docs/companymanagement/README.md#create_connection) - Create connection
+* [list_companies](docs/companymanagement/README.md#list_companies) - List companies
+* [list_connections](docs/companymanagement/README.md#list_connections) - List data connections
+* [update_connection](docs/companymanagement/README.md#update_connection) - Update data connection
 
-### [configuration](docs/sdks/configuration/README.md)
+### [configuration](docs/configuration/README.md)
 
-* [get_configuration](docs/sdks/configuration/README.md#get_configuration) - Retrieve config preferences set for a company.
-* [set_configuration](docs/sdks/configuration/README.md#set_configuration) - Create or update configuration.
+* [get_configuration](docs/configuration/README.md#get_configuration) - Retrieve config preferences set for a company.
+* [get_sync_status](docs/configuration/README.md#get_sync_status) - Get status for a company's syncs
+* [set_configuration](docs/configuration/README.md#set_configuration) - Create or update configuration.
 
-### [integrations](docs/sdks/integrations/README.md)
+### [integrations](docs/integrations/README.md)
 
-* [get_integration_branding](docs/sdks/integrations/README.md#get_integration_branding) - Get branding for an integration
-* [list_integrations](docs/sdks/integrations/README.md#list_integrations) - List information on Codat's supported integrations
+* [get_integration_branding](docs/integrations/README.md#get_integration_branding) - Get branding for an integration
+* [list_integrations](docs/integrations/README.md#list_integrations) - List information on Codat's supported integrations
 
-### [sync](docs/sdks/sync/README.md)
+### [sync](docs/sync/README.md)
 
-* [get_sync_status](docs/sdks/sync/README.md#get_sync_status) - Get status for a company's syncs
-* [request_sync](docs/sdks/sync/README.md#request_sync) - Sync new
-* [request_sync_for_date_range](docs/sdks/sync/README.md#request_sync_for_date_range) - Sync range
+* [request_sync](docs/sync/README.md#request_sync) - Run a Commerce sync from the last successful sync
+* [request_sync_for_date_range](docs/sync/README.md#request_sync_for_date_range) - Run a Commerce sync from a given date range
 
-### [sync_flow_preferences](docs/sdks/syncflowpreferences/README.md)
+### [sync_flow_preferences](docs/syncflowpreferences/README.md)
 
-* [get_config_text_sync_flow](docs/sdks/syncflowpreferences/README.md#get_config_text_sync_flow) - Retrieve preferences for text fields on Sync Flow
-* [get_sync_flow_url](docs/sdks/syncflowpreferences/README.md#get_sync_flow_url) - Retrieve sync flow url
-* [get_visible_accounts](docs/sdks/syncflowpreferences/README.md#get_visible_accounts) - List visible accounts
-* [update_config_text_sync_flow](docs/sdks/syncflowpreferences/README.md#update_config_text_sync_flow) - Update preferences for text fields on sync flow
-* [update_visible_accounts_sync_flow](docs/sdks/syncflowpreferences/README.md#update_visible_accounts_sync_flow) - Update the visible accounts on Sync Flow
+* [get_config_text_sync_flow](docs/syncflowpreferences/README.md#get_config_text_sync_flow) - Retrieve preferences for text fields on Sync Flow
+* [get_sync_flow_url](docs/syncflowpreferences/README.md#get_sync_flow_url) - Retrieve sync flow url
+* [get_visible_accounts](docs/syncflowpreferences/README.md#get_visible_accounts) - List visible accounts
+* [update_config_text_sync_flow](docs/syncflowpreferences/README.md#update_config_text_sync_flow) - Update preferences for text fields on sync flow
+* [update_visible_accounts_sync_flow](docs/syncflowpreferences/README.md#update_visible_accounts_sync_flow) - Update the visible accounts on Sync Flow
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
-
-
```

### Comparing `codat-sync-for-commerce-0.30.1/README.md` & `codat-sync-for-commerce-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: codat-sync-for-commerce
+Version: 0.9.0
+Summary: Python Client SDK Generated by Speakeasy
+Home-page: UNKNOWN
+Author: Speakeasy
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # Sync for Commerce
 
 Embedded accounting integrations for POS and eCommerce platforms.
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
@@ -14,60 +25,63 @@
 <!-- Start SDK Example Usage -->
 ```python
 import codatsynccommerce
 from codatsynccommerce.models import shared
 
 s = codatsynccommerce.CodatSyncCommerce(
     security=shared.Security(
-        auth_header="Basic BASE_64_ENCODED(API_KEY)",
+        auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
+
 req = shared.CreateCompany(
-    name='Bob's Burgers',
+    name="Bob's Burgers",
 )
 
 res = s.company_management.create_company(req)
 
 if res.company is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### [company_management](docs/sdks/companymanagement/README.md)
+### [company_management](docs/companymanagement/README.md)
 
-* [create_company](docs/sdks/companymanagement/README.md#create_company) - Create Sync for Commerce company
-* [create_connection](docs/sdks/companymanagement/README.md#create_connection) - Create connection
-* [list_companies](docs/sdks/companymanagement/README.md#list_companies) - List companies
-* [list_connections](docs/sdks/companymanagement/README.md#list_connections) - List data connections
-* [update_connection](docs/sdks/companymanagement/README.md#update_connection) - Update data connection
+* [create_company](docs/companymanagement/README.md#create_company) - Create Sync for Commerce company
+* [create_connection](docs/companymanagement/README.md#create_connection) - Create connection
+* [list_companies](docs/companymanagement/README.md#list_companies) - List companies
+* [list_connections](docs/companymanagement/README.md#list_connections) - List data connections
+* [update_connection](docs/companymanagement/README.md#update_connection) - Update data connection
 
-### [configuration](docs/sdks/configuration/README.md)
+### [configuration](docs/configuration/README.md)
 
-* [get_configuration](docs/sdks/configuration/README.md#get_configuration) - Retrieve config preferences set for a company.
-* [set_configuration](docs/sdks/configuration/README.md#set_configuration) - Create or update configuration.
+* [get_configuration](docs/configuration/README.md#get_configuration) - Retrieve config preferences set for a company.
+* [get_sync_status](docs/configuration/README.md#get_sync_status) - Get status for a company's syncs
+* [set_configuration](docs/configuration/README.md#set_configuration) - Create or update configuration.
 
-### [integrations](docs/sdks/integrations/README.md)
+### [integrations](docs/integrations/README.md)
 
-* [get_integration_branding](docs/sdks/integrations/README.md#get_integration_branding) - Get branding for an integration
-* [list_integrations](docs/sdks/integrations/README.md#list_integrations) - List information on Codat's supported integrations
+* [get_integration_branding](docs/integrations/README.md#get_integration_branding) - Get branding for an integration
+* [list_integrations](docs/integrations/README.md#list_integrations) - List information on Codat's supported integrations
 
-### [sync](docs/sdks/sync/README.md)
+### [sync](docs/sync/README.md)
 
-* [get_sync_status](docs/sdks/sync/README.md#get_sync_status) - Get status for a company's syncs
-* [request_sync](docs/sdks/sync/README.md#request_sync) - Sync new
-* [request_sync_for_date_range](docs/sdks/sync/README.md#request_sync_for_date_range) - Sync range
+* [request_sync](docs/sync/README.md#request_sync) - Run a Commerce sync from the last successful sync
+* [request_sync_for_date_range](docs/sync/README.md#request_sync_for_date_range) - Run a Commerce sync from a given date range
 
-### [sync_flow_preferences](docs/sdks/syncflowpreferences/README.md)
+### [sync_flow_preferences](docs/syncflowpreferences/README.md)
 
-* [get_config_text_sync_flow](docs/sdks/syncflowpreferences/README.md#get_config_text_sync_flow) - Retrieve preferences for text fields on Sync Flow
-* [get_sync_flow_url](docs/sdks/syncflowpreferences/README.md#get_sync_flow_url) - Retrieve sync flow url
-* [get_visible_accounts](docs/sdks/syncflowpreferences/README.md#get_visible_accounts) - List visible accounts
-* [update_config_text_sync_flow](docs/sdks/syncflowpreferences/README.md#update_config_text_sync_flow) - Update preferences for text fields on sync flow
-* [update_visible_accounts_sync_flow](docs/sdks/syncflowpreferences/README.md#update_visible_accounts_sync_flow) - Update the visible accounts on Sync Flow
+* [get_config_text_sync_flow](docs/syncflowpreferences/README.md#get_config_text_sync_flow) - Retrieve preferences for text fields on Sync Flow
+* [get_sync_flow_url](docs/syncflowpreferences/README.md#get_sync_flow_url) - Retrieve sync flow url
+* [get_visible_accounts](docs/syncflowpreferences/README.md#get_visible_accounts) - List visible accounts
+* [update_config_text_sync_flow](docs/syncflowpreferences/README.md#update_config_text_sync_flow) - Update preferences for text fields on sync flow
+* [update_visible_accounts_sync_flow](docs/syncflowpreferences/README.md#update_visible_accounts_sync_flow) - Update the visible accounts on Sync Flow
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
+
+
```

### Comparing `codat-sync-for-commerce-0.30.1/setup.py` & `codat-sync-for-commerce-0.9.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,37 +6,34 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-commerce",
-    version="0.30.1",
+    version="0.9.0",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
-        "certifi>=2022.12.7",
-        "charset-normalizer>=2.1.1",
-        "dataclasses-json-speakeasy>=0.5.8",
-        "idna>=3.3",
-        "jsonpath-python>=1.0.6 ",
-        "marshmallow>=3.17.1",
-        "marshmallow-enum>=1.5.1",
-        "mypy-extensions>=0.4.3",
-        "packaging>=21.3",
-        "pyparsing>=3.0.9",
-        "python-dateutil>=2.8.2",
-        "requests>=2.28.1",
-        "six>=1.16.0",
-        "typing-inspect>=0.8.0",
-        "typing_extensions>=4.3.0",
-        "urllib3>=1.26.12",
+        "certifi==2022.12.7",
+        "charset-normalizer==2.1.1",
+        "dataclasses-json-speakeasy==0.5.8",
+        "idna==3.3",
+        "marshmallow==3.17.1",
+        "marshmallow-enum==1.5.1",
+        "mypy-extensions==0.4.3",
+        "packaging==21.3",
+        "pyparsing==3.0.9",
+        "python-dateutil==2.8.2",
+        "requests==2.28.1",
+        "six==1.16.0",
+        "typing-inspect==0.8.0",
+        "typing_extensions==4.3.0",
+        "urllib3==1.26.12",
+        "pylint==2.16.2",
     ],
-    extras_require={
-        "dev":["pylint==2.16.2"]
-    },
     package_dir={'': 'src'},
     python_requires='>=3.9'
 )
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codat_sync_for_commerce.egg-info/PKG-INFO` & `codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-commerce
-Version: 0.30.1
+Version: 0.9.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 
 # Sync for Commerce
 
 Embedded accounting integrations for POS and eCommerce platforms.
 
 <!-- Start SDK Installation -->
 ## SDK Installation
@@ -26,62 +25,63 @@
 <!-- Start SDK Example Usage -->
 ```python
 import codatsynccommerce
 from codatsynccommerce.models import shared
 
 s = codatsynccommerce.CodatSyncCommerce(
     security=shared.Security(
-        auth_header="Basic BASE_64_ENCODED(API_KEY)",
+        auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
+
 req = shared.CreateCompany(
-    name='Bob's Burgers',
+    name="Bob's Burgers",
 )
 
 res = s.company_management.create_company(req)
 
 if res.company is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### [company_management](docs/sdks/companymanagement/README.md)
+### [company_management](docs/companymanagement/README.md)
 
-* [create_company](docs/sdks/companymanagement/README.md#create_company) - Create Sync for Commerce company
-* [create_connection](docs/sdks/companymanagement/README.md#create_connection) - Create connection
-* [list_companies](docs/sdks/companymanagement/README.md#list_companies) - List companies
-* [list_connections](docs/sdks/companymanagement/README.md#list_connections) - List data connections
-* [update_connection](docs/sdks/companymanagement/README.md#update_connection) - Update data connection
+* [create_company](docs/companymanagement/README.md#create_company) - Create Sync for Commerce company
+* [create_connection](docs/companymanagement/README.md#create_connection) - Create connection
+* [list_companies](docs/companymanagement/README.md#list_companies) - List companies
+* [list_connections](docs/companymanagement/README.md#list_connections) - List data connections
+* [update_connection](docs/companymanagement/README.md#update_connection) - Update data connection
 
-### [configuration](docs/sdks/configuration/README.md)
+### [configuration](docs/configuration/README.md)
 
-* [get_configuration](docs/sdks/configuration/README.md#get_configuration) - Retrieve config preferences set for a company.
-* [set_configuration](docs/sdks/configuration/README.md#set_configuration) - Create or update configuration.
+* [get_configuration](docs/configuration/README.md#get_configuration) - Retrieve config preferences set for a company.
+* [get_sync_status](docs/configuration/README.md#get_sync_status) - Get status for a company's syncs
+* [set_configuration](docs/configuration/README.md#set_configuration) - Create or update configuration.
 
-### [integrations](docs/sdks/integrations/README.md)
+### [integrations](docs/integrations/README.md)
 
-* [get_integration_branding](docs/sdks/integrations/README.md#get_integration_branding) - Get branding for an integration
-* [list_integrations](docs/sdks/integrations/README.md#list_integrations) - List information on Codat's supported integrations
+* [get_integration_branding](docs/integrations/README.md#get_integration_branding) - Get branding for an integration
+* [list_integrations](docs/integrations/README.md#list_integrations) - List information on Codat's supported integrations
 
-### [sync](docs/sdks/sync/README.md)
+### [sync](docs/sync/README.md)
 
-* [get_sync_status](docs/sdks/sync/README.md#get_sync_status) - Get status for a company's syncs
-* [request_sync](docs/sdks/sync/README.md#request_sync) - Sync new
-* [request_sync_for_date_range](docs/sdks/sync/README.md#request_sync_for_date_range) - Sync range
+* [request_sync](docs/sync/README.md#request_sync) - Run a Commerce sync from the last successful sync
+* [request_sync_for_date_range](docs/sync/README.md#request_sync_for_date_range) - Run a Commerce sync from a given date range
 
-### [sync_flow_preferences](docs/sdks/syncflowpreferences/README.md)
+### [sync_flow_preferences](docs/syncflowpreferences/README.md)
 
-* [get_config_text_sync_flow](docs/sdks/syncflowpreferences/README.md#get_config_text_sync_flow) - Retrieve preferences for text fields on Sync Flow
-* [get_sync_flow_url](docs/sdks/syncflowpreferences/README.md#get_sync_flow_url) - Retrieve sync flow url
-* [get_visible_accounts](docs/sdks/syncflowpreferences/README.md#get_visible_accounts) - List visible accounts
-* [update_config_text_sync_flow](docs/sdks/syncflowpreferences/README.md#update_config_text_sync_flow) - Update preferences for text fields on sync flow
-* [update_visible_accounts_sync_flow](docs/sdks/syncflowpreferences/README.md#update_visible_accounts_sync_flow) - Update the visible accounts on Sync Flow
+* [get_config_text_sync_flow](docs/syncflowpreferences/README.md#get_config_text_sync_flow) - Retrieve preferences for text fields on Sync Flow
+* [get_sync_flow_url](docs/syncflowpreferences/README.md#get_sync_flow_url) - Retrieve sync flow url
+* [get_visible_accounts](docs/syncflowpreferences/README.md#get_visible_accounts) - List visible accounts
+* [update_config_text_sync_flow](docs/syncflowpreferences/README.md#update_config_text_sync_flow) - Update preferences for text fields on sync flow
+* [update_visible_accounts_sync_flow](docs/syncflowpreferences/README.md#update_visible_accounts_sync_flow) - Update the visible accounts on Sync Flow
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codat_sync_for_commerce.egg-info/SOURCES.txt` & `codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 src/codat_sync_for_commerce.egg-info/requires.txt
 src/codat_sync_for_commerce.egg-info/top_level.txt
 src/codatsynccommerce/__init__.py
 src/codatsynccommerce/company_management.py
 src/codatsynccommerce/configuration.py
 src/codatsynccommerce/integrations.py
 src/codatsynccommerce/sdk.py
-src/codatsynccommerce/sdkconfiguration.py
 src/codatsynccommerce/sync.py
 src/codatsynccommerce/sync_flow_preferences.py
 src/codatsynccommerce/models/__init__.py
 src/codatsynccommerce/models/operations/__init__.py
 src/codatsynccommerce/models/operations/create_company.py
 src/codatsynccommerce/models/operations/create_connection.py
 src/codatsynccommerce/models/operations/get_config_text_sync_flow.py
@@ -43,19 +42,19 @@
 src/codatsynccommerce/models/shared/configaccount.py
 src/codatsynccommerce/models/shared/configuration.py
 src/codatsynccommerce/models/shared/connection.py
 src/codatsynccommerce/models/shared/connections.py
 src/codatsynccommerce/models/shared/createcompany.py
 src/codatsynccommerce/models/shared/customer.py
 src/codatsynccommerce/models/shared/dataconnectionerror.py
-src/codatsynccommerce/models/shared/dataconnectionstatus.py
+src/codatsynccommerce/models/shared/dataconnectionstatus_enum.py
 src/codatsynccommerce/models/shared/datatypefeature.py
 src/codatsynccommerce/models/shared/daterange.py
-src/codatsynccommerce/models/shared/featurestate.py
-src/codatsynccommerce/models/shared/featuretype.py
+src/codatsynccommerce/models/shared/featurestate_enum.py
+src/codatsynccommerce/models/shared/featuretype_enum.py
 src/codatsynccommerce/models/shared/fees.py
 src/codatsynccommerce/models/shared/feessupplier.py
 src/codatsynccommerce/models/shared/grouping.py
 src/codatsynccommerce/models/shared/groupinglevels.py
 src/codatsynccommerce/models/shared/groupingperiod.py
 src/codatsynccommerce/models/shared/halref.py
 src/codatsynccommerce/models/shared/imagereference.py
@@ -68,18 +67,17 @@
 src/codatsynccommerce/models/shared/localization.py
 src/codatsynccommerce/models/shared/newpayments.py
 src/codatsynccommerce/models/shared/newtaxrates.py
 src/codatsynccommerce/models/shared/option.py
 src/codatsynccommerce/models/shared/payments.py
 src/codatsynccommerce/models/shared/sales.py
 src/codatsynccommerce/models/shared/security.py
-src/codatsynccommerce/models/shared/sourcetype.py
+src/codatsynccommerce/models/shared/sourcetype_enum.py
 src/codatsynccommerce/models/shared/supportedfeature.py
 src/codatsynccommerce/models/shared/syncflowurl.py
-src/codatsynccommerce/models/shared/syncrange.py
 src/codatsynccommerce/models/shared/syncsummary.py
 src/codatsynccommerce/models/shared/synctolatestargs.py
 src/codatsynccommerce/models/shared/taxrateamount.py
 src/codatsynccommerce/models/shared/taxratemapping.py
 src/codatsynccommerce/models/shared/updateconnection.py
 src/codatsynccommerce/models/shared/visibleaccounts.py
 src/codatsynccommerce/utils/__init__.py
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/company_management.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/company_management.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from codatsynccommerce import utils
+import requests as requests_http
+from . import utils
 from codatsynccommerce.models import operations, shared
 from typing import Optional
 
 class CompanyManagement:
     r"""Create new and manage existing Sync for Commerce companies."""
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
     def create_company(self, request: shared.CreateCompany, retries: Optional[utils.RetryConfig] = None) -> operations.CreateCompanyResponse:
         r"""Create Sync for Commerce company
         Creates a Codat company with a commerce partner data connection.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/meta/companies/sync'
         
-        url = base_url + '/meta/companies/sync'
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
             return client.request('POST', url, data=data, files=form, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
@@ -48,34 +58,34 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
                 res.company = out
 
         return res
 
-    
     def create_connection(self, request: operations.CreateConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateConnectionResponse:
         r"""Create connection
         Create a data connection for company.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.CreateConnectionRequest, base_url, '/meta/companies/{companyId}/connections', request)
+        
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'string')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
             return client.request('POST', url, data=data, files=form, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
@@ -88,35 +98,34 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
 
         return res
 
-    
     def list_companies(self, request: operations.ListCompaniesRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListCompaniesResponse:
         r"""List companies
         Retrieve a list of all companies the client has created.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/meta/companies'
         
-        url = base_url + '/meta/companies'
-        headers = {}
         query_params = utils.get_query_params(operations.ListCompaniesRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
-            return client.request('GET', url, params=query_params, headers=headers)
+            return client.request('GET', url, params=query_params)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
@@ -126,35 +135,34 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Companies])
                 res.companies = out
 
         return res
 
-    
     def list_connections(self, request: operations.ListConnectionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListConnectionsResponse:
         r"""List data connections
         Retrieve previously created data connections.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ListConnectionsRequest, base_url, '/meta/companies/{companyId}/connections', request)
-        headers = {}
+        
         query_params = utils.get_query_params(operations.ListConnectionsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
-            return client.request('GET', url, params=query_params, headers=headers)
+            return client.request('GET', url, params=query_params)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
@@ -164,34 +172,34 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connections])
                 res.connections = out
 
         return res
 
-    
     def update_connection(self, request: operations.UpdateConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateConnectionResponse:
         r"""Update data connection
         Update a data connection
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateConnectionRequest, base_url, '/meta/companies/{companyId}/connections/{connectionId}', request)
+        
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "update_connection", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
             return client.request('PATCH', url, data=data, files=form, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/integrations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,98 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from codatsynccommerce import utils
+import requests as requests_http
+from . import utils
 from codatsynccommerce.models import operations, shared
 from typing import Optional
 
-class Configuration:
-    r"""Expressively configure preferences for any given Sync for Commerce company."""
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
-        
-    
-    def get_configuration(self, request: operations.GetConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetConfigurationResponse:
-        r"""Retrieve config preferences set for a company.
-        Retrieve current config preferences.
+class Integrations:
+    r"""View useful information about codat's integrations."""
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
+        
+    def get_integration_branding(self, request: operations.GetIntegrationBrandingRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetIntegrationBrandingResponse:
+        r"""Get branding for an integration
+        Retrieve Integration branding assets.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = utils.generate_url(operations.GetConfigurationRequest, base_url, '/config/companies/{companyId}/sync/commerce', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        url = utils.generate_url(operations.GetIntegrationBrandingRequest, base_url, '/config/integrations/{platformKey}/branding', request)
         
-        client = self.sdk_configuration.security_client
+        
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
-            return client.request('GET', url, headers=headers)
+            return client.request('GET', url)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetConfigurationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetIntegrationBrandingResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Configuration])
-                res.configuration = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Branding])
+                res.branding = out
 
         return res
 
-    
-    def set_configuration(self, request: operations.SetConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.SetConfigurationResponse:
-        r"""Create or update configuration.
-        Make changes to configuration preferences.
+    def list_integrations(self, request: operations.ListIntegrationsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListIntegrationsResponse:
+        r"""List information on Codat's supported integrations
+        Retrieve a list of available integrations support by datatype and state of release.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/config/integrations'
         
-        url = utils.generate_url(operations.SetConfigurationRequest, base_url, '/config/companies/{companyId}/sync/commerce', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        query_params = utils.get_query_params(operations.ListIntegrationsRequest, request)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
-            return client.request('POST', url, headers=headers)
+            return client.request('GET', url, params=query_params)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SetConfigurationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListIntegrationsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Configuration])
-                res.configuration = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Integrations])
+                res.integrations = out
 
         return res
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/__init__.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/create_company.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import company as shared_company
+from ..shared import localization as shared_localization
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class CreateCompanyResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    company: Optional[shared_company.Company] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class GetConfigTextSyncFlowResponse:
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    localization_info: Optional[dict[str, shared_localization.Localization]] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/create_connection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/create_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import connection as shared_connection
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class CreateConnectionRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    request_body: Optional[str] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
-
-
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    request_body: Optional[str] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    
 
 @dataclasses.dataclass
 class CreateConnectionResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    connection: Optional[shared_connection.Connection] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    connection: Optional[shared_connection.Connection] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_config_text_sync_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import localization as shared_localization
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class GetConfigTextSyncFlowResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    localization_info: Optional[dict[str, shared_localization.Localization]] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class UpdateConfigTextSyncFlowResponse:
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    localization_info: Optional[dict[str, shared_localization.Localization]] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import configuration as shared_configuration
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetConfigurationRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
-
-
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    
 
 @dataclasses.dataclass
 class GetConfigurationResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    configuration: Optional[shared_configuration.Configuration] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    configuration: Optional[shared_configuration.Configuration] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_integration_branding.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_integration_branding.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import branding as shared_branding
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetIntegrationBrandingRequest:
+    
     platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})
-    r"""PlatformKey"""
+    r"""PlatformKey"""  
     
 
-
-
-
 @dataclasses.dataclass
 class GetIntegrationBrandingResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    branding: Optional[shared_branding.Branding] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    branding: Optional[shared_branding.Branding] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_sync_flow_url.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_companies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import syncflowurl as shared_syncflowurl
+from ..shared import companies as shared_companies
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class GetSyncFlowURLRequest:
-    accounting_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'accountingKey', 'style': 'simple', 'explode': False }})
-    r"""Accounting platform key"""
-    commerce_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'commerceKey', 'style': 'simple', 'explode': False }})
-    r"""Commerce platform key"""
-    merchant_identifier: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'merchantIdentifier', 'style': 'form', 'explode': True }})
-    r"""Identifier for your merchant, can be the merchant name or Codat company id."""
+class ListCompaniesRequest:
+    
+    page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
+    order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
+    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""  
+    page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
+    query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
+    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""  
     
-
-
-
 
 @dataclasses.dataclass
-class GetSyncFlowURLResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    sync_flow_url: Optional[shared_syncflowurl.SyncFlowURL] = dataclasses.field(default=None)
-    r"""Success"""
+class ListCompaniesResponse:
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    companies: Optional[shared_companies.Companies] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_sync_status.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_sync_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetSyncStatusRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
-
-
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    
 
 @dataclasses.dataclass
 class GetSyncStatusResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/get_visible_accounts.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_visible_accounts.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import visibleaccounts as shared_visibleaccounts
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetVisibleAccountsRequest:
-    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
-    platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})
     
-
-
-
+    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})  
+    platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})  
+    
 
 @dataclasses.dataclass
 class GetVisibleAccountsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None)
-    r"""Success"""
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None)
+    r"""Success"""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/list_companies.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_connections.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import companies as shared_companies
+from ..shared import connections as shared_connections
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class ListCompaniesRequest:
+class ListConnectionsRequest:
+    
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
-    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""
-    page: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""  
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""
+    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""  
     
 
-
-
-
 @dataclasses.dataclass
-class ListCompaniesResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    companies: Optional[shared_companies.Companies] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class ListConnectionsResponse:
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    connections: Optional[shared_connections.Connections] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/list_connections.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_integrations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import connections as shared_connections
+from ..shared import integrations as shared_integrations
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class ListConnectionsRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+class ListIntegrationsRequest:
+    
+    page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
-    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""
-    page: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""  
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""
+    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""  
     
 
-
-
-
 @dataclasses.dataclass
-class ListConnectionsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    connections: Optional[shared_connections.Connections] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class ListIntegrationsResponse:
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    integrations: Optional[shared_integrations.Integrations] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/request_sync.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,23 @@
 import dataclasses
 import requests as requests_http
 from ..shared import syncsummary as shared_syncsummary
 from ..shared import synctolatestargs as shared_synctolatestargs
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class RequestSyncRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    sync_to_latest_args: Optional[shared_synctolatestargs.SyncToLatestArgs] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
-
-
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    sync_to_latest_args: Optional[shared_synctolatestargs.SyncToLatestArgs] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    
 
 @dataclasses.dataclass
 class RequestSyncResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    sync_summary: Optional[shared_syncsummary.SyncSummary] = dataclasses.field(default=None)
-    r"""Success"""
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    sync_summary: Optional[shared_syncsummary.SyncSummary] = dataclasses.field(default=None)
+    r"""Success"""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/request_sync_for_date_range.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync_for_date_range.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import syncrange as shared_syncrange
+from ..shared import daterange as shared_daterange
 from ..shared import syncsummary as shared_syncsummary
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class RequestSyncForDateRangeRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    sync_range: Optional[shared_syncrange.SyncRange] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
-
-
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    date_range: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    
 
 @dataclasses.dataclass
 class RequestSyncForDateRangeResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    sync_summary: Optional[shared_syncsummary.SyncSummary] = dataclasses.field(default=None)
-    r"""Success"""
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    sync_summary: Optional[shared_syncsummary.SyncSummary] = dataclasses.field(default=None)
+    r"""Success"""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/set_configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/set_configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import configuration as shared_configuration
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class SetConfigurationRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
-
-
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    
 
 @dataclasses.dataclass
 class SetConfigurationResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    configuration: Optional[shared_configuration.Configuration] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    configuration: Optional[shared_configuration.Configuration] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/update_connection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,27 +4,24 @@
 import dataclasses
 import requests as requests_http
 from ..shared import connection as shared_connection
 from ..shared import updateconnection as shared_updateconnection
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class UpdateConnectionRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    update_connection: Optional[shared_updateconnection.UpdateConnection] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
-
-
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    update_connection: Optional[shared_updateconnection.UpdateConnection] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    
 
 @dataclasses.dataclass
 class UpdateConnectionResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    connection: Optional[shared_connection.Connection] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    connection: Optional[shared_connection.Connection] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import visibleaccounts as shared_visibleaccounts
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class UpdateVisibleAccountsSyncFlowRequest:
-    commerce_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'commerceKey', 'style': 'simple', 'explode': False }})
-    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
-
-
-
+    commerce_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'commerceKey', 'style': 'simple', 'explode': False }})  
+    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    
 
 @dataclasses.dataclass
 class UpdateVisibleAccountsSyncFlowResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None)
-    r"""Success"""
     
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None)
+    r"""Success"""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/__init__.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from .configaccount import *
 from .configuration import *
 from .connection import *
 from .connections import *
 from .createcompany import *
 from .customer import *
 from .dataconnectionerror import *
-from .dataconnectionstatus import *
+from .dataconnectionstatus_enum import *
 from .datatypefeature import *
 from .daterange import *
-from .featurestate import *
-from .featuretype import *
+from .featurestate_enum import *
+from .featuretype_enum import *
 from .fees import *
 from .feessupplier import *
 from .grouping import *
 from .groupinglevels import *
 from .groupingperiod import *
 from .halref import *
 from .imagereference import *
@@ -35,19 +35,18 @@
 from .localization import *
 from .newpayments import *
 from .newtaxrates import *
 from .option import *
 from .payments import *
 from .sales import *
 from .security import *
-from .sourcetype import *
+from .sourcetype_enum import *
 from .supportedfeature import *
 from .syncflowurl import *
-from .syncrange import *
 from .syncsummary import *
 from .synctolatestargs import *
 from .taxrateamount import *
 from .taxratemapping import *
 from .updateconnection import *
 from .visibleaccounts import *
 
-__all__ = ["AccountOption","Branding","BrandingButton","BrandingImage","BrandingLogo","Companies","Company","ConfigAccount","Configuration","Connection","ConnectionSourceType","Connections","CreateCompany","Customer","DataConnectionError","DataConnectionStatus","DataTypeFeature","DataTypeFeatureDataType","DateRange","FeatureState","FeatureType","Fees","FeesSupplier","Grouping","GroupingLevels","GroupingPeriod","HalRef","ImageReference","Integration","Integrations","InvoiceLevelSelection","InvoiceLineLevelSelection","InvoiceStatus","Links","Localization","NewPayments","NewTaxRates","Option","Payments","Sales","Security","SourceType","SupportedFeature","SyncFlowURL","SyncRange","SyncRangeDateRange","SyncSummary","SyncToLatestArgs","TaxRateAmount","TaxRateMapping","UpdateConnection","VisibleAccounts"]
+__all__ = ["AccountOption","Branding","BrandingButton","BrandingImage","BrandingLogo","Companies","Company","ConfigAccount","Configuration","Connection","ConnectionSourceTypeEnum","Connections","CreateCompany","Customer","DataConnectionError","DataConnectionStatusEnum","DataTypeFeature","DataTypeFeatureDataTypeEnum","DateRange","FeatureStateEnum","FeatureTypeEnum","Fees","FeesSupplier","Grouping","GroupingLevels","GroupingPeriod","HalRef","ImageReference","Integration","Integrations","InvoiceLevelSelection","InvoiceLineLevelSelection","InvoiceStatus","Links","Localization","NewPayments","NewTaxRates","Option","Payments","Sales","Security","SourceTypeEnum","SupportedFeature","SyncFlowURL","SyncSummary","SyncToLatestArgs","TaxRateAmount","TaxRateMapping","UpdateConnection","VisibleAccounts"]
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/accountoption.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/accountoption.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class AccountOption:
+    
     classification: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('classification'), 'exclude': lambda f: f is None }})
-    r"""Classification of the type of G/L account."""
+    r"""Classification of the type of G/L account."""  
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Identifier for the account, unique for the company."""
+    r"""Identifier for the account, unique for the company."""  
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    r"""Name of the account."""
+    r"""Name of the account."""  
     nominal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nominalCode'), 'exclude': lambda f: f is None }})
-    r"""Reference given to each nominal account for a business. It ensures money is allocated to the correct account. This code isn't a unique identifier in the Codat system."""
-    
-
+    r"""Reference given to each nominal account for a business. It ensures money is allocated to the correct account. This code isn't a unique identifier in the Codat system."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/branding.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/branding.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 from ..shared import brandinglogo as shared_brandinglogo
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Branding:
     r"""Success"""
+    
     button: Optional[shared_brandingbutton.BrandingButton] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('button'), 'exclude': lambda f: f is None }})
-    r"""Button branding references."""
+    r"""Button branding references."""  
     logo: Optional[shared_brandinglogo.BrandingLogo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logo'), 'exclude': lambda f: f is None }})
-    r"""Logo branding references."""
+    r"""Logo branding references."""  
     source_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId'), 'exclude': lambda f: f is None }})
-    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
-    
-
+    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/brandingbutton.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingbutton.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from ..shared import brandingimage as shared_brandingimage
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class BrandingButton:
     r"""Button branding references."""
-    default: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default'), 'exclude': lambda f: f is None }})
-    hover: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hover'), 'exclude': lambda f: f is None }})
     
-
+    default: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default'), 'exclude': lambda f: f is None }})  
+    hover: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hover'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/brandingimage.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingimage.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import imagereference as shared_imagereference
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class BrandingImage:
-    image: Optional[shared_imagereference.ImageReference] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('image'), 'exclude': lambda f: f is None }})
-    r"""Image reference."""
     
-
+    image: Optional[shared_imagereference.ImageReference] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('image'), 'exclude': lambda f: f is None }})
+    r"""Image reference."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/brandinglogo.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandinglogo.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from ..shared import brandingimage as shared_brandingimage
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class BrandingLogo:
     r"""Logo branding references."""
-    full: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('full'), 'exclude': lambda f: f is None }})
-    square: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('square'), 'exclude': lambda f: f is None }})
     
-
+    full: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('full'), 'exclude': lambda f: f is None }})  
+    square: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('square'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/companies.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integrations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import company as shared_company
+from ..shared import integration as shared_integration
 from ..shared import links as shared_links
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Companies:
+class Integrations:
     r"""Success"""
-    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-    results: Optional[list[shared_company.Company]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
     
-
+    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
+    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
+    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
+    results: Optional[list[shared_integration.Integration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/company.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/company.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,24 @@
 from ..shared import connection as shared_connection
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Company:
-    r"""In Codat, a company represents a business sharing access to their data. Each company can have multiple [connections](https://docs.codat.io/codat-api#/schemas/Connection) to different data sources such as one connection to [Xero](https://docs.codat.io/integrations/accounting/xero/accounting-xero) for accounting data, two connections to [Plaid](https://docs.codat.io/integrations/banking/plaid/banking-plaid) for two bank accounts and a connection to [Zettle](https://docs.codat.io/integrations/commerce/zettle/commerce-zettle) for POS data.
-    
-    Typically each company is one of your customers.
+    r"""A company in Codat represent a small or medium sized business, whose data you wish to share"""
     
-    When you create a company, you can specify a `name` and we will automatically generate a unique `id` for the company. You can also add a `description` to store any additional information about the company.
-    """
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique identifier for your SMB in Codat."""
+    r"""Unique identifier for your SMB in Codat."""  
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    r"""The name of the company"""
+    r"""The name of the company"""  
     redirect: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('redirect') }})
-    r"""The `redirect` [Link URL](https://docs.codat.io/auth-flow/authorize-hosted-link) enabling the customer to start their auth flow journey for the company."""
+    r"""The `redirect` [Link URL](https://docs.codat.io/auth-flow/authorize-hosted-link) enabling the customer to start their auth flow journey for the company."""  
     created: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -40,19 +35,19 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    created_by_user_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdByUserName'), 'exclude': lambda f: f is None }})
-    data_connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnections'), 'exclude': lambda f: f is None }})
+    """  
+    created_by_user_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdByUserName'), 'exclude': lambda f: f is None }})  
+    data_connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnections'), 'exclude': lambda f: f is None }})  
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    r"""Additional information about the company. This can be used to store foreign IDs, references, etc."""
+    r"""Additional information about the company. This can be used to store foreign IDs, references, etc."""  
     last_sync: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSync'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -65,12 +60,10 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    platform: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platform'), 'exclude': lambda f: f is None }})
-    r"""Deprecated: this field will be removed in a future release, please migrate away from it as soon as possible"""
-    
-
+    """  
+    platform: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platform'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/configaccount.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configaccount.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 from ..shared import accountoption as shared_accountoption
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConfigAccount:
     r"""G/L account object for configuration."""
+    
     account_options: Optional[list[shared_accountoption.AccountOption]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountOptions'), 'exclude': lambda f: f is None }})
-    r"""Object containing account options."""
+    r"""Object containing account options."""  
     description_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptionText'), 'exclude': lambda f: f is None }})
-    r"""Descriprtive text for sales configuration section."""
+    r"""Descriprtive text for sales configuration section."""  
     label_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('labelText'), 'exclude': lambda f: f is None }})
-    r"""Label text for sales configuration section."""
+    r"""Label text for sales configuration section."""  
     required: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required'), 'exclude': lambda f: f is None }})
-    r"""Required section to be configured for sync."""
+    r"""Required section to be configured for sync."""  
     selected_account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedAccountId'), 'exclude': lambda f: f is None }})
-    r"""Selected account id from the list of available accounts."""
-    
-
+    r"""Selected account id from the list of available accounts."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 from ..shared import sales as shared_sales
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Configuration:
     r"""Success"""
-    fees: Optional[shared_fees.Fees] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fees'), 'exclude': lambda f: f is None }})
-    new_payments: Optional[shared_newpayments.NewPayments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newPayments'), 'exclude': lambda f: f is None }})
-    payments: Optional[shared_payments.Payments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payments'), 'exclude': lambda f: f is None }})
-    sales: Optional[shared_sales.Sales] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sales'), 'exclude': lambda f: f is None }})
     
-
+    fees: Optional[shared_fees.Fees] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fees'), 'exclude': lambda f: f is None }})  
+    new_payments: Optional[shared_newpayments.NewPayments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newPayments'), 'exclude': lambda f: f is None }})  
+    payments: Optional[shared_payments.Payments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payments'), 'exclude': lambda f: f is None }})  
+    sales: Optional[shared_sales.Sales] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sales'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/connection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import dataconnectionerror as shared_dataconnectionerror
-from ..shared import dataconnectionstatus as shared_dataconnectionstatus
+from ..shared import dataconnectionstatus_enum as shared_dataconnectionstatus_enum
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Any, Optional
 
-class ConnectionSourceType(str, Enum):
+class ConnectionSourceTypeEnum(str, Enum):
     r"""The type of platform of the connection."""
     ACCOUNTING = 'Accounting'
     BANKING = 'Banking'
     COMMERCE = 'Commerce'
     OTHER = 'Other'
     UNKNOWN = 'Unknown'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Connection:
-    r"""A connection represents a [company's](https://docs.codat.io/codat-api#/schemas/Company) connection to a data source and allows you to synchronize data (pull and/or push) with that source.
-    
-    A company can have multiple data connections depending on the type of data source it is connecting to. For example, a single company can link to:
-    
-    - [Accounting data](https://docs.codat.io/accounting-api/overview) - 1 active connection.
-    - [Banking data](https://docs.codat.io/banking-api/overview) - Multiple active connections.
-    - [Commerce data](https://docs.codat.io/commerce-api/overview) - Multiple active connections.
-    Any combination of accounting, banking, and commerce data connections is allowed.
+    r"""A connection represents the link between a `company` and a source of data."""
     
-    Before you can use a data connection to pull or push data, the company must grant you access to their business data by [linking the connection](https://docs.codat.io/auth-flow/overview).
-    """
     created: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created') }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -49,32 +39,32 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """  
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique identifier for a company's data connection."""
+    r"""Unique identifier for a company's data connection."""  
     integration_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId') }})
-    r"""A Codat ID representing the integration."""
+    r"""A Codat ID representing the integration."""  
     integration_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationKey') }})
-    r"""A unique four-character ID that identifies the platform of the company's data connection. This ensures continuity if the platform changes its name in the future."""
-    link_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkUrl') }})
-    platform_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformName') }})
+    r"""A unique four-character ID that identifies the platform of the company's data connection. This ensures continuity if the platform changes its name in the future."""  
+    link_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkUrl') }})  
+    platform_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformName') }})  
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
-    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
-    source_type: ConnectionSourceType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-    r"""The type of platform of the connection."""
-    status: shared_dataconnectionstatus.DataConnectionStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    r"""The current authorization status of the data connection."""
-    additional_properties: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalProperties'), 'exclude': lambda f: f is None }})
-    connection_info: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionInfo'), 'exclude': lambda f: f is None }})
-    data_connection_errors: Optional[list[shared_dataconnectionerror.DataConnectionError]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionErrors'), 'exclude': lambda f: f is None }})
+    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""  
+    source_type: ConnectionSourceTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    r"""The type of platform of the connection."""  
+    status: shared_dataconnectionstatus_enum.DataConnectionStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    r"""The current authorization status of the data connection."""  
+    additional_properties: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalProperties'), 'exclude': lambda f: f is None }})  
+    connection_info: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionInfo'), 'exclude': lambda f: f is None }})  
+    data_connection_errors: Optional[list[shared_dataconnectionerror.DataConnectionError]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionErrors'), 'exclude': lambda f: f is None }})  
     last_sync: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSync'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -87,10 +77,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    
-
+    """  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/connections.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelinelevelselection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import connection as shared_connection
-from ..shared import links as shared_links
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Connections:
-    r"""Success"""
-    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-    results: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+class InvoiceLineLevelSelection:
     
-
+    group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupByOptions'), 'exclude': lambda f: f is None }})
+    r"""Options for grouping on invoice lines."""  
+    selected_group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupByOptions'), 'exclude': lambda f: f is None }})
+    r"""Invoice line level selection."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/createcompany.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/updateconnection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CreateCompany:
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    r"""Name of the company in Codat with a partner-commerce data connection."""
+class UpdateConnection:
     
-
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    r"""The current authorization status of the data connection."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/customer.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/customer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from ..shared import option as shared_option
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Customer:
+    
     customer_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerOptions'), 'exclude': lambda f: f is None }})
-    r"""List of customer options from the list of customer records on the accounting software."""
+    r"""List of customer options from the list of customer records on the accounting software."""  
     selected_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedCustomerId'), 'exclude': lambda f: f is None }})
-    r"""Selected customer id from the list of customer records on the accounting software."""
-    
-
+    r"""Selected customer id from the list of customer records on the accounting software."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/dataconnectionerror.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/dataconnectionerror.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class DataConnectionError:
+    
     errored_on_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('erroredOnUtc'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -27,13 +27,12 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-    status_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
-    status_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusText'), 'exclude': lambda f: f is None }})
-    
-
+    """  
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})  
+    status_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})  
+    status_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusText'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/datatypefeature.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/datatypefeature.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import dataclasses
 from ..shared import supportedfeature as shared_supportedfeature
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class DataTypeFeatureDataType(str, Enum):
+class DataTypeFeatureDataTypeEnum(str, Enum):
     r"""Available Data types"""
     ACCOUNT_TRANSACTIONS = 'accountTransactions'
     BALANCE_SHEET = 'balanceSheet'
     BANK_ACCOUNTS = 'bankAccounts'
     BANK_TRANSACTIONS = 'bankTransactions'
     BILL_CREDIT_NOTES = 'billCreditNotes'
     BILL_PAYMENTS = 'billPayments'
@@ -51,16 +51,15 @@
     COMMERCE_PRODUCT_CATEGORIES = 'commerce-productCategories'
     COMMERCE_PRODUCTS = 'commerce-products'
     COMMERCE_TAX_COMPONENTS = 'commerce-taxComponents'
     COMMERCE_TRANSACTIONS = 'commerce-transactions'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class DataTypeFeature:
     r"""Describes support for a given datatype and associated operations"""
-    supported_features: list[shared_supportedfeature.SupportedFeature] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supportedFeatures') }})
-    data_type: Optional[DataTypeFeatureDataType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-    r"""Available Data types"""
     
-
+    supported_features: list[shared_supportedfeature.SupportedFeature] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supportedFeatures') }})  
+    data_type: Optional[DataTypeFeatureDataTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
+    r"""Available Data types"""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/daterange.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/daterange.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class DateRange:
+    
     finish: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('finish'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -27,15 +27,15 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """  
     start: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -48,10 +48,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    
-
+    """  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/fees.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/fees.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from ..shared import feessupplier as shared_feessupplier
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Fees:
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-    fees_supplier: Optional[shared_feessupplier.FeesSupplier] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('feesSupplier'), 'exclude': lambda f: f is None }})
-    sync_fees: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncFees'), 'exclude': lambda f: f is None }})
-    r"""Boolean indicator to enable syncing fees."""
     
-
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
+    fees_supplier: Optional[shared_feessupplier.FeesSupplier] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('feesSupplier'), 'exclude': lambda f: f is None }})  
+    sync_fees: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncFees'), 'exclude': lambda f: f is None }})
+    r"""Boolean indicator to enable syncing fees."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/feessupplier.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/feessupplier.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from ..shared import option as shared_option
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class FeesSupplier:
+    
     selected_supplier_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedSupplierId'), 'exclude': lambda f: f is None }})
-    r"""Selected supplier id from the list of supplier records on the accounting software."""
+    r"""Selected supplier id from the list of supplier records on the accounting software."""  
     supplier_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplierOptions'), 'exclude': lambda f: f is None }})
-    r"""List of supplier options from the list of supplier records on the accounting software."""
-    
-
+    r"""List of supplier options from the list of supplier records on the accounting software."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/grouping.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/grouping.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,13 @@
 from ..shared import groupingperiod as shared_groupingperiod
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Grouping:
-    grouping_levels: Optional[shared_groupinglevels.GroupingLevels] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingLevels'), 'exclude': lambda f: f is None }})
-    grouping_period: Optional[shared_groupingperiod.GroupingPeriod] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingPeriod'), 'exclude': lambda f: f is None }})
     
-
+    grouping_levels: Optional[shared_groupinglevels.GroupingLevels] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingLevels'), 'exclude': lambda f: f is None }})  
+    grouping_period: Optional[shared_groupingperiod.GroupingPeriod] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingPeriod'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/groupinglevels.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupinglevels.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,13 @@
 from ..shared import invoicelinelevelselection as shared_invoicelinelevelselection
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GroupingLevels:
-    invoice_level: Optional[shared_invoicelevelselection.InvoiceLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLevel'), 'exclude': lambda f: f is None }})
-    invoice_line_level: Optional[shared_invoicelinelevelselection.InvoiceLineLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLineLevel'), 'exclude': lambda f: f is None }})
     
-
+    invoice_level: Optional[shared_invoicelevelselection.InvoiceLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLevel'), 'exclude': lambda f: f is None }})  
+    invoice_line_level: Optional[shared_invoicelinelevelselection.InvoiceLineLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLineLevel'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/groupingperiod.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupingperiod.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GroupingPeriod:
+    
     grouping_period_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingPeriodOptions'), 'exclude': lambda f: f is None }})
-    r"""Array of grouping period options."""
+    r"""Array of grouping period options."""  
     selected_grouping_period: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupingPeriod'), 'exclude': lambda f: f is None }})
-    r"""Grouping period i.e. Daily sales."""
-    
-
+    r"""Grouping period i.e. Daily sales."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/imagereference.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/imagereference.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ImageReference:
     r"""Image reference."""
+    
     alt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alt'), 'exclude': lambda f: f is None }})
-    r"""Alternative text when image is not available."""
+    r"""Alternative text when image is not available."""  
     src: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('src'), 'exclude': lambda f: f is None }})
-    r"""Source URL for image."""
-    
-
+    r"""Source URL for image."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/integration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import datatypefeature as shared_datatypefeature
-from ..shared import sourcetype as shared_sourcetype
+from ..shared import sourcetype_enum as shared_sourcetype_enum
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Integration:
     r"""An integration that Codat supports"""
+    
     enabled: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('enabled') }})
-    r"""Whether this integration is enabled for your customers to use"""
+    r"""Whether this integration is enabled for your customers to use"""  
     key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
-    r"""A unique 4-letter key to represent a platform in each integration. View [accounting](https://docs.codat.io/integrations/accounting/accounting-platform-keys), [banking](https://docs.codat.io/integrations/banking/banking-platform-keys), and [commerce](https://docs.codat.io/integrations/commerce/commerce-platform-keys) platform keys."""
-    logo_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logoUrl') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    data_provided_by: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataProvidedBy'), 'exclude': lambda f: f is None }})
-    datatype_features: Optional[list[shared_datatypefeature.DataTypeFeature]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datatypeFeatures'), 'exclude': lambda f: f is None }})
+    r"""A unique 4-letter key to represent a platform in each integration. View [accounting](https://docs.codat.io/integrations/accounting/accounting-platform-keys), [banking](https://docs.codat.io/integrations/banking/banking-platform-keys), and [commerce](https://docs.codat.io/integrations/commerce/commerce-platform-keys) platform keys."""  
+    logo_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logoUrl') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    data_provided_by: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataProvidedBy'), 'exclude': lambda f: f is None }})  
+    datatype_features: Optional[list[shared_datatypefeature.DataTypeFeature]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datatypeFeatures'), 'exclude': lambda f: f is None }})  
     integration_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
-    r"""A Codat ID representing the integration."""
-    is_beta: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBeta'), 'exclude': lambda f: f is None }})
-    is_offline_connector: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isOfflineConnector'), 'exclude': lambda f: f is None }})
+    r"""A Codat ID representing the integration."""  
+    is_beta: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBeta'), 'exclude': lambda f: f is None }})  
+    is_offline_connector: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isOfflineConnector'), 'exclude': lambda f: f is None }})  
     source_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId'), 'exclude': lambda f: f is None }})
-    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
-    source_type: Optional[shared_sourcetype.SourceType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType'), 'exclude': lambda f: f is None }})
-    r"""The type of platform of the connection."""
-    
-
+    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""  
+    source_type: Optional[shared_sourcetype_enum.SourceTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType'), 'exclude': lambda f: f is None }})
+    r"""The type of platform of the connection."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/integrations.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/links.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import integration as shared_integration
-from ..shared import links as shared_links
+from ..shared import halref as shared_halref
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Integrations:
-    r"""Success"""
-    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-    results: Optional[list[shared_integration.Integration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+class Links:
     
-
+    current: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})  
+    self_: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})  
+    next: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})  
+    previous: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/invoicelevelselection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelevelselection.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class InvoiceLevelSelection:
+    
     group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupByOptions'), 'exclude': lambda f: f is None }})
-    r"""Options for grouping sales."""
+    r"""Options for grouping sales."""  
     selected_group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupByOptions'), 'exclude': lambda f: f is None }})
-    r"""Selected array of grouping options."""
-    
-
+    r"""Selected array of grouping options."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/invoicelinelevelselection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/localization.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class InvoiceLineLevelSelection:
-    group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupByOptions'), 'exclude': lambda f: f is None }})
-    r"""Options for grouping on invoice lines."""
-    selected_group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupByOptions'), 'exclude': lambda f: f is None }})
-    r"""Invoice line level selection."""
+class Localization:
     
-
+    required: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required'), 'exclude': lambda f: f is None }})  
+    text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text'), 'exclude': lambda f: f is None }})
+    r"""Value of the property."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/invoicestatus.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicestatus.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class InvoiceStatus:
+    
     invoice_status_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceStatusOptions'), 'exclude': lambda f: f is None }})
-    r"""Options for invoice statuses."""
+    r"""Options for invoice statuses."""  
     selected_invoice_status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedInvoiceStatus'), 'exclude': lambda f: f is None }})
-    r"""Selected option for invoice status for invoice to be synced."""
-    
-
+    r"""Selected option for invoice status for invoice to be synced."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/links.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newpayments.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import halref as shared_halref
+from ..shared import configaccount as shared_configaccount
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Links:
-    current: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})
-    self_: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})
-    next: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+class NewPayments:
     
-
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
+    sync_payments: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncPayments'), 'exclude': lambda f: f is None }})
+    r"""Boolean indicator for syncing payments."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/localization.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxrateamount.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import option as shared_option
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Localization:
-    required: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required'), 'exclude': lambda f: f is None }})
-    text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text'), 'exclude': lambda f: f is None }})
-    r"""Value of the property."""
+class TaxRateAmount:
     
-
+    selected_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedTaxRateId'), 'exclude': lambda f: f is None }})
+    r"""Selected tax rate id from the list of tax rates on the accounting software."""  
+    tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateOptions'), 'exclude': lambda f: f is None }})
+    r"""Array of tax rate options object."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/newpayments.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/payments.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from ..shared import configaccount as shared_configaccount
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class NewPayments:
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-    sync_payments: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncPayments'), 'exclude': lambda f: f is None }})
-    r"""Boolean indicator for syncing payments."""
+class Payments:
     
-
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
+    sync_payments: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncPayments'), 'exclude': lambda f: f is None }})
+    r"""Boolean indicator for syncing sales."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/newtaxrates.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newtaxrates.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,21 @@
 from ..shared import taxratemapping as shared_taxratemapping
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class NewTaxRates:
+    
     accounting_tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountingTaxRateOptions'), 'exclude': lambda f: f is None }})
-    r"""Array of accounting tax rate options."""
+    r"""Array of accounting tax rate options."""  
     commerce_tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commerceTaxRateOptions'), 'exclude': lambda f: f is None }})
-    r"""Array of tax component options."""
+    r"""Array of tax component options."""  
     default_zero_tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('defaultZeroTaxRateOptions'), 'exclude': lambda f: f is None }})
-    r"""Default zero tax rate selected for sync."""
+    r"""Default zero tax rate selected for sync."""  
     selected_default_zero_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedDefaultZeroTaxRateId'), 'exclude': lambda f: f is None }})
-    r"""Default tax rate selected for sync."""
+    r"""Default tax rate selected for sync."""  
     tax_rate_mappings: Optional[list[shared_taxratemapping.TaxRateMapping]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateMappings'), 'exclude': lambda f: f is None }})
-    r"""Array of tax component to rate mapppings."""
-    
-
+    r"""Array of tax component to rate mapppings."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/option.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/option.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Option:
+    
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the option."""
+    r"""Unique identifier for the option."""  
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    r"""Name value of the option."""
-    
-
+    r"""Name value of the option."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/sales.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/sales.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 from ..shared import taxrateamount as shared_taxrateamount
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Sales:
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-    grouping: Optional[shared_grouping.Grouping] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping'), 'exclude': lambda f: f is None }})
-    invoice_status: Optional[shared_invoicestatus.InvoiceStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceStatus'), 'exclude': lambda f: f is None }})
-    new_tax_rates: Optional[shared_newtaxrates.NewTaxRates] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newTaxRates'), 'exclude': lambda f: f is None }})
-    sales_customer: Optional[shared_customer.Customer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('salesCustomer'), 'exclude': lambda f: f is None }})
-    sync_sales: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncSales'), 'exclude': lambda f: f is None }})
-    r"""Boolean indicator for syncing sales."""
-    tax_rates: Optional[dict[str, shared_taxrateamount.TaxRateAmount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRates'), 'exclude': lambda f: f is None }})
     
-
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
+    grouping: Optional[shared_grouping.Grouping] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping'), 'exclude': lambda f: f is None }})  
+    invoice_status: Optional[shared_invoicestatus.InvoiceStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceStatus'), 'exclude': lambda f: f is None }})  
+    new_tax_rates: Optional[shared_newtaxrates.NewTaxRates] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newTaxRates'), 'exclude': lambda f: f is None }})  
+    sales_customer: Optional[shared_customer.Customer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('salesCustomer'), 'exclude': lambda f: f is None }})  
+    sync_sales: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncSales'), 'exclude': lambda f: f is None }})
+    r"""Boolean indicator for syncing sales."""  
+    tax_rates: Optional[dict[str, shared_taxrateamount.TaxRateAmount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRates'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/supportedfeature.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/supportedfeature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import featurestate as shared_featurestate
-from ..shared import featuretype as shared_featuretype
+from ..shared import featurestate_enum as shared_featurestate_enum
+from ..shared import featuretype_enum as shared_featuretype_enum
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SupportedFeature:
-    feature_state: shared_featurestate.FeatureState = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureState') }})
-    feature_type: shared_featuretype.FeatureType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureType') }})
     
-
+    feature_state: shared_featurestate_enum.FeatureStateEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureState') }})  
+    feature_type: shared_featuretype_enum.FeatureTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureType') }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/syncflowurl.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncflowurl.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SyncFlowURL:
     r"""Success"""
-    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
-    r"""Sync flow URL."""
     
-
+    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
+    r"""Sync flow URL."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/syncrange.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/synctolatestargs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SyncRangeDateRange:
-    finish: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('finish') }})
-    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
-    
-    ```
-    2020-10-08T22:40:50Z
-    2021-01-01T00:00:00
-    ```
-    
-    
-    
-    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
-    
-    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
-    - Unqualified local time: `2021-11-15T01:00:00`
-    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+class SyncToLatestArgs:
     
-    > Time zones
-    > 
-    > Not all dates from Codat will contain information about time zones.  
-    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    start: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start') }})
+    sync_to: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncTo'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -47,19 +27,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
-@dataclasses.dataclass
-class SyncRange:
-    date_range: SyncRangeDateRange = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dateRange') }})
-    
-
+    """  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/syncsummary.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncsummary.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,35 +6,35 @@
 from ..shared import daterange as shared_daterange
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SyncSummary:
     r"""Success"""
+    
     commerce_sync_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commerceSyncId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the sync in Codat."""
+    r"""Unique identifier for the sync in Codat."""  
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for your SMB in Codat."""
+    r"""Unique identifier for your SMB in Codat."""  
     data_connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnections'), 'exclude': lambda f: f is None }})
-    r"""Array of containing objects data connection information for the company."""
+    r"""Array of containing objects data connection information for the company."""  
     data_pushed: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataPushed'), 'exclude': lambda f: f is None }})
-    r"""Boolean indicator for data being pushed during a sync operation."""
+    r"""Boolean indicator for data being pushed during a sync operation."""  
     error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-    r"""Friendly error message for the sync operation."""
-    sync_date_range_utc: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncDateRangeUtc'), 'exclude': lambda f: f is None }})
+    r"""Friendly error message for the sync operation."""  
+    sync_date_range_utc: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncDateRangeUtc'), 'exclude': lambda f: f is None }})  
     sync_exception_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncExceptionMessage'), 'exclude': lambda f: f is None }})
-    r"""Exception message for the sync operation."""
+    r"""Exception message for the sync operation."""  
     sync_status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncStatus'), 'exclude': lambda f: f is None }})
-    r"""Status of the sync of the company data. This is linked to status code."""
+    r"""Status of the sync of the company data. This is linked to status code."""  
     sync_status_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncStatusCode'), 'exclude': lambda f: f is None }})
-    r"""Numerical status code sync of the company data."""
+    r"""Numerical status code sync of the company data."""  
     sync_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncUtc'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -47,10 +47,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    
-
+    """  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/taxrateamount.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connections.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import option as shared_option
+from ..shared import connection as shared_connection
+from ..shared import links as shared_links
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class TaxRateAmount:
-    selected_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedTaxRateId'), 'exclude': lambda f: f is None }})
-    r"""Selected tax rate id from the list of tax rates on the accounting software."""
-    tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateOptions'), 'exclude': lambda f: f is None }})
-    r"""Array of tax rate options object."""
+class Connections:
+    r"""Success"""
     
-
+    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
+    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
+    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
+    results: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/taxratemapping.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxratemapping.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TaxRateMapping:
+    
     selected_accounting_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedAccountingTaxRateId'), 'exclude': lambda f: f is None }})
-    r"""Selected tax rate id from the list of tax rates on the accounting software."""
+    r"""Selected tax rate id from the list of tax rates on the accounting software."""  
     selected_commerce_tax_rate_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedCommerceTaxRateIds'), 'exclude': lambda f: f is None }})
-    r"""Selected tax component id from the list of tax components on the commerce software."""
-    
-
+    r"""Selected tax component id from the list of tax components on the commerce software."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/models/shared/visibleaccounts.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/visibleaccounts.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import dataclasses
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class VisibleAccounts:
     r"""Success"""
-    visible_accounts: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('visibleAccounts'), 'exclude': lambda f: f is None }})
-    r"""Visible accounts on sync flow."""
     
-
+    visible_accounts: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('visibleAccounts'), 'exclude': lambda f: f is None }})
+    r"""Visible accounts on sync flow."""  
+
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/sync_flow_preferences.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync_flow_preferences.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from codatsynccommerce import utils
+import requests as requests_http
+from . import utils
 from codatsynccommerce.models import operations, shared
 from typing import Optional
 
 class SyncFlowPreferences:
     r"""Configure preferences for any given Sync for Commerce company using sync flow."""
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
     def get_config_text_sync_flow(self, retries: Optional[utils.RetryConfig] = None) -> operations.GetConfigTextSyncFlowResponse:
         r"""Retrieve preferences for text fields on Sync Flow
         To enable retrieval of preferences set for the text fields on Sync Flow.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/sync/commerce/config/ui/text'
         
-        url = base_url + '/sync/commerce/config/ui/text'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
-            return client.request('GET', url, headers=headers)
+            return client.request('GET', url)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
@@ -45,35 +54,34 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[dict[str, shared.Localization]])
                 res.localization_info = out
 
         return res
 
-    
     def get_sync_flow_url(self, request: operations.GetSyncFlowURLRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncFlowURLResponse:
         r"""Retrieve sync flow url
         Get a URL for Sync Flow including a one time passcode.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncFlowURLRequest, base_url, '/config/sync/commerce/{commerceKey}/{accountingKey}/start', request)
-        headers = {}
+        
         query_params = utils.get_query_params(operations.GetSyncFlowURLRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
-            return client.request('GET', url, params=query_params, headers=headers)
+            return client.request('GET', url, params=query_params)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
@@ -83,34 +91,33 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.SyncFlowURL])
                 res.sync_flow_url = out
 
         return res
 
-    
     def get_visible_accounts(self, request: operations.GetVisibleAccountsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetVisibleAccountsResponse:
         r"""List visible accounts
         Enable retrieval for accounts which are visible on sync flow.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetVisibleAccountsRequest, base_url, '/clients/{clientId}/config/ui/accounts/platform/{platformKey}', request)
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
-            return client.request('GET', url, headers=headers)
+            return client.request('GET', url)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
@@ -120,34 +127,34 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.VisibleAccounts])
                 res.visible_accounts = out
 
         return res
 
-    
     def update_config_text_sync_flow(self, request: dict[str, shared.Localization], retries: Optional[utils.RetryConfig] = None) -> operations.UpdateConfigTextSyncFlowResponse:
         r"""Update preferences for text fields on sync flow
         To enable update of preferences set for the text fields on sync flow.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/sync/commerce/config/ui/text'
         
-        url = base_url + '/sync/commerce/config/ui/text'
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
             return client.request('PATCH', url, data=data, files=form, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
@@ -160,34 +167,34 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[dict[str, shared.Localization]])
                 res.localization_info = out
 
         return res
 
-    
     def update_visible_accounts_sync_flow(self, request: operations.UpdateVisibleAccountsSyncFlowRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateVisibleAccountsSyncFlowResponse:
         r"""Update the visible accounts on Sync Flow
         To enable update of accounts visible preferences set on Sync Flow.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateVisibleAccountsSyncFlowRequest, base_url, '/sync/commerce/config/ui/accounts/platform/{commerceKey}', request)
+        
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "visible_accounts", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
         def do_request():
             return client.request('PATCH', url, data=data, files=form, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/utils/retries.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/retries.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 
 
 class RetryConfig:
     strategy: str
     backoff: BackoffStrategy
     retry_connection_errors: bool
 
-    def __init__(self, strategy: str, backoff: BackoffStrategy, retry_connection_errors: bool):
+    def __init__(self, strategy: str, retry_connection_errors: bool):
         self.strategy = strategy
-        self.backoff = backoff
         self.retry_connection_errors = retry_connection_errors
 
 
 class Retries:
     config: RetryConfig
     status_codes: list[str]
```

### Comparing `codat-sync-for-commerce-0.30.1/src/codatsynccommerce/utils/utils.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             raise Exception('not supported')
     elif scheme_type == "openIdConnect":
         client.client.headers[header_name] = value
     elif scheme_type == 'oauth2':
         client.client.headers[header_name] = value
     elif scheme_type == 'http':
         if sub_type == 'bearer':
-            client.client.headers[header_name] = value.lower().startswith('bearer ') and value or f'Bearer {value}'
+            client.client.headers[header_name] = value
         else:
             raise Exception('not supported')
     else:
         raise Exception('not supported')
 
 
 def _parse_basic_auth_scheme(client: SecurityClient, scheme: dataclass):
@@ -137,16 +137,15 @@
         if field_name == 'password':
             password = value
 
     data = f'{username}:{password}'.encode()
     client.client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass,
-                 gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
+def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
     path_param_fields: Tuple[Field, ...] = fields(clazz)
     for field in path_param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
@@ -230,16 +229,15 @@
     for key, value in params.items():
         url_with_params = url_with_params.replace(
             '{' + key + '}', value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[
-    str, list[str]]:
+def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     param_fields: Tuple[Field, ...] = fields(clazz)
     for field in param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
@@ -265,19 +263,16 @@
                     params[key] = [value]
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
-                params = params | _get_delimited_query_params(
-                    metadata, f_name, value, ",")
-            elif style == 'pipeDelimited':
-                params = params | _get_delimited_query_params(
-                    metadata, f_name, value, "|")
+                params = params | _get_form_query_params(
+                    metadata, f_name, value)
             else:
                 raise Exception('not yet implemented')
     return params
 
 
 def get_headers(headers_params: dataclass) -> dict[str, str]:
     if headers_params is None:
@@ -328,23 +323,20 @@
                 continue
 
             if isinstance(obj_val, list):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
-                        params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
+                    if params.get(f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                        params[f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                         ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(_val_to_string(val))
             else:
                 params[
                     f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                     _val_to_string(obj_val)]
     elif isinstance(obj, dict):
         for key, value in obj.items():
             if value is None:
@@ -372,52 +364,48 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: dict, field_name: str, obj: any, delimiter: str) -> dict[
-    str, list[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
+def _get_form_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
+    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name)
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
+    'json':      'application/json',
+    'form':      'application/x-www-form-urlencoded',
     'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    'raw':       'application/octet-stream',
+    'string':    'text/plain',
 }
 
 
-def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[
-    str, any, any]:
+def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[str, any, any]:
     if request is None:
         return None, None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request)
+        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method], request)
 
     request_val = getattr(request, request_field_name)
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
             request_metadata = field.metadata.get('request')
             break
 
     if request_metadata is None:
         raise Exception('invalid request type')
 
-    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'), request_val)
 
 
 def serialize_content_type(field_name: str, media_type: str, request: dataclass) -> Tuple[str, any, list[list[any]]]:
     if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
         return media_type, marshal_json(request), None
     if re.match(r'multipart\/.*', media_type) is not None:
         return serialize_multipart_form(media_type, request)
@@ -482,15 +470,15 @@
                         [field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
 def serialize_dict(original: dict, explode: bool, field_name, existing: Optional[dict[str, list[str]]]) -> dict[
-    str, list[str]]:
+        str, list[str]]:
     if existing is None:
         existing = []
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -522,15 +510,15 @@
             field_name = metadata.get('field_name', field.name)
 
             if metadata.get('json'):
                 form[field_name] = [marshal_json(val)]
             else:
                 if metadata.get('style', 'form') == 'form':
                     form = form | _populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")
+                        field_name, metadata.get('explode', True), val, _get_form_field_name)
                 else:
                     raise Exception(
                         f'Invalid form style for field {field.name}')
     elif isinstance(data, dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
@@ -544,16 +532,15 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, delimiter: str) -> \
-        dict[str, list[str]]:
+def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable) -> dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     if obj is None:
         return params
 
     if is_dataclass(obj):
         items = []
@@ -568,31 +555,31 @@
             if val is None:
                 continue
 
             if explode:
                 params[obj_field_name] = [_val_to_string(val)]
             else:
                 items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                    f'{obj_field_name},{_val_to_string(val)}')
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            params[field_name] = [','.join(items)]
     elif isinstance(obj, dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
                 params[key] = _val_to_string(value)
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f'{key},{_val_to_string(value)}')
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            params[field_name] = [','.join(items)]
     elif isinstance(obj, list):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
@@ -600,15 +587,15 @@
                 if not field_name in params:
                     params[field_name] = []
                 params[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join([str(item) for item in items])]
+            params[field_name] = [','.join([str(item) for item in items])]
     else:
         params[field_name] = [_val_to_string(obj)]
 
     return params
 
 
 def _serialize_header(explode: bool, obj: any) -> str:
@@ -740,15 +727,15 @@
 
 def _val_to_string(val):
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
         return val.isoformat().replace('+00:00', 'Z')
     if isinstance(val, Enum):
-        return str(val.value)
+        return val.value
 
     return str(val)
 
 
 def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: dict[str, dict[str, dict[str, Any]]]):
     if value is None and gbls is not None:
         if 'parameters' in gbls:
```

