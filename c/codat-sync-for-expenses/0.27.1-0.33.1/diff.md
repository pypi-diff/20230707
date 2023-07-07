# Comparing `tmp/codat-sync-for-expenses-0.27.1.tar.gz` & `tmp/codat-sync-for-expenses-0.33.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-0.27.1.tar", last modified: Fri Jun 16 11:14:27 2023, max compression
+gzip compressed data, was "codat-sync-for-expenses-0.33.1.tar", last modified: Fri Jul  7 09:29:17 2023, max compression
```

## Comparing `codat-sync-for-expenses-0.27.1.tar` & `codat-sync-for-expenses-0.33.1.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.990173 codat-sync-for-expenses-0.27.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-16 11:14:27.990173 codat-sync-for-expenses-0.27.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:14:27.990173 codat-sync-for-expenses-0.27.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.982173 codat-sync-for-expenses-0.27.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.982173 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-16 11:14:27.000000 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-16 11:14:27.000000 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:14:27.000000 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-16 11:14:27.000000 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 11:14:27.000000 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.986173 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4840 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5131 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/expenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/mapping_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.986173 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.986173 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1158 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/intiate_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/list_syncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/upload_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.990173 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1817 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/bankaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3073 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      590 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5366 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/dataconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4833 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/expensetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/hallink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/integrationtype.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/mappingoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/postsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      573 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/recordref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1503 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/syncinitiated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2411 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2014 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/transactionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3511 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sdkconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8477 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4724 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.990173 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:17.409758 codat-sync-for-expenses-0.33.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-07 09:29:17.409758 codat-sync-for-expenses-0.33.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:29:17.413758 codat-sync-for-expenses-0.33.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:17.401758 codat-sync-for-expenses-0.33.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:17.405758 codat-sync-for-expenses-0.33.1/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-07 09:29:17.000000 codat-sync-for-expenses-0.33.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-07 09:29:17.000000 codat-sync-for-expenses-0.33.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:29:17.000000 codat-sync-for-expenses-0.33.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-07 09:29:17.000000 codat-sync-for-expenses-0.33.1/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 09:29:17.000000 codat-sync-for-expenses-0.33.1/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:17.405758 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4840 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7511 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/expenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/mapping_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:17.405758 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:17.405758 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1158 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/intiate_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/list_syncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1819 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/update_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/upload_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:17.409758 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1876 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3073 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      590 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6214 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/dataconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5099 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/hallink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/integrationtype.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/postsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      573 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1503 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2411 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2014 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/transactionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/updateexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3511 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/sdkconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8477 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4724 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:29:17.409758 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-07 09:29:05.000000 codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.27.1/PKG-INFO` & `codat-sync-for-expenses-0.33.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.27.1
+Version: 0.33.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -57,14 +57,15 @@
 ### [connections](docs/sdks/connections/README.md)
 
 * [create_partner_expense_connection](docs/sdks/connections/README.md#create_partner_expense_connection) - Create Partner Expense connection
 
 ### [expenses](docs/sdks/expenses/README.md)
 
 * [create_expense_dataset](docs/sdks/expenses/README.md#create_expense_dataset) - Create expense-transactions
+* [update_expense_dataset](docs/sdks/expenses/README.md#update_expense_dataset) - Update expense-transactions
 * [upload_attachment](docs/sdks/expenses/README.md#upload_attachment) - Upload attachment
 
 ### [mapping_options](docs/sdks/mappingoptions/README.md)
 
 * [get_mapping_options](docs/sdks/mappingoptions/README.md#get_mapping_options) - Mapping options
 
 ### [sync](docs/sdks/sync/README.md)
```

### Comparing `codat-sync-for-expenses-0.27.1/README.md` & `codat-sync-for-expenses-0.33.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 ### [connections](docs/sdks/connections/README.md)
 
 * [create_partner_expense_connection](docs/sdks/connections/README.md#create_partner_expense_connection) - Create Partner Expense connection
 
 ### [expenses](docs/sdks/expenses/README.md)
 
 * [create_expense_dataset](docs/sdks/expenses/README.md#create_expense_dataset) - Create expense-transactions
+* [update_expense_dataset](docs/sdks/expenses/README.md#update_expense_dataset) - Update expense-transactions
 * [upload_attachment](docs/sdks/expenses/README.md#upload_attachment) - Upload attachment
 
 ### [mapping_options](docs/sdks/mappingoptions/README.md)
 
 * [get_mapping_options](docs/sdks/mappingoptions/README.md#get_mapping_options) - Mapping options
 
 ### [sync](docs/sdks/sync/README.md)
```

### Comparing `codat-sync-for-expenses-0.27.1/setup.py` & `codat-sync-for-expenses-0.33.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-expenses",
-    version="0.27.1",
+    version="0.33.1",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
```

### Comparing `codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/PKG-INFO` & `codat-sync-for-expenses-0.33.1/src/codat_sync_for_expenses.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.27.1
+Version: 0.33.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -57,14 +57,15 @@
 ### [connections](docs/sdks/connections/README.md)
 
 * [create_partner_expense_connection](docs/sdks/connections/README.md#create_partner_expense_connection) - Create Partner Expense connection
 
 ### [expenses](docs/sdks/expenses/README.md)
 
 * [create_expense_dataset](docs/sdks/expenses/README.md#create_expense_dataset) - Create expense-transactions
+* [update_expense_dataset](docs/sdks/expenses/README.md#update_expense_dataset) - Update expense-transactions
 * [upload_attachment](docs/sdks/expenses/README.md#upload_attachment) - Upload attachment
 
 ### [mapping_options](docs/sdks/mappingoptions/README.md)
 
 * [get_mapping_options](docs/sdks/mappingoptions/README.md#get_mapping_options) - Mapping options
 
 ### [sync](docs/sdks/sync/README.md)
```

### Comparing `codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-0.33.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/codatsyncexpenses/models/operations/get_mapping_options.py
 src/codatsyncexpenses/models/operations/get_sync_by_id.py
 src/codatsyncexpenses/models/operations/get_sync_transaction.py
 src/codatsyncexpenses/models/operations/intiate_sync.py
 src/codatsyncexpenses/models/operations/list_sync_transactions.py
 src/codatsyncexpenses/models/operations/list_syncs.py
 src/codatsyncexpenses/models/operations/save_company_configuration.py
+src/codatsyncexpenses/models/operations/update_expense_dataset.py
 src/codatsyncexpenses/models/operations/upload_attachment.py
 src/codatsyncexpenses/models/shared/__init__.py
 src/codatsyncexpenses/models/shared/accountmappinginfo.py
 src/codatsyncexpenses/models/shared/attachment.py
 src/codatsyncexpenses/models/shared/bankaccount.py
 src/codatsyncexpenses/models/shared/codaterrormessage.py
 src/codatsyncexpenses/models/shared/companyconfiguration.py
@@ -55,10 +56,11 @@
 src/codatsyncexpenses/models/shared/supplier.py
 src/codatsyncexpenses/models/shared/syncinitiated.py
 src/codatsyncexpenses/models/shared/taxratemappinginfo.py
 src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
 src/codatsyncexpenses/models/shared/transactionmetadata.py
 src/codatsyncexpenses/models/shared/transactionmetadatalist.py
 src/codatsyncexpenses/models/shared/transactionstatus.py
+src/codatsyncexpenses/models/shared/updateexpenserequest.py
 src/codatsyncexpenses/utils/__init__.py
 src/codatsyncexpenses/utils/retries.py
 src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/connections.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/transaction_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,98 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
 from codatsyncexpenses.models import operations, shared
 from typing import Optional
 
-class Expenses:
-    r"""Create expense datasets and upload receipts."""
+class TransactionStatus:
+    r"""Retrieve the status of transactions within a sync."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
-    def create_expense_dataset(self, request: operations.CreateExpenseDatasetRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateExpenseDatasetResponse:
-        r"""Create expense-transactions
-        Create an expense transaction
+    def get_sync_transaction(self, request: operations.GetSyncTransactionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncTransactionResponse:
+        r"""Get Sync Transaction
+        Gets the status of a transaction for a sync
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateExpenseDatasetRequest, base_url, '/companies/{companyId}/sync/expenses/data/expense-transactions', request)
+        url = utils.generate_url(operations.GetSyncTransactionRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}', request)
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "create_expense_request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
-            return client.request('POST', url, data=data, files=form, headers=headers)
+            return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.CreateExpenseDatasetResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetSyncTransactionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateExpenseResponse])
-                res.create_expense_response = out
-        elif http_res.status_code in [400, 401, 404, 429]:
+                out = utils.unmarshal_json(http_res.text, Optional[list[shared.TransactionMetadata]])
+                res.transaction_metadata = out
+        elif http_res.status_code in [401, 404, 429]:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
                 res.schema = out
 
         return res
 
     
-    def upload_attachment(self, request: operations.UploadAttachmentRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UploadAttachmentResponse:
-        r"""Upload attachment
-        Creates an attachment in the accounting software against the given transactionId
+    def list_sync_transactions(self, request: operations.ListSyncTransactionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncTransactionsResponse:
+        r"""Get Sync transactions
+        Get's the transactions and status for a sync
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UploadAttachmentRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}/attachments', request)
+        url = utils.generate_url(operations.ListSyncTransactionsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions', request)
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
+        query_params = utils.get_query_params(operations.ListSyncTransactionsRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
-            return client.request('POST', url, data=data, files=form, headers=headers)
+            return client.request('GET', url, params=query_params, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.UploadAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListSyncTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Attachment])
-                res.attachment = out
-        elif http_res.status_code in [400, 401, 404, 429]:
+                out = utils.unmarshal_json(http_res.text, Optional[shared.TransactionMetadataList])
+                res.transaction_metadata_list = out
+        elif http_res.status_code in [401, 404, 429]:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
                 res.schema = out
 
         return res
```

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/mapping_options.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/mapping_options.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,10 +8,11 @@
 from .get_mapping_options import *
 from .get_sync_by_id import *
 from .get_sync_transaction import *
 from .intiate_sync import *
 from .list_sync_transactions import *
 from .list_syncs import *
 from .save_company_configuration import *
+from .update_expense_dataset import *
 from .upload_attachment import *
 
-__all__ = ["CreateExpenseDatasetRequest","CreateExpenseDatasetResponse","CreatePartnerExpenseConnectionRequest","CreatePartnerExpenseConnectionResponse","GetCompanyConfigurationRequest","GetCompanyConfigurationResponse","GetLastSuccessfulSyncRequest","GetLastSuccessfulSyncResponse","GetLatestSyncRequest","GetLatestSyncResponse","GetMappingOptionsRequest","GetMappingOptionsResponse","GetSyncByIDRequest","GetSyncByIDResponse","GetSyncTransactionRequest","GetSyncTransactionResponse","IntiateSyncRequest","IntiateSyncResponse","ListSyncTransactionsRequest","ListSyncTransactionsResponse","ListSyncsRequest","ListSyncsResponse","SaveCompanyConfigurationRequest","SaveCompanyConfigurationResponse","UploadAttachmentRequest","UploadAttachmentRequestBody","UploadAttachmentResponse"]
+__all__ = ["CreateExpenseDatasetRequest","CreateExpenseDatasetResponse","CreatePartnerExpenseConnectionRequest","CreatePartnerExpenseConnectionResponse","GetCompanyConfigurationRequest","GetCompanyConfigurationResponse","GetLastSuccessfulSyncRequest","GetLastSuccessfulSyncResponse","GetLatestSyncRequest","GetLatestSyncResponse","GetMappingOptionsRequest","GetMappingOptionsResponse","GetSyncByIDRequest","GetSyncByIDResponse","GetSyncTransactionRequest","GetSyncTransactionResponse","IntiateSyncRequest","IntiateSyncResponse","ListSyncTransactionsRequest","ListSyncTransactionsResponse","ListSyncsRequest","ListSyncsResponse","SaveCompanyConfigurationRequest","SaveCompanyConfigurationResponse","UpdateExpenseDataset202ApplicationJSON","UpdateExpenseDatasetRequest","UpdateExpenseDatasetResponse","UploadAttachmentRequest","UploadAttachmentRequestBody","UploadAttachmentResponse"]
```

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_mapping_options.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_mapping_options.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/intiate_sync.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/intiate_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/save_company_configuration.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/save_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/upload_attachment.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/operations/upload_attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 from .supplier import *
 from .syncinitiated import *
 from .taxratemappinginfo import *
 from .trackingcategorymappinginfo import *
 from .transactionmetadata import *
 from .transactionmetadatalist import *
 from .transactionstatus import *
+from .updateexpenserequest import *
 
-__all__ = ["AccountMappingInfo","AccountMappingInfoAccountType","AccountMappingInfoValidTransactionTypes","Attachment","BankAccount","CodatErrorMessage","CodatErrorMessageValidation","CodatErrorMessageValidationErrors","CodatErrorMessageValidationInternals","CodatErrorMessageValidationWarnings","CompanyConfiguration","CompanySyncStatus","CreateExpenseRequest","CreateExpenseResponse","Customer","DataConnection","DataConnectionError","DataConnectionSourceType","DataConnectionStatus","ExpenseTransaction","ExpenseTransactionLine","ExpenseTransactionType","HalLink","IntegrationType","MappingOptions","PostSync","RecordRef","Schema","Security","Supplier","SyncInitiated","TaxRateMappingInfo","TaxRateMappingInfoValidTransactionTypes","TrackingCategoryMappingInfo","TransactionMetadata","TransactionMetadataList","TransactionMetadataListLinks","TransactionStatus"]
+__all__ = ["AccountMappingInfo","AccountMappingInfoAccountType","AccountMappingInfoValidTransactionTypes","Attachment","BankAccount","CodatErrorMessage","CodatErrorMessageValidation","CodatErrorMessageValidationErrors","CodatErrorMessageValidationInternals","CodatErrorMessageValidationWarnings","CompanyConfiguration","CompanySyncStatus","CreateExpenseRequest","CreateExpenseResponse","Customer","DataConnection","DataConnectionError","DataConnectionSourceType","DataConnectionStatus","ExpenseTransaction","ExpenseTransactionLine","ExpenseTransactionType","HalLink","IntegrationType","MappingOptions","PostSync","RecordRef","Schema","Security","Supplier","SyncInitiated","TaxRateMappingInfo","TaxRateMappingInfoValidTransactionTypes","TrackingCategoryMappingInfo","TransactionMetadata","TransactionMetadataList","TransactionMetadataListLinks","TransactionStatus","UpdateExpenseRequest"]
```

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/codaterrormessage.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/codaterrormessage.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/companyconfiguration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/dataconnection.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/dataconnection.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,25 @@
     UNKNOWN = 'Unknown'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 
 @dataclasses.dataclass
 class DataConnection:
-    r"""A connection represents the link between a `company` and a source of data."""
+    r"""A connection represents a [company's](https://docs.codat.io/codat-api#/schemas/Company) connection to a data source and allows you to synchronize data (pull and/or push) with that source.
+    
+    A company can have multiple data connections depending on the type of data source it is connecting to. For example, a single company can link to:
+    
+    - [Accounting data](https://docs.codat.io/accounting-api/overview) - 1 active connection.
+    - [Banking data](https://docs.codat.io/banking-api/overview) - Multiple active connections.
+    - [Commerce data](https://docs.codat.io/commerce-api/overview) - Multiple active connections.
+    Any combination of accounting, banking, and commerce data connections is allowed.
+    
+    Before you can use a data connection to pull or push data, the company must grant you access to their business data by [linking the connection](https://docs.codat.io/auth-flow/overview).
+    """
     created: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created') }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
```

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     type: ExpenseTransactionType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     r"""The type of transaction."""
     currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
     r"""Rate to convert the total amount of the payment into the base currency for the company at the time of the payment.
     
     Currency rates in Codat are implemented as the multiple of foreign currency units to each base currency unit.  
     
+    It is not possible to perform the currency conversion with two or more non-base currencies participating in the transaction. For example, if a company's base currency is USD, and it has a bill issued in EUR, then the bill payment must happen in USD or EUR.
+    
     Where the currency rate is provided by the underlying accounting platform, it will be available from Codat with the same precision (up to a maximum of 9 decimal places). 
     
     For accounting platforms which do not provide an explicit currency rate, it is calculated as `baseCurrency / foreignCurrency` and will be returned to 9 decimal places.
     
     ## Examples with base currency of GBP
     
     | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (GBP) |
```

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/postsync.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/postsync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/schema.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/syncinitiated.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/transactionmetadata.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/transactionmetadata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sdk.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/sdk.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sdkconfiguration.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/sdkconfiguration.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 class SDKConfiguration:
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     language: str = 'python'
     openapi_doc_version: str = 'prealpha'
-    sdk_version: str = '0.27.1'
-    gen_version: str = '2.41.1'
+    sdk_version: str = '0.33.1'
+    gen_version: str = '2.58.0'
 
     def get_server_details(self) -> tuple[str, dict[str, str]]:
         if self.server_url:
             return self.server_url.removesuffix('/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sync.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sync_status.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/sync_status.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-0.33.1/src/codatsyncexpenses/utils/utils.py`

 * *Files identical despite different names*

