# Comparing `tmp/MambuPy-2.0.0b8.tar.gz` & `tmp/MambuPy-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MambuPy-2.0.0b8.tar", last modified: Thu Aug  4 00:48:13 2022, max compression
+gzip compressed data, was "MambuPy-2.0.0b9.tar", last modified: Thu Aug  4 20:12:59 2022, max compression
```

## Comparing `MambuPy-2.0.0b8.tar` & `MambuPy-2.0.0b9.tar`

### file list

```diff
@@ -1,159 +1,158 @@
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.762422 MambuPy-2.0.0b8/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    35165 2022-03-09 20:14:27.000000 MambuPy-2.0.0b8/LICENSE
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.744423 MambuPy-2.0.0b8/MambuPy/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1110 2022-08-04 00:33:53.000000 MambuPy-2.0.0b8/MambuPy/__init__.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.747423 MambuPy-2.0.0b8/MambuPy/api/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      502 2022-05-17 00:45:24.000000 MambuPy-2.0.0b8/MambuPy/api/__init__.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     7758 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/api/classes.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.747423 MambuPy-2.0.0b8/MambuPy/api/connector/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)        0 2022-07-25 22:12:52.000000 MambuPy-2.0.0b8/MambuPy/api/connector/__init__.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     7007 2022-07-25 22:12:52.000000 MambuPy-2.0.0b8/MambuPy/api/connector/mambuconnector.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    23045 2022-08-03 22:51:01.000000 MambuPy-2.0.0b8/MambuPy/api/connector/rest.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    25885 2022-08-04 00:28:12.000000 MambuPy-2.0.0b8/MambuPy/api/entities.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4466 2022-08-03 22:51:21.000000 MambuPy-2.0.0b8/MambuPy/api/interfaces.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      771 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/MambuPy/api/mambubranch.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      789 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/MambuPy/api/mambucentre.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1742 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/MambuPy/api/mambuclient.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      323 2022-07-27 04:22:30.000000 MambuPy-2.0.0b8/MambuPy/api/mambucustomfield.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1541 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/MambuPy/api/mambugroup.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4665 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/MambuPy/api/mambuloan.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2893 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/MambuPy/api/mambuproduct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    24913 2022-08-01 16:06:01.000000 MambuPy-2.0.0b8/MambuPy/api/mambustruct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2485 2022-05-16 14:58:32.000000 MambuPy-2.0.0b8/MambuPy/api/mambutask.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1509 2022-04-07 04:16:33.000000 MambuPy-2.0.0b8/MambuPy/api/mambutransaction.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2808 2022-08-03 23:34:05.000000 MambuPy-2.0.0b8/MambuPy/api/mambuuser.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1101 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/MambuPy/api/vos.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     6575 2022-05-17 00:45:24.000000 MambuPy-2.0.0b8/MambuPy/mambuconfig.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    23291 2022-07-19 18:49:41.000000 MambuPy-2.0.0b8/MambuPy/mambugeturl.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    15791 2022-07-31 04:06:31.000000 MambuPy-2.0.0b8/MambuPy/mambuutil.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.752423 MambuPy-2.0.0b8/MambuPy/orm/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      801 2022-05-29 01:22:22.000000 MambuPy-2.0.0b8/MambuPy/orm/__init__.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3391 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_activities.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1598 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_addresses.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1814 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_branches.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1161 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_centres.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4956 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_clients.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     6279 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_customfields.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     6371 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_dummies.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3238 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_groups.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     8308 2022-06-13 16:55:01.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_loans.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1101 2022-03-10 00:09:27.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_mambu.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1477 2022-06-21 20:32:40.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_orm.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2314 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_tasks.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2754 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/MambuPy/orm/schema_users.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.754423 MambuPy-2.0.0b8/MambuPy/rest/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1746 2022-05-29 01:18:37.000000 MambuPy-2.0.0b8/MambuPy/rest/__init__.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2986 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mambuactivity.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3747 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mambubranch.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2850 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mambucentre.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    11142 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mambuclient.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    12541 2022-07-05 21:03:30.000000 MambuPy-2.0.0b8/MambuPy/rest/mambugroup.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    24417 2022-07-15 03:09:42.000000 MambuPy-2.0.0b8/MambuPy/rest/mambuloan.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     6795 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mambuproduct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3377 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mamburepayment.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3293 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mamburoles.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3671 2022-07-08 20:39:42.000000 MambuPy-2.0.0b8/MambuPy/rest/mambusaving.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3435 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mambusavingfundingrepayment.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     5686 2022-07-07 02:24:06.000000 MambuPy-2.0.0b8/MambuPy/rest/mambusavingtransaction.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    40745 2022-07-07 02:24:06.000000 MambuPy-2.0.0b8/MambuPy/rest/mambustruct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4707 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mambutask.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3621 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mambutransaction.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3393 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mambutransactionchannel.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     7483 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/MambuPy/rest/mambuuser.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.754423 MambuPy-2.0.0b8/MambuPy/rest1to2/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      460 2022-06-10 18:31:34.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/__init__.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2410 2022-07-14 00:20:18.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mambubranch.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1160 2022-07-09 00:23:09.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mambucentre.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4257 2022-07-14 00:20:18.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mambuclient.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3658 2022-07-09 00:23:09.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mambugroup.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     7305 2022-07-14 00:20:18.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mambuloan.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1103 2022-07-14 00:20:18.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mambuproduct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2964 2022-06-29 03:59:45.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mamburepayment.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    12061 2022-08-03 22:51:21.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mambustruct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2065 2022-07-09 00:39:42.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mambutask.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1465 2022-07-27 15:47:46.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mambutransaction.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2525 2022-07-09 00:23:09.000000 MambuPy-2.0.0b8/MambuPy/rest1to2/mambuuser.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.745423 MambuPy-2.0.0b8/MambuPy.egg-info/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1075 2022-08-04 00:48:13.000000 MambuPy-2.0.0b8/MambuPy.egg-info/PKG-INFO
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4087 2022-08-04 00:48:13.000000 MambuPy-2.0.0b8/MambuPy.egg-info/SOURCES.txt
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)        1 2022-08-04 00:48:13.000000 MambuPy-2.0.0b8/MambuPy.egg-info/dependency_links.txt
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)       79 2022-08-04 00:48:13.000000 MambuPy-2.0.0b8/MambuPy.egg-info/requires.txt
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      168 2022-08-04 00:48:13.000000 MambuPy-2.0.0b8/MambuPy.egg-info/top_level.txt
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1075 2022-08-04 00:48:13.761422 MambuPy-2.0.0b8/PKG-INFO
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      714 2022-05-09 02:48:54.000000 MambuPy-2.0.0b8/README.md
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.755423 MambuPy-2.0.0b8/mambupy/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1110 2022-08-04 00:33:53.000000 MambuPy-2.0.0b8/mambupy/__init__.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.756423 MambuPy-2.0.0b8/mambupy/api/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      502 2022-05-17 00:45:24.000000 MambuPy-2.0.0b8/mambupy/api/__init__.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     7758 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/api/classes.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.756423 MambuPy-2.0.0b8/mambupy/api/connector/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)        0 2022-07-25 22:12:52.000000 MambuPy-2.0.0b8/mambupy/api/connector/__init__.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     7007 2022-07-25 22:12:52.000000 MambuPy-2.0.0b8/mambupy/api/connector/mambuconnector.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    23045 2022-08-03 22:51:01.000000 MambuPy-2.0.0b8/mambupy/api/connector/rest.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    25885 2022-08-04 00:28:12.000000 MambuPy-2.0.0b8/mambupy/api/entities.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4466 2022-08-03 22:51:21.000000 MambuPy-2.0.0b8/mambupy/api/interfaces.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      771 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/mambupy/api/mambubranch.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      789 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/mambupy/api/mambucentre.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1742 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/mambupy/api/mambuclient.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      323 2022-07-27 04:22:30.000000 MambuPy-2.0.0b8/mambupy/api/mambucustomfield.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1541 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/mambupy/api/mambugroup.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4665 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/mambupy/api/mambuloan.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2893 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/mambupy/api/mambuproduct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    24913 2022-08-01 16:06:01.000000 MambuPy-2.0.0b8/mambupy/api/mambustruct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2485 2022-05-16 14:58:32.000000 MambuPy-2.0.0b8/mambupy/api/mambutask.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1509 2022-04-07 04:16:33.000000 MambuPy-2.0.0b8/mambupy/api/mambutransaction.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2808 2022-08-03 23:34:05.000000 MambuPy-2.0.0b8/mambupy/api/mambuuser.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1101 2022-07-21 20:36:26.000000 MambuPy-2.0.0b8/mambupy/api/vos.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     6575 2022-05-17 00:45:24.000000 MambuPy-2.0.0b8/mambupy/mambuconfig.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    23291 2022-07-19 18:49:41.000000 MambuPy-2.0.0b8/mambupy/mambugeturl.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    15791 2022-07-31 04:06:31.000000 MambuPy-2.0.0b8/mambupy/mambuutil.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.759423 MambuPy-2.0.0b8/mambupy/orm/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      801 2022-05-29 01:22:22.000000 MambuPy-2.0.0b8/mambupy/orm/__init__.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3391 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/orm/schema_activities.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1598 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/orm/schema_addresses.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1814 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/orm/schema_branches.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1161 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/orm/schema_centres.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4956 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/orm/schema_clients.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     6279 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/orm/schema_customfields.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     6371 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/orm/schema_dummies.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3238 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/orm/schema_groups.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     8308 2022-06-13 16:55:01.000000 MambuPy-2.0.0b8/mambupy/orm/schema_loans.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1101 2022-03-10 00:09:27.000000 MambuPy-2.0.0b8/mambupy/orm/schema_mambu.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1477 2022-06-21 20:32:40.000000 MambuPy-2.0.0b8/mambupy/orm/schema_orm.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2314 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/orm/schema_tasks.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2754 2022-03-15 21:43:58.000000 MambuPy-2.0.0b8/mambupy/orm/schema_users.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.760423 MambuPy-2.0.0b8/mambupy/rest/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1746 2022-05-29 01:18:37.000000 MambuPy-2.0.0b8/mambupy/rest/__init__.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2986 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mambuactivity.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3747 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mambubranch.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2850 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mambucentre.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    11142 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mambuclient.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    12541 2022-07-05 21:03:30.000000 MambuPy-2.0.0b8/mambupy/rest/mambugroup.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    24417 2022-07-15 03:09:42.000000 MambuPy-2.0.0b8/mambupy/rest/mambuloan.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     6795 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mambuproduct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3377 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mamburepayment.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3293 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mamburoles.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3671 2022-07-08 20:39:42.000000 MambuPy-2.0.0b8/mambupy/rest/mambusaving.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3435 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mambusavingfundingrepayment.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     5686 2022-07-07 02:24:06.000000 MambuPy-2.0.0b8/mambupy/rest/mambusavingtransaction.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    40745 2022-07-07 02:24:06.000000 MambuPy-2.0.0b8/mambupy/rest/mambustruct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4707 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mambutask.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3621 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mambutransaction.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3393 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mambutransactionchannel.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     7483 2022-07-05 14:39:40.000000 MambuPy-2.0.0b8/mambupy/rest/mambuuser.py
-drwxr-xr-x   0 jstitch   (1000) jstitch   (1000)        0 2022-08-04 00:48:13.761422 MambuPy-2.0.0b8/mambupy/rest1to2/
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)      460 2022-06-10 18:31:34.000000 MambuPy-2.0.0b8/mambupy/rest1to2/__init__.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2410 2022-07-14 00:20:18.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mambubranch.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1160 2022-07-09 00:23:09.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mambucentre.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     4257 2022-07-14 00:20:18.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mambuclient.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     3658 2022-07-09 00:23:09.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mambugroup.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     7305 2022-07-14 00:20:18.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mambuloan.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1103 2022-07-14 00:20:18.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mambuproduct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2964 2022-06-29 03:59:45.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mamburepayment.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)    12061 2022-08-03 22:51:21.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mambustruct.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2065 2022-07-09 00:39:42.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mambutask.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1465 2022-07-27 15:47:46.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mambutransaction.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     2525 2022-07-09 00:23:09.000000 MambuPy-2.0.0b8/mambupy/rest1to2/mambuuser.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)       38 2022-08-04 00:48:13.762422 MambuPy-2.0.0b8/setup.cfg
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1999 2022-07-26 00:37:33.000000 MambuPy-2.0.0b8/setup.py
--rw-r--r--   0 jstitch   (1000) jstitch   (1000)     1566 2022-05-30 02:45:14.000000 MambuPy-2.0.0b8/setup_nosql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.327387 MambuPy-2.0.0b9/
+-rw-rw-rw-   0 root         (0) root         (0)    35165 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.285218 MambuPy-2.0.0b9/MambuPy/
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.290718 MambuPy-2.0.0b9/MambuPy/api/
+-rw-rw-rw-   0 root         (0) root         (0)      502 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7758 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.291635 MambuPy-2.0.0b9/MambuPy/api/connector/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/connector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7007 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/connector/mambuconnector.py
+-rw-rw-rw-   0 root         (0) root         (0)    23045 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/connector/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)    25885 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     4430 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambubranch.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambucentre.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambuclient.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambucustomfield.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambugroup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambuloan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambuproduct.py
+-rw-rw-rw-   0 root         (0) root         (0)    24913 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambustruct.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambutask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambutransaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/mambuuser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/api/vos.py
+-rw-rw-rw-   0 root         (0) root         (0)     6575 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/mambuconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    23291 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/mambugeturl.py
+-rw-rw-rw-   0 root         (0) root         (0)    15791 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/mambuutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.296219 MambuPy-2.0.0b9/MambuPy/orm/
+-rw-rw-rw-   0 root         (0) root         (0)      801 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_activities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_addresses.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_branches.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_centres.py
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_clients.py
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_customfields.py
+-rw-rw-rw-   0 root         (0) root         (0)     6371 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_dummies.py
+-rw-rw-rw-   0 root         (0) root         (0)     3238 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     8308 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_loans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_mambu.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_orm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/orm/schema_users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.301719 MambuPy-2.0.0b9/MambuPy/rest/
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambuactivity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3747 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambubranch.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambucentre.py
+-rw-rw-rw-   0 root         (0) root         (0)    11142 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambuclient.py
+-rw-rw-rw-   0 root         (0) root         (0)    12541 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambugroup.py
+-rw-rw-rw-   0 root         (0) root         (0)    24417 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambuloan.py
+-rw-rw-rw-   0 root         (0) root         (0)     6795 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambuproduct.py
+-rw-rw-rw-   0 root         (0) root         (0)     3377 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mamburepayment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mamburoles.py
+-rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambusaving.py
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambusavingfundingrepayment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5686 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambusavingtransaction.py
+-rw-rw-rw-   0 root         (0) root         (0)    40745 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambustruct.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambutask.py
+-rw-rw-rw-   0 root         (0) root         (0)     3621 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambutransaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3393 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambutransactionchannel.py
+-rw-rw-rw-   0 root         (0) root         (0)     7483 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest/mambuuser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.305386 MambuPy-2.0.0b9/MambuPy/rest1to2/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mambubranch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mambucentre.py
+-rw-rw-rw-   0 root         (0) root         (0)     4257 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mambuclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3658 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mambugroup.py
+-rw-rw-rw-   0 root         (0) root         (0)     7305 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mambuloan.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mambuproduct.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mamburepayment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11868 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mambustruct.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mambutask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mambutransaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2525 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/MambuPy/rest1to2/mambuuser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.286135 MambuPy-2.0.0b9/MambuPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1030 2022-08-04 20:12:59.000000 MambuPy-2.0.0b9/MambuPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4072 2022-08-04 20:12:59.000000 MambuPy-2.0.0b9/MambuPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-04 20:12:59.000000 MambuPy-2.0.0b9/MambuPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2022-08-04 20:12:59.000000 MambuPy-2.0.0b9/MambuPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2022-08-04 20:12:59.000000 MambuPy-2.0.0b9/MambuPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1030 2022-08-04 20:12:59.325554 MambuPy-2.0.0b9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      714 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.307219 MambuPy-2.0.0b9/mambupy/
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.310886 MambuPy-2.0.0b9/mambupy/api/
+-rw-rw-rw-   0 root         (0) root         (0)      502 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7758 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.311803 MambuPy-2.0.0b9/mambupy/api/connector/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/connector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7007 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/connector/mambuconnector.py
+-rw-rw-rw-   0 root         (0) root         (0)    23045 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/connector/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)    25885 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     4430 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambubranch.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambucentre.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambuclient.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambucustomfield.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambugroup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambuloan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambuproduct.py
+-rw-rw-rw-   0 root         (0) root         (0)    24913 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambustruct.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambutask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambutransaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/mambuuser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/api/vos.py
+-rw-rw-rw-   0 root         (0) root         (0)     6575 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/mambuconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    23291 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/mambugeturl.py
+-rw-rw-rw-   0 root         (0) root         (0)    15791 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/mambuutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.317303 MambuPy-2.0.0b9/mambupy/orm/
+-rw-rw-rw-   0 root         (0) root         (0)      801 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_activities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_addresses.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_branches.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_centres.py
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_clients.py
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_customfields.py
+-rw-rw-rw-   0 root         (0) root         (0)     6371 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_dummies.py
+-rw-rw-rw-   0 root         (0) root         (0)     3238 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     8308 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_loans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_mambu.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_orm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/orm/schema_users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.321887 MambuPy-2.0.0b9/mambupy/rest/
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambuactivity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3747 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambubranch.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambucentre.py
+-rw-rw-rw-   0 root         (0) root         (0)    11142 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambuclient.py
+-rw-rw-rw-   0 root         (0) root         (0)    12541 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambugroup.py
+-rw-rw-rw-   0 root         (0) root         (0)    24417 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambuloan.py
+-rw-rw-rw-   0 root         (0) root         (0)     6795 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambuproduct.py
+-rw-rw-rw-   0 root         (0) root         (0)     3377 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mamburepayment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mamburoles.py
+-rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambusaving.py
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambusavingfundingrepayment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5686 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambusavingtransaction.py
+-rw-rw-rw-   0 root         (0) root         (0)    40745 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambustruct.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambutask.py
+-rw-rw-rw-   0 root         (0) root         (0)     3621 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambutransaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3393 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambutransactionchannel.py
+-rw-rw-rw-   0 root         (0) root         (0)     7483 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest/mambuuser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-04 20:12:59.325554 MambuPy-2.0.0b9/mambupy/rest1to2/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mambubranch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mambucentre.py
+-rw-rw-rw-   0 root         (0) root         (0)     4257 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mambuclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3658 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mambugroup.py
+-rw-rw-rw-   0 root         (0) root         (0)     7305 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mambuloan.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mambuproduct.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mamburepayment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11868 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mambustruct.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mambutask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mambutransaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2525 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/mambupy/rest1to2/mambuuser.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-04 20:12:59.327387 MambuPy-2.0.0b9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2022-08-04 20:12:47.000000 MambuPy-2.0.0b9/setup.py
```

### Comparing `MambuPy-2.0.0b8/LICENSE` & `MambuPy-2.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/__init__.py` & `MambuPy-2.0.0b9/MambuPy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 TODOS
 =====
 
 .. todo:: Unit testing of some modules is currently very basic. The purpose is
           to achive TDD when implementing features or correcting bugs.
 """
 
-__version__ = "2.0.0b8"
+__version__ = "2.0.0b9"
 """The version of this module."""
```

### Comparing `MambuPy-2.0.0b8/MambuPy/api/classes.py` & `MambuPy-2.0.0b9/MambuPy/api/classes.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/connector/mambuconnector.py` & `MambuPy-2.0.0b9/MambuPy/api/connector/mambuconnector.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/connector/rest.py` & `MambuPy-2.0.0b9/MambuPy/api/connector/rest.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/entities.py` & `MambuPy-2.0.0b9/MambuPy/api/entities.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/interfaces.py` & `MambuPy-2.0.0b9/MambuPy/api/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,13 +134,9 @@
         raise NotImplementedError
 
 
 class MambuOwner(ABC):
     """"""
 
 
-class MambuOwned(ABC):
-    """"""
-
-
 class MambuHolder(ABC):
     """"""
```

### Comparing `MambuPy-2.0.0b8/MambuPy/api/mambubranch.py` & `MambuPy-2.0.0b9/MambuPy/api/mambubranch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """MambuBranch entity: a MambuEntity struct for Branches.
 
 .. autosummary::
    :nosignatures:
    :toctree: _autosummary
 """
 
-from .entities import MambuEntity
-from .interfaces import MambuOwner, MambuCommentable
+from .entities import MambuEntity, MambuEntityCommentable
+from .interfaces import MambuOwner
 
 
-class MambuBranch(MambuEntity, MambuCommentable, MambuOwner):
+class MambuBranch(MambuEntity, MambuEntityCommentable, MambuOwner):
     """MambuBranch entity"""
 
     _prefix = "branches"
     """prefix constant for connections to Mambu"""
 
     _filter_keys = [
     ]
```

### Comparing `MambuPy-2.0.0b8/MambuPy/api/mambucentre.py` & `MambuPy-2.0.0b9/MambuPy/api/mambucentre.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """MambuCentre entity: a MambuEntity struct for Centres.
 
 .. autosummary::
    :nosignatures:
    :toctree: _autosummary
 """
 
-from .entities import MambuEntity
-from .interfaces import MambuOwner, MambuCommentable
+from .entities import MambuEntity, MambuEntityCommentable
+from .interfaces import MambuOwner
 
 
-class MambuCentre(MambuEntity, MambuCommentable, MambuOwner):
+class MambuCentre(MambuEntity, MambuEntityCommentable, MambuOwner):
     """MambuCentre entity"""
 
     _prefix = "centres"
     """prefix constant for connections to Mambu"""
 
     _filter_keys = [
         "branchId",
```

### Comparing `MambuPy-2.0.0b8/MambuPy/api/mambuclient.py` & `MambuPy-2.0.0b9/MambuPy/api/mambuclient.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/mambugroup.py` & `MambuPy-2.0.0b9/MambuPy/api/mambugroup.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/mambuloan.py` & `MambuPy-2.0.0b9/MambuPy/api/mambuloan.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/mambuproduct.py` & `MambuPy-2.0.0b9/MambuPy/api/mambuproduct.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/mambustruct.py` & `MambuPy-2.0.0b9/MambuPy/api/mambustruct.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/mambutask.py` & `MambuPy-2.0.0b9/MambuPy/api/mambutask.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/mambutransaction.py` & `MambuPy-2.0.0b9/MambuPy/api/mambutransaction.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/mambuuser.py` & `MambuPy-2.0.0b9/MambuPy/api/mambuuser.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/api/vos.py` & `MambuPy-2.0.0b9/MambuPy/api/vos.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/mambuconfig.py` & `MambuPy-2.0.0b9/MambuPy/mambuconfig.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/mambugeturl.py` & `MambuPy-2.0.0b9/MambuPy/mambugeturl.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/mambuutil.py` & `MambuPy-2.0.0b9/MambuPy/mambuutil.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/__init__.py` & `MambuPy-2.0.0b9/MambuPy/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_activities.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_activities.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_addresses.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_addresses.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_branches.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_branches.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_centres.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_centres.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_clients.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_clients.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_customfields.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_customfields.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_dummies.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_dummies.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_groups.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_groups.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_loans.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_loans.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_mambu.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_mambu.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_orm.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_orm.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_tasks.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_tasks.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/orm/schema_users.py` & `MambuPy-2.0.0b9/MambuPy/orm/schema_users.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/__init__.py` & `MambuPy-2.0.0b9/MambuPy/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambuactivity.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambuactivity.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambubranch.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambubranch.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambucentre.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambucentre.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambuclient.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambuclient.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambugroup.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambugroup.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambuloan.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambuloan.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambuproduct.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambuproduct.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mamburepayment.py` & `MambuPy-2.0.0b9/MambuPy/rest/mamburepayment.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mamburoles.py` & `MambuPy-2.0.0b9/MambuPy/rest/mamburoles.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambusaving.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambusaving.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambusavingfundingrepayment.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambusavingfundingrepayment.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambusavingtransaction.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambusavingtransaction.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambustruct.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambustruct.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambutask.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambutask.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambutransaction.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambutransaction.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambutransactionchannel.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambutransactionchannel.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest/mambuuser.py` & `MambuPy-2.0.0b9/MambuPy/rest/mambuuser.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mambubranch.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mambubranch.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mambucentre.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mambucentre.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mambuclient.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mambuclient.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mambugroup.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mambugroup.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mambuloan.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mambuloan.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mambuproduct.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mambuproduct.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mamburepayment.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mamburepayment.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mambustruct.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mambustruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,17 +119,14 @@
             except AttributeError:
                 try:
                     return self.DEFAULTS[name]
                 except KeyError:
                     if (not self.wrapped1 and
                         self._entid and self._entid != "" and
                         name not in [
-                            "_ipython_canary_method_should_not_exist_",
-                            "_ipython_canary_method_should_not_exist_",
-                            "_repr_mimebundle_",
                             "__getstate__"]):
                         _class_base = import_class(
                             "MambuPy.rest", self.mambuclassname)
                         _class = self.mambuclass1
                         print("setting wrapped1 of {} for prop {}".format(repr(self), name))
                         self.wrapped1 = _class(
                             fullDetails=self.fullDetails, entid=self._entid,
```

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mambutask.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mambutask.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mambutransaction.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mambutransaction.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy/rest1to2/mambuuser.py` & `MambuPy-2.0.0b9/MambuPy/rest1to2/mambuuser.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/MambuPy.egg-info/PKG-INFO` & `MambuPy-2.0.0b9/MambuPy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: MambuPy
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: A python lib for using Mambu APIs.
 Home-page: https://mambupydocs.readthedocs.io
 Author: Javier Novoa C.
 Author-email: jstitch@gmail.com
 License: GPLv3
 Keywords: mambu
-Platform: UNKNOWN
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 MambuPy
 =======
 
-
-.. image:: https://travis-ci.org/jstitch/MambuPy.svg?branch=master
-   :target: https://travis-ci.org/jstitch/MambuPy
-   :alt: Build Status
+[![Build Status](https://travis-ci.org/jstitch/MambuPy.svg?branch=master)](https://travis-ci.org/jstitch/MambuPy)
 
 
 A python API for using Mambu.
 -----------------------------
 
 Allows accessing Mambu programatically.
 
@@ -32,21 +27,21 @@
 
 Mambu is a cloud platform which lets you rapidly build, integrate,
 launch and service any lending portfolio into any market
 (https://www.mambu.com).
 
 Official documentation is found at https://mambupydocs.readthedocs.io
 
+
 More Information
 ----------------
 
 You can look at tha CHANGELOG for release notes.
 
 MambuPy is licensed under GPLv3, LICENSE has more details.
 
+
 Author
 ------
 
 JNC
 jstitch@gmail.com
-
-
```

### Comparing `MambuPy-2.0.0b8/MambuPy.egg-info/SOURCES.txt` & `MambuPy-2.0.0b9/MambuPy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 setup.py
-setup_nosql.py
 MambuPy/__init__.py
 MambuPy/mambuconfig.py
 MambuPy/mambugeturl.py
 MambuPy/mambuutil.py
 MambuPy.egg-info/PKG-INFO
 MambuPy.egg-info/SOURCES.txt
 MambuPy.egg-info/dependency_links.txt
```

### Comparing `MambuPy-2.0.0b8/PKG-INFO` & `MambuPy-2.0.0b9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: MambuPy
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: A python lib for using Mambu APIs.
 Home-page: https://mambupydocs.readthedocs.io
 Author: Javier Novoa C.
 Author-email: jstitch@gmail.com
 License: GPLv3
 Keywords: mambu
-Platform: UNKNOWN
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 MambuPy
 =======
 
-
-.. image:: https://travis-ci.org/jstitch/MambuPy.svg?branch=master
-   :target: https://travis-ci.org/jstitch/MambuPy
-   :alt: Build Status
+[![Build Status](https://travis-ci.org/jstitch/MambuPy.svg?branch=master)](https://travis-ci.org/jstitch/MambuPy)
 
 
 A python API for using Mambu.
 -----------------------------
 
 Allows accessing Mambu programatically.
 
@@ -32,21 +27,21 @@
 
 Mambu is a cloud platform which lets you rapidly build, integrate,
 launch and service any lending portfolio into any market
 (https://www.mambu.com).
 
 Official documentation is found at https://mambupydocs.readthedocs.io
 
+
 More Information
 ----------------
 
 You can look at tha CHANGELOG for release notes.
 
 MambuPy is licensed under GPLv3, LICENSE has more details.
 
+
 Author
 ------
 
 JNC
 jstitch@gmail.com
-
-
```

### Comparing `MambuPy-2.0.0b8/README.md` & `MambuPy-2.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/__init__.py` & `MambuPy-2.0.0b9/mambupy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 TODOS
 =====
 
 .. todo:: Unit testing of some modules is currently very basic. The purpose is
           to achive TDD when implementing features or correcting bugs.
 """
 
-__version__ = "2.0.0b8"
+__version__ = "2.0.0b9"
 """The version of this module."""
```

### Comparing `MambuPy-2.0.0b8/mambupy/api/classes.py` & `MambuPy-2.0.0b9/mambupy/api/classes.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/connector/mambuconnector.py` & `MambuPy-2.0.0b9/mambupy/api/connector/mambuconnector.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/connector/rest.py` & `MambuPy-2.0.0b9/mambupy/api/connector/rest.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/entities.py` & `MambuPy-2.0.0b9/mambupy/api/entities.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/interfaces.py` & `MambuPy-2.0.0b9/mambupy/api/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,13 +134,9 @@
         raise NotImplementedError
 
 
 class MambuOwner(ABC):
     """"""
 
 
-class MambuOwned(ABC):
-    """"""
-
-
 class MambuHolder(ABC):
     """"""
```

### Comparing `MambuPy-2.0.0b8/mambupy/api/mambubranch.py` & `MambuPy-2.0.0b9/mambupy/api/mambubranch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """MambuBranch entity: a MambuEntity struct for Branches.
 
 .. autosummary::
    :nosignatures:
    :toctree: _autosummary
 """
 
-from .entities import MambuEntity
-from .interfaces import MambuOwner, MambuCommentable
+from .entities import MambuEntity, MambuEntityCommentable
+from .interfaces import MambuOwner
 
 
-class MambuBranch(MambuEntity, MambuCommentable, MambuOwner):
+class MambuBranch(MambuEntity, MambuEntityCommentable, MambuOwner):
     """MambuBranch entity"""
 
     _prefix = "branches"
     """prefix constant for connections to Mambu"""
 
     _filter_keys = [
     ]
```

### Comparing `MambuPy-2.0.0b8/mambupy/api/mambucentre.py` & `MambuPy-2.0.0b9/mambupy/api/mambucentre.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """MambuCentre entity: a MambuEntity struct for Centres.
 
 .. autosummary::
    :nosignatures:
    :toctree: _autosummary
 """
 
-from .entities import MambuEntity
-from .interfaces import MambuOwner, MambuCommentable
+from .entities import MambuEntity, MambuEntityCommentable
+from .interfaces import MambuOwner
 
 
-class MambuCentre(MambuEntity, MambuCommentable, MambuOwner):
+class MambuCentre(MambuEntity, MambuEntityCommentable, MambuOwner):
     """MambuCentre entity"""
 
     _prefix = "centres"
     """prefix constant for connections to Mambu"""
 
     _filter_keys = [
         "branchId",
```

### Comparing `MambuPy-2.0.0b8/mambupy/api/mambuclient.py` & `MambuPy-2.0.0b9/mambupy/api/mambuclient.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/mambugroup.py` & `MambuPy-2.0.0b9/mambupy/api/mambugroup.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/mambuloan.py` & `MambuPy-2.0.0b9/mambupy/api/mambuloan.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/mambuproduct.py` & `MambuPy-2.0.0b9/mambupy/api/mambuproduct.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/mambustruct.py` & `MambuPy-2.0.0b9/mambupy/api/mambustruct.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/mambutask.py` & `MambuPy-2.0.0b9/mambupy/api/mambutask.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/mambutransaction.py` & `MambuPy-2.0.0b9/mambupy/api/mambutransaction.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/mambuuser.py` & `MambuPy-2.0.0b9/mambupy/api/mambuuser.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/api/vos.py` & `MambuPy-2.0.0b9/mambupy/api/vos.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/mambuconfig.py` & `MambuPy-2.0.0b9/mambupy/mambuconfig.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/mambugeturl.py` & `MambuPy-2.0.0b9/mambupy/mambugeturl.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/mambuutil.py` & `MambuPy-2.0.0b9/mambupy/mambuutil.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/__init__.py` & `MambuPy-2.0.0b9/mambupy/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_activities.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_activities.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_addresses.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_addresses.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_branches.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_branches.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_centres.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_centres.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_clients.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_clients.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_customfields.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_customfields.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_dummies.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_dummies.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_groups.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_groups.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_loans.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_loans.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_mambu.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_mambu.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_orm.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_orm.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_tasks.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_tasks.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/orm/schema_users.py` & `MambuPy-2.0.0b9/mambupy/orm/schema_users.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/__init__.py` & `MambuPy-2.0.0b9/mambupy/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambuactivity.py` & `MambuPy-2.0.0b9/mambupy/rest/mambuactivity.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambubranch.py` & `MambuPy-2.0.0b9/mambupy/rest/mambubranch.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambucentre.py` & `MambuPy-2.0.0b9/mambupy/rest/mambucentre.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambuclient.py` & `MambuPy-2.0.0b9/mambupy/rest/mambuclient.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambugroup.py` & `MambuPy-2.0.0b9/mambupy/rest/mambugroup.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambuloan.py` & `MambuPy-2.0.0b9/mambupy/rest/mambuloan.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambuproduct.py` & `MambuPy-2.0.0b9/mambupy/rest/mambuproduct.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mamburepayment.py` & `MambuPy-2.0.0b9/mambupy/rest/mamburepayment.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mamburoles.py` & `MambuPy-2.0.0b9/mambupy/rest/mamburoles.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambusaving.py` & `MambuPy-2.0.0b9/mambupy/rest/mambusaving.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambusavingfundingrepayment.py` & `MambuPy-2.0.0b9/mambupy/rest/mambusavingfundingrepayment.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambusavingtransaction.py` & `MambuPy-2.0.0b9/mambupy/rest/mambusavingtransaction.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambustruct.py` & `MambuPy-2.0.0b9/mambupy/rest/mambustruct.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambutask.py` & `MambuPy-2.0.0b9/mambupy/rest/mambutask.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambutransaction.py` & `MambuPy-2.0.0b9/mambupy/rest/mambutransaction.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambutransactionchannel.py` & `MambuPy-2.0.0b9/mambupy/rest/mambutransactionchannel.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest/mambuuser.py` & `MambuPy-2.0.0b9/mambupy/rest/mambuuser.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mambubranch.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mambubranch.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mambucentre.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mambucentre.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mambuclient.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mambuclient.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mambugroup.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mambugroup.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mambuloan.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mambuloan.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mambuproduct.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mambuproduct.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mamburepayment.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mamburepayment.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mambustruct.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mambustruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,17 +119,14 @@
             except AttributeError:
                 try:
                     return self.DEFAULTS[name]
                 except KeyError:
                     if (not self.wrapped1 and
                         self._entid and self._entid != "" and
                         name not in [
-                            "_ipython_canary_method_should_not_exist_",
-                            "_ipython_canary_method_should_not_exist_",
-                            "_repr_mimebundle_",
                             "__getstate__"]):
                         _class_base = import_class(
                             "MambuPy.rest", self.mambuclassname)
                         _class = self.mambuclass1
                         print("setting wrapped1 of {} for prop {}".format(repr(self), name))
                         self.wrapped1 = _class(
                             fullDetails=self.fullDetails, entid=self._entid,
```

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mambutask.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mambutask.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mambutransaction.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mambutransaction.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/mambupy/rest1to2/mambuuser.py` & `MambuPy-2.0.0b9/mambupy/rest1to2/mambuuser.py`

 * *Files identical despite different names*

### Comparing `MambuPy-2.0.0b8/setup.py` & `MambuPy-2.0.0b9/setup.py`

 * *Files identical despite different names*

